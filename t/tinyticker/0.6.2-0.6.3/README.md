# Comparing `tmp/tinyticker-0.6.2.tar.gz` & `tmp/tinyticker-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinyticker-0.6.2.tar", max compression
+gzip compressed data, was "tinyticker-0.6.3.tar", max compression
```

## Comparing `tinyticker-0.6.2.tar` & `tinyticker-0.6.3.tar`

### file list

```diff
@@ -1,40 +1,41 @@
--rw-r--r--   0        0        0     1068 2024-05-22 15:08:06.073083 tinyticker-0.6.2/LICENSE
--rw-r--r--   0        0        0     3953 2024-05-22 15:08:06.073083 tinyticker-0.6.2/README.md
--rw-r--r--   0        0        0      917 2024-05-22 15:08:06.073083 tinyticker-0.6.2/pyproject.toml
--rw-r--r--   0        0        0      465 2024-05-22 15:08:06.077083 tinyticker-0.6.2/tinyticker/__init__.py
--rw-r--r--   0        0        0     5893 2024-05-22 15:08:06.077083 tinyticker-0.6.2/tinyticker/__main__.py
--rw-r--r--   0        0        0     2496 2024-05-22 15:08:06.077083 tinyticker-0.6.2/tinyticker/config.py
--rw-r--r--   0        0        0     9000 2024-05-22 15:08:06.077083 tinyticker-0.6.2/tinyticker/display.py
--rw-r--r--   0        0        0      345 2024-05-22 15:08:06.077083 tinyticker-0.6.2/tinyticker/paths.py
--rw-r--r--   0        0        0     4235 2024-05-22 15:08:06.081083 tinyticker-0.6.2/tinyticker/sequence.py
--rw-r--r--   0        0        0     1112 2024-05-22 15:08:06.081083 tinyticker-0.6.2/tinyticker/tickers/__init__.py
--rw-r--r--   0        0        0     3618 2024-05-22 15:08:06.081083 tinyticker-0.6.2/tinyticker/tickers/_base.py
--rw-r--r--   0        0        0     4620 2024-05-22 15:08:06.081083 tinyticker-0.6.2/tinyticker/tickers/crypto.py
--rw-r--r--   0        0        0     2915 2024-05-22 15:08:06.081083 tinyticker-0.6.2/tinyticker/tickers/stock.py
--rw-r--r--   0        0        0     2391 2024-05-22 15:08:06.081083 tinyticker-0.6.2/tinyticker/utils.py
--rw-r--r--   0        0        0      278 2024-05-22 15:08:06.081083 tinyticker-0.6.2/tinyticker/waveshare_lib/__init__.py
--rw-r--r--   0        0        0     1297 2024-05-22 15:08:06.081083 tinyticker-0.6.2/tinyticker/waveshare_lib/_base.py
--rw-r--r--   0        0        0     4104 2024-05-22 15:08:06.081083 tinyticker-0.6.2/tinyticker/waveshare_lib/device.py
--rw-r--r--   0        0        0     8593 2024-05-22 15:08:06.081083 tinyticker-0.6.2/tinyticker/waveshare_lib/epd2in13.py
--rw-r--r--   0        0        0    12127 2024-05-22 15:08:06.081083 tinyticker-0.6.2/tinyticker/waveshare_lib/epd2in13_V2.py
--rw-r--r--   0        0        0    14828 2024-05-22 15:08:06.081083 tinyticker-0.6.2/tinyticker/waveshare_lib/epd2in13_V3.py
--rw-r--r--   0        0        0    10709 2024-05-22 15:08:06.081083 tinyticker-0.6.2/tinyticker/waveshare_lib/epd2in13_V4.py
--rw-r--r--   0        0        0     6057 2024-05-22 15:08:06.081083 tinyticker-0.6.2/tinyticker/waveshare_lib/epd2in13b_V3.py
--rw-r--r--   0        0        0     6860 2024-05-22 15:08:06.081083 tinyticker-0.6.2/tinyticker/waveshare_lib/epd2in13b_V4.py
--rw-r--r--   0        0        0     5907 2024-05-22 15:08:06.081083 tinyticker-0.6.2/tinyticker/waveshare_lib/epd2in13bc.py
--rw-r--r--   0        0        0    19697 2024-05-22 15:08:06.081083 tinyticker-0.6.2/tinyticker/waveshare_lib/epd2in7_V2.py
--rw-r--r--   0        0        0     1423 2024-05-22 15:08:06.081083 tinyticker-0.6.2/tinyticker/waveshare_lib/models.py
--rw-r--r--   0        0        0       95 2024-05-22 15:08:06.081083 tinyticker-0.6.2/tinyticker/web/__init__.py
--rw-r--r--   0        0        0     2583 2024-05-22 15:08:06.081083 tinyticker-0.6.2/tinyticker/web/__main__.py
--rw-r--r--   0        0        0     6750 2024-05-22 15:08:06.081083 tinyticker-0.6.2/tinyticker/web/app.py
--rw-r--r--   0        0        0     3021 2024-05-22 15:08:06.081083 tinyticker-0.6.2/tinyticker/web/command.py
--rw-r--r--   0        0        0   274777 2024-05-22 15:08:06.085083 tinyticker-0.6.2/tinyticker/web/templates/css/uikit.min.css
--rw-r--r--   0        0        0    12844 2024-05-22 15:08:06.085083 tinyticker-0.6.2/tinyticker/web/templates/images/apple-touch-icon.png
--rw-r--r--   0        0        0      742 2024-05-22 15:08:06.085083 tinyticker-0.6.2/tinyticker/web/templates/images/favicon-16x16.png
--rw-r--r--   0        0        0     1645 2024-05-22 15:08:06.085083 tinyticker-0.6.2/tinyticker/web/templates/images/favicon-32x32.png
--rw-r--r--   0        0        0    15682 2024-05-22 15:08:06.085083 tinyticker-0.6.2/tinyticker/web/templates/index.html
--rw-r--r--   0        0        0     1904 2024-05-22 15:08:06.085083 tinyticker-0.6.2/tinyticker/web/templates/js/index.js
--rw-r--r--   0        0        0    65291 2024-05-22 15:08:06.085083 tinyticker-0.6.2/tinyticker/web/templates/js/uikit-icons.min.js
--rw-r--r--   0        0        0   136629 2024-05-22 15:08:06.085083 tinyticker-0.6.2/tinyticker/web/templates/js/uikit.min.js
--rw-r--r--   0        0        0     2349 2024-05-22 15:08:06.085083 tinyticker-0.6.2/tinyticker/web/templates/logfiles.html
--rw-r--r--   0        0        0     5242 1970-01-01 00:00:00.000000 tinyticker-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-05-22 21:05:12.232667 tinyticker-0.6.3/LICENSE
+-rw-r--r--   0        0        0     3787 2024-05-22 21:05:12.232667 tinyticker-0.6.3/README.md
+-rw-r--r--   0        0        0      917 2024-05-22 21:05:12.236667 tinyticker-0.6.3/pyproject.toml
+-rw-r--r--   0        0        0      465 2024-05-22 21:05:12.240666 tinyticker-0.6.3/tinyticker/__init__.py
+-rw-r--r--   0        0        0     5893 2024-05-22 21:05:12.240666 tinyticker-0.6.3/tinyticker/__main__.py
+-rw-r--r--   0        0        0     2496 2024-05-22 21:05:12.240666 tinyticker-0.6.3/tinyticker/config.py
+-rw-r--r--   0        0        0     9000 2024-05-22 21:05:12.240666 tinyticker-0.6.3/tinyticker/display.py
+-rw-r--r--   0        0        0      345 2024-05-22 21:05:12.240666 tinyticker-0.6.3/tinyticker/paths.py
+-rw-r--r--   0        0        0     4235 2024-05-22 21:05:12.240666 tinyticker-0.6.3/tinyticker/sequence.py
+-rw-r--r--   0        0        0     1112 2024-05-22 21:05:12.240666 tinyticker-0.6.3/tinyticker/tickers/__init__.py
+-rw-r--r--   0        0        0     3618 2024-05-22 21:05:12.240666 tinyticker-0.6.3/tinyticker/tickers/_base.py
+-rw-r--r--   0        0        0     4620 2024-05-22 21:05:12.240666 tinyticker-0.6.3/tinyticker/tickers/crypto.py
+-rw-r--r--   0        0        0     2915 2024-05-22 21:05:12.240666 tinyticker-0.6.3/tinyticker/tickers/stock.py
+-rw-r--r--   0        0        0     2391 2024-05-22 21:05:12.240666 tinyticker-0.6.3/tinyticker/utils.py
+-rw-r--r--   0        0        0      278 2024-05-22 21:05:12.240666 tinyticker-0.6.3/tinyticker/waveshare_lib/__init__.py
+-rw-r--r--   0        0        0     1297 2024-05-22 21:05:12.240666 tinyticker-0.6.3/tinyticker/waveshare_lib/_base.py
+-rw-r--r--   0        0        0     4104 2024-05-22 21:05:12.240666 tinyticker-0.6.3/tinyticker/waveshare_lib/device.py
+-rw-r--r--   0        0        0     8593 2024-05-22 21:05:12.240666 tinyticker-0.6.3/tinyticker/waveshare_lib/epd2in13.py
+-rw-r--r--   0        0        0    12127 2024-05-22 21:05:12.240666 tinyticker-0.6.3/tinyticker/waveshare_lib/epd2in13_V2.py
+-rw-r--r--   0        0        0    14828 2024-05-22 21:05:12.240666 tinyticker-0.6.3/tinyticker/waveshare_lib/epd2in13_V3.py
+-rw-r--r--   0        0        0    10709 2024-05-22 21:05:12.240666 tinyticker-0.6.3/tinyticker/waveshare_lib/epd2in13_V4.py
+-rw-r--r--   0        0        0     6057 2024-05-22 21:05:12.240666 tinyticker-0.6.3/tinyticker/waveshare_lib/epd2in13b_V3.py
+-rw-r--r--   0        0        0     6860 2024-05-22 21:05:12.240666 tinyticker-0.6.3/tinyticker/waveshare_lib/epd2in13b_V4.py
+-rw-r--r--   0        0        0     5907 2024-05-22 21:05:12.240666 tinyticker-0.6.3/tinyticker/waveshare_lib/epd2in13bc.py
+-rw-r--r--   0        0        0    21091 2024-05-22 21:05:12.240666 tinyticker-0.6.3/tinyticker/waveshare_lib/epd2in7.py
+-rw-r--r--   0        0        0    19697 2024-05-22 21:05:12.240666 tinyticker-0.6.3/tinyticker/waveshare_lib/epd2in7_V2.py
+-rw-r--r--   0        0        0     1551 2024-05-22 21:05:12.240666 tinyticker-0.6.3/tinyticker/waveshare_lib/models.py
+-rw-r--r--   0        0        0       95 2024-05-22 21:05:12.240666 tinyticker-0.6.3/tinyticker/web/__init__.py
+-rw-r--r--   0        0        0     2583 2024-05-22 21:05:12.240666 tinyticker-0.6.3/tinyticker/web/__main__.py
+-rw-r--r--   0        0        0     6750 2024-05-22 21:05:12.244667 tinyticker-0.6.3/tinyticker/web/app.py
+-rw-r--r--   0        0        0     3021 2024-05-22 21:05:12.244667 tinyticker-0.6.3/tinyticker/web/command.py
+-rw-r--r--   0        0        0   274777 2024-05-22 21:05:12.244667 tinyticker-0.6.3/tinyticker/web/templates/css/uikit.min.css
+-rw-r--r--   0        0        0    12844 2024-05-22 21:05:12.244667 tinyticker-0.6.3/tinyticker/web/templates/images/apple-touch-icon.png
+-rw-r--r--   0        0        0      742 2024-05-22 21:05:12.244667 tinyticker-0.6.3/tinyticker/web/templates/images/favicon-16x16.png
+-rw-r--r--   0        0        0     1645 2024-05-22 21:05:12.244667 tinyticker-0.6.3/tinyticker/web/templates/images/favicon-32x32.png
+-rw-r--r--   0        0        0    15682 2024-05-22 21:05:12.244667 tinyticker-0.6.3/tinyticker/web/templates/index.html
+-rw-r--r--   0        0        0     1904 2024-05-22 21:05:12.244667 tinyticker-0.6.3/tinyticker/web/templates/js/index.js
+-rw-r--r--   0        0        0    65291 2024-05-22 21:05:12.244667 tinyticker-0.6.3/tinyticker/web/templates/js/uikit-icons.min.js
+-rw-r--r--   0        0        0   136629 2024-05-22 21:05:12.244667 tinyticker-0.6.3/tinyticker/web/templates/js/uikit.min.js
+-rw-r--r--   0        0        0     2349 2024-05-22 21:05:12.244667 tinyticker-0.6.3/tinyticker/web/templates/logfiles.html
+-rw-r--r--   0        0        0     5076 1970-01-01 00:00:00.000000 tinyticker-0.6.3/PKG-INFO
```

### Comparing `tinyticker-0.6.2/LICENSE` & `tinyticker-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.2/README.md` & `tinyticker-0.6.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -78,25 +78,21 @@
   - Install `tinyticker`:
 
   ```sh
   pip install tinyticker
   ```
 
   - To setup `tinyticker` to start on boot, copy over the [`systemd` unit files](./systemd) and enable them.
