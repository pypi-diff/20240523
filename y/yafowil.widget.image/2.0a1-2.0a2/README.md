# Comparing `tmp/yafowil.widget.image-2.0a1.tar.gz` & `tmp/yafowil_widget_image-2.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yafowil.widget.image-2.0a1.tar", last modified: Mon May 15 12:44:45 2023, max compression
+gzip compressed data, was "yafowil_widget_image-2.0a2.tar", last modified: Thu May 23 14:22:19 2024, max compression
```

## Comparing `yafowil.widget.image-2.0a1.tar` & `yafowil_widget_image-2.0a2.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:44:45.960886 yafowil.widget.image-2.0a1/
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1674 2023-05-15 12:44:45.000000 yafowil.widget.image-2.0a1/CHANGES.rst
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1403 2023-05-15 12:44:45.000000 yafowil.widget.image-2.0a1/LICENSE.rst
--rw-r--r--   0 rnix      (1000) rnix      (1000)       72 2023-05-15 12:44:45.000000 yafowil.widget.image-2.0a1/MANIFEST.in
--rw-r--r--   0 rnix      (1000) rnix      (1000)     4391 2023-05-15 12:44:45.960886 yafowil.widget.image-2.0a1/PKG-INFO
--rw-r--r--   0 rnix      (1000) rnix      (1000)      574 2023-05-15 12:44:45.000000 yafowil.widget.image-2.0a1/README.rst
--rw-r--r--   0 rnix      (1000) rnix      (1000)       38 2023-05-15 12:44:45.960886 yafowil.widget.image-2.0a1/setup.cfg
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1736 2023-05-15 12:44:45.000000 yafowil.widget.image-2.0a1/setup.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:44:45.960886 yafowil.widget.image-2.0a1/src/
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:44:45.960886 yafowil.widget.image-2.0a1/src/yafowil/
--rw-r--r--   0 rnix      (1000) rnix      (1000)       56 2023-05-15 12:44:45.000000 yafowil.widget.image-2.0a1/src/yafowil/__init__.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:44:45.960886 yafowil.widget.image-2.0a1/src/yafowil/widget/
--rw-r--r--   0 rnix      (1000) rnix      (1000)       56 2023-05-15 12:44:45.000000 yafowil.widget.image-2.0a1/src/yafowil/widget/__init__.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:44:45.960886 yafowil.widget.image-2.0a1/src/yafowil/widget/image/
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1588 2023-05-15 12:44:45.000000 yafowil.widget.image-2.0a1/src/yafowil/widget/image/__init__.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)      608 2023-05-15 12:44:45.000000 yafowil.widget.image-2.0a1/src/yafowil/widget/image/configure.zcml
--rw-r--r--   0 rnix      (1000) rnix      (1000)     4031 2023-05-15 12:44:45.000000 yafowil.widget.image-2.0a1/src/yafowil/widget/image/example.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:44:45.960886 yafowil.widget.image-2.0a1/src/yafowil/widget/image/locales/
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:44:45.960886 yafowil.widget.image-2.0a1/src/yafowil/widget/image/locales/de/
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:44:45.960886 yafowil.widget.image-2.0a1/src/yafowil/widget/image/locales/de/LC_MESSAGES/
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1259 2023-05-15 12:44:45.000000 yafowil.widget.image-2.0a1/src/yafowil/widget/image/locales/de/LC_MESSAGES/yafowil.widget.image.mo
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2295 2023-05-15 12:44:45.000000 yafowil.widget.image-2.0a1/src/yafowil/widget/image/locales/de/LC_MESSAGES/yafowil.widget.image.po
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:44:45.960886 yafowil.widget.image-2.0a1/src/yafowil/widget/image/locales/en/
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:44:45.960886 yafowil.widget.image-2.0a1/src/yafowil/widget/image/locales/en/LC_MESSAGES/
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1230 2023-05-15 12:44:45.000000 yafowil.widget.image-2.0a1/src/yafowil/widget/image/locales/en/LC_MESSAGES/yafowil.widget.image.mo
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2261 2023-05-15 12:44:45.000000 yafowil.widget.image-2.0a1/src/yafowil/widget/image/locales/en/LC_MESSAGES/yafowil.widget.image.po
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1693 2023-05-15 12:44:45.000000 yafowil.widget.image-2.0a1/src/yafowil/widget/image/locales/yafowil.widget.image.pot
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:44:45.960886 yafowil.widget.image-2.0a1/src/yafowil/widget/image/resources/
--rw-r--r--   0 rnix      (1000) rnix      (1000)       97 2023-05-15 12:44:45.000000 yafowil.widget.image-2.0a1/src/yafowil/widget/image/resources/widget.css
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1468 2023-05-15 12:44:45.000000 yafowil.widget.image-2.0a1/src/yafowil/widget/image/resources/widget.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)      747 2023-05-15 12:44:45.000000 yafowil.widget.image-2.0a1/src/yafowil/widget/image/resources/widget.min.js
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:44:45.960886 yafowil.widget.image-2.0a1/src/yafowil/widget/image/testing/
--rw-r--r--   0 rnix      (1000) rnix      (1000)        1 2023-05-15 12:44:45.000000 yafowil.widget.image-2.0a1/src/yafowil/widget/image/testing/__init__.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)      698 2023-05-15 12:44:45.000000 yafowil.widget.image-2.0a1/src/yafowil/widget/image/testing/dummy.jpg
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1239 2023-05-15 12:44:45.000000 yafowil.widget.image-2.0a1/src/yafowil/widget/image/testing/dummy.pdf
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1853 2023-05-15 12:44:45.000000 yafowil.widget.image-2.0a1/src/yafowil/widget/image/testing/dummy.png
--rw-r--r--   0 rnix      (1000) rnix      (1000)    41672 2023-05-15 12:44:45.000000 yafowil.widget.image-2.0a1/src/yafowil/widget/image/tests.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)      785 2023-05-15 12:44:45.000000 yafowil.widget.image-2.0a1/src/yafowil/widget/image/utils.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)    12283 2023-05-15 12:44:45.000000 yafowil.widget.image-2.0a1/src/yafowil/widget/image/widget.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:44:45.960886 yafowil.widget.image-2.0a1/src/yafowil.widget.image.egg-info/
--rw-r--r--   0 rnix      (1000) rnix      (1000)     4391 2023-05-15 12:44:45.000000 yafowil.widget.image-2.0a1/src/yafowil.widget.image.egg-info/PKG-INFO
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1380 2023-05-15 12:44:45.000000 yafowil.widget.image-2.0a1/src/yafowil.widget.image.egg-info/SOURCES.txt
--rw-r--r--   0 rnix      (1000) rnix      (1000)        1 2023-05-15 12:44:45.000000 yafowil.widget.image-2.0a1/src/yafowil.widget.image.egg-info/dependency_links.txt
--rw-r--r--   0 rnix      (1000) rnix      (1000)      109 2023-05-15 12:44:45.000000 yafowil.widget.image-2.0a1/src/yafowil.widget.image.egg-info/entry_points.txt
--rw-r--r--   0 rnix      (1000) rnix      (1000)       23 2023-05-15 12:44:45.000000 yafowil.widget.image-2.0a1/src/yafowil.widget.image.egg-info/namespace_packages.txt
--rw-r--r--   0 rnix      (1000) rnix      (1000)        1 2023-05-15 12:44:45.000000 yafowil.widget.image-2.0a1/src/yafowil.widget.image.egg-info/not-zip-safe
--rw-r--r--   0 rnix      (1000) rnix      (1000)       62 2023-05-15 12:44:45.000000 yafowil.widget.image-2.0a1/src/yafowil.widget.image.egg-info/requires.txt
--rw-r--r--   0 rnix      (1000) rnix      (1000)        8 2023-05-15 12:44:45.000000 yafowil.widget.image-2.0a1/src/yafowil.widget.image.egg-info/top_level.txt
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-05-23 14:22:19.263442 yafowil_widget_image-2.0a2/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1813 2024-05-23 14:22:19.000000 yafowil_widget_image-2.0a2/CHANGES.rst
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1403 2024-05-23 14:22:19.000000 yafowil_widget_image-2.0a2/LICENSE.rst
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       72 2024-05-23 14:22:19.000000 yafowil_widget_image-2.0a2/MANIFEST.in
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     4693 2024-05-23 14:22:19.263442 yafowil_widget_image-2.0a2/PKG-INFO
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      574 2024-05-23 14:22:19.000000 yafowil_widget_image-2.0a2/README.rst
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       38 2024-05-23 14:22:19.263442 yafowil_widget_image-2.0a2/setup.cfg
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1736 2024-05-23 14:22:19.000000 yafowil_widget_image-2.0a2/setup.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-05-23 14:22:19.259442 yafowil_widget_image-2.0a2/src/
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-05-23 14:22:19.259442 yafowil_widget_image-2.0a2/src/yafowil/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       56 2024-05-23 14:22:19.000000 yafowil_widget_image-2.0a2/src/yafowil/__init__.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-05-23 14:22:19.259442 yafowil_widget_image-2.0a2/src/yafowil/widget/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       56 2024-05-23 14:22:19.000000 yafowil_widget_image-2.0a2/src/yafowil/widget/__init__.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-05-23 14:22:19.259442 yafowil_widget_image-2.0a2/src/yafowil/widget/image/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1588 2024-05-23 14:22:19.000000 yafowil_widget_image-2.0a2/src/yafowil/widget/image/__init__.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      608 2024-05-23 14:22:19.000000 yafowil_widget_image-2.0a2/src/yafowil/widget/image/configure.zcml
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     4031 2024-05-23 14:22:19.000000 yafowil_widget_image-2.0a2/src/yafowil/widget/image/example.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-05-23 14:22:19.259442 yafowil_widget_image-2.0a2/src/yafowil/widget/image/locales/
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-05-23 14:22:19.259442 yafowil_widget_image-2.0a2/src/yafowil/widget/image/locales/de/
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-05-23 14:22:19.259442 yafowil_widget_image-2.0a2/src/yafowil/widget/image/locales/de/LC_MESSAGES/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1259 2024-05-23 14:22:19.000000 yafowil_widget_image-2.0a2/src/yafowil/widget/image/locales/de/LC_MESSAGES/yafowil.widget.image.mo
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2295 2024-05-23 14:22:19.000000 yafowil_widget_image-2.0a2/src/yafowil/widget/image/locales/de/LC_MESSAGES/yafowil.widget.image.po
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-05-23 14:22:19.259442 yafowil_widget_image-2.0a2/src/yafowil/widget/image/locales/en/
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-05-23 14:22:19.263442 yafowil_widget_image-2.0a2/src/yafowil/widget/image/locales/en/LC_MESSAGES/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1230 2024-05-23 14:22:19.000000 yafowil_widget_image-2.0a2/src/yafowil/widget/image/locales/en/LC_MESSAGES/yafowil.widget.image.mo
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2261 2024-05-23 14:22:19.000000 yafowil_widget_image-2.0a2/src/yafowil/widget/image/locales/en/LC_MESSAGES/yafowil.widget.image.po
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1693 2024-05-23 14:22:19.000000 yafowil_widget_image-2.0a2/src/yafowil/widget/image/locales/yafowil.widget.image.pot
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-05-23 14:22:19.263442 yafowil_widget_image-2.0a2/src/yafowil/widget/image/resources/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       97 2024-05-23 14:22:19.000000 yafowil_widget_image-2.0a2/src/yafowil/widget/image/resources/widget.css
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1468 2024-05-23 14:22:19.000000 yafowil_widget_image-2.0a2/src/yafowil/widget/image/resources/widget.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      747 2024-05-23 14:22:19.000000 yafowil_widget_image-2.0a2/src/yafowil/widget/image/resources/widget.min.js
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-05-23 14:22:19.263442 yafowil_widget_image-2.0a2/src/yafowil/widget/image/testing/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)        1 2024-05-23 14:22:19.000000 yafowil_widget_image-2.0a2/src/yafowil/widget/image/testing/__init__.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      698 2024-05-23 14:22:19.000000 yafowil_widget_image-2.0a2/src/yafowil/widget/image/testing/dummy.jpg
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1239 2024-05-23 14:22:19.000000 yafowil_widget_image-2.0a2/src/yafowil/widget/image/testing/dummy.pdf
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1853 2024-05-23 14:22:19.000000 yafowil_widget_image-2.0a2/src/yafowil/widget/image/testing/dummy.png
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    41672 2024-05-23 14:22:19.000000 yafowil_widget_image-2.0a2/src/yafowil/widget/image/tests.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      785 2024-05-23 14:22:19.000000 yafowil_widget_image-2.0a2/src/yafowil/widget/image/utils.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    12313 2024-05-23 14:22:19.000000 yafowil_widget_image-2.0a2/src/yafowil/widget/image/widget.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-05-23 14:22:19.263442 yafowil_widget_image-2.0a2/src/yafowil.widget.image.egg-info/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     4693 2024-05-23 14:22:19.000000 yafowil_widget_image-2.0a2/src/yafowil.widget.image.egg-info/PKG-INFO
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1380 2024-05-23 14:22:19.000000 yafowil_widget_image-2.0a2/src/yafowil.widget.image.egg-info/SOURCES.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)        1 2024-05-23 14:22:19.000000 yafowil_widget_image-2.0a2/src/yafowil.widget.image.egg-info/dependency_links.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      109 2024-05-23 14:22:19.000000 yafowil_widget_image-2.0a2/src/yafowil.widget.image.egg-info/entry_points.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       23 2024-05-23 14:22:19.000000 yafowil_widget_image-2.0a2/src/yafowil.widget.image.egg-info/namespace_packages.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)        1 2024-05-23 14:22:19.000000 yafowil_widget_image-2.0a2/src/yafowil.widget.image.egg-info/not-zip-safe
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       62 2024-05-23 14:22:19.000000 yafowil_widget_image-2.0a2/src/yafowil.widget.image.egg-info/requires.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)        8 2024-05-23 14:22:19.000000 yafowil_widget_image-2.0a2/src/yafowil.widget.image.egg-info/top_level.txt
```

### Comparing `yafowil.widget.image-2.0a1/CHANGES.rst` & `yafowil_widget_image-2.0a2/CHANGES.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,20 @@
 Changes
 =======
 
