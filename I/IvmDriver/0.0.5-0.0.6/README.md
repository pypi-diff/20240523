# Comparing `tmp/ivmdriver-0.0.5.tar.gz` & `tmp/ivmdriver-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ivmdriver-0.0.5.tar", last modified: Thu May 23 11:14:34 2024, max compression
+gzip compressed data, was "ivmdriver-0.0.6.tar", last modified: Thu May 23 11:47:35 2024, max compression
```

## Comparing `ivmdriver-0.0.5.tar` & `ivmdriver-0.0.6.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:14:34.631993 ivmdriver-0.0.5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:14:34.619993 ivmdriver-0.0.5/IvmDriver/
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-23 11:14:18.000000 ivmdriver-0.0.5/IvmDriver/DFTMatrix.spec
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-23 11:14:18.000000 ivmdriver-0.0.5/IvmDriver/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-23 11:14:18.000000 ivmdriver-0.0.5/IvmDriver/Matrixgui.py
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-23 11:14:18.000000 ivmdriver-0.0.5/IvmDriver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-23 11:14:18.000000 ivmdriver-0.0.5/IvmDriver/appexe.spec
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:14:34.623993 ivmdriver-0.0.5/IvmDriver/assets/
--rw-r--r--   0 runner    (1001) docker     (127)    67646 2024-05-23 11:14:18.000000 ivmdriver-0.0.5/IvmDriver/assets/logo.ico
--rw-r--r--   0 runner    (1001) docker     (127)    45518 2024-05-23 11:14:18.000000 ivmdriver-0.0.5/IvmDriver/assets/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:14:34.627992 ivmdriver-0.0.5/IvmDriver/docs/
--rw-r--r--   0 runner    (1001) docker     (127)  1722187 2024-05-23 11:14:18.000000 ivmdriver-0.0.5/IvmDriver/docs/DFT Matrix.pptx
--rw-r--r--   0 runner    (1001) docker     (127)  1019348 2024-05-23 11:14:18.000000 ivmdriver-0.0.5/IvmDriver/docs/MCP23017-Data-Sheet-DS20001952.pdf
--rw-r--r--   0 runner    (1001) docker     (127)  1049439 2024-05-23 11:14:18.000000 ivmdriver-0.0.5/IvmDriver/docs/expand-2-click-manual-v100-1484105.pdf
--rw-r--r--   0 runner    (1001) docker     (127)    10458 2024-05-23 11:14:18.000000 ivmdriver-0.0.5/IvmDriver/driver.py
--rw-r--r--   0 runner    (1001) docker     (127)    12828 2024-05-23 11:14:18.000000 ivmdriver-0.0.5/IvmDriver/driver.ui
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 11:14:18.000000 ivmdriver-0.0.5/IvmDriver/driverPage.py
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-23 11:14:18.000000 ivmdriver-0.0.5/IvmDriver/exeGenerate.py
--rw-r--r--   0 runner    (1001) docker     (127)     6295 2024-05-23 11:14:18.000000 ivmdriver-0.0.5/IvmDriver/fileopen.py
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-23 11:14:18.000000 ivmdriver-0.0.5/IvmDriver/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-23 11:14:18.000000 ivmdriver-0.0.5/IvmDriver/mainDriver.spec
--rw-r--r--   0 runner    (1001) docker     (127)    77406 2024-05-23 11:14:18.000000 ivmdriver-0.0.5/IvmDriver/matrix.py
--rw-r--r--   0 runner    (1001) docker     (127)     4492 2024-05-23 11:14:18.000000 ivmdriver-0.0.5/IvmDriver/matrixDriver.py
--rw-r--r--   0 runner    (1001) docker     (127)    87565 2024-05-23 11:14:18.000000 ivmdriver-0.0.5/IvmDriver/matrixFrame.ui
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-23 11:14:18.000000 ivmdriver-0.0.5/IvmDriver/mcp2221.py
--rw-r--r--   0 runner    (1001) docker     (127)     3666 2024-05-23 11:14:18.000000 ivmdriver-0.0.5/IvmDriver/mcp2317.py
--rw-r--r--   0 runner    (1001) docker     (127)    22289 2024-05-23 11:14:18.000000 ivmdriver-0.0.5/IvmDriver/reserach.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     3904 2024-05-23 11:14:18.000000 ivmdriver-0.0.5/IvmDriver/signalRoot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:14:34.627992 ivmdriver-0.0.5/IvmDriver/signals/
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-23 11:14:18.000000 ivmdriver-0.0.5/IvmDriver/signals/SignalConfig.json
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-23 11:14:18.000000 ivmdriver-0.0.5/IvmDriver/signals/dummysignalconfig.json
--rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-23 11:14:18.000000 ivmdriver-0.0.5/IvmDriver/signals/dummysignalconfig1.json
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-23 11:14:18.000000 ivmdriver-0.0.5/IvmDriver/signals/intrepretor.json
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-23 11:14:18.000000 ivmdriver-0.0.5/IvmDriver/signals/signalConfigtest.json
--rw-r--r--   0 runner    (1001) docker     (127)    18653 2024-05-23 11:14:18.000000 ivmdriver-0.0.5/IvmDriver/signals/signalroot_matrix.json
--rw-r--r--   0 runner    (1001) docker     (127)    18675 2024-05-23 11:14:18.000000 ivmdriver-0.0.5/IvmDriver/signals/signalroot_matrix1.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:14:34.627992 ivmdriver-0.0.5/IvmDriver/styles/
--rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-05-23 11:14:18.000000 ivmdriver-0.0.5/IvmDriver/styles/app.qss
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-23 11:14:18.000000 ivmdriver-0.0.5/IvmDriver/styles/scrollAreaFrame.qss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:14:34.627992 ivmdriver-0.0.5/IvmDriver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-23 11:14:34.000000 ivmdriver-0.0.5/IvmDriver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-23 11:14:34.000000 ivmdriver-0.0.5/IvmDriver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 11:14:34.000000 ivmdriver-0.0.5/IvmDriver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-23 11:14:34.000000 ivmdriver-0.0.5/IvmDriver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-23 11:14:34.000000 ivmdriver-0.0.5/IvmDriver.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-23 11:14:34.627992 ivmdriver-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-23 11:14:18.000000 ivmdriver-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 11:14:34.631993 ivmdriver-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-05-23 11:14:18.000000 ivmdriver-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:47:35.519399 ivmdriver-0.0.6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:47:35.511399 ivmdriver-0.0.6/IvmDriver/
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-23 11:47:20.000000 ivmdriver-0.0.6/IvmDriver/DFTMatrix.spec
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-23 11:47:20.000000 ivmdriver-0.0.6/IvmDriver/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-23 11:47:20.000000 ivmdriver-0.0.6/IvmDriver/Matrixgui.py
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-23 11:47:20.000000 ivmdriver-0.0.6/IvmDriver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-23 11:47:20.000000 ivmdriver-0.0.6/IvmDriver/appexe.spec
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:47:35.511399 ivmdriver-0.0.6/IvmDriver/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)    67646 2024-05-23 11:47:20.000000 ivmdriver-0.0.6/IvmDriver/assets/logo.ico
+-rw-r--r--   0 runner    (1001) docker     (127)    45518 2024-05-23 11:47:20.000000 ivmdriver-0.0.6/IvmDriver/assets/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:47:35.515399 ivmdriver-0.0.6/IvmDriver/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)  1722187 2024-05-23 11:47:20.000000 ivmdriver-0.0.6/IvmDriver/docs/DFT Matrix.pptx
+-rw-r--r--   0 runner    (1001) docker     (127)  1019348 2024-05-23 11:47:20.000000 ivmdriver-0.0.6/IvmDriver/docs/MCP23017-Data-Sheet-DS20001952.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)  1049439 2024-05-23 11:47:20.000000 ivmdriver-0.0.6/IvmDriver/docs/expand-2-click-manual-v100-1484105.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)    10458 2024-05-23 11:47:20.000000 ivmdriver-0.0.6/IvmDriver/driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12828 2024-05-23 11:47:20.000000 ivmdriver-0.0.6/IvmDriver/driver.ui
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 11:47:20.000000 ivmdriver-0.0.6/IvmDriver/driverPage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-05-23 11:47:20.000000 ivmdriver-0.0.6/IvmDriver/exeGenerate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6295 2024-05-23 11:47:20.000000 ivmdriver-0.0.6/IvmDriver/fileopen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-23 11:47:20.000000 ivmdriver-0.0.6/IvmDriver/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-23 11:47:20.000000 ivmdriver-0.0.6/IvmDriver/mainDriver.spec
+-rw-r--r--   0 runner    (1001) docker     (127)    77406 2024-05-23 11:47:20.000000 ivmdriver-0.0.6/IvmDriver/matrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4621 2024-05-23 11:47:20.000000 ivmdriver-0.0.6/IvmDriver/matrixDriver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    87565 2024-05-23 11:47:20.000000 ivmdriver-0.0.6/IvmDriver/matrixFrame.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-05-23 11:47:20.000000 ivmdriver-0.0.6/IvmDriver/mcp2221.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3666 2024-05-23 11:47:20.000000 ivmdriver-0.0.6/IvmDriver/mcp2317.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22289 2024-05-23 11:47:20.000000 ivmdriver-0.0.6/IvmDriver/reserach.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3904 2024-05-23 11:47:20.000000 ivmdriver-0.0.6/IvmDriver/signalRoot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:47:35.515399 ivmdriver-0.0.6/IvmDriver/signals/
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-23 11:47:20.000000 ivmdriver-0.0.6/IvmDriver/signals/SignalConfig.json
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-23 11:47:20.000000 ivmdriver-0.0.6/IvmDriver/signals/dummysignalconfig.json
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-23 11:47:20.000000 ivmdriver-0.0.6/IvmDriver/signals/dummysignalconfig1.json
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-23 11:47:20.000000 ivmdriver-0.0.6/IvmDriver/signals/intrepretor.json
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-23 11:47:20.000000 ivmdriver-0.0.6/IvmDriver/signals/signalConfigtest.json
+-rw-r--r--   0 runner    (1001) docker     (127)    18653 2024-05-23 11:47:20.000000 ivmdriver-0.0.6/IvmDriver/signals/signalroot_matrix.json
+-rw-r--r--   0 runner    (1001) docker     (127)    18675 2024-05-23 11:47:20.000000 ivmdriver-0.0.6/IvmDriver/signals/signalroot_matrix1.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:47:35.515399 ivmdriver-0.0.6/IvmDriver/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-05-23 11:47:20.000000 ivmdriver-0.0.6/IvmDriver/styles/app.qss
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-23 11:47:20.000000 ivmdriver-0.0.6/IvmDriver/styles/scrollAreaFrame.qss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 11:47:35.515399 ivmdriver-0.0.6/IvmDriver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-23 11:47:35.000000 ivmdriver-0.0.6/IvmDriver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-23 11:47:35.000000 ivmdriver-0.0.6/IvmDriver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 11:47:35.000000 ivmdriver-0.0.6/IvmDriver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-23 11:47:35.000000 ivmdriver-0.0.6/IvmDriver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-23 11:47:35.000000 ivmdriver-0.0.6/IvmDriver.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-23 11:47:35.519399 ivmdriver-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-23 11:47:20.000000 ivmdriver-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 11:47:35.519399 ivmdriver-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-05-23 11:47:20.000000 ivmdriver-0.0.6/setup.py
```

### Comparing `ivmdriver-0.0.5/IvmDriver/DFTMatrix.spec` & `ivmdriver-0.0.6/IvmDriver/DFTMatrix.spec`

 * *Files identical despite different names*

### Comparing `ivmdriver-0.0.5/IvmDriver/appexe.spec` & `ivmdriver-0.0.6/IvmDriver/appexe.spec`

 * *Files identical despite different names*

### Comparing `ivmdriver-0.0.5/IvmDriver/assets/logo.ico` & `ivmdriver-0.0.6/IvmDriver/assets/logo.ico`

 * *Files identical despite different names*

### Comparing `ivmdriver-0.0.5/IvmDriver/assets/logo.png` & `ivmdriver-0.0.6/IvmDriver/assets/logo.png`

 * *Files identical despite different names*

### Comparing `ivmdriver-0.0.5/IvmDriver/docs/DFT Matrix.pptx` & `ivmdriver-0.0.6/IvmDriver/docs/DFT Matrix.pptx`

 * *Files identical despite different names*

### Comparing `ivmdriver-0.0.5/IvmDriver/docs/MCP23017-Data-Sheet-DS20001952.pdf` & `ivmdriver-0.0.6/IvmDriver/docs/MCP23017-Data-Sheet-DS20001952.pdf`

 * *Files identical despite different names*

### Comparing `ivmdriver-0.0.5/IvmDriver/docs/expand-2-click-manual-v100-1484105.pdf` & `ivmdriver-0.0.6/IvmDriver/docs/expand-2-click-manual-v100-1484105.pdf`

 * *Files identical despite different names*

### Comparing `ivmdriver-0.0.5/IvmDriver/driver.py` & `ivmdriver-0.0.6/IvmDriver/driver.py`

 * *Files identical despite different names*

### Comparing `ivmdriver-0.0.5/IvmDriver/driver.ui` & `ivmdriver-0.0.6/IvmDriver/driver.ui`

 * *Files identical despite different names*

### Comparing `ivmdriver-0.0.5/IvmDriver/exeGenerate.py` & `ivmdriver-0.0.6/IvmDriver/exeGenerate.py`

 * *Files identical despite different names*

### Comparing `ivmdriver-0.0.5/IvmDriver/fileopen.py` & `ivmdriver-0.0.6/IvmDriver/fileopen.py`

 * *Files identical despite different names*

### Comparing `ivmdriver-0.0.5/IvmDriver/logger.py` & `ivmdriver-0.0.6/IvmDriver/logger.py`

 * *Files identical despite different names*

### Comparing `ivmdriver-0.0.5/IvmDriver/mainDriver.spec` & `ivmdriver-0.0.6/IvmDriver/mainDriver.spec`

 * *Files identical despite different names*

### Comparing `ivmdriver-0.0.5/IvmDriver/matrix.py` & `ivmdriver-0.0.6/IvmDriver/matrix.py`

 * *Files identical despite different names*

### Comparing `ivmdriver-0.0.5/IvmDriver/matrixDriver.py` & `ivmdriver-0.0.6/IvmDriver/matrixDriver.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,17 +21,16 @@
         self.lockConfigPushButton.clicked.connect(self.lockConfig)
         self.generateConfigPushButton.clicked.connect(self.generateConfig)
         self.loadMatrix.clicked.connect(self.loadMatrixConfigFile)
         
         self.closeButton.clicked.connect(self.mainWindowClosing) # type: ignore
         self.matrixLayout = {}
         self.matrixIndex = 0
