# Comparing `tmp/pimoroni-mics6814-0.0.2.tar.gz` & `tmp/pimoroni_mics6814-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pimoroni-mics6814-0.0.2.tar", last modified: Wed Sep 15 10:26:15 2021, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `pimoroni-mics6814-0.0.2.tar` & `pimoroni_mics6814-1.0.0.tar`

### file list

```diff
@@ -1,17 +1,20 @@
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2021-09-15 10:26:15.015026 pimoroni-mics6814-0.0.2/
--rw-rw-r--   0 phil      (1000) phil      (1000)      100 2021-09-15 10:23:19.000000 pimoroni-mics6814-0.0.2/CHANGELOG.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)     1070 2021-09-14 11:10:22.000000 pimoroni-mics6814-0.0.2/LICENSE.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)      109 2021-09-14 11:10:22.000000 pimoroni-mics6814-0.0.2/MANIFEST.in
--rw-rw-r--   0 phil      (1000) phil      (1000)     2528 2021-09-15 10:26:15.015026 pimoroni-mics6814-0.0.2/PKG-INFO
--rw-rw-r--   0 phil      (1000) phil      (1000)     1345 2021-09-15 10:23:19.000000 pimoroni-mics6814-0.0.2/README.md
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2021-09-15 10:26:15.015026 pimoroni-mics6814-0.0.2/mics6814/
--rw-rw-r--   0 phil      (1000) phil      (1000)     5070 2021-09-15 10:23:19.000000 pimoroni-mics6814-0.0.2/mics6814/__init__.py
-drwxrwxr-x   0 phil      (1000) phil      (1000)        0 2021-09-15 10:26:15.015026 pimoroni-mics6814-0.0.2/pimoroni_mics6814.egg-info/
--rw-rw-r--   0 phil      (1000) phil      (1000)     2528 2021-09-15 10:26:14.000000 pimoroni-mics6814-0.0.2/pimoroni_mics6814.egg-info/PKG-INFO
--rw-rw-r--   0 phil      (1000) phil      (1000)      306 2021-09-15 10:26:14.000000 pimoroni-mics6814-0.0.2/pimoroni_mics6814.egg-info/SOURCES.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)        1 2021-09-15 10:26:14.000000 pimoroni-mics6814-0.0.2/pimoroni_mics6814.egg-info/dependency_links.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)       20 2021-09-15 10:26:14.000000 pimoroni-mics6814-0.0.2/pimoroni_mics6814.egg-info/requires.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)        9 2021-09-15 10:26:14.000000 pimoroni-mics6814-0.0.2/pimoroni_mics6814.egg-info/top_level.txt
--rw-rw-r--   0 phil      (1000) phil      (1000)       98 2021-09-14 11:10:22.000000 pimoroni-mics6814-0.0.2/pyproject.toml
--rw-rw-r--   0 phil      (1000) phil      (1000)     1109 2021-09-15 10:26:15.015026 pimoroni-mics6814-0.0.2/setup.cfg
--rwxrwxr-x   0 phil      (1000) phil      (1000)     1388 2021-09-14 11:10:22.000000 pimoroni-mics6814-0.0.2/setup.py
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 pimoroni_mics6814-1.0.0/CHANGELOG.md
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 pimoroni_mics6814-1.0.0/MANIFEST.in
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 pimoroni_mics6814-1.0.0/Makefile
+-rw-r--r--   0        0        0     1991 2020-02-02 00:00:00.000000 pimoroni_mics6814-1.0.0/README.md
+-rw-r--r--   0        0        0     3497 2020-02-02 00:00:00.000000 pimoroni_mics6814-1.0.0/REFERENCE.md
+-rwxr-xr-x   0        0        0     2050 2020-02-02 00:00:00.000000 pimoroni_mics6814-1.0.0/check.sh
+-rwxr-xr-x   0        0        0     9742 2020-02-02 00:00:00.000000 pimoroni_mics6814-1.0.0/install.sh
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 pimoroni_mics6814-1.0.0/requirements-dev.txt
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 pimoroni_mics6814-1.0.0/tox.ini
+-rwxr-xr-x   0        0        0     1283 2020-02-02 00:00:00.000000 pimoroni_mics6814-1.0.0/uninstall.sh
+-rwxr-xr-x   0        0        0      514 2020-02-02 00:00:00.000000 pimoroni_mics6814-1.0.0/examples/gas.py
+-rwxr-xr-x   0        0        0      398 2020-02-02 00:00:00.000000 pimoroni_mics6814-1.0.0/examples/led.py
+-rw-r--r--   0        0        0     4983 2020-02-02 00:00:00.000000 pimoroni_mics6814-1.0.0/mics6814/__init__.py
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 pimoroni_mics6814-1.0.0/tests/conftest.py
+-rw-r--r--   0        0        0     3012 2020-02-02 00:00:00.000000 pimoroni_mics6814-1.0.0/tests/test_io.py
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 pimoroni_mics6814-1.0.0/tests/test_setup.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 pimoroni_mics6814-1.0.0/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 pimoroni_mics6814-1.0.0/LICENSE
+-rw-r--r--   0        0        0     2339 2020-02-02 00:00:00.000000 pimoroni_mics6814-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     4581 2020-02-02 00:00:00.000000 pimoroni_mics6814-1.0.0/PKG-INFO
```

