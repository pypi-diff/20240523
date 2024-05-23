# Comparing `tmp/ivmdriver-0.0.7.tar.gz` & `tmp/ivmdriver-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ivmdriver-0.0.7.tar", last modified: Thu May 23 11:49:47 2024, max compression
+gzip compressed data, was "ivmdriver-0.0.8.tar", last modified: Thu May 23 14:38:38 2024, max compression
```

## Comparing `ivmdriver-0.0.7.tar` & `ivmdriver-0.0.8.tar`

### file list

```diff
@@ -1,49 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:49:47.006130 ivmdriver-0.0.7/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:49:46.998129 ivmdriver-0.0.7/IvmDriver/
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-23 11:49:29.000000 ivmdriver-0.0.7/IvmDriver/DFTMatrix.spec
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-23 11:49:29.000000 ivmdriver-0.0.7/IvmDriver/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-23 11:49:29.000000 ivmdriver-0.0.7/IvmDriver/Matrixgui.py
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-23 11:49:29.000000 ivmdriver-0.0.7/IvmDriver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-23 11:49:29.000000 ivmdriver-0.0.7/IvmDriver/appexe.spec
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:49:46.998129 ivmdriver-0.0.7/IvmDriver/assets/
--rw-r--r--   0 runner    (1001) docker     (127)    67646 2024-05-23 11:49:29.000000 ivmdriver-0.0.7/IvmDriver/assets/logo.ico
--rw-r--r--   0 runner    (1001) docker     (127)    45518 2024-05-23 11:49:29.000000 ivmdriver-0.0.7/IvmDriver/assets/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:49:47.002129 ivmdriver-0.0.7/IvmDriver/docs/
--rw-r--r--   0 runner    (1001) docker     (127)  1722187 2024-05-23 11:49:29.000000 ivmdriver-0.0.7/IvmDriver/docs/DFT Matrix.pptx
--rw-r--r--   0 runner    (1001) docker     (127)  1019348 2024-05-23 11:49:29.000000 ivmdriver-0.0.7/IvmDriver/docs/MCP23017-Data-Sheet-DS20001952.pdf
--rw-r--r--   0 runner    (1001) docker     (127)  1049439 2024-05-23 11:49:29.000000 ivmdriver-0.0.7/IvmDriver/docs/expand-2-click-manual-v100-1484105.pdf
--rw-r--r--   0 runner    (1001) docker     (127)    10458 2024-05-23 11:49:29.000000 ivmdriver-0.0.7/IvmDriver/driver.py
--rw-r--r--   0 runner    (1001) docker     (127)    12828 2024-05-23 11:49:29.000000 ivmdriver-0.0.7/IvmDriver/driver.ui
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 11:49:29.000000 ivmdriver-0.0.7/IvmDriver/driverPage.py
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-23 11:49:29.000000 ivmdriver-0.0.7/IvmDriver/exeGenerate.py
--rw-r--r--   0 runner    (1001) docker     (127)     6295 2024-05-23 11:49:29.000000 ivmdriver-0.0.7/IvmDriver/fileopen.py
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-23 11:49:29.000000 ivmdriver-0.0.7/IvmDriver/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-23 11:49:29.000000 ivmdriver-0.0.7/IvmDriver/mainDriver.spec
--rw-r--r--   0 runner    (1001) docker     (127)    77406 2024-05-23 11:49:29.000000 ivmdriver-0.0.7/IvmDriver/matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)     4621 2024-05-23 11:49:29.000000 ivmdriver-0.0.7/IvmDriver/matrixDriver.py
--rw-r--r--   0 runner    (1001) docker     (127)    87565 2024-05-23 11:49:29.000000 ivmdriver-0.0.7/IvmDriver/matrixFrame.ui
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-23 11:49:29.000000 ivmdriver-0.0.7/IvmDriver/mcp2221.py
--rw-r--r--   0 runner    (1001) docker     (127)     3666 2024-05-23 11:49:29.000000 ivmdriver-0.0.7/IvmDriver/mcp2317.py
--rw-r--r--   0 runner    (1001) docker     (127)    22289 2024-05-23 11:49:29.000000 ivmdriver-0.0.7/IvmDriver/reserach.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     3904 2024-05-23 11:49:29.000000 ivmdriver-0.0.7/IvmDriver/signalRoot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:49:47.002129 ivmdriver-0.0.7/IvmDriver/signals/
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-23 11:49:29.000000 ivmdriver-0.0.7/IvmDriver/signals/SignalConfig.json
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-23 11:49:29.000000 ivmdriver-0.0.7/IvmDriver/signals/dummysignalconfig.json
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-23 11:49:29.000000 ivmdriver-0.0.7/IvmDriver/signals/dummysignalconfig1.json
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-23 11:49:29.000000 ivmdriver-0.0.7/IvmDriver/signals/intrepretor.json
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-23 11:49:29.000000 ivmdriver-0.0.7/IvmDriver/signals/signalConfigtest.json
--rw-r--r--   0 runner    (1001) docker     (127)    18653 2024-05-23 11:49:29.000000 ivmdriver-0.0.7/IvmDriver/signals/signalroot_matrix.json
--rw-r--r--   0 runner    (1001) docker     (127)    18675 2024-05-23 11:49:29.000000 ivmdriver-0.0.7/IvmDriver/signals/signalroot_matrix1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:49:47.006130 ivmdriver-0.0.7/IvmDriver/styles/
--rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-05-23 11:49:29.000000 ivmdriver-0.0.7/IvmDriver/styles/app.qss
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-23 11:49:29.000000 ivmdriver-0.0.7/IvmDriver/styles/scrollAreaFrame.qss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:49:47.006130 ivmdriver-0.0.7/IvmDriver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-23 11:49:46.000000 ivmdriver-0.0.7/IvmDriver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-23 11:49:46.000000 ivmdriver-0.0.7/IvmDriver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 11:49:46.000000 ivmdriver-0.0.7/IvmDriver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-23 11:49:46.000000 ivmdriver-0.0.7/IvmDriver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-23 11:49:46.000000 ivmdriver-0.0.7/IvmDriver.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-23 11:49:47.006130 ivmdriver-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-23 11:49:29.000000 ivmdriver-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 11:49:47.006130 ivmdriver-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-05-23 11:49:29.000000 ivmdriver-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:38:38.164986 ivmdriver-0.0.8/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:38:38.160986 ivmdriver-0.0.8/IvmDriver/
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-23 14:38:22.000000 ivmdriver-0.0.8/IvmDriver/DFTMatrix.spec
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-23 14:38:22.000000 ivmdriver-0.0.8/IvmDriver/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:38:38.160986 ivmdriver-0.0.8/IvmDriver/GPIOExpander/
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-05-23 14:38:22.000000 ivmdriver-0.0.8/IvmDriver/GPIOExpander/pcf8547.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-23 14:38:22.000000 ivmdriver-0.0.8/IvmDriver/Matrixgui.py
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-23 14:38:22.000000 ivmdriver-0.0.8/IvmDriver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-23 14:38:22.000000 ivmdriver-0.0.8/IvmDriver/appexe.spec
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:38:38.160986 ivmdriver-0.0.8/IvmDriver/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)    67646 2024-05-23 14:38:22.000000 ivmdriver-0.0.8/IvmDriver/assets/logo.ico
+-rw-r--r--   0 runner    (1001) docker     (127)    45518 2024-05-23 14:38:22.000000 ivmdriver-0.0.8/IvmDriver/assets/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:38:38.160986 ivmdriver-0.0.8/IvmDriver/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)  1722187 2024-05-23 14:38:22.000000 ivmdriver-0.0.8/IvmDriver/docs/DFT Matrix.pptx
+-rw-r--r--   0 runner    (1001) docker     (127)  1019348 2024-05-23 14:38:22.000000 ivmdriver-0.0.8/IvmDriver/docs/MCP23017-Data-Sheet-DS20001952.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)  1049439 2024-05-23 14:38:22.000000 ivmdriver-0.0.8/IvmDriver/docs/expand-2-click-manual-v100-1484105.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)    10458 2024-05-23 14:38:22.000000 ivmdriver-0.0.8/IvmDriver/driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12828 2024-05-23 14:38:22.000000 ivmdriver-0.0.8/IvmDriver/driver.ui
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 14:38:22.000000 ivmdriver-0.0.8/IvmDriver/driverPage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-23 14:38:22.000000 ivmdriver-0.0.8/IvmDriver/exeGenerate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6295 2024-05-23 14:38:22.000000 ivmdriver-0.0.8/IvmDriver/fileopen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-23 14:38:22.000000 ivmdriver-0.0.8/IvmDriver/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-23 14:38:22.000000 ivmdriver-0.0.8/IvmDriver/mainDriver.spec
+-rw-r--r--   0 runner    (1001) docker     (127)    77406 2024-05-23 14:38:22.000000 ivmdriver-0.0.8/IvmDriver/matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4621 2024-05-23 14:38:22.000000 ivmdriver-0.0.8/IvmDriver/matrixDriver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    87565 2024-05-23 14:38:22.000000 ivmdriver-0.0.8/IvmDriver/matrixFrame.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-05-23 14:38:22.000000 ivmdriver-0.0.8/IvmDriver/mcp2221.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3666 2024-05-23 14:38:22.000000 ivmdriver-0.0.8/IvmDriver/mcp2317.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22289 2024-05-23 14:38:22.000000 ivmdriver-0.0.8/IvmDriver/reserach.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3904 2024-05-23 14:38:22.000000 ivmdriver-0.0.8/IvmDriver/signalRoot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:38:38.164986 ivmdriver-0.0.8/IvmDriver/signals/
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-23 14:38:22.000000 ivmdriver-0.0.8/IvmDriver/signals/SignalConfig.json
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-23 14:38:22.000000 ivmdriver-0.0.8/IvmDriver/signals/dummysignalconfig.json
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-23 14:38:22.000000 ivmdriver-0.0.8/IvmDriver/signals/dummysignalconfig1.json
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-23 14:38:22.000000 ivmdriver-0.0.8/IvmDriver/signals/intrepretor.json
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-23 14:38:22.000000 ivmdriver-0.0.8/IvmDriver/signals/signalConfigtest.json
+-rw-r--r--   0 runner    (1001) docker     (127)    18653 2024-05-23 14:38:22.000000 ivmdriver-0.0.8/IvmDriver/signals/signalroot_matrix.json
+-rw-r--r--   0 runner    (1001) docker     (127)    18675 2024-05-23 14:38:22.000000 ivmdriver-0.0.8/IvmDriver/signals/signalroot_matrix1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:38:38.164986 ivmdriver-0.0.8/IvmDriver/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-05-23 14:38:22.000000 ivmdriver-0.0.8/IvmDriver/styles/app.qss
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-23 14:38:22.000000 ivmdriver-0.0.8/IvmDriver/styles/scrollAreaFrame.qss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:38:38.164986 ivmdriver-0.0.8/IvmDriver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-23 14:38:38.000000 ivmdriver-0.0.8/IvmDriver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-23 14:38:38.000000 ivmdriver-0.0.8/IvmDriver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 14:38:38.000000 ivmdriver-0.0.8/IvmDriver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-23 14:38:38.000000 ivmdriver-0.0.8/IvmDriver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-23 14:38:38.000000 ivmdriver-0.0.8/IvmDriver.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-23 14:38:38.164986 ivmdriver-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-23 14:38:22.000000 ivmdriver-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 14:38:38.164986 ivmdriver-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-23 14:38:22.000000 ivmdriver-0.0.8/setup.py
```

### Comparing `ivmdriver-0.0.7/IvmDriver/DFTMatrix.spec` & `ivmdriver-0.0.8/IvmDriver/DFTMatrix.spec`

 * *Files identical despite different names*

### Comparing `ivmdriver-0.0.7/IvmDriver/appexe.spec` & `ivmdriver-0.0.8/IvmDriver/appexe.spec`

 * *Files identical despite different names*

### Comparing `ivmdriver-0.0.7/IvmDriver/assets/logo.ico` & `ivmdriver-0.0.8/IvmDriver/assets/logo.ico`

 * *Files identical despite different names*

### Comparing `ivmdriver-0.0.7/IvmDriver/assets/logo.png` & `ivmdriver-0.0.8/IvmDriver/assets/logo.png`

 * *Files identical despite different names*

### Comparing `ivmdriver-0.0.7/IvmDriver/docs/DFT Matrix.pptx` & `ivmdriver-0.0.8/IvmDriver/docs/DFT Matrix.pptx`

 * *Files identical despite different names*

### Comparing `ivmdriver-0.0.7/IvmDriver/docs/MCP23017-Data-Sheet-DS20001952.pdf` & `ivmdriver-0.0.8/IvmDriver/docs/MCP23017-Data-Sheet-DS20001952.pdf`

 * *Files identical despite different names*

### Comparing `ivmdriver-0.0.7/IvmDriver/docs/expand-2-click-manual-v100-1484105.pdf` & `ivmdriver-0.0.8/IvmDriver/docs/expand-2-click-manual-v100-1484105.pdf`

 * *Files identical despite different names*

### Comparing `ivmdriver-0.0.7/IvmDriver/driver.py` & `ivmdriver-0.0.8/IvmDriver/driver.py`

 * *Files identical despite different names*

### Comparing `ivmdriver-0.0.7/IvmDriver/driver.ui` & `ivmdriver-0.0.8/IvmDriver/driver.ui`

 * *Files identical despite different names*

### Comparing `ivmdriver-0.0.7/IvmDriver/exeGenerate.py` & `ivmdriver-0.0.8/IvmDriver/exeGenerate.py`

 * *Files identical despite different names*

### Comparing `ivmdriver-0.0.7/IvmDriver/fileopen.py` & `ivmdriver-0.0.8/IvmDriver/fileopen.py`

 * *Files identical despite different names*

### Comparing `ivmdriver-0.0.7/IvmDriver/logger.py` & `ivmdriver-0.0.8/IvmDriver/logger.py`

 * *Files identical despite different names*

### Comparing `ivmdriver-0.0.7/IvmDriver/mainDriver.spec` & `ivmdriver-0.0.8/IvmDriver/mainDriver.spec`

 * *Files identical despite different names*

### Comparing `ivmdriver-0.0.7/IvmDriver/matrix.py` & `ivmdriver-0.0.8/IvmDriver/matrix.py`

 * *Files identical despite different names*

### Comparing `ivmdriver-0.0.7/IvmDriver/matrixDriver.py` & `ivmdriver-0.0.8/IvmDriver/matrixDriver.py`

 * *Files identical despite different names*

### Comparing `ivmdriver-0.0.7/IvmDriver/matrixFrame.ui` & `ivmdriver-0.0.8/IvmDriver/matrixFrame.ui`

 * *Files identical despite different names*

### Comparing `ivmdriver-0.0.7/IvmDriver/mcp2317.py` & `ivmdriver-0.0.8/IvmDriver/mcp2317.py`

 * *Files identical despite different names*

### Comparing `ivmdriver-0.0.7/IvmDriver/reserach.ipynb` & `ivmdriver-0.0.8/IvmDriver/reserach.ipynb`

 * *Files identical despite different names*

### Comparing `ivmdriver-0.0.7/IvmDriver/signalRoot.py` & `ivmdriver-0.0.8/IvmDriver/signalRoot.py`

 * *Files identical despite different names*

### Comparing `ivmdriver-0.0.7/IvmDriver/signals/SignalConfig.json` & `ivmdriver-0.0.8/IvmDriver/signals/SignalConfig.json`

 * *Files identical despite different names*

### Comparing `ivmdriver-0.0.7/IvmDriver/signals/signalConfigtest.json` & `ivmdriver-0.0.8/IvmDriver/signals/signalConfigtest.json`

 * *Files identical despite different names*

### Comparing `ivmdriver-0.0.7/IvmDriver/signals/signalroot_matrix.json` & `ivmdriver-0.0.8/IvmDriver/signals/signalroot_matrix.json`

 * *Files identical despite different names*

### Comparing `ivmdriver-0.0.7/IvmDriver/signals/signalroot_matrix1.json` & `ivmdriver-0.0.8/IvmDriver/signals/signalroot_matrix1.json`

 * *Files identical despite different names*

### Comparing `ivmdriver-0.0.7/IvmDriver/styles/app.qss` & `ivmdriver-0.0.8/IvmDriver/styles/app.qss`

 * *Files identical despite different names*

### Comparing `ivmdriver-0.0.7/IvmDriver/styles/scrollAreaFrame.qss` & `ivmdriver-0.0.8/IvmDriver/styles/scrollAreaFrame.qss`

 * *Files identical despite different names*

### Comparing `ivmdriver-0.0.7/IvmDriver.egg-info/PKG-INFO` & `ivmdriver-0.0.8/IvmDriver.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: IvmDriver
-Version: 0.0.7
+Version: 0.0.8
 Home-page: https://github.com/HarishKumarSedu/matrix
 Author: HarishKumarSedu
 Author-email: harishkumarsedu@gmail.com
 Project-URL: Bug Tracker, https://github.com/HarishKumarSedu/matrix/issues
 Description-Content-Type: ['text/plain', 'text/x-rst', 'text/markdown']
 Requires-Dist: pymcp2221a
 Requires-Dist: pyqt5
 Requires-Dist: setuptools
 Requires-Dist: pathlib
 Requires-Dist: PyVISA