-        with open('styles/app.qss',"r") as appStyles :
-            app.setStyleSheet(appStyles.read())
-    
+        with open(os.path.join(os.path.dirname(__file__),'styles/scrollAreaFrame.qss'), 'r') as file:
+            self.scrollArea.setStyleSheet(file.read())
     def mainWindowClosing(self):
         for _,matrix in self.matrixLayout.items():
             sleep(1)
             matrix.locked = True
             matrix.freezeLineEdit()
         self.close()
     def mousePressEvent(self, event):
@@ -97,19 +96,19 @@
                         self.matrixLayout[literal_eval(matrix)].setSignalText(data=literal_eval(path), relay=data.get('relay'))
         except :
             print('File is not loaded')
             
 def MatrixDriver_gui():
     app = QtWidgets.QApplication(sys.argv)
     window = MatrixDriver()
-    with open('styles/app.qss',"r") as appStyles :
+    with open(os.path.join(os.path.dirname(__file__),'styles/app.qss'),"r") as appStyles :
         app.setStyleSheet(appStyles.read())
     window.show()
     sys.exit(app.exec())
     
 if __name__ == '__main__':
     app = QtWidgets.QApplication(sys.argv)
     window = MatrixDriver()
-    with open('styles/app.qss',"r") as appStyles :
+    with open(os.path.join(os.path.dirname(__file__),'styles/app.qss'),"r") as appStyles :
         app.setStyleSheet(appStyles.read())
     window.show()
     sys.exit(app.exec())
