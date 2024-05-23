# Comparing `tmp/aeroterra_ds-1.1.2.tar.gz` & `tmp/aeroterra_ds-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aeroterra_ds-1.1.2.tar", last modified: Thu May 23 18:33:14 2024, max compression
+gzip compressed data, was "aeroterra_ds-1.1.3.tar", last modified: Thu May 23 18:36:29 2024, max compression
```

## Comparing `aeroterra_ds-1.1.2.tar` & `aeroterra_ds-1.1.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 18:33:14.398308 aeroterra_ds-1.1.2/
--rw-rw-rw-   0        0        0     1324 2024-05-23 18:33:14.397302 aeroterra_ds-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      853 2024-05-23 18:24:06.000000 aeroterra_ds-1.1.2/README.md
--rw-rw-rw-   0        0        0       42 2024-05-23 18:33:14.398308 aeroterra_ds-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0      888 2024-05-23 18:33:13.000000 aeroterra_ds-1.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-23 18:33:14.375801 aeroterra_ds-1.1.2/src/
-drwxrwxrwx   0        0        0        0 2024-05-23 18:33:14.384251 aeroterra_ds-1.1.2/src/aeroterra_ds.egg-info/
--rw-rw-rw-   0        0        0     1324 2024-05-23 18:33:14.000000 aeroterra_ds-1.1.2/src/aeroterra_ds.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      453 2024-05-23 18:33:14.000000 aeroterra_ds-1.1.2/src/aeroterra_ds.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 18:33:14.000000 aeroterra_ds-1.1.2/src/aeroterra_ds.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2024-05-23 18:33:14.000000 aeroterra_ds-1.1.2/src/aeroterra_ds.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-05-23 18:33:14.000000 aeroterra_ds-1.1.2/src/aeroterra_ds.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-23 18:33:14.387763 aeroterra_ds-1.1.2/src/geometry/
--rw-rw-rw-   0        0        0       53 2024-04-19 19:51:19.000000 aeroterra_ds-1.1.2/src/geometry/__init__.py
--rw-rw-rw-   0        0        0     4193 2024-04-22 20:53:00.000000 aeroterra_ds-1.1.2/src/geometry/change_crs.py
--rw-rw-rw-   0        0        0     5752 2024-04-19 19:51:29.000000 aeroterra_ds-1.1.2/src/geometry/geometry.py
-drwxrwxrwx   0        0        0        0 2024-05-23 18:33:14.396282 aeroterra_ds-1.1.2/src/layers/
--rw-rw-rw-   0        0        0       53 2024-04-19 18:38:17.000000 aeroterra_ds-1.1.2/src/layers/__init__.py
--rw-rw-rw-   0        0        0     1720 2024-04-29 14:04:32.000000 aeroterra_ds-1.1.2/src/layers/common.py
--rw-rw-rw-   0        0        0      466 2024-04-18 20:25:50.000000 aeroterra_ds-1.1.2/src/layers/constants.py
--rw-rw-rw-   0        0        0     4759 2024-05-23 18:33:04.000000 aeroterra_ds-1.1.2/src/layers/fields.py
--rw-rw-rw-   0        0        0    14697 2024-05-23 18:31:31.000000 aeroterra_ds-1.1.2/src/layers/layers.py
--rw-rw-rw-   0        0        0     6691 2024-04-29 14:04:39.000000 aeroterra_ds-1.1.2/src/layers/properties.py
--rw-rw-rw-   0        0        0     2323 2024-04-18 20:36:51.000000 aeroterra_ds-1.1.2/src/layers/symbology.py
+drwxrwxrwx   0        0        0        0 2024-05-23 18:36:29.191994 aeroterra_ds-1.1.3/
+-rw-rw-rw-   0        0        0     1324 2024-05-23 18:36:29.191994 aeroterra_ds-1.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      853 2024-05-23 18:24:06.000000 aeroterra_ds-1.1.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-23 18:36:29.193001 aeroterra_ds-1.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      888 2024-05-23 18:36:22.000000 aeroterra_ds-1.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 18:36:29.169438 aeroterra_ds-1.1.3/src/
+drwxrwxrwx   0        0        0        0 2024-05-23 18:36:29.177951 aeroterra_ds-1.1.3/src/aeroterra_ds.egg-info/
+-rw-rw-rw-   0        0        0     1324 2024-05-23 18:36:29.000000 aeroterra_ds-1.1.3/src/aeroterra_ds.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      453 2024-05-23 18:36:29.000000 aeroterra_ds-1.1.3/src/aeroterra_ds.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 18:36:29.000000 aeroterra_ds-1.1.3/src/aeroterra_ds.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2024-05-23 18:36:29.000000 aeroterra_ds-1.1.3/src/aeroterra_ds.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-23 18:36:29.000000 aeroterra_ds-1.1.3/src/aeroterra_ds.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-23 18:36:29.183465 aeroterra_ds-1.1.3/src/geometry/
+-rw-rw-rw-   0        0        0       53 2024-04-19 19:51:19.000000 aeroterra_ds-1.1.3/src/geometry/__init__.py
+-rw-rw-rw-   0        0        0     4193 2024-04-22 20:53:00.000000 aeroterra_ds-1.1.3/src/geometry/change_crs.py
+-rw-rw-rw-   0        0        0     5752 2024-04-19 19:51:29.000000 aeroterra_ds-1.1.3/src/geometry/geometry.py
+drwxrwxrwx   0        0        0        0 2024-05-23 18:36:29.190983 aeroterra_ds-1.1.3/src/layers/
+-rw-rw-rw-   0        0        0       53 2024-04-19 18:38:17.000000 aeroterra_ds-1.1.3/src/layers/__init__.py
+-rw-rw-rw-   0        0        0     1720 2024-04-29 14:04:32.000000 aeroterra_ds-1.1.3/src/layers/common.py
+-rw-rw-rw-   0        0        0      466 2024-04-18 20:25:50.000000 aeroterra_ds-1.1.3/src/layers/constants.py
+-rw-rw-rw-   0        0        0     4759 2024-05-23 18:33:04.000000 aeroterra_ds-1.1.3/src/layers/fields.py
+-rw-rw-rw-   0        0        0    14718 2024-05-23 18:36:18.000000 aeroterra_ds-1.1.3/src/layers/layers.py
+-rw-rw-rw-   0        0        0     6691 2024-04-29 14:04:39.000000 aeroterra_ds-1.1.3/src/layers/properties.py
+-rw-rw-rw-   0        0        0     2323 2024-04-18 20:36:51.000000 aeroterra_ds-1.1.3/src/layers/symbology.py
```

### Comparing `aeroterra_ds-1.1.2/PKG-INFO` & `aeroterra_ds-1.1.3/src/aeroterra_ds.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: aeroterra_ds
-Version: 1.1.2
+Name: aeroterra-ds
+Version: 1.1.3
 Summary: Python Functions To Work With GeoSpatial Data & ArcGis in a simpler way
 Home-page: https://example.com
 Author: Data Science
 Author-email: aeroterra_ds@aeroterra.com
 Keywords: arcgis
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `aeroterra_ds-1.1.2/README.md` & `aeroterra_ds-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `aeroterra_ds-1.1.2/setup.py` & `aeroterra_ds-1.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='aeroterra_ds',
-    version='1.1.2',
+    version='1.1.3',
     author='Data Science',
     author_email='aeroterra_ds@aeroterra.com',
     description='Python Functions To Work With GeoSpatial Data & ArcGis in a simpler way',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://example.com',
     package_dir={'': "src"},
