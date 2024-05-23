# Comparing `tmp/aeroterra_ds-1.1.7.tar.gz` & `tmp/aeroterra_ds-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aeroterra_ds-1.1.7.tar", last modified: Thu May 23 19:25:41 2024, max compression
+gzip compressed data, was "aeroterra_ds-1.1.8.tar", last modified: Thu May 23 19:28:52 2024, max compression
```

## Comparing `aeroterra_ds-1.1.7.tar` & `aeroterra_ds-1.1.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 19:25:41.502490 aeroterra_ds-1.1.7/
--rw-rw-rw-   0        0        0     1325 2024-05-23 19:25:41.501162 aeroterra_ds-1.1.7/PKG-INFO
--rw-rw-rw-   0        0        0      854 2024-05-23 18:46:51.000000 aeroterra_ds-1.1.7/README.md
--rw-rw-rw-   0        0        0       42 2024-05-23 19:25:41.502490 aeroterra_ds-1.1.7/setup.cfg
--rw-rw-rw-   0        0        0      888 2024-05-23 19:25:35.000000 aeroterra_ds-1.1.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-23 19:25:41.481379 aeroterra_ds-1.1.7/src/
-drwxrwxrwx   0        0        0        0 2024-05-23 19:25:41.487703 aeroterra_ds-1.1.7/src/aeroterra_ds.egg-info/
--rw-rw-rw-   0        0        0     1325 2024-05-23 19:25:41.000000 aeroterra_ds-1.1.7/src/aeroterra_ds.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      453 2024-05-23 19:25:41.000000 aeroterra_ds-1.1.7/src/aeroterra_ds.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 19:25:41.000000 aeroterra_ds-1.1.7/src/aeroterra_ds.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2024-05-23 19:25:41.000000 aeroterra_ds-1.1.7/src/aeroterra_ds.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-05-23 19:25:41.000000 aeroterra_ds-1.1.7/src/aeroterra_ds.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-23 19:25:41.489711 aeroterra_ds-1.1.7/src/geometry/
--rw-rw-rw-   0        0        0       53 2024-04-19 19:51:19.000000 aeroterra_ds-1.1.7/src/geometry/__init__.py
--rw-rw-rw-   0        0        0     4193 2024-04-22 20:53:00.000000 aeroterra_ds-1.1.7/src/geometry/change_crs.py
--rw-rw-rw-   0        0        0     5752 2024-04-19 19:51:29.000000 aeroterra_ds-1.1.7/src/geometry/geometry.py
-drwxrwxrwx   0        0        0        0 2024-05-23 19:25:41.500181 aeroterra_ds-1.1.7/src/layers/
--rw-rw-rw-   0        0        0       53 2024-04-19 18:38:17.000000 aeroterra_ds-1.1.7/src/layers/__init__.py
--rw-rw-rw-   0        0        0     1720 2024-04-29 14:04:32.000000 aeroterra_ds-1.1.7/src/layers/common.py
--rw-rw-rw-   0        0        0      466 2024-04-18 20:25:50.000000 aeroterra_ds-1.1.7/src/layers/constants.py
--rw-rw-rw-   0        0        0     5510 2024-05-23 18:49:59.000000 aeroterra_ds-1.1.7/src/layers/fields.py
--rw-rw-rw-   0        0        0    15183 2024-05-23 19:25:30.000000 aeroterra_ds-1.1.7/src/layers/layers.py
--rw-rw-rw-   0        0        0     6691 2024-04-29 14:04:39.000000 aeroterra_ds-1.1.7/src/layers/properties.py
--rw-rw-rw-   0        0        0     2323 2024-04-18 20:36:51.000000 aeroterra_ds-1.1.7/src/layers/symbology.py
+drwxrwxrwx   0        0        0        0 2024-05-23 19:28:52.501031 aeroterra_ds-1.1.8/
+-rw-rw-rw-   0        0        0     1325 2024-05-23 19:28:52.500031 aeroterra_ds-1.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0      854 2024-05-23 18:46:51.000000 aeroterra_ds-1.1.8/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-23 19:28:52.501031 aeroterra_ds-1.1.8/setup.cfg
+-rw-rw-rw-   0        0        0      888 2024-05-23 19:28:47.000000 aeroterra_ds-1.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 19:28:52.476565 aeroterra_ds-1.1.8/src/
+drwxrwxrwx   0        0        0        0 2024-05-23 19:28:52.485922 aeroterra_ds-1.1.8/src/aeroterra_ds.egg-info/
+-rw-rw-rw-   0        0        0     1325 2024-05-23 19:28:52.000000 aeroterra_ds-1.1.8/src/aeroterra_ds.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      453 2024-05-23 19:28:52.000000 aeroterra_ds-1.1.8/src/aeroterra_ds.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 19:28:52.000000 aeroterra_ds-1.1.8/src/aeroterra_ds.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2024-05-23 19:28:52.000000 aeroterra_ds-1.1.8/src/aeroterra_ds.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-23 19:28:52.000000 aeroterra_ds-1.1.8/src/aeroterra_ds.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-23 19:28:52.489939 aeroterra_ds-1.1.8/src/geometry/
+-rw-rw-rw-   0        0        0       53 2024-04-19 19:51:19.000000 aeroterra_ds-1.1.8/src/geometry/__init__.py
+-rw-rw-rw-   0        0        0     4267 2024-05-23 19:28:06.000000 aeroterra_ds-1.1.8/src/geometry/change_crs.py
+-rw-rw-rw-   0        0        0     5752 2024-04-19 19:51:29.000000 aeroterra_ds-1.1.8/src/geometry/geometry.py
+drwxrwxrwx   0        0        0        0 2024-05-23 19:28:52.498042 aeroterra_ds-1.1.8/src/layers/
+-rw-rw-rw-   0        0        0       53 2024-04-19 18:38:17.000000 aeroterra_ds-1.1.8/src/layers/__init__.py
+-rw-rw-rw-   0        0        0     1720 2024-04-29 14:04:32.000000 aeroterra_ds-1.1.8/src/layers/common.py
+-rw-rw-rw-   0        0        0      466 2024-04-18 20:25:50.000000 aeroterra_ds-1.1.8/src/layers/constants.py
+-rw-rw-rw-   0        0        0     5510 2024-05-23 18:49:59.000000 aeroterra_ds-1.1.8/src/layers/fields.py
+-rw-rw-rw-   0        0        0    15183 2024-05-23 19:25:30.000000 aeroterra_ds-1.1.8/src/layers/layers.py
+-rw-rw-rw-   0        0        0     6691 2024-04-29 14:04:39.000000 aeroterra_ds-1.1.8/src/layers/properties.py
+-rw-rw-rw-   0        0        0     2323 2024-04-18 20:36:51.000000 aeroterra_ds-1.1.8/src/layers/symbology.py
```

### Comparing `aeroterra_ds-1.1.7/PKG-INFO` & `aeroterra_ds-1.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aeroterra_ds
-Version: 1.1.7
+Version: 1.1.8
 Summary: Python Functions To Work With GeoSpatial Data & ArcGis in a simpler way
 Home-page: https://example.com
 Author: Data Science
 Author-email: aeroterra_ds@aeroterra.com
 Keywords: arcgis
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `aeroterra_ds-1.1.7/README.md` & `aeroterra_ds-1.1.8/README.md`

 * *Files identical despite different names*

