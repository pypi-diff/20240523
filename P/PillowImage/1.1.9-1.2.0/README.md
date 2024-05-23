# Comparing `tmp/PillowImage-1.1.9.tar.gz` & `tmp/PillowImage-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/PillowImage-1.1.9.tar", last modified: Tue Jan 19 19:42:04 2021, max compression
+gzip compressed data, was "PillowImage-1.2.0.tar", last modified: Thu May 23 19:04:54 2024, max compression
```

## Comparing `PillowImage-1.1.9.tar` & `PillowImage-1.2.0.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 Stephen    (501) staff       (20)        0 2021-01-19 19:42:04.000000 PillowImage-1.1.9/
--rw-r--r--   0 Stephen    (501) staff       (20)       26 2019-04-03 16:50:30.000000 PillowImage-1.1.9/MANIFEST.in
--rw-r--r--   0 Stephen    (501) staff       (20)      337 2021-01-19 19:42:04.000000 PillowImage-1.1.9/PKG-INFO
-drwxr-xr-x   0 Stephen    (501) staff       (20)        0 2021-01-19 19:42:04.000000 PillowImage-1.1.9/PillowImage/
--rw-r--r--   0 Stephen    (501) staff       (20)       97 2019-04-03 19:36:27.000000 PillowImage-1.1.9/PillowImage/__init__.py
--rw-r--r--   0 Stephen    (501) staff       (20)       22 2021-01-19 19:41:28.000000 PillowImage-1.1.9/PillowImage/_version.py
-drwxr-xr-x   0 Stephen    (501) staff       (20)        0 2021-01-19 19:42:04.000000 PillowImage-1.1.9/PillowImage/font/
--rw-r--r--   0 Stephen    (501) staff       (20)    65932 2018-08-24 17:38:09.000000 PillowImage-1.1.9/PillowImage/font/Vera.ttf
--rw-r--r--   0 Stephen    (501) staff       (20)       64 2019-04-03 19:36:33.000000 PillowImage-1.1.9/PillowImage/font/__init__.py
--rw-r--r--   0 Stephen    (501) staff       (20)      523 2019-04-03 16:45:36.000000 PillowImage-1.1.9/PillowImage/font/register.py
--rw-r--r--   0 Stephen    (501) staff       (20)     9992 2020-09-15 15:11:17.000000 PillowImage-1.1.9/PillowImage/pillow.py
--rw-r--r--   0 Stephen    (501) staff       (20)     1776 2019-06-14 19:57:07.000000 PillowImage-1.1.9/PillowImage/utils.py
-drwxr-xr-x   0 Stephen    (501) staff       (20)        0 2021-01-19 19:42:04.000000 PillowImage-1.1.9/PillowImage.egg-info/
--rw-r--r--   0 Stephen    (501) staff       (20)      337 2021-01-19 19:42:04.000000 PillowImage-1.1.9/PillowImage.egg-info/PKG-INFO
--rw-r--r--   0 Stephen    (501) staff       (20)      490 2021-01-19 19:42:04.000000 PillowImage-1.1.9/PillowImage.egg-info/SOURCES.txt
--rw-r--r--   0 Stephen    (501) staff       (20)        1 2021-01-19 19:42:04.000000 PillowImage-1.1.9/PillowImage.egg-info/dependency_links.txt
--rw-r--r--   0 Stephen    (501) staff       (20)       46 2021-01-19 19:42:04.000000 PillowImage-1.1.9/PillowImage.egg-info/requires.txt
--rw-r--r--   0 Stephen    (501) staff       (20)       18 2021-01-19 19:42:04.000000 PillowImage-1.1.9/PillowImage.egg-info/top_level.txt
--rw-r--r--   0 Stephen    (501) staff       (20)     2721 2021-01-19 19:34:01.000000 PillowImage-1.1.9/README.md
--rw-r--r--   0 Stephen    (501) staff       (20)       38 2021-01-19 19:42:04.000000 PillowImage-1.1.9/setup.cfg
--rw-r--r--   0 Stephen    (501) staff       (20)     1123 2021-01-19 19:40:57.000000 PillowImage-1.1.9/setup.py
-drwxr-xr-x   0 Stephen    (501) staff       (20)        0 2021-01-19 19:42:04.000000 PillowImage-1.1.9/tests/
--rw-r--r--   0 Stephen    (501) staff       (20)     1157 2019-08-12 14:33:59.000000 PillowImage-1.1.9/tests/__init__.py
--rw-r--r--   0 Stephen    (501) staff       (20)     6134 2019-08-12 14:38:53.000000 PillowImage-1.1.9/tests/test_PillowImage_jpeg.py
--rw-r--r--   0 Stephen    (501) staff       (20)     6132 2019-08-12 14:40:58.000000 PillowImage-1.1.9/tests/test_PillowImage_png.py
--rw-r--r--   0 Stephen    (501) staff       (20)      726 2019-06-14 18:16:07.000000 PillowImage-1.1.9/tests/test_PillowImage_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:04:54.251288 PillowImage-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-23 19:04:46.000000 PillowImage-1.2.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-23 19:04:46.000000 PillowImage-1.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-23 19:04:54.251288 PillowImage-1.2.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:04:54.251288 PillowImage-1.2.0/PillowImage/
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-23 19:04:46.000000 PillowImage-1.2.0/PillowImage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-23 19:04:46.000000 PillowImage-1.2.0/PillowImage/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:04:54.251288 PillowImage-1.2.0/PillowImage/font/
+-rw-r--r--   0 runner    (1001) docker     (127)    65932 2024-05-23 19:04:46.000000 PillowImage-1.2.0/PillowImage/font/Vera.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-23 19:04:46.000000 PillowImage-1.2.0/PillowImage/font/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-23 19:04:46.000000 PillowImage-1.2.0/PillowImage/font/register.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10125 2024-05-23 19:04:46.000000 PillowImage-1.2.0/PillowImage/pillow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-05-23 19:04:46.000000 PillowImage-1.2.0/PillowImage/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:04:54.251288 PillowImage-1.2.0/PillowImage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-23 19:04:54.000000 PillowImage-1.2.0/PillowImage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-23 19:04:54.000000 PillowImage-1.2.0/PillowImage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 19:04:54.000000 PillowImage-1.2.0/PillowImage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-23 19:04:54.000000 PillowImage-1.2.0/PillowImage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-23 19:04:54.000000 PillowImage-1.2.0/PillowImage.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3038 2024-05-23 19:04:46.000000 PillowImage-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 19:04:54.251288 PillowImage-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-05-23 19:04:46.000000 PillowImage-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 19:04:54.251288 PillowImage-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-23 19:04:46.000000 PillowImage-1.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6283 2024-05-23 19:04:46.000000 PillowImage-1.2.0/tests/test_PillowImage_jpeg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6128 2024-05-23 19:04:46.000000 PillowImage-1.2.0/tests/test_PillowImage_png.py
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-05-23 19:04:46.000000 PillowImage-1.2.0/tests/test_PillowImage_utils.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `PillowImage-1.1.9/PillowImage/font/Vera.ttf` & `PillowImage-1.2.0/PillowImage/font/Vera.ttf`

 * *Files identical despite different names*

