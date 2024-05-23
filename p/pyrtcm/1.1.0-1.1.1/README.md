# Comparing `tmp/pyrtcm-1.1.0.tar.gz` & `tmp/pyrtcm-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrtcm-1.1.0.tar", last modified: Thu May 16 08:57:22 2024, max compression
+gzip compressed data, was "pyrtcm-1.1.1.tar", last modified: Thu May 23 12:21:45 2024, max compression
```

## Comparing `pyrtcm-1.1.0.tar` & `pyrtcm-1.1.1.tar`

### file list

```diff
@@ -1,30 +1,32 @@
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-05-16 08:57:22.851837 pyrtcm-1.1.0/
--rw-r--r--   0 steve      (501) staff       (20)     1613 2024-04-10 08:11:47.000000 pyrtcm-1.1.0/LICENSE
--rw-r--r--   0 steve      (501) staff       (20)       64 2024-04-10 08:11:47.000000 pyrtcm-1.1.0/MANIFEST.in
--rw-r--r--   0 steve      (501) staff       (20)    17908 2024-05-16 08:57:22.851451 pyrtcm-1.1.0/PKG-INFO
--rw-r--r--   0 steve      (501) staff       (20)    14397 2024-05-16 08:53:31.000000 pyrtcm-1.1.0/README.md
--rw-r--r--   0 steve      (501) staff       (20)     2426 2024-05-16 08:53:31.000000 pyrtcm-1.1.0/pyproject.toml
--rw-r--r--   0 steve      (501) staff       (20)       38 2024-05-16 08:57:22.851888 pyrtcm-1.1.0/setup.cfg
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-05-16 08:57:22.845620 pyrtcm-1.1.0/src/
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-05-16 08:57:22.848469 pyrtcm-1.1.0/src/pyrtcm/
--rw-r--r--   0 steve      (501) staff       (20)      600 2024-04-10 08:11:47.000000 pyrtcm-1.1.0/src/pyrtcm/__init__.py
--rw-r--r--   0 steve      (501) staff       (20)      162 2024-05-16 08:53:31.000000 pyrtcm-1.1.0/src/pyrtcm/_version.py
--rw-r--r--   0 steve      (501) staff       (20)      734 2024-04-10 08:11:47.000000 pyrtcm-1.1.0/src/pyrtcm/exceptions.py
--rw-r--r--   0 steve      (501) staff       (20)     8961 2024-05-16 08:53:31.000000 pyrtcm-1.1.0/src/pyrtcm/rtcmhelpers.py
--rw-r--r--   0 steve      (501) staff       (20)    14502 2024-05-16 08:53:31.000000 pyrtcm-1.1.0/src/pyrtcm/rtcmmessage.py
--rw-r--r--   0 steve      (501) staff       (20)     9459 2024-05-16 08:53:31.000000 pyrtcm-1.1.0/src/pyrtcm/rtcmreader.py
--rw-r--r--   0 steve      (501) staff       (20)     3564 2024-05-16 08:53:31.000000 pyrtcm-1.1.0/src/pyrtcm/rtcmtables.py
--rw-r--r--   0 steve      (501) staff       (20)    41265 2024-05-16 08:53:31.000000 pyrtcm-1.1.0/src/pyrtcm/rtcmtypes_core.py
--rw-r--r--   0 steve      (501) staff       (20)    65495 2024-05-16 08:53:31.000000 pyrtcm-1.1.0/src/pyrtcm/rtcmtypes_get.py
--rw-r--r--   0 steve      (501) staff       (20)     2508 2024-04-10 08:11:47.000000 pyrtcm-1.1.0/src/pyrtcm/socket_stream.py
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-05-16 08:57:22.850456 pyrtcm-1.1.0/src/pyrtcm.egg-info/
--rw-r--r--   0 steve      (501) staff       (20)    17908 2024-05-16 08:57:22.000000 pyrtcm-1.1.0/src/pyrtcm.egg-info/PKG-INFO
--rw-r--r--   0 steve      (501) staff       (20)      560 2024-05-16 08:57:22.000000 pyrtcm-1.1.0/src/pyrtcm.egg-info/SOURCES.txt
--rw-r--r--   0 steve      (501) staff       (20)        1 2024-05-16 08:57:22.000000 pyrtcm-1.1.0/src/pyrtcm.egg-info/dependency_links.txt
--rw-r--r--   0 steve      (501) staff       (20)      113 2024-05-16 08:57:22.000000 pyrtcm-1.1.0/src/pyrtcm.egg-info/requires.txt
--rw-r--r--   0 steve      (501) staff       (20)        7 2024-05-16 08:57:22.000000 pyrtcm-1.1.0/src/pyrtcm.egg-info/top_level.txt
-drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-05-16 08:57:22.850023 pyrtcm-1.1.0/tests/
--rw-r--r--   0 steve      (501) staff       (20)     1008 2024-05-08 07:05:03.000000 pyrtcm-1.1.0/tests/test_definitions.py
--rw-r--r--   0 steve      (501) staff       (20)     6032 2024-04-10 08:11:47.000000 pyrtcm-1.1.0/tests/test_socket.py
--rw-r--r--   0 steve      (501) staff       (20)    24603 2024-05-16 08:53:31.000000 pyrtcm-1.1.0/tests/test_static.py
--rw-r--r--   0 steve      (501) staff       (20)   195338 2024-05-16 08:53:31.000000 pyrtcm-1.1.0/tests/test_stream.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-05-23 12:21:45.575170 pyrtcm-1.1.1/
+-rw-r--r--   0 steve      (501) staff       (20)     1613 2024-04-10 08:11:47.000000 pyrtcm-1.1.1/LICENSE
+-rw-r--r--   0 steve      (501) staff       (20)       64 2024-04-10 08:11:47.000000 pyrtcm-1.1.1/MANIFEST.in
+-rw-r--r--   0 steve      (501) staff       (20)    17862 2024-05-23 12:21:45.574812 pyrtcm-1.1.1/PKG-INFO
+-rw-r--r--   0 steve      (501) staff       (20)    14348 2024-05-23 12:21:11.000000 pyrtcm-1.1.1/README.md
+-rw-r--r--   0 steve      (501) staff       (20)     2426 2024-05-23 12:21:11.000000 pyrtcm-1.1.1/pyproject.toml
+-rw-r--r--   0 steve      (501) staff       (20)       38 2024-05-23 12:21:45.575235 pyrtcm-1.1.1/setup.cfg
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-05-23 12:21:45.568197 pyrtcm-1.1.1/src/
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-05-23 12:21:45.570621 pyrtcm-1.1.1/src/pyrtcm/
+-rw-r--r--   0 steve      (501) staff       (20)      680 2024-05-23 12:21:11.000000 pyrtcm-1.1.1/src/pyrtcm/__init__.py
+-rw-r--r--   0 steve      (501) staff       (20)      162 2024-05-23 12:21:11.000000 pyrtcm-1.1.1/src/pyrtcm/_version.py
+-rw-r--r--   0 steve      (501) staff       (20)      734 2024-04-10 08:11:47.000000 pyrtcm-1.1.1/src/pyrtcm/exceptions.py
+-rw-r--r--   0 steve      (501) staff       (20)     7090 2024-05-23 12:21:11.000000 pyrtcm-1.1.1/src/pyrtcm/rtcmhelpers.py
+-rw-r--r--   0 steve      (501) staff       (20)    14631 2024-05-23 12:21:11.000000 pyrtcm-1.1.1/src/pyrtcm/rtcmmessage.py
+-rw-r--r--   0 steve      (501) staff       (20)     9962 2024-05-23 12:21:11.000000 pyrtcm-1.1.1/src/pyrtcm/rtcmreader.py
+-rw-r--r--   0 steve      (501) staff       (20)     3564 2024-05-16 08:53:31.000000 pyrtcm-1.1.1/src/pyrtcm/rtcmtables.py
+-rw-r--r--   0 steve      (501) staff       (20)    39334 2024-05-23 12:21:11.000000 pyrtcm-1.1.1/src/pyrtcm/rtcmtypes_core.py
+-rw-r--r--   0 steve      (501) staff       (20)    41818 2024-05-23 12:21:11.000000 pyrtcm-1.1.1/src/pyrtcm/rtcmtypes_get.py
+-rw-r--r--   0 steve      (501) staff       (20)     8357 2024-05-23 12:21:11.000000 pyrtcm-1.1.1/src/pyrtcm/rtcmtypes_get_igs.py
+-rw-r--r--   0 steve      (501) staff       (20)    16094 2024-05-23 12:21:11.000000 pyrtcm-1.1.1/src/pyrtcm/rtcmtypes_get_msm.py
+-rw-r--r--   0 steve      (501) staff       (20)     2508 2024-04-10 08:11:47.000000 pyrtcm-1.1.1/src/pyrtcm/socket_stream.py
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-05-23 12:21:45.573881 pyrtcm-1.1.1/src/pyrtcm.egg-info/
+-rw-r--r--   0 steve      (501) staff       (20)    17862 2024-05-23 12:21:45.000000 pyrtcm-1.1.1/src/pyrtcm.egg-info/PKG-INFO
+-rw-r--r--   0 steve      (501) staff       (20)      624 2024-05-23 12:21:45.000000 pyrtcm-1.1.1/src/pyrtcm.egg-info/SOURCES.txt
+-rw-r--r--   0 steve      (501) staff       (20)        1 2024-05-23 12:21:45.000000 pyrtcm-1.1.1/src/pyrtcm.egg-info/dependency_links.txt
+-rw-r--r--   0 steve      (501) staff       (20)      113 2024-05-23 12:21:45.000000 pyrtcm-1.1.1/src/pyrtcm.egg-info/requires.txt
+-rw-r--r--   0 steve      (501) staff       (20)        7 2024-05-23 12:21:45.000000 pyrtcm-1.1.1/src/pyrtcm.egg-info/top_level.txt
+drwxr-xr-x   0 steve      (501) staff       (20)        0 2024-05-23 12:21:45.573532 pyrtcm-1.1.1/tests/
+-rw-r--r--   0 steve      (501) staff       (20)     1097 2024-05-23 12:21:11.000000 pyrtcm-1.1.1/tests/test_definitions.py
+-rw-r--r--   0 steve      (501) staff       (20)     6404 2024-05-23 12:21:11.000000 pyrtcm-1.1.1/tests/test_socket.py
+-rw-r--r--   0 steve      (501) staff       (20)    22900 2024-05-23 12:21:11.000000 pyrtcm-1.1.1/tests/test_static.py
+-rw-r--r--   0 steve      (501) staff       (20)   184535 2024-05-23 12:21:11.000000 pyrtcm-1.1.1/tests/test_stream.py
```

### Comparing `pyrtcm-1.1.0/LICENSE` & `pyrtcm-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrtcm-1.1.0/PKG-INFO` & `pyrtcm-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrtcm
-Version: 1.1.0
+Version: 1.1.1
 Summary: RTCM3 protocol parser
 Author-email: semuadmin <semuadmin@semuconsulting.com>
 Maintainer-email: semuadmin <semuadmin@semuconsulting.com>
 License: BSD 3-Clause License ("BSD License 2.0", "Revised BSD License", "New BSD License", or "Modified BSD License")
         
         Copyright (c) 2022, SEMU Consulting
         All rights reserved.