-  - On boot, a qrcode linking to the `flask` app will be flashed on the display
-  - Leave a star, reboot and HODL !
 
 </details>
 
 ## 👢 First boot
 
 On first boot, you will need to connect your RPi to your wifi network.
 
 - Connect to the `tinyticker` wifi AP
 - Select the wifi network you want your RPi to connect to
 - Enter the wifi password
 
 Your RPi will now connect to your wifi and the `tinyticker` services will start.
 
 Once the web app is running, head over to `http://tinyticker.local` to configure it.
-
-> The RPi zero isn't very fast, so be patient :)
```

#### html2text {}

```diff
@@ -36,15 +36,13 @@
 Install the `BCM2835` driver: ```sh curl http://www.airspayce.com/mikem/
 bcm2835/bcm2835-1.60.tar.gz | tar xzv cd bcm2835-1.60/ ./configure make make
 install ``` - Install `pip`: ```sh sudo apt install python3-pip ``` - Install
 dependency requirements: ```sh sudo apt install libxml2-dev libxslt1-dev
 libatlas-base-dev ninja-build patchelf libopenjp2-7 libtiff-dev libjpeg-dev ```
 - Install `tinyticker`: ```sh pip install tinyticker ``` - To setup
 `tinyticker` to start on boot, copy over the [`systemd` unit files](./systemd)