### Comparing `PillowImage-1.1.9/PillowImage/font/register.py` & `PillowImage-1.2.0/PillowImage/font/register.py`

 * *Files identical despite different names*

### Comparing `PillowImage-1.1.9/PillowImage/pillow.py` & `PillowImage-1.2.0/PillowImage/pillow.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,15 +24,15 @@
             self.img = Image.open(img)
             if self.img.mode != 'RGBA':
                 self.img = self.img.convert('RGBA')
             else:
                 self.img = self.img.copy()
         else:
             # Create a black image
-            self.img = Image.new(mode, size, color=color)  # 2200, 1700 for 200 DPI
+            self.img = Image.new(mode, size, color=color)    # 2200, 1700 for 200 DPI
         self._tempdir = None
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.cleanup()
@@ -79,15 +79,15 @@
 
         :param text: String to be centered
         :param drawing: PIL.ImageDraw.Draw instance
         :param font_type: Registered font family type
         :return: X coordinate value
         """
         # ('Page Width' - 'Text Width') / 2
-        return (self.width - drawing.textsize(text, font=font_type)[0]) / 2
+        return (self.width - drawing.textlength(text, font=font_type)) / 2
 
     def _text_centered_y(self, font_size):
         """
         Retrieve a 'y' value that centers the image in the canvas.
 
         :param font_size: Font size
         :return: Y coordinate value
