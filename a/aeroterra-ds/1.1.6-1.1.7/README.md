# Comparing `tmp/aeroterra_ds-1.1.6.tar.gz` & `tmp/aeroterra_ds-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aeroterra_ds-1.1.6.tar", last modified: Thu May 23 18:50:09 2024, max compression
+gzip compressed data, was "aeroterra_ds-1.1.7.tar", last modified: Thu May 23 19:25:41 2024, max compression
```

## Comparing `aeroterra_ds-1.1.6.tar` & `aeroterra_ds-1.1.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 18:50:09.009834 aeroterra_ds-1.1.6/
--rw-rw-rw-   0        0        0     1325 2024-05-23 18:50:09.009834 aeroterra_ds-1.1.6/PKG-INFO
--rw-rw-rw-   0        0        0      854 2024-05-23 18:46:51.000000 aeroterra_ds-1.1.6/README.md
--rw-rw-rw-   0        0        0       42 2024-05-23 18:50:09.010856 aeroterra_ds-1.1.6/setup.cfg
--rw-rw-rw-   0        0        0      888 2024-05-23 18:50:02.000000 aeroterra_ds-1.1.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-23 18:50:08.978482 aeroterra_ds-1.1.6/src/
-drwxrwxrwx   0        0        0        0 2024-05-23 18:50:08.997317 aeroterra_ds-1.1.6/src/aeroterra_ds.egg-info/
--rw-rw-rw-   0        0        0     1325 2024-05-23 18:50:08.000000 aeroterra_ds-1.1.6/src/aeroterra_ds.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      453 2024-05-23 18:50:08.000000 aeroterra_ds-1.1.6/src/aeroterra_ds.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 18:50:08.000000 aeroterra_ds-1.1.6/src/aeroterra_ds.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2024-05-23 18:50:08.000000 aeroterra_ds-1.1.6/src/aeroterra_ds.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-05-23 18:50:08.000000 aeroterra_ds-1.1.6/src/aeroterra_ds.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-23 18:50:09.000316 aeroterra_ds-1.1.6/src/geometry/
--rw-rw-rw-   0        0        0       53 2024-04-19 19:51:19.000000 aeroterra_ds-1.1.6/src/geometry/__init__.py
--rw-rw-rw-   0        0        0     4193 2024-04-22 20:53:00.000000 aeroterra_ds-1.1.6/src/geometry/change_crs.py
--rw-rw-rw-   0        0        0     5752 2024-04-19 19:51:29.000000 aeroterra_ds-1.1.6/src/geometry/geometry.py
-drwxrwxrwx   0        0        0        0 2024-05-23 18:50:09.007833 aeroterra_ds-1.1.6/src/layers/
--rw-rw-rw-   0        0        0       53 2024-04-19 18:38:17.000000 aeroterra_ds-1.1.6/src/layers/__init__.py
--rw-rw-rw-   0        0        0     1720 2024-04-29 14:04:32.000000 aeroterra_ds-1.1.6/src/layers/common.py
--rw-rw-rw-   0        0        0      466 2024-04-18 20:25:50.000000 aeroterra_ds-1.1.6/src/layers/constants.py
--rw-rw-rw-   0        0        0     5510 2024-05-23 18:49:59.000000 aeroterra_ds-1.1.6/src/layers/fields.py
--rw-rw-rw-   0        0        0    14718 2024-05-23 18:36:18.000000 aeroterra_ds-1.1.6/src/layers/layers.py
--rw-rw-rw-   0        0        0     6691 2024-04-29 14:04:39.000000 aeroterra_ds-1.1.6/src/layers/properties.py
--rw-rw-rw-   0        0        0     2323 2024-04-18 20:36:51.000000 aeroterra_ds-1.1.6/src/layers/symbology.py
+drwxrwxrwx   0        0        0        0 2024-05-23 19:25:41.502490 aeroterra_ds-1.1.7/
+-rw-rw-rw-   0        0        0     1325 2024-05-23 19:25:41.501162 aeroterra_ds-1.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0      854 2024-05-23 18:46:51.000000 aeroterra_ds-1.1.7/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-23 19:25:41.502490 aeroterra_ds-1.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      888 2024-05-23 19:25:35.000000 aeroterra_ds-1.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 19:25:41.481379 aeroterra_ds-1.1.7/src/
+drwxrwxrwx   0        0        0        0 2024-05-23 19:25:41.487703 aeroterra_ds-1.1.7/src/aeroterra_ds.egg-info/
+-rw-rw-rw-   0        0        0     1325 2024-05-23 19:25:41.000000 aeroterra_ds-1.1.7/src/aeroterra_ds.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      453 2024-05-23 19:25:41.000000 aeroterra_ds-1.1.7/src/aeroterra_ds.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 19:25:41.000000 aeroterra_ds-1.1.7/src/aeroterra_ds.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2024-05-23 19:25:41.000000 aeroterra_ds-1.1.7/src/aeroterra_ds.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-23 19:25:41.000000 aeroterra_ds-1.1.7/src/aeroterra_ds.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-23 19:25:41.489711 aeroterra_ds-1.1.7/src/geometry/
+-rw-rw-rw-   0        0        0       53 2024-04-19 19:51:19.000000 aeroterra_ds-1.1.7/src/geometry/__init__.py
+-rw-rw-rw-   0        0        0     4193 2024-04-22 20:53:00.000000 aeroterra_ds-1.1.7/src/geometry/change_crs.py
+-rw-rw-rw-   0        0        0     5752 2024-04-19 19:51:29.000000 aeroterra_ds-1.1.7/src/geometry/geometry.py
+drwxrwxrwx   0        0        0        0 2024-05-23 19:25:41.500181 aeroterra_ds-1.1.7/src/layers/
+-rw-rw-rw-   0        0        0       53 2024-04-19 18:38:17.000000 aeroterra_ds-1.1.7/src/layers/__init__.py
+-rw-rw-rw-   0        0        0     1720 2024-04-29 14:04:32.000000 aeroterra_ds-1.1.7/src/layers/common.py
+-rw-rw-rw-   0        0        0      466 2024-04-18 20:25:50.000000 aeroterra_ds-1.1.7/src/layers/constants.py
+-rw-rw-rw-   0        0        0     5510 2024-05-23 18:49:59.000000 aeroterra_ds-1.1.7/src/layers/fields.py
+-rw-rw-rw-   0        0        0    15183 2024-05-23 19:25:30.000000 aeroterra_ds-1.1.7/src/layers/layers.py
+-rw-rw-rw-   0        0        0     6691 2024-04-29 14:04:39.000000 aeroterra_ds-1.1.7/src/layers/properties.py
+-rw-rw-rw-   0        0        0     2323 2024-04-18 20:36:51.000000 aeroterra_ds-1.1.7/src/layers/symbology.py
```

### Comparing `aeroterra_ds-1.1.6/PKG-INFO` & `aeroterra_ds-1.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aeroterra_ds
-Version: 1.1.6
+Version: 1.1.7
 Summary: Python Functions To Work With GeoSpatial Data & ArcGis in a simpler way
 Home-page: https://example.com
 Author: Data Science
 Author-email: aeroterra_ds@aeroterra.com
 Keywords: arcgis
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `aeroterra_ds-1.1.6/README.md` & `aeroterra_ds-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `aeroterra_ds-1.1.6/setup.py` & `aeroterra_ds-1.1.7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='aeroterra_ds',
-    version='1.1.6',
+    version='1.1.7',
     author='Data Science',
     author_email='aeroterra_ds@aeroterra.com',
     description='Python Functions To Work With GeoSpatial Data & ArcGis in a simpler way',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://example.com',
     package_dir={'': "src"},
