# Comparing `tmp/PySigmaKoki-2.1.2.tar.gz` & `tmp/pysigmakoki-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PySigmaKoki-2.1.2.tar", last modified: Mon May 22 09:07:39 2023, max compression
+gzip compressed data, was "pysigmakoki-2.1.3.tar", last modified: Thu May 23 01:49:06 2024, max compression
```

## Comparing `PySigmaKoki-2.1.2.tar` & `pysigmakoki-2.1.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 oxon       (501) staff       (20)        0 2023-05-22 09:07:39.504839 PySigmaKoki-2.1.2/
--rw-r--r--   0 oxon       (501) staff       (20)      507 2023-05-22 09:07:39.504489 PySigmaKoki-2.1.2/PKG-INFO
-drwxr-xr-x   0 oxon       (501) staff       (20)        0 2023-05-22 09:07:39.503969 PySigmaKoki-2.1.2/PySigmaKoki.egg-info/
--rw-r--r--   0 oxon       (501) staff       (20)      507 2023-05-22 09:07:39.000000 PySigmaKoki-2.1.2/PySigmaKoki.egg-info/PKG-INFO
--rw-r--r--   0 oxon       (501) staff       (20)      206 2023-05-22 09:07:39.000000 PySigmaKoki-2.1.2/PySigmaKoki.egg-info/SOURCES.txt
--rw-r--r--   0 oxon       (501) staff       (20)        1 2023-05-22 09:07:39.000000 PySigmaKoki-2.1.2/PySigmaKoki.egg-info/dependency_links.txt
--rw-r--r--   0 oxon       (501) staff       (20)        9 2023-05-22 09:07:39.000000 PySigmaKoki-2.1.2/PySigmaKoki.egg-info/requires.txt
--rw-r--r--   0 oxon       (501) staff       (20)       11 2023-05-22 09:07:39.000000 PySigmaKoki-2.1.2/PySigmaKoki.egg-info/top_level.txt
--rw-r--r--   0 oxon       (501) staff       (20)      384 2018-07-20 01:12:39.000000 PySigmaKoki-2.1.2/README.md
--rw-r--r--   0 oxon       (501) staff       (20)       38 2023-05-22 09:07:39.504943 PySigmaKoki-2.1.2/setup.cfg
--rw-r--r--   0 oxon       (501) staff       (20)      691 2023-05-17 06:13:42.000000 PySigmaKoki-2.1.2/setup.py
--rw-r--r--   0 oxon       (501) staff       (20)    10732 2023-05-17 06:00:32.000000 PySigmaKoki-2.1.2/sigma_koki.py
+drwxr-xr-x   0 oxon       (501) staff       (20)        0 2024-05-23 01:49:06.186113 pysigmakoki-2.1.3/
+-rw-r--r--   0 oxon       (501) staff       (20)      999 2024-05-23 01:49:06.185926 pysigmakoki-2.1.3/PKG-INFO
+drwxr-xr-x   0 oxon       (501) staff       (20)        0 2024-05-23 01:49:06.185753 pysigmakoki-2.1.3/PySigmaKoki.egg-info/
+-rw-r--r--   0 oxon       (501) staff       (20)      999 2024-05-23 01:49:06.000000 pysigmakoki-2.1.3/PySigmaKoki.egg-info/PKG-INFO
+-rw-r--r--   0 oxon       (501) staff       (20)      212 2024-05-23 01:49:06.000000 pysigmakoki-2.1.3/PySigmaKoki.egg-info/SOURCES.txt
+-rw-r--r--   0 oxon       (501) staff       (20)        1 2024-05-23 01:49:06.000000 pysigmakoki-2.1.3/PySigmaKoki.egg-info/dependency_links.txt
+-rw-r--r--   0 oxon       (501) staff       (20)        9 2024-05-23 01:49:06.000000 pysigmakoki-2.1.3/PySigmaKoki.egg-info/requires.txt
+-rw-r--r--   0 oxon       (501) staff       (20)       11 2024-05-23 01:49:06.000000 pysigmakoki-2.1.3/PySigmaKoki.egg-info/top_level.txt
+-rw-r--r--   0 oxon       (501) staff       (20)      466 2024-05-22 07:01:37.000000 pysigmakoki-2.1.3/README.md
+-rw-r--r--   0 oxon       (501) staff       (20)      712 2024-05-23 01:40:24.000000 pysigmakoki-2.1.3/pyproject.toml
+-rw-r--r--   0 oxon       (501) staff       (20)       38 2024-05-23 01:49:06.186149 pysigmakoki-2.1.3/setup.cfg
+-rw-r--r--   0 oxon       (501) staff       (20)    10733 2024-05-22 13:08:28.000000 pysigmakoki-2.1.3/sigma_koki.py
```

### Comparing `PySigmaKoki-2.1.2/sigma_koki.py` & `pysigmakoki-2.1.3/sigma_koki.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,20 +20,21 @@
         self.__dataBit = 8
         self.__stopBit = 1
         self.__rtscts = True
         self.__product = product
         self.__acknowledge =  True
 
     def setBaudRate(self, rate):
-        if product == 'GSC-02' and rate in (2400, 4800, 9600, 19200):
-            self.__baudRate = rate
-        elif product == 'SHOT-702' and rate == 38400:
+        rates = {'GSC-02': (2400, 4800, 9600, 19200),
+                 'SHOT-702' : (38400,),
+                 'SHOT-702H' : (38400,)}
+        if rate in rates[self.__product]:
             self.__baudRate = rate
         else:
-            raise ValueError('Attempting to set an invalid buard rate %d to %s. Must be chosen from 2400/4800/9600/19200 for GSC-02 and 38400 for SHOT-702.' % (rate, self.__product))
+            raise ValueError('Attempting to set an invalid buard rate of %d to %s. The rate must be chosen from %s.' % (rate, self.__product, rates[self.__product]))
 
     def disableAcknowledge(self):
         self.__acknowledge = False
 
     def write(self, command, acknowledge=True):
         # 'str' class needs be converted into 'bytes'
         # e.g., 'command' -> b'command'
```