```

### Comparing `ivmdriver-0.0.5/IvmDriver/matrixFrame.ui` & `ivmdriver-0.0.6/IvmDriver/matrixFrame.ui`

 * *Files identical despite different names*

### Comparing `ivmdriver-0.0.5/IvmDriver/mcp2221.py` & `ivmdriver-0.0.6/IvmDriver/mcp2221.py`

 * *Files identical despite different names*

### Comparing `ivmdriver-0.0.5/IvmDriver/mcp2317.py` & `ivmdriver-0.0.6/IvmDriver/mcp2317.py`

 * *Files identical despite different names*

### Comparing `ivmdriver-0.0.5/IvmDriver/reserach.ipynb` & `ivmdriver-0.0.6/IvmDriver/reserach.ipynb`

 * *Files identical despite different names*

### Comparing `ivmdriver-0.0.5/IvmDriver/signalRoot.py` & `ivmdriver-0.0.6/IvmDriver/signalRoot.py`

 * *Files identical despite different names*

### Comparing `ivmdriver-0.0.5/IvmDriver/signals/SignalConfig.json` & `ivmdriver-0.0.6/IvmDriver/signals/SignalConfig.json`

 * *Files identical despite different names*

### Comparing `ivmdriver-0.0.5/IvmDriver/signals/signalConfigtest.json` & `ivmdriver-0.0.6/IvmDriver/signals/signalConfigtest.json`

 * *Files identical despite different names*

### Comparing `ivmdriver-0.0.5/IvmDriver/signals/signalroot_matrix.json` & `ivmdriver-0.0.6/IvmDriver/signals/signalroot_matrix.json`

 * *Files identical despite different names*

### Comparing `ivmdriver-0.0.5/IvmDriver/signals/signalroot_matrix1.json` & `ivmdriver-0.0.6/IvmDriver/signals/signalroot_matrix1.json`

 * *Files identical despite different names*

### Comparing `ivmdriver-0.0.5/IvmDriver/styles/app.qss` & `ivmdriver-0.0.6/IvmDriver/styles/app.qss`

 * *Files identical despite different names*

### Comparing `ivmdriver-0.0.5/IvmDriver/styles/scrollAreaFrame.qss` & `ivmdriver-0.0.6/IvmDriver/styles/scrollAreaFrame.qss`

 * *Files identical despite different names*

### Comparing `ivmdriver-0.0.5/IvmDriver.egg-info/PKG-INFO` & `ivmdriver-0.0.6/IvmDriver.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IvmDriver
-Version: 0.0.5
+Version: 0.0.6
 Home-page: https://github.com/HarishKumarSedu/matrix
 Author: HarishKumarSedu
 Author-email: harishkumarsedu@gmail.com
 Project-URL: Bug Tracker, https://github.com/HarishKumarSedu/matrix/issues
 Description-Content-Type: ['text/plain', 'text/x-rst', 'text/markdown']
 Requires-Dist: pymcp2221a
 Requires-Dist: pyqt5