+2.0a2 (2024-05-23)
+------------------
+
+- Fix deprecated imports.
+  [rnix]
+
+- Use Image.Resampling.LANCZOS instead of ANTIALIAS.
+  [rnix]
+
+
 2.0a1 (2023-05-15)
 ------------------
 
 - Add ``webresource`` support.
   [rnix]
 
 - Rewrite JavaScript using ES6.
```

### Comparing `yafowil.widget.image-2.0a1/LICENSE.rst` & `yafowil_widget_image-2.0a2/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `yafowil.widget.image-2.0a1/PKG-INFO` & `yafowil_widget_image-2.0a2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 Metadata-Version: 2.1
 Name: yafowil.widget.image
-Version: 2.0a1
+Version: 2.0a2
 Summary: Image Widget for YAFOWIL
 Home-page: http://github.com/conestack/yafowil.widget.image
 Author: Yafowil Contributors
 Author-email: dev@conestack.org
 License: Simplified BSD
 Classifier: Environment :: Web Environment
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
-Provides-Extra: test
 License-File: LICENSE.rst
+Requires-Dist: Pillow
+Requires-Dist: setuptools
+Requires-Dist: yafowil>2.1.99
+Provides-Extra: test
+Requires-Dist: lxml; extra == "test"
+Requires-Dist: zope.testrunner; extra == "test"
 
 This is an **image widget** for for `YAFOWIL
 <http://pypi.python.org/pypi/yafowil>`_ .
 
 - `Documentation <http://docs.yafowil.info/en/latest/blueprints.html#image>`_
 - `DEMO - see it Live <http://demo.yafowil.info/++widget++yafowil.widget.image/index.html>`_
 
