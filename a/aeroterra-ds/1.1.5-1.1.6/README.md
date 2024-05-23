# Comparing `tmp/aeroterra_ds-1.1.5.tar.gz` & `tmp/aeroterra_ds-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aeroterra_ds-1.1.5.tar", last modified: Thu May 23 18:47:04 2024, max compression
+gzip compressed data, was "aeroterra_ds-1.1.6.tar", last modified: Thu May 23 18:50:09 2024, max compression
```

## Comparing `aeroterra_ds-1.1.5.tar` & `aeroterra_ds-1.1.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 18:47:04.071501 aeroterra_ds-1.1.5/
--rw-rw-rw-   0        0        0     1325 2024-05-23 18:47:04.071501 aeroterra_ds-1.1.5/PKG-INFO
--rw-rw-rw-   0        0        0      854 2024-05-23 18:46:51.000000 aeroterra_ds-1.1.5/README.md
--rw-rw-rw-   0        0        0       42 2024-05-23 18:47:04.071501 aeroterra_ds-1.1.5/setup.cfg
--rw-rw-rw-   0        0        0      888 2024-05-23 18:46:57.000000 aeroterra_ds-1.1.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-23 18:47:04.051916 aeroterra_ds-1.1.5/src/
-drwxrwxrwx   0        0        0        0 2024-05-23 18:47:04.058429 aeroterra_ds-1.1.5/src/aeroterra_ds.egg-info/
--rw-rw-rw-   0        0        0     1325 2024-05-23 18:47:03.000000 aeroterra_ds-1.1.5/src/aeroterra_ds.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      453 2024-05-23 18:47:03.000000 aeroterra_ds-1.1.5/src/aeroterra_ds.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 18:47:03.000000 aeroterra_ds-1.1.5/src/aeroterra_ds.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2024-05-23 18:47:03.000000 aeroterra_ds-1.1.5/src/aeroterra_ds.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-05-23 18:47:03.000000 aeroterra_ds-1.1.5/src/aeroterra_ds.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-23 18:47:04.061426 aeroterra_ds-1.1.5/src/geometry/
--rw-rw-rw-   0        0        0       53 2024-04-19 19:51:19.000000 aeroterra_ds-1.1.5/src/geometry/__init__.py
--rw-rw-rw-   0        0        0     4193 2024-04-22 20:53:00.000000 aeroterra_ds-1.1.5/src/geometry/change_crs.py
--rw-rw-rw-   0        0        0     5752 2024-04-19 19:51:29.000000 aeroterra_ds-1.1.5/src/geometry/geometry.py
-drwxrwxrwx   0        0        0        0 2024-05-23 18:47:04.070501 aeroterra_ds-1.1.5/src/layers/
--rw-rw-rw-   0        0        0       53 2024-04-19 18:38:17.000000 aeroterra_ds-1.1.5/src/layers/__init__.py
--rw-rw-rw-   0        0        0     1720 2024-04-29 14:04:32.000000 aeroterra_ds-1.1.5/src/layers/common.py
--rw-rw-rw-   0        0        0      466 2024-04-18 20:25:50.000000 aeroterra_ds-1.1.5/src/layers/constants.py
--rw-rw-rw-   0        0        0     5458 2024-05-23 18:46:50.000000 aeroterra_ds-1.1.5/src/layers/fields.py
--rw-rw-rw-   0        0        0    14718 2024-05-23 18:36:18.000000 aeroterra_ds-1.1.5/src/layers/layers.py
--rw-rw-rw-   0        0        0     6691 2024-04-29 14:04:39.000000 aeroterra_ds-1.1.5/src/layers/properties.py
--rw-rw-rw-   0        0        0     2323 2024-04-18 20:36:51.000000 aeroterra_ds-1.1.5/src/layers/symbology.py
+drwxrwxrwx   0        0        0        0 2024-05-23 18:50:09.009834 aeroterra_ds-1.1.6/
+-rw-rw-rw-   0        0        0     1325 2024-05-23 18:50:09.009834 aeroterra_ds-1.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0      854 2024-05-23 18:46:51.000000 aeroterra_ds-1.1.6/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-23 18:50:09.010856 aeroterra_ds-1.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      888 2024-05-23 18:50:02.000000 aeroterra_ds-1.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 18:50:08.978482 aeroterra_ds-1.1.6/src/
+drwxrwxrwx   0        0        0        0 2024-05-23 18:50:08.997317 aeroterra_ds-1.1.6/src/aeroterra_ds.egg-info/
+-rw-rw-rw-   0        0        0     1325 2024-05-23 18:50:08.000000 aeroterra_ds-1.1.6/src/aeroterra_ds.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      453 2024-05-23 18:50:08.000000 aeroterra_ds-1.1.6/src/aeroterra_ds.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 18:50:08.000000 aeroterra_ds-1.1.6/src/aeroterra_ds.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2024-05-23 18:50:08.000000 aeroterra_ds-1.1.6/src/aeroterra_ds.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-23 18:50:08.000000 aeroterra_ds-1.1.6/src/aeroterra_ds.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-23 18:50:09.000316 aeroterra_ds-1.1.6/src/geometry/
+-rw-rw-rw-   0        0        0       53 2024-04-19 19:51:19.000000 aeroterra_ds-1.1.6/src/geometry/__init__.py
+-rw-rw-rw-   0        0        0     4193 2024-04-22 20:53:00.000000 aeroterra_ds-1.1.6/src/geometry/change_crs.py
+-rw-rw-rw-   0        0        0     5752 2024-04-19 19:51:29.000000 aeroterra_ds-1.1.6/src/geometry/geometry.py
+drwxrwxrwx   0        0        0        0 2024-05-23 18:50:09.007833 aeroterra_ds-1.1.6/src/layers/
+-rw-rw-rw-   0        0        0       53 2024-04-19 18:38:17.000000 aeroterra_ds-1.1.6/src/layers/__init__.py
+-rw-rw-rw-   0        0        0     1720 2024-04-29 14:04:32.000000 aeroterra_ds-1.1.6/src/layers/common.py
+-rw-rw-rw-   0        0        0      466 2024-04-18 20:25:50.000000 aeroterra_ds-1.1.6/src/layers/constants.py
+-rw-rw-rw-   0        0        0     5510 2024-05-23 18:49:59.000000 aeroterra_ds-1.1.6/src/layers/fields.py
+-rw-rw-rw-   0        0        0    14718 2024-05-23 18:36:18.000000 aeroterra_ds-1.1.6/src/layers/layers.py
+-rw-rw-rw-   0        0        0     6691 2024-04-29 14:04:39.000000 aeroterra_ds-1.1.6/src/layers/properties.py
+-rw-rw-rw-   0        0        0     2323 2024-04-18 20:36:51.000000 aeroterra_ds-1.1.6/src/layers/symbology.py
```

### Comparing `aeroterra_ds-1.1.5/PKG-INFO` & `aeroterra_ds-1.1.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aeroterra_ds
-Version: 1.1.5
+Version: 1.1.6
 Summary: Python Functions To Work With GeoSpatial Data & ArcGis in a simpler way
 Home-page: https://example.com
 Author: Data Science
 Author-email: aeroterra_ds@aeroterra.com
 Keywords: arcgis
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `aeroterra_ds-1.1.5/README.md` & `aeroterra_ds-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `aeroterra_ds-1.1.5/setup.py` & `aeroterra_ds-1.1.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='aeroterra_ds',
-    version='1.1.5',
+    version='1.1.6',
     author='Data Science',
     author_email='aeroterra_ds@aeroterra.com',
     description='Python Functions To Work With GeoSpatial Data & ArcGis in a simpler way',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://example.com',
     package_dir={'': "src"},