@@ -112,15 +112,14 @@
 
 
         :param image: Image to-be pasted
         :param x:
         :param y:
         :return: X and Y values
         """
-
         def calculator(value, img_size, center_func):
             """Helper function to perform bound calculations for either x or y values."""
             # Center the image
             if 'center' in str(value).lower():
                 return center_func(image)
 
             # Percentage value, calculate based on percentages
@@ -129,16 +128,16 @@
 
             # Negative value, calculate distance from far edge (Right, Bottom
             elif int(value) < 0:
                 return int(img_size - abs(value))
             else:
                 return int(value)
 
-        return (abs(calculator(x, self.width, self._img_centered_x)),
-                abs(calculator(y, self.height, self._img_centered_y)))
+        return (abs(calculator(x, self.width,
+                               self._img_centered_x)), abs(calculator(y, self.height, self._img_centered_y)))
 
     def scale_to_fit(self, img, func='min', scale=None, multiplier=float(1)):
         """
         Scale an image to fit the Pillow canvas.
 
         :param img: Image object
         :param func: Scale calculation function
@@ -166,22 +165,22 @@
         """Resize by specifying the longest side length."""
         return self.resize_width(longest_side) if self.width > self.height else self.resize_height(longest_side)
 
     def resize_width(self, max_width):
         """Adjust an images width while proportionately scaling height."""
         width_percent = (max_width / float(self.width))
         height_size = int((float(self.height)) * float(width_percent))
-        self.img = self.img.resize((max_width, height_size), Image.ANTIALIAS)
+        self.img = self.img.resize((max_width, height_size), Image.LANCZOS)
         return self.img
 
     def resize_height(self, max_height):
         """Adjust an images height while proportionately scaling width."""
         height_percent = (max_height / float(self.height))
         width_size = int((float(self.width) * float(height_percent)))
-        self.img = self.img.resize((width_size, max_height), Image.ANTIALIAS)
+        self.img = self.img.resize((width_size, max_height), Image.LANCZOS)
         return self.img
 
     def draw_text(self, text, x='center', y=140, font=FONT, font_size=40, opacity=25):
         """
         Draw text onto a Pillow image canvas.
 
         :param text: Text string
@@ -192,25 +191,32 @@
         :param opacity: Opacity of text to be drawn
         :return:
         """
         # Set drawing context
         d = ImageDraw.Draw(self.img)
 
         # Set a font
-        fnt = ImageFont.truetype(font, int(font_size * 1.00))  # multiply size of font if needed
+        fnt = ImageFont.truetype(font, int(font_size * 1.00))    # multiply size of font if needed
 
         # Check if x or y is set to 'center'
         x = self._text_centered_x(text, d, fnt) if 'center' in str(x).lower() else x
         y = self._text_centered_y(font_size) if 'center' in str(y).lower() else y
 
         # Draw text to image
         opacity = int(opacity * 100) if opacity < 1 else opacity
         d.text((x, y), text, font=fnt, fill=(0, 0, 0, opacity))
 
