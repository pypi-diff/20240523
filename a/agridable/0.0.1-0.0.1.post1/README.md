# Comparing `tmp/agridable-0.0.1.tar.gz` & `tmp/agridable-0.0.1.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agridable-0.0.1.tar", last modified: Thu May 23 14:29:31 2024, max compression
+gzip compressed data, was "agridable-0.0.1.post1.tar", last modified: Thu May 23 15:49:04 2024, max compression
```

## Comparing `agridable-0.0.1.tar` & `agridable-0.0.1.post1.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 jameslaidler   (501) staff       (20)        0 2024-05-23 14:29:31.883586 agridable-0.0.1/
--rw-r--r--   0 jameslaidler   (501) staff       (20)    11357 2024-05-15 07:53:22.000000 agridable-0.0.1/LICENSE
--rw-r--r--   0 jameslaidler   (501) staff       (20)      578 2024-05-23 14:29:31.883310 agridable-0.0.1/PKG-INFO
-drwxr-xr-x   0 jameslaidler   (501) staff       (20)        0 2024-05-23 14:29:31.877196 agridable-0.0.1/agridable/
--rw-r--r--   0 jameslaidler   (501) staff       (20)        0 2024-05-09 15:09:48.000000 agridable-0.0.1/agridable/__init__.py
-drwxr-xr-x   0 jameslaidler   (501) staff       (20)        0 2024-05-23 14:29:31.878388 agridable-0.0.1/agridable/agridable/
--rw-r--r--   0 jameslaidler   (501) staff       (20)       33 2024-05-15 13:59:13.000000 agridable-0.0.1/agridable/agridable/__init__.py
--rw-r--r--   0 jameslaidler   (501) staff       (20)     3631 2024-05-22 15:16:14.000000 agridable-0.0.1/agridable/agridable/agridable.py
-drwxr-xr-x   0 jameslaidler   (501) staff       (20)        0 2024-05-23 14:29:31.878648 agridable-0.0.1/agridable/formats/
--rw-r--r--   0 jameslaidler   (501) staff       (20)        0 2024-05-15 14:33:12.000000 agridable-0.0.1/agridable/formats/__init__.py
--rw-r--r--   0 jameslaidler   (501) staff       (20)      395 2024-05-15 12:51:47.000000 agridable-0.0.1/agridable/formats/_base.py
-drwxr-xr-x   0 jameslaidler   (501) staff       (20)        0 2024-05-23 14:29:31.879256 agridable-0.0.1/agridable/formats/cell/
--rw-r--r--   0 jameslaidler   (501) staff       (20)       65 2024-05-15 15:55:35.000000 agridable-0.0.1/agridable/formats/cell/__init__.py
--rw-r--r--   0 jameslaidler   (501) staff       (20)      171 2024-05-16 11:46:41.000000 agridable-0.0.1/agridable/formats/cell/_base.py
--rw-r--r--   0 jameslaidler   (501) staff       (20)     1929 2024-05-22 15:19:21.000000 agridable-0.0.1/agridable/formats/cell/align.py
--rw-r--r--   0 jameslaidler   (501) staff       (20)     1504 2024-05-16 14:25:03.000000 agridable-0.0.1/agridable/formats/cell/border.py
-drwxr-xr-x   0 jameslaidler   (501) staff       (20)        0 2024-05-23 14:29:31.879924 agridable-0.0.1/agridable/formats/conditional/
--rw-r--r--   0 jameslaidler   (501) staff       (20)       92 2024-05-15 14:06:03.000000 agridable-0.0.1/agridable/formats/conditional/__init__.py
--rw-r--r--   0 jameslaidler   (501) staff       (20)      178 2024-05-16 14:26:04.000000 agridable-0.0.1/agridable/formats/conditional/_base.py
--rw-r--r--   0 jameslaidler   (501) staff       (20)     7043 2024-05-22 15:47:18.000000 agridable-0.0.1/agridable/formats/conditional/continuous_colour.py
--rw-r--r--   0 jameslaidler   (501) staff       (20)     1496 2024-05-22 15:51:32.000000 agridable-0.0.1/agridable/formats/conditional/discrete_colour.py
-drwxr-xr-x   0 jameslaidler   (501) staff       (20)        0 2024-05-23 14:29:31.880498 agridable-0.0.1/agridable/formats/grid/
--rw-r--r--   0 jameslaidler   (501) staff       (20)       46 2024-05-15 15:55:04.000000 agridable-0.0.1/agridable/formats/grid/__init__.py
--rw-r--r--   0 jameslaidler   (501) staff       (20)      171 2024-05-21 13:07:02.000000 agridable-0.0.1/agridable/formats/grid/_base.py
--rw-r--r--   0 jameslaidler   (501) staff       (20)      735 2024-05-22 15:53:39.000000 agridable-0.0.1/agridable/formats/grid/pin.py
--rw-r--r--   0 jameslaidler   (501) staff       (20)     1412 2024-05-22 15:56:47.000000 agridable-0.0.1/agridable/formats/grid/width.py
-drwxr-xr-x   0 jameslaidler   (501) staff       (20)        0 2024-05-23 14:29:31.881735 agridable-0.0.1/agridable/formats/value/
--rw-r--r--   0 jameslaidler   (501) staff       (20)      170 2024-05-15 14:00:22.000000 agridable-0.0.1/agridable/formats/value/__init__.py
--rw-r--r--   0 jameslaidler   (501) staff       (20)     1268 2024-05-15 14:34:33.000000 agridable-0.0.1/agridable/formats/value/_base.py
--rw-r--r--   0 jameslaidler   (501) staff       (20)     1536 2024-05-21 13:16:33.000000 agridable-0.0.1/agridable/formats/value/currency.py
--rw-r--r--   0 jameslaidler   (501) staff       (20)      916 2024-05-21 13:17:42.000000 agridable-0.0.1/agridable/formats/value/duration.py
--rw-r--r--   0 jameslaidler   (501) staff       (20)      222 2024-05-21 13:18:23.000000 agridable-0.0.1/agridable/formats/value/image.py
--rw-r--r--   0 jameslaidler   (501) staff       (20)     1838 2024-05-21 13:27:07.000000 agridable-0.0.1/agridable/formats/value/number.py
--rw-r--r--   0 jameslaidler   (501) staff       (20)     1315 2024-05-21 13:33:39.000000 agridable-0.0.1/agridable/formats/value/percentage.py
--rw-r--r--   0 jameslaidler   (501) staff       (20)      219 2024-05-21 13:33:54.000000 agridable-0.0.1/agridable/formats/value/url.py
-drwxr-xr-x   0 jameslaidler   (501) staff       (20)        0 2024-05-23 14:29:31.882590 agridable-0.0.1/agridable/formatters/
--rw-r--r--   0 jameslaidler   (501) staff       (20)      155 2024-05-09 15:09:48.000000 agridable-0.0.1/agridable/formatters/__init__.py
--rw-r--r--   0 jameslaidler   (501) staff       (20)      669 2024-05-09 15:09:48.000000 agridable-0.0.1/agridable/formatters/_base.py
--rw-r--r--   0 jameslaidler   (501) staff       (20)     4957 2024-05-21 13:38:18.000000 agridable-0.0.1/agridable/formatters/column_formatter.py
--rw-r--r--   0 jameslaidler   (501) staff       (20)     2290 2024-05-21 14:24:32.000000 agridable-0.0.1/agridable/formatters/conditional_column_formatter.py
--rw-r--r--   0 jameslaidler   (501) staff       (20)     1459 2024-05-22 16:46:27.000000 agridable-0.0.1/agridable/formatters/row_formatter.py
-drwxr-xr-x   0 jameslaidler   (501) staff       (20)        0 2024-05-23 14:29:31.882805 agridable-0.0.1/agridable.egg-info/
--rw-r--r--   0 jameslaidler   (501) staff       (20)      578 2024-05-23 14:29:31.000000 agridable-0.0.1/agridable.egg-info/PKG-INFO
--rw-r--r--   0 jameslaidler   (501) staff       (20)     1238 2024-05-23 14:29:31.000000 agridable-0.0.1/agridable.egg-info/SOURCES.txt
--rw-r--r--   0 jameslaidler   (501) staff       (20)        1 2024-05-23 14:29:31.000000 agridable-0.0.1/agridable.egg-info/dependency_links.txt
--rw-r--r--   0 jameslaidler   (501) staff       (20)       98 2024-05-23 14:29:31.000000 agridable-0.0.1/agridable.egg-info/requires.txt
--rw-r--r--   0 jameslaidler   (501) staff       (20)       10 2024-05-23 14:29:31.000000 agridable-0.0.1/agridable.egg-info/top_level.txt
--rw-r--r--   0 jameslaidler   (501) staff       (20)       38 2024-05-23 14:29:31.883636 agridable-0.0.1/setup.cfg
--rw-r--r--   0 jameslaidler   (501) staff       (20)      802 2024-05-23 14:26:45.000000 agridable-0.0.1/setup.py
+drwxr-xr-x   0 jameslaidler   (501) staff       (20)        0 2024-05-23 15:49:04.148532 agridable-0.0.1.post1/
+-rw-r--r--   0 jameslaidler   (501) staff       (20)    11357 2024-05-15 07:53:22.000000 agridable-0.0.1.post1/LICENSE
+-rw-r--r--   0 jameslaidler   (501) staff       (20)     1299 2024-05-23 15:49:04.148220 agridable-0.0.1.post1/PKG-INFO
+drwxr-xr-x   0 jameslaidler   (501) staff       (20)        0 2024-05-23 15:49:04.135832 agridable-0.0.1.post1/agridable/
+-rw-r--r--   0 jameslaidler   (501) staff       (20)        0 2024-05-09 15:09:48.000000 agridable-0.0.1.post1/agridable/__init__.py
+drwxr-xr-x   0 jameslaidler   (501) staff       (20)        0 2024-05-23 15:49:04.137265 agridable-0.0.1.post1/agridable/agridable/
+-rw-r--r--   0 jameslaidler   (501) staff       (20)       33 2024-05-15 13:59:13.000000 agridable-0.0.1.post1/agridable/agridable/__init__.py
+-rw-r--r--   0 jameslaidler   (501) staff       (20)     3631 2024-05-22 15:16:14.000000 agridable-0.0.1.post1/agridable/agridable/agridable.py
+drwxr-xr-x   0 jameslaidler   (501) staff       (20)        0 2024-05-23 15:49:04.137851 agridable-0.0.1.post1/agridable/formats/
+-rw-r--r--   0 jameslaidler   (501) staff       (20)        0 2024-05-15 14:33:12.000000 agridable-0.0.1.post1/agridable/formats/__init__.py
+-rw-r--r--   0 jameslaidler   (501) staff       (20)      395 2024-05-15 12:51:47.000000 agridable-0.0.1.post1/agridable/formats/_base.py
+drwxr-xr-x   0 jameslaidler   (501) staff       (20)        0 2024-05-23 15:49:04.139326 agridable-0.0.1.post1/agridable/formats/cell/
+-rw-r--r--   0 jameslaidler   (501) staff       (20)       65 2024-05-15 15:55:35.000000 agridable-0.0.1.post1/agridable/formats/cell/__init__.py
+-rw-r--r--   0 jameslaidler   (501) staff       (20)      171 2024-05-16 11:46:41.000000 agridable-0.0.1.post1/agridable/formats/cell/_base.py
+-rw-r--r--   0 jameslaidler   (501) staff       (20)     1929 2024-05-22 15:19:21.000000 agridable-0.0.1.post1/agridable/formats/cell/align.py
+-rw-r--r--   0 jameslaidler   (501) staff       (20)     1504 2024-05-16 14:25:03.000000 agridable-0.0.1.post1/agridable/formats/cell/border.py
+drwxr-xr-x   0 jameslaidler   (501) staff       (20)        0 2024-05-23 15:49:04.140910 agridable-0.0.1.post1/agridable/formats/conditional/
+-rw-r--r--   0 jameslaidler   (501) staff       (20)       92 2024-05-15 14:06:03.000000 agridable-0.0.1.post1/agridable/formats/conditional/__init__.py
+-rw-r--r--   0 jameslaidler   (501) staff       (20)      178 2024-05-16 14:26:04.000000 agridable-0.0.1.post1/agridable/formats/conditional/_base.py
+-rw-r--r--   0 jameslaidler   (501) staff       (20)     7043 2024-05-22 15:47:18.000000 agridable-0.0.1.post1/agridable/formats/conditional/continuous_colour.py
+-rw-r--r--   0 jameslaidler   (501) staff       (20)     1496 2024-05-22 15:51:32.000000 agridable-0.0.1.post1/agridable/formats/conditional/discrete_colour.py
+drwxr-xr-x   0 jameslaidler   (501) staff       (20)        0 2024-05-23 15:49:04.142485 agridable-0.0.1.post1/agridable/formats/grid/
+-rw-r--r--   0 jameslaidler   (501) staff       (20)       46 2024-05-15 15:55:04.000000 agridable-0.0.1.post1/agridable/formats/grid/__init__.py
+-rw-r--r--   0 jameslaidler   (501) staff       (20)      171 2024-05-21 13:07:02.000000 agridable-0.0.1.post1/agridable/formats/grid/_base.py
+-rw-r--r--   0 jameslaidler   (501) staff       (20)      735 2024-05-22 15:53:39.000000 agridable-0.0.1.post1/agridable/formats/grid/pin.py
+-rw-r--r--   0 jameslaidler   (501) staff       (20)     1412 2024-05-22 15:56:47.000000 agridable-0.0.1.post1/agridable/formats/grid/width.py
+drwxr-xr-x   0 jameslaidler   (501) staff       (20)        0 2024-05-23 15:49:04.145286 agridable-0.0.1.post1/agridable/formats/value/
+-rw-r--r--   0 jameslaidler   (501) staff       (20)      170 2024-05-15 14:00:22.000000 agridable-0.0.1.post1/agridable/formats/value/__init__.py
+-rw-r--r--   0 jameslaidler   (501) staff       (20)     1268 2024-05-15 14:34:33.000000 agridable-0.0.1.post1/agridable/formats/value/_base.py
+-rw-r--r--   0 jameslaidler   (501) staff       (20)     1536 2024-05-21 13:16:33.000000 agridable-0.0.1.post1/agridable/formats/value/currency.py
+-rw-r--r--   0 jameslaidler   (501) staff       (20)      916 2024-05-21 13:17:42.000000 agridable-0.0.1.post1/agridable/formats/value/duration.py
+-rw-r--r--   0 jameslaidler   (501) staff       (20)      222 2024-05-21 13:18:23.000000 agridable-0.0.1.post1/agridable/formats/value/image.py
+-rw-r--r--   0 jameslaidler   (501) staff       (20)     1838 2024-05-21 13:27:07.000000 agridable-0.0.1.post1/agridable/formats/value/number.py
+-rw-r--r--   0 jameslaidler   (501) staff       (20)     1315 2024-05-21 13:33:39.000000 agridable-0.0.1.post1/agridable/formats/value/percentage.py
+-rw-r--r--   0 jameslaidler   (501) staff       (20)      219 2024-05-21 13:33:54.000000 agridable-0.0.1.post1/agridable/formats/value/url.py
+drwxr-xr-x   0 jameslaidler   (501) staff       (20)        0 2024-05-23 15:49:04.147184 agridable-0.0.1.post1/agridable/formatters/
+-rw-r--r--   0 jameslaidler   (501) staff       (20)      155 2024-05-09 15:09:48.000000 agridable-0.0.1.post1/agridable/formatters/__init__.py
+-rw-r--r--   0 jameslaidler   (501) staff       (20)      669 2024-05-09 15:09:48.000000 agridable-0.0.1.post1/agridable/formatters/_base.py
+-rw-r--r--   0 jameslaidler   (501) staff       (20)     4957 2024-05-21 13:38:18.000000 agridable-0.0.1.post1/agridable/formatters/column_formatter.py
+-rw-r--r--   0 jameslaidler   (501) staff       (20)     2290 2024-05-21 14:24:32.000000 agridable-0.0.1.post1/agridable/formatters/conditional_column_formatter.py
+-rw-r--r--   0 jameslaidler   (501) staff       (20)     1459 2024-05-22 16:46:27.000000 agridable-0.0.1.post1/agridable/formatters/row_formatter.py
+drwxr-xr-x   0 jameslaidler   (501) staff       (20)        0 2024-05-23 15:49:04.147575 agridable-0.0.1.post1/agridable.egg-info/
+-rw-r--r--   0 jameslaidler   (501) staff       (20)     1299 2024-05-23 15:49:04.000000 agridable-0.0.1.post1/agridable.egg-info/PKG-INFO
+-rw-r--r--   0 jameslaidler   (501) staff       (20)     1238 2024-05-23 15:49:04.000000 agridable-0.0.1.post1/agridable.egg-info/SOURCES.txt
+-rw-r--r--   0 jameslaidler   (501) staff       (20)        1 2024-05-23 15:49:04.000000 agridable-0.0.1.post1/agridable.egg-info/dependency_links.txt
+-rw-r--r--   0 jameslaidler   (501) staff       (20)       98 2024-05-23 15:49:04.000000 agridable-0.0.1.post1/agridable.egg-info/requires.txt
+-rw-r--r--   0 jameslaidler   (501) staff       (20)       10 2024-05-23 15:49:04.000000 agridable-0.0.1.post1/agridable.egg-info/top_level.txt
+-rw-r--r--   0 jameslaidler   (501) staff       (20)       38 2024-05-23 15:49:04.148587 agridable-0.0.1.post1/setup.cfg
+-rw-r--r--   0 jameslaidler   (501) staff       (20)     1624 2024-05-23 15:48:51.000000 agridable-0.0.1.post1/setup.py
```

### Comparing `agridable-0.0.1/LICENSE` & `agridable-0.0.1.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `agridable-0.0.1/agridable/agridable/agridable.py` & `agridable-0.0.1.post1/agridable/agridable/agridable.py`

 * *Files identical despite different names*