### Comparing `aeroterra_ds-1.1.7/setup.py` & `aeroterra_ds-1.1.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='aeroterra_ds',
-    version='1.1.7',
+    version='1.1.8',
     author='Data Science',
     author_email='aeroterra_ds@aeroterra.com',
     description='Python Functions To Work With GeoSpatial Data & ArcGis in a simpler way',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://example.com',
     package_dir={'': "src"},
```

### Comparing `aeroterra_ds-1.1.7/src/aeroterra_ds.egg-info/PKG-INFO` & `aeroterra_ds-1.1.8/src/aeroterra_ds.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aeroterra-ds
-Version: 1.1.7
+Version: 1.1.8
 Summary: Python Functions To Work With GeoSpatial Data & ArcGis in a simpler way
 Home-page: https://example.com
 Author: Data Science
 Author-email: aeroterra_ds@aeroterra.com
 Keywords: arcgis
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `aeroterra_ds-1.1.7/src/geometry/change_crs.py` & `aeroterra_ds-1.1.8/src/geometry/change_crs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 import pyproj
 from shapely.geometry import Point, MultiPoint, LineString, MultiLineString, Polygon, MultiPolygon
+from shapely.ops import unary_union
+
+from pandas import DataFrame
 
 def change_crs_polygon(polygon, crs_fuente, crs_final):
     src_origen = pyproj.CRS(crs_fuente)
     src_destino = pyproj.CRS(crs_final)
     transformador = pyproj.Transformer.from_crs(src_origen, src_destino, always_xy=True)
 
-    transformed_exterior = [transformador.transform(v[0], v[1]) for v in pol.exterior.coords]
-    transformed_interiors = [[transformador.transform(v[0], v[1]) for v in hole.coords] for hole in pol.interiors]
+    transformed_exterior = [transformador.transform(v[0], v[1]) for v in polygon.exterior.coords]
+    transformed_interiors = [[transformador.transform(v[0], v[1]) for v in hole.coords] for hole in polygon.interiors]
 
     return Polygon(transformed_exterior, transformed_interiors)
 
 
 def change_crs_tuple_point(punto, crs_in, crs_out):
     src_origen = pyproj.CRS(crs_in)
     src_destino = pyproj.CRS(crs_out)
```

### Comparing `aeroterra_ds-1.1.7/src/geometry/geometry.py` & `aeroterra_ds-1.1.8/src/geometry/geometry.py`

 * *Files identical despite different names*

### Comparing `aeroterra_ds-1.1.7/src/layers/common.py` & `aeroterra_ds-1.1.8/src/layers/common.py`

 * *Files identical despite different names*

### Comparing `aeroterra_ds-1.1.7/src/layers/fields.py` & `aeroterra_ds-1.1.8/src/layers/fields.py`

 * *Files identical despite different names*

### Comparing `aeroterra_ds-1.1.7/src/layers/layers.py` & `aeroterra_ds-1.1.8/src/layers/layers.py`

 * *Files identical despite different names*

### Comparing `aeroterra_ds-1.1.7/src/layers/properties.py` & `aeroterra_ds-1.1.8/src/layers/properties.py`

 * *Files identical despite different names*

### Comparing `aeroterra_ds-1.1.7/src/layers/symbology.py` & `aeroterra_ds-1.1.8/src/layers/symbology.py`

 * *Files identical despite different names*

