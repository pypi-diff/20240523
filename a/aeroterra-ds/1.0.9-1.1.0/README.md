# Comparing `tmp/aeroterra_ds-1.0.9.tar.gz` & `tmp/aeroterra_ds-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aeroterra_ds-1.0.9.tar", last modified: Mon Apr 22 20:51:44 2024, max compression
+gzip compressed data, was "aeroterra_ds-1.1.0.tar", last modified: Thu May 23 18:24:44 2024, max compression
```

## Comparing `aeroterra_ds-1.0.9.tar` & `aeroterra_ds-1.1.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-22 20:51:44.642631 aeroterra_ds-1.0.9/
--rw-rw-rw-   0        0        0     1306 2024-04-22 20:51:44.642631 aeroterra_ds-1.0.9/PKG-INFO
--rw-rw-rw-   0        0        0      835 2024-04-19 19:51:22.000000 aeroterra_ds-1.0.9/README.md
--rw-rw-rw-   0        0        0       42 2024-04-22 20:51:44.642631 aeroterra_ds-1.0.9/setup.cfg
--rw-rw-rw-   0        0        0      888 2024-04-22 20:51:40.000000 aeroterra_ds-1.0.9/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-22 20:51:44.614255 aeroterra_ds-1.0.9/src/
-drwxrwxrwx   0        0        0        0 2024-04-22 20:51:44.630347 aeroterra_ds-1.0.9/src/aeroterra_ds.egg-info/
--rw-rw-rw-   0        0        0     1306 2024-04-22 20:51:44.000000 aeroterra_ds-1.0.9/src/aeroterra_ds.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      453 2024-04-22 20:51:44.000000 aeroterra_ds-1.0.9/src/aeroterra_ds.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-22 20:51:44.000000 aeroterra_ds-1.0.9/src/aeroterra_ds.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2024-04-22 20:51:44.000000 aeroterra_ds-1.0.9/src/aeroterra_ds.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-04-22 20:51:44.000000 aeroterra_ds-1.0.9/src/aeroterra_ds.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-22 20:51:44.634165 aeroterra_ds-1.0.9/src/geometry/
--rw-rw-rw-   0        0        0       53 2024-04-19 19:51:19.000000 aeroterra_ds-1.0.9/src/geometry/__init__.py
--rw-rw-rw-   0        0        0     4193 2024-04-22 20:51:04.000000 aeroterra_ds-1.0.9/src/geometry/change_crs.py
--rw-rw-rw-   0        0        0     5752 2024-04-19 19:51:29.000000 aeroterra_ds-1.0.9/src/geometry/geometry.py
-drwxrwxrwx   0        0        0        0 2024-04-22 20:51:44.641219 aeroterra_ds-1.0.9/src/layers/
--rw-rw-rw-   0        0        0       53 2024-04-19 18:38:17.000000 aeroterra_ds-1.0.9/src/layers/__init__.py
--rw-rw-rw-   0        0        0     1405 2024-04-18 20:25:51.000000 aeroterra_ds-1.0.9/src/layers/common.py
--rw-rw-rw-   0        0        0      466 2024-04-18 20:25:50.000000 aeroterra_ds-1.0.9/src/layers/constants.py
--rw-rw-rw-   0        0        0     3096 2024-04-19 19:15:15.000000 aeroterra_ds-1.0.9/src/layers/fields.py
--rw-rw-rw-   0        0        0    10632 2024-04-19 20:58:06.000000 aeroterra_ds-1.0.9/src/layers/layers.py
--rw-rw-rw-   0        0        0     4125 2024-04-22 14:26:14.000000 aeroterra_ds-1.0.9/src/layers/properties.py
--rw-rw-rw-   0        0        0     2323 2024-04-18 20:36:51.000000 aeroterra_ds-1.0.9/src/layers/symbology.py
+drwxrwxrwx   0        0        0        0 2024-05-23 18:24:44.822752 aeroterra_ds-1.1.0/
+-rw-rw-rw-   0        0        0     1324 2024-05-23 18:24:44.821731 aeroterra_ds-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      853 2024-05-23 18:24:06.000000 aeroterra_ds-1.1.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-23 18:24:44.822752 aeroterra_ds-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      888 2024-05-23 18:24:33.000000 aeroterra_ds-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 18:24:44.800305 aeroterra_ds-1.1.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-23 18:24:44.809480 aeroterra_ds-1.1.0/src/aeroterra_ds.egg-info/
+-rw-rw-rw-   0        0        0     1324 2024-05-23 18:24:44.000000 aeroterra_ds-1.1.0/src/aeroterra_ds.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      453 2024-05-23 18:24:44.000000 aeroterra_ds-1.1.0/src/aeroterra_ds.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 18:24:44.000000 aeroterra_ds-1.1.0/src/aeroterra_ds.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2024-05-23 18:24:44.000000 aeroterra_ds-1.1.0/src/aeroterra_ds.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-23 18:24:44.000000 aeroterra_ds-1.1.0/src/aeroterra_ds.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-23 18:24:44.812476 aeroterra_ds-1.1.0/src/geometry/
+-rw-rw-rw-   0        0        0       53 2024-04-19 19:51:19.000000 aeroterra_ds-1.1.0/src/geometry/__init__.py
+-rw-rw-rw-   0        0        0     4193 2024-04-22 20:53:00.000000 aeroterra_ds-1.1.0/src/geometry/change_crs.py
+-rw-rw-rw-   0        0        0     5752 2024-04-19 19:51:29.000000 aeroterra_ds-1.1.0/src/geometry/geometry.py
+drwxrwxrwx   0        0        0        0 2024-05-23 18:24:44.820381 aeroterra_ds-1.1.0/src/layers/
+-rw-rw-rw-   0        0        0       53 2024-04-19 18:38:17.000000 aeroterra_ds-1.1.0/src/layers/__init__.py
+-rw-rw-rw-   0        0        0     1720 2024-04-29 14:04:32.000000 aeroterra_ds-1.1.0/src/layers/common.py
+-rw-rw-rw-   0        0        0      466 2024-04-18 20:25:50.000000 aeroterra_ds-1.1.0/src/layers/constants.py
+-rw-rw-rw-   0        0        0     4768 2024-05-23 18:24:17.000000 aeroterra_ds-1.1.0/src/layers/fields.py
+-rw-rw-rw-   0        0        0    14697 2024-05-23 18:09:00.000000 aeroterra_ds-1.1.0/src/layers/layers.py
+-rw-rw-rw-   0        0        0     6691 2024-04-29 14:04:39.000000 aeroterra_ds-1.1.0/src/layers/properties.py
+-rw-rw-rw-   0        0        0     2323 2024-04-18 20:36:51.000000 aeroterra_ds-1.1.0/src/layers/symbology.py
```

### Comparing `aeroterra_ds-1.0.9/PKG-INFO` & `aeroterra_ds-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aeroterra_ds
-Version: 1.0.9
+Version: 1.1.0
 Summary: Python Functions To Work With GeoSpatial Data & ArcGis in a simpler way
 Home-page: https://example.com
 Author: Data Science
 Author-email: aeroterra_ds@aeroterra.com
 Keywords: arcgis
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -37,14 +37,15 @@
 	 - read_layer_gdf
  - fields
 	 - add_field
 	 - delete_field
 	 - get_fields
 	 - get_fields
 	 - get_objectid_field