```

### Comparing `aeroterra_ds-1.1.6/src/aeroterra_ds.egg-info/PKG-INFO` & `aeroterra_ds-1.1.7/src/aeroterra_ds.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aeroterra-ds
-Version: 1.1.6
+Version: 1.1.7
 Summary: Python Functions To Work With GeoSpatial Data & ArcGis in a simpler way
 Home-page: https://example.com
 Author: Data Science
 Author-email: aeroterra_ds@aeroterra.com
 Keywords: arcgis
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `aeroterra_ds-1.1.6/src/geometry/change_crs.py` & `aeroterra_ds-1.1.7/src/geometry/change_crs.py`

 * *Files identical despite different names*

### Comparing `aeroterra_ds-1.1.6/src/geometry/geometry.py` & `aeroterra_ds-1.1.7/src/geometry/geometry.py`

 * *Files identical despite different names*

### Comparing `aeroterra_ds-1.1.6/src/layers/common.py` & `aeroterra_ds-1.1.7/src/layers/common.py`

 * *Files identical despite different names*

### Comparing `aeroterra_ds-1.1.6/src/layers/fields.py` & `aeroterra_ds-1.1.7/src/layers/fields.py`

 * *Files identical despite different names*

### Comparing `aeroterra_ds-1.1.6/src/layers/layers.py` & `aeroterra_ds-1.1.7/src/layers/layers.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from arcgis.geometry.filters import intersects
 #TODO: Remove GeoAccessor
 
 from .common import get_layer, ordinal
 from .properties import get_layer_crs_aux, get_objectid_field_aux, get_fields_aux, get_symbology_aux
 from .properties import get_pop_up, update_pop_up
 from geometry.geometry import create_geo_json