### Comparing `pimoroni-mics6814-0.0.2/LICENSE.txt` & `pimoroni_mics6814-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pimoroni-mics6814-0.0.2/mics6814/__init__.py` & `pimoroni_mics6814-1.0.0/mics6814/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,48 +1,43 @@
 import ioexpander as io
 
-
-__version__ = '0.0.2'
+__version__ = "1.0.0"
 
 MICS6814_I2C_ADDR = 0x19
 
 MICS6814_LED_R = 3  # P1.2
 MICS6814_LED_G = 7  # P1.1
 MICS6814_LED_B = 2  # P1.0
 
 MICS6814_VREF = 14  # P1.4 AIN0 - 3v3
-MICS6814_RED = 13   # P0.7 AIN2 - Oxidizing
+MICS6814_RED = 13   # P0.7 AIN2 - Reducing
 MICS6814_NH3 = 11   # P0.6 AIN3 - NH3
-MICS6814_OX = 12    # P0.5 AIN4 - Reducing
+MICS6814_OX = 12    # P0.5 AIN4 - Oxidizing
 
 MICS6814_HEATER_EN = 1  # P1.5 Heater Enable
 
 
 class Mics6814Reading(object):
-    __slots__ = 'oxidising', 'reducing', 'nh3', 'adc'
+    __slots__ = "oxidising", "reducing", "nh3", "adc"
 
     def __init__(self, ox, red, nh3, adc=None):
         self.oxidising = ox
         self.reducing = red
         self.nh3 = nh3
         self.adc = adc
 
     def __repr__(self):
-        fmt = """Oxidising: {ox:05.02f} Ohms
-Reducing: {red:05.02f} Ohms
-NH3: {nh3:05.02f} Ohms"""
+        repr = f"""Oxidising: {self.oxidising:05.02f} Ohms
+Reducing: {self.reducing:05.02f} Ohms
+NH3: {self.nh3:05.02f} Ohms"""
         if self.adc is not None:
-            fmt += """
-ADC (ref): {adc:05.02f} Volts
+            repr += """
+ADC (ref): {self.adc:05.02f} Volts
 """
-        return fmt.format(
-            ox=self.oxidising,
-            red=self.reducing,
-            nh3=self.nh3,
-            adc=self.adc)
+        return repr
 
     __str__ = __repr__
 
 
 class MICS6814():
     def __init__(self, i2c_addr=MICS6814_I2C_ADDR, interrupt_timeout=1.0, interrupt_pin=None, gpio=None):
         self._ioe = io.IOE(i2c_addr, interrupt_timeout, interrupt_pin, gpio)
```

