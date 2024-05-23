# Comparing `tmp/grayscale_to_rgb-1.0.1-py3-none-any.whl.zip` & `tmp/grayscale_to_rgb-1.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,10 @@
-Zip file size: 4323 bytes, number of entries: 7
--rw-r--r--  2.0 unx      160 b- defN 24-May-16 14:12 __init__.py
+Zip file size: 4584 bytes, number of entries: 8
+-rw-r--r--  2.0 unx      160 b- defN 24-May-23 11:58 __init__.py
 -rw-r--r--  2.0 unx     2054 b- defN 24-May-16 14:13 grayscale_to_rgb.py
 -rw-r--r--  2.0 unx     2054 b- defN 24-May-16 14:13 grayscale_to_rgb/grayscale_to_rgb.py
--rw-r--r--  2.0 unx     2032 b- defN 24-May-23 11:24 grayscale_to_rgb-1.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-23 11:24 grayscale_to_rgb-1.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       26 b- defN 24-May-23 11:24 grayscale_to_rgb-1.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      570 b- defN 24-May-23 11:24 grayscale_to_rgb-1.0.1.dist-info/RECORD
-7 files, 6988 bytes uncompressed, 3309 bytes compressed:  52.6%
+-rw-r--r--  2.0 unx     2032 b- defN 24-May-23 11:59 grayscale_to_rgb-1.1.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-23 11:59 grayscale_to_rgb-1.1.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       58 b- defN 24-May-23 11:59 grayscale_to_rgb-1.1.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       17 b- defN 24-May-23 11:59 grayscale_to_rgb-1.1.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      674 b- defN 24-May-23 11:59 grayscale_to_rgb-1.1.0.dist-info/RECORD
+8 files, 7141 bytes uncompressed, 3396 bytes compressed:  52.4%
```

## zipnote {}

```diff
@@ -3,20 +3,23 @@
 
 Filename: grayscale_to_rgb.py
 Comment: 
 
 Filename: grayscale_to_rgb/grayscale_to_rgb.py
 Comment: 
 
-Filename: grayscale_to_rgb-1.0.1.dist-info/METADATA
+Filename: grayscale_to_rgb-1.1.0.dist-info/METADATA
 Comment: 
 
-Filename: grayscale_to_rgb-1.0.1.dist-info/WHEEL
+Filename: grayscale_to_rgb-1.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: grayscale_to_rgb-1.0.1.dist-info/top_level.txt
+Filename: grayscale_to_rgb-1.1.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: grayscale_to_rgb-1.0.1.dist-info/RECORD
+Filename: grayscale_to_rgb-1.1.0.dist-info/top_level.txt
+Comment: 
+
+Filename: grayscale_to_rgb-1.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## __init__.py

```diff
@@ -1,9 +1,9 @@
 """
 grayscale-to-rgb
 
 Mapping grayscale images to RGB
 """
 
-__version__ = "1.0.1"
+__version__ = "1.1.0"
 __author__ = 'Elina Jansone'
 __credits__ = 'Functional Genomics Center Zurich'
```

## Comparing `grayscale_to_rgb-1.0.1.dist-info/METADATA` & `grayscale_to_rgb-1.1.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grayscale-to-rgb
-Version: 1.0.1
+Version: 1.1.0
 Summary: Mapping grayscale images to RGB
 Home-page: https://gitlab.bfabric.org/jens/grayscale-to-rgb
 Author: Elina Jansone
 Author-email: hertaelina@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