+Requires-Dist: rich
 
 # Driver 
 
 - Install py-chill package to freeze python local packages without versioning 
 
 ``` pip install py-chill
     pip-chill --no-version > requirements.txt
```

### Comparing `ivmdriver-0.0.7/IvmDriver.egg-info/SOURCES.txt` & `ivmdriver-0.0.8/IvmDriver.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 IvmDriver/reserach.ipynb
 IvmDriver/signalRoot.py
 IvmDriver.egg-info/PKG-INFO
 IvmDriver.egg-info/SOURCES.txt
 IvmDriver.egg-info/dependency_links.txt
 IvmDriver.egg-info/requires.txt
 IvmDriver.egg-info/top_level.txt
+IvmDriver/GPIOExpander/pcf8547.py
 IvmDriver/assets/logo.ico
 IvmDriver/assets/logo.png
 IvmDriver/docs/DFT Matrix.pptx
 IvmDriver/docs/MCP23017-Data-Sheet-DS20001952.pdf
 IvmDriver/docs/expand-2-click-manual-v100-1484105.pdf
 IvmDriver/signals/SignalConfig.json
 IvmDriver/signals/dummysignalconfig.json
```

### Comparing `ivmdriver-0.0.7/PKG-INFO` & `ivmdriver-0.0.8/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: IvmDriver
-Version: 0.0.7
+Version: 0.0.8
 Home-page: https://github.com/HarishKumarSedu/matrix
 Author: HarishKumarSedu
 Author-email: harishkumarsedu@gmail.com
 Project-URL: Bug Tracker, https://github.com/HarishKumarSedu/matrix/issues
 Description-Content-Type: ['text/plain', 'text/x-rst', 'text/markdown']
 Requires-Dist: pymcp2221a
 Requires-Dist: pyqt5
 Requires-Dist: setuptools
 Requires-Dist: pathlib
 Requires-Dist: PyVISA