```

### Comparing `aeroterra_ds-1.1.5/src/aeroterra_ds.egg-info/PKG-INFO` & `aeroterra_ds-1.1.6/src/aeroterra_ds.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aeroterra-ds
-Version: 1.1.5
+Version: 1.1.6
 Summary: Python Functions To Work With GeoSpatial Data & ArcGis in a simpler way
 Home-page: https://example.com
 Author: Data Science
 Author-email: aeroterra_ds@aeroterra.com
 Keywords: arcgis
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `aeroterra_ds-1.1.5/src/geometry/change_crs.py` & `aeroterra_ds-1.1.6/src/geometry/change_crs.py`

 * *Files identical despite different names*

### Comparing `aeroterra_ds-1.1.5/src/geometry/geometry.py` & `aeroterra_ds-1.1.6/src/geometry/geometry.py`

 * *Files identical despite different names*

### Comparing `aeroterra_ds-1.1.5/src/layers/common.py` & `aeroterra_ds-1.1.6/src/layers/common.py`

 * *Files identical despite different names*

### Comparing `aeroterra_ds-1.1.5/src/layers/fields.py` & `aeroterra_ds-1.1.6/src/layers/fields.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,15 +139,15 @@
     old_names = []
     data_types = {}
     fields = get_fields_aux(layer)
     for old_name in change_names.keys():
         data_type = None
         for field in fields:
             if field[0] == old_name:
-                data_types[old_name] = data_type
+                data_types[old_name] = field[2]
                 old_names.append(old_name)
                 break
     
     if len(old_names) == 0:
         raise Exception("No Valid Field Found To Change")
 
     object_id_field = get_objectid_field_aux(layer)
@@ -155,16 +155,18 @@
     fields_to_ask = [object_id_field]
     fields_to_ask.extend(old_names)
 
     old_data = read_full_layer(gis, layer_id)[fields_to_ask]
     
     new_names = []
     for old_name, new_name in change_names.items():
-        new_names.append(new_name)
         data_type = data_types.get(old_name)
+        if data_type is None:
+            continue
+        new_names.append(new_name)
         add_field_aux(layer, new_name, data_type)
 
     new_data = old_data.rename(columns=change_names)
 
     adds = update_layer(new_data, gis, layer_id, columns=new_names)
     for old_name in old_names:
         delete_field_aux(layer, old_name)
```

### Comparing `aeroterra_ds-1.1.5/src/layers/layers.py` & `aeroterra_ds-1.1.6/src/layers/layers.py`

 * *Files identical despite different names*

### Comparing `aeroterra_ds-1.1.5/src/layers/properties.py` & `aeroterra_ds-1.1.6/src/layers/properties.py`

 * *Files identical despite different names*

### Comparing `aeroterra_ds-1.1.5/src/layers/symbology.py` & `aeroterra_ds-1.1.6/src/layers/symbology.py`

 * *Files identical despite different names*