+from geometry.change_crs import change_crs
 
 BATCH_AMOUNT = 1000
 READ_BATCH = 10000
 
 def get_layer_in_list(layers_found, title):
     """
     Find Layer titled as title inside all the layers found
@@ -352,15 +353,15 @@
     Returns a GeoDataFrame
     """
     layer = get_layer(gis, layer_id)
 
     return read_full_layer_aux(layer)
 
 
-def read_layer_gdf(gis, layer_id, number=None, query=None, geometry_filter=None, geometry_crs=4326, out_fields=None, out_crs=None):
+def read_layer_gdf(gis, layer_id, number=None, query=None, geometry_filter=None, geometry_crs=4326, out_fields=None, out_crs=None, geometry_post=True):
     """
     Returns the full data stored in an asked layer.
     
     Parameters:
         - gis: GIS struct from the user that owns the layer
         - layer_id: Layer ID of the layer wanting to be asked
         - number (Optional): Layer Number inside the item. If not provided
@@ -368,22 +369,23 @@
         - query (Optional): String representing a SQL query to filter the data to 
             to be read from the layer. If None, all the data will be providen.
         - geometry_filter (Optional): Shapely (Multi)Polygon to filter data geographically.
             If None, all the data will be providen.
         - geometry_crs (Optional): CRS of the given geometry_filer. If missing, 4326 will be assumed.
         - out_fields (Optional): List of fields names to recieve. If None, all will be returned.
         - out_crs (Optional): CRS of the returned gdf. If None, the crs of the layer will be used.
+        - geometry_post (Optional): If the geometry filter exists, if it should be done after the layer query. True by default
 
 
     Returns a GeoDataFrame
     """
     layer = get_layer(gis, layer_id, number)
 
     geo_filter = None
-    if geometry_filter is not None:
+    if geometry_filter is not None and not geometry_post:
         bounds = create_geo_json(geometry_filter, geometry_crs)
         geo_filter = intersects(bounds)
 
     if out_crs is None:
         out_crs = get_layer_crs_aux(layer)
 
     object_id_col = get_objectid_field_aux(layer)
@@ -415,9 +417,16 @@
         total_data = total_data.rename(columns = {"SHAPE": "geometry"})
         return total_data
 
     if out_fields != "*" and object_id_col not in out_fields:
         total_data = total_data.drop(columns=[object_id_col])
 
     total_data = total_data.rename(columns = {"SHAPE": "geometry"})
-    return gpd.GeoDataFrame(total_data, geometry="geometry", crs=out_crs)
+
+    gdf_result = gpd.GeoDataFrame(total_data, geometry="geometry", crs=out_crs)
+
+    if geometry_filter is not None and geometry_post:
+        filter_polygon = change_crs(geometry_filter, geometry_crs, out_crs)
+        gdf_result = gdf_result[gdf_result["geometry"].intersects(filter_polygon)]
+
+    return gdf_result
```

### Comparing `aeroterra_ds-1.1.6/src/layers/properties.py` & `aeroterra_ds-1.1.7/src/layers/properties.py`

 * *Files identical despite different names*

### Comparing `aeroterra_ds-1.1.6/src/layers/symbology.py` & `aeroterra_ds-1.1.7/src/layers/symbology.py`

 * *Files identical despite different names*

