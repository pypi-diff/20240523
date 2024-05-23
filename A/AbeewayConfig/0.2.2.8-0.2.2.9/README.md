# Comparing `tmp/abeewayconfig-0.2.2.8.tar.gz` & `tmp/abeewayconfig-0.2.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abeewayconfig-0.2.2.8.tar", last modified: Thu May 23 03:01:29 2024, max compression
+gzip compressed data, was "abeewayconfig-0.2.2.9.tar", last modified: Thu May 23 16:33:55 2024, max compression
```

## Comparing `abeewayconfig-0.2.2.8.tar` & `abeewayconfig-0.2.2.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 lucas     (1000) lucas     (1000)        0 2024-05-23 03:01:29.180239 abeewayconfig-0.2.2.8/
--rw-r--r--   0 lucas     (1000) lucas     (1000)    35149 2024-05-19 01:48:12.000000 abeewayconfig-0.2.2.8/LICENSE
--rw-r--r--   0 lucas     (1000) lucas     (1000)     1695 2024-05-23 03:01:29.180239 abeewayconfig-0.2.2.8/PKG-INFO
--rw-r--r--   0 lucas     (1000) lucas     (1000)     1307 2024-05-23 03:01:08.000000 abeewayconfig-0.2.2.8/README.md
--rw-r--r--   0 lucas     (1000) lucas     (1000)       38 2024-05-23 03:01:29.180239 abeewayconfig-0.2.2.8/setup.cfg
--rw-r--r--   0 lucas     (1000) lucas     (1000)      851 2024-05-23 02:53:17.000000 abeewayconfig-0.2.2.8/setup.py
-drwxr-xr-x   0 lucas     (1000) lucas     (1000)        0 2024-05-23 03:01:29.176905 abeewayconfig-0.2.2.8/src/
-drwxr-xr-x   0 lucas     (1000) lucas     (1000)        0 2024-05-23 03:01:29.176905 abeewayconfig-0.2.2.8/src/AbeewayConfig/
--rw-r--r--   0 lucas     (1000) lucas     (1000)     4758 2024-05-23 02:51:28.000000 abeewayconfig-0.2.2.8/src/AbeewayConfig/CSVFile.py
--rw-r--r--   0 lucas     (1000) lucas     (1000)     3430 2024-05-23 00:22:55.000000 abeewayconfig-0.2.2.8/src/AbeewayConfig/Config.py
--rw-r--r--   0 lucas     (1000) lucas     (1000)     2807 2024-05-23 00:22:55.000000 abeewayconfig-0.2.2.8/src/AbeewayConfig/Device.py
--rw-r--r--   0 lucas     (1000) lucas     (1000)       32 2024-05-19 01:48:12.000000 abeewayconfig-0.2.2.8/src/AbeewayConfig/__init__.py
--rw-r--r--   0 lucas     (1000) lucas     (1000)     6138 2024-05-23 02:27:42.000000 abeewayconfig-0.2.2.8/src/AbeewayConfig/abeewayconfig.py
--rw-r--r--   0 lucas     (1000) lucas     (1000)     4026 2024-05-19 01:48:12.000000 abeewayconfig-0.2.2.8/src/AbeewayConfig/smartbadgecfgdict.py
-drwxr-xr-x   0 lucas     (1000) lucas     (1000)        0 2024-05-23 03:01:29.180239 abeewayconfig-0.2.2.8/src/AbeewayConfig.egg-info/
--rw-r--r--   0 lucas     (1000) lucas     (1000)     1695 2024-05-23 03:01:29.000000 abeewayconfig-0.2.2.8/src/AbeewayConfig.egg-info/PKG-INFO
--rw-r--r--   0 lucas     (1000) lucas     (1000)      463 2024-05-23 03:01:29.000000 abeewayconfig-0.2.2.8/src/AbeewayConfig.egg-info/SOURCES.txt
--rw-r--r--   0 lucas     (1000) lucas     (1000)        1 2024-05-23 03:01:29.000000 abeewayconfig-0.2.2.8/src/AbeewayConfig.egg-info/dependency_links.txt
--rw-r--r--   0 lucas     (1000) lucas     (1000)      121 2024-05-23 03:01:29.000000 abeewayconfig-0.2.2.8/src/AbeewayConfig.egg-info/entry_points.txt
--rw-r--r--   0 lucas     (1000) lucas     (1000)       12 2024-05-23 03:01:29.000000 abeewayconfig-0.2.2.8/src/AbeewayConfig.egg-info/requires.txt
--rw-r--r--   0 lucas     (1000) lucas     (1000)       14 2024-05-23 03:01:29.000000 abeewayconfig-0.2.2.8/src/AbeewayConfig.egg-info/top_level.txt
+drwxr-xr-x   0 lucas     (1001) lucas     (1001)        0 2024-05-23 16:33:55.008016 abeewayconfig-0.2.2.9/
+-rw-r--r--   0 lucas     (1001) lucas     (1001)    35149 2024-05-15 17:30:13.000000 abeewayconfig-0.2.2.9/LICENSE
+-rw-r--r--   0 lucas     (1001) lucas     (1001)     1695 2024-05-23 16:33:55.008016 abeewayconfig-0.2.2.9/PKG-INFO
+-rw-r--r--   0 lucas     (1001) lucas     (1001)     1307 2024-05-23 15:33:30.000000 abeewayconfig-0.2.2.9/README.md
+-rw-r--r--   0 lucas     (1001) lucas     (1001)       38 2024-05-23 16:33:55.008016 abeewayconfig-0.2.2.9/setup.cfg
+-rw-r--r--   0 lucas     (1001) lucas     (1001)      851 2024-05-23 16:29:40.000000 abeewayconfig-0.2.2.9/setup.py
+drwxr-xr-x   0 lucas     (1001) lucas     (1001)        0 2024-05-23 16:33:55.004683 abeewayconfig-0.2.2.9/src/
+drwxr-xr-x   0 lucas     (1001) lucas     (1001)        0 2024-05-23 16:33:55.008016 abeewayconfig-0.2.2.9/src/AbeewayConfig/
+-rw-r--r--   0 lucas     (1001) lucas     (1001)     4700 2024-05-23 16:09:37.000000 abeewayconfig-0.2.2.9/src/AbeewayConfig/CSVFile.py
+-rw-r--r--   0 lucas     (1001) lucas     (1001)     3430 2024-05-22 20:24:17.000000 abeewayconfig-0.2.2.9/src/AbeewayConfig/Config.py
+-rw-r--r--   0 lucas     (1001) lucas     (1001)     2906 2024-05-23 16:27:23.000000 abeewayconfig-0.2.2.9/src/AbeewayConfig/Device.py
+-rw-r--r--   0 lucas     (1001) lucas     (1001)       32 2024-05-16 13:41:49.000000 abeewayconfig-0.2.2.9/src/AbeewayConfig/__init__.py
+-rw-r--r--   0 lucas     (1001) lucas     (1001)     6138 2024-05-23 15:33:47.000000 abeewayconfig-0.2.2.9/src/AbeewayConfig/abeewayconfig.py
+-rw-r--r--   0 lucas     (1001) lucas     (1001)     4026 2024-05-14 13:11:26.000000 abeewayconfig-0.2.2.9/src/AbeewayConfig/smartbadgecfgdict.py
+drwxr-xr-x   0 lucas     (1001) lucas     (1001)        0 2024-05-23 16:33:55.008016 abeewayconfig-0.2.2.9/src/AbeewayConfig.egg-info/
+-rw-r--r--   0 lucas     (1001) lucas     (1001)     1695 2024-05-23 16:33:54.000000 abeewayconfig-0.2.2.9/src/AbeewayConfig.egg-info/PKG-INFO
+-rw-r--r--   0 lucas     (1001) lucas     (1001)      463 2024-05-23 16:33:55.000000 abeewayconfig-0.2.2.9/src/AbeewayConfig.egg-info/SOURCES.txt
+-rw-r--r--   0 lucas     (1001) lucas     (1001)        1 2024-05-23 16:33:54.000000 abeewayconfig-0.2.2.9/src/AbeewayConfig.egg-info/dependency_links.txt
+-rw-r--r--   0 lucas     (1001) lucas     (1001)      121 2024-05-23 16:33:55.000000 abeewayconfig-0.2.2.9/src/AbeewayConfig.egg-info/entry_points.txt
+-rw-r--r--   0 lucas     (1001) lucas     (1001)       12 2024-05-23 16:33:55.000000 abeewayconfig-0.2.2.9/src/AbeewayConfig.egg-info/requires.txt
+-rw-r--r--   0 lucas     (1001) lucas     (1001)       14 2024-05-23 16:33:55.000000 abeewayconfig-0.2.2.9/src/AbeewayConfig.egg-info/top_level.txt
```

### Comparing `abeewayconfig-0.2.2.8/LICENSE` & `abeewayconfig-0.2.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `abeewayconfig-0.2.2.8/PKG-INFO` & `abeewayconfig-0.2.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AbeewayConfig
-Version: 0.2.2.8
+Version: 0.2.2.9
 Summary: Abeeway configuration tool
 Home-page: https://github.com/jlabbude/AbeewayConfig
 Author: João Lucas
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.0
 Description-Content-Type: text/markdown
```

