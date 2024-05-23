# Comparing `tmp/loadupch-0.0.1-py3-none-any.whl.zip` & `tmp/loadupch-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 17252 bytes, number of entries: 8
+Zip file size: 17255 bytes, number of entries: 8
 -rw-rw-rw-  2.0 fat       38 b- defN 24-May-23 18:29 loadupch/__init__.py
 -rw-rw-rw-  2.0 fat      116 b- defN 24-May-23 18:37 loadupch/__main__.py
--rw-rw-rw-  2.0 fat    13518 b- defN 24-May-23 18:24 loadupch/app.py
--rw-rw-rw-  2.0 fat    35821 b- defN 24-May-23 18:38 loadupch-0.0.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      684 b- defN 24-May-23 18:38 loadupch-0.0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-May-23 18:38 loadupch-0.0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 24-May-23 18:38 loadupch-0.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      614 b- defN 24-May-23 18:38 loadupch-0.0.1.dist-info/RECORD
-8 files, 50892 bytes uncompressed, 16184 bytes compressed:  68.2%
+-rw-rw-rw-  2.0 fat    13522 b- defN 24-May-23 20:23 loadupch/app.py
+-rw-rw-rw-  2.0 fat    35821 b- defN 24-May-23 20:24 loadupch-0.0.2.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      684 b- defN 24-May-23 20:24 loadupch-0.0.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-May-23 20:24 loadupch-0.0.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        9 b- defN 24-May-23 20:24 loadupch-0.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      614 b- defN 24-May-23 20:24 loadupch-0.0.2.dist-info/RECORD
+8 files, 50896 bytes uncompressed, 16187 bytes compressed:  68.2%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: loadupch/__main__.py
 Comment: 
 
 Filename: loadupch/app.py
 Comment: 
 
-Filename: loadupch-0.0.1.dist-info/LICENSE
+Filename: loadupch-0.0.2.dist-info/LICENSE
 Comment: 
 
-Filename: loadupch-0.0.1.dist-info/METADATA
+Filename: loadupch-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: loadupch-0.0.1.dist-info/WHEEL
+Filename: loadupch-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: loadupch-0.0.1.dist-info/top_level.txt
+Filename: loadupch-0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: loadupch-0.0.1.dist-info/RECORD
+Filename: loadupch-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## loadupch/app.py

```diff
@@ -26,15 +26,15 @@
         if dev is None:
             raise Exception('ERROR: No CH55x device found!')
 
         try:
             dev.set_configuration()
         except usb.core.USBError as ex:
             error_msg = 'ERROR: Failed to access USB device.'
-            if str(ex).startswith('[Errno 13]') and platform.system() == 'Linux':
+            if str(ex).startswith('[Errno 13]') and sys.platform.system() == 'Linux':
                 error_msg += ' Configure udev or run as root (sudo).'
             raise Exception(error_msg)
 
         cfg = dev.get_active_configuration()
         intf = cfg[(0, 0)]
 
         self.epout = usb.util.find_descriptor(intf, custom_match=lambda e: usb.util.endpoint_direction(e.bEndpointAddress) == usb.util.ENDPOINT_OUT)
```

## Comparing `loadupch-0.0.1.dist-info/LICENSE` & `loadupch-0.0.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `loadupch-0.0.1.dist-info/METADATA` & `loadupch-0.0.2.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: loadupch
-Version: 0.0.1
-Summary: Uploader tool for flashing firmware onto the CH552 device. v0.0.1
+Version: 0.0.2
+Summary: Uploader tool for flashing firmware onto the CH552 device. v0.0.2
 Author: Master
 Author-email: name@email.com
 License: GPL-3.0 License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: tk
 Requires-Dist: pyusb
@@ -15,15 +15,15 @@
 This tool allows you to flash, erase, and verify the firmware on your development board. To recognize the device, you only need to install the `libusb-win32` driver using Zadig.
 
 - Download Zadig from [Zadig](https://zadig.akeo.ie/)
 
 ### Installation
 
 ```bash
-pip install loaderch
+pip install loadupch
 ```
 
 ### Test
 
 ```bash
-python -m loaderch
+python -m loadupch
 ```
```

## Comparing `loadupch-0.0.1.dist-info/RECORD` & `loadupch-0.0.2.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 loadupch/__init__.py,sha256=nJ6eBM0ejv7XlwD4TFzp8nU_YXDoFIlytXzJ8aje2Xc,38
 loadupch/__main__.py,sha256=YLfvhMoj6mxi7fQlgugKfS14YTeUB2IrH9eOoIhGa64,116
-loadupch/app.py,sha256=prhnlDZ-9USi4hekzWhNnCklcIcHzgHoiY1sDKE-3so,13518
-loadupch-0.0.1.dist-info/LICENSE,sha256=gcuuhKKc5-dwvyvHsXjlC9oM6N5gZ6umYbC8ewW1Yvg,35821
-loadupch-0.0.1.dist-info/METADATA,sha256=nguINYHR6aS3UDZujsy28QAhDsdl7eDylQP16KPiZw4,684
-loadupch-0.0.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-loadupch-0.0.1.dist-info/top_level.txt,sha256=JgdXx5q_dKhQcxdMLqN_Ia_wHX2M6rWcJx6GqXVmNEI,9
-loadupch-0.0.1.dist-info/RECORD,,
+loadupch/app.py,sha256=qitADHv0mQ5DGqQ5jnZkXvClKmv48QePboYZfvKkLbQ,13522
+loadupch-0.0.2.dist-info/LICENSE,sha256=gcuuhKKc5-dwvyvHsXjlC9oM6N5gZ6umYbC8ewW1Yvg,35821
+loadupch-0.0.2.dist-info/METADATA,sha256=wcHDZp2JL8nT6Gq7pPZyCflisiNlyLlCGHRyZEKnioo,684
+loadupch-0.0.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+loadupch-0.0.2.dist-info/top_level.txt,sha256=JgdXx5q_dKhQcxdMLqN_Ia_wHX2M6rWcJx6GqXVmNEI,9
+loadupch-0.0.2.dist-info/RECORD,,
```

