# Comparing `tmp/covjsonkit-0.0.8.tar.gz` & `tmp/covjsonkit-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "covjsonkit-0.0.8.tar", last modified: Thu May 23 14:32:01 2024, max compression
+gzip compressed data, was "covjsonkit-0.0.9.tar", last modified: Thu May 23 14:55:01 2024, max compression
```

## Comparing `covjsonkit-0.0.8.tar` & `covjsonkit-0.0.9.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:32:01.192847 covjsonkit-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)    11379 2024-05-23 14:31:50.000000 covjsonkit-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-23 14:32:01.192847 covjsonkit-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-23 14:31:50.000000 covjsonkit-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:32:01.188847 covjsonkit-0.0.8/covjsonkit/
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-23 14:31:50.000000 covjsonkit-0.0.8/covjsonkit/Coverage.py
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-23 14:31:50.000000 covjsonkit-0.0.8/covjsonkit/CoverageCollection.py
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-23 14:31:50.000000 covjsonkit-0.0.8/covjsonkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-05-23 14:31:50.000000 covjsonkit-0.0.8/covjsonkit/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:32:01.188847 covjsonkit-0.0.8/covjsonkit/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 14:31:50.000000 covjsonkit-0.0.8/covjsonkit/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:32:01.192847 covjsonkit-0.0.8/covjsonkit/decoder/
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-05-23 14:31:50.000000 covjsonkit-0.0.8/covjsonkit/decoder/BoundingBox.py
--rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-05-23 14:31:50.000000 covjsonkit-0.0.8/covjsonkit/decoder/Frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-05-23 14:31:50.000000 covjsonkit-0.0.8/covjsonkit/decoder/Path.py
--rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-05-23 14:31:50.000000 covjsonkit-0.0.8/covjsonkit/decoder/Shapefile.py
--rw-r--r--   0 runner    (1001) docker     (127)     3603 2024-05-23 14:31:50.000000 covjsonkit-0.0.8/covjsonkit/decoder/TimeSeries.py
--rw-r--r--   0 runner    (1001) docker     (127)     3373 2024-05-23 14:31:50.000000 covjsonkit-0.0.8/covjsonkit/decoder/VerticalProfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-05-23 14:31:50.000000 covjsonkit-0.0.8/covjsonkit/decoder/Wkt.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 14:31:50.000000 covjsonkit-0.0.8/covjsonkit/decoder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-05-23 14:31:50.000000 covjsonkit-0.0.8/covjsonkit/decoder/decoder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:32:01.192847 covjsonkit-0.0.8/covjsonkit/encoder/
--rw-r--r--   0 runner    (1001) docker     (127)     4941 2024-05-23 14:31:50.000000 covjsonkit-0.0.8/covjsonkit/encoder/BoundingBox.py
--rw-r--r--   0 runner    (1001) docker     (127)     4935 2024-05-23 14:31:50.000000 covjsonkit-0.0.8/covjsonkit/encoder/Frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     4737 2024-05-23 14:31:50.000000 covjsonkit-0.0.8/covjsonkit/encoder/Path.py
--rw-r--r--   0 runner    (1001) docker     (127)     4939 2024-05-23 14:31:50.000000 covjsonkit-0.0.8/covjsonkit/encoder/Shapefile.py
--rw-r--r--   0 runner    (1001) docker     (127)     6204 2024-05-23 14:31:50.000000 covjsonkit-0.0.8/covjsonkit/encoder/TimeSeries.py
--rw-r--r--   0 runner    (1001) docker     (127)     5800 2024-05-23 14:31:50.000000 covjsonkit-0.0.8/covjsonkit/encoder/VerticalProfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     4933 2024-05-23 14:31:50.000000 covjsonkit-0.0.8/covjsonkit/encoder/Wkt.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 14:31:50.000000 covjsonkit-0.0.8/covjsonkit/encoder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3843 2024-05-23 14:31:50.000000 covjsonkit-0.0.8/covjsonkit/encoder/encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-05-23 14:31:50.000000 covjsonkit-0.0.8/covjsonkit/param_db.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-23 14:31:50.000000 covjsonkit-0.0.8/covjsonkit/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:32:01.188847 covjsonkit-0.0.8/covjsonkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-23 14:32:00.000000 covjsonkit-0.0.8/covjsonkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-05-23 14:32:01.000000 covjsonkit-0.0.8/covjsonkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 14:32:00.000000 covjsonkit-0.0.8/covjsonkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 14:32:00.000000 covjsonkit-0.0.8/covjsonkit.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-23 14:32:00.000000 covjsonkit-0.0.8/covjsonkit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-23 14:31:50.000000 covjsonkit-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 14:32:01.192847 covjsonkit-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-23 14:31:50.000000 covjsonkit-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:55:01.913174 covjsonkit-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11379 2024-05-23 14:54:51.000000 covjsonkit-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-23 14:55:01.913174 covjsonkit-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-23 14:54:51.000000 covjsonkit-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:55:01.909174 covjsonkit-0.0.9/covjsonkit/
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-23 14:54:51.000000 covjsonkit-0.0.9/covjsonkit/Coverage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-23 14:54:51.000000 covjsonkit-0.0.9/covjsonkit/CoverageCollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-23 14:54:51.000000 covjsonkit-0.0.9/covjsonkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-05-23 14:54:51.000000 covjsonkit-0.0.9/covjsonkit/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:55:01.909174 covjsonkit-0.0.9/covjsonkit/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 14:54:51.000000 covjsonkit-0.0.9/covjsonkit/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:55:01.913174 covjsonkit-0.0.9/covjsonkit/decoder/
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-05-23 14:54:51.000000 covjsonkit-0.0.9/covjsonkit/decoder/BoundingBox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-05-23 14:54:51.000000 covjsonkit-0.0.9/covjsonkit/decoder/Frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-05-23 14:54:51.000000 covjsonkit-0.0.9/covjsonkit/decoder/Path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-05-23 14:54:51.000000 covjsonkit-0.0.9/covjsonkit/decoder/Shapefile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3603 2024-05-23 14:54:51.000000 covjsonkit-0.0.9/covjsonkit/decoder/TimeSeries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3373 2024-05-23 14:54:51.000000 covjsonkit-0.0.9/covjsonkit/decoder/VerticalProfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-05-23 14:54:51.000000 covjsonkit-0.0.9/covjsonkit/decoder/Wkt.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 14:54:51.000000 covjsonkit-0.0.9/covjsonkit/decoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-05-23 14:54:51.000000 covjsonkit-0.0.9/covjsonkit/decoder/decoder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:55:01.913174 covjsonkit-0.0.9/covjsonkit/encoder/
+-rw-r--r--   0 runner    (1001) docker     (127)     4941 2024-05-23 14:54:51.000000 covjsonkit-0.0.9/covjsonkit/encoder/BoundingBox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4935 2024-05-23 14:54:51.000000 covjsonkit-0.0.9/covjsonkit/encoder/Frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4737 2024-05-23 14:54:51.000000 covjsonkit-0.0.9/covjsonkit/encoder/Path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4939 2024-05-23 14:54:51.000000 covjsonkit-0.0.9/covjsonkit/encoder/Shapefile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6204 2024-05-23 14:54:51.000000 covjsonkit-0.0.9/covjsonkit/encoder/TimeSeries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5800 2024-05-23 14:54:51.000000 covjsonkit-0.0.9/covjsonkit/encoder/VerticalProfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4933 2024-05-23 14:54:51.000000 covjsonkit-0.0.9/covjsonkit/encoder/Wkt.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 14:54:51.000000 covjsonkit-0.0.9/covjsonkit/encoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3843 2024-05-23 14:54:51.000000 covjsonkit-0.0.9/covjsonkit/encoder/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-05-23 14:54:51.000000 covjsonkit-0.0.9/covjsonkit/param_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-23 14:54:51.000000 covjsonkit-0.0.9/covjsonkit/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:55:01.909174 covjsonkit-0.0.9/covjsonkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-23 14:55:01.000000 covjsonkit-0.0.9/covjsonkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-05-23 14:55:01.000000 covjsonkit-0.0.9/covjsonkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 14:55:01.000000 covjsonkit-0.0.9/covjsonkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 14:55:01.000000 covjsonkit-0.0.9/covjsonkit.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-23 14:55:01.000000 covjsonkit-0.0.9/covjsonkit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-23 14:54:51.000000 covjsonkit-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 14:55:01.913174 covjsonkit-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-23 14:54:51.000000 covjsonkit-0.0.9/setup.py
```

### Comparing `covjsonkit-0.0.8/LICENSE` & `covjsonkit-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `covjsonkit-0.0.8/README.md` & `covjsonkit-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `covjsonkit-0.0.8/covjsonkit/api.py` & `covjsonkit-0.0.9/covjsonkit/api.py`

 * *Files identical despite different names*

### Comparing `covjsonkit-0.0.8/covjsonkit/decoder/BoundingBox.py` & `covjsonkit-0.0.9/covjsonkit/decoder/BoundingBox.py`

 * *Files identical despite different names*

### Comparing `covjsonkit-0.0.8/covjsonkit/decoder/Frame.py` & `covjsonkit-0.0.9/covjsonkit/decoder/Frame.py`

 * *Files identical despite different names*

### Comparing `covjsonkit-0.0.8/covjsonkit/decoder/Path.py` & `covjsonkit-0.0.9/covjsonkit/decoder/Path.py`

 * *Files identical despite different names*

### Comparing `covjsonkit-0.0.8/covjsonkit/decoder/Shapefile.py` & `covjsonkit-0.0.9/covjsonkit/decoder/Shapefile.py`

 * *Files identical despite different names*

### Comparing `covjsonkit-0.0.8/covjsonkit/decoder/TimeSeries.py` & `covjsonkit-0.0.9/covjsonkit/decoder/TimeSeries.py`

 * *Files identical despite different names*

### Comparing `covjsonkit-0.0.8/covjsonkit/decoder/VerticalProfile.py` & `covjsonkit-0.0.9/covjsonkit/decoder/VerticalProfile.py`

 * *Files identical despite different names*

### Comparing `covjsonkit-0.0.8/covjsonkit/decoder/Wkt.py` & `covjsonkit-0.0.9/covjsonkit/decoder/Wkt.py`

 * *Files identical despite different names*

### Comparing `covjsonkit-0.0.8/covjsonkit/decoder/decoder.py` & `covjsonkit-0.0.9/covjsonkit/decoder/decoder.py`

 * *Files identical despite different names*

### Comparing `covjsonkit-0.0.8/covjsonkit/encoder/BoundingBox.py` & `covjsonkit-0.0.9/covjsonkit/encoder/BoundingBox.py`

 * *Files identical despite different names*

### Comparing `covjsonkit-0.0.8/covjsonkit/encoder/Frame.py` & `covjsonkit-0.0.9/covjsonkit/encoder/Frame.py`

 * *Files identical despite different names*

### Comparing `covjsonkit-0.0.8/covjsonkit/encoder/Path.py` & `covjsonkit-0.0.9/covjsonkit/encoder/Path.py`

 * *Files identical despite different names*

### Comparing `covjsonkit-0.0.8/covjsonkit/encoder/Shapefile.py` & `covjsonkit-0.0.9/covjsonkit/encoder/Shapefile.py`

 * *Files identical despite different names*

### Comparing `covjsonkit-0.0.8/covjsonkit/encoder/TimeSeries.py` & `covjsonkit-0.0.9/covjsonkit/encoder/TimeSeries.py`

 * *Files identical despite different names*

### Comparing `covjsonkit-0.0.8/covjsonkit/encoder/VerticalProfile.py` & `covjsonkit-0.0.9/covjsonkit/encoder/VerticalProfile.py`

 * *Files identical despite different names*

### Comparing `covjsonkit-0.0.8/covjsonkit/encoder/Wkt.py` & `covjsonkit-0.0.9/covjsonkit/encoder/Wkt.py`

 * *Files identical despite different names*

### Comparing `covjsonkit-0.0.8/covjsonkit/encoder/encoder.py` & `covjsonkit-0.0.9/covjsonkit/encoder/encoder.py`

 * *Files identical despite different names*

### Comparing `covjsonkit-0.0.8/covjsonkit/param_db.py` & `covjsonkit-0.0.9/covjsonkit/param_db.py`

 * *Files identical despite different names*

### Comparing `covjsonkit-0.0.8/covjsonkit.egg-info/SOURCES.txt` & `covjsonkit-0.0.9/covjsonkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

