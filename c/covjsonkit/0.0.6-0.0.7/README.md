# Comparing `tmp/covjsonkit-0.0.6.tar.gz` & `tmp/covjsonkit-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "covjsonkit-0.0.6.tar", last modified: Thu May 23 07:40:24 2024, max compression
+gzip compressed data, was "covjsonkit-0.0.7.tar", last modified: Thu May 23 14:03:54 2024, max compression
```

## Comparing `covjsonkit-0.0.6.tar` & `covjsonkit-0.0.7.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:40:24.809061 covjsonkit-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)    11379 2024-05-23 07:40:13.000000 covjsonkit-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-23 07:40:24.809061 covjsonkit-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-23 07:40:13.000000 covjsonkit-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:40:24.805061 covjsonkit-0.0.6/covjsonkit/
--rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-23 07:40:13.000000 covjsonkit-0.0.6/covjsonkit/Coverage.py
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-23 07:40:13.000000 covjsonkit-0.0.6/covjsonkit/CoverageCollection.py
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-23 07:40:13.000000 covjsonkit-0.0.6/covjsonkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-05-23 07:40:13.000000 covjsonkit-0.0.6/covjsonkit/api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:40:24.805061 covjsonkit-0.0.6/covjsonkit/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 07:40:13.000000 covjsonkit-0.0.6/covjsonkit/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:40:24.809061 covjsonkit-0.0.6/covjsonkit/decoder/
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-05-23 07:40:13.000000 covjsonkit-0.0.6/covjsonkit/decoder/BoundingBox.py
--rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-05-23 07:40:13.000000 covjsonkit-0.0.6/covjsonkit/decoder/Frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-05-23 07:40:13.000000 covjsonkit-0.0.6/covjsonkit/decoder/Path.py
--rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-05-23 07:40:13.000000 covjsonkit-0.0.6/covjsonkit/decoder/Shapefile.py
--rw-r--r--   0 runner    (1001) docker     (127)     3603 2024-05-23 07:40:13.000000 covjsonkit-0.0.6/covjsonkit/decoder/TimeSeries.py
--rw-r--r--   0 runner    (1001) docker     (127)     3373 2024-05-23 07:40:13.000000 covjsonkit-0.0.6/covjsonkit/decoder/VerticalProfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-05-23 07:40:13.000000 covjsonkit-0.0.6/covjsonkit/decoder/Wkt.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 07:40:13.000000 covjsonkit-0.0.6/covjsonkit/decoder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-05-23 07:40:13.000000 covjsonkit-0.0.6/covjsonkit/decoder/decoder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:40:24.809061 covjsonkit-0.0.6/covjsonkit/encoder/
--rw-r--r--   0 runner    (1001) docker     (127)     4941 2024-05-23 07:40:13.000000 covjsonkit-0.0.6/covjsonkit/encoder/BoundingBox.py
--rw-r--r--   0 runner    (1001) docker     (127)     4935 2024-05-23 07:40:13.000000 covjsonkit-0.0.6/covjsonkit/encoder/Frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     4737 2024-05-23 07:40:13.000000 covjsonkit-0.0.6/covjsonkit/encoder/Path.py
--rw-r--r--   0 runner    (1001) docker     (127)     4939 2024-05-23 07:40:13.000000 covjsonkit-0.0.6/covjsonkit/encoder/Shapefile.py
--rw-r--r--   0 runner    (1001) docker     (127)     6204 2024-05-23 07:40:13.000000 covjsonkit-0.0.6/covjsonkit/encoder/TimeSeries.py
--rw-r--r--   0 runner    (1001) docker     (127)     5800 2024-05-23 07:40:13.000000 covjsonkit-0.0.6/covjsonkit/encoder/VerticalProfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     4933 2024-05-23 07:40:13.000000 covjsonkit-0.0.6/covjsonkit/encoder/Wkt.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 07:40:13.000000 covjsonkit-0.0.6/covjsonkit/encoder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3905 2024-05-23 07:40:13.000000 covjsonkit-0.0.6/covjsonkit/encoder/encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-05-23 07:40:13.000000 covjsonkit-0.0.6/covjsonkit/param_db.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-23 07:40:13.000000 covjsonkit-0.0.6/covjsonkit/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:40:24.805061 covjsonkit-0.0.6/covjsonkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-23 07:40:24.000000 covjsonkit-0.0.6/covjsonkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-05-23 07:40:24.000000 covjsonkit-0.0.6/covjsonkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 07:40:24.000000 covjsonkit-0.0.6/covjsonkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 07:40:24.000000 covjsonkit-0.0.6/covjsonkit.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-23 07:40:24.000000 covjsonkit-0.0.6/covjsonkit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-23 07:40:13.000000 covjsonkit-0.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 07:40:24.809061 covjsonkit-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-23 07:40:13.000000 covjsonkit-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:03:54.024509 covjsonkit-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    11379 2024-05-23 14:03:45.000000 covjsonkit-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-23 14:03:54.024509 covjsonkit-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-23 14:03:45.000000 covjsonkit-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:03:54.020509 covjsonkit-0.0.7/covjsonkit/
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-23 14:03:45.000000 covjsonkit-0.0.7/covjsonkit/Coverage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-23 14:03:45.000000 covjsonkit-0.0.7/covjsonkit/CoverageCollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-23 14:03:45.000000 covjsonkit-0.0.7/covjsonkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-05-23 14:03:45.000000 covjsonkit-0.0.7/covjsonkit/api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:03:54.020509 covjsonkit-0.0.7/covjsonkit/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 14:03:45.000000 covjsonkit-0.0.7/covjsonkit/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:03:54.020509 covjsonkit-0.0.7/covjsonkit/decoder/
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-05-23 14:03:45.000000 covjsonkit-0.0.7/covjsonkit/decoder/BoundingBox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-05-23 14:03:45.000000 covjsonkit-0.0.7/covjsonkit/decoder/Frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-05-23 14:03:45.000000 covjsonkit-0.0.7/covjsonkit/decoder/Path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-05-23 14:03:45.000000 covjsonkit-0.0.7/covjsonkit/decoder/Shapefile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3603 2024-05-23 14:03:45.000000 covjsonkit-0.0.7/covjsonkit/decoder/TimeSeries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3373 2024-05-23 14:03:45.000000 covjsonkit-0.0.7/covjsonkit/decoder/VerticalProfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-05-23 14:03:45.000000 covjsonkit-0.0.7/covjsonkit/decoder/Wkt.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 14:03:45.000000 covjsonkit-0.0.7/covjsonkit/decoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-05-23 14:03:45.000000 covjsonkit-0.0.7/covjsonkit/decoder/decoder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:03:54.024509 covjsonkit-0.0.7/covjsonkit/encoder/
+-rw-r--r--   0 runner    (1001) docker     (127)     4941 2024-05-23 14:03:45.000000 covjsonkit-0.0.7/covjsonkit/encoder/BoundingBox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4935 2024-05-23 14:03:45.000000 covjsonkit-0.0.7/covjsonkit/encoder/Frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4737 2024-05-23 14:03:45.000000 covjsonkit-0.0.7/covjsonkit/encoder/Path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4939 2024-05-23 14:03:45.000000 covjsonkit-0.0.7/covjsonkit/encoder/Shapefile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6204 2024-05-23 14:03:45.000000 covjsonkit-0.0.7/covjsonkit/encoder/TimeSeries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5800 2024-05-23 14:03:45.000000 covjsonkit-0.0.7/covjsonkit/encoder/VerticalProfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4933 2024-05-23 14:03:45.000000 covjsonkit-0.0.7/covjsonkit/encoder/Wkt.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 14:03:45.000000 covjsonkit-0.0.7/covjsonkit/encoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3843 2024-05-23 14:03:45.000000 covjsonkit-0.0.7/covjsonkit/encoder/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-05-23 14:03:45.000000 covjsonkit-0.0.7/covjsonkit/param_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-23 14:03:45.000000 covjsonkit-0.0.7/covjsonkit/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:03:54.020509 covjsonkit-0.0.7/covjsonkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-23 14:03:53.000000 covjsonkit-0.0.7/covjsonkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-05-23 14:03:53.000000 covjsonkit-0.0.7/covjsonkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 14:03:53.000000 covjsonkit-0.0.7/covjsonkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 14:03:53.000000 covjsonkit-0.0.7/covjsonkit.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-23 14:03:53.000000 covjsonkit-0.0.7/covjsonkit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-23 14:03:45.000000 covjsonkit-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 14:03:54.024509 covjsonkit-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-23 14:03:45.000000 covjsonkit-0.0.7/setup.py
```

### Comparing `covjsonkit-0.0.6/LICENSE` & `covjsonkit-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `covjsonkit-0.0.6/README.md` & `covjsonkit-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `covjsonkit-0.0.6/covjsonkit/api.py` & `covjsonkit-0.0.7/covjsonkit/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     "shapefile": covjsonkit.decoder.Shapefile.Shapefile,
     "frame": covjsonkit.decoder.Frame.Frame,
     "path": covjsonkit.decoder.Path.Path,
     "wkt": covjsonkit.decoder.Wkt.Wkt,
 }
 
 