-and enable them. - On boot, a qrcode linking to the `flask` app will be flashed
-on the display - Leave a star, reboot and HODL ! ## ð¢ First boot On first
-boot, you will need to connect your RPi to your wifi network. - Connect to the
-`tinyticker` wifi AP - Select the wifi network you want your RPi to connect to
-- Enter the wifi password Your RPi will now connect to your wifi and the
-`tinyticker` services will start. Once the web app is running, head over to
-`http://tinyticker.local` to configure it. > The RPi zero isn't very fast, so
-be patient :)
+and enable them. ## ð¢ First boot On first boot, you will need to connect
+your RPi to your wifi network. - Connect to the `tinyticker` wifi AP - Select
+the wifi network you want your RPi to connect to - Enter the wifi password Your
+RPi will now connect to your wifi and the `tinyticker` services will start.
+Once the web app is running, head over to `http://tinyticker.local` to
+configure it.
```

### Comparing `tinyticker-0.6.2/pyproject.toml` & `tinyticker-0.6.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tinyticker"
-version = "0.6.2"
+version = "0.6.3"
 description = "A tiny Raspberry Pi powered ePaper ticker."
 authors = ["Loic Coyle <loic.coyle@hotmail.fr>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/loiccoyle/tinyticker"
 keywords = ["raspberry-pi", "ticker", "stock", "crypto", "epaper", "finance"]
```

### Comparing `tinyticker-0.6.2/tinyticker/__main__.py` & `tinyticker-0.6.3/tinyticker/__main__.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.2/tinyticker/config.py` & `tinyticker-0.6.3/tinyticker/config.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.2/tinyticker/display.py` & `tinyticker-0.6.3/tinyticker/display.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.2/tinyticker/sequence.py` & `tinyticker-0.6.3/tinyticker/sequence.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.2/tinyticker/tickers/__init__.py` & `tinyticker-0.6.3/tinyticker/tickers/__init__.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.2/tinyticker/tickers/_base.py` & `tinyticker-0.6.3/tinyticker/tickers/_base.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.2/tinyticker/tickers/crypto.py` & `tinyticker-0.6.3/tinyticker/tickers/crypto.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.2/tinyticker/tickers/stock.py` & `tinyticker-0.6.3/tinyticker/tickers/stock.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.2/tinyticker/utils.py` & `tinyticker-0.6.3/tinyticker/utils.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.2/tinyticker/waveshare_lib/_base.py` & `tinyticker-0.6.3/tinyticker/waveshare_lib/_base.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.2/tinyticker/waveshare_lib/device.py` & `tinyticker-0.6.3/tinyticker/waveshare_lib/device.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.2/tinyticker/waveshare_lib/epd2in13.py` & `tinyticker-0.6.3/tinyticker/waveshare_lib/epd2in13.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.2/tinyticker/waveshare_lib/epd2in13_V2.py` & `tinyticker-0.6.3/tinyticker/waveshare_lib/epd2in13_V2.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.2/tinyticker/waveshare_lib/epd2in13_V3.py` & `tinyticker-0.6.3/tinyticker/waveshare_lib/epd2in13_V3.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.2/tinyticker/waveshare_lib/epd2in13_V4.py` & `tinyticker-0.6.3/tinyticker/waveshare_lib/epd2in13_V4.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.2/tinyticker/waveshare_lib/epd2in13b_V3.py` & `tinyticker-0.6.3/tinyticker/waveshare_lib/epd2in13b_V3.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.2/tinyticker/waveshare_lib/epd2in13b_V4.py` & `tinyticker-0.6.3/tinyticker/waveshare_lib/epd2in13b_V4.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.2/tinyticker/waveshare_lib/epd2in13bc.py` & `tinyticker-0.6.3/tinyticker/waveshare_lib/epd2in13bc.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.2/tinyticker/waveshare_lib/epd2in7_V2.py` & `tinyticker-0.6.3/tinyticker/waveshare_lib/epd2in7_V2.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.2/tinyticker/waveshare_lib/models.py` & `tinyticker-0.6.3/tinyticker/waveshare_lib/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
     epd2in13,
     epd2in13_V2,
     epd2in13_V3,
     epd2in13_V4,
     epd2in13b_V3,
     epd2in13b_V4,
     epd2in13bc,
+    epd2in7,
     epd2in7_V2,
 )
 from ._base import EPDHighlight, EPDMonochrome
 
 
 @dataclass
 class EPDModel:
