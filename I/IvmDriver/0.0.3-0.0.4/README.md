# Comparing `tmp/IvmDriver-0.0.3.tar.gz` & `tmp/IvmDriver-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IvmDriver-0.0.3.tar", last modified: Thu May 23 10:53:17 2024, max compression
+gzip compressed data, was "IvmDriver-0.0.4.tar", last modified: Thu May 23 11:05:34 2024, max compression
```

## Comparing `IvmDriver-0.0.3.tar` & `IvmDriver-0.0.4.tar`

### file list

```diff
@@ -1,65 +1,64 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 10:53:17.893294 IvmDriver-0.0.3/
-drwxrwxrwx   0        0        0        0 2024-05-23 10:53:17.612888 IvmDriver-0.0.3/IvmDriver/
--rw-rw-rw-   0        0        0       18 2024-05-14 07:51:40.000000 IvmDriver-0.0.3/IvmDriver/.gitignore
--rw-rw-rw-   0        0        0      863 2024-05-07 14:46:28.000000 IvmDriver-0.0.3/IvmDriver/DFTMatrix.spec
--rw-rw-rw-   0        0        0      298 2024-05-06 08:56:20.000000 IvmDriver-0.0.3/IvmDriver/Dockerfile
--rw-rw-rw-   0        0        0      339 2024-05-23 10:14:37.000000 IvmDriver-0.0.3/IvmDriver/Matrixgui.py
--rw-rw-rw-   0        0        0      179 2024-05-23 10:16:39.000000 IvmDriver-0.0.3/IvmDriver/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 10:53:17.727512 IvmDriver-0.0.3/IvmDriver/__pycache__/
--rw-rw-rw-   0        0        0      233 2024-04-30 13:51:12.000000 IvmDriver-0.0.3/IvmDriver/__pycache__/__init__.cpython-311.pyc
--rw-rw-rw-   0        0        0    16447 2024-05-07 10:48:50.000000 IvmDriver-0.0.3/IvmDriver/__pycache__/driver.cpython-311.pyc
--rw-rw-rw-   0        0        0      914 2024-04-29 16:06:45.000000 IvmDriver-0.0.3/IvmDriver/__pycache__/logger.cpython-311.pyc
--rw-rw-rw-   0        0        0     9239 2024-05-14 07:42:30.000000 IvmDriver-0.0.3/IvmDriver/__pycache__/mainDriver.cpython-311.pyc
--rw-rw-rw-   0        0        0    92965 2024-05-02 13:08:41.000000 IvmDriver-0.0.3/IvmDriver/__pycache__/matirx.cpython-311.pyc
--rw-rw-rw-   0        0        0   136825 2024-05-07 10:46:15.000000 IvmDriver-0.0.3/IvmDriver/__pycache__/matrix.cpython-311.pyc
--rw-rw-rw-   0        0        0     2074 2024-04-30 13:46:14.000000 IvmDriver-0.0.3/IvmDriver/__pycache__/mcp2221.cpython-311.pyc
--rw-rw-rw-   0        0        0     4390 2024-04-30 14:28:50.000000 IvmDriver-0.0.3/IvmDriver/__pycache__/mcp2317.cpython-311.pyc
--rw-rw-rw-   0        0        0     5988 2024-04-29 16:20:34.000000 IvmDriver-0.0.3/IvmDriver/__pycache__/signalRoot.cpython-311.pyc
--rw-rw-rw-   0        0        0      861 2024-05-07 15:16:00.000000 IvmDriver-0.0.3/IvmDriver/appexe.spec
-drwxrwxrwx   0        0        0        0 2024-05-23 10:53:17.745809 IvmDriver-0.0.3/IvmDriver/assets/
--rw-rw-rw-   0        0        0    67646 2024-05-07 16:08:21.000000 IvmDriver-0.0.3/IvmDriver/assets/logo.ico
--rw-rw-rw-   0        0        0    45518 2024-05-07 16:04:59.000000 IvmDriver-0.0.3/IvmDriver/assets/logo.png
-drwxrwxrwx   0        0        0        0 2024-05-23 10:53:17.463106 IvmDriver-0.0.3/IvmDriver/build/
-drwxrwxrwx   0        0        0        0 2024-05-23 10:53:17.463106 IvmDriver-0.0.3/IvmDriver/build/lib/
-drwxrwxrwx   0        0        0        0 2024-05-23 10:53:17.751408 IvmDriver-0.0.3/IvmDriver/build/lib/src/
--rw-rw-rw-   0        0        0        0 2024-05-23 10:06:06.000000 IvmDriver-0.0.3/IvmDriver/build/lib/src/__init__.py
--rw-rw-rw-   0        0        0        0 2024-05-23 10:03:27.000000 IvmDriver-0.0.3/IvmDriver/build/lib/src/dummy.py
-drwxrwxrwx   0        0        0        0 2024-05-23 10:53:17.800725 IvmDriver-0.0.3/IvmDriver/docs/
--rw-rw-rw-   0        0        0  1722187 2024-04-30 14:57:14.000000 IvmDriver-0.0.3/IvmDriver/docs/DFT Matrix.pptx
--rw-rw-rw-   0        0        0  1019348 2024-04-29 09:16:32.000000 IvmDriver-0.0.3/IvmDriver/docs/MCP23017-Data-Sheet-DS20001952.pdf
--rw-rw-rw-   0        0        0  1049439 2024-04-29 09:16:38.000000 IvmDriver-0.0.3/IvmDriver/docs/expand-2-click-manual-v100-1484105.pdf
--rw-rw-rw-   0        0        0    10640 2024-05-07 10:48:18.000000 IvmDriver-0.0.3/IvmDriver/driver.py
--rw-rw-rw-   0        0        0    13255 2024-05-07 09:46:46.000000 IvmDriver-0.0.3/IvmDriver/driver.ui
--rw-rw-rw-   0        0        0        0 2024-05-02 13:19:09.000000 IvmDriver-0.0.3/IvmDriver/driverPage.py
--rw-rw-rw-   0        0        0      552 2024-05-08 11:50:37.000000 IvmDriver-0.0.3/IvmDriver/exeGenerate.py
--rw-rw-rw-   0        0        0     6451 2024-05-07 09:19:54.000000 IvmDriver-0.0.3/IvmDriver/fileopen.py
--rw-rw-rw-   0        0        0     1104 2024-05-07 14:46:01.000000 IvmDriver-0.0.3/IvmDriver/logger.py
--rw-rw-rw-   0        0        0      865 2024-05-07 15:49:19.000000 IvmDriver-0.0.3/IvmDriver/mainDriver.spec
--rw-rw-rw-   0        0        0    78821 2024-05-07 10:46:12.000000 IvmDriver-0.0.3/IvmDriver/matrix.py
--rw-rw-rw-   0        0        0     4607 2024-05-23 10:14:52.000000 IvmDriver-0.0.3/IvmDriver/matrixDriver.py
--rw-rw-rw-   0        0        0    90133 2024-05-02 15:32:10.000000 IvmDriver-0.0.3/IvmDriver/matrixFrame.ui
--rw-rw-rw-   0        0        0     1069 2024-04-30 13:44:36.000000 IvmDriver-0.0.3/IvmDriver/mcp2221.py
--rw-rw-rw-   0        0        0     3747 2024-04-30 14:24:47.000000 IvmDriver-0.0.3/IvmDriver/mcp2317.py
--rw-rw-rw-   0        0        0      124 2024-05-14 07:48:08.000000 IvmDriver-0.0.3/IvmDriver/requirements.txt
--rw-rw-rw-   0        0        0    22289 2024-04-30 10:16:58.000000 IvmDriver-0.0.3/IvmDriver/reserach.ipynb
--rw-rw-rw-   0        0        0     3986 2024-05-06 09:00:54.000000 IvmDriver-0.0.3/IvmDriver/signalRoot.py
-drwxrwxrwx   0        0        0        0 2024-05-23 10:53:17.871446 IvmDriver-0.0.3/IvmDriver/signals/
--rw-rw-rw-   0        0        0      727 2024-04-30 15:58:16.000000 IvmDriver-0.0.3/IvmDriver/signals/SignalConfig.json
--rw-rw-rw-   0        0        0      391 2024-05-07 09:03:47.000000 IvmDriver-0.0.3/IvmDriver/signals/dummysignalconfig.json
--rw-rw-rw-   0        0        0      391 2024-05-07 11:12:16.000000 IvmDriver-0.0.3/IvmDriver/signals/dummysignalconfig1.json
--rw-rw-rw-   0        0        0      379 2024-04-30 15:33:06.000000 IvmDriver-0.0.3/IvmDriver/signals/intrepretor.json
--rw-rw-rw-   0        0        0      799 2024-04-30 13:52:21.000000 IvmDriver-0.0.3/IvmDriver/signals/signalConfigtest.json
--rw-rw-rw-   0        0        0    19075 2024-04-30 15:58:34.000000 IvmDriver-0.0.3/IvmDriver/signals/signalroot_matrix.json
--rw-rw-rw-   0        0        0    19099 2024-05-08 08:51:46.000000 IvmDriver-0.0.3/IvmDriver/signals/signalroot_matrix1.json
-drwxrwxrwx   0        0        0        0 2024-05-23 10:53:17.883866 IvmDriver-0.0.3/IvmDriver/styles/
--rw-rw-rw-   0        0        0     2895 2024-05-07 09:42:08.000000 IvmDriver-0.0.3/IvmDriver/styles/app.qss
--rw-rw-rw-   0        0        0      711 2024-05-03 10:42:19.000000 IvmDriver-0.0.3/IvmDriver/styles/scrollAreaFrame.qss
-drwxrwxrwx   0        0        0        0 2024-05-23 10:53:17.629448 IvmDriver-0.0.3/IvmDriver.egg-info/
--rw-rw-rw-   0        0        0      637 2024-05-23 10:53:17.000000 IvmDriver-0.0.3/IvmDriver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1642 2024-05-23 10:53:17.000000 IvmDriver-0.0.3/IvmDriver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 10:53:17.000000 IvmDriver-0.0.3/IvmDriver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-05-23 10:53:17.000000 IvmDriver-0.0.3/IvmDriver.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      637 2024-05-23 10:53:17.889896 IvmDriver-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      310 2024-05-23 09:25:33.000000 IvmDriver-0.0.3/README.md
--rw-rw-rw-   0        0        0       42 2024-05-23 10:53:17.893294 IvmDriver-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1487 2024-05-23 10:53:14.000000 IvmDriver-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 11:05:34.642095 IvmDriver-0.0.4/
+drwxrwxrwx   0        0        0        0 2024-05-23 11:05:34.372549 IvmDriver-0.0.4/IvmDriver/
+-rw-rw-rw-   0        0        0       18 2024-05-14 07:51:40.000000 IvmDriver-0.0.4/IvmDriver/.gitignore
+-rw-rw-rw-   0        0        0      863 2024-05-07 14:46:28.000000 IvmDriver-0.0.4/IvmDriver/DFTMatrix.spec
+-rw-rw-rw-   0        0        0      298 2024-05-06 08:56:20.000000 IvmDriver-0.0.4/IvmDriver/Dockerfile
+-rw-rw-rw-   0        0        0      339 2024-05-23 10:14:37.000000 IvmDriver-0.0.4/IvmDriver/Matrixgui.py
+-rw-rw-rw-   0        0        0      179 2024-05-23 10:16:39.000000 IvmDriver-0.0.4/IvmDriver/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 11:05:34.466919 IvmDriver-0.0.4/IvmDriver/__pycache__/
+-rw-rw-rw-   0        0        0      233 2024-04-30 13:51:12.000000 IvmDriver-0.0.4/IvmDriver/__pycache__/__init__.cpython-311.pyc
+-rw-rw-rw-   0        0        0    16447 2024-05-07 10:48:50.000000 IvmDriver-0.0.4/IvmDriver/__pycache__/driver.cpython-311.pyc
+-rw-rw-rw-   0        0        0      914 2024-04-29 16:06:45.000000 IvmDriver-0.0.4/IvmDriver/__pycache__/logger.cpython-311.pyc
+-rw-rw-rw-   0        0        0     9239 2024-05-14 07:42:30.000000 IvmDriver-0.0.4/IvmDriver/__pycache__/mainDriver.cpython-311.pyc
+-rw-rw-rw-   0        0        0    92965 2024-05-02 13:08:41.000000 IvmDriver-0.0.4/IvmDriver/__pycache__/matirx.cpython-311.pyc
+-rw-rw-rw-   0        0        0   136825 2024-05-07 10:46:15.000000 IvmDriver-0.0.4/IvmDriver/__pycache__/matrix.cpython-311.pyc
+-rw-rw-rw-   0        0        0     2074 2024-04-30 13:46:14.000000 IvmDriver-0.0.4/IvmDriver/__pycache__/mcp2221.cpython-311.pyc
+-rw-rw-rw-   0        0        0     4390 2024-04-30 14:28:50.000000 IvmDriver-0.0.4/IvmDriver/__pycache__/mcp2317.cpython-311.pyc
+-rw-rw-rw-   0        0        0     5988 2024-04-29 16:20:34.000000 IvmDriver-0.0.4/IvmDriver/__pycache__/signalRoot.cpython-311.pyc
+-rw-rw-rw-   0        0        0      861 2024-05-07 15:16:00.000000 IvmDriver-0.0.4/IvmDriver/appexe.spec
+drwxrwxrwx   0        0        0        0 2024-05-23 11:05:34.479580 IvmDriver-0.0.4/IvmDriver/assets/
+-rw-rw-rw-   0        0        0    67646 2024-05-07 16:08:21.000000 IvmDriver-0.0.4/IvmDriver/assets/logo.ico
+-rw-rw-rw-   0        0        0    45518 2024-05-07 16:04:59.000000 IvmDriver-0.0.4/IvmDriver/assets/logo.png
+drwxrwxrwx   0        0        0        0 2024-05-23 11:05:34.177709 IvmDriver-0.0.4/IvmDriver/build/
+drwxrwxrwx   0        0        0        0 2024-05-23 11:05:34.178709 IvmDriver-0.0.4/IvmDriver/build/lib/
+drwxrwxrwx   0        0        0        0 2024-05-23 11:05:34.485235 IvmDriver-0.0.4/IvmDriver/build/lib/src/
+-rw-rw-rw-   0        0        0        0 2024-05-23 10:06:06.000000 IvmDriver-0.0.4/IvmDriver/build/lib/src/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-05-23 10:03:27.000000 IvmDriver-0.0.4/IvmDriver/build/lib/src/dummy.py
+drwxrwxrwx   0        0        0        0 2024-05-23 11:05:34.545799 IvmDriver-0.0.4/IvmDriver/docs/
+-rw-rw-rw-   0        0        0  1722187 2024-04-30 14:57:14.000000 IvmDriver-0.0.4/IvmDriver/docs/DFT Matrix.pptx
+-rw-rw-rw-   0        0        0  1019348 2024-04-29 09:16:32.000000 IvmDriver-0.0.4/IvmDriver/docs/MCP23017-Data-Sheet-DS20001952.pdf
+-rw-rw-rw-   0        0        0  1049439 2024-04-29 09:16:38.000000 IvmDriver-0.0.4/IvmDriver/docs/expand-2-click-manual-v100-1484105.pdf
+-rw-rw-rw-   0        0        0    10640 2024-05-07 10:48:18.000000 IvmDriver-0.0.4/IvmDriver/driver.py
+-rw-rw-rw-   0        0        0    13255 2024-05-07 09:46:46.000000 IvmDriver-0.0.4/IvmDriver/driver.ui
+-rw-rw-rw-   0        0        0        0 2024-05-02 13:19:09.000000 IvmDriver-0.0.4/IvmDriver/driverPage.py
+-rw-rw-rw-   0        0        0      552 2024-05-08 11:50:37.000000 IvmDriver-0.0.4/IvmDriver/exeGenerate.py
+-rw-rw-rw-   0        0        0     6451 2024-05-07 09:19:54.000000 IvmDriver-0.0.4/IvmDriver/fileopen.py
+-rw-rw-rw-   0        0        0     1104 2024-05-07 14:46:01.000000 IvmDriver-0.0.4/IvmDriver/logger.py
+-rw-rw-rw-   0        0        0      865 2024-05-07 15:49:19.000000 IvmDriver-0.0.4/IvmDriver/mainDriver.spec
+-rw-rw-rw-   0        0        0    78821 2024-05-07 10:46:12.000000 IvmDriver-0.0.4/IvmDriver/matrix.py
+-rw-rw-rw-   0        0        0     4607 2024-05-23 10:14:52.000000 IvmDriver-0.0.4/IvmDriver/matrixDriver.py
+-rw-rw-rw-   0        0        0    90133 2024-05-02 15:32:10.000000 IvmDriver-0.0.4/IvmDriver/matrixFrame.ui
+-rw-rw-rw-   0        0        0     1069 2024-04-30 13:44:36.000000 IvmDriver-0.0.4/IvmDriver/mcp2221.py
+-rw-rw-rw-   0        0        0     3747 2024-04-30 14:24:47.000000 IvmDriver-0.0.4/IvmDriver/mcp2317.py
+-rw-rw-rw-   0        0        0    22289 2024-04-30 10:16:58.000000 IvmDriver-0.0.4/IvmDriver/reserach.ipynb
+-rw-rw-rw-   0        0        0     3986 2024-05-06 09:00:54.000000 IvmDriver-0.0.4/IvmDriver/signalRoot.py
+drwxrwxrwx   0        0        0        0 2024-05-23 11:05:34.610925 IvmDriver-0.0.4/IvmDriver/signals/
+-rw-rw-rw-   0        0        0      727 2024-04-30 15:58:16.000000 IvmDriver-0.0.4/IvmDriver/signals/SignalConfig.json
+-rw-rw-rw-   0        0        0      391 2024-05-07 09:03:47.000000 IvmDriver-0.0.4/IvmDriver/signals/dummysignalconfig.json
+-rw-rw-rw-   0        0        0      391 2024-05-07 11:12:16.000000 IvmDriver-0.0.4/IvmDriver/signals/dummysignalconfig1.json
+-rw-rw-rw-   0        0        0      379 2024-04-30 15:33:06.000000 IvmDriver-0.0.4/IvmDriver/signals/intrepretor.json
+-rw-rw-rw-   0        0        0      799 2024-04-30 13:52:21.000000 IvmDriver-0.0.4/IvmDriver/signals/signalConfigtest.json
+-rw-rw-rw-   0        0        0    19075 2024-04-30 15:58:34.000000 IvmDriver-0.0.4/IvmDriver/signals/signalroot_matrix.json
+-rw-rw-rw-   0        0        0    19099 2024-05-08 08:51:46.000000 IvmDriver-0.0.4/IvmDriver/signals/signalroot_matrix1.json
+drwxrwxrwx   0        0        0        0 2024-05-23 11:05:34.634043 IvmDriver-0.0.4/IvmDriver/styles/
+-rw-rw-rw-   0        0        0     2895 2024-05-07 09:42:08.000000 IvmDriver-0.0.4/IvmDriver/styles/app.qss
+-rw-rw-rw-   0        0        0      711 2024-05-03 10:42:19.000000 IvmDriver-0.0.4/IvmDriver/styles/scrollAreaFrame.qss
+drwxrwxrwx   0        0        0        0 2024-05-23 11:05:34.390872 IvmDriver-0.0.4/IvmDriver.egg-info/
+-rw-rw-rw-   0        0        0      735 2024-05-23 11:05:33.000000 IvmDriver-0.0.4/IvmDriver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1615 2024-05-23 11:05:34.000000 IvmDriver-0.0.4/IvmDriver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 11:05:34.000000 IvmDriver-0.0.4/IvmDriver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-05-23 11:05:34.000000 IvmDriver-0.0.4/IvmDriver.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      735 2024-05-23 11:05:34.638054 IvmDriver-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      310 2024-05-23 09:25:33.000000 IvmDriver-0.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-23 11:05:34.642095 IvmDriver-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1552 2024-05-23 11:05:27.000000 IvmDriver-0.0.4/setup.py
```

### Comparing `IvmDriver-0.0.3/IvmDriver/DFTMatrix.spec` & `IvmDriver-0.0.4/IvmDriver/DFTMatrix.spec`

 * *Files identical despite different names*

### Comparing `IvmDriver-0.0.3/IvmDriver/__pycache__/driver.cpython-311.pyc` & `IvmDriver-0.0.4/IvmDriver/__pycache__/driver.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `IvmDriver-0.0.3/IvmDriver/__pycache__/logger.cpython-311.pyc` & `IvmDriver-0.0.4/IvmDriver/__pycache__/logger.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `IvmDriver-0.0.3/IvmDriver/__pycache__/mainDriver.cpython-311.pyc` & `IvmDriver-0.0.4/IvmDriver/__pycache__/mainDriver.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `IvmDriver-0.0.3/IvmDriver/__pycache__/matirx.cpython-311.pyc` & `IvmDriver-0.0.4/IvmDriver/__pycache__/matirx.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `IvmDriver-0.0.3/IvmDriver/__pycache__/matrix.cpython-311.pyc` & `IvmDriver-0.0.4/IvmDriver/__pycache__/matrix.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `IvmDriver-0.0.3/IvmDriver/__pycache__/mcp2221.cpython-311.pyc` & `IvmDriver-0.0.4/IvmDriver/__pycache__/mcp2221.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `IvmDriver-0.0.3/IvmDriver/__pycache__/mcp2317.cpython-311.pyc` & `IvmDriver-0.0.4/IvmDriver/__pycache__/mcp2317.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `IvmDriver-0.0.3/IvmDriver/__pycache__/signalRoot.cpython-311.pyc` & `IvmDriver-0.0.4/IvmDriver/__pycache__/signalRoot.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `IvmDriver-0.0.3/IvmDriver/appexe.spec` & `IvmDriver-0.0.4/IvmDriver/appexe.spec`

 * *Files identical despite different names*

### Comparing `IvmDriver-0.0.3/IvmDriver/assets/logo.ico` & `IvmDriver-0.0.4/IvmDriver/assets/logo.ico`

 * *Files identical despite different names*

### Comparing `IvmDriver-0.0.3/IvmDriver/assets/logo.png` & `IvmDriver-0.0.4/IvmDriver/assets/logo.png`

 * *Files identical despite different names*

### Comparing `IvmDriver-0.0.3/IvmDriver/docs/DFT Matrix.pptx` & `IvmDriver-0.0.4/IvmDriver/docs/DFT Matrix.pptx`

 * *Files identical despite different names*

### Comparing `IvmDriver-0.0.3/IvmDriver/docs/MCP23017-Data-Sheet-DS20001952.pdf` & `IvmDriver-0.0.4/IvmDriver/docs/MCP23017-Data-Sheet-DS20001952.pdf`

 * *Files identical despite different names*

### Comparing `IvmDriver-0.0.3/IvmDriver/docs/expand-2-click-manual-v100-1484105.pdf` & `IvmDriver-0.0.4/IvmDriver/docs/expand-2-click-manual-v100-1484105.pdf`

 * *Files identical despite different names*

### Comparing `IvmDriver-0.0.3/IvmDriver/driver.py` & `IvmDriver-0.0.4/IvmDriver/driver.py`

 * *Files identical despite different names*

### Comparing `IvmDriver-0.0.3/IvmDriver/driver.ui` & `IvmDriver-0.0.4/IvmDriver/driver.ui`

 * *Files identical despite different names*

### Comparing `IvmDriver-0.0.3/IvmDriver/exeGenerate.py` & `IvmDriver-0.0.4/IvmDriver/exeGenerate.py`

 * *Files identical despite different names*

### Comparing `IvmDriver-0.0.3/IvmDriver/fileopen.py` & `IvmDriver-0.0.4/IvmDriver/fileopen.py`

 * *Files identical despite different names*

### Comparing `IvmDriver-0.0.3/IvmDriver/logger.py` & `IvmDriver-0.0.4/IvmDriver/logger.py`

 * *Files identical despite different names*

### Comparing `IvmDriver-0.0.3/IvmDriver/mainDriver.spec` & `IvmDriver-0.0.4/IvmDriver/mainDriver.spec`

 * *Files identical despite different names*

### Comparing `IvmDriver-0.0.3/IvmDriver/matrix.py` & `IvmDriver-0.0.4/IvmDriver/matrix.py`

 * *Files identical despite different names*

### Comparing `IvmDriver-0.0.3/IvmDriver/matrixDriver.py` & `IvmDriver-0.0.4/IvmDriver/matrixDriver.py`

 * *Files identical despite different names*

### Comparing `IvmDriver-0.0.3/IvmDriver/matrixFrame.ui` & `IvmDriver-0.0.4/IvmDriver/matrixFrame.ui`

 * *Files identical despite different names*

### Comparing `IvmDriver-0.0.3/IvmDriver/mcp2221.py` & `IvmDriver-0.0.4/IvmDriver/mcp2221.py`

 * *Files identical despite different names*

### Comparing `IvmDriver-0.0.3/IvmDriver/mcp2317.py` & `IvmDriver-0.0.4/IvmDriver/mcp2317.py`

 * *Files identical despite different names*

### Comparing `IvmDriver-0.0.3/IvmDriver/reserach.ipynb` & `IvmDriver-0.0.4/IvmDriver/reserach.ipynb`

 * *Files identical despite different names*

### Comparing `IvmDriver-0.0.3/IvmDriver/signalRoot.py` & `IvmDriver-0.0.4/IvmDriver/signalRoot.py`

 * *Files identical despite different names*

### Comparing `IvmDriver-0.0.3/IvmDriver/signals/SignalConfig.json` & `IvmDriver-0.0.4/IvmDriver/signals/SignalConfig.json`

 * *Files identical despite different names*

### Comparing `IvmDriver-0.0.3/IvmDriver/signals/signalConfigtest.json` & `IvmDriver-0.0.4/IvmDriver/signals/signalConfigtest.json`

 * *Files identical despite different names*

### Comparing `IvmDriver-0.0.3/IvmDriver/signals/signalroot_matrix.json` & `IvmDriver-0.0.4/IvmDriver/signals/signalroot_matrix.json`

 * *Files identical despite different names*

### Comparing `IvmDriver-0.0.3/IvmDriver/signals/signalroot_matrix1.json` & `IvmDriver-0.0.4/IvmDriver/signals/signalroot_matrix1.json`

 * *Files identical despite different names*

### Comparing `IvmDriver-0.0.3/IvmDriver/styles/app.qss` & `IvmDriver-0.0.4/IvmDriver/styles/app.qss`

 * *Files identical despite different names*

### Comparing `IvmDriver-0.0.3/IvmDriver/styles/scrollAreaFrame.qss` & `IvmDriver-0.0.4/IvmDriver/styles/scrollAreaFrame.qss`

 * *Files identical despite different names*

### Comparing `IvmDriver-0.0.3/IvmDriver.egg-info/SOURCES.txt` & `IvmDriver-0.0.4/IvmDriver.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 IvmDriver/logger.py
 IvmDriver/mainDriver.spec
 IvmDriver/matrix.py
 IvmDriver/matrixDriver.py
 IvmDriver/matrixFrame.ui
 IvmDriver/mcp2221.py
 IvmDriver/mcp2317.py