@@ -43,14 +48,24 @@
 
 - Lena Daxenbichler
 
 
 Changes
 =======
 
+2.0a2 (2024-05-23)
+------------------
+
+- Fix deprecated imports.
+  [rnix]
+
+- Use Image.Resampling.LANCZOS instead of ANTIALIAS.
+  [rnix]
+
+
 2.0a1 (2023-05-15)
 ------------------
 
 - Add ``webresource`` support.
   [rnix]
 
 - Rewrite JavaScript using ES6.
```

### Comparing `yafowil.widget.image-2.0a1/README.rst` & `yafowil_widget_image-2.0a2/README.rst`

 * *Files identical despite different names*

### Comparing `yafowil.widget.image-2.0a1/setup.py` & `yafowil_widget_image-2.0a2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 def read_file(name):
     with open(os.path.join(os.path.dirname(__file__), name)) as f:
         return f.read()
 
 
-version = '2.0a1'
+version = '2.0a2'
 shortdesc = 'Image Widget for YAFOWIL'
 longdesc = '\n\n'.join([read_file(name) for name in [
     'README.rst',
     'CHANGES.rst',
     'LICENSE.rst'
 ]])
```

### Comparing `yafowil.widget.image-2.0a1/src/yafowil/widget/image/__init__.py` & `yafowil_widget_image-2.0a2/src/yafowil/widget/image/__init__.py`

 * *Files identical despite different names*

### Comparing `yafowil.widget.image-2.0a1/src/yafowil/widget/image/configure.zcml` & `yafowil_widget_image-2.0a2/src/yafowil/widget/image/configure.zcml`

 * *Files identical despite different names*

### Comparing `yafowil.widget.image-2.0a1/src/yafowil/widget/image/example.py` & `yafowil_widget_image-2.0a2/src/yafowil/widget/image/example.py`

 * *Files identical despite different names*

### Comparing `yafowil.widget.image-2.0a1/src/yafowil/widget/image/locales/de/LC_MESSAGES/yafowil.widget.image.mo` & `yafowil_widget_image-2.0a2/src/yafowil/widget/image/locales/de/LC_MESSAGES/yafowil.widget.image.mo`

 * *Files identical despite different names*

### Comparing `yafowil.widget.image-2.0a1/src/yafowil/widget/image/locales/de/LC_MESSAGES/yafowil.widget.image.po` & `yafowil_widget_image-2.0a2/src/yafowil/widget/image/locales/de/LC_MESSAGES/yafowil.widget.image.po`

 * *Files identical despite different names*

### Comparing `yafowil.widget.image-2.0a1/src/yafowil/widget/image/locales/en/LC_MESSAGES/yafowil.widget.image.mo` & `yafowil_widget_image-2.0a2/src/yafowil/widget/image/locales/en/LC_MESSAGES/yafowil.widget.image.mo`

 * *Files identical despite different names*

### Comparing `yafowil.widget.image-2.0a1/src/yafowil/widget/image/locales/en/LC_MESSAGES/yafowil.widget.image.po` & `yafowil_widget_image-2.0a2/src/yafowil/widget/image/locales/en/LC_MESSAGES/yafowil.widget.image.po`

 * *Files identical despite different names*

### Comparing `yafowil.widget.image-2.0a1/src/yafowil/widget/image/locales/yafowil.widget.image.pot` & `yafowil_widget_image-2.0a2/src/yafowil/widget/image/locales/yafowil.widget.image.pot`

 * *Files identical despite different names*

### Comparing `yafowil.widget.image-2.0a1/src/yafowil/widget/image/resources/widget.js` & `yafowil_widget_image-2.0a2/src/yafowil/widget/image/resources/widget.js`

 * *Files identical despite different names*

### Comparing `yafowil.widget.image-2.0a1/src/yafowil/widget/image/resources/widget.min.js` & `yafowil_widget_image-2.0a2/src/yafowil/widget/image/resources/widget.min.js`

 * *Files identical despite different names*

### Comparing `yafowil.widget.image-2.0a1/src/yafowil/widget/image/testing/dummy.jpg` & `yafowil_widget_image-2.0a2/src/yafowil/widget/image/testing/dummy.jpg`

 * *Files identical despite different names*

### Comparing `yafowil.widget.image-2.0a1/src/yafowil/widget/image/testing/dummy.pdf` & `yafowil_widget_image-2.0a2/src/yafowil/widget/image/testing/dummy.pdf`

 * *Files identical despite different names*

### Comparing `yafowil.widget.image-2.0a1/src/yafowil/widget/image/testing/dummy.png` & `yafowil_widget_image-2.0a2/src/yafowil/widget/image/testing/dummy.png`

 * *Files identical despite different names*

### Comparing `yafowil.widget.image-2.0a1/src/yafowil/widget/image/tests.py` & `yafowil_widget_image-2.0a2/src/yafowil/widget/image/tests.py`

 * *Files identical despite different names*

### Comparing `yafowil.widget.image-2.0a1/src/yafowil/widget/image/utils.py` & `yafowil_widget_image-2.0a2/src/yafowil/widget/image/utils.py`

 * *Files identical despite different names*

### Comparing `yafowil.widget.image-2.0a1/src/yafowil/widget/image/widget.py` & `yafowil_widget_image-2.0a2/src/yafowil/widget/image/widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from PIL import Image
 from node.utils import UNSET
 from yafowil.base import ExtractionError
 from yafowil.base import factory