@@ -54,13 +55,18 @@
     ),
     EPDModel(
         name="EPDbc",
         class_=epd2in13bc.EPD,
         desc="Black, White and Yellow 2.13 inch",
     ),
     EPDModel(
+        name="EPD_2in7",
+        class_=epd2in7.EPD,
+        desc="Black and White 2.7 inch",
+    ),
+    EPDModel(
         name="EPD_2in7_v2",
         class_=epd2in7_V2.EPD,
         desc="Black and White 2.7 inch V2",
     ),
 ]
 MODELS = {model.name: model for model in MODELS}
```

### Comparing `tinyticker-0.6.2/tinyticker/web/__main__.py` & `tinyticker-0.6.3/tinyticker/web/__main__.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.2/tinyticker/web/app.py` & `tinyticker-0.6.3/tinyticker/web/app.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.2/tinyticker/web/command.py` & `tinyticker-0.6.3/tinyticker/web/command.py`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.2/tinyticker/web/templates/css/uikit.min.css` & `tinyticker-0.6.3/tinyticker/web/templates/css/uikit.min.css`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.2/tinyticker/web/templates/images/apple-touch-icon.png` & `tinyticker-0.6.3/tinyticker/web/templates/images/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.2/tinyticker/web/templates/images/favicon-16x16.png` & `tinyticker-0.6.3/tinyticker/web/templates/images/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.2/tinyticker/web/templates/images/favicon-32x32.png` & `tinyticker-0.6.3/tinyticker/web/templates/images/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.2/tinyticker/web/templates/index.html` & `tinyticker-0.6.3/tinyticker/web/templates/index.html`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.2/tinyticker/web/templates/js/index.js` & `tinyticker-0.6.3/tinyticker/web/templates/js/index.js`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.2/tinyticker/web/templates/js/uikit-icons.min.js` & `tinyticker-0.6.3/tinyticker/web/templates/js/uikit-icons.min.js`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.2/tinyticker/web/templates/js/uikit.min.js` & `tinyticker-0.6.3/tinyticker/web/templates/js/uikit.min.js`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.2/tinyticker/web/templates/logfiles.html` & `tinyticker-0.6.3/tinyticker/web/templates/logfiles.html`

 * *Files identical despite different names*

### Comparing `tinyticker-0.6.2/PKG-INFO` & `tinyticker-0.6.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tinyticker
-Version: 0.6.2
+Version: 0.6.3
 Summary: A tiny Raspberry Pi powered ePaper ticker.
 Home-page: https://github.com/loiccoyle/tinyticker
 License: MIT
 Keywords: raspberry-pi,ticker,stock,crypto,epaper,finance
 Author: Loic Coyle
 Author-email: loic.coyle@hotmail.fr
 Requires-Python: >=3.9