+	 - rename_field
  - properties
 	 - get_symbology
 	 - get_layer_crs
 	 - get_layer_extent
 
 ## Geometry
```

### Comparing `aeroterra_ds-1.0.9/README.md` & `aeroterra_ds-1.1.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 	 - read_layer_gdf
  - fields
 	 - add_field
 	 - delete_field
 	 - get_fields
 	 - get_fields
 	 - get_objectid_field
+	 - rename_field
  - properties
 	 - get_symbology
 	 - get_layer_crs
 	 - get_layer_extent
 
 ## Geometry
```

### Comparing `aeroterra_ds-1.0.9/setup.py` & `aeroterra_ds-1.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='aeroterra_ds',
-    version='1.0.9',
+    version='1.1.0',
     author='Data Science',
     author_email='aeroterra_ds@aeroterra.com',
     description='Python Functions To Work With GeoSpatial Data & ArcGis in a simpler way',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://example.com',
     package_dir={'': "src"},
```

### Comparing `aeroterra_ds-1.0.9/src/aeroterra_ds.egg-info/PKG-INFO` & `aeroterra_ds-1.1.0/src/aeroterra_ds.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aeroterra-ds
-Version: 1.0.9
+Version: 1.1.0
 Summary: Python Functions To Work With GeoSpatial Data & ArcGis in a simpler way
 Home-page: https://example.com
 Author: Data Science
 Author-email: aeroterra_ds@aeroterra.com
 Keywords: arcgis
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -37,14 +37,15 @@
 	 - read_layer_gdf
  - fields
 	 - add_field
 	 - delete_field
 	 - get_fields
 	 - get_fields
 	 - get_objectid_field