### Comparing `abeewayconfig-0.2.2.8/README.md` & `abeewayconfig-0.2.2.9/README.md`

 * *Files identical despite different names*

### Comparing `abeewayconfig-0.2.2.8/setup.py` & `abeewayconfig-0.2.2.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     description = f.read()
 
 setup(
     name="AbeewayConfig",
-    version="0.2.2.8",
+    version="0.2.2.9",
     description="Abeeway configuration tool",
     author="João Lucas",
     url="https://github.com/jlabbude/AbeewayConfig",
     packages=find_packages(where="src"),
     package_dir={"": "src"},
     install_requires=[
         "pyserial",
```

### Comparing `abeewayconfig-0.2.2.8/src/AbeewayConfig/CSVFile.py` & `abeewayconfig-0.2.2.9/src/AbeewayConfig/CSVFile.py`

 * *Files 5% similar despite different names*

```diff
@@ -51,20 +51,19 @@
 
     def write_to_csv(data: list[str]) -> None:
         global csv_file
         csv_file = os.path.join(os.path.dirname(__file__), "utils", "output.csv")
 
         pattern = re.compile(data[0][1], re.IGNORECASE)
 
-        with open(csv_file, mode='r', newline='') as file:
+        with open(csv_file, mode='a+', newline='') as file:
             lines = file.readlines()
             for line in lines:
                 if pattern.search(line.strip()):
                     return
-        with open(csv_file, mode='a', newline='') as file:
             writer = csv.writer(file)
             writer.writerows(data)
 
     @staticmethod
     def grab_dev_info(deveui: str, console_output: Text) -> DevStruct:
         devstruct = DevStruct()
```

### Comparing `abeewayconfig-0.2.2.8/src/AbeewayConfig/Config.py` & `abeewayconfig-0.2.2.9/src/AbeewayConfig/Config.py`

 * *Files identical despite different names*

### Comparing `abeewayconfig-0.2.2.8/src/AbeewayConfig/Device.py` & `abeewayconfig-0.2.2.9/src/AbeewayConfig/Device.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,22 +24,24 @@
         with Serial(serial_port, br, timeout=1) as ser:
             ser.write(b'123\r')
             ser.write(b'123\r')
             ser.write(b'lora info\r')
             output = ser.read(1000).decode('utf-8')
             p = re.compile(r"DevEUI: (.*)")
             deveui = p.search(output)
-            # TODO: make creator for deveui.txt
             if deveui is not None:
                 deveui_file = os.path.join(os.path.dirname(os.path.abspath(__file__)), "utils", "deveui.txt")
                 deveui = deveui.group(1).strip()
-                with open(deveui_file, 'r') as deveui_log:
-                    deveui_log_content = deveui_log.read().splitlines()
-                if deveui not in deveui_log_content:
-                    with open(deveui_file, 'a') as deveui_log:
+                if os.path.isfile(deveui_file):
+                    with open(deveui_file, 'r+') as deveui_log:
+                        deveui_log_content = deveui_log.read().splitlines()
+                        if deveui not in deveui_log_content:
+                            deveui_log.write(deveui + "\n")
+                else:
+                    with open(deveui_file, 'w') as deveui_log:
                         deveui_log.write(deveui + "\n")
                 return deveui
 
     def set_config_on_device(serial_port: str, br: int) -> None:
         with Serial(serial_port, br, timeout=1) as ser:
             ser.write(b'123\r')
             config_file = os.path.join(os.path.join(os.path.dirname(os.path.abspath(__file__)), "utils"), "config.cfg")
```

### Comparing `abeewayconfig-0.2.2.8/src/AbeewayConfig/abeewayconfig.py` & `abeewayconfig-0.2.2.9/src/AbeewayConfig/abeewayconfig.py`

 * *Files identical despite different names*

### Comparing `abeewayconfig-0.2.2.8/src/AbeewayConfig/smartbadgecfgdict.py` & `abeewayconfig-0.2.2.9/src/AbeewayConfig/smartbadgecfgdict.py`

 * *Files identical despite different names*

### Comparing `abeewayconfig-0.2.2.8/src/AbeewayConfig.egg-info/PKG-INFO` & `abeewayconfig-0.2.2.9/src/AbeewayConfig.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AbeewayConfig
-Version: 0.2.2.8
+Version: 0.2.2.9
 Summary: Abeeway configuration tool
 Home-page: https://github.com/jlabbude/AbeewayConfig
 Author: João Lucas
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.0
 Description-Content-Type: text/markdown
```