```

### Comparing `aeroterra_ds-1.1.2/src/aeroterra_ds.egg-info/PKG-INFO` & `aeroterra_ds-1.1.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: aeroterra-ds
-Version: 1.1.2
+Name: aeroterra_ds
+Version: 1.1.3
 Summary: Python Functions To Work With GeoSpatial Data & ArcGis in a simpler way
 Home-page: https://example.com
 Author: Data Science
 Author-email: aeroterra_ds@aeroterra.com
 Keywords: arcgis
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `aeroterra_ds-1.1.2/src/geometry/change_crs.py` & `aeroterra_ds-1.1.3/src/geometry/change_crs.py`

 * *Files identical despite different names*

### Comparing `aeroterra_ds-1.1.2/src/geometry/geometry.py` & `aeroterra_ds-1.1.3/src/geometry/geometry.py`

 * *Files identical despite different names*

### Comparing `aeroterra_ds-1.1.2/src/layers/common.py` & `aeroterra_ds-1.1.3/src/layers/common.py`

 * *Files identical despite different names*

### Comparing `aeroterra_ds-1.1.2/src/layers/fields.py` & `aeroterra_ds-1.1.3/src/layers/fields.py`

 * *Files identical despite different names*

### Comparing `aeroterra_ds-1.1.2/src/layers/layers.py` & `aeroterra_ds-1.1.3/src/layers/layers.py`

 * *Files 1% similar despite different names*

```diff
@@ -203,32 +203,31 @@
         raise Exception(f"{object_id_col} Must Be Present In GDF In Order To Know Which Line To Update")
 
     if "geometry" in gdf.columns:
         gdf = change_gdf_to_layer_crs(gdf, layer)
         gdf = GeoAccessor.from_geodataframe(gdf)
 
     feature_set = FeatureSet(features=[])
-
+    total = []
     for index, row in gdf.iterrows():
         if "geometry" in gdf.columns:
             data = row.to_dict()
             geo = data.pop("geometry")
             feature = Feature(attributes=data, geometry=geo)
         else:
             data = row.to_dict()
             feature = Feature(attributes=data, geometry=None)
             
         feature_set.features.append(feature)
+        if len(feature_set) == 1000:
+            total.append(layer.edit_features(updates = feature_set))
+            feature_set = FeatureSet(features=[])
     
-    total = []
-    for i in range(0, len(feature_set), BATCH_AMOUNT):
-        end = i + BATCH_AMOUNT
-        if i > len(feature_set):
-            end = len(feature_set)
-        total.append(layer.edit_features(updates = feature_set[i: end]))
+    if len(feature_set) > 0:
+        total.append(layer.edit_features(updates = feature_set))
 
     return total
 
 
 def empty_layer(gis, layer_id):
     """
     Empty the data from a layer
```

### Comparing `aeroterra_ds-1.1.2/src/layers/properties.py` & `aeroterra_ds-1.1.3/src/layers/properties.py`

 * *Files identical despite different names*

### Comparing `aeroterra_ds-1.1.2/src/layers/symbology.py` & `aeroterra_ds-1.1.3/src/layers/symbology.py`

 * *Files identical despite different names*

