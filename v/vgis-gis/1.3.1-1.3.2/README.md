# Comparing `tmp/vgis_gis-1.3.1.tar.gz` & `tmp/vgis_gis-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\vgis_gis-1.3.1.tar", last modified: Thu May 23 06:52:57 2024, max compression
+gzip compressed data, was "dist\vgis_gis-1.3.2.tar", last modified: Thu May 23 07:19:09 2024, max compression
```

## Comparing `vgis_gis-1.3.1.tar` & `vgis_gis-1.3.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 06:52:57.179441 vgis_gis-1.3.1/
--rw-rw-rw-   0        0        0      981 2024-05-23 06:52:57.178451 vgis_gis-1.3.1/PKG-INFO
--rw-rw-rw-   0        0        0      117 2023-09-25 02:35:06.000000 vgis_gis-1.3.1/README.md
--rw-rw-rw-   0        0        0       42 2024-05-23 06:52:57.179441 vgis_gis-1.3.1/setup.cfg
--rw-rw-rw-   0        0        0     2189 2024-05-23 06:51:44.000000 vgis_gis-1.3.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-23 06:52:57.168468 vgis_gis-1.3.1/vgis_gis/
--rw-rw-rw-   0        0        0    10927 2023-12-21 07:26:16.000000 vgis_gis-1.3.1/vgis_gis/PoiTools.py
--rw-rw-rw-   0        0        0      202 2023-06-27 07:32:12.000000 vgis_gis-1.3.1/vgis_gis/__init__.py
--rw-rw-rw-   0        0        0     1491 2023-09-25 02:57:23.000000 vgis_gis-1.3.1/vgis_gis/arcgisTools.py
--rw-rw-rw-   0        0        0     3475 2021-08-30 10:03:04.000000 vgis_gis-1.3.1/vgis_gis/coordTools.py
--rw-rw-rw-   0        0        0     5166 2023-12-05 05:41:00.000000 vgis_gis-1.3.1/vgis_gis/geocodeTools.py
--rw-rw-rw-   0        0        0     3909 2024-03-22 01:58:29.000000 vgis_gis-1.3.1/vgis_gis/geojsonTools.py
--rw-rw-rw-   0        0        0    13904 2023-10-27 02:59:01.000000 vgis_gis-1.3.1/vgis_gis/geoserverTools.py
--rw-rw-rw-   0        0        0    23633 2024-05-23 06:51:32.000000 vgis_gis-1.3.1/vgis_gis/gisTools.py
--rw-rw-rw-   0        0        0     2581 2023-06-13 09:19:32.000000 vgis_gis-1.3.1/vgis_gis/projTools.py
--rw-rw-rw-   0        0        0      216 2021-11-05 05:26:50.000000 vgis_gis-1.3.1/vgis_gis/qgisTools.py
--rw-rw-rw-   0        0        0    71648 2024-03-20 07:15:51.000000 vgis_gis-1.3.1/vgis_gis/shpTools.py
-drwxrwxrwx   0        0        0        0 2024-05-23 06:52:57.176450 vgis_gis-1.3.1/vgis_gis.egg-info/
--rw-rw-rw-   0        0        0      981 2024-05-23 06:52:57.000000 vgis_gis-1.3.1/vgis_gis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      429 2024-05-23 06:52:57.000000 vgis_gis-1.3.1/vgis_gis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 06:52:57.000000 vgis_gis-1.3.1/vgis_gis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2024-05-23 06:52:57.000000 vgis_gis-1.3.1/vgis_gis.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-23 06:52:57.000000 vgis_gis-1.3.1/vgis_gis.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-23 07:19:09.398617 vgis_gis-1.3.2/
+-rw-rw-rw-   0        0        0      981 2024-05-23 07:19:09.397617 vgis_gis-1.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0      117 2023-09-25 02:35:06.000000 vgis_gis-1.3.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-23 07:19:09.398617 vgis_gis-1.3.2/setup.cfg
+-rw-rw-rw-   0        0        0     2189 2024-05-23 07:18:47.000000 vgis_gis-1.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 07:19:09.386617 vgis_gis-1.3.2/vgis_gis/
+-rw-rw-rw-   0        0        0    10927 2023-12-21 07:26:16.000000 vgis_gis-1.3.2/vgis_gis/PoiTools.py
+-rw-rw-rw-   0        0        0      202 2023-06-27 07:32:12.000000 vgis_gis-1.3.2/vgis_gis/__init__.py
+-rw-rw-rw-   0        0        0     1491 2023-09-25 02:57:23.000000 vgis_gis-1.3.2/vgis_gis/arcgisTools.py
+-rw-rw-rw-   0        0        0     3475 2021-08-30 10:03:04.000000 vgis_gis-1.3.2/vgis_gis/coordTools.py
+-rw-rw-rw-   0        0        0     5166 2023-12-05 05:41:00.000000 vgis_gis-1.3.2/vgis_gis/geocodeTools.py
+-rw-rw-rw-   0        0        0     3909 2024-03-22 01:58:29.000000 vgis_gis-1.3.2/vgis_gis/geojsonTools.py
+-rw-rw-rw-   0        0        0    13904 2023-10-27 02:59:01.000000 vgis_gis-1.3.2/vgis_gis/geoserverTools.py
+-rw-rw-rw-   0        0        0    23633 2024-05-23 07:18:36.000000 vgis_gis-1.3.2/vgis_gis/gisTools.py
+-rw-rw-rw-   0        0        0     2581 2023-06-13 09:19:32.000000 vgis_gis-1.3.2/vgis_gis/projTools.py
+-rw-rw-rw-   0        0        0      216 2021-11-05 05:26:50.000000 vgis_gis-1.3.2/vgis_gis/qgisTools.py
+-rw-rw-rw-   0        0        0    71648 2024-03-20 07:15:51.000000 vgis_gis-1.3.2/vgis_gis/shpTools.py
+drwxrwxrwx   0        0        0        0 2024-05-23 07:19:09.396618 vgis_gis-1.3.2/vgis_gis.egg-info/
+-rw-rw-rw-   0        0        0      981 2024-05-23 07:19:09.000000 vgis_gis-1.3.2/vgis_gis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      429 2024-05-23 07:19:09.000000 vgis_gis-1.3.2/vgis_gis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 07:19:09.000000 vgis_gis-1.3.2/vgis_gis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2024-05-23 07:19:09.000000 vgis_gis-1.3.2/vgis_gis.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-23 07:19:09.000000 vgis_gis-1.3.2/vgis_gis.egg-info/top_level.txt
```

### Comparing `vgis_gis-1.3.1/PKG-INFO` & `vgis_gis-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vgis_gis
-Version: 1.3.1
+Version: 1.3.2
 Summary: A libary for gis operator
 Home-page: https://github.com/gisfanmachel/vgisGis
 Author: gisfanmachel
 Author-email: gisfanmachel@gmail.com
 License: UNKNOWN
 Keywords: gis,setuptools,development
 Platform: UNKNOWN
