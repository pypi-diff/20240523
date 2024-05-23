# Comparing `tmp/mlab_py-0.5.0.tar.gz` & `tmp/mlab_py-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlab_py-0.5.0.tar", max compression
+gzip compressed data, was "mlab_py-0.5.1.tar", max compression
```

## Comparing `mlab_py-0.5.0.tar` & `mlab_py-0.5.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        8 2024-05-22 22:06:07.525956 mlab_py-0.5.0/README.md
--rw-r--r--   0        0        0      388 2024-05-23 14:35:31.605387 mlab_py-0.5.0/pymlab/__init__.py
--rw-r--r--   0        0        0     1854 2024-05-23 14:42:03.689669 mlab_py-0.5.0/pymlab/main.py
--rw-r--r--   0        0        0     2524 2024-05-23 14:45:07.714237 mlab_py-0.5.0/pymlab/test.py
--rw-r--r--   0        0        0     2176 2024-05-23 14:44:59.601775 mlab_py-0.5.0/pymlab/train.py
--rw-r--r--   0        0        0     2337 2024-05-23 07:44:20.219924 mlab_py-0.5.0/pymlab/utils.py
--rw-r--r--   0        0        0      371 2024-05-23 14:47:27.097420 mlab_py-0.5.0/pyproject.toml
--rw-r--r--   0        0        0      545 1970-01-01 00:00:00.000000 mlab_py-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0        8 2024-05-22 22:06:07.525956 mlab_py-0.5.1/README.md
+-rw-r--r--   0        0        0      388 2024-05-23 14:35:31.605387 mlab_py-0.5.1/pymlab/__init__.py
+-rw-r--r--   0        0        0     1854 2024-05-23 14:42:03.689669 mlab_py-0.5.1/pymlab/main.py
+-rw-r--r--   0        0        0     2524 2024-05-23 14:45:07.714237 mlab_py-0.5.1/pymlab/test.py
+-rw-r--r--   0        0        0     2176 2024-05-23 14:44:59.601775 mlab_py-0.5.1/pymlab/train.py
+-rw-r--r--   0        0        0     2337 2024-05-23 07:44:20.219924 mlab_py-0.5.1/pymlab/utils.py
+-rw-r--r--   0        0        0      371 2024-05-23 19:47:29.984103 mlab_py-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0      545 1970-01-01 00:00:00.000000 mlab_py-0.5.1/PKG-INFO
```

### Comparing `mlab_py-0.5.0/pymlab/main.py` & `mlab_py-0.5.1/pymlab/main.py`

 * *Files identical despite different names*

### Comparing `mlab_py-0.5.0/pymlab/test.py` & `mlab_py-0.5.1/pymlab/test.py`

 * *Files identical despite different names*

### Comparing `mlab_py-0.5.0/pymlab/train.py` & `mlab_py-0.5.1/pymlab/train.py`

 * *Files identical despite different names*

### Comparing `mlab_py-0.5.0/pymlab/utils.py` & `mlab_py-0.5.1/pymlab/utils.py`

 * *Files identical despite different names*

### Comparing `mlab_py-0.5.0/PKG-INFO` & `mlab_py-0.5.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlab.py
-Version: 0.5.0
+Version: 0.5.1
 Summary: Python packages for mlab ecosystem
 Author: Kelvin Nketia-Achiampong
 Author-email: achiampongk22@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