+	 - rename_field
  - properties
 	 - get_symbology
 	 - get_layer_crs
 	 - get_layer_extent
 
 ## Geometry
```

### Comparing `aeroterra_ds-1.0.9/src/geometry/change_crs.py` & `aeroterra_ds-1.1.0/src/geometry/change_crs.py`

 * *Files identical despite different names*

### Comparing `aeroterra_ds-1.0.9/src/geometry/geometry.py` & `aeroterra_ds-1.1.0/src/geometry/geometry.py`

 * *Files identical despite different names*

### Comparing `aeroterra_ds-1.0.9/src/layers/common.py` & `aeroterra_ds-1.1.0/src/layers/common.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,29 +8,43 @@
     if 11 <= (n % 100) <= 13:
         suffix = 'th'
     else:
         suffix = ['th', 'st', 'nd', 'rd', 'th'][min(n % 10, 4)]
     return str(n) + suffix
 
 
+def get_item(gis, item_id):
+    """
+    Find Item from its id
+    
+    Parameters:
+        - gis: GIS object logged in where to search from
+        - item_id: ID of the asked item
+    
+    Returns the item object inside the service
+    """
+    gis_item = gis.content.get(item_id)
+    if gis_item is None:
+        raise Exception(f"Layer (Id: {item_id}) Can't Be Found")
+    
+    return gis_item
+
 def get_layer(gis, layer_id, number=None):
     """
     Find Layer from its id
     
     Parameters:
         - gis: GIS object logged in where to search from
         - layer_id: ID of the asked layer
         - number (Optional): Layer Number inside the item. If not provided
             it'll be assumed the item should only have 1 layer
     
     Returns the layer object inside the service
     """
-    layer_item = gis.content.get(layer_id)
-    if layer_item is None:
-        raise Exception(f"Layer (Id: {layer_id}) Can't Be Found")
+    layer_item = get_item(gis, layer_id)
     
     layers = layer_item.layers
     if len(layers) > 1 and number is None:
         raise Exception(f"Layer (Id: {layer_id}) Has Too Many Layers ({layers})")
     elif len(layers) == 0:
         raise Exception(f"Layer (Id: {layer_id}) Has NO Layers")
```

### Comparing `aeroterra_ds-1.0.9/src/layers/layers.py` & `aeroterra_ds-1.1.0/src/layers/layers.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 import geopandas as gpd
 import pandas as pd
 
-from arcgis.features import GeoAccessor, FeatureSet
+from arcgis.features import GeoAccessor, FeatureSet, Feature
 from arcgis.geometry.filters import intersects
 #TODO: Remove GeoAccessor
 
 from .common import get_layer, ordinal
-from .properties import get_layer_crs_aux, get_objectid_field_aux, get_objectid_field_aux, get_fields_aux
+from .properties import get_layer_crs_aux, get_objectid_field_aux, get_fields_aux, get_symbology_aux
+from .properties import get_pop_up, update_pop_up
 from geometry.geometry import create_geo_json
 
+BATCH_AMOUNT = 1000
+READ_BATCH = 10000
 
 def get_layer_in_list(layers_found, title):
     """
     Find Layer titled as title inside all the layers found
     
     Parameters:
         - layers_found: List of Items to check from
@@ -38,15 +41,15 @@
     Returns the sucess status of each add.
     """
     layer_crs = get_layer_crs_aux(layer)
     gdf_crs = gdf.crs
     if gdf_crs is None:
         raise Exception("GeoDataFrame Must Have A CRS Assigned")
     elif gdf_crs != layer_crs:
-        new_gdf = gdf.to_crs(layer_crs, inplace=True)
+        new_gdf = gdf.to_crs(layer_crs, inplace=False)
     else:
         new_gdf = gdf.copy()
     
     return new_gdf
 
 
 def clone_layer(og_gis, og_id, new_gis, new_name=None):
@@ -60,38 +63,69 @@
         - og_id: id of the original layer
         - new_gis: GIS struct from the user that will own the new layer
         - new_name (Optional): Name to be assigned to the new layer, if None the
             original name will be conserved.
     
     Returns the new layer item.
     """
-    try:
-        old_item = og_gis.content.get(og_id)
-        old_layer = old_item.layers[0]
-    except:
-        raise Exception(f"Couldn't find layer {og_id} For {og_gis}")
-    
-    layer_content = old_layer.query().sdf
+    old_layer = get_layer(og_gis, og_id)
+
+    layer_content = read_full_layer_aux_sdf(old_layer)
+    object_id = get_objectid_field_aux(old_layer)
     if len(layer_content) == 0:
-        raise Exception("Can't Clone Empty Layer")
-    
-    title = old_item.title
+        layer_content = create_empty_gdf_aux(old_layer)
+    symbology = get_symbology_aux(old_layer)
+    layer_content = layer_content.drop(columns=[object_id])
+    if "SHAPE__Length" in layer_content.columns:
+        layer_content = layer_content.drop(columns=["SHAPE__Length"])
+    if "SHAPE__Area" in layer_content.columns:
+        layer_content = layer_content.drop(columns=["SHAPE__Area"])
+
+    title = og_gis.content.get(og_id).title
     if new_name is None:
         new_name = title
-    
+
     og_name = new_name
     names_matching = new_gis.content.search(f"title:{new_name}")
     i = 1
     while get_layer_in_list(names_matching, new_name) is not None:
         ord_i = ordinal(i)
         new_name = f"{og_name} ({ord_i} Copy)"
         names_matching = new_gis.content.search(f"title:{new_name}")
         i += 1
     
-    new_layer = layer_content.spatial.to_featurelayer(title=new_name, gis=new_gis)  
+    fields_ordered = []
+    fields_real = get_fields_aux(old_layer)
+    fields_real = [field[0] for field in fields_real]
+    for field in layer_content.columns:
+        if field in fields_real:
+            fields_ordered.append(field)
+    if "SHAPE" not in fields_ordered:
+        fields_ordered.append("SHAPE")
+    layer_content = layer_content[fields_ordered]
+    
+    end = BATCH_AMOUNT
+    if end < len(layer_content):
+        end = len(layer_content)
+        new_layer = layer_content[:end].spatial.to_featurelayer(title=new_name, gis=new_gis)
+    else:
+        new_layer = layer_content[:end].spatial.to_featurelayer(title=new_name, gis=new_gis)
+        missing_registers = layer_content[end:]
+        for i in range(0, len(missing_registers), BATCH_AMOUNT):
+            end = i + BATCH_AMOUNT
+            if i > len(missing_registers):
+                end = len(missing_registers)
+            new_layer.edit_features(adds = missing_registers[i: end])
+
+    symbology_dict = {"drawingInfo": dict(symbology)}
+    ret_sym = new_layer.layers[0].manager.update_definition(symbology_dict)
+
+    pop_up = get_pop_up(og_gis, og_id)
+    update_pop_up(new_gis, new_layer.id, 0, pop_up)
+
     return new_layer
 
 
 def create_layer(gdf, gis, title=None, folder=None):
     """
     Given a geodataframe it creates a feature layer with its data in a new item
     