-    def draw_img(self, img, x='center', y='center', opacity=1.0, rotate=0, fit=1, scale_to_fit=True,
+    def draw_img(self,
+                 img,
+                 x='center',
+                 y='center',
+                 opacity=1.0,
+                 rotate=0,
+                 fit=1,
+                 scale_to_fit=True,
                  scale_multiplier=float(1)):
         """
         Scale an image to fit the canvas then alpha composite paste the image.
 
         Optionally place the image (x, y), adjust the images opacity
         or apply a rotation.
 
@@ -220,15 +226,15 @@
         :param opacity: Opacity value
         :param rotate: Rotation degrees
         :param fit: When true, expands image canvas size to fit rotated image
         :param scale_to_fit: When true, image is scaled to fit canvas size
         :param scale_multiplier: Value to multiple calculated scale by
         :return:
         """
-        img = img_adjust(img,opacity, rotate, fit, self.tempdir.name)
+        img = img_adjust(img, opacity, rotate, fit, self.tempdir.name)
         with Image.open(self.scale_to_fit(img, multiplier=scale_multiplier) if scale_to_fit else img) as image:
             x, y = self.image_bound(image, x, y)
             self.img.alpha_composite(image, (x, y))
 
     def rotate(self, rotate):
         # Create transparent image that is the same size as self.img
         mask = Image.new('L', self.img.size, 255)
```

### Comparing `PillowImage-1.1.9/PillowImage/utils.py` & `PillowImage-1.2.0/PillowImage/utils.py`

 * *Files identical despite different names*

### Comparing `PillowImage-1.1.9/README.md` & `PillowImage-1.2.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # PillowImage
 
 [![Build Status](https://travis-ci.com/sfneal/PillowImage.svg?branch=master)](https://travis-ci.com/sfneal/PillowImage)
 [![PyPi version](https://img.shields.io/pypi/v/PillowImage)](https://pypi.org/project/PillowImage)
 [![PyPi Python support](https://img.shields.io/pypi/pyversions/PillowImage)](https://pypi.org/project/PillowImage)
 [![PyPi downloads per month](https://img.shields.io/pypi/dm/PillowImage)](https://pypi.org/project/PillowImage)
 [![PyPi license](https://img.shields.io/pypi/l/PillowImage)](https://pypi.org/project/PillowImage)
+[![StyleCI](https://github.styleci.io/repos/179334000/shield?branch=master)](https://github.styleci.io/repos/179334000?branch=master)
+[![Scrutinizer Code Quality](https://scrutinizer-ci.com/g/sfneal/PillowImage/badges/quality-score.png?b=master)](https://scrutinizer-ci.com/g/sfneal/PillowImage/?branch=master)
 
 Pillow wrapper for quick image alterations.
 
 Package features:
 
 * Resize, rotate, stretch & scale images
 * Draw text
@@ -75,12 +77,12 @@
 
 ## Versioning
 
 We use [SemVer](http://semver.org/) for versioning. For the versions available, see the [tags on this repository](https://github.com/sfneal/PillowImage). 
 
 ## Authors
 
-* **Stephen Neal** - *Initial work* - [synfo](https://github.com/sfneal)
+* **Stephen Neal** - *Initial work* - [PillowImage](https://github.com/sfneal)
 
 ## License
 
 This project is licensed under the Apache License - see the [LICENSE.md](LICENSE.md) file for details
```

### Comparing `PillowImage-1.1.9/setup.py` & `PillowImage-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 setup(
     name=NAME,
     version=get_version(NAME),
     packages=find_packages(),
     python_requires='>=3.6',
     install_requires=[
         'reportlab>=3.5.19',
-        'Pillow>=7.0',
+        'Pillow>=9.0',
         'PyBundle>=1.0.6',
     ],
     include_package_data=True,
     url='https://github.com/sfneal/PillowImage',
     license='MIT',
     author='Stephen Neal',
     author_email='stephen@stephenneal.net',
```

### Comparing `PillowImage-1.1.9/tests/__init__.py` & `PillowImage-1.2.0/tests/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import os
 
-
 TEST_DATA_DIR = os.path.join(os.path.dirname(__file__), 'data')
 TEST_RESULTS_DIR = os.path.join(os.path.dirname(__file__), 'results')
 
 IMG_NAME = 'floor plan.png'
 IMG_PATH = os.path.join(TEST_DATA_DIR, IMG_NAME)
 
 IMG_NAME_JPEG = 'elevation.jpg'
@@ -31,9 +30,10 @@
         for f in os.listdir(folder):
             os.remove(os.path.join(folder, f))
     else:
         os.mkdir(folder)
     return folder
 
 
-__all__ = ['IMG_PATH', 'WTR_PATH', 'TEST_DATA_DIR', 'TEST_RESULTS_DIR', 'IMG_NAME_JPEG', 'IMG_PATH_JPEG',
-           'init_result_dir']
+__all__ = [
+    'IMG_PATH', 'WTR_PATH', 'TEST_DATA_DIR', 'TEST_RESULTS_DIR', 'IMG_NAME_JPEG', 'IMG_PATH_JPEG', 'init_result_dir'
+]
```

### Comparing `PillowImage-1.1.9/tests/test_PillowImage_jpeg.py` & `PillowImage-1.2.0/tests/test_PillowImage_png.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 
 from looptools import Timer
 
 from PillowImage import PillowImage
 from tests import *
 
 
-class TestPillowImageJPEG(unittest.TestCase):
-    result_dir = init_result_dir('jpg')
+class TestPillowImagePNG(unittest.TestCase):
+    result_dir = init_result_dir('png')
 
     @classmethod
     def setUpClass(cls):
-        cls.img_path = IMG_PATH_JPEG
+        cls.img_path = IMG_PATH
         cls.wtrmrk_path = WTR_PATH
         cls.pdf = None
 
     @Timer.decorator
     def test_draw_text(self):
         """Draw text onto an image."""
         with PillowImage() as draw:
@@ -150,41 +150,41 @@
             d = draw.save(destination=self.result_dir, file_name='size')
 
         # Assert file exists
         self.assertTrue(os.path.exists(d))
 
         # Assert image size is correct
         self.assertIsInstance(size, tuple)
-        self.assertTrue(size == (4094, 1317))
+        self.assertTrue(size == (2706, 2226))
         return d
 
     @Timer.decorator
     def test_width(self):
         """Draw text onto an image."""
         with PillowImage(img=self.img_path) as draw:
             width = draw.width
             d = draw.save(destination=self.result_dir, file_name='width')
 
         # Assert file exists
         self.assertTrue(os.path.exists(d))
 
         # Assert image size is correct
-        self.assertTrue(width == 4094)
+        self.assertTrue(width == 2706)
         return d
 
     @Timer.decorator
     def test_height(self):
         """Draw text onto an image."""
         with PillowImage(img=self.img_path) as draw:
             height = draw.height
             d = draw.save(destination=self.result_dir, file_name='height')
 
         # Assert file exists
         self.assertTrue(os.path.exists(d))
 
         # Assert image size is correct
-        self.assertTrue(height == 1317)
+        self.assertTrue(height == 2226)
         return d
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `PillowImage-1.1.9/tests/test_PillowImage_png.py` & `PillowImage-1.2.0/tests/test_PillowImage_jpeg.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,94 +3,94 @@
 
 from looptools import Timer
 
 from PillowImage import PillowImage
 from tests import *
 
 
-class TestPillowImagePNG(unittest.TestCase):
-    result_dir = init_result_dir('png')
-    
+class TestPillowImageJPEG(unittest.TestCase):
+    result_dir = init_result_dir('jpg')
+
     @classmethod
     def setUpClass(cls):
-        cls.img_path = IMG_PATH
+        cls.img_path = IMG_PATH_JPEG
         cls.wtrmrk_path = WTR_PATH
         cls.pdf = None
 
     @Timer.decorator
     def test_draw_text(self):
-        """Draw text onto an image."""
+        """Draw text onto a black canvas."""
         with PillowImage() as draw:
             draw.draw_text('Here is the first text', y=10, opacity=50)
             draw.draw_text('Here is the second text', y=50, opacity=50)
             d = draw.save(destination=self.result_dir, file_name='draw_text')
 
         # Assert file exists
         self.assertTrue(os.path.exists(d))
         return d
 
     @Timer.decorator
     def test_draw_img(self):
-        """Draw text onto an image."""
+        """Draw text and an image onto a black canvas."""
         with PillowImage() as draw:
             draw.draw_img(self.img_path)
             draw.draw_img(self.wtrmrk_path, opacity=0.08, rotate=30)
             d = draw.save(destination=self.result_dir, file_name='draw_img')
 
         # Assert file exists
         self.assertTrue(os.path.exists(d))
         return d
 
     @Timer.decorator
     def test_draw_img_overlay(self):
-        """Draw text onto an image."""
+        """Overlay text onto an image."""
         with PillowImage(img=self.img_path) as draw:
             draw.draw_img(self.wtrmrk_path, opacity=0.08, rotate=30)
             d = draw.save(destination=self.result_dir, file_name='draw_img_overlay')
 
         # Assert file exists
         self.assertTrue(os.path.exists(d))
         return d
 
     @Timer.decorator
     def test_draw_img_centered(self):
-        """Draw text onto an image."""
+        """Draw centered text onto an image."""
         with PillowImage(img=self.img_path) as draw:
             draw.draw_img(self.wtrmrk_path, opacity=0.08, rotate=30, x='center', y='center')
             d = draw.save(destination=self.result_dir, file_name='draw_img_centered')
 
         # Assert file exists
         self.assertTrue(os.path.exists(d))
         return d
 
     @Timer.decorator
     def test_draw_img_negbound(self):
-        """Draw text onto an image."""
+        """Draw text onto an image with a negative bound."""
         with PillowImage(img=self.img_path) as draw:
             draw.draw_img(self.wtrmrk_path, opacity=0.08, rotate=30, x=-2000, y=-2000)
             d = draw.save(destination=self.result_dir, file_name='draw_img_negbound')
 
         # Assert file exists
         self.assertTrue(os.path.exists(d))
         return d
 
     @Timer.decorator
     def test_draw_img_percentage(self):
-        """Draw text onto an image."""
+        """Draw text onto an image based on percentage."""
         with PillowImage(img=self.img_path) as draw:
             draw.draw_img(self.wtrmrk_path, opacity=0.08, rotate=30, x=.5, y=.1)
             d = draw.save(destination=self.result_dir, file_name='draw_img_percentage')
 
         # Assert file exists
         self.assertTrue(os.path.exists(d))
         return d
 
     @Timer.decorator
     def test_draw_img_resized(self):
-        """Draw text onto an image."""
+        """Draw text onto a resized image."""
         longest_side = 500
         with PillowImage(img=self.img_path) as draw:
             draw.draw_img(self.wtrmrk_path, opacity=0.08, rotate=30)
             draw.resize(longest_side)
             d = draw.save(destination=self.result_dir, file_name='draw_img_resized')
 
         # Assert file exists
@@ -98,93 +98,93 @@
 
         # Assert actual longest edge is equal to target longest edge
         self.assertEqual(longest_side, draw.longest_side)
         return d
 
     @Timer.decorator
     def test_draw_img_resize_width(self):
-        """Draw text onto an image."""
+        """Draw text onto a horizontally resized image."""
         width = 300
         with PillowImage(img=self.img_path) as draw:
             draw.resize_width(width)
             d = draw.save(destination=self.result_dir, file_name='draw_img_resized_width')
 
         # Assert file exists
         self.assertTrue(os.path.exists(d))
 
         # Assert actual longest edge is equal to target longest edge
         self.assertEqual(width, draw.width)
         return d
 
     @Timer.decorator
     def test_draw_img_resize_height(self):
-        """Draw text onto an image."""
+        """Draw text onto a vertically resized image."""
         height = 300
         with PillowImage(img=self.img_path) as draw:
             draw.resize_height(height)
             d = draw.save(destination=self.result_dir, file_name='draw_img_resized_height')
 
         # Assert file exists
         self.assertTrue(os.path.exists(d))
 
         # Assert actual longest edge is equal to target longest edge
         self.assertEqual(height, draw.height)
         return d
 
     @Timer.decorator
     def test_rotate(self):
-        """Draw text onto an image."""
+        """Draw a rotated image."""
         with PillowImage() as draw:
             draw.draw_img(self.img_path)
             draw.rotate(30)
             d = draw.save(destination=self.result_dir, file_name='rotate')
 
         # Assert file exists
         self.assertTrue(os.path.exists(d))
         return d
 
     @Timer.decorator
     def test_size(self):
-        """Draw text onto an image."""
+        """Draw text onto an image with a modified size."""
         with PillowImage(img=self.img_path) as draw:
             size = draw.size
             d = draw.save(destination=self.result_dir, file_name='size')
 
         # Assert file exists
         self.assertTrue(os.path.exists(d))
 
         # Assert image size is correct
         self.assertIsInstance(size, tuple)
-        self.assertTrue(size == (2706, 2226))
+        self.assertTrue(size == (4094, 1317))
         return d
 
     @Timer.decorator
     def test_width(self):
-        """Draw text onto an image."""
+        """Test the width of an image."""
         with PillowImage(img=self.img_path) as draw:
             width = draw.width
             d = draw.save(destination=self.result_dir, file_name='width')
 
         # Assert file exists
         self.assertTrue(os.path.exists(d))
 
         # Assert image size is correct
-        self.assertTrue(width == 2706)
+        self.assertTrue(width == 4094)
         return d
 
     @Timer.decorator
     def test_height(self):
-        """Draw text onto an image."""
+        """Test the height of an image."""
         with PillowImage(img=self.img_path) as draw:
             height = draw.height
             d = draw.save(destination=self.result_dir, file_name='height')
 
         # Assert file exists
         self.assertTrue(os.path.exists(d))
 
         # Assert image size is correct
-        self.assertTrue(height == 2226)
+        self.assertTrue(height == 1317)
         return d
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `PillowImage-1.1.9/tests/test_PillowImage_utils.py` & `PillowImage-1.2.0/tests/test_PillowImage_utils.py`

 * *Files identical despite different names*