-from yafowil.common import file_extractor
-from yafowil.common import file_options_renderer
 from yafowil.common import generic_required_extractor
-from yafowil.common import input_file_edit_renderer
+from yafowil.file import file_extractor
+from yafowil.file import file_options_renderer
+from yafowil.file import input_file_edit_renderer
 from yafowil.tsf import TSF
 from yafowil.utils import attr_value
 from yafowil.utils import css_managed_props
 from yafowil.utils import cssid
 from yafowil.utils import managedprops
 from yafowil.widget.image.utils import aspect_ratio_approximate
 from yafowil.widget.image.utils import same_aspect_ratio
@@ -176,15 +176,15 @@
             image_size = size
         # scale x
         if image_appr > scale_appr:
             image_size = scale_size(image.size, (size[0], None))
         # scale y
         if image_appr < scale_appr:
             image_size = scale_size(image.size, (None, size[1]))
-        scaled_images[name] = image.resize(image_size, Image.ANTIALIAS)
+        scaled_images[name] = image.resize(image_size, Image.Resampling.LANCZOS)
     data.extracted['scales'] = scaled_images
     return data.extracted
 
 
 @managedprops('crop')
 def crop_extractor(widget, data):
     """XXX:
@@ -202,25 +202,25 @@
     offset = crop.get('offset', (0, 0))
     fitting = crop.get('fitting', False)
     image = data.extracted['image']
     image_appr = aspect_ratio_approximate(image.size)
     crop_appr = aspect_ratio_approximate(size)
     if fitting:
         if same_aspect_ratio(size, image.size):
-            image = image.resize(size, Image.ANTIALIAS)
+            image = image.resize(size, Image.Resampling.LANCZOS)
             offset = (0, 0)
         # scale x
         if image_appr < crop_appr:
             image_size = scale_size(image.size, (size[0], None))
-            image = image.resize(image_size, Image.ANTIALIAS)
+            image = image.resize(image_size, Image.Resampling.LANCZOS)
             offset = (0, (image_size[1] - size[1]) / 2)
         # scale y
         if image_appr > crop_appr:
             image_size = scale_size(image.size, (None, size[1]))
-            image = image.resize(image_size, Image.ANTIALIAS)
+            image = image.resize(image_size, Image.Resampling.LANCZOS)
             offset = ((image_size[0] - size[0]) / 2, 0)
     image = image.crop(
         (offset[0], offset[1], size[0] + offset[0], size[1] + offset[1]))
     data.extracted['cropped'] = image
     return data.extracted
```

### Comparing `yafowil.widget.image-2.0a1/src/yafowil.widget.image.egg-info/PKG-INFO` & `yafowil_widget_image-2.0a2/src/yafowil.widget.image.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 Metadata-Version: 2.1
 Name: yafowil.widget.image
-Version: 2.0a1
+Version: 2.0a2
 Summary: Image Widget for YAFOWIL
 Home-page: http://github.com/conestack/yafowil.widget.image
 Author: Yafowil Contributors
 Author-email: dev@conestack.org
 License: Simplified BSD
 Classifier: Environment :: Web Environment
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
-Provides-Extra: test
 License-File: LICENSE.rst
+Requires-Dist: Pillow
+Requires-Dist: setuptools
+Requires-Dist: yafowil>2.1.99
+Provides-Extra: test
+Requires-Dist: lxml; extra == "test"
+Requires-Dist: zope.testrunner; extra == "test"
 
 This is an **image widget** for for `YAFOWIL
 <http://pypi.python.org/pypi/yafowil>`_ .
 
 - `Documentation <http://docs.yafowil.info/en/latest/blueprints.html#image>`_
 - `DEMO - see it Live <http://demo.yafowil.info/++widget++yafowil.widget.image/index.html>`_
 
@@ -43,14 +48,24 @@
 
 - Lena Daxenbichler
 
 
 Changes
 =======
 
+2.0a2 (2024-05-23)
+------------------
+
+- Fix deprecated imports.
+  [rnix]
+
+- Use Image.Resampling.LANCZOS instead of ANTIALIAS.
+  [rnix]
+
+
 2.0a1 (2023-05-15)
 ------------------
 
 - Add ``webresource`` support.
   [rnix]
 
 - Rewrite JavaScript using ES6.
```

### Comparing `yafowil.widget.image-2.0a1/src/yafowil.widget.image.egg-info/SOURCES.txt` & `yafowil_widget_image-2.0a2/src/yafowil.widget.image.egg-info/SOURCES.txt`

 * *Files identical despite different names*