+Requires-Dist: rich
 
 # Driver 
 
 - Install py-chill package to freeze python local packages without versioning 
 
 ``` pip install py-chill
     pip-chill --no-version > requirements.txt
```

### Comparing `ivmdriver-0.0.7/setup.py` & `ivmdriver-0.0.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,27 +21,27 @@
 AUTHOR_EMAIL = 'harishkumarsedu@gmail.com'
 REPO_NAME = 'matrix'
 # datafiles = [(datadir, list(glob.glob(os.path.join(datadir, '*'))))]
 setup(
     name=f'IvmDriver',
     author=AUTHOR_USER_NAME,
     author_email=AUTHOR_EMAIL,
-    version='0.0.7',
+    version='0.0.8',
     # py_modules=['src'],
     # description=[ 'text/markdown','text/x-rst'],
     url=f"https://github.com/{AUTHOR_USER_NAME}/{REPO_NAME}",
     project_urls={
         "Bug Tracker": f"https://github.com/{AUTHOR_USER_NAME}/{REPO_NAME}/issues",
     },
     long_description_content_type=['text/plain', 'text/x-rst', 'text/markdown'],
     long_description=long_description,
     packages=find_packages(exclude=['__pycache__']),
     package_data={'static': files},
     include_package_data=True,
     # include_dirs=['IvmDriver'],
     data_files = files,
-    install_requires=['pymcp2221a','pyqt5','setuptools','pathlib','PyVISA'],
+    install_requires=['pymcp2221a','pyqt5','setuptools','pathlib','PyVISA','rich'],
     
 
     
     
 )
```