```

### Comparing `ivmdriver-0.0.5/IvmDriver.egg-info/SOURCES.txt` & `ivmdriver-0.0.6/IvmDriver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ivmdriver-0.0.5/PKG-INFO` & `ivmdriver-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IvmDriver
-Version: 0.0.5
+Version: 0.0.6
 Home-page: https://github.com/HarishKumarSedu/matrix
 Author: HarishKumarSedu
 Author-email: harishkumarsedu@gmail.com
 Project-URL: Bug Tracker, https://github.com/HarishKumarSedu/matrix/issues
 Description-Content-Type: ['text/plain', 'text/x-rst', 'text/markdown']
 Requires-Dist: pymcp2221a
 Requires-Dist: pyqt5
```

### Comparing `ivmdriver-0.0.5/setup.py` & `ivmdriver-0.0.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 AUTHOR_EMAIL = 'harishkumarsedu@gmail.com'
 REPO_NAME = 'matrix'
 # datafiles = [(datadir, list(glob.glob(os.path.join(datadir, '*'))))]
 setup(
     name=f'IvmDriver',
     author=AUTHOR_USER_NAME,
     author_email=AUTHOR_EMAIL,
-    version='0.0.5',
+    version='0.0.6',
     # py_modules=['src'],
     # description=[ 'text/markdown','text/x-rst'],
     url=f"https://github.com/{AUTHOR_USER_NAME}/{REPO_NAME}",
     project_urls={
         "Bug Tracker": f"https://github.com/{AUTHOR_USER_NAME}/{REPO_NAME}/issues",
     },
     long_description_content_type=['text/plain', 'text/x-rst', 'text/markdown'],
```