### Comparing `agridable-0.0.1/agridable/formats/cell/align.py` & `agridable-0.0.1.post1/agridable/formats/cell/align.py`

 * *Files identical despite different names*

### Comparing `agridable-0.0.1/agridable/formats/cell/border.py` & `agridable-0.0.1.post1/agridable/formats/cell/border.py`

 * *Files identical despite different names*

### Comparing `agridable-0.0.1/agridable/formats/conditional/continuous_colour.py` & `agridable-0.0.1.post1/agridable/formats/conditional/continuous_colour.py`

 * *Files identical despite different names*

### Comparing `agridable-0.0.1/agridable/formats/conditional/discrete_colour.py` & `agridable-0.0.1.post1/agridable/formats/conditional/discrete_colour.py`

 * *Files identical despite different names*

### Comparing `agridable-0.0.1/agridable/formats/grid/pin.py` & `agridable-0.0.1.post1/agridable/formats/grid/pin.py`

 * *Files identical despite different names*

### Comparing `agridable-0.0.1/agridable/formats/grid/width.py` & `agridable-0.0.1.post1/agridable/formats/grid/width.py`

 * *Files identical despite different names*

### Comparing `agridable-0.0.1/agridable/formats/value/_base.py` & `agridable-0.0.1.post1/agridable/formats/value/_base.py`

 * *Files identical despite different names*