-IvmDriver/requirements.txt
 IvmDriver/reserach.ipynb
 IvmDriver/signalRoot.py
 IvmDriver.egg-info/PKG-INFO
 IvmDriver.egg-info/SOURCES.txt
 IvmDriver.egg-info/dependency_links.txt
 IvmDriver.egg-info/top_level.txt
 IvmDriver/__pycache__/__init__.cpython-311.pyc
```

### Comparing `IvmDriver-0.0.3/setup.py` & `IvmDriver-0.0.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from setuptools import setup, find_packages
-
 import pathlib
 import os 
 files = []
 def list_files_scandir(path='./IvmDriver'):
     with os.scandir(path) as entries:
         for entry in entries:
             if entry.is_file():
@@ -12,36 +11,36 @@
             elif entry.is_dir():
                 list_files_scandir(entry.path)
  
 # Specify the directory path you want to start from
 directory_path = './IvmDriver'
 list_files_scandir(directory_path)
 
-
 with open('./README.md', 'r') as file :
     long_description = file.read()
 AUTHOR_USER_NAME = 'HarishKumarSedu'
 AUTHOR_EMAIL = 'harishkumarsedu@gmail.com'
 REPO_NAME = 'matrix'
 # datafiles = [(datadir, list(glob.glob(os.path.join(datadir, '*'))))]
 setup(
     name=f'IvmDriver',
     author=AUTHOR_USER_NAME,
     author_email=AUTHOR_EMAIL,
-    version='0.0.3',
+    version='0.0.4',
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
+    requires=['pymcp2221a','pyqt5','setuptools','pathlib','PyVISA']
 
     
     
 )
```