@@ -99,17 +133,26 @@
         - gdf: GeoDataFrame to publish
         - gis: GIS struct from the user that will own the new layer
         - title (Optional): Name to be given to the layer
         - folder (Optional): Folder in the portal where to store the layer
     
     Returns the new layer item.
     """
-    sdf = GeoAccessor.from_geodataframe(gdf)
-    
+    end = BATCH_AMOUNT
+    if end > len(gdf):
+        end = len(gdf)
+
+    sdf = GeoAccessor.from_geodataframe(gdf[:end])
+
     layer = sdf.spatial.to_featurelayer(gis=gis, title=title, folder=folder)
+
+    if end == len(gdf):
+        return layer
+
+    add_to_layer(gdf[end:], gis, layer.id)
     
     return layer
 
 
 def add_to_layer(gdf, gis, layer_id):
     """
     Given a geodataframe it adds all its features to a layer
@@ -122,15 +165,22 @@
     Returns the sucess status of each add.
     """
     layer = get_layer(gis, layer_id)
 
     gdf = change_gdf_to_layer_crs(gdf, layer)
         
     sdf = GeoAccessor.from_geodataframe(gdf)
-    return layer.edit_features(adds = sdf)
+    total = []
+    for i in range(0, len(sdf), BATCH_AMOUNT):
+        end = i + BATCH_AMOUNT
+        if i > len(sdf):
+            end = len(sdf)
+        total.append(layer.edit_features(adds = sdf[i: end]))
+                    
+    return total
 
 
 def update_layer(gdf, gis, layer_id, columns=None):
     """
     Given a geodataframe it updates the features asked in columns to a layer
     
     Parameters:
@@ -148,19 +198,39 @@
         if object_id_col not in columns:
             columns.append(object_id_col)
         gdf = gdf[columns]
     
     if object_id_col not in gdf.columns:
         raise Exception(f"{object_id_col} Must Be Present In GDF In Order To Know Which Line To Update")
 
-    gdf = change_gdf_to_layer_crs(gdf, layer)
-        
-    sdf = GeoAccessor.from_geodataframe(gdf)
-    feature_set = FeatureSet(sdf)
-    return layer.edit_features(updates = feature_set)
+    if "geometry" in gdf.columns:
+        gdf = change_gdf_to_layer_crs(gdf, layer)
+        gdf = GeoAccessor.from_geodataframe(gdf)
+
+    feature_set = FeatureSet(features=[])
+
+    for index, row in gdf.iterrows():
+        if "geometry" in gdf.columns:
+            data = row.to_dict()
+            geo = data.pop("geometry")
+            feature = Feature(attributes=data, geometry=geo)
+        else:
+            data = row.to_dict()
+            feature = Feature(attributes=data, geometry=None)
+            
+        feature_set.features.append(feature)
+    
+    total = []
+    for i in range(0, len(feature_set), BATCH_AMOUNT):
+        end = i + BATCH_AMOUNT
+        if i > len(feature_set):
+            end = len(feature_set)
+        total.append(layer.edit_features(updates = feature_set[i: end]))
+
+    return total
 
 
 def empty_layer(gis, layer_id):
     """
     Empty the data from a layer
     
     Parameters:
@@ -215,50 +285,82 @@
             the one of the layer will be used
     """
     layer = get_layer(gis, layer_id)
     
     return create_empty_gdf_aux(layer, crs)
 
 
-def read_full_layer(gis, layer_id, out_crs=None):
+def read_full_layer_aux_sdf(layer, out_crs=None):
     """
     Returns the full data stored in an asked layer.
     
     Parameters:
-        - gis: GIS struct from the user that owns the layer
-        - layer_id: Layer ID of the layer wanting to be asked
+        - layer: Layer wanting to be asked
         - out_crs (Optional): Wanted CRS of the returned GeoDataFrame. If not
             loaded, it'll be returned in the one of the layer.
 
-    Returns a GeoDataFrame
+    Returns a SDF
     """
-    layer = get_layer(gis, layer_id)
     object_id_col = get_objectid_field_aux(layer)
 
     total_data = None
     if out_crs is None:
         out_crs = get_layer_crs_aux(layer)
-    new_data = layer.query(out_sr=out_crs).sdf
+    new_data = layer.query(out_sr=out_crs, result_record_count=READ_BATCH, return_all_records=False).sdf
     while len(new_data) > 0:
         if total_data is None:
             total_data = new_data.copy()
         else:
             total_data = pd.concat([total_data, new_data])
 
         last_time = new_data[object_id_col].max()
         new_where = f"{object_id_col} > {last_time}"