### Comparing `agridable-0.0.1/agridable/formats/value/currency.py` & `agridable-0.0.1.post1/agridable/formats/value/currency.py`

 * *Files identical despite different names*

### Comparing `agridable-0.0.1/agridable/formats/value/duration.py` & `agridable-0.0.1.post1/agridable/formats/value/duration.py`

 * *Files identical despite different names*

### Comparing `agridable-0.0.1/agridable/formats/value/number.py` & `agridable-0.0.1.post1/agridable/formats/value/number.py`

 * *Files identical despite different names*

### Comparing `agridable-0.0.1/agridable/formats/value/percentage.py` & `agridable-0.0.1.post1/agridable/formats/value/percentage.py`

 * *Files identical despite different names*

### Comparing `agridable-0.0.1/agridable/formatters/_base.py` & `agridable-0.0.1.post1/agridable/formatters/_base.py`

 * *Files identical despite different names*

### Comparing `agridable-0.0.1/agridable/formatters/column_formatter.py` & `agridable-0.0.1.post1/agridable/formatters/column_formatter.py`

 * *Files identical despite different names*

### Comparing `agridable-0.0.1/agridable/formatters/conditional_column_formatter.py` & `agridable-0.0.1.post1/agridable/formatters/conditional_column_formatter.py`

 * *Files identical despite different names*

### Comparing `agridable-0.0.1/agridable/formatters/row_formatter.py` & `agridable-0.0.1.post1/agridable/formatters/row_formatter.py`

 * *Files identical despite different names*

### Comparing `agridable-0.0.1/agridable.egg-info/SOURCES.txt` & `agridable-0.0.1.post1/agridable.egg-info/SOURCES.txt`

 * *Files identical despite different names*