-class Eccovjson:
+class Covjsonkit:
     def __init__(self):
         pass
 
     def encode(self, type, domaintype):
         if domaintype == "timeseries":
             domaintype = "PointSeries"
         elif domaintype == "trajectory":
```

### Comparing `covjsonkit-0.0.6/covjsonkit/decoder/BoundingBox.py` & `covjsonkit-0.0.7/covjsonkit/decoder/BoundingBox.py`

 * *Files identical despite different names*

### Comparing `covjsonkit-0.0.6/covjsonkit/decoder/Frame.py` & `covjsonkit-0.0.7/covjsonkit/decoder/Frame.py`

 * *Files identical despite different names*

### Comparing `covjsonkit-0.0.6/covjsonkit/decoder/Path.py` & `covjsonkit-0.0.7/covjsonkit/decoder/Path.py`

 * *Files identical despite different names*

### Comparing `covjsonkit-0.0.6/covjsonkit/decoder/Shapefile.py` & `covjsonkit-0.0.7/covjsonkit/decoder/Shapefile.py`

 * *Files identical despite different names*

### Comparing `covjsonkit-0.0.6/covjsonkit/decoder/TimeSeries.py` & `covjsonkit-0.0.7/covjsonkit/decoder/TimeSeries.py`

 * *Files identical despite different names*

### Comparing `covjsonkit-0.0.6/covjsonkit/decoder/VerticalProfile.py` & `covjsonkit-0.0.7/covjsonkit/decoder/VerticalProfile.py`

 * *Files identical despite different names*

### Comparing `covjsonkit-0.0.6/covjsonkit/decoder/Wkt.py` & `covjsonkit-0.0.7/covjsonkit/decoder/Wkt.py`

 * *Files identical despite different names*

### Comparing `covjsonkit-0.0.6/covjsonkit/decoder/decoder.py` & `covjsonkit-0.0.7/covjsonkit/decoder/decoder.py`

 * *Files identical despite different names*

### Comparing `covjsonkit-0.0.6/covjsonkit/encoder/BoundingBox.py` & `covjsonkit-0.0.7/covjsonkit/encoder/BoundingBox.py`

 * *Files identical despite different names*

### Comparing `covjsonkit-0.0.6/covjsonkit/encoder/Frame.py` & `covjsonkit-0.0.7/covjsonkit/encoder/Frame.py`

 * *Files identical despite different names*

### Comparing `covjsonkit-0.0.6/covjsonkit/encoder/Path.py` & `covjsonkit-0.0.7/covjsonkit/encoder/Path.py`

 * *Files identical despite different names*

### Comparing `covjsonkit-0.0.6/covjsonkit/encoder/Shapefile.py` & `covjsonkit-0.0.7/covjsonkit/encoder/Shapefile.py`

 * *Files identical despite different names*

### Comparing `covjsonkit-0.0.6/covjsonkit/encoder/TimeSeries.py` & `covjsonkit-0.0.7/covjsonkit/encoder/TimeSeries.py`

 * *Files identical despite different names*

### Comparing `covjsonkit-0.0.6/covjsonkit/encoder/VerticalProfile.py` & `covjsonkit-0.0.7/covjsonkit/encoder/VerticalProfile.py`

 * *Files identical despite different names*

### Comparing `covjsonkit-0.0.6/covjsonkit/encoder/Wkt.py` & `covjsonkit-0.0.7/covjsonkit/encoder/Wkt.py`

 * *Files identical despite different names*

### Comparing `covjsonkit-0.0.6/covjsonkit/encoder/encoder.py` & `covjsonkit-0.0.7/covjsonkit/encoder/encoder.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from abc import ABC, abstractmethod
 
 from covjson_pydantic.coverage import CoverageCollection
 from covjson_pydantic.domain import DomainType
 from covjson_pydantic.parameter import Parameter
 from covjson_pydantic.reference_system import ReferenceSystemConnectionObject
 
-# from eccovjson.CoverageCollection import CoverageCollection
 from covjsonkit.param_db import get_param_from_db, get_unit_from_db
 
 
 class Encoder(ABC):
     def __init__(self, type, domaintype):
         self.covjson = {}
```

### Comparing `covjsonkit-0.0.6/covjsonkit/param_db.py` & `covjsonkit-0.0.7/covjsonkit/param_db.py`

 * *Files identical despite different names*

### Comparing `covjsonkit-0.0.6/covjsonkit.egg-info/SOURCES.txt` & `covjsonkit-0.0.7/covjsonkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `covjsonkit-0.0.6/setup.py` & `covjsonkit-0.0.7/setup.py`

 * *Files identical despite different names*