-        new_data = layer.query(where = new_where, out_sr=out_crs).sdf
+        new_data = layer.query(where = new_where, out_sr=out_crs, result_record_count=READ_BATCH, return_all_records=False).sdf
 
     if total_data is None:
         return create_empty_gdf_aux(layer, crs=out_crs)
 
+    return total_data
+
+
+def read_full_layer_aux(layer, out_crs=None):
+    """
+    Returns the full data stored in an asked layer.
+    
+    Parameters:
+        - layer: Layer wanting to be asked
+        - out_crs (Optional): Wanted CRS of the returned GeoDataFrame. If not
+            loaded, it'll be returned in the one of the layer.
+
+    Returns a GeoDataFrame
+    """
+    if out_crs is None:
+        out_crs = get_layer_crs_aux(layer)
+    total_data = read_full_layer_aux_sdf(layer, out_crs=out_crs)
     total_data = total_data.rename(columns = {"SHAPE": "geometry"})
     return gpd.GeoDataFrame(total_data, geometry="geometry", crs=out_crs)
 
 
+def read_full_layer(gis, layer_id, out_crs=None):
+    """
+    Returns the full data stored in an asked layer.
+    
+    Parameters:
+        - gis: GIS struct from the user that owns the layer
+        - layer_id: Layer ID of the layer wanting to be asked
+        - out_crs (Optional): Wanted CRS of the returned GeoDataFrame. If not
+            loaded, it'll be returned in the one of the layer.
+
+    Returns a GeoDataFrame
+    """
+    layer = get_layer(gis, layer_id)
+
+    return read_full_layer_aux(layer)
+
+
 def read_layer_gdf(gis, layer_id, number=None, query=None, geometry_filter=None, geometry_crs=4326, out_fields=None, out_crs=None):
     """
     Returns the full data stored in an asked layer.
     
     Parameters:
         - gis: GIS struct from the user that owns the layer
         - layer_id: Layer ID of the layer wanting to be asked
@@ -288,26 +390,35 @@
     object_id_col = get_objectid_field_aux(layer)
     
     basic_where = query
     if out_fields is None:
        out_fields = "*"
 
     total_data = None
-    new_data = layer.query(where = basic_where, geometry_filter=geo_filter, out_fields=out_fields, out_sr=out_crs).sdf
+    new_data = layer.query(where = basic_where, geometry_filter=geo_filter, out_fields=out_fields, out_sr=out_crs, result_record_count=READ_BATCH, return_all_records=False).sdf
     while len(new_data) > 0:
         if total_data is None:
             total_data = new_data.copy()
         else:
             total_data = pd.concat([total_data, new_data])
 
         last_time = new_data[object_id_col].max()
         if query:
             new_where = basic_where + f" AND {object_id_col} > {last_time}"
         else:
             new_where = f"{object_id_col} > {last_time}"
-        new_data = layer.query(where = new_where, geometry_filter=geo_filter, out_fields=out_fields, out_sr=out_crs).sdf
+        new_data = layer.query(where = new_where, geometry_filter=geo_filter, out_fields=out_fields, out_sr=out_crs, result_record_count=READ_BATCH, return_all_records=False).sdf
 
     if total_data is None:
-        return create_empty_gdf_aux(layer)
+        total_data = create_empty_gdf_aux(layer, crs=out_crs)
+        if isinstance(out_fields, list):
+            out_fields.append("SHAPE")
+            total_data = total_data[out_fields]
+        total_data = total_data.rename(columns = {"SHAPE": "geometry"})
+        return total_data
+
+    if out_fields != "*" and object_id_col not in out_fields:
+        total_data = total_data.drop(columns=[object_id_col])
 
     total_data = total_data.rename(columns = {"SHAPE": "geometry"})
     return gpd.GeoDataFrame(total_data, geometry="geometry", crs=out_crs)
+
```

### Comparing `aeroterra_ds-1.0.9/src/layers/symbology.py` & `aeroterra_ds-1.1.0/src/layers/symbology.py`

 * *Files identical despite different names*