@@ -111,16 +111,14 @@
   - Install `tinyticker`:
 
   ```sh
   pip install tinyticker
   ```
 
   - To setup `tinyticker` to start on boot, copy over the [`systemd` unit files](./systemd) and enable them.
-  - On boot, a qrcode linking to the `flask` app will be flashed on the display
-  - Leave a star, reboot and HODL !
 
 </details>
 
 ## 👢 First boot
 
 On first boot, you will need to connect your RPi to your wifi network.
 
@@ -128,9 +126,7 @@
 - Select the wifi network you want your RPi to connect to
 - Enter the wifi password
 
 Your RPi will now connect to your wifi and the `tinyticker` services will start.
 
 Once the web app is running, head over to `http://tinyticker.local` to configure it.
 
-> The RPi zero isn't very fast, so be patient :)
-
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tinyticker Version: 0.6.2 Summary: A tiny Raspberry
+Metadata-Version: 2.1 Name: tinyticker Version: 0.6.3 Summary: A tiny Raspberry
 Pi powered ePaper ticker. Home-page: https://github.com/loiccoyle/tinyticker
 License: MIT Keywords: raspberry-pi,ticker,stock,crypto,epaper,finance Author:
 Loic Coyle Author-email: loic.coyle@hotmail.fr Requires-Python: >=3.9
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
@@ -54,15 +54,13 @@
 Install the `BCM2835` driver: ```sh curl http://www.airspayce.com/mikem/
 bcm2835/bcm2835-1.60.tar.gz | tar xzv cd bcm2835-1.60/ ./configure make make
 install ``` - Install `pip`: ```sh sudo apt install python3-pip ``` - Install
 dependency requirements: ```sh sudo apt install libxml2-dev libxslt1-dev
 libatlas-base-dev ninja-build patchelf libopenjp2-7 libtiff-dev libjpeg-dev ```
 - Install `tinyticker`: ```sh pip install tinyticker ``` - To setup
 `tinyticker` to start on boot, copy over the [`systemd` unit files](./systemd)
-and enable them. - On boot, a qrcode linking to the `flask` app will be flashed
-on the display - Leave a star, reboot and HODL ! ## ð¢ First boot On first
-boot, you will need to connect your RPi to your wifi network. - Connect to the
-`tinyticker` wifi AP - Select the wifi network you want your RPi to connect to
-- Enter the wifi password Your RPi will now connect to your wifi and the
-`tinyticker` services will start. Once the web app is running, head over to
-`http://tinyticker.local` to configure it. > The RPi zero isn't very fast, so
-be patient :)
+and enable them. ## ð¢ First boot On first boot, you will need to connect
+your RPi to your wifi network. - Connect to the `tinyticker` wifi AP - Select
+the wifi network you want your RPi to connect to - Enter the wifi password Your
+RPi will now connect to your wifi and the `tinyticker` services will start.
+Once the web app is running, head over to `http://tinyticker.local` to
+configure it.
```