```

### Comparing `vgis_gis-1.3.1/setup.py` & `vgis_gis-1.3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 # Arguments marked as "Required" below must be included for upload to PyPI.
 # Fields marked as "Optional" may be commented out.
 
 setup(
 
     name="vgis_gis",  # Required 项目名称
-    version="1.3.1",  # Required 发布版本号
+    version="1.3.2",  # Required 发布版本号
 
     description="A libary for gis operator",  # Optional 项目简单描述
     long_description=long_description,  # Optional 详细描述
     long_description_content_type="text/markdown",  # 内容类型
     url="https://github.com/gisfanmachel/vgisGis",  # Optional github项目地址
     author="gisfanmachel",  # Optional 作者
     author_email="gisfanmachel@gmail.com",  # Optional 作者邮箱
```

### Comparing `vgis_gis-1.3.1/vgis_gis/PoiTools.py` & `vgis_gis-1.3.2/vgis_gis/PoiTools.py`

 * *Files identical despite different names*

### Comparing `vgis_gis-1.3.1/vgis_gis/arcgisTools.py` & `vgis_gis-1.3.2/vgis_gis/arcgisTools.py`

 * *Files identical despite different names*

### Comparing `vgis_gis-1.3.1/vgis_gis/coordTools.py` & `vgis_gis-1.3.2/vgis_gis/coordTools.py`

 * *Files identical despite different names*

### Comparing `vgis_gis-1.3.1/vgis_gis/geocodeTools.py` & `vgis_gis-1.3.2/vgis_gis/geocodeTools.py`

 * *Files identical despite different names*

### Comparing `vgis_gis-1.3.1/vgis_gis/geojsonTools.py` & `vgis_gis-1.3.2/vgis_gis/geojsonTools.py`

 * *Files identical despite different names*

### Comparing `vgis_gis-1.3.1/vgis_gis/geoserverTools.py` & `vgis_gis-1.3.2/vgis_gis/geoserverTools.py`

 * *Files identical despite different names*

### Comparing `vgis_gis-1.3.1/vgis_gis/gisTools.py` & `vgis_gis-1.3.2/vgis_gis/gisTools.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,15 +131,15 @@
     @staticmethod
     def convert_points_from_epsg(point_list, from_epsg, to_epsg):
         transformer = Transformer.from_crs("epsg:" + str(from_epsg), "epsg:" + str(to_epsg))
         new_point_list = []
         for point in point_list:
             x = point[0]
             y = point[1]
-            x2, y2 = transformer.transform(x, y)
+            y2, x2 = transformer.transform(y, x)
             new_point_list.append[[x2, y2]]
         return new_point_list
 
     # 4326坐标转3857坐标
     # point [[123.5,23.6]]
     @staticmethod
     def convert_point_from_wgs84_to_mercator(point):
```

### Comparing `vgis_gis-1.3.1/vgis_gis/projTools.py` & `vgis_gis-1.3.2/vgis_gis/projTools.py`

 * *Files identical despite different names*

### Comparing `vgis_gis-1.3.1/vgis_gis/shpTools.py` & `vgis_gis-1.3.2/vgis_gis/shpTools.py`

 * *Files identical despite different names*

### Comparing `vgis_gis-1.3.1/vgis_gis.egg-info/PKG-INFO` & `vgis_gis-1.3.2/vgis_gis.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vgis-gis
-Version: 1.3.1
+Version: 1.3.2
 Summary: A libary for gis operator
 Home-page: https://github.com/gisfanmachel/vgisGis
 Author: gisfanmachel
 Author-email: gisfanmachel@gmail.com
 License: UNKNOWN
 Keywords: gis,setuptools,development
 Platform: UNKNOWN
```