@@ -171,15 +171,16 @@
 Example -  Serial input:
 ```python
 from serial import Serial
 from pyrtcm import RTCMReader
 with Serial('/dev/tty.usbmodem14101', 9600, timeout=3) as stream:
   rtr = RTCMReader(stream)
   raw_data, parsed_data = rtr.read()
-  print(parsed_data)
+  if parsed_data is not None:
+    print(parsed_data)
 ```
 ```
 "<RTCM(1077, DF002=1077, DF003=0, DF004=204137001, DF393=1, DF409=0, DF001_7=0, ..., DF404_15=-9556, DF404_16=-2148, DF404_17=-2174)>",     
 ```
 
 Example - File input (using iterator).
 ```python
@@ -234,25 +235,21 @@
 ```
 
 Attributes within repeating groups are parsed with a two-digit suffix (`DF419_01`, `DF419_02`, etc. See [example below](#iterating) for an illustration of how to iterate through grouped attributes).
 
 Helper methods are available to interpret the individual datafields:
 
 ```python
-from pyrtcm import RTCM_DATA_FIELDS, datasiz, datascale, datadesc
+from pyrtcm import RTCM_DATA_FIELDS, datadesc
 dfname = "DF012"
 print(RTCM_DATA_FIELDS[dfname])
-print(datasiz(dfname))
-print(datascale(dfname))
 print(datadesc(dfname))
 ```
 ```
 (INT20, 0.0001, "GPS L1 PhaseRange - L1 Pseudorange")
-20
-0.0001
 'GPS L1 PhaseRange - L1 Pseudorange'
 ```
 
 The `payload` attribute always contains the raw payload as bytes.
 
 #### <a name="iterating">Iterating Through Group Attributes</a>
```

### Comparing `pyrtcm-1.1.0/README.md` & `pyrtcm-1.1.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -98,15 +98,16 @@
 Example -  Serial input:
 ```python
 from serial import Serial
 from pyrtcm import RTCMReader
 with Serial('/dev/tty.usbmodem14101', 9600, timeout=3) as stream:
   rtr = RTCMReader(stream)
   raw_data, parsed_data = rtr.read()
-  print(parsed_data)
+  if parsed_data is not None:
+    print(parsed_data)
 ```
 ```
 "<RTCM(1077, DF002=1077, DF003=0, DF004=204137001, DF393=1, DF409=0, DF001_7=0, ..., DF404_15=-9556, DF404_16=-2148, DF404_17=-2174)>",     
 ```
 
 Example - File input (using iterator).
 ```python
@@ -161,25 +162,21 @@
 ```
 
 Attributes within repeating groups are parsed with a two-digit suffix (`DF419_01`, `DF419_02`, etc. See [example below](#iterating) for an illustration of how to iterate through grouped attributes).
 
 Helper methods are available to interpret the individual datafields:
 
 ```python
-from pyrtcm import RTCM_DATA_FIELDS, datasiz, datascale, datadesc
+from pyrtcm import RTCM_DATA_FIELDS, datadesc
 dfname = "DF012"
 print(RTCM_DATA_FIELDS[dfname])
-print(datasiz(dfname))
-print(datascale(dfname))
 print(datadesc(dfname))
 ```
 ```
 (INT20, 0.0001, "GPS L1 PhaseRange - L1 Pseudorange")
-20
-0.0001
 'GPS L1 PhaseRange - L1 Pseudorange'
 ```
 
 The `payload` attribute always contains the raw payload as bytes.
 
 #### <a name="iterating">Iterating Through Group Attributes</a>
```

### Comparing `pyrtcm-1.1.0/pyproject.toml` & `pyrtcm-1.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta:__legacy__"
 
 [project]
 name = "pyrtcm"
 authors = [{ name = "semuadmin", email = "semuadmin@semuconsulting.com" }]
 maintainers = [{ name = "semuadmin", email = "semuadmin@semuconsulting.com" }]
 description = "RTCM3 protocol parser"
-version = "1.1.0"
+version = "1.1.1"
 license = { file = "LICENSE" }
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Operating System :: OS Independent",
     "Development Status :: 5 - Production/Stable",
     "Environment :: MacOS X",
```

### Comparing `pyrtcm-1.1.0/src/pyrtcm/__init__.py` & `pyrtcm-1.1.1/src/pyrtcm/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -15,10 +15,12 @@
     RTCMTypeError,
 )
 from pyrtcm.rtcmhelpers import *
 from pyrtcm.rtcmmessage import RTCMMessage
 from pyrtcm.rtcmreader import RTCMReader
 from pyrtcm.rtcmtypes_core import *
 from pyrtcm.rtcmtypes_get import *
+from pyrtcm.rtcmtypes_get_igs import *
+from pyrtcm.rtcmtypes_get_msm import *
 from pyrtcm.socket_stream import SocketStream
 
 version = __version__  # pylint: disable=invalid-name
```

### Comparing `pyrtcm-1.1.0/src/pyrtcm/exceptions.py` & `pyrtcm-1.1.1/src/pyrtcm/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyrtcm-1.1.0/src/pyrtcm/rtcmhelpers.py` & `pyrtcm-1.1.1/src/pyrtcm/rtcmhelpers.py`

 * *Files 17% similar despite different names*

```diff
@@ -22,15 +22,21 @@
 
     :param str att: grouped attribute name e.g. DF406_01
     :return: index as integer, or 0 if not grouped
     :rtype: int
     """
 
     try:
-        return int(att[att.rindex("_") - len(att) + 1 :])
+        att = att.split("_")
+        ln = len(att)
+        if ln == 2:  # one group level
+            return int(att[1])
+        if ln > 2:  # nested group level(s)
+            return tuple(int(att[i]) for i in range(1, ln))
+        return 0  # not grouped
     except ValueError:
         return 0
 
 
 def att2name(att: str) -> str:
     """
     Get name of grouped attribute.
@@ -38,53 +44,15 @@
     e.g. DF389_06 -> DF389; DF406_103 -> DF406
 
     :param str att: grouped attribute name e.g. DF406_01
     :return: name without index e.g. DF406
     :rtype: str
     """
 
-    try:
-        return att[: att.rindex("_")]
-    except ValueError:
-        return att
-
-
-def bits2val(att: str, scale: float, bitfield: int) -> object:
-    """
-    Convert bitfield to value for given attribute type.
-
-    :param str att: attribute type e.g. "UNT008"
-    :param float scale: scaling factor (where defined)
-    :param int bitfield: attribute as integer
-    :return: value
-    :rtype: object (int, float, char, bool)
-    """
-
-    typ = atttyp(att)
-    siz = attsiz(att)
-    val = msb = 0
-
-    if typ in ("SNT", "INT"):
-        msb = 2 ** (siz - 1)
-    if typ == "SNT":  # int, MSB indicates sign
-        val = bitfield & msb - 1
-        if bitfield & msb:
-            val *= -1
-    else:  # all other types
-        val = bitfield
-    if typ == "INT" and (bitfield & msb):  # 2's compliment -ve int
-        val = val - (1 << siz)
-    if typ in ("CHA", "UTF"):  # ASCII or UTF-8 character
-        val = chr(val)
-    # apply any scaling factor
-    else:
-        if scale not in (0, 1):
-            val *= scale
-
-    return val
+    return att.split("_")[0]
 
 
 def calc_crc24q(message: bytes) -> int:
     """
     Perform CRC24Q cyclic redundancy check.
 
     If the message includes the appended CRC bytes, the
@@ -131,77 +99,24 @@
     :return: payload length as 2 bytes padded with leading zeros
     :rtype: bytes
     """
 
     return len(payload).to_bytes(2, "big")
 
 
-def atttyp(att: str) -> str:
-    """
-    Get attribute type as string.
-
-    :param str att: attribute type e.g. 'UNT002'
-    :return: type of attribute as string e.g. 'UNT'
-    :rtype: str
-
-    """
-
-    return att[0:3]
-
-
-def attsiz(att: str) -> int:
-    """
-    Get attribute size in bits.
-
-    :param str att: attribute type e.g. 'U002'
-    :return: size of attribute in bits
-    :rtype: int
-
-    """
-
-    return int(att[-3:])
-
-
-def datasiz(datafield: str) -> int:
-    """
-    Get data field size in bits.
-
-    :param str datafield: datafield e.g. 'DF234'
-    :return: size of data field in bits
-    :rtype: int
-
-    """
-
-    (att, _, _) = RTCM_DATA_FIELDS[datafield[0:5]]
-    return attsiz(att)
-
-
-def datascale(datafield: str) -> float:
-    """
-    Get scaling factor of data field.
-
-    :param str datafield: datafield e.g. 'DF234'
-    :return: datafield scale factor or 0 if N/A
-    :rtype: float
-    """
-
-    (_, res, _) = RTCM_DATA_FIELDS[datafield[0:5]]
-    return res
-
-
 def datadesc(datafield: str) -> str:
     """
     Get description of data field.
 
     :param str datafield: datafield e.g. 'DF234'
     :return: datafield description
     :rtype: str
     """
 
-    (_, _, desc) = RTCM_DATA_FIELDS[datafield[0:5]]
+    (_, _, _, desc) = RTCM_DATA_FIELDS[datafield[0:5]]
     return desc
 
 
 def get_bit(data: bytes, num: int) -> int:
     """
     Get specified bit from bytes.
```

### Comparing `pyrtcm-1.1.0/src/pyrtcm/rtcmmessage.py` & `pyrtcm-1.1.1/src/pyrtcm/rtcmmessage.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,17 +4,16 @@
 Created on 14 Feb 2022
 
 :author: semuadmin
 :copyright: SEMU Consulting © 2022
 :license: BSD 3-Clause
 """
 
-import pyrtcm.exceptions as rte
-import pyrtcm.rtcmtypes_get as rtg
-from pyrtcm.rtcmhelpers import attsiz, bits2val, crc2bytes, escapeall, len2bytes
+from pyrtcm.exceptions import RTCMMessageError, RTCMTypeError
+from pyrtcm.rtcmhelpers import crc2bytes, escapeall, len2bytes
 from pyrtcm.rtcmtables import PRNSIGMAP
 from pyrtcm.rtcmtypes_core import (
     CELPRN,
     CELSIG,
     NA,
     NCELL,
     NHARMCOEFFC,
@@ -22,38 +21,40 @@
     NSAT,
     NSIG,
     PRN,
     RTCM_DATA_FIELDS,
     RTCM_HDR,
     RTCM_MSGIDS,
 )
+from pyrtcm.rtcmtypes_get import RTCM_PAYLOADS_GET
+from pyrtcm.rtcmtypes_get_igs import RTCM_PAYLOADS_GET_IGS
+from pyrtcm.rtcmtypes_get_msm import RTCM_PAYLOADS_GET_MSM
 
 BOOL = "B"
 
 
 class RTCMMessage:
     """RTCM Message Class."""
 
-    def __init__(self, payload: bytes = None, scaling: bool = True, labelmsm: int = 1):
+    def __init__(self, payload: bytes = None, labelmsm: int = 1):
         """Constructor.
 
         :param bytes payload: message payload (mandatory)
-        :param bool scaling: whether to apply attribute scaling True/False (True)
         :param int labelmsm: MSM NSAT and NCELL attribute label (1 = RINEX, 2 = freq)
         :raises: RTCMMessageError
         """
 
         # object is mutable during initialisation only
         super().__setattr__("_immutable", False)
 
         self._payload = payload
         if self._payload is None:
-            raise rte.RTCMMessageError("Payload must be specified")
+            raise RTCMMessageError("Payload must be specified")
+        self._payloadi = int.from_bytes(self._payload, "big")  # payload as int
         self._payblen = len(self._payload) * 8  # length of payload in bits
-        self._scaling = scaling
         self._labelmsm = labelmsm
         self._unknown = False
         self._satmap = None
         self._cellmap = None
         self._do_attributes()
 
         self._immutable = True  # once initialised, object is immutable
@@ -63,26 +64,26 @@
         Populate RTCMMessage attributes from payload.
 
         :raises: RTCMTypeError
         """
 
         offset = 0  # payload offset in bits
         index = []  # array of (nested) group indices
-
+        anam = ""
         try:
             # get payload definition dict for this message identity
             pdict = self._get_dict()
             if pdict is None:  # unknown (or not yet implemented) message identity
                 self._do_unknown()
                 return
             for anam in pdict:  # process each attribute in dict
-                (offset, index) = self._set_attribute(anam, pdict, offset, index)
+                offset, index = self._set_attribute(anam, pdict, offset, index)
 
-        except Exception as err:
-            raise rte.RTCMTypeError(
+        except Exception as err:  # pragma: no cover
+            raise RTCMTypeError(
                 (
                     f"Error processing attribute '{anam}' "
                     f"in message type {self.identity} {err}"
                 )
             ) from err
 
     def _set_attribute(self, anam: str, pdict: dict, offset: int, index: list) -> tuple:
@@ -98,21 +99,21 @@
 
         """
 
         adef = pdict[anam]  # get attribute definition
         if isinstance(adef, tuple):  # attribute group
             gtyp, _ = adef
             if isinstance(gtyp, tuple):  # conditional group of attributes
-                (offset, index) = self._set_attribute_optional(adef, offset, index)
+                offset, index = self._set_attribute_optional(adef, offset, index)
             else:  # repeating group of attributes
-                (offset, index) = self._set_attribute_group(adef, offset, index)
+                offset, index = self._set_attribute_group(adef, offset, index)
         else:  # single attribute
             offset = self._set_attribute_single(anam, offset, index)
 
-        return (offset, index)
+        return offset, index
 
     def _set_attribute_optional(self, adef: tuple, offset: int, index: list) -> tuple:
         """
         Process conditional group of attributes - group is present if attribute value
         = specific value, otherwise absent.
 
         :param tuple adef: attribute definition - tuple of ((attribute name, condition), group dict)
@@ -130,17 +131,17 @@
         #     for i in range(int(nestlevel)):
         #        anam += f"_{index[i]:02d}"
 
         if getattr(self, anam) == con:  # if condition is met...
             # recursively process each group attribute,
             # incrementing the payload offset as we go
             for anamg in gdict:
-                (offset, index) = self._set_attribute(anamg, gdict, offset, index)
+                offset, index = self._set_attribute(anamg, gdict, offset, index)
 
-        return (offset, index)
+        return offset, index
 
     def _set_attribute_group(self, adef: tuple, offset: int, index: list) -> tuple:
         """
         Process (nested) group of attributes.
 
         :param tuple adef: attribute definition - tuple of (attr name, attribute dict)
         :param int offset: payload offset in bits
@@ -167,19 +168,19 @@
 
         index.append(0)  # add a (nested) group index level
         # recursively process each group attribute,
         # incrementing the payload offset and index as we go
         for i in range(gsiz):
             index[-1] = i + 1
             for anamg in gdict:
-                (offset, index) = self._set_attribute(anamg, gdict, offset, index)
+                offset, index = self._set_attribute(anamg, gdict, offset, index)
 
         index.pop()  # remove this (nested) group index
 
-        return (offset, index)
+        return offset, index
 
     def _set_attribute_single(
         self,
         anam: str,
         offset: int,
         index: list,
     ) -> int:
@@ -190,50 +191,60 @@
         :param int offset: payload offset in bits
         :param list index: repeating group index array
         :return: offset
         :rtype: int
 
         """
 
-        # pylint: disable=invalid-name
+        # pylint: disable=invalid-name, line-too-long
 
         # if attribute is part of a (nested) repeating group, suffix name with index
         anami = anam
         for i in index:  # one index for each nested level
             if i > 0:
                 anami += f"_{i:02d}"
 
         # get value of required number of bits at current payload offset
-        atyp, ares, _ = RTCM_DATA_FIELDS[anam]
-        if not self._scaling:
-            ares = 0
+        atyp, asiz, ares, _ = RTCM_DATA_FIELDS[anam]
         if anam == "DF396":  # this MSM attribute has variable length
             asiz = getattr(self, NSAT) * getattr(self, NSIG)
-        else:
-            asiz = attsiz(atyp)
         if atyp == PRN:
             val = self._satmap[index[0]]
         elif atyp == CELPRN:
             val = self._cellmap[index[0]][0]
         elif atyp == CELSIG:
             val = self._cellmap[index[0]][1]
         else:
-            bitfield = self._getbits(offset, asiz)
-            val = bits2val(atyp, ares, bitfield)
+            # done inline for performance reasons...
+            bits = self._payloadi >> (self._payblen - offset - asiz) & ((1 << asiz) - 1)
+            msb = 1 << asiz - 1 if atyp in ("SNT", "INT") else 0
+            if atyp == "SNT":  # int, MSB indicates sign
+                val = bits & msb - 1
+                if bits & msb:
+                    val *= -1
+            else:  # all other types
+                val = bits
+            if atyp == "INT" and bits & msb:  # 2's compliment -ve int
+                val -= 1 << asiz
+            if atyp in ("CHA", "UTF"):  # ASCII or UTF-8 character
+                val = chr(val)
+            else:
+                if ares not in (0, 1):  # apply any scaling factor
+                    val *= ares
 
         setattr(self, anami, val)
         offset += asiz
 
         # add special attributes to keep track of
         # MSM message group sizes
         # NB: This is predicated on MSM payload dictionaries
         # always having attributes DF394, DF395 and DF396
         # in that order
         if anam in ("DF394", "DF395", "DF396"):
-            nbits = bin(bitfield).count("1")  # number of bits set
+            nbits = bin(bits).count("1")  # number of bits set
             if anam == "DF394":  # num of satellites in MSM message
                 setattr(self, NSAT, nbits)
             elif anam == "DF395":  # num of signals in MSM message
                 setattr(self, NSIG, nbits)
             elif anam == "DF396":  # num of cells in MSM message
                 setattr(self, NCELL, nbits)
                 # populate NSAT and NCELL mapping dictionaries
@@ -243,15 +254,14 @@
         if anam == "IDF038":
             i = index[0]
             N = getattr(self, f"IDF037_{i:02d}") + 1
             M = getattr(self, f"IDF038_{i:02d}") + 1
             nc = int(((N + 1) * (N + 2) / 2) - ((N - M) * (N - M + 1) / 2))
             ns = int(nc - (N + 1))
             # ncs = (N + 1) * (N + 1) - (N - M) * (N - M + 1)
-            # print(f"DEBUG nc {nc} ns {ns} ncs {ncs} nc+ns {nc+ns}")
             setattr(self, NHARMCOEFFC, nc)
             setattr(self, NHARMCOEFFS, ns)
 
         return offset
 
     def _getsatcellmaps(self):
         """
@@ -287,46 +297,28 @@
                 if getattr(self, "DF396") >> (ncells - idx) & 1:
                     ncell += 1
                     cells[ncell] = (sats[sat + 1], sigs[sig])
 
         self._satmap = sats
         self._cellmap = cells
 
-    def _getbits(self, position: int, length: int) -> int:
-        """
-        Get unsigned integer value of masked bits in bytes.
-
-        :param int position: position in bitfield, from leftmost bit
-        :param int length: length of masked bits
-        :return: value
-        :rtype: int
-        """
-
-        if length == 0:
-            return 0
-        if position + length > self._payblen:
-            raise rte.RTCMMessageError(
-                f"Attribute size {length} exceeds remaining "
-                + f"payload length {self._payblen - position}"
-            )
-
-        return int.from_bytes(self._payload, "big") >> (
-            self._payblen - position - length
-        ) & ((2 << length - 1) - 1)
-
     def _get_dict(self) -> dict:
         """
         Get payload dictionary corresponding to message identity
         (or None if message type not defined)
 
         :return: dictionary representing payload definition
         :rtype: dict or None
         """
 
-        return rtg.RTCM_PAYLOADS_GET.get(self.identity, None)
+        if "1070" <= self.identity <= "1229":  # MSM types
+            return RTCM_PAYLOADS_GET_MSM.get(self.identity, None)
+        if self.identity[:4] == "4076":  # IGS types
+            return RTCM_PAYLOADS_GET_IGS.get(self.identity, None)
+        return RTCM_PAYLOADS_GET.get(self.identity, None)
 
     def _do_unknown(self):
         """
         Handle unknown message type.
         """
 
         setattr(self, "DF002", self.identity)
@@ -341,15 +333,15 @@
         """
 
         stg = f"<RTCM({self.identity}, "
         for i, att in enumerate(self.__dict__):
             if att[0] != "_":  # only show public attributes
                 val = self.__dict__[att]
                 # escape all byte chars
-                if isinstance(val, bytes):
+                if isinstance(val, bytes):  # pragma: no cover
                     val = escapeall(val)
                 stg += att + "=" + str(val)
                 if i < len(self.__dict__) - 1:
                     stg += ", "
         if self._unknown:
             stg += ", Not_Yet_Implemented"
         stg += ")>"
@@ -374,15 +366,15 @@
 
         :param str name: attribute name
         :param object value: attribute value
         :raises: rtcmMessageError
         """
 
         if self._immutable:
-            raise rte.RTCMMessageError(
+            raise RTCMMessageError(
                 f"Object is immutable. Updates to {name} not permitted after initialisation."
             )
 
         super().__setattr__(name, value)
 
     def serialize(self) -> bytes:
         """
```

### Comparing `pyrtcm-1.1.0/src/pyrtcm/rtcmreader.py` & `pyrtcm-1.1.1/src/pyrtcm/rtcmreader.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,59 +20,64 @@
 Created on 14 Feb 2022
 
 :author: semuadmin
 :copyright: SEMU Consulting © 2022
 :license: BSD 3-Clause
 """
 
+from logging import getLogger
 from socket import socket
 
-import pyrtcm.exceptions as rte
-import pyrtcm.rtcmtypes_core as rtt
+from pyrtcm.exceptions import (
+    RTCMMessageError,
+    RTCMParseError,
+    RTCMStreamError,
+    RTCMTypeError,
+)
 from pyrtcm.rtcmhelpers import calc_crc24q
 from pyrtcm.rtcmmessage import RTCMMessage
+from pyrtcm.rtcmtypes_core import ERR_LOG, ERR_RAISE, NMEA_HDR, UBX_HDR, VALCKSUM
 from pyrtcm.socket_stream import SocketStream
 
 
 class RTCMReader:
     """
     rtcmReader class.
     """
 
     def __init__(
         self,
         datastream,
-        validate: int = rtt.VALCKSUM,
-        quitonerror: int = rtt.ERR_LOG,
-        scaling: bool = True,
+        validate: int = VALCKSUM,
+        quitonerror: int = ERR_LOG,
         labelmsm: int = 1,
         bufsize: int = 4096,
         errorhandler: object = None,
     ):  # pylint: disable=too-many-arguments
         """Constructor.
 
         :param datastream stream: input data stream
         :param int validate: 0 = ignore invalid checksum, 1 = validate checksum (1)
-        :param int quitonerror: 0 = ignore,  1 = log and continue, 2 = (re)raise (1)
-        :param bool scaling: apply attribute scaling True/False (True)
+        :param int quitonerror: ERR_IGNORE (0) = ignore errors,  ERR_LOG (1) = log continue,
+            ERR_RAISE (2) = (re)raise (1)
         :param int labelmsm: MSM NSAT and NCELL attribute label (1 = RINEX, 2 = freq)
         :param int bufsize: socket recv buffer size (4096)
         :param object errorhandler: error handling object or function (None)
         :raises: RTCMStreamError (if mode is invalid)
         """
 
         if isinstance(datastream, socket):
             self._stream = SocketStream(datastream, bufsize=bufsize)
         else:
             self._stream = datastream
         self._quitonerror = quitonerror
         self._errorhandler = errorhandler
         self._validate = validate
-        self._scaling = scaling
         self._labelmsm = labelmsm
+        self._logger = getLogger(__name__)
 
     def __iter__(self):
         """Iterator."""
 
         return self
 
     def __next__(self) -> tuple:
@@ -99,52 +104,52 @@
         :return: tuple of (raw_data as bytes, parsed_data as RTCMMessage)
         :rtype: tuple
         :raises: RTCMStreamError (if unrecognised protocol in data stream)
         """
 
         parsing = True
 
-        try:
-            while parsing:  # loop until end of valid message or EOF
+        while parsing:  # loop until end of valid message or EOF
+            try:
                 raw_data = None
                 parsed_data = None
                 byte1 = self._read_bytes(1)  # read the first byte
                 # if not UBX, NMEA or RTCM3, discard and continue
                 if byte1 not in (b"\xb5", b"\x24", b"\xd3"):
                     continue
                 byte2 = self._read_bytes(1)
                 bytehdr = byte1 + byte2
                 # if it's a UBX message (b'\xb5\x62'), ignore it
-                if bytehdr == rtt.UBX_HDR:
+                if bytehdr == UBX_HDR:
                     (raw_data, parsed_data) = self._parse_ubx(bytehdr)
                     continue
                 # if it's an NMEA message ('$G' or '$P'), ignore it
-                if bytehdr in rtt.NMEA_HDR:
+                if bytehdr in NMEA_HDR:
                     (raw_data, parsed_data) = self._parse_nmea(bytehdr)
                     continue
                 # if it's a RTCM3 message
                 # (byte1 = 0xd3; byte2 = 0b000000**)
                 if byte1 == b"\xd3" and (byte2[0] & ~0x03) == 0:
                     (raw_data, parsed_data) = self._parse_rtcm3(bytehdr)
                     parsing = False
                 # unrecognised protocol header
                 else:
-                    continue
+                    raise RTCMParseError(f"Unknown protocol header {bytehdr}.")
 
-        except EOFError:
-            return (None, None)
-        except (
-            rte.RTCMMessageError,
-            rte.RTCMParseError,
-            rte.RTCMStreamError,
-            rte.RTCMTypeError,
-        ) as err:
-            if self._quitonerror:
-                self._do_error(str(err))
-            parsed_data = str(err)
+            except EOFError:
+                return (None, None)
+            except (
+                RTCMMessageError,
+                RTCMParseError,
+                RTCMStreamError,
+                RTCMTypeError,
+            ) as err:
+                if self._quitonerror:
+                    self._do_error(err)
+                continue
 
         return (raw_data, parsed_data)
 
     def _parse_ubx(self, hdr: bytes) -> tuple:
         """
         Parse remainder of UBX message.
 
@@ -193,15 +198,14 @@
         size = (hdr[1] << 8) | hdr3[0]
         payload = self._read_bytes(size)
         crc = self._read_bytes(3)
         raw_data = hdr + hdr3 + payload + crc
         parsed_data = self.parse(
             raw_data,
             validate=self._validate,
-            scaling=self._scaling,
             labelmsm=self._labelmsm,
         )
         return (raw_data, parsed_data)
 
     def _read_bytes(self, size: int) -> bytes:
         """
         Read a specified number of bytes from stream.
@@ -209,46 +213,56 @@
         :param int size: number of bytes to read
         :return: bytes
         :rtype: bytes
         :raises: EOFError if stream ends prematurely
         """
 
         data = self._stream.read(size)
-        if len(data) < size:  # EOF
+        if len(data) == 0:  # EOF
             raise EOFError()
+        if 0 < len(data) < size:  # truncated stream
+            raise RTCMStreamError(
+                "Serial stream terminated unexpectedly. "
+                f"{size} bytes requested, {len(data)} bytes returned."
+            )
         return data
 
     def _read_line(self) -> bytes:
         """
-        Read until end of line (CRLF).
+        Read bytes until LF (0x0a) terminator.
 
         :return: bytes
         :rtype: bytes
         :raises: EOFError if stream ends prematurely
         """
 
-        data = self._stream.readline()
-        if data[-2:] != b"\x0d\x0a":
-            raise EOFError()
+        data = self._stream.readline()  # NMEA protocol is CRLF-terminated
+        if len(data) == 0:
+            raise EOFError()  # EOF
+        if data[-1:] != b"\x0a":  # truncated stream
+            raise RTCMStreamError(
+                "Serial stream terminated unexpectedly. "
+                f"Line requested, {len(data)} bytes returned."
+            )
         return data
 
-    def _do_error(self, err: str):
+    def _do_error(self, err: Exception):
         """
         Handle error.
 
-        :param str err: error message
-        :raises: RTCMParseError if quitonerror = 2
+        :param Exception err: error message
+        :raises: Exception if quitonerror = 2
         """
 
-        if self._quitonerror == rtt.ERR_RAISE:
-            raise rte.RTCMParseError(err)
-        if self._quitonerror == rtt.ERR_LOG:
+        if self._quitonerror == ERR_RAISE:
+            raise err from err
+        if self._quitonerror == ERR_LOG:
             # pass to error handler if there is one
             if self._errorhandler is None:
-                print(err)
+                self._logger.error(err)
             else:
                 self._errorhandler(err)
 
     @property
     def datastream(self) -> object:
         """
         Getter for stream.
@@ -258,30 +272,28 @@
         """
 
         return self._stream
 
     @staticmethod
     def parse(
         message: bytes,
-        validate: int = rtt.VALCKSUM,
-        scaling: bool = True,
+        validate: int = VALCKSUM,
         labelmsm: int = 1,
-    ) -> "RTCMMessage":
+    ) -> RTCMMessage:
         """
         Parse RTCM message to RTCMMessage object.
 
         :param bytes message: RTCM raw message bytes
         :param int validate: 0 = don't validate CRC, 1 = validate CRC (1)
-        :param bool scaling: apply attribute scaling True/False (True)
         :param int labelmsm: MSM NSAT and NCELL attribute label (1 = RINEX, 2 = freq)
         :return: RTCMMessage object
         :rtype: RTCMMessage
         :raises: RTCMParseError (if data stream contains invalid data or unknown message type)
         """
 
-        if validate & rtt.VALCKSUM:
+        if validate & VALCKSUM:
             if calc_crc24q(message):
-                raise rte.RTCMParseError(
+                raise RTCMParseError(
                     f"RTCM3 message invalid - failed CRC: {message[-3:]}"
                 )
         payload = message[3:-3]
-        return RTCMMessage(payload=payload, scaling=scaling, labelmsm=labelmsm)
+        return RTCMMessage(payload=payload, labelmsm=labelmsm)
```

### Comparing `pyrtcm-1.1.0/src/pyrtcm/rtcmtables.py` & `pyrtcm-1.1.1/src/pyrtcm/rtcmtables.py`

 * *Files identical despite different names*

### Comparing `pyrtcm-1.1.0/src/pyrtcm/rtcmtypes_core.py` & `pyrtcm-1.1.1/src/pyrtcm/rtcmtypes_core.py`

 * *Files 16% similar despite different names*

```diff
@@ -79,649 +79,599 @@
 P2_55 = 2.7755575615628914e-17  # 2**-55
 P2_59 = 1.734723475976807e-18  # 2**-59
 P2_66 = 1.3552527156068805e-20  # 2**-66
 
 # ***************************************************
 # THESE ARE THE RTCM PROTOCOL DATA TYPES
 # ***************************************************
-BIT1 = "BIT001"  # 1 bit bit field
-BIT2 = "BIT002"  # 2 bit bit field
-BIT3 = "BIT003"  # 3 bit bit field
-BIT4 = "BIT004"  # 4 bit bit field
-BIT6 = "BIT006"  # 6 bit bit field
-BIT7 = "BIT007"  # 7 bit bit field
-BIT8 = "BIT008"  # 8 bit bit field
-BIT10 = "BIT010"  # 10 bit bit field
-BIT12 = "BIT012"  # 12 bit bit field
-BIT32 = "BIT032"  # 32 bit bit field
-BIT64 = "BIT064"  # 64 bit bit field
-BITX = "BIT999"  # variable bit field
-CHAR8 = "CHA008"  # 8 bit characters, ISO 8859-1 (not limited to ASCII)
-INT6 = "INT006"  # 6 bit 2’s complement integer
-INT8 = "INT008"  # 8 bit 2’s complement integer
-INT9 = "INT009"  # 9 bit 2’s complement integer
-INT10 = "INT010"  # 10 bit 2’s complement integer
-INT11 = "INT011"  # 11 bit 2’s complement integer
-INT12 = "INT012"  # 12 bit 2’s complement integer
-INT14 = "INT014"  # 14 bit 2’s complement integer
-INT15 = "INT015"  # 15 bit 2’s complement integer
-INT16 = "INT016"  # 16 bit 2’s complement integer
-INT17 = "INT017"  # 17 bit 2’s complement integer
-INT18 = "INT018"  # 18 bit 2’s complement integer
-INT19 = "INT019"  # 19 bit 2’s complement integer
-INT20 = "INT020"  # 20 bit 2’s complement integer
-INT21 = "INT021"  # 21 bit 2’s complement integer
-INT22 = "INT022"  # 22 bit 2’s complement integer
-INT23 = "INT023"  # 23 bit 2’s complement integer
-INT24 = "INT024"  # 24 bit 2’s complement integer
-INT25 = "INT025"  # 25 bit 2’s complement integer
-INT26 = "INT026"  # 26 bit 2’s complement integer
-INT27 = "INT027"  # 27 bit 2's complement integer
-INT30 = "INT030"  # 30 bit 2’s complement integer
-INT31 = "INT031"  # 31 bit 2’s complement integer
-INT32 = "INT032"  # 32 bit 2’s complement integer
-INT34 = "INT034"  # 34 bit 2’s complement integer
-INT35 = "INT035"  # 35 bit 2’s complement integer
-INT38 = "INT038"  # 38 bit 2’s complement integer
-UINT2 = "UINT002"  # 2 bit unsigned integer
-UINT3 = "UINT003"  # 3 bit unsigned integer
-UINT4 = "UINT004"  # 4 bit unsigned integer
-UINT5 = "UINT005"  # 5 bit unsigned integer
-UINT6 = "UINT006"  # 6 bit unsigned integer
-UINT7 = "UINT007"  # 7 bit unsigned integer
-UINT8 = "UINT008"  # 8 bit unsigned integer
-UINT9 = "UINT009"  # 9 bit unsigned integer
-UINT10 = "UNT010"  # 10 bit unsigned integer
-UINT11 = "UNT011"  # 11 bit unsigned integer
-UINT12 = "UNT012"  # 12 bit unsigned integer
-UINT13 = "UNT013"  # 13 bit unsigned integer
-UINT14 = "UNT014"  # 14 bit unsigned integer
-UINT16 = "UNT016"  # 16 bit unsigned integer
-UINT17 = "UNT017"  # 17 bit unsigned integer
-UINT18 = "UNT018"  # 18 bit unsigned integer
-UINT20 = "UNT020"  # 20 bit unsigned integer
-UINT23 = "UNT023"  # 23 bit unsigned integer
-UINT24 = "UNT024"  # 24 bit unsigned integer
-UINT25 = "UNT025"  # 25 bit unsigned integer
-UINT26 = "UNT026"  # 26 bit unsigned integer
-UINT27 = "UNT027"  # 27 bit unsigned integer
-UINT30 = "UNT030"  # 30 bit unsigned integer
-UINT32 = "UNT032"  # 32 bit unsigned integer
-UINT35 = "UNT035"  # 35 bit unsigned integer
-UINT36 = "UNT036"  # 36 bit unsigned integer
-INTS5 = "SNT005"  # 5 bit sign-magnitude integer
-INTS11 = "SNT011"  # 11 bit sign-magnitude integer
-INTS22 = "SNT022"  # 22 bit sign-magnitude integer
-INTS24 = "SNT024"  # 24 bit sign-magnitude integer
-INTS27 = "SNT027"  # 27 bit sign-magnitude integer
-INTS32 = "SNT032"  # 32 bit sign-magnitude integer
-UTF8 = "UTF008"  # Unicode UTF-8 Code Unit
-PRN = "PRN000"  # Derived satellite PRN
-CELPRN = "CPR000"  # Derived cell PRN
-CELSIG = "CSG000"  # Derived cell Signal ID
+BIT = "BIT"  # bitfield
+BITX = "BITX"  # variable bitfield
+CHA = "CHA"  # characters, ISO 8859-1 (not limited to ASCII)
+INT = "INT"  # 2’s complement integer
+UINT = "UINT"  # unsigned integer
+INTS = "SNT"  # sign-magnitude integer
+UTF = "UTF"  # Unicode UTF-8 Code Unit
+PRN = "PRN"  # Derived satellite PRN
+CELPRN = "CPR"  # Derived cell PRN
+CELSIG = "CSG"  # Derived cell Signal ID
 
 # ****************************************************
 # THESE ARE THE RTCM PROTOCOL DATA FIELDS
 #
-# DF key: (data_type, scale_factor, description)
+# DF key: (data_type, size in bits, resolution (scale factor), description)
 # scale_factor of 0 means N/A (no scaling)
 #
 # NOTICE 1: These values are provided in semicircles;
-#           multiply by π to use in orbit computations
+#           multiply by π to use in orbit,  computations
 #
 # ****************************************************
 RTCM_DATA_FIELDS = {
-    "PRN": (PRN, 0, "Derived satellite PRN"),
-    "CELLPRN": (CELPRN, 0, "Derived satellite PRN"),
-    "CELLSIG": (CELSIG, 0, "Derived satellite Signal ID"),
-    "DF001": (BIT1, 0, "Reserved Field"),
-    "DF001_1": (BIT1, 0, "Reserved 1 bit"),
-    "DF001_2": (BIT2, 0, "Reserved 2 bits"),
-    "DF001_3": (BIT3, 0, "Reserved 3 bits"),
-    "DF001_7": (BIT7, 0, "Reserved 7 bits"),
-    "DF002": (UINT12, 0, "Message Number"),
-    "DF003": (UINT12, 0, "Reference Station ID"),
-    "DF004": (UINT30, 1, "GPS Epoch Time (TOW)"),
-    "DF005": (BIT1, 0, "Synchronous GNSS Message Flag"),
-    "DF006": (UINT5, 0, "No. of GPS Satellite Signals Processed"),
-    "DF007": (BIT1, 0, "GPS Divergencefree Smoothing Indicator"),
-    "DF008": (BIT3, 0, "GPS Smoothing Interval"),
-    "DF009": (UINT6, 0, "GPS Satellite ID"),
-    "DF010": (BIT1, 0, "GPS L1 Code Indicator"),
-    "DF011": (UINT24, 0.02, "GPS L1 Pseudorange"),
-    "DF012": (INT20, 0.0005, "GPS L1 PhaseRange - L1 Pseudorange"),
-    "DF013": (UINT7, 0, "GPS L1 Lock Time Indicator"),
-    "DF014": (UINT8, 0, "GPS Integer L1 Pseudorange Modulus Ambiguity"),
-    "DF015": (UINT8, 0.25, "GPS L1 CNR"),
-    "DF016": (BIT2, 0, "GPS L2 Code Indicator"),
-    "DF017": (INT14, 0.02, "GPS L2-L1 Pseudorange Difference"),
-    "DF018": (INT20, 0.0005, "GPS L2 PhaseRange - L1 Pseudorange"),
-    "DF019": (UINT7, 0, "GPS L2 Lock Time Indicator"),
-    "DF020": (UINT8, 0.25, "GPS L2 CNR"),
-    "DF021": (UINT6, 0, "ITRF Realization Year"),
-    "DF022": (BIT1, 0, "GPS Indicator"),
-    "DF023": (BIT1, 0, "GLONASS Indicator"),
-    "DF024": (BIT1, 0, "Galileo Indicator"),
-    "DF025": (INT38, 0.0001, "Antenna Ref. Point ECEF-X"),
-    "DF026": (INT38, 0.0001, "Antenna Ref. Point ECEF-Y"),
-    "DF027": (INT38, 0.0001, "Antenna Ref. Point ECEF-Z"),
-    "DF028": (UINT16, 0.0001, "Antenna Height"),
-    "DF029": (UINT8, 0, "Descriptor Counter"),
-    "DF030": (CHAR8, 0, "Antenna Descriptor"),
-    "DF031": (UINT8, 0, "Antenna Setup ID"),
-    "DF032": (UINT8, 0, "Serial Number Counter"),
-    "DF033": (CHAR8, 0, "Antenna Serial Number"),
-    "DF034": (UINT27, 1, "GLONASS Epoch Time (tk)"),
-    "DF035": (UINT5, 1, "No. of GLONASS Satellite Signals Processed"),
-    "DF036": (BIT1, 0, "GLONASS Divergence-free Smoothing Indicator"),
-    "DF037": (BIT3, 0, "GLONASS Smoothing Interval"),
-    "DF038": (UINT6, 0, "GLONASS Satellite ID (Satellite Slot Number)"),
-    "DF039": (BIT1, 0, "GLONASS L1 Code Indicator"),
-    "DF040": (UINT5, 1, "GLONASS Satellite Frequency Channel Number"),
-    "DF041": (UINT25, 0.02, "GLONASS L1 Pseudorange"),
-    "DF042": (INT20, 0.0005, "GLONASS L1 PhaseRange - L1 Pseudorange"),
-    "DF043": (UINT7, 0, "GLONASS L1 Lock Time Indicator"),
+    "PRN": (PRN, 0, 0, "Derived satellite PRN"),
+    "CELLPRN": (CELPRN, 0, 0, "Derived satellite PRN"),
+    "CELLSIG": (CELSIG, 0, 0, "Derived satellite Signal ID"),
+    "DF001": (BIT, 1, 0, "Reserved Field"),
+    "DF001_1": (BIT, 1, 0, "Reserved 1 BIT, "),
+    "DF001_2": (BIT, 2, 0, "Reserved 2 BIT, s"),
+    "DF001_3": (BIT, 3, 0, "Reserved 3 BIT, s"),
+    "DF001_7": (BIT, 7, 0, "Reserved 7 BIT, s"),
+    "DF002": (UINT, 12, 0, "Message Number"),
+    "DF003": (UINT, 12, 0, "Reference Station ID"),
+    "DF004": (UINT, 30, 1, "GPS Epoch Time (TOW)"),
+    "DF005": (BIT, 1, 0, "Synchronous GNSS Message Flag"),
+    "DF006": (UINT, 5, 0, "No. of GPS Satellite Signals Processed"),
+    "DF007": (BIT, 1, 0, "GPS Divergence-free Smoothing Indicator"),
+    "DF008": (BIT, 3, 0, "GPS Smoothing Interval"),
+    "DF009": (UINT, 6, 0, "GPS Satellite ID"),
+    "DF010": (BIT, 1, 0, "GPS L1 Code Indicator"),
+    "DF011": (UINT, 24, 0.02, "GPS L1 Pseudorange"),
+    "DF012": (INT, 20, 0.0005, "GPS L1 PhaseRange - L1 Pseudorange"),
+    "DF013": (UINT, 7, 0, "GPS L1 Lock Time Indicator"),
+    "DF014": (UINT, 8, 0, "GPS INT,eger L1 Pseudorange Modulus Ambiguity"),
+    "DF015": (UINT, 8, 0.25, "GPS L1 CNR"),
+    "DF016": (BIT, 2, 0, "GPS L2 Code Indicator"),
+    "DF017": (INT, 14, 0.02, "GPS L2-L1 Pseudorange Difference"),
+    "DF018": (INT, 20, 0.0005, "GPS L2 PhaseRange - L1 Pseudorange"),
+    "DF019": (UINT, 7, 0, "GPS L2 Lock Time Indicator"),
+    "DF020": (UINT, 8, 0.25, "GPS L2 CNR"),
+    "DF021": (UINT, 6, 0, "ITRF Realization Year"),
+    "DF022": (BIT, 1, 0, "GPS Indicator"),
+    "DF023": (BIT, 1, 0, "GLONASS Indicator"),
+    "DF024": (BIT, 1, 0, "Galileo Indicator"),
+    "DF025": (INT, 38, 0.0001, "Antenna Ref. Point, ECEF-X"),
+    "DF026": (INT, 38, 0.0001, "Antenna Ref. Point, ECEF-Y"),
+    "DF027": (INT, 38, 0.0001, "Antenna Ref. Point, ECEF-Z"),
+    "DF028": (UINT, 16, 0.0001, "Antenna Height"),
+    "DF029": (UINT, 8, 0, "Descriptor Counter"),
+    "DF030": (CHA, 8, 0, "Antenna Descriptor"),
+    "DF031": (UINT, 8, 0, "Antenna Setup ID"),
+    "DF032": (UINT, 8, 0, "Serial Number Counter"),
+    "DF033": (CHA, 8, 0, "Antenna Serial Number"),
+    "DF034": (UINT, 27, 1, "GLONASS Epoch Time (tk)"),
+    "DF035": (UINT, 5, 1, "No. of GLONASS Satellite Signals Processed"),
+    "DF036": (BIT, 1, 0, "GLONASS Divergence-free Smoothing Indicator"),
+    "DF037": (BIT, 3, 0, "GLONASS Smoothing Interval"),
+    "DF038": (UINT, 6, 0, "GLONASS Satellite ID (Satellite Slot Number)"),
+    "DF039": (BIT, 1, 0, "GLONASS L1 Code Indicator"),
+    "DF040": (UINT, 5, 1, "GLONASS Satellite Frequency Channel Number"),
+    "DF041": (UINT, 25, 0.02, "GLONASS L1 Pseudorange"),
+    "DF042": (INT, 20, 0.0005, "GLONASS L1 PhaseRange - L1 Pseudorange"),
+    "DF043": (UINT, 7, 0, "GLONASS L1 Lock Time Indicator"),
     "DF044": (
-        UINT7,
+        UINT,
+        7,
         0,
-        "GLONASS Integer L1 Pseudorange Modulus Ambiguity",
+        "GLONASS INT,eger L1 Pseudorange Modulus Ambiguity",
     ),
-    "DF045": (UINT8, 0.25, "GLONASS L1 CNR"),
-    "DF046": (BIT2, 0, "GLONASS L2 Code Indicator"),
-    "DF047": (INT14, 0.02, "GLONASS L2-L1 Pseudorange Difference"),
-    "DF048": (INT20, 0.0005, "GLONASS L2 PhaseRange - L1 Pseudorange"),
-    "DF049": (UINT7, 0, "GLONASS L2 Lock Time Indicator"),
-    "DF050": (UINT8, 0.25, "GLONASS L2 CNR"),
-    "DF051": (UINT16, 1, "Modified Julian Day (MJD) Number"),
-    "DF052": (UINT17, 1, "Seconds of Day (UTC)"),
-    "DF053": (UINT5, 1, "Number of Message ID Announcements  to Follow (Nm)"),
-    "DF054": (UINT8, 1, "Leap Seconds, GPS-UTC"),
-    "DF055": (UINT12, 1, "Message ID"),
-    "DF056": (BIT1, 0, "Message Sync Flag"),
-    "DF057": (UINT16, 0.1, "Message Transmission Interval"),
-    "DF058": (UINT5, 1, "Number of Auxiliary Stations Transmitted"),
-    "DF059": (UINT8, 1, "Network ID"),
-    "DF060": (UINT12, 1, "Master Reference Station ID"),
-    "DF061": (UINT12, 1, "Auxiliary Reference Station ID"),
-    "DF062": (INT20, 25 * 10**6, "Aux-Master Delta Latitude"),
-    "DF063": (INT21, 25 * 10**6, "Aux-Master Delta Longitude"),
-    "DF064": (INT23, 1, "Aux-Master Delta Height"),
-    "DF065": (UINT23, 0.1, "GPS Epoch Time (GPS TOW)"),
-    "DF066": (BIT1, 1, "GPS Multiple Message Indicator"),
-    "DF067": (UINT4, 1, "Number of GPS Satellites"),
-    "DF068": (UINT6, 1, "GPS Satellite ID"),
-    "DF069": (INT17, 0.5, "GPS Ionospheric Carrier Phase Correction Difference"),
-    "DF070": (INT17, 0.5, "GPS Geometric Carrier Phase Correction Difference"),
-    "DF071": (BIT8, 1, "GPS IODE"),
-    "DF072": (UINT4, 0, "Subnetwork ID"),
-    "DF073": (UINT8, 0, "RESERVED for Provider ID"),
-    "DF074": (BIT2, 0, "GPS Ambiguity Status Flag"),
-    "DF075": (UINT3, 0, "GPS Non Sync Count"),
-    "DF076": (UINT10, 0, "GPS Week number"),
-    "DF077": (BIT4, 0, "GPS SV Acc. (URA)"),
-    "DF078": (BIT2, 1, "GPS CODE ON L2"),
-    "DF079": (INT14, P2_43, "GPS IDOT (Issue of Data, Time)"),  # see NOTICE 1 above
-    "DF080": (UINT8, 1, "GPS IODE (Issue of Data, Ephemeris)"),
-    "DF081": (UINT16, P2_P4, "GPS toc (Reference Time, Clock)"),
-    "DF082": (INT8, P2_55, "GPS af2 (Clock correction drift rate)"),
-    "DF083": (INT16, P2_43, "GPS af1 (Clock correction drift)"),
-    "DF084": (INT22, P2_31, "GPS af0 (Clock correction bias)"),
-    "DF085": (UINT10, 1, "GPS IODC (Issue of Data, Clock)"),
+    "DF045": (UINT, 8, 0.25, "GLONASS L1 CNR"),
+    "DF046": (BIT, 2, 0, "GLONASS L2 Code Indicator"),
+    "DF047": (INT, 14, 0.02, "GLONASS L2-L1 Pseudorange Difference"),
+    "DF048": (INT, 20, 0.0005, "GLONASS L2 PhaseRange - L1 Pseudorange"),
+    "DF049": (UINT, 7, 0, "GLONASS L2 Lock Time Indicator"),
+    "DF050": (UINT, 8, 0.25, "GLONASS L2 CNR"),
+    "DF051": (UINT, 16, 1, "Modified Julian Day (MJD) Number"),
+    "DF052": (UINT, 17, 1, "Seconds of Day (UTC)"),
+    "DF053": (UINT, 5, 1, "Number of Message ID Announcements to Follow (Nm)"),
+    "DF054": (UINT, 8, 1, "Leap Seconds, GPS-UTC"),
+    "DF055": (UINT, 12, 1, "Message ID"),
+    "DF056": (BIT, 1, 0, "Message Sync Flag"),
+    "DF057": (UINT, 16, 0.1, "Message Transmission Interval"),
+    "DF058": (UINT, 5, 1, "Number of Auxiliary Stations Transmitted"),
+    "DF059": (UINT, 8, 1, "Network ID"),
+    "DF060": (UINT, 12, 1, "Master Reference Station ID"),
+    "DF061": (UINT, 12, 1, "Auxiliary Reference Station ID"),
+    "DF062": (INT, 20, 25 * 10**6, "Aux-Master Delta Latitude"),
+    "DF063": (INT, 21, 25 * 10**6, "Aux-Master Delta Longitude"),
+    "DF064": (INT, 23, 1, "Aux-Master Delta Height"),
+    "DF065": (UINT, 23, 0.1, "GPS Epoch Time (GPS TOW)"),
+    "DF066": (BIT, 1, 1, "GPS Multiple Message Indicator"),
+    "DF067": (UINT, 4, 1, "Number of GPS Satellites"),
+    "DF068": (UINT, 6, 1, "GPS Satellite ID"),
+    "DF069": (INT, 17, 0.5, "GPS Ionospheric Carrier Phase Correction Difference"),
+    "DF070": (INT, 17, 0.5, "GPS Geometric Carrier Phase Correction Difference"),
+    "DF071": (BIT, 8, 1, "GPS IODE"),
+    "DF072": (UINT, 4, 0, "Subnetwork ID"),
+    "DF073": (UINT, 8, 0, "RESERVED for Provider ID"),
+    "DF074": (BIT, 2, 0, "GPS Ambiguity Status Flag"),
+    "DF075": (UINT, 3, 0, "GPS Non Sync Count"),
+    "DF076": (UINT, 10, 0, "GPS Week number"),
+    "DF077": (BIT, 4, 0, "GPS SV Acc. (URA)"),
+    "DF078": (BIT, 2, 1, "GPS CODE ON L2"),
+    "DF079": (INT, 14, P2_43, "GPS IDOT (Issue of Data, Time)"),  # see NOTICE 1 above
+    "DF080": (UINT, 8, 1, "GPS IODE (Issue of Data, Ephemeris)"),
+    "DF081": (UINT, 16, P2_P4, "GPS toc (Reference Time, Clock)"),
+    "DF082": (INT, 8, P2_55, "GPS af2 (Clock correction drift rate)"),
+    "DF083": (INT, 16, P2_43, "GPS af1 (Clock correction drift)"),
+    "DF084": (INT, 22, P2_31, "GPS af0 (Clock correction bias)"),
+    "DF085": (UINT, 10, 1, "GPS IODC (Issue of Data, Clock)"),
     "DF086": (
-        INT16,
+        INT,
+        16,
         P2_5,
-        "GPS Crs (Amplitude of sine harmonic correction term to the orbit radius)",
+        "GPS Crs (Amplitude of sine harmonic correction term to the orbit, radius)",
     ),
     "DF087": (
-        INT16,
+        INT,
+        16,
         P2_43,
         "GPS ∆n (Mean motion difference from computed value)",
     ),  # see NOTICE 1 above
-    "DF088": (INT32, P2_31, "GPS M0 (Mean Anomaly)"),  # see NOTICE 1 above
+    "DF088": (INT, 32, P2_31, "GPS M0 (Mean Anomaly)"),  # see NOTICE 1 above
     "DF089": (
-        INT16,
+        INT,
+        16,
         P2_29,
         "GPS Cuc (Amplitude of cosine harmonic correction term to argument of latitude)",
     ),
-    "DF090": (UINT32, P2_33, "GPS e (Eccentricity)"),
+    "DF090": (UINT, 32, P2_33, "GPS e (Eccentricity)"),
     "DF091": (
-        INT16,
+        INT,
+        16,
         P2_29,
         "GPS Cus (Amplitude of sine harmonic correction term to argument of latitude)",
     ),
-    "DF092": (UINT32, P2_19, "GPS A½ (Square root of Semi-major Axis)"),
-    "DF093": (UINT16, P2_P4, "GPS toe (Reference Time, Ephemeris)"),
+    "DF092": (UINT, 32, P2_19, "GPS A½ (Square root of Semi-major Axis)"),
+    "DF093": (UINT, 16, P2_P4, "GPS toe (Reference Time, Ephemeris)"),
     "DF094": (
-        INT16,
+        INT,
+        16,
         P2_29,
         "GPS Cic (Amplitude of cosine harmonic correction term to angle of inclination)",
     ),
     "DF095": (
-        INT32,
+        INT,
+        32,
         P2_31,
         "GPS Ω0 (Longitude of Ascending Node)",
     ),  # see NOTICE 1 above
     "DF096": (
-        INT16,
+        INT,
+        16,
         P2_29,
         "GPS Cis (Amplitude of sine harmonic correction term to angle of inclination)",
     ),
-    "DF097": (INT32, P2_31, "GPS i0 (Inclination)"),  # see NOTICE 1 above
+    "DF097": (INT, 32, P2_31, "GPS i0 (Inclination)"),  # see NOTICE 1 above
     "DF098": (
-        INT16,
+        INT,
+        16,
         P2_5,
-        "GPS Crc (Amplitude of cosine harmonic correction term to orbit radius)",
+        "GPS Crc (Amplitude of cosine harmonic correction term to orbit,  radius)",
     ),
-    "DF099": (INT32, P2_31, "GPS ω (Argument of Perigee)"),  # see NOTICE 1 above
+    "DF099": (INT, 32, P2_31, "GPS ω (Argument of Perigee)"),  # see NOTICE 1 above
     "DF100": (
-        INT24,
+        INT,
+        24,
         P2_43,
         "GPS ΩDOT (Rate of Change of Right Ascension)",
     ),  # see NOTICE 1 above
-    "DF101": (INT8, P2_31, "GPS tGD"),
-    "DF102": (UINT6, 1, "GPS SV HEALTH"),
-    "DF103": (BIT1, 1, "GPS L2 P data flag"),
-    "DF104": (BIT1, 0, "GLONASS almanac health"),
-    "DF105": (BIT1, 0, "GLONASS almanac health availability indicator"),
-    "DF106": (BIT2, 0, "GLONASS P1"),
-    "DF107": (BIT12, 0, "GLONASS tk"),
-    "DF108": (BIT1, 0, "GLONASS MSB of Bn word"),
-    "DF109": (BIT1, 0, "GLONASS P2"),
-    "DF110": (UINT7, 1, "GLONASS tb"),
-    "DF111": (INTS24, P2_20, "GLONASS xn(tb), first derivative"),
-    "DF112": (INTS27, P2_11, "GLONASS xn(tb)"),
-    "DF113": (INTS5, P2_30, "GLONASS xn(tb), second derivative"),
-    "DF114": (INTS24, P2_20, "GLONASS yn(tb), first derivative"),
-    "DF115": (INTS27, P2_11, "GLONASS yn(tb)"),
-    "DF116": (INTS5, P2_30, "GLONASS yn(tb), second derivative"),
-    "DF117": (INTS24, P2_20, "GLONASS zn(tb), first derivative"),
-    "DF118": (INTS27, P2_11, "GLONASS zn(tb)"),
-    "DF119": (INTS5, P2_30, "GLONASS zn(tb), second derivative"),
-    "DF120": (BIT1, 0, "GLONASS P3"),
-    "DF121": (INTS11, 0, "GLONASS γn(tb) (Relative deviation)"),
-    "DF122": (BIT2, 0, "GLONASS-M P"),
-    "DF123": (BIT1, 0, "GLONASS-M ln (third string)"),
-    "DF124": (INTS22, 0, "GLONASS τn (tb)"),
-    "DF125": (INTS5, 0, "GLONASS-M Δτn"),
-    "DF126": (UINT5, 1, "GLONASS En"),
-    "DF127": (BIT1, 0, "GLONASS-M P4"),
-    "DF128": (UINT4, 0, "GLONASS-M FT"),
-    "DF129": (UINT11, 1, "GLONASS-M NT"),
-    "DF130": (BIT2, 0, "GLONASS-M M"),
-    "DF131": (BIT1, 0, "GLONASS The Availability of Additional Data"),
-    "DF132": (UINT11, 1, "GLONASS NA"),
-    "DF133": (INTS32, 0, "GLONASS τc"),
-    "DF134": (UINT5, 0, "GLONASS-M N4"),
-    "DF135": (INTS22, 0, "GLONASS-M τGPS"),
-    "DF136": (BIT1, 0, "GLONASS-M ln (fifth string)"),
-    "DF137": (BIT1, 1, "GPS Fit Interval"),
-    "DF138": (UINT7, 1, "Number of Characters to Follow"),
-    "DF139": (UINT8, 1, "Number of UTF-8 Code Units"),
-    "DF140": (UTF8, 0, "UTF-8 Character Code Units"),
-    "DF141": (BIT1, 0, "Reference-Station Indicator"),
-    "DF142": (BIT1, 0, "Single Receiver Oscillator Indicator"),
-    "DF143": (UINT5, 0, "Source-Name Counter"),
-    "DF144": (CHAR8, 0, "Source-Name"),
-    "DF145": (UINT5, 0, "Target-Name Counter"),
-    "DF146": (CHAR8, 0, "Target-Name"),
-    "DF147": (UINT8, 0, "SystemIdentification Number"),
-    "DF148": (BIT10, 0, "Utilized Tranformation Message Indicator"),
-    "DF149": (UINT5, 0, "Plate Number"),
-    "DF150": (UINT4, 0, "Computation Indicator"),
-    "DF151": (UINT2, 0, "Height Indicator"),
-    "DF152": (INT19, 2, "ΦV (Area of validity, lat)"),
-    "DF153": (INT20, 2, "ΛV (Area of validity, lon)"),
-    "DF154": (UINT14, 2, "∆ΦV (Area of validity, NS extension"),
-    "DF155": (UINT14, 2, "∆ΛV (Area of validity, EW extension"),
-    "DF156": (INT23, 0.001, "dX (Translation in X"),
-    "DF157": (INT23, 0.001, "dY (Translation in Y)"),
-    "DF158": (INT23, 0.001, "dZ (Translation in Z)"),
-    "DF159": (INT32, 0.00002, "R1 (Rotation around X)"),
-    "DF160": (INT32, 0.00002, "R2 (Rotation around Y)"),
-    "DF161": (INT32, 0.00002, "R3 (Rotation around Z)"),
-    "DF162": (INT25, 0.00002, "dS (Scale correction)"),
-    "DF163": (INT35, 0.001, "XP (X-coord for Molodenski-Badekas rotation)"),
-    "DF164": (INT35, 0.001, "YP (Y-coord for Molodenski-Badekas rotation)"),
-    "DF165": (INT35, 0.001, "ZP (Z-coord for Molodenski-Badekas rotation)"),
-    "DF166": (UINT24, 0.001, "add aS"),
-    "DF167": (UINT25, 0.001, "add bS"),
-    "DF168": (UINT24, 0.001, "add aT"),
-    "DF169": (UINT25, 0.001, "add bT"),
-    "DF170": (UINT6, 0, "Projection Type"),
-    "DF171": (INT34, 0.000000011, "LaNO [°]"),
-    "DF172": (INT35, 0.000000011, "LoNO [°]"),
-    "DF173": (UINT30, 0.00001, "add SNO"),
-    "DF174": (UINT36, 0.001, "FE"),
-    "DF175": (INT35, 0.001, "FN"),
-    "DF176": (INT34, 0.000000011, "LaFO [°]"),
-    "DF177": (INT35, 0.000000011, "LoFO [°]"),
-    "DF178": (INT34, 0.000000011, "LaSP1 [°]"),
-    "DF179": (INT34, 0.000000011, "LaSP2 [°]"),
-    "DF180": (UINT36, 0.001, "EFO"),
-    "DF181": (INT35, 0.001, "NFO"),
-    "DF182": (BIT1, 0, "Rectification Flag"),
-    "DF183": (INT34, 0.000000011, "LaPC"),
-    "DF184": (INT35, 0.000000011, "LoPC"),
-    "DF185": (UINT35, 0.000000011, "AzIL"),
-    "DF186": (INT26, 0.000000011, "Diff ARSG"),
-    "DF187": (UINT30, 0.00001, "Add SIL"),
-    "DF188": (UINT36, 0.001, "EPC"),
-    "DF189": (INT35, 0.001, "NPC"),
-    "DF190": (BIT1, 0, "Horizontal Shift Indicator"),
-    "DF191": (BIT1, 0, "Vertical Shift Indicator"),
-    "DF192": (INT21, 0.5, "Φ0"),
-    "DF193": (INT22, 0.5, "Λ0"),
-    "DF194": (UINT12, 0.5, "∆φ"),
-    "DF195": (UINT12, 0.5, "∆λ"),
-    "DF196": (INT8, 0.001, "Mean ∆φ"),
-    "DF197": (INT8, 0.001, "Mean ∆λ"),
-    "DF198": (INT15, 0.01, "Mean ∆H"),
-    "DF199": (INT9, 0.00003, "δφi"),
-    "DF200": (INT9, 0.00003, "δλi"),
-    "DF201": (INT9, 0.001, "δhi"),
-    "DF202": (INT25, 10, "N0"),
-    "DF203": (UINT26, 10, "E0"),
-    "DF204": (UINT12, 10, "∆N"),
-    "DF205": (UINT12, 10, "∆E"),
-    "DF206": (INT10, 0.01, "Mean ∆N"),
-    "DF207": (INT10, 0.01, "Mean ∆E"),
-    "DF208": (INT15, 0.01, "Mean ∆h"),
-    "DF209": (INT9, 0.001, "δNi"),
-    "DF210": (INT9, 0.001, "δEi"),
-    "DF211": (INT9, 0.001, "δhi"),
-    "DF212": (UINT2, 0, "Horizontal Interpolation Method Indicator"),
-    "DF213": (UINT2, 0, "Vertical Interpolation Method Indicator"),
-    "DF214": (UINT3, 0, "Horizontal Helmert/Molodenski Quality Indicator"),
-    "DF215": (UINT3, 0, "Vertical Helmert/Molodenski Quality Indicator"),
-    "DF216": (UINT3, 0, "Horizontal Grid Quality Indicator"),
-    "DF217": (UINT3, 0, "Vertical Grid Quality Indicator"),
-    "DF218": (UINT8, 0.5, "soc"),
-    "DF219": (UINT9, 0.01, "sod"),
-    "DF220": (UINT6, 0.1, "soh"),
-    "DF221": (UINT10, 0.5, "sIc"),
-    "DF222": (UINT10, 0.01, "sId"),
-    "DF223": (UINT7, 0, "N-Refs"),
-    "DF224": (UINT20, 1, "GPS Residuals Epoch Time (TOW)"),
-    "DF225": (UINT17, 1, "GLONASS Residuals Epoch Time (tk)"),
-    "DF226": (UINT12, 0, "Physical Reference Station ID"),
-    "DF227": (UINT8, 0, "Receiver Type Descriptor Counter"),
-    "DF228": (CHAR8, 0, "Receiver Type Descriptor"),
-    "DF229": (UINT8, 0, "Receiver Firmware Version Counter"),
-    "DF230": (CHAR8, 0, "Receiver Firmware Version"),
-    "DF231": (UINT8, 0, "Receiver Serial Number Counter"),
-    "DF232": (CHAR8, 0, "Receiver Serial Number"),
-    "DF233": (UINT20, 0.1, "GLONASS NW Epoch Time"),
-    "DF234": (UINT4, 0, "Number of GLONASS Data Entries"),
-    "DF235": (BIT2, 0, "GLONASS Ambiguity Status Flag"),
-    "DF236": (UINT3, 0, "GLONASS Non Sync Count"),
+    "DF101": (INT, 8, P2_31, "GPS tGD"),
+    "DF102": (UINT, 6, 1, "GPS SV HEALTH"),
+    "DF103": (BIT, 1, 1, "GPS L2 P data flag"),
+    "DF104": (BIT, 1, 0, "GLONASS almanac health"),
+    "DF105": (BIT, 1, 0, "GLONASS almanac health availability indicator"),
+    "DF106": (BIT, 2, 0, "GLONASS P1"),
+    "DF107": (BIT, 12, 0, "GLONASS tk"),
+    "DF108": (BIT, 1, 0, "GLONASS MSB of Bn word"),
+    "DF109": (BIT, 1, 0, "GLONASS P2"),
+    "DF110": (UINT, 7, 1, "GLONASS tb"),
+    "DF111": (INTS, 24, P2_20, "GLONASS xn(tb), first derivative"),
+    "DF112": (INTS, 27, P2_11, "GLONASS xn(tb)"),
+    "DF113": (INTS, 5, P2_30, "GLONASS xn(tb), second derivative"),
+    "DF114": (INTS, 24, P2_20, "GLONASS yn(tb), first derivative"),
+    "DF115": (INTS, 27, P2_11, "GLONASS yn(tb)"),
+    "DF116": (INTS, 5, P2_30, "GLONASS yn(tb), second derivative"),
+    "DF117": (INTS, 24, P2_20, "GLONASS zn(tb), first derivative"),
+    "DF118": (INTS, 27, P2_11, "GLONASS zn(tb)"),
+    "DF119": (INTS, 5, P2_30, "GLONASS zn(tb), second derivative"),
+    "DF120": (BIT, 1, 0, "GLONASS P3"),
+    "DF121": (INTS, 11, 0, "GLONASS γn(tb) (Relative deviation)"),
+    "DF122": (BIT, 2, 0, "GLONASS-M P"),
+    "DF123": (BIT, 1, 0, "GLONASS-M ln (third string)"),
+    "DF124": (INTS, 22, 0, "GLONASS τn (tb)"),
+    "DF125": (INTS, 5, 0, "GLONASS-M Δτn"),
+    "DF126": (UINT, 5, 1, "GLONASS En"),
+    "DF127": (BIT, 1, 0, "GLONASS-M P4"),
+    "DF128": (UINT, 4, 0, "GLONASS-M FT"),
+    "DF129": (UINT, 11, 1, "GLONASS-M NT"),
+    "DF130": (BIT, 2, 0, "GLONASS-M M"),
+    "DF131": (BIT, 1, 0, "GLONASS The Availability of Additional Data"),
+    "DF132": (UINT, 11, 1, "GLONASS NA"),
+    "DF133": (INTS, 32, 0, "GLONASS τc"),
+    "DF134": (UINT, 5, 0, "GLONASS-M N4"),
+    "DF135": (INTS, 22, 0, "GLONASS-M τGPS"),
+    "DF136": (BIT, 1, 0, "GLONASS-M ln (fifth string)"),
+    "DF137": (BIT, 1, 1, "GPS Fit Interval"),
+    "DF138": (UINT, 7, 1, "Number of Characters to Follow"),
+    "DF139": (UINT, 8, 1, "Number of UTF-8 Code Units"),
+    "DF140": (UTF, 8, 0, "UTF-8 Character Code Units"),
+    "DF141": (BIT, 1, 0, "Reference-Station Indicator"),
+    "DF142": (BIT, 1, 0, "Single Receiver Oscillator Indicator"),
+    "DF143": (UINT, 5, 0, "Source-Name Counter"),
+    "DF144": (CHA, 8, 0, "Source-Name"),
+    "DF145": (UINT, 5, 0, "Target-Name Counter"),
+    "DF146": (CHA, 8, 0, "Target-Name"),
+    "DF147": (UINT, 8, 0, "SystemIdentification Number"),
+    "DF148": (BIT, 10, 0, "Utilized Tranformation Message Indicator"),
+    "DF149": (UINT, 5, 0, "Plate Number"),
+    "DF150": (UINT, 4, 0, "Computation Indicator"),
+    "DF151": (UINT, 2, 0, "Height Indicator"),
+    "DF152": (INT, 19, 2, "ΦV (Area of validity, lat)"),
+    "DF153": (INT, 20, 2, "ΛV (Area of validity, lon)"),
+    "DF154": (UINT, 14, 2, "∆ΦV (Area of validity, NS extension"),
+    "DF155": (UINT, 14, 2, "∆ΛV (Area of validity, EW extension"),
+    "DF156": (INT, 23, 0.001, "dX (Translation in X"),
+    "DF157": (INT, 23, 0.001, "dY (Translation in Y)"),
+    "DF158": (INT, 23, 0.001, "dZ (Translation in Z)"),
+    "DF159": (INT, 32, 0.00002, "R1 (Rotation around X)"),
+    "DF160": (INT, 32, 0.00002, "R2 (Rotation around Y)"),
+    "DF161": (INT, 32, 0.00002, "R3 (Rotation around Z)"),
+    "DF162": (INT, 25, 0.00002, "dS (Scale correction)"),
+    "DF163": (INT, 35, 0.001, "XP (X-coord for Molodenski-Badekas rotation)"),
+    "DF164": (INT, 35, 0.001, "YP (Y-coord for Molodenski-Badekas rotation)"),
+    "DF165": (INT, 35, 0.001, "ZP (Z-coord for Molodenski-Badekas rotation)"),
+    "DF166": (UINT, 24, 0.001, "add aS"),
+    "DF167": (UINT, 25, 0.001, "add bS"),
+    "DF168": (UINT, 24, 0.001, "add aT"),
+    "DF169": (UINT, 25, 0.001, "add bT"),
+    "DF170": (UINT, 6, 0, "Projection Type"),
+    "DF171": (INT, 34, 0.000000011, "LaNO [°]"),
+    "DF172": (INT, 35, 0.000000011, "LoNO [°]"),
+    "DF173": (UINT, 30, 0.00001, "add SNO"),
+    "DF174": (UINT, 36, 0.001, "FE"),
+    "DF175": (INT, 35, 0.001, "FN"),
+    "DF176": (INT, 34, 0.000000011, "LaFO [°]"),
+    "DF177": (INT, 35, 0.000000011, "LoFO [°]"),
+    "DF178": (INT, 34, 0.000000011, "LaSP1 [°]"),
+    "DF179": (INT, 34, 0.000000011, "LaSP2 [°]"),
+    "DF180": (UINT, 36, 0.001, "EFO"),
+    "DF181": (INT, 35, 0.001, "NFO"),
+    "DF182": (BIT, 1, 0, "Rectification Flag"),
+    "DF183": (INT, 34, 0.000000011, "LaPC"),
+    "DF184": (INT, 35, 0.000000011, "LoPC"),
+    "DF185": (UINT, 35, 0.000000011, "AzIL"),
+    "DF186": (INT, 26, 0.000000011, "Diff ARSG"),
+    "DF187": (UINT, 30, 0.00001, "Add SIL"),
+    "DF188": (UINT, 36, 0.001, "EPC"),
+    "DF189": (INT, 35, 0.001, "NPC"),
+    "DF190": (BIT, 1, 0, "Horizontal Shift Indicator"),
+    "DF191": (BIT, 1, 0, "Vertical Shift Indicator"),
+    "DF192": (INT, 21, 0.5, "Φ0"),
+    "DF193": (INT, 22, 0.5, "Λ0"),
+    "DF194": (UINT, 12, 0.5, "∆φ"),
+    "DF195": (UINT, 12, 0.5, "∆λ"),
+    "DF196": (INT, 8, 0.001, "Mean ∆φ"),
+    "DF197": (INT, 8, 0.001, "Mean ∆λ"),
+    "DF198": (INT, 15, 0.01, "Mean ∆H"),
+    "DF199": (INT, 9, 0.00003, "δφi"),
+    "DF200": (INT, 9, 0.00003, "δλi"),
+    "DF201": (INT, 9, 0.001, "δhi"),
+    "DF202": (INT, 25, 10, "N0"),
+    "DF203": (UINT, 26, 10, "E0"),
+    "DF204": (UINT, 12, 10, "∆N"),
+    "DF205": (UINT, 12, 10, "∆E"),
+    "DF206": (INT, 10, 0.01, "Mean ∆N"),
+    "DF207": (INT, 10, 0.01, "Mean ∆E"),
+    "DF208": (INT, 15, 0.01, "Mean ∆h"),
+    "DF209": (INT, 9, 0.001, "δNi"),
+    "DF210": (INT, 9, 0.001, "δEi"),
+    "DF211": (INT, 9, 0.001, "δhi"),
+    "DF212": (UINT, 2, 0, "Horizontal Interpolation Method Indicator"),
+    "DF213": (UINT, 2, 0, "Vertical Interpolation Method Indicator"),
+    "DF214": (UINT, 3, 0, "Horizontal Helmert/Molodenski Quality Indicator"),
+    "DF215": (UINT, 3, 0, "Vertical Helmert/Molodenski Quality Indicator"),
+    "DF216": (UINT, 3, 0, "Horizontal Grid Quality Indicator"),
+    "DF217": (UINT, 3, 0, "Vertical Grid Quality Indicator"),
+    "DF218": (UINT, 8, 0.5, "soc"),
+    "DF219": (UINT, 9, 0.01, "sod"),
+    "DF220": (UINT, 6, 0.1, "soh"),
+    "DF221": (UINT, 10, 0.5, "sIc"),
+    "DF222": (UINT, 10, 0.01, "sId"),
+    "DF223": (UINT, 7, 0, "N-Refs"),
+    "DF224": (UINT, 20, 1, "GPS Residuals Epoch Time (TOW)"),
+    "DF225": (UINT, 17, 1, "GLONASS Residuals Epoch Time (tk)"),
+    "DF226": (UINT, 12, 0, "Physical Reference Station ID"),
+    "DF227": (UINT, 8, 0, "Receiver Type Descriptor Counter"),
+    "DF228": (CHA, 8, 0, "Receiver Type Descriptor"),
+    "DF229": (UINT, 8, 0, "Receiver Firmware Version Counter"),
+    "DF230": (CHA, 8, 0, "Receiver Firmware Version"),
+    "DF231": (UINT, 8, 0, "Receiver Serial Number Counter"),
+    "DF232": (CHA, 8, 0, "Receiver Serial Number"),
+    "DF233": (UINT, 20, 0.1, "GLONASS NW Epoch Time"),
+    "DF234": (UINT, 4, 0, "Number of GLONASS Data Entries"),
+    "DF235": (BIT, 2, 0, "GLONASS Ambiguity Status Flag"),
+    "DF236": (UINT, 3, 0, "GLONASS Non Sync Count"),
     "DF237": (
-        INT17,
+        INT,
+        17,
         0.5,
         "GLONASS Ionospheric Carrier Phase Correction Difference",
     ),
-    "DF238": (INT17, 0.5, "GLONASS Geometric Carrier Phase Correction Difference"),
-    "DF239": (BIT8, 0, "GLONASS IOD"),
-    "DF240": (UINT20, 1, "GPS FKP Epoch Time"),
-    "DF241": (UINT17, 1, "GLONASS FKP Epoch Time"),
-    "DF242": (INT12, 0.01, "N0: Geometric Gradient in North (ppm)"),
-    "DF243": (INT12, 0.01, "E0: Geometric gradient in east (ppm)"),
-    "DF244": (INT14, 0.01, "NI: Ionospheric gradient in north  (ppm)"),
-    "DF245": (INT14, 0.01, "EI: Ionospheric gradient in east  (ppm)"),
+    "DF238": (INT, 17, 0.5, "GLONASS Geometric Carrier Phase Correction Difference"),
+    "DF239": (BIT, 8, 0, "GLONASS IOD"),
+    "DF240": (UINT, 20, 1, "GPS FKP Epoch Time"),
+    "DF241": (UINT, 17, 1, "GLONASS FKP Epoch Time"),
+    "DF242": (INT, 12, 0.01, "N0: Geometric Gradient in north (ppm)"),
+    "DF243": (INT, 12, 0.01, "E0: Geometric gradient in east (ppm)"),
+    "DF244": (INT, 14, 0.01, "NI: Ionospheric gradient in north  (ppm)"),
+    "DF245": (INT, 14, 0.01, "EI: Ionospheric gradient in east  (ppm)"),
     # 'DF246-DF251': RESERVED,
-    "DF248": (UINT30, 1, "Galileo Epoch Time (TOW)"),
-    "DF252": (UINT6, 0, "Galileo Satellite ID"),
-    "DF286": (BIT8, 0, "Galileo SISA (E1,E5b"),
-    "DF287": (BIT2, 0, "Galileo E1-B Signal Health Status"),
-    "DF288": (BIT1, 0, "Galileo E1-B Data Validity Status"),
-    "DF289": (UINT12, 1, "Galileo Week Number"),
-    "DF290": (UINT10, 1, "Galileo IODnav"),
-    "DF291": (BIT8, 0, "Galileo SV SISA"),
-    "DF292": (INT14, P2_43, "Galileo Rate of Inclination (IDOT)"),
-    "DF293": (UINT14, 60, "Galileo toc"),
-    "DF294": (INT6, P2_59, "Galileo af2"),
-    "DF295": (INT21, P2_46, "Galileo af1"),
-    "DF296": (INT31, P2_34, "Galileo af0"),
-    "DF297": (INT16, P2_5, "Galileo Crs"),
-    "DF298": (INT16, P2_43, "Galileo ∆n"),
-    "DF299": (INT32, P2_31, "Galileo M0"),
-    "DF300": (INT16, P2_29, "Galileo Cuc"),
-    "DF301": (UINT32, P2_33, "Galileo Eccentricity (e)"),
-    "DF302": (INT16, P2_29, "Galileo Cus"),
-    "DF303": (UINT32, P2_19, "Galileo A½"),
-    "DF304": (UINT14, 60, "Galileo toe"),
-    "DF305": (INT16, P2_29, "Galileo Cic"),
-    "DF306": (INT32, P2_31, "Galileo Ω0"),
-    "DF307": (INT16, P2_29, "Galileo Cis"),
-    "DF308": (INT32, P2_31, "Galileo i0"),
-    "DF309": (INT16, P2_5, "Galileo Crc"),
-    "DF310": (INT32, P2_31, "Galileo ω (Argument of Perigee)"),
-    "DF311": (INT24, P2_43, "Galileo ΩDOT"),
-    "DF312": (INT10, P2_32, "Galileo BGD (E1/E5a)"),
-    "DF313": (INT10, P2_32, "Galileo BGD E5b/E1"),
-    "DF314": (BIT2, 0, "Galileo E5a Signal Health Status"),
-    "DF315": (BIT1, 0, "Galileo E5a Data Validity Status"),
-    "DF316": (BIT2, 0, "Galileo SOL NAV Signal Health Status (SOLHS)"),
-    "DF317": (BIT1, 0, "Galileo SOL NAV Data Validity Status (SOLDVS)"),
+    "DF248": (UINT, 30, 1, "Galileo Epoch Time (TOW)"),
+    "DF252": (UINT, 6, 0, "Galileo Satellite ID"),
+    "DF286": (BIT, 8, 0, "Galileo SISA (E1,E5b"),
+    "DF287": (BIT, 2, 0, "Galileo E1-B Signal Health Status"),
+    "DF288": (BIT, 1, 0, "Galileo E1-B Data Validity Status"),
+    "DF289": (UINT, 12, 1, "Galileo Week Number"),
+    "DF290": (UINT, 10, 1, "Galileo IODnav"),
+    "DF291": (BIT, 8, 0, "Galileo SV SISA"),
+    "DF292": (INT, 14, P2_43, "Galileo Rate of Inclination (IDOT)"),
+    "DF293": (UINT, 14, 60, "Galileo toc"),
+    "DF294": (INT, 6, P2_59, "Galileo af2"),
+    "DF295": (INT, 21, P2_46, "Galileo af1"),
+    "DF296": (INT, 31, P2_34, "Galileo af0"),
+    "DF297": (INT, 16, P2_5, "Galileo Crs"),
+    "DF298": (INT, 16, P2_43, "Galileo ∆n"),
+    "DF299": (INT, 32, P2_31, "Galileo M0"),
+    "DF300": (INT, 16, P2_29, "Galileo Cuc"),
+    "DF301": (UINT, 32, P2_33, "Galileo Eccentricity (e)"),
+    "DF302": (INT, 16, P2_29, "Galileo Cus"),
+    "DF303": (UINT, 32, P2_19, "Galileo A½"),
+    "DF304": (UINT, 14, 60, "Galileo toe"),
+    "DF305": (INT, 16, P2_29, "Galileo Cic"),
+    "DF306": (INT, 32, P2_31, "Galileo Ω0"),
+    "DF307": (INT, 16, P2_29, "Galileo Cis"),
+    "DF308": (INT, 32, P2_31, "Galileo i0"),
+    "DF309": (INT, 16, P2_5, "Galileo Crc"),
+    "DF310": (INT, 32, P2_31, "Galileo ω (Argument of Perigee)"),
+    "DF311": (INT, 24, P2_43, "Galileo ΩDOT"),
+    "DF312": (INT, 10, P2_32, "Galileo BGD (E1/E5a)"),
+    "DF313": (INT, 10, P2_32, "Galileo BGD E5b/E1"),
+    "DF314": (BIT, 2, 0, "Galileo E5a Signal Health Status"),
+    "DF315": (BIT, 1, 0, "Galileo E5a Data Validity Status"),
+    "DF316": (BIT, 2, 0, "Galileo SOL NAV Signal Health Status (SOLHS)"),
+    "DF317": (BIT, 1, 0, "Galileo SOL NAV Data Validity Status (SOLDVS)"),
     # 'DF318-DF363': RESERVED,
-    "DF364": (BIT2, 0, "Quarter Cycle Indicator"),
-    "DF365": (INT22, 0.1, "Delta Radial"),
-    "DF366": (INT20, 0.4, "Delta Along-Track"),
-    "DF367": (INT20, 0.4, "Delta Cross-Track"),
-    "DF368": (INT21, 0.001, "Dot Delta Radial"),
-    "DF369": (INT19, 0.004, "Dot Delta AlongTrack"),
-    "DF370": (INT19, 0.004, "Dot Delta CrossTrack"),
-    "DF371": (INT27, 0.00002, "RESERVED for Dot Dot Delta Radial"),
-    "DF372": (INT25, 0.00008, "RESERVED for Dot Dot DeltaAlong-Track"),
-    "DF373": (INT25, 0.00008, "RESERVED for Dot Dot Delta Cross-Track"),
-    "DF374": (BIT1, 0, "Satellite Reference Point"),
-    "DF375": (BIT1, 0, "Satellite Reference Datum"),
-    "DF376": (INT22, 0.1, "Delta Clock C0"),
-    "DF377": (INT21, 0.001, "Delta Clock C1"),
-    "DF378": (INT27, 0.00002, "Delta Clock C2"),
-    "DF379": (UINT5, 1, "No. of Code Biases Processed"),
-    "DF380": (UINT5, 1, "GPS Signal and Tracking Mode Identifier"),
-    "DF381": (UINT5, 1, "GLONASS Signal and Tracking Mode Identifier"),
-    "DF382": (UINT5, 1, "RESERVED for Galileo Signal and Tracking Mode Identifier"),
-    "DF383": (INT14, 0.01, "Code Bias"),
-    "DF384": (UINT5, 1, "GLONASS Satellite ID"),
-    "DF385": (UINT20, 1, "GPS Epoch Time 1s"),
-    "DF386": (UINT17, 1, "GLONASS Epoch Time 1s"),
-    "DF387": (UINT6, 1, "No. of Satellites"),
-    "DF388": (BIT1, 1, "Multiple Message Indicator"),
-    "DF389": (BIT6, 0, "SSR URA"),
-    "DF390": (INT22, 0.1, "High Rate Clock Correction"),
-    "DF391": (BIT4, 1, "SSR Update Interval"),
-    "DF392": (BIT8, 0, "GLONASS Issue Of Data (IOD)"),
-    "DF393": (BIT1, 0, "MSM Multiple message bit"),
-    "DF394": (BIT64, 0, "GNSS Satellite mask"),
-    "DF395": (BIT32, 0, "GNSS Signal mask"),
-    "DF396": (BITX, 0, "GNSS Cell mask"),
+    "DF364": (BIT, 2, 0, "Quarter Cycle Indicator"),
+    "DF365": (INT, 22, 0.1, "Delta Radial"),
+    "DF366": (INT, 20, 0.4, "Delta Along-Track"),
+    "DF367": (INT, 20, 0.4, "Delta Cross-Track"),
+    "DF368": (INT, 21, 0.001, "Dot Delta Radial"),
+    "DF369": (INT, 19, 0.004, "Dot Delta AlongTrack"),
+    "DF370": (INT, 19, 0.004, "Dot Delta CrossTrack"),
+    "DF371": (INT, 27, 0.00002, "RESERVED for Dot Dot Delta Radial"),
+    "DF372": (INT, 25, 0.00008, "RESERVED for Dot Dot DeltaAlong-Track"),
+    "DF373": (INT, 25, 0.00008, "RESERVED for Dot Dot Delta Cross-Track"),
+    "DF374": (BIT, 1, 0, "Satellite Reference Point"),
+    "DF375": (BIT, 1, 0, "Satellite Reference Datum"),
+    "DF376": (INT, 22, 0.1, "Delta Clock C0"),
+    "DF377": (INT, 21, 0.001, "Delta Clock C1"),
+    "DF378": (INT, 27, 0.00002, "Delta Clock C2"),
+    "DF379": (UINT, 5, 1, "No. of Code Biases Processed"),
+    "DF380": (UINT, 5, 1, "GPS Signal and Tracking Mode Identifier"),
+    "DF381": (UINT, 5, 1, "GLONASS Signal and Tracking Mode Identifier"),
+    "DF382": (UINT, 5, 1, "RESERVED for Galileo Signal and Tracking Mode Identifier"),
+    "DF383": (INT, 14, 0.01, "Code Bias"),
+    "DF384": (UINT, 5, 1, "GLONASS Satellite ID"),
+    "DF385": (UINT, 20, 1, "GPS Epoch Time 1s"),
+    "DF386": (UINT, 17, 1, "GLONASS Epoch Time 1s"),
+    "DF387": (UINT, 6, 1, "No. of Satellites"),
+    "DF388": (BIT, 1, 1, "Multiple Message Indicator"),
+    "DF389": (BIT, 6, 0, "SSR URA"),
+    "DF390": (INT, 22, 0.1, "High Rate Clock Correction"),
+    "DF391": (BIT, 4, 1, "SSR Update Interval"),
+    "DF392": (BIT, 8, 0, "GLONASS Issue Of Data (IOD)"),
+    "DF393": (BIT, 1, 0, "MSM Multiple message bit"),
+    "DF394": (BIT, 64, 0, "GNSS Satellite mask"),
+    "DF395": (BIT, 32, 0, "GNSS Signal mask"),
+    "DF396": (BITX, 0, 0, "GNSS Cell mask"),
     "DF397": (
-        UINT8,
+        UINT,
+        8,
         1,
-        "The number of integer milliseconds in GNSS Satellite  rough range",
+        "The number of INT,eger milliseconds in GNSS Satellite  rough range",
     ),
-    "DF398": (UINT10, P2_10, "GNSS Satellite rough range modulo 1 millisecond"),
-    "DF399": (INT14, 1, "GNSS Satellite rough Phase Range Rate"),
-    "DF400": (INT15, P2_24, "GNSS signal fine Pseudorange"),
-    "DF401": (INT22, P2_29, "GNSS signal fine PhaseRange data"),
-    "DF402": (UINT4, 0, "GNSS PhaseRange Lock Time Indicator"),
-    "DF403": (UINT6, 1, "GNSS signal CNR"),
-    "DF404": (INT15, 0.0001, "GNSS signal fine Phase Range Rate"),
+    "DF398": (UINT, 10, P2_10, "GNSS Satellite rough range modulo 1 millisecond"),
+    "DF399": (INT, 14, 1, "GNSS Satellite rough Phase Range Rate"),
+    "DF400": (INT, 15, P2_24, "GNSS signal fine Pseudorange"),
+    "DF401": (INT, 22, P2_29, "GNSS signal fine PhaseRange data"),
+    "DF402": (UINT, 4, 0, "GNSS PhaseRange Lock Time Indicator"),
+    "DF403": (UINT, 6, 1, "GNSS signal CNR"),
+    "DF404": (INT, 15, 0.0001, "GNSS signal fine Phase Range Rate"),
     "DF405": (
-        INT20,
+        INT,
+        20,
         P2_29,
         "GNSS signal fine Pseudorange with extended resolution",
     ),
     "DF406": (
-        INT24,
+        INT,
+        24,
         P2_31,
         "GNSS signal fine PhaseRange data with extended resolution",
     ),
     "DF407": (
-        UINT10,
+        UINT,
+        10,
         0,
         "GNSS PhaseRange Lock Time Indicator with extended range and resolution.",
     ),
-    "DF408": (UINT10, P2_4, "GNSS signal CNR with extended resolution"),
-    "DF409": (UINT3, 1, "IODS - Issue Of Data Station"),
+    "DF408": (UINT, 10, P2_4, "GNSS signal CNR with extended resolution"),
+    "DF409": (UINT, 3, 1, "IODS - Issue Of Data Station"),
     # 'DF410': RESERVED,
-    "DF411": (UINT2, 0, "Clock Steering Indicator"),
-    "DF412": (UINT2, 0, "External Clock Indicator"),
-    "DF413": (UINT4, 1, "IOD SSR"),
-    "DF414": (UINT16, 1, "SSR Provider ID"),
-    "DF415": (UINT4, 1, "SSR Solution ID"),
-    "DF416": (UINT3, 1, "GLONASS Day Of Week"),
-    "DF417": (BIT1, 0, "GNSS Smoothing Type Indicator"),
-    "DF418": (BIT3, 0, "GNSS Smoothing Interval"),
-    "DF419": (UINT4, 1, "GLONASS Satellite Frequency Channel Number"),
-    "DF420": (BIT1, 0, "Half-cycle ambiguity indicator"),
-    "DF421": (BIT1, 0, "GLONASS Code-Phase Bias Indicator"),
-    "DF422_1": (BIT1, 0, "GLONASS FDMA Signals Mask L1 C/A"),
-    "DF422_2": (BIT1, 0, "GLONASS FDMA Signals Mask L1 P"),
-    "DF422_3": (BIT1, 0, "GLONASS FDMA Signals Mask L2 C/A"),
-    "DF422_4": (BIT1, 0, "GLONASS FDMA Signals Mask L2 P"),
-    "DF423": (INT16, 0.02, "GLONASS L1 C/A Code-Phase Bias"),
-    "DF424": (INT16, 0.02, "GLONASS L1 P Code-Phase Bias"),
-    "DF425": (INT16, 0.02, "GLONASS L2 C/A Code-Phase Bias"),
-    "DF426": (INT16, 0.02, "GLONASS L2 P Code-Phase Bias"),
-    "DF427": (UINT30, 1, "BeiDou Epoch Time (TOW)"),
-    "DF428": (UINT30, 1, "QZSS Epoch Time (TOW)"),
-    "DF429": (UINT4, 1, "QZSS Satellite ID"),
-    "DF430": (UINT16, P2_P4, "QZSS toc"),
-    "DF431": (INT8, P2_55, "QZSS af2"),
-    "DF432": (INT16, P2_43, "QZSS af1"),
-    "DF433": (INT22, P2_31, "QZSS af0"),
-    "DF434": (UINT8, 1, "QZSS IODE"),
-    "DF435": (INT16, P2_5, "QZSS Crs"),
-    "DF436": (INT16, P2_43, "QZSS ∆n"),
-    "DF437": (INT32, P2_31, "QZSS M0"),
-    "DF438": (INT16, P2_29, "QZSS Cuc"),
-    "DF439": (UINT32, P2_33, "QZSS e"),
-    "DF440": (INT16, P2_29, "QZSS Cus"),
-    "DF441": (UINT32, P2_19, "QZSS A½"),
-    "DF442": (UINT16, P2_P4, "QZSS toe"),
-    "DF443": (INT16, P2_29, "QZSS Cic"),
-    "DF444": (INT32, P2_31, "QZSS Ω0"),
-    "DF445": (INT16, P2_29, "QZSS Cis"),
-    "DF446": (INT32, P2_31, "QZSS i0"),
-    "DF447": (INT16, P2_5, "QZSS Crc"),
-    "DF448": (INT32, P2_31, "QZSS ω (Argument of Perigee)"),
-    "DF449": (INT24, P2_43, "QZSS ΩDOT (Rate of Right Ascension)"),
-    "DF450": (INT14, P2_43, "QZSS i0-DOT"),
-    "DF451": (BIT2, 1, "QZSS Codes on L2 Channel"),
-    "DF452": (UINT10, 1, "QZSS Week Number"),
-    "DF453": (UINT4, 0, "QZSS URA"),
-    "DF454": (UINT6, 1, "QZSS SV health"),
-    "DF455": (INT8, P2_31, "QZSS TGD"),
-    "DF456": (UINT10, 1, "QZSS IODC"),
-    "DF457": (BIT1, 1, "QZSS Fit Interval"),
-    "DF488": (UINT6, 0, "BDS Satellite ID"),
-    "DF489": (UINT13, 1, "BDS Week Number"),
-    "DF490": (BIT4, 1, "BDS URAI"),
-    "DF491": (INT14, P2_43, "BDS IDOT"),
-    "DF492": (UINT5, 1, "BDS AODE"),
-    "DF493": (UINT17, 8, "BDS Toc"),
-    "DF494": (INT11, P2_66, "BDS a2"),
-    "DF495": (INT22, P2_50, "BDS a1"),
-    "DF496": (INT24, P2_33, "BSD a0"),
-    "DF497": (UINT5, 1, "BDS AODC"),
-    "DF498": (INT18, P2_6, "BDS Crs"),
-    "DF499": (INT16, P2_43, "BDS ∆n"),
-    "DF500": (INT32, P2_31, "BDS M0"),
-    "DF501": (INT18, P2_31, "BDS Cuc"),
-    "DF502": (UINT32, P2_33, "BDS e (Eccentricity)"),
-    "DF503": (INT18, P2_31, "BDS Cus"),
-    "DF504": (UINT32, P2_19, "BDS A½"),
-    "DF505": (UINT17, 8, "BDS Toe"),
-    "DF506": (INT18, P2_31, "BDS Cic"),
-    "DF507": (INT32, P2_31, "BDS Ω0"),
-    "DF508": (INT18, P2_31, "BDS Cis"),
-    "DF509": (INT32, P2_31, "BDS i0"),
-    "DF510": (INT18, P2_6, "BDS Crc"),
-    "DF511": (INT32, P2_31, "BDS ω (Argument of Perigee)"),
-    "DF512": (INT24, P2_43, "BDS ΩDOT (Rate of Right Ascension)"),
-    "DF513": (INT10, 0.1, "BDS TGD1"),
-    "DF514": (INT10, 0.1, "BDS TGD2"),
-    "DF515": (BIT1, 1, "BSD SV Health"),
-    "DF516": (UINT6, 1, "NAVIC/IRNSS Satellite ID"),
-    "DF517": (UINT10, 1, "NAVIC/IRNSS Week Number (WN)"),
-    "DF518": (INT22, P2_31, "NAVIC/IRNSS Clock Bias (af0)"),
-    "DF519": (INT16, P2_43, "NAVIC/IRNSS Clock Drift (af1)"),
-    "DF520": (INT8, P2_55, "NAVIC/IRNSS Clock Drift Rate (af2)"),
-    "DF521": (UINT4, 1, "NAVIC/IRNSS SV Accuracy (URA)"),
-    "DF522": (UINT16, 16, "NAVIC/IRNSS Time of Clock (toc)"),
-    "DF523": (INT8, P2_31, "NAVIC/IRNSS Total Group Delay (TGD)"),
-    "DF524": (INT22, P2_41, "NAVIC/IRNSS Mean Motion Difference (∆n)"),
-    "DF525": (UINT8, 1, "NAVIC/IRNSS Issue of Data Ephemeric & Clock (IODEC)"),
-    "DF526": (UINT10, 1, "NAVIC/IRNSS Reserved Bits after IODEC"),
-    "DF527": (BIT1, 1, "NAVIC/IRNSS L5 Flag"),
-    "DF528": (BIT1, 1, "NAVIC/IRNSS S Flag"),
-    "DF529": (INT15, P2_28, "NAVIC/IRNSS Cuc"),
-    "DF530": (INT15, P2_28, "NAVIC/IRNSS Cus"),
-    "DF531": (INT15, P2_28, "NAVIC/IRNSS Cic"),
-    "DF532": (INT15, P2_28, "NAVIC/IRNSS Cis"),
-    "DF533": (INT15, P2_4, "NAVIC/IRNSS Crc"),
-    "DF534": (INT15, P2_4, "NAVIC/IRNSS Crs"),
-    "DF535": (INT14, P2_43, "NAVIC/IRNSS IDOT"),
-    "DF536": (INT32, P2_31, "NAVIC/IRNSS M0"),
-    "DF537": (UINT16, 16, "NAVIC/IRNSS tOE"),
-    "DF538": (UINT32, P2_33, "NAVIC/IRNSS e (Eccentricity)"),
-    "DF539": (UINT32, P2_19, "NAVIC/IRNSS √A (Square root of semi major axis)"),
-    "DF540": (INT32, P2_31, "NAVIC/IRNSS Ω0 (Long of Ascending Node)"),
-    "DF541": (INT32, P2_31, "NAVIC/IRNSS ω (Argument of perigee)"),
-    "DF542": (INT22, P2_41, "NAVIC/IRNSS ΩDOT (Rate of Right Ascension)"),
-    "DF543": (INT32, P2_31, "NAVIC/IRNSS i0 (Inclination)"),
-    "DF544": (BIT2, 1, "NAVIC/IRNSS 2 spare bits after IDOT"),
-    "DF545": (BIT2, 1, "NAVIC/IRNSS 2 spare bits after i0"),
-    "DF546": (UINT30, 1, "NAVIC/IRNSS Epoch Time (TOW)"),
-    "ExtSatInfo": (UINT4, 0, "Extended Satellite Information"),
+    "DF411": (UINT, 2, 0, "Clock Steering Indicator"),
+    "DF412": (UINT, 2, 0, "External Clock Indicator"),
+    "DF413": (UINT, 4, 1, "IOD SSR"),
+    "DF414": (UINT, 16, 1, "SSR Provider ID"),
+    "DF415": (UINT, 4, 1, "SSR Solution ID"),
+    "DF416": (UINT, 3, 1, "GLONASS Day Of Week"),
+    "DF417": (BIT, 1, 0, "GNSS Smoothing Type Indicator"),
+    "DF418": (BIT, 3, 0, "GNSS Smoothing Interval"),
+    "DF419": (UINT, 4, 1, "GLONASS Satellite Frequency Channel Number"),
+    "DF420": (BIT, 1, 0, "Half-cycle ambiguity indicator"),
+    "DF421": (BIT, 1, 0, "GLONASS Code-Phase Bias Indicator"),
+    "DF422_1": (BIT, 1, 0, "GLONASS FDMA Signals Mask L1 C/A"),
+    "DF422_2": (BIT, 1, 0, "GLONASS FDMA Signals Mask L1 P"),
+    "DF422_3": (BIT, 1, 0, "GLONASS FDMA Signals Mask L2 C/A"),
+    "DF422_4": (BIT, 1, 0, "GLONASS FDMA Signals Mask L2 P"),
+    "DF423": (INT, 16, 0.02, "GLONASS L1 C/A Code-Phase Bias"),
+    "DF424": (INT, 16, 0.02, "GLONASS L1 P Code-Phase Bias"),
+    "DF425": (INT, 16, 0.02, "GLONASS L2 C/A Code-Phase Bias"),
+    "DF426": (INT, 16, 0.02, "GLONASS L2 P Code-Phase Bias"),
+    "DF427": (UINT, 30, 1, "BeiDou Epoch Time (TOW)"),
+    "DF428": (UINT, 30, 1, "QZSS Epoch Time (TOW)"),
+    "DF429": (UINT, 4, 1, "QZSS Satellite ID"),
+    "DF430": (UINT, 16, P2_P4, "QZSS toc"),
+    "DF431": (INT, 8, P2_55, "QZSS af2"),
+    "DF432": (INT, 16, P2_43, "QZSS af1"),
+    "DF433": (INT, 22, P2_31, "QZSS af0"),
+    "DF434": (UINT, 8, 1, "QZSS IODE"),
+    "DF435": (INT, 16, P2_5, "QZSS Crs"),
+    "DF436": (INT, 16, P2_43, "QZSS ∆n"),
+    "DF437": (INT, 32, P2_31, "QZSS M0"),
+    "DF438": (INT, 16, P2_29, "QZSS Cuc"),
+    "DF439": (UINT, 32, P2_33, "QZSS e"),
+    "DF440": (INT, 16, P2_29, "QZSS Cus"),
+    "DF441": (UINT, 32, P2_19, "QZSS A½"),
+    "DF442": (UINT, 16, P2_P4, "QZSS toe"),
+    "DF443": (INT, 16, P2_29, "QZSS Cic"),
+    "DF444": (INT, 32, P2_31, "QZSS Ω0"),
+    "DF445": (INT, 16, P2_29, "QZSS Cis"),
+    "DF446": (INT, 32, P2_31, "QZSS i0"),
+    "DF447": (INT, 16, P2_5, "QZSS Crc"),
+    "DF448": (INT, 32, P2_31, "QZSS ω (Argument of Perigee)"),
+    "DF449": (INT, 24, P2_43, "QZSS ΩDOT (Rate of Right Ascension)"),
+    "DF450": (INT, 14, P2_43, "QZSS i0-DOT"),
+    "DF451": (BIT, 2, 1, "QZSS Codes on L2 Channel"),
+    "DF452": (UINT, 10, 1, "QZSS Week Number"),
+    "DF453": (UINT, 4, 0, "QZSS URA"),
+    "DF454": (UINT, 6, 1, "QZSS SV health"),
+    "DF455": (INT, 8, P2_31, "QZSS TGD"),
+    "DF456": (UINT, 10, 1, "QZSS IODC"),
+    "DF457": (BIT, 1, 1, "QZSS Fit Interval"),
+    "DF488": (UINT, 6, 0, "BDS Satellite ID"),
+    "DF489": (UINT, 13, 1, "BDS Week Number"),
+    "DF490": (BIT, 4, 1, "BDS URAI"),
+    "DF491": (INT, 14, P2_43, "BDS IDOT"),
+    "DF492": (UINT, 5, 1, "BDS AODE"),
+    "DF493": (UINT, 17, 8, "BDS Toc"),
+    "DF494": (INT, 11, P2_66, "BDS a2"),
+    "DF495": (INT, 22, P2_50, "BDS a1"),
+    "DF496": (INT, 24, P2_33, "BSD a0"),
+    "DF497": (UINT, 5, 1, "BDS AODC"),
+    "DF498": (INT, 18, P2_6, "BDS Crs"),
+    "DF499": (INT, 16, P2_43, "BDS ∆n"),
+    "DF500": (INT, 32, P2_31, "BDS M0"),
+    "DF501": (INT, 18, P2_31, "BDS Cuc"),
+    "DF502": (UINT, 32, P2_33, "BDS e (Eccentricity)"),
+    "DF503": (INT, 18, P2_31, "BDS Cus"),
+    "DF504": (UINT, 32, P2_19, "BDS A½"),
+    "DF505": (UINT, 17, 8, "BDS Toe"),
+    "DF506": (INT, 18, P2_31, "BDS Cic"),
+    "DF507": (INT, 32, P2_31, "BDS Ω0"),
+    "DF508": (INT, 18, P2_31, "BDS Cis"),
+    "DF509": (INT, 32, P2_31, "BDS i0"),
+    "DF510": (INT, 18, P2_6, "BDS Crc"),
+    "DF511": (INT, 32, P2_31, "BDS ω (Argument of Perigee)"),
+    "DF512": (INT, 24, P2_43, "BDS ΩDOT (Rate of Right Ascension)"),
+    "DF513": (INT, 10, 0.1, "BDS TGD1"),
+    "DF514": (INT, 10, 0.1, "BDS TGD2"),
+    "DF515": (BIT, 1, 1, "BSD SV Health"),
+    "DF516": (UINT, 6, 1, "NAVIC/IRNSS Satellite ID"),
+    "DF517": (UINT, 10, 1, "NAVIC/IRNSS Week Number (WN)"),
+    "DF518": (INT, 22, P2_31, "NAVIC/IRNSS Clock Bias (af0)"),
+    "DF519": (INT, 16, P2_43, "NAVIC/IRNSS Clock Drift (af1)"),
+    "DF520": (INT, 8, P2_55, "NAVIC/IRNSS Clock Drift Rate (af2)"),
+    "DF521": (UINT, 4, 1, "NAVIC/IRNSS SV Accuracy (URA)"),
+    "DF522": (UINT, 16, 16, "NAVIC/IRNSS Time of Clock (toc)"),
+    "DF523": (INT, 8, P2_31, "NAVIC/IRNSS Total Group Delay (TGD)"),
+    "DF524": (INT, 22, P2_41, "NAVIC/IRNSS Mean Motion Difference (∆n)"),
+    "DF525": (UINT, 8, 1, "NAVIC/IRNSS Issue of Data Ephemeric & Clock (IODEC)"),
+    "DF526": (UINT, 10, 1, "NAVIC/IRNSS Reserved bits after IODEC"),
+    "DF527": (BIT, 1, 1, "NAVIC/IRNSS L5 Flag"),
+    "DF528": (BIT, 1, 1, "NAVIC/IRNSS S Flag"),
+    "DF529": (INT, 15, P2_28, "NAVIC/IRNSS Cuc"),
+    "DF530": (INT, 15, P2_28, "NAVIC/IRNSS Cus"),
+    "DF531": (INT, 15, P2_28, "NAVIC/IRNSS Cic"),
+    "DF532": (INT, 15, P2_28, "NAVIC/IRNSS Cis"),
+    "DF533": (INT, 15, P2_4, "NAVIC/IRNSS Crc"),
+    "DF534": (INT, 15, P2_4, "NAVIC/IRNSS Crs"),
+    "DF535": (INT, 14, P2_43, "NAVIC/IRNSS IDOT"),
+    "DF536": (INT, 32, P2_31, "NAVIC/IRNSS M0"),
+    "DF537": (UINT, 16, 16, "NAVIC/IRNSS tOE"),
+    "DF538": (UINT, 32, P2_33, "NAVIC/IRNSS e (Eccentricity)"),
+    "DF539": (UINT, 32, P2_19, "NAVIC/IRNSS √A (Square root of semi major axis)"),
+    "DF540": (INT, 32, P2_31, "NAVIC/IRNSS Ω0 (Long of Ascending Node)"),
+    "DF541": (INT, 32, P2_31, "NAVIC/IRNSS ω (Argument of perigee)"),
+    "DF542": (INT, 22, P2_41, "NAVIC/IRNSS ΩDOT (Rate of Right Ascension)"),
+    "DF543": (INT, 32, P2_31, "NAVIC/IRNSS i0 (Inclination)"),
+    "DF544": (BIT, 2, 1, "NAVIC/IRNSS 2 spare bits after IDOT"),
+    "DF545": (BIT, 2, 1, "NAVIC/IRNSS 2 spare bits after i0"),
+    "DF546": (UINT, 30, 1, "NAVIC/IRNSS Epoch Time (TOW)"),
+    "ExtSatInfo": (UINT, 4, 0, "Extended Satellite Information"),
     # IGS SSR data types, used in 4076 messages
     # https://files.igs.org/pub/data/format/igs_ssr_v1.pdf
-    "IDF001": (UINT3, 1, "IGM/IM Version"),
-    "IDF002": (UINT8, 1, "IGS Message Number"),
-    "IDF003": (UINT20, 1, "SSR Epoch Time 1s"),
-    "IDF004": (BIT4, 1, "SSR Update Interval"),
-    "IDF005": (BIT1, 1, "SSR Multiple Message Indicator"),
-    "IDF006": (BIT1, 1, "Global/Regional CRS Indicator"),
-    "IDF007": (UINT4, 1, "IOD SSR"),
-    "IDF008": (UINT16, 1, "SSR Provider ID"),
-    "IDF009": (UINT4, 1, "SSR Solution ID"),
-    "IDF010": (UINT6, 1, "No. of Satellites"),
-    "IDF011": (UINT6, 1, "GNSS Satellite ID"),
-    "IDF012": (BIT8, 1, "GNSS IOD"),
-    "IDF013": (INT22, 0.1, "Delta Orbit Radial"),
-    "IDF014": (INT20, 0.4, "Delta Orbit Along-Track"),
-    "IDF015": (INT20, 0.4, "Delta Orbit Cross-Track"),
-    "IDF016": (INT21, 0.001, "Dot Orbit Delta Radial"),
-    "IDF017": (INT19, 0.004, "Dot Orbit Delta Along-Track"),
-    "IDF018": (INT19, 0.004, "Dot Orbit Delta Cross-Track"),
-    "IDF019": (INT22, 0.1, "Delta Clock C0"),
-    "IDF020": (INT21, 0.001, "Delta Clock C1"),
-    "IDF021": (INT27, 0.00002, "Delta Clock C2"),
-    "IDF022": (INT22, 0.1, "High Rate Clock Correction"),
-    "IDF023": (UINT5, 1, "No. of Biases Processed"),
-    "IDF024": (UINT5, 1, "GNSS Signal and Tracking Mode Identifier"),
-    "IDF025": (INT14, 0.01, "Code Bias"),
-    "IDF026": (UINT9, 1 / 256, "Yaw Angle"),
-    "IDF027": (INT8, 1 / 8192, "Yaw Rate"),
-    "IDF028": (INT20, 0.0001, "Phase Bias"),
-    "IDF029": (BIT1, 1, "Signal Integer Indicator"),
-    "IDF030": (BIT2, 1, "Signals Wide-Lane Integer Indicator"),
-    "IDF031": (UINT4, 1, "Signal Discontinuity Counter"),
-    "IDF032": (BIT1, 1, "Dispersive Bias Consistency Indicator"),
-    "IDF033": (BIT1, 1, "MW Consistency Indicator"),
-    "IDF034": (BIT6, 1, "SSR URA"),
-    "IDF035": (UINT2, 1, "Number of Ionospheric Layers"),
-    "IDF036": (UINT8, 10, "Height of Ionospheric Layer"),
-    "IDF037": (UINT4, 1, "Spherical Harmonics Degree"),
-    "IDF038": (UINT4, 1, "Spherical Harmonics Order"),
-    "IDF039": (INT16, 0.005, "Spherical Harmonic Coefficient C"),
-    "IDF040": (INT16, 0.005, "Spherical Harmonic Coefficient S"),
-    "IDF041": (UINT9, 0.05, "VTEC Quality Indicator"),
+    "IDF001": (UINT, 3, 1, "IGM/IM Version"),
+    "IDF002": (UINT, 8, 1, "IGS Message Number"),
+    "IDF003": (UINT, 20, 1, "SSR Epoch Time 1s"),
+    "IDF004": (BIT, 4, 1, "SSR Update Interval"),
+    "IDF005": (BIT, 1, 1, "SSR Multiple Message Indicator"),
+    "IDF006": (BIT, 1, 1, "Global/Regional CRS Indicator"),
+    "IDF007": (UINT, 4, 1, "IOD SSR"),
+    "IDF008": (UINT, 16, 1, "SSR Provider ID"),
+    "IDF009": (UINT, 4, 1, "SSR Solution ID"),
+    "IDF010": (UINT, 6, 1, "No. of Satellites"),
+    "IDF011": (UINT, 6, 1, "GNSS Satellite ID"),
+    "IDF012": (BIT, 8, 1, "GNSS IOD"),
+    "IDF013": (INT, 22, 0.1, "Delta Orbit Radial"),
+    "IDF014": (INT, 20, 0.4, "Delta Orbit Along-Track"),
+    "IDF015": (INT, 20, 0.4, "Delta Orbit Cross-Track"),
+    "IDF016": (INT, 21, 0.001, "Dot Orbit Delta Radial"),
+    "IDF017": (INT, 19, 0.004, "Dot Orbit Delta Along-Track"),
+    "IDF018": (INT, 19, 0.004, "Dot Orbit Delta Cross-Track"),
+    "IDF019": (INT, 22, 0.1, "Delta Clock C0"),
+    "IDF020": (INT, 21, 0.001, "Delta Clock C1"),
+    "IDF021": (INT, 27, 0.00002, "Delta Clock C2"),
+    "IDF022": (INT, 22, 0.1, "High Rate Clock Correction"),
+    "IDF023": (UINT, 5, 1, "No. of Biases Processed"),
+    "IDF024": (UINT, 5, 1, "GNSS Signal and Tracking Mode Identifier"),
+    "IDF025": (INT, 14, 0.01, "Code Bias"),
+    "IDF026": (UINT, 9, 1 / 256, "Yaw Angle"),
+    "IDF027": (INT, 8, 1 / 8192, "Yaw Rate"),
+    "IDF028": (INT, 20, 0.0001, "Phase Bias"),
+    "IDF029": (BIT, 1, 1, "Signal Integer Indicator"),
+    "IDF030": (BIT, 2, 1, "Signals Wide-Lane Integer Indicator"),
+    "IDF031": (UINT, 4, 1, "Signal Discontinuity Counter"),
+    "IDF032": (BIT, 1, 1, "Dispersive Bias Consistency Indicator"),
+    "IDF033": (BIT, 1, 1, "MW Consistency Indicator"),
+    "IDF034": (BIT, 6, 1, "SSR URA"),
+    "IDF035": (UINT, 2, 1, "Number of Ionospheric Layers"),
+    "IDF036": (UINT, 8, 10, "Height of Ionospheric Layer"),
+    "IDF037": (UINT, 4, 1, "Spherical Harmonics Degree"),
+    "IDF038": (UINT, 4, 1, "Spherical Harmonics Order"),
+    "IDF039": (INT, 16, 0.005, "Spherical Harmonic Coefficient C"),
+    "IDF040": (INT, 16, 0.005, "Spherical Harmonic Coefficient S"),
+    "IDF041": (UINT, 9, 0.05, "VTEC Quality Indicator"),
 }
 
 # ***************************************************************************
 # THESE ARE THE RTCM PROTOCOL CORE MESSAGE IDENTITIES
 # Payloads for each of these identities are defined in the rtcmtypes_* modules
 # ***************************************************************************
 RTCM_MSGIDS = {
@@ -764,24 +714,24 @@
     "1038": "GLONASS Geometric Correction Differences",
     "1039": "GLONASS Combined Geometric and Ionospheric Correction Differences",
     "1041": "NavIC/IRNSS Ephemerides",
     "1042": "Beidou Ephemerides",
     "1044": "QZSS Ephemerides",
     "1045": "Galileo F/NAV Ephemerides",
     "1046": "Galileo I/NAV Ephemerides",
-    "1057": "GPS SSROrbit Correction",
+    "1057": "GPS SSROrBIT,  Correction",
     "1058": "GPS SSR Clock Correction",
     "1059": "GPS SSR Code Bias",
-    "1060": "GPS SSR Combined Orbit and Clock Corrections",
+    "1060": "GPS SSR Combined OrBIT,  and Clock Corrections",
     "1061": "GPS SSR URA",
     "1062": "GPS SSR High Rate Clock Correction",
-    "1063": "GLONASS SSR Orbit Correction",
+    "1063": "GLONASS SSR OrBIT,  Correction",
     "1064": "GLONASS SSR Clock Correction",
     "1065": "GLONASS SSR Code Bias",
-    "1066": "GLONASS SSR Combined Orbit and Clock Correction",
+    "1066": "GLONASS SSR Combined OrBIT,  and Clock Correction",
     "1067": "GLONASS SSR URA",
     "1068": "GLONASS SSR High Rate Clock Correction",
     "1070": "Reserved MSM",
     "1071": "GPS MSM1",
     "1072": "GPS MSM2",
     "1073": "GPS MSM3",
     "1074": "GPS MSM4",
@@ -855,58 +805,58 @@
     # NB: Only those proprietary messages with public
     # domain definitions have been implemented.
     #
     # "4001-4095":"Proprietary Messages",
     # "4072": "Mitsubishi Electric Corp",
     # "4073": "Unicore Communications Inc",
     # "4075": "Alberding GmbH",
-    # "4076": "International GNSS Service (IGS)",
-    "4076_021": "GPS SSR Orbit Correction",
+    # "4076": "INT,ernational GNSS Service (IGS)",
+    "4076_021": "GPS SSR OrBIT,  Correction",
     "4076_022": "GPS SSR Clock Correction",
-    "4076_023": "GPS SSR Combined Orbit and Clock Correction",
+    "4076_023": "GPS SSR Combined OrBIT,  and Clock Correction",
     "4076_024": "GPS SSR High Rate Clock Correction",
     "4076_025": "GPS SSR Code Bias",
     "4076_026": "GPS SSR Phase Bias",
     "4076_027": "GPS SSR URA",
     # "4076_028-040": "Reserved for GPS",
-    "4076_041": "GLONASS SSR Orbit Correction",
+    "4076_041": "GLONASS SSR OrBIT,  Correction",
     "4076_042": "GLONASS SSR Clock Correction",
-    "4076_043": "GLONASS SSR Combined Orbit and Clock Correction",
+    "4076_043": "GLONASS SSR Combined OrBIT,  and Clock Correction",
     "4076_044": "GLONASS SSR High Rate Clock Correction",
     "4076_045": "GLONASS SSR Code Bias",
     "4076_046": "GLONASS SSR Phase Bias",
     "4076_047": "GLONASS SSR URA",
     # "4076_048-060": "Reserved for GLONASS",
-    "4076_061": "Galileo SSR Orbit Correction",
+    "4076_061": "Galileo SSR OrBIT,  Correction",
     "4076_062": "Galileo SSR Clock Correction",
-    "4076_063": "Galileo SSR Combined Orbit and Clock Correction",
+    "4076_063": "Galileo SSR Combined OrBIT,  and Clock Correction",
     "4076_064": "Galileo SSR High Rate Clock Correction",
     "4076_065": "Galileo SSR Code Bias",
     "4076_066": "Galileo SSR Phase Bias",
     "4076_067": "Galileo SSR URA",
     # "4076_068-080": "Reserved for Galileo",
-    "4076_081": "QZSS SSR Orbit Correction",
+    "4076_081": "QZSS SSR OrBIT,  Correction",
     "4076_082": "QZSS SSR Clock Correction",
-    "4076_083": "QZSS SSR Combined Orbit and Clock Correction",
+    "4076_083": "QZSS SSR Combined OrBIT,  and Clock Correction",
     "4076_084": "QZSS SSR High Rate Clock Correction",
     "4076_085": "QZSS SSR Code Bias",
     "4076_086": "QZSS SSR Phase Bias",
     "4076_087": "QZSS SSR URA",
     # "4076_088-100": "Reserved for QZSS",
-    "4076_101": "BeiDou SSR Orbit Correction",
+    "4076_101": "BeiDou SSR OrBIT,  Correction",
     "4076_102": "BeiDou SSR Clock Correction",
-    "4076_103": "BeiDou SSR Combined Orbit and Clock Correction",
+    "4076_103": "BeiDou SSR Combined OrBIT,  and Clock Correction",
     "4076_104": "BeiDou SSR High Rate Clock Correction",
     "4076_105": "BeiDou SSR Code Bias",
     "4076_106": "BeiDou SSR Phase Bias",
     "4076_107": "BeiDou SSR URA",
     # "4076_108-120": "Reserved for BeiDou",
-    "4076_121": "SBAS SSR Orbit Correction",
+    "4076_121": "SBAS SSR OrBIT,  Correction",
     "4076_122": "SBAS SSR Clock Correction",
-    "4076_123": "SBAS SSR Combined Orbit and Clock Correction",
+    "4076_123": "SBAS SSR Combined OrBIT,  and Clock Correction",
     "4076_124": "SBAS SSR High Rate Clock Correction",
     "4076_125": "SBAS SSR Code Bias",
     "4076_126": "SBAS SSR Phase Bias",
     "4076_127": "SBAS SSR URA",
     # "4076_128-140": "Reserved for SBAS",
     # "4076_141-160": "Reserved for NavIC/IRNSS",
     # "4076_161-200": "Reserved",
```

### Comparing `pyrtcm-1.1.0/src/pyrtcm/socket_stream.py` & `pyrtcm-1.1.1/src/pyrtcm/socket_stream.py`

 * *Files identical despite different names*

### Comparing `pyrtcm-1.1.0/src/pyrtcm.egg-info/PKG-INFO` & `pyrtcm-1.1.1/src/pyrtcm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrtcm
-Version: 1.1.0
+Version: 1.1.1
 Summary: RTCM3 protocol parser
 Author-email: semuadmin <semuadmin@semuconsulting.com>
 Maintainer-email: semuadmin <semuadmin@semuconsulting.com>
 License: BSD 3-Clause License ("BSD License 2.0", "Revised BSD License", "New BSD License", or "Modified BSD License")
         
         Copyright (c) 2022, SEMU Consulting
         All rights reserved.
@@ -171,15 +171,16 @@
 Example -  Serial input:
 ```python
 from serial import Serial
 from pyrtcm import RTCMReader
 with Serial('/dev/tty.usbmodem14101', 9600, timeout=3) as stream:
   rtr = RTCMReader(stream)
   raw_data, parsed_data = rtr.read()
-  print(parsed_data)
+  if parsed_data is not None:
+    print(parsed_data)
 ```
 ```
 "<RTCM(1077, DF002=1077, DF003=0, DF004=204137001, DF393=1, DF409=0, DF001_7=0, ..., DF404_15=-9556, DF404_16=-2148, DF404_17=-2174)>",     
 ```
 
 Example - File input (using iterator).
 ```python
@@ -234,25 +235,21 @@
 ```
 
 Attributes within repeating groups are parsed with a two-digit suffix (`DF419_01`, `DF419_02`, etc. See [example below](#iterating) for an illustration of how to iterate through grouped attributes).
 
 Helper methods are available to interpret the individual datafields:
 
 ```python
-from pyrtcm import RTCM_DATA_FIELDS, datasiz, datascale, datadesc
+from pyrtcm import RTCM_DATA_FIELDS, datadesc
 dfname = "DF012"
 print(RTCM_DATA_FIELDS[dfname])
-print(datasiz(dfname))
-print(datascale(dfname))
 print(datadesc(dfname))
 ```
 ```
 (INT20, 0.0001, "GPS L1 PhaseRange - L1 Pseudorange")
-20
-0.0001
 'GPS L1 PhaseRange - L1 Pseudorange'
 ```
 
 The `payload` attribute always contains the raw payload as bytes.
 
 #### <a name="iterating">Iterating Through Group Attributes</a>
```

### Comparing `pyrtcm-1.1.0/src/pyrtcm.egg-info/SOURCES.txt` & `pyrtcm-1.1.1/src/pyrtcm.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 src/pyrtcm/exceptions.py
 src/pyrtcm/rtcmhelpers.py
 src/pyrtcm/rtcmmessage.py
 src/pyrtcm/rtcmreader.py
 src/pyrtcm/rtcmtables.py
 src/pyrtcm/rtcmtypes_core.py
 src/pyrtcm/rtcmtypes_get.py
+src/pyrtcm/rtcmtypes_get_igs.py
+src/pyrtcm/rtcmtypes_get_msm.py
 src/pyrtcm/socket_stream.py
 src/pyrtcm.egg-info/PKG-INFO
 src/pyrtcm.egg-info/SOURCES.txt
 src/pyrtcm.egg-info/dependency_links.txt
 src/pyrtcm.egg-info/requires.txt
 src/pyrtcm.egg-info/top_level.txt
 tests/test_definitions.py
```

### Comparing `pyrtcm-1.1.0/tests/test_definitions.py` & `pyrtcm-1.1.1/tests/test_definitions.py`

 * *Files 23% similar despite different names*

```diff
@@ -21,18 +21,19 @@
 class DefinitionTest(unittest.TestCase):
     def setUp(self):
         self.maxDiff = None
 
     def tearDown(self):
         pass
 
-    def testpayloaddfs(
-        self,
-    ):  # test all payload datafields are defined in RTCM_DATA_FIELDS
-        for _, pdict in RTCM_PAYLOADS_GET.items():
-            for df, _ in pdict.items():
-                if df[0:3] not in ("gro", "opt"):
-                    self.assertIn(df, RTCM_DATA_FIELDS)
+    # def testpayloaddfs(
+    #     self,
+    # ):  # test all payload datafields are defined in RTCM_DATA_FIELDS
+    #     for _, pdict in RTCM_PAYLOADS_GET.items():
+    #         for df, _ in pdict.items():
+    #             if df[0:3] not in ("gro", "opt"):
+    #                 self.assertIn(df, RTCM_DATA_FIELDS)
 
-    def testdfres(self):  # test all resolution values are int or float
-        for _, (_, res, _) in RTCM_DATA_FIELDS.items():
-            self.assertIsInstance(res, (int, float))
+    # def testdfres(self):  # test all size and resolution values are int or float
+    #     for _, (_, siz, res, _) in RTCM_DATA_FIELDS.items():
+    #         self.assertIsInstance(siz, (int, float))
+    #         self.assertIsInstance(res, (int, float))
```

### Comparing `pyrtcm-1.1.0/tests/test_socket.py` & `pyrtcm-1.1.1/tests/test_socket.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,14 +39,28 @@
             + b"\xD3\x00\x13\x3E\xD7\xD3\x02\x02\x98\x0E\xDE\xEF\x34\xB4\xBD\x62\xAC\x09\x41\x98\x6F\x33\x36\x0B\x98"
             + b"\xd3\x00\x13>\xd0\x00\x03\x8aX\xd9I<\x87/4\x10\x9d\x07\xd6\xafH Z\xd7\xf7"
             + b"\xd3\x00\x12B\x91\x81\xc9\x84\x00\x04B\xb8\x88\x008\x80\t\xd0F\x00(\xf0kf"
         )
         self._stream = pool * round(4096 / len(pool))
         self._buffer = self._stream
 
+    def __enter__(self):
+        """
+        Context manager enter routine.
+        """
+
+        return self
+
+    def __exit__(self, exc_type, exc_value, exc_traceback):
+        """
+        Context manager exit routine.
+        """
+
+        self.close()
+
     def recv(self, num: int) -> bytes:
         if self._timeout:
             raise TimeoutError
         if len(self._buffer) < num:
             self._buffer = self._buffer + self._stream
         buff = self._buffer[:num]
         self._buffer = self._buffer[num:]
@@ -76,48 +90,48 @@
             "<RTCM(1005, DF002=1005, DF003=0, DF021=0, DF022=1, DF023=1, DF024=1, DF141=0, DF025=4444030.802800001, DF142=1, DF001_1=0, DF026=3085671.2349, DF364=0, DF027=3366658.256)>",
             "<RTCM(1065, DF002=1065, DF386=12345, DF391=3, DF388=0, DF413=1, DF414=1, DF415=1, DF387=2, DF384_01=23, DF379_01=2, DF381_01_01=4, DF383_01_01=0.07, DF381_01_02=2, DF383_01_02=0.09, DF384_02=26, DF379_02=1, DF381_02_01=3, DF383_02_01=0.05)>",
             "<RTCM(1005, DF002=1005, DF003=2003, DF021=0, DF022=1, DF023=0, DF024=0, DF141=0, DF025=1114104.5999, DF142=0, DF001_1=0, DF026=-4850729.7108000005, DF364=0, DF027=3975521.4643)>",
             "<RTCM(1005, DF002=1005, DF003=0, DF021=0, DF022=1, DF023=1, DF024=1, DF141=0, DF025=4444030.802800001, DF142=1, DF001_1=0, DF026=3085671.2349, DF364=0, DF027=3366658.256)>",
             "<RTCM(1065, DF002=1065, DF386=12345, DF391=3, DF388=0, DF413=1, DF414=1, DF415=1, DF387=2, DF384_01=23, DF379_01=2, DF381_01_01=4, DF383_01_01=0.07, DF381_01_02=2, DF383_01_02=0.09, DF384_02=26, DF379_02=1, DF381_02_01=3, DF383_02_01=0.05)>",
         )
         raw = None
-        stream = DummySocket()
-        rtr = RTCMReader(stream, bufsize=512)
-        buff = rtr._stream.buffer  # test buffer getter method
-        i = 0
-        for raw, parsed in rtr:
-            if raw is not None:
-                # print(f'"{parsed},"')
-                self.assertEqual(str(parsed), EXPECTED_RESULTS[i])
-                i += 1
-                if i >= 12:
-                    break
+        with DummySocket() as stream:
+            rtr = RTCMReader(stream, bufsize=512)
+            buff = rtr._stream.buffer  # test buffer getter method
+            i = 0
+            for raw, parsed in rtr:
+                if raw is not None:
+                    # print(f'"{parsed},"')
+                    self.assertEqual(str(parsed), EXPECTED_RESULTS[i])
+                    i += 1
+                    if i >= 12:
+                        break
         self.assertEqual(i, 12)
 
     def testSocketIter(self):  # test for extended stream
         raw = None
-        stream = DummySocket()
-        rtr = RTCMReader(stream)
-        i = 0
-        for raw, parsed in rtr:
-            if raw is None:
-                raise EOFError
-            i += 1
-            if i >= 123:
-                break
+        with DummySocket() as stream:
+            rtr = RTCMReader(stream)
+            i = 0
+            for raw, parsed in rtr:
+                if raw is None:
+                    raise EOFError
+                i += 1
+                if i >= 123:
+                    break
         self.assertEqual(i, 123)
 
     def testSocketError(self):  # test for simulated socket timeout
         raw = None
-        stream = DummySocket(timeout=True)
-        rtr = RTCMReader(stream)
-        i = 0
-        for raw, parsed in rtr:
-            i += 1
-            if i >= 12:
-                break
+        with DummySocket(timeout=True) as stream:
+            rtr = RTCMReader(stream)
+            i = 0
+            for raw, parsed in rtr:
+                i += 1
+                if i >= 12:
+                    break
         self.assertEqual(i, 0)
 
 
 if __name__ == "__main__":
     # import sys;sys.argv = ['', 'Test.testName']
     unittest.main()
```

### Comparing `pyrtcm-1.1.0/tests/test_stream.py` & `pyrtcm-1.1.1/tests/test_stream.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,31 +7,38 @@
 
 @author: semuadmin
 """
 
 # pylint: disable=line-too-long, invalid-name, missing-docstring, no-member
 
 import os
+from io import BufferedReader
 import sys
 import unittest
+from logging import ERROR
 
 from io import StringIO
 from pyrtcm import (
     RTCMReader,
     RTCMMessage,
     RTCMParseError,
     RTCMMessageError,
+    ERR_IGNORE,
+    ERR_LOG,
+    ERR_RAISE,
 )
 import pyrtcm.rtcmtypes_core as rtt
 
+DIRNAME = os.path.dirname(__file__)
+
 
 class StreamTest(unittest.TestCase):
     def setUp(self):
         self.maxDiff = None
-        dirname = os.path.dirname(__file__)
+
         self._raw1005ex = b"\xD3\x00\x13\x3E\xD7\xD3\x02\x02\x98\x0E\xDE\xEF\x34\xB4\xBD\x62\xAC\x09\x41\x98\x6F\x33\x36\x0B\x98"
         self._raw1005 = (
             b"\xd3\x00\x13>\xd0\x00\x03\x8aX\xd9I<\x87/4\x10\x9d\x07\xd6\xafH Z\xd7\xf7"
         )
         self._raw1007 = b"\xd3\x00\x08>\xf4\xd2\x03ABC\xeapo\xc7"
         # 00111110 11110100 11010010 00000011 01000001 01000010 01000011 11101010
         self._raw1065 = (
@@ -110,41 +117,17 @@
             rtr = RTCMReader(stream, quitonerror=2)
             i = 0
             for raw, parsed in rtr:
                 # print(f'"{parsed}",')
                 self.assertEqual(str(parsed), EXPECTED_RESULT[i])
                 i += 1
             self.assertEqual(i, 3)
-
-    def testMIXEDRTCM_NOSCALE(
-        self,
-    ):  # test mixed stream of NMEA, UBX & RTCM messages with no scaling applied
-        EXPECTED_RESULTS = (
-            "<RTCM(1005, DF002=1005, DF003=0, DF021=0, DF022=1, DF023=1, DF024=1, DF141=0, DF025=44440308028, DF142=1, DF001_1=0, DF026=30856712349, DF364=0, DF027=33666582560)>",
-            "<RTCM(4072, DF002=4072, Not_Yet_Implemented)>",
-            "<RTCM(1077, DF002=1077, DF003=0, DF004=204137001, DF393=1, DF409=0, DF001_7=0, DF411=0, DF412=0, DF417=0, DF418=0, DF394=760738918298550272, NSat=10, DF395=1073807360, NSig=2, DF396=1044459, NCell=17, PRN_01=005, PRN_02=007, PRN_03=009, PRN_04=013, PRN_05=014, PRN_06=015, PRN_07=017, PRN_08=019, PRN_09=020, PRN_10=030, DF397_01=75, DF397_02=75, DF397_03=81, DF397_04=72, DF397_05=67, DF397_06=80, DF397_07=75, DF397_08=82, DF397_09=75, DF397_10=71, ExtSatInfo_01=0, ExtSatInfo_02=0, ExtSatInfo_03=0, ExtSatInfo_04=0, ExtSatInfo_05=0, ExtSatInfo_06=0, ExtSatInfo_07=0, ExtSatInfo_08=0, ExtSatInfo_09=0, ExtSatInfo_10=0, DF398_01=6, DF398_02=547, DF398_03=781, DF398_04=142, DF398_05=563, DF398_06=116, DF398_07=823, DF398_08=105, DF398_09=534, DF398_10=354, DF399_01=-178, DF399_02=-304, DF399_03=-643, DF399_04=477, DF399_05=-52, DF399_06=645, DF399_07=529, DF399_08=643, DF399_09=-428, DF399_10=-181, CELLPRN_01=005, CELLSIG_01=1C, CELLPRN_02=005, CELLSIG_02=2L, CELLPRN_03=007, CELLSIG_03=1C, CELLPRN_04=007, CELLSIG_04=2L, CELLPRN_05=009, CELLSIG_05=1C, CELLPRN_06=009, CELLSIG_06=2L, CELLPRN_07=013, CELLSIG_07=1C, CELLPRN_08=014, CELLSIG_08=1C, CELLPRN_09=014, CELLSIG_09=2L, CELLPRN_10=015, CELLSIG_10=1C, CELLPRN_11=015, CELLSIG_11=2L, CELLPRN_12=017, CELLSIG_12=1C, CELLPRN_13=017, CELLSIG_13=2L, CELLPRN_14=019, CELLSIG_14=1C, CELLPRN_15=020, CELLSIG_15=1C, CELLPRN_16=030, CELLSIG_16=1C, CELLPRN_17=030, CELLSIG_17=2L, DF405_01=76821, DF405_02=76146, DF405_03=208482, DF405_04=207990, DF405_05=-259757, DF405_06=-251705, DF405_07=186759, DF405_08=117947, DF405_09=115540, DF405_10=-101213, DF405_11=-98350, DF405_12=-54158, DF405_13=-52852, DF405_14=257029, DF405_15=234424, DF405_16=-166735, DF405_17=-165708, DF406_01=304801, DF406_02=307946, DF406_03=838384, DF406_04=832000, DF406_05=-1040227, DF406_06=-1005568, DF406_07=745973, DF406_08=467269, DF406_09=463801, DF406_10=-400680, DF406_11=-394066, DF406_12=-214602, DF406_13=-208840, DF406_14=886532, DF406_15=935439, DF406_16=-668448, DF406_17=-663545, DF407_01=341, DF407_02=341, DF407_03=341, DF407_04=341, DF407_05=341, DF407_06=341, DF407_07=341, DF407_08=341, DF407_09=341, DF407_10=341, DF407_11=341, DF407_12=341, DF407_13=341, DF407_14=295, DF407_15=341, DF407_16=341, DF407_17=341, DF420_01=0, DF420_02=0, DF420_03=0, DF420_04=0, DF420_05=0, DF420_06=0, DF420_07=0, DF420_08=0, DF420_09=0, DF420_10=0, DF420_11=0, DF420_12=0, DF420_13=0, DF420_14=0, DF420_15=0, DF420_16=0, DF420_17=0, DF408_01=720, DF408_02=608, DF408_03=688, DF408_04=624, DF408_05=624, DF408_06=592, DF408_07=720, DF408_08=736, DF408_09=736, DF408_10=624, DF408_11=544, DF408_12=720, DF408_13=608, DF408_14=496, DF408_15=720, DF408_16=736, DF408_17=656, DF404_01=-9231, DF404_02=-9194, DF404_03=-8321, DF404_04=-8326, DF404_05=-4107, DF404_06=-4072, DF404_07=2451, DF404_08=-693, DF404_09=-684, DF404_10=9390, DF404_11=9417, DF404_12=2384, DF404_13=2416, DF404_14=6636, DF404_15=-9556, DF404_16=-2148, DF404_17=-2174)>",
-            "<RTCM(1087, DF002=1087, DF003=0, DF416=2, DF034=42119001, DF393=1, DF409=0, DF001_7=0, DF411=0, DF412=0, DF417=0, DF418=0, DF394=4039168114821169152, NSat=7, DF395=1090519040, NSig=2, DF396=16382, NCell=13, PRN_01=003, PRN_02=004, PRN_03=005, PRN_04=013, PRN_05=014, PRN_06=015, PRN_07=023, DF397_01=69, DF397_02=64, DF397_03=73, DF397_04=76, DF397_05=66, DF397_06=70, DF397_07=78, DF419_01=12, DF419_02=13, DF419_03=8, DF419_04=5, DF419_05=0, DF419_06=7, DF419_07=10, DF398_01=649, DF398_02=351, DF398_03=260, DF398_04=318, DF398_05=525, DF398_06=847, DF398_07=905, DF399_01=-665, DF399_02=29, DF399_03=672, DF399_04=-573, DF399_05=-211, DF399_06=312, DF399_07=317, CELLPRN_01=003, CELLSIG_01=1C, CELLPRN_02=003, CELLSIG_02=2C, CELLPRN_03=004, CELLSIG_03=1C, CELLPRN_04=004, CELLSIG_04=2C, CELLPRN_05=005, CELLSIG_05=1C, CELLPRN_06=005, CELLSIG_06=2C, CELLPRN_07=013, CELLSIG_07=1C, CELLPRN_08=013, CELLSIG_08=2C, CELLPRN_09=014, CELLSIG_09=1C, CELLPRN_10=014, CELLSIG_10=2C, CELLPRN_11=015, CELLSIG_11=1C, CELLPRN_12=015, CELLSIG_12=2C, CELLPRN_13=023, CELLSIG_13=1C, DF405_01=133875, DF405_02=134842, DF405_03=-25120, DF405_04=-27605, DF405_05=5983, DF405_06=11545, DF405_07=252755, DF405_08=257427, DF405_09=-208262, DF405_10=-201884, DF405_11=148812, DF405_12=154159, DF405_13=-126765, DF406_01=535524, DF406_02=538534, DF406_03=-103820, DF406_04=-110050, DF406_05=23943, DF406_06=46822, DF406_07=1009883, DF406_08=1041159, DF406_09=-832392, DF406_10=-807014, DF406_11=596748, DF406_12=618626, DF406_13=-508918, DF407_01=341, DF407_02=341, DF407_03=340, DF407_04=340, DF407_05=341, DF407_06=341, DF407_07=340, DF407_08=341, DF407_09=341, DF407_10=341, DF407_11=341, DF407_12=341, DF407_13=340, DF420_01=0, DF420_02=0, DF420_03=0, DF420_04=0, DF420_05=0, DF420_06=0, DF420_07=0, DF420_08=0, DF420_09=0, DF420_10=0, DF420_11=0, DF420_12=0, DF420_13=0, DF408_01=752, DF408_02=640, DF408_03=752, DF408_04=672, DF408_05=752, DF408_06=624, DF408_07=576, DF408_08=528, DF408_09=768, DF408_10=688, DF408_11=768, DF408_12=640, DF408_13=656, DF404_01=-8193, DF404_02=-8173, DF404_03=8539, DF404_04=8501, DF404_05=7333, DF404_06=7311, DF404_07=-2493, DF404_08=-2543, DF404_09=-2158, DF404_10=-2178, DF404_11=3924, DF404_12=3947, DF404_13=6146)>",
-            "<RTCM(1097, DF002=1097, DF003=0, DF248=204137001, DF393=1, DF409=0, DF001_7=0, DF411=0, DF412=0, DF417=0, DF418=0, DF394=216181732825628672, NSat=5, DF395=1073872896, NSig=2, DF396=1023, NCell=10, PRN_01=007, PRN_02=008, PRN_03=021, PRN_04=027, PRN_05=030, DF397_01=79, DF397_02=84, DF397_03=89, DF397_04=78, DF397_05=83, ExtSatInfo_01=0, ExtSatInfo_02=0, ExtSatInfo_03=0, ExtSatInfo_04=0, ExtSatInfo_05=0, DF398_01=160, DF398_02=257, DF398_03=363, DF398_04=380, DF398_05=266, DF399_01=-198, DF399_02=-516, DF399_03=423, DF399_04=63, DF399_05=-384, CELLPRN_01=007, CELLSIG_01=1C, CELLPRN_02=007, CELLSIG_02=7Q, CELLPRN_03=008, CELLSIG_03=1C, CELLPRN_04=008, CELLSIG_04=7Q, CELLPRN_05=021, CELLSIG_05=1C, CELLPRN_06=021, CELLSIG_06=7Q, CELLPRN_07=027, CELLSIG_07=1C, CELLPRN_08=027, CELLSIG_08=7Q, CELLPRN_09=030, CELLSIG_09=1C, CELLPRN_10=030, CELLSIG_10=7Q, DF405_01=-24373, DF405_02=-15168, DF405_03=-185743, DF405_04=-175463, DF405_05=258219, DF405_06=269106, DF405_07=-73530, DF405_08=-67668, DF405_09=-9900, DF405_10=-1633, DF406_01=-95448, DF406_02=-60891, DF406_03=-757091, DF406_04=-700882, DF406_05=1035170, DF406_06=1075556, DF406_07=-295430, DF406_08=-271348, DF406_09=-38736, DF406_10=-7071, DF407_01=341, DF407_02=341, DF407_03=341, DF407_04=341, DF407_05=341, DF407_06=341, DF407_07=341, DF407_08=341, DF407_09=341, DF407_10=341, DF420_01=0, DF420_02=0, DF420_03=0, DF420_04=0, DF420_05=0, DF420_06=0, DF420_07=0, DF420_08=0, DF420_09=0, DF420_10=0, DF408_01=736, DF408_02=784, DF408_03=656, DF408_04=688, DF408_05=688, DF408_06=688, DF408_07=720, DF408_08=784, DF408_09=688, DF408_10=752, DF404_01=-5806, DF404_02=-5831, DF404_03=-7947, DF404_04=-7943, DF404_05=7243, DF404_06=7174, DF404_07=5534, DF404_08=5545, DF404_09=-7726, DF404_10=-7733)>",
-            "<RTCM(1127, DF002=1127, DF003=0, DF427=204123001, DF393=0, DF409=0, DF001_7=0, DF411=0, DF412=0, DF417=0, DF418=0, DF394=198178247981137920, NSat=10, DF395=1074003968, NSig=2, DF396=387754, NCell=11, PRN_01=007, PRN_02=009, PRN_03=010, PRN_04=020, PRN_05=023, PRN_06=028, PRN_07=032, PRN_08=037, PRN_09=040, PRN_10=043, DF397_01=129, DF397_02=132, DF397_03=126, DF397_04=75, DF397_05=81, DF397_06=84, DF397_07=78, DF397_08=74, DF397_09=130, DF397_10=86, ExtSatInfo_01=0, ExtSatInfo_02=0, ExtSatInfo_03=0, ExtSatInfo_04=0, ExtSatInfo_05=0, ExtSatInfo_06=0, ExtSatInfo_07=0, ExtSatInfo_08=0, ExtSatInfo_09=0, ExtSatInfo_10=0, DF398_01=120, DF398_02=493, DF398_03=317, DF398_04=743, DF398_05=420, DF398_06=584, DF398_07=573, DF398_08=330, DF398_09=592, DF398_10=690, DF399_01=-130, DF399_02=-58, DF399_03=-81, DF399_04=32, DF399_05=-398, DF399_06=436, DF399_07=-523, DF399_08=-65, DF399_09=-182, DF399_10=79, CELLPRN_01=007, CELLSIG_01=7I, CELLPRN_02=009, CELLSIG_02=7I, CELLPRN_03=010, CELLSIG_03=2I, CELLPRN_04=010, CELLSIG_04=7I, CELLPRN_05=020, CELLSIG_05=2I, CELLPRN_06=023, CELLSIG_06=2I, CELLPRN_07=028, CELLSIG_07=2I, CELLPRN_08=032, CELLSIG_08=2I, CELLPRN_09=037, CELLSIG_09=2I, CELLPRN_10=040, CELLSIG_10=2I, CELLPRN_11=043, CELLSIG_11=2I, DF405_01=-208596, DF405_02=122033, DF405_03=216714, DF405_04=212638, DF405_05=-89572, DF405_06=-25529, DF405_07=197283, DF405_08=142968, DF405_09=-134357, DF405_10=-63371, DF405_11=-157715, DF406_01=-833669, DF406_02=486390, DF406_03=865861, DF406_04=851310, DF406_05=-358508, DF406_06=-104126, DF406_07=793957, DF406_08=569965, DF406_09=-539350, DF406_10=-254868, DF406_11=-633415, DF407_01=341, DF407_02=341, DF407_03=341, DF407_04=341, DF407_05=341, DF407_06=341, DF407_07=341, DF407_08=341, DF407_09=341, DF407_10=341, DF407_11=341, DF420_01=0, DF420_02=0, DF420_03=0, DF420_04=0, DF420_05=0, DF420_06=0, DF420_07=0, DF420_08=0, DF420_09=0, DF420_10=0, DF420_11=0, DF408_01=720, DF408_02=656, DF408_03=672, DF408_04=720, DF408_05=768, DF408_06=736, DF408_07=672, DF408_08=752, DF408_09=768, DF408_10=704, DF408_11=688, DF404_01=-5674, DF404_02=-6120, DF404_03=-1384, DF404_04=-1332, DF404_05=5992, DF404_06=-7312, DF404_07=1732, DF404_08=-4308, DF404_09=-5975, DF404_10=-6733, DF404_11=6122)>",
-            "<RTCM(1230, DF002=1230, DF003=0, DF421=1, DF001_3=0, DF422_1=0, DF422_2=0, DF422_3=0, DF422_4=0)>",
-            "<RTCM(1007, DF002=1007, DF003=1234, DF029=3, DF030_01=A, DF030_02=B, DF030_03=C, DF031=234)>",
-            "<RTCM(1117, DF002=1117, DF003=0, DF428=385820000, DF393=1, DF409=0, DF001_7=0, DF411=1, DF412=0, DF417=0, DF418=0, DF394=7061644215716937728, NSat=3, DF395=1073774849, NSig=4, DF396=4095, NCell=12, PRN_01=194, PRN_02=195, PRN_03=199, DF397_01=140, DF397_02=112, DF397_03=133, ExtSatInfo_01=0, ExtSatInfo_02=0, ExtSatInfo_03=0, DF398_01=176, DF398_02=128, DF398_03=893, DF399_01=481, DF399_02=-28, DF399_03=1, CELLPRN_01=194, CELLSIG_01=1C, CELLPRN_02=194, CELLSIG_02=2X, CELLPRN_03=194, CELLSIG_03=5X, CELLPRN_04=194, CELLSIG_04=1X, CELLPRN_05=195, CELLSIG_05=1C, CELLPRN_06=195, CELLSIG_06=2X, CELLPRN_07=195, CELLSIG_07=5X, CELLPRN_08=195, CELLSIG_08=1X, CELLPRN_09=199, CELLSIG_09=1C, CELLPRN_10=199, CELLSIG_10=2X, CELLPRN_11=199, CELLSIG_11=5X, CELLPRN_12=199, CELLSIG_12=1X, DF405_01=121518, DF405_02=141210, DF405_03=131740, DF405_04=123624, DF405_05=-20668, DF405_06=-4471, DF405_07=-12126, DF405_08=-17656, DF405_09=-52645, DF405_10=-38454, DF405_11=-46050, DF405_12=-51391, DF406_01=-471984, DF406_02=1075651, DF406_03=-8483, DF406_04=476711, DF406_05=837780, DF406_06=-367061, DF406_07=-358394, DF406_08=-404031, DF406_09=610251, DF406_10=-420698, DF406_11=441746, DF406_12=381254, DF407_01=516, DF407_02=462, DF407_03=684, DF407_04=365, DF407_05=648, DF407_06=649, DF407_07=649, DF407_08=649, DF407_09=568, DF407_10=704, DF407_11=704, DF407_12=704, DF420_01=0, DF420_02=0, DF420_03=0, DF420_04=0, DF420_05=0, DF420_06=0, DF420_07=0, DF420_08=0, DF420_09=0, DF420_10=0, DF420_11=0, DF420_12=0, DF408_01=485, DF408_02=574, DF408_03=552, DF408_04=552, DF408_05=778, DF408_06=808, DF408_07=842, DF408_08=819, DF408_09=613, DF408_10=699, DF408_11=733, DF408_12=645, DF404_01=-1064, DF404_02=-16384, DF404_03=-16384, DF404_04=-16384, DF404_05=-5875, DF404_06=-16384, DF404_07=-16384, DF404_08=-16384, DF404_09=-4130, DF404_10=-16384, DF404_11=-16384, DF404_12=-16384)>",
-        )
-
-        dirname = os.path.dirname(__file__)
-        with open(os.path.join(dirname, "pygpsdata-RTCM3.log"), "rb") as stream:
-            i = 0
-            raw = 0
-            rtr = RTCMReader(stream, scaling=False)
-            for raw, parsed in rtr:
-                if raw is not None:
-                    # print(f'"{parsed}",')
-                    self.assertEqual(str(parsed), EXPECTED_RESULTS[i])
-                    i += 1
-        self.assertEqual(i, 9)
+            self.assertIsInstance(
+                rtr.datastream, BufferedReader
+            )  # test datastream getter
 
     def testMIXEDRTCM_SCALE(
         self,
     ):  # test mixed stream of NMEA, UBX & RTCM messages with scaling applied
         EXPECTED_RESULTS = (
             "<RTCM(1005, DF002=1005, DF003=0, DF021=0, DF022=1, DF023=1, DF024=1, DF141=0, DF025=4444030.802800001, DF142=1, DF001_1=0, DF026=3085671.2349, DF364=0, DF027=3366658.256)>",
             "<RTCM(4072, DF002=4072, Not_Yet_Implemented)>",
@@ -156,15 +139,15 @@
             "<RTCM(1007, DF002=1007, DF003=1234, DF029=3, DF030_01=A, DF030_02=B, DF030_03=C, DF031=234)>",
             "<RTCM(1117, DF002=1117, DF003=0, DF428=385820000, DF393=1, DF409=0, DF001_7=0, DF411=1, DF412=0, DF417=0, DF418=0, DF394=7061644215716937728, NSat=3, DF395=1073774849, NSig=4, DF396=4095, NCell=12, PRN_01=194, PRN_02=195, PRN_03=199, DF397_01=140, DF397_02=112, DF397_03=133, ExtSatInfo_01=0, ExtSatInfo_02=0, ExtSatInfo_03=0, DF398_01=0.171875, DF398_02=0.125, DF398_03=0.8720703125, DF399_01=481, DF399_02=-28, DF399_03=1, CELLPRN_01=194, CELLSIG_01=1C, CELLPRN_02=194, CELLSIG_02=2X, CELLPRN_03=194, CELLSIG_03=5X, CELLPRN_04=194, CELLSIG_04=1X, CELLPRN_05=195, CELLSIG_05=1C, CELLPRN_06=195, CELLSIG_06=2X, CELLPRN_07=195, CELLSIG_07=5X, CELLPRN_08=195, CELLSIG_08=1X, CELLPRN_09=199, CELLSIG_09=1C, CELLPRN_10=199, CELLSIG_10=2X, CELLPRN_11=199, CELLSIG_11=5X, CELLPRN_12=199, CELLSIG_12=1X, DF405_01=0.00022634491324424744, DF405_02=0.00026302412152290344, DF405_03=0.0002453848719596863, DF405_04=0.00023026764392852783, DF405_05=-3.849714994430542e-05, DF405_06=-8.327886462211609e-06, DF405_07=-2.2586435079574585e-05, DF405_08=-3.288686275482178e-05, DF405_09=-9.805895388126373e-05, DF405_10=-7.162615656852722e-05, DF405_11=-8.577480912208557e-05, DF405_12=-9.572319686412811e-05, DF406_01=-0.000219784677028656, DF406_02=0.000500889029353857, DF406_03=-3.950204700231552e-06, DF406_04=0.0002219858579337597, DF406_05=0.0003901217132806778, DF406_06=-0.00017092609778046608, DF406_07=-0.0001668902114033699, DF406_08=-0.0001881415955722332, DF406_09=0.0002841702662408352, DF406_10=-0.0001959027722477913, DF406_11=0.00020570401102304459, DF406_12=0.00017753522843122482, DF407_01=516, DF407_02=462, DF407_03=684, DF407_04=365, DF407_05=648, DF407_06=649, DF407_07=649, DF407_08=649, DF407_09=568, DF407_10=704, DF407_11=704, DF407_12=704, DF420_01=0, DF420_02=0, DF420_03=0, DF420_04=0, DF420_05=0, DF420_06=0, DF420_07=0, DF420_08=0, DF420_09=0, DF420_10=0, DF420_11=0, DF420_12=0, DF408_01=30.3125, DF408_02=35.875, DF408_03=34.5, DF408_04=34.5, DF408_05=48.625, DF408_06=50.5, DF408_07=52.625, DF408_08=51.1875, DF408_09=38.3125, DF408_10=43.6875, DF408_11=45.8125, DF408_12=40.3125, DF404_01=-0.10640000000000001, DF404_02=-1.6384, DF404_03=-1.6384, DF404_04=-1.6384, DF404_05=-0.5875, DF404_06=-1.6384, DF404_07=-1.6384, DF404_08=-1.6384, DF404_09=-0.41300000000000003, DF404_10=-1.6384, DF404_11=-1.6384, DF404_12=-1.6384)>",
         )
         dirname = os.path.dirname(__file__)
         with open(os.path.join(dirname, "pygpsdata-RTCM3.log"), "rb") as stream:
             i = 0
             raw = 0
-            rtr = RTCMReader(stream, scaling=True)
+            rtr = RTCMReader(stream)
             for raw, parsed in rtr:
                 if raw is not None:
                     # print(f'"{parsed}",')
                     self.assertEqual(str(parsed), EXPECTED_RESULTS[i])
                     i += 1
         self.assertEqual(i, 9)
 
@@ -183,17 +166,15 @@
             "<RTCM(1117, DF002=1117, DF003=0, DF428=385820000, DF393=1, DF409=0, DF001_7=0, DF411=1, DF412=0, DF417=0, DF418=0, DF394=7061644215716937728, NSat=3, DF395=1073774849, NSig=4, DF396=4095, NCell=12, PRN_01=194, PRN_02=195, PRN_03=199, DF397_01=140, DF397_02=112, DF397_03=133, ExtSatInfo_01=0, ExtSatInfo_02=0, ExtSatInfo_03=0, DF398_01=0.171875, DF398_02=0.125, DF398_03=0.8720703125, DF399_01=481, DF399_02=-28, DF399_03=1, CELLPRN_01=194, CELLSIG_01=1C, CELLPRN_02=194, CELLSIG_02=2X, CELLPRN_03=194, CELLSIG_03=5X, CELLPRN_04=194, CELLSIG_04=1X, CELLPRN_05=195, CELLSIG_05=1C, CELLPRN_06=195, CELLSIG_06=2X, CELLPRN_07=195, CELLSIG_07=5X, CELLPRN_08=195, CELLSIG_08=1X, CELLPRN_09=199, CELLSIG_09=1C, CELLPRN_10=199, CELLSIG_10=2X, CELLPRN_11=199, CELLSIG_11=5X, CELLPRN_12=199, CELLSIG_12=1X, DF405_01=0.00022634491324424744, DF405_02=0.00026302412152290344, DF405_03=0.0002453848719596863, DF405_04=0.00023026764392852783, DF405_05=-3.849714994430542e-05, DF405_06=-8.327886462211609e-06, DF405_07=-2.2586435079574585e-05, DF405_08=-3.288686275482178e-05, DF405_09=-9.805895388126373e-05, DF405_10=-7.162615656852722e-05, DF405_11=-8.577480912208557e-05, DF405_12=-9.572319686412811e-05, DF406_01=-0.000219784677028656, DF406_02=0.000500889029353857, DF406_03=-3.950204700231552e-06, DF406_04=0.0002219858579337597, DF406_05=0.0003901217132806778, DF406_06=-0.00017092609778046608, DF406_07=-0.0001668902114033699, DF406_08=-0.0001881415955722332, DF406_09=0.0002841702662408352, DF406_10=-0.0001959027722477913, DF406_11=0.00020570401102304459, DF406_12=0.00017753522843122482, DF407_01=516, DF407_02=462, DF407_03=684, DF407_04=365, DF407_05=648, DF407_06=649, DF407_07=649, DF407_08=649, DF407_09=568, DF407_10=704, DF407_11=704, DF407_12=704, DF420_01=0, DF420_02=0, DF420_03=0, DF420_04=0, DF420_05=0, DF420_06=0, DF420_07=0, DF420_08=0, DF420_09=0, DF420_10=0, DF420_11=0, DF420_12=0, DF408_01=30.3125, DF408_02=35.875, DF408_03=34.5, DF408_04=34.5, DF408_05=48.625, DF408_06=50.5, DF408_07=52.625, DF408_08=51.1875, DF408_09=38.3125, DF408_10=43.6875, DF408_11=45.8125, DF408_12=40.3125, DF404_01=-0.10640000000000001, DF404_02=-1.6384, DF404_03=-1.6384, DF404_04=-1.6384, DF404_05=-0.5875, DF404_06=-1.6384, DF404_07=-1.6384, DF404_08=-1.6384, DF404_09=-0.41300000000000003, DF404_10=-1.6384, DF404_11=-1.6384, DF404_12=-1.6384)>",
         )
 
         dirname = os.path.dirname(__file__)
         with open(os.path.join(dirname, "pygpsdata-RTCM3.log"), "rb") as stream:
             i = 0
             raw = 0
-            rtr = RTCMReader(
-                stream, scaling=True, labelmsm=True, quitonerror=rtt.ERR_RAISE
-            )
+            rtr = RTCMReader(stream, labelmsm=True, quitonerror=rtt.ERR_RAISE)
             for raw, parsed in rtr:
                 if raw is not None:
                     # print(f'"{parsed}",')
                     self.assertEqual(str(parsed), EXPECTED_RESULTS[i])
                     i += 1
         self.assertEqual(i, 9)
 
@@ -212,17 +193,15 @@
             "<RTCM(1117, DF002=1117, DF003=0, DF428=385820000, DF393=1, DF409=0, DF001_7=0, DF411=1, DF412=0, DF417=0, DF418=0, DF394=7061644215716937728, NSat=3, DF395=1073774849, NSig=4, DF396=4095, NCell=12, PRN_01=194, PRN_02=195, PRN_03=199, DF397_01=140, DF397_02=112, DF397_03=133, ExtSatInfo_01=0, ExtSatInfo_02=0, ExtSatInfo_03=0, DF398_01=0.171875, DF398_02=0.125, DF398_03=0.8720703125, DF399_01=481, DF399_02=-28, DF399_03=1, CELLPRN_01=194, CELLSIG_01=L1, CELLPRN_02=194, CELLSIG_02=L2, CELLPRN_03=194, CELLSIG_03=L5, CELLPRN_04=194, CELLSIG_04=L1, CELLPRN_05=195, CELLSIG_05=L1, CELLPRN_06=195, CELLSIG_06=L2, CELLPRN_07=195, CELLSIG_07=L5, CELLPRN_08=195, CELLSIG_08=L1, CELLPRN_09=199, CELLSIG_09=L1, CELLPRN_10=199, CELLSIG_10=L2, CELLPRN_11=199, CELLSIG_11=L5, CELLPRN_12=199, CELLSIG_12=L1, DF405_01=0.00022634491324424744, DF405_02=0.00026302412152290344, DF405_03=0.0002453848719596863, DF405_04=0.00023026764392852783, DF405_05=-3.849714994430542e-05, DF405_06=-8.327886462211609e-06, DF405_07=-2.2586435079574585e-05, DF405_08=-3.288686275482178e-05, DF405_09=-9.805895388126373e-05, DF405_10=-7.162615656852722e-05, DF405_11=-8.577480912208557e-05, DF405_12=-9.572319686412811e-05, DF406_01=-0.000219784677028656, DF406_02=0.000500889029353857, DF406_03=-3.950204700231552e-06, DF406_04=0.0002219858579337597, DF406_05=0.0003901217132806778, DF406_06=-0.00017092609778046608, DF406_07=-0.0001668902114033699, DF406_08=-0.0001881415955722332, DF406_09=0.0002841702662408352, DF406_10=-0.0001959027722477913, DF406_11=0.00020570401102304459, DF406_12=0.00017753522843122482, DF407_01=516, DF407_02=462, DF407_03=684, DF407_04=365, DF407_05=648, DF407_06=649, DF407_07=649, DF407_08=649, DF407_09=568, DF407_10=704, DF407_11=704, DF407_12=704, DF420_01=0, DF420_02=0, DF420_03=0, DF420_04=0, DF420_05=0, DF420_06=0, DF420_07=0, DF420_08=0, DF420_09=0, DF420_10=0, DF420_11=0, DF420_12=0, DF408_01=30.3125, DF408_02=35.875, DF408_03=34.5, DF408_04=34.5, DF408_05=48.625, DF408_06=50.5, DF408_07=52.625, DF408_08=51.1875, DF408_09=38.3125, DF408_10=43.6875, DF408_11=45.8125, DF408_12=40.3125, DF404_01=-0.10640000000000001, DF404_02=-1.6384, DF404_03=-1.6384, DF404_04=-1.6384, DF404_05=-0.5875, DF404_06=-1.6384, DF404_07=-1.6384, DF404_08=-1.6384, DF404_09=-0.41300000000000003, DF404_10=-1.6384, DF404_11=-1.6384, DF404_12=-1.6384)>",
         )
 
         dirname = os.path.dirname(__file__)
         with open(os.path.join(dirname, "pygpsdata-RTCM3.log"), "rb") as stream:
             i = 0
             raw = 0
-            rtr = RTCMReader(
-                stream, scaling=True, labelmsm=2, quitonerror=rtt.ERR_RAISE
-            )
+            rtr = RTCMReader(stream, labelmsm=2, quitonerror=rtt.ERR_RAISE)
             for raw, parsed in rtr:
                 if raw is not None:
                     # print(f'"{parsed}",')
                     self.assertEqual(str(parsed), EXPECTED_RESULTS[i])
                     i += 1
         self.assertEqual(i, 9)
 
@@ -268,15 +247,15 @@
         ]
         dirname = os.path.dirname(__file__)
         with open(
             os.path.join(dirname, "pygpsdata-NTRIP-USCL00CHL0.log"), "rb"
         ) as stream:
             i = 0
             raw = 0
-            rtr = RTCMReader(stream, scaling=True, labelmsm=True)
+            rtr = RTCMReader(stream, labelmsm=True)
             for raw, parsed in rtr:
                 if raw is not None:
                     # print(f'"{parsed}",')
                     self.assertEqual(f"{parsed}", EXPECTED_RESULTS[i])
                     i += 1
         self.assertEqual(i, 35)
 
@@ -296,15 +275,15 @@
             "<RTCM(4076_025, DF002=4076, IDF001=3, IDF002=25, IDF003=311130, IDF004=3, IDF005=0, IDF007=1, IDF008=0, IDF009=2, IDF010=31, IDF011_01=2, IDF023_01=3, IDF024_01_01=0, IDF025_01_01=-3.3200000000000003, IDF024_01_02=2, IDF025_01_02=-3.87, IDF024_01_03=11, IDF025_01_03=-6.37, IDF011_02=3, IDF023_02=7, IDF024_02_01=0, IDF025_02_01=1.85, IDF024_02_02=2, IDF025_02_02=2.23, IDF024_02_03=5, IDF025_02_03=3.87, IDF024_02_04=8, IDF025_02_04=3.88, IDF024_02_05=7, IDF025_02_05=3.8000000000000003, IDF024_02_06=11, IDF025_02_06=3.68, IDF024_02_07=15, IDF025_02_07=1.53, IDF011_03=4, IDF023_03=7, IDF024_03_01=0, IDF025_03_01=-0.01, IDF024_03_02=2, IDF025_03_02=0.2, IDF024_03_03=5, IDF025_03_03=0.14, IDF024_03_04=8, IDF025_03_04=0.13, IDF024_03_05=7, IDF025_03_05=0.15, IDF024_03_06=11, IDF025_03_06=0.34, IDF024_03_07=15, IDF025_03_07=1.71, IDF011_04=5, IDF023_04=6, IDF024_04_01=0, IDF025_04_01=-2.12, IDF024_04_02=2, IDF025_04_02=-1.8900000000000001, IDF024_04_03=5, IDF025_04_03=-2.97, IDF024_04_04=8, IDF025_04_04=-2.97, IDF024_04_05=7, IDF025_04_05=-2.87, IDF024_04_06=11, IDF025_04_06=-3.11, IDF011_05=6, IDF023_05=7, IDF024_05_01=0, IDF025_05_01=2.74, IDF024_05_02=2, IDF025_05_02=3.12, IDF024_05_03=5, IDF025_05_03=5.47, IDF024_05_04=8, IDF025_05_04=5.46, IDF024_05_05=7, IDF025_05_05=5.41, IDF024_05_06=11, IDF025_05_06=5.13, IDF024_05_07=15, IDF025_05_07=3.35, IDF011_06=7, IDF023_06=6, IDF024_06_01=0, IDF025_06_01=-1.82, IDF024_06_02=2, IDF025_06_02=-1.75, IDF024_06_03=5, IDF025_06_03=-2.99, IDF024_06_04=8, IDF025_06_04=-3.0, IDF024_06_05=7, IDF025_06_05=-2.94, IDF024_06_06=11, IDF025_06_06=-2.88, IDF011_07=8, IDF023_07=7, IDF024_07_01=0, IDF025_07_01=3.08, IDF024_07_02=2, IDF025_07_02=3.0100000000000002, IDF024_07_03=5, IDF025_07_03=5.36, IDF024_07_04=8, IDF025_07_04=5.36, IDF024_07_05=7, IDF025_07_05=5.28, IDF024_07_06=11, IDF025_07_06=4.95, IDF024_07_07=15, IDF025_07_07=1.8, IDF011_08=9, IDF023_08=7, IDF024_08_01=0, IDF025_08_01=2.08, IDF024_08_02=2, IDF025_08_02=2.09, IDF024_08_03=5, IDF025_08_03=3.36, IDF024_08_04=8, IDF025_08_04=3.38, IDF024_08_05=7, IDF025_08_05=3.25, IDF024_08_06=11, IDF025_08_06=3.44, IDF024_08_07=15, IDF025_08_07=1.3900000000000001, IDF011_09=10, IDF023_09=7, IDF024_09_01=0, IDF025_09_01=2.2, IDF024_09_02=2, IDF025_09_02=2.29, IDF024_09_03=5, IDF025_09_03=3.34, IDF024_09_04=8, IDF025_09_04=3.34, IDF024_09_05=7, IDF025_09_05=3.23, IDF024_09_06=11, IDF025_09_06=3.7600000000000002, IDF024_09_07=15, IDF025_09_07=-0.23, IDF011_10=11, IDF023_10=7, IDF024_10_01=0, IDF025_10_01=-1.16, IDF024_10_02=2, IDF025_10_02=-0.89, IDF024_10_03=5, IDF025_10_03=-1.6300000000000001, IDF024_10_04=8, IDF025_10_04=-1.61, IDF024_10_05=7, IDF025_10_05=-1.61, IDF024_10_06=11, IDF025_10_06=-1.47, IDF024_10_07=15, IDF025_10_07=0.3, IDF011_11=12, IDF023_11=6, IDF024_11_01=0, IDF025_11_01=-2.17, IDF024_11_02=2, IDF025_11_02=-2.12, IDF024_11_03=5, IDF025_11_03=-3.35, IDF024_11_04=8, IDF025_11_04=-3.34, IDF024_11_05=7, IDF025_11_05=-3.2800000000000002, IDF024_11_06=11, IDF025_11_06=-3.5, IDF011_12=13, IDF023_12=3, IDF024_12_01=0, IDF025_12_01=-1.69, IDF024_12_02=2, IDF025_12_02=-1.68, IDF024_12_03=11, IDF025_12_03=-2.7600000000000002, IDF011_13=14, IDF023_13=7, IDF024_13_01=0, IDF025_13_01=-0.91, IDF024_13_02=2, IDF025_13_02=-0.68, IDF024_13_03=5, IDF025_13_03=-1.23, IDF024_13_04=8, IDF025_13_04=-1.23, IDF024_13_05=7, IDF025_13_05=-1.23, IDF024_13_06=11, IDF025_13_06=-1.12, IDF024_13_07=15, IDF025_13_07=0.73, IDF011_14=15, IDF023_14=6, IDF024_14_01=0, IDF025_14_01=-2.07, IDF024_14_02=2, IDF025_14_02=-1.84, IDF024_14_03=5, IDF025_14_03=-2.96, IDF024_14_04=8, IDF025_14_04=-2.96, IDF024_14_05=7, IDF025_14_05=-2.91, IDF024_14_06=11, IDF025_14_06=-3.0300000000000002, IDF011_15=16, IDF023_15=3, IDF024_15_01=0, IDF025_15_01=-1.34, IDF024_15_02=2, IDF025_15_02=-1.72, IDF024_15_03=11, IDF025_15_03=-2.83, IDF011_16=17, IDF023_16=6, IDF024_16_01=0, IDF025_16_01=-1.7, IDF024_16_02=2, IDF025_16_02=-1.61, IDF024_16_03=5, IDF025_16_03=-2.7600000000000002, IDF024_16_04=8, IDF025_16_04=-2.7600000000000002, IDF024_16_05=7, IDF025_16_05=-2.64, IDF024_16_06=11, IDF025_16_06=-2.65, IDF011_17=18, IDF023_17=7, IDF024_17_01=0, IDF025_17_01=-1.26, IDF024_17_02=2, IDF025_17_02=-1.0, IDF024_17_03=5, IDF025_17_03=-1.74, IDF024_17_04=8, IDF025_17_04=-1.74, IDF024_17_05=7, IDF025_17_05=-1.72, IDF024_17_06=11, IDF025_17_06=-1.6500000000000001, IDF024_17_07=15, IDF025_17_07=0.28, IDF011_18=19, IDF023_18=3, IDF024_18_01=0, IDF025_18_01=-2.15, IDF024_18_02=2, IDF025_18_02=-2.91, IDF024_18_03=11, IDF025_18_03=-4.79, IDF011_19=20, IDF023_19=3, IDF024_19_01=0, IDF025_19_01=-0.38, IDF024_19_02=2, IDF025_19_02=-1.03, IDF024_19_03=11, IDF025_19_03=-1.69, IDF011_20=21, IDF023_20=3, IDF024_20_01=0, IDF025_20_01=-1.1300000000000001, IDF024_20_02=2, IDF025_20_02=-1.76, IDF024_20_03=11, IDF025_20_03=-2.91, IDF011_21=22, IDF023_21=3, IDF024_21_01=0, IDF025_21_01=-1.23, IDF024_21_02=2, IDF025_21_02=-1.56, IDF024_21_03=11, IDF025_21_03=-2.57, IDF011_22=23, IDF023_22=7, IDF024_22_01=0, IDF025_22_01=-1.27, IDF024_22_02=2, IDF025_22_02=-1.03, IDF024_22_03=5, IDF025_22_03=-1.86, IDF024_22_04=8, IDF025_22_04=-1.86, IDF024_22_05=7, IDF025_22_05=-1.83, IDF024_22_06=11, IDF025_22_06=-1.7, IDF024_22_07=15, IDF025_22_07=0.23, IDF011_23=24, IDF023_23=7, IDF024_23_01=0, IDF025_23_01=2.23, IDF024_23_02=2, IDF025_23_02=2.47, IDF024_23_03=5, IDF025_23_03=4.0, IDF024_23_04=8, IDF025_23_04=4.01, IDF024_23_05=7, IDF025_23_05=4.01, IDF024_23_06=11, IDF025_23_06=4.0600000000000005, IDF024_23_07=15, IDF025_23_07=2.35, IDF011_24=25, IDF023_24=7, IDF024_24_01=0, IDF025_24_01=3.62, IDF024_24_02=2, IDF025_24_02=3.3200000000000003, IDF024_24_03=5, IDF025_24_03=5.7700000000000005, IDF024_24_04=8, IDF025_24_04=5.76, IDF024_24_05=7, IDF025_24_05=5.69, IDF024_24_06=11, IDF025_24_06=5.47, IDF024_24_07=15, IDF025_24_07=3.75, IDF011_25=26, IDF023_25=7, IDF024_25_01=0, IDF025_25_01=3.79, IDF024_25_02=2, IDF025_25_02=3.7600000000000002, IDF024_25_03=5, IDF025_25_03=5.99, IDF024_25_04=8, IDF025_25_04=5.97, IDF024_25_05=7, IDF025_25_05=5.98, IDF024_25_06=11, IDF025_25_06=6.19, IDF024_25_07=15, IDF025_25_07=2.77, IDF011_26=27, IDF023_26=7, IDF024_26_01=0, IDF025_26_01=2.27, IDF024_26_02=2, IDF025_26_02=2.16, IDF024_26_03=5, IDF025_26_03=3.62, IDF024_26_04=8, IDF025_26_04=3.62, IDF024_26_05=7, IDF025_26_05=3.63, IDF024_26_06=11, IDF025_26_06=3.56, IDF024_26_07=15, IDF025_26_07=1.08, IDF011_27=28, IDF023_27=7, IDF024_27_01=0, IDF025_27_01=-1.5, IDF024_27_02=2, IDF025_27_02=-1.26, IDF024_27_03=5, IDF025_27_03=-2.19, IDF024_27_04=8, IDF025_27_04=-2.2, IDF024_27_05=7, IDF025_27_05=-2.16, IDF024_27_06=11, IDF025_27_06=-2.07, IDF024_27_07=15, IDF025_27_07=0.12, IDF011_28=29, IDF023_28=6, IDF024_28_01=0, IDF025_28_01=-1.6400000000000001, IDF024_28_02=2, IDF025_28_02=-1.57, IDF024_28_03=5, IDF025_28_03=-2.5300000000000002, IDF024_28_04=8, IDF025_28_04=-2.5300000000000002, IDF024_28_05=7, IDF025_28_05=-2.34, IDF024_28_06=11, IDF025_28_06=-2.58, IDF011_29=30, IDF023_29=7, IDF024_29_01=0, IDF025_29_01=3.27, IDF024_29_02=2, IDF025_29_02=2.99, IDF024_29_03=5, IDF025_29_03=5.08, IDF024_29_04=8, IDF025_29_04=5.07, IDF024_29_05=7, IDF025_29_05=5.08, IDF024_29_06=11, IDF025_29_06=4.92, IDF024_29_07=15, IDF025_29_07=2.73, IDF011_30=31, IDF023_30=6, IDF024_30_01=0, IDF025_30_01=-2.57, IDF024_30_02=2, IDF025_30_02=-2.4, IDF024_30_03=5, IDF025_30_03=-3.8200000000000003, IDF024_30_04=8, IDF025_30_04=-3.83, IDF024_30_05=7, IDF025_30_05=-3.79, IDF024_30_06=11, IDF025_30_06=-3.95, IDF011_31=32, IDF023_31=7, IDF024_31_01=0, IDF025_31_01=1.46, IDF024_31_02=2, IDF025_31_02=1.79, IDF024_31_03=5, IDF025_31_03=3.14, IDF024_31_04=8, IDF025_31_04=3.13, IDF024_31_05=7, IDF025_31_05=3.0300000000000002, IDF024_31_06=11, IDF025_31_06=2.94, IDF024_31_07=15, IDF025_31_07=-0.41000000000000003)>",
             "<RTCM(4076_045, DF002=4076, IDF001=3, IDF002=45, IDF003=311130, IDF004=3, IDF005=0, IDF007=1, IDF008=0, IDF009=2, IDF010=21, IDF011_01=1, IDF023_01=4, IDF024_01_01=0, IDF025_01_01=2.54, IDF024_01_02=1, IDF025_01_02=2.36, IDF024_01_03=2, IDF025_01_03=3.42, IDF024_01_04=3, IDF025_01_04=3.91, IDF011_02=2, IDF023_02=4, IDF024_02_01=0, IDF025_02_01=0.53, IDF024_02_02=1, IDF025_02_02=0.49, IDF024_02_03=2, IDF025_02_03=0.79, IDF024_02_04=3, IDF025_02_04=0.8200000000000001, IDF011_03=3, IDF023_03=4, IDF024_03_01=0, IDF025_03_01=-0.97, IDF024_03_02=1, IDF025_03_02=-0.86, IDF024_03_03=2, IDF025_03_03=-1.3900000000000001, IDF024_03_04=3, IDF025_03_04=-1.43, IDF011_04=4, IDF023_04=4, IDF024_04_01=0, IDF025_04_01=-1.29, IDF024_04_02=1, IDF025_04_02=-1.1, IDF024_04_03=2, IDF025_04_03=-1.86, IDF024_04_04=3, IDF025_04_04=-1.81, IDF011_05=5, IDF023_05=4, IDF024_05_01=0, IDF025_05_01=-0.51, IDF024_05_02=1, IDF025_05_02=-0.28, IDF024_05_03=2, IDF025_05_03=-0.47000000000000003, IDF024_05_04=3, IDF025_05_04=-0.47000000000000003, IDF011_06=7, IDF023_06=4, IDF024_06_01=0, IDF025_06_01=-0.23, IDF024_06_02=1, IDF025_06_02=-0.13, IDF024_06_03=2, IDF025_06_03=-0.13, IDF024_06_04=3, IDF025_06_04=-0.22, IDF011_07=8, IDF023_07=4, IDF024_07_01=0, IDF025_07_01=-1.79, IDF024_07_02=1, IDF025_07_02=-1.5, IDF024_07_03=2, IDF025_07_03=-2.5100000000000002, IDF024_07_04=3, IDF025_07_04=-2.48, IDF011_08=9, IDF023_08=4, IDF024_08_01=0, IDF025_08_01=-1.58, IDF024_08_02=1, IDF025_08_02=-1.37, IDF024_08_03=2, IDF025_08_03=-2.29, IDF024_08_04=3, IDF025_08_04=-2.27, IDF011_09=11, IDF023_09=4, IDF024_09_01=0, IDF025_09_01=-1.93, IDF024_09_02=1, IDF025_09_02=-1.79, IDF024_09_03=2, IDF025_09_03=-2.94, IDF024_09_04=3, IDF025_09_04=-2.96, IDF011_10=12, IDF023_10=4, IDF024_10_01=0, IDF025_10_01=0.6, IDF024_10_02=1, IDF025_10_02=0.75, IDF024_10_03=2, IDF025_10_03=1.08, IDF024_10_04=3, IDF025_10_04=1.24, IDF011_11=13, IDF023_11=4, IDF024_11_01=0, IDF025_11_01=1.52, IDF024_11_02=1, IDF025_11_02=0.92, IDF024_11_03=2, IDF025_11_03=1.43, IDF024_11_04=3, IDF025_11_04=1.53, IDF011_12=14, IDF023_12=4, IDF024_12_01=0, IDF025_12_01=0.8300000000000001, IDF024_12_02=1, IDF025_12_02=0.84, IDF024_12_03=2, IDF025_12_03=1.45, IDF024_12_04=3, IDF025_12_04=1.3900000000000001, IDF011_13=15, IDF023_13=4, IDF024_13_01=0, IDF025_13_01=-0.13, IDF024_13_02=1, IDF025_13_02=0.07, IDF024_13_03=2, IDF025_13_03=0.02, IDF024_13_04=3, IDF025_13_04=0.12, IDF011_14=16, IDF023_14=4, IDF024_14_01=0, IDF025_14_01=0.14, IDF024_14_02=1, IDF025_14_02=0.27, IDF024_14_03=2, IDF025_14_03=0.41000000000000003, IDF024_14_04=3, IDF025_14_04=0.44, IDF011_15=17, IDF023_15=4, IDF024_15_01=0, IDF025_15_01=-0.26, IDF024_15_02=1, IDF025_15_02=-0.23, IDF024_15_03=2, IDF025_15_03=-0.41000000000000003, IDF024_15_04=3, IDF025_15_04=-0.38, IDF011_16=18, IDF023_16=4, IDF024_16_01=0, IDF025_16_01=0.55, IDF024_16_02=1, IDF025_16_02=0.66, IDF024_16_03=2, IDF025_16_03=0.96, IDF024_16_04=3, IDF025_16_04=1.09, IDF011_17=19, IDF023_17=4, IDF024_17_01=0, IDF025_17_01=-0.04, IDF024_17_02=1, IDF025_17_02=-0.28, IDF024_17_03=2, IDF025_17_03=-0.01, IDF024_17_04=3, IDF025_17_04=-0.46, IDF011_18=20, IDF023_18=4, IDF024_18_01=0, IDF025_18_01=2.63, IDF024_18_02=1, IDF025_18_02=2.61, IDF024_18_03=2, IDF025_18_03=4.98, IDF024_18_04=3, IDF025_18_04=4.3100000000000005, IDF011_19=21, IDF023_19=4, IDF024_19_01=0, IDF025_19_01=-0.04, IDF024_19_02=1, IDF025_19_02=0.0, IDF024_19_03=2, IDF025_19_03=-0.13, IDF024_19_04=3, IDF025_19_04=0.0, IDF011_20=22, IDF023_20=4, IDF024_20_01=0, IDF025_20_01=-1.49, IDF024_20_02=1, IDF025_20_02=-1.3800000000000001, IDF024_20_03=2, IDF025_20_03=-2.41, IDF024_20_04=3, IDF025_20_04=-2.29, IDF011_21=24, IDF023_21=4, IDF024_21_01=0, IDF025_21_01=-0.07, IDF024_21_02=1, IDF025_21_02=-0.03, IDF024_21_03=2, IDF025_21_03=-0.08, IDF024_21_04=3, IDF025_21_04=-0.06)>",
         ]
         dirname = os.path.dirname(__file__)
         with open(os.path.join(dirname, "pygpsdata-NTRIP-4076.log"), "rb") as stream:
             i = 0
             raw = 0
-            rtr = RTCMReader(stream, scaling=True, labelmsm=True)
+            rtr = RTCMReader(stream, labelmsm=True)
             for raw, parsed in rtr:
                 if raw is not None:
                     # print(f'"{parsed}",')
                     self.assertEqual(f"{parsed}", EXPECTED_RESULTS[i])
                     i += 1
 
     def testSerialize(self):  # test serialize()
@@ -346,24 +325,23 @@
         msg1 = RTCMMessage(payload=self._payload1007)
         msg2 = RTCMReader.parse(self._raw1007)
         self.assertEqual(str(msg1), EXPECTED_RESULT)
         self.assertEqual(str(msg2), EXPECTED_RESULT)
 
     def testnestedgroups(self):  # test message with nested repeating group (1059, 1065)
         EXPECTED_RESULT = "<RTCM(1065, DF002=1065, DF386=12345, DF391=3, DF388=0, DF413=1, DF414=1, DF415=1, DF387=2, DF384_01=23, DF379_01=2, DF381_01_01=4, DF383_01_01=0.07, DF381_01_02=2, DF383_01_02=0.09, DF384_02=26, DF379_02=1, DF381_02_01=3, DF383_02_01=0.05)>"
-        msg = RTCMReader.parse(self._raw1065, scaling=True)
+        msg = RTCMReader.parse(self._raw1065)
         self.assertEqual(str(msg), EXPECTED_RESULT)
 
     def testbadCRC(
         self,
     ):  # test mixed stream of NMEA, UBX & RTCM messages with invalid RTCM CRC
         EXPECTED_ERROR = "RTCM3 message invalid - failed CRC: (.*)"
-        dirname = os.path.dirname(__file__)
         with open(
-            os.path.join(dirname, "pygpsdata-MIXED-RTCM3BADCRC.log"), "rb"
+            os.path.join(DIRNAME, "pygpsdata-MIXED-RTCM3BADCRC.log"), "rb"
         ) as stream:
             i = 0
             raw = 0
             rtr = RTCMReader(stream, quitonerror=rtt.ERR_RAISE)
             with self.assertRaisesRegex(RTCMParseError, EXPECTED_ERROR):
                 for raw, parsed in rtr:
                     if raw is not None:
@@ -391,28 +369,59 @@
             output = self.restoreio()
             self.assertEqual(output, EXPECTED_ERROR)
 
     def testbadCRC3(
         self,
     ):  # test mixed stream of NMEA, UBX & RTCM messages with invalid RTCM CRC
         EXPECTED_ERROR = "RTCM3 message invalid - failed CRC: b'Z\\xd7\\xf7'"
-        dirname = os.path.dirname(__file__)
-        with open(
-            os.path.join(dirname, "pygpsdata-MIXED-RTCM3BADCRC.log"), "rb"
-        ) as stream:
-            self.catchio()
-            rtr = RTCMReader(
-                stream,
-                quitonerror=rtt.ERR_LOG,
-                errorhandler=None,
+        with self.assertLogs(level=ERROR) as log:
+            with open(
+                os.path.join(DIRNAME, "pygpsdata-MIXED-RTCM3BADCRC.log"), "rb"
+            ) as stream:
+                rtr = RTCMReader(
+                    stream,
+                    quitonerror=rtt.ERR_LOG,
+                    errorhandler=None,
+                )
+                for raw, parsed in rtr:
+                    if raw is not None:
+                        pass
+            self.assertEqual(
+                [
+                    "ERROR:pyrtcm.rtcmreader:RTCM3 message invalid - failed CRC: b'Z\\xd7\\xf7'"
+                ],
+                log.output,
             )
-            for raw, parsed in rtr:
-                if raw is not None:
-                    pass
-            stream.close()
-            output = self.restoreio()
-            self.assertEqual(output, EXPECTED_ERROR)
+
+    def testBADHDR_FAIL(self):  # invalid header in data with quitonerror = 2
+        EXPECTED_ERROR = "Unknown protocol header b'\\xb5w'"
+        with self.assertRaises(RTCMParseError) as context:
+            i = 0
+            with open(os.path.join(DIRNAME, "pygpsdata-BADHDR.log"), "rb") as stream:
+                ubr = RTCMReader(stream, quitonerror=ERR_RAISE)
+                for _, _ in ubr:
+                    i += 1
+        self.assertTrue(EXPECTED_ERROR in str(context.exception))
+
+    def testBADHDR_LOG(self):  # invalid header in data with quitonerror = 1
+        i = 0
+        with self.assertLogs(level=ERROR) as log:
+            with open(os.path.join(DIRNAME, "pygpsdata-BADHDR.log"), "rb") as stream:
+                ubr = RTCMReader(stream, quitonerror=ERR_LOG)
+                for raw, parsed in ubr:
+                    i += 1
+            self.assertEqual(
+                ["ERROR:pyrtcm.rtcmreader:Unknown protocol header b'\\xb5w'."],
+                log.output,
+            )
+
+    def testBADHDR_IGNORE(self):  # invalid header in data with quitonerror = 0
+        i = 0
+        with open(os.path.join(DIRNAME, "pygpsdata-BADHDR.log"), "rb") as stream:
+            ubr = RTCMReader(stream, quitonerror=ERR_IGNORE)
+            for raw, parsed in ubr:
+                i += 1
 
 
 if __name__ == "__main__":
     # import sys;sys.argv = ['', 'Test.testName']
     unittest.main()
```

