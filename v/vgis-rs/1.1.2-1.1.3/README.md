# Comparing `tmp/vgis_rs-1.1.2.tar.gz` & `tmp/vgis_rs-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\vgis_rs-1.1.2.tar", last modified: Thu Jan 11 10:01:47 2024, max compression
+gzip compressed data, was "dist\vgis_rs-1.1.3.tar", last modified: Thu May 23 08:05:00 2024, max compression
```

## Comparing `vgis_rs-1.1.2.tar` & `vgis_rs-1.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-01-11 10:01:47.315983 vgis_rs-1.1.2/
--rw-rw-rw-   0        0        0      976 2024-01-11 10:01:47.314984 vgis_rs-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      116 2023-09-25 02:55:06.000000 vgis_rs-1.1.2/README.md
--rw-rw-rw-   0        0        0       42 2024-01-11 10:01:47.315983 vgis_rs-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0     2173 2024-01-11 10:01:00.000000 vgis_rs-1.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-01-11 10:01:47.270984 vgis_rs-1.1.2/vgis_rs/
--rw-rw-rw-   0        0        0      202 2023-06-27 07:32:13.000000 vgis_rs-1.1.2/vgis_rs/__init__.py
--rw-rw-rw-   0        0        0    15124 2024-01-11 10:00:52.000000 vgis_rs-1.1.2/vgis_rs/rsTools.py
--rw-rw-rw-   0        0        0     3814 2023-09-25 02:59:59.000000 vgis_rs-1.1.2/vgis_rs/tifTools.py
-drwxrwxrwx   0        0        0        0 2024-01-11 10:01:47.313013 vgis_rs-1.1.2/vgis_rs.egg-info/
--rw-rw-rw-   0        0        0      976 2024-01-11 10:01:47.000000 vgis_rs-1.1.2/vgis_rs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      231 2024-01-11 10:01:47.000000 vgis_rs-1.1.2/vgis_rs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-11 10:01:47.000000 vgis_rs-1.1.2/vgis_rs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-01-11 10:01:47.000000 vgis_rs-1.1.2/vgis_rs.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-01-11 10:01:47.000000 vgis_rs-1.1.2/vgis_rs.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-23 08:05:00.932397 vgis_rs-1.1.3/
+-rw-rw-rw-   0        0        0      976 2024-05-23 08:05:00.932397 vgis_rs-1.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      116 2023-09-25 02:55:06.000000 vgis_rs-1.1.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-23 08:05:00.932397 vgis_rs-1.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     2173 2024-05-23 08:04:37.000000 vgis_rs-1.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 08:05:00.923397 vgis_rs-1.1.3/vgis_rs/
+-rw-rw-rw-   0        0        0      202 2023-06-27 07:32:13.000000 vgis_rs-1.1.3/vgis_rs/__init__.py
+-rw-rw-rw-   0        0        0    15308 2024-05-23 08:04:06.000000 vgis_rs-1.1.3/vgis_rs/rsTools.py
+-rw-rw-rw-   0        0        0     3814 2023-09-25 02:59:59.000000 vgis_rs-1.1.3/vgis_rs/tifTools.py
+drwxrwxrwx   0        0        0        0 2024-05-23 08:05:00.930396 vgis_rs-1.1.3/vgis_rs.egg-info/
+-rw-rw-rw-   0        0        0      976 2024-05-23 08:05:00.000000 vgis_rs-1.1.3/vgis_rs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      231 2024-05-23 08:05:00.000000 vgis_rs-1.1.3/vgis_rs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 08:05:00.000000 vgis_rs-1.1.3/vgis_rs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-05-23 08:05:00.000000 vgis_rs-1.1.3/vgis_rs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-23 08:05:00.000000 vgis_rs-1.1.3/vgis_rs.egg-info/top_level.txt
```

### Comparing `vgis_rs-1.1.2/PKG-INFO` & `vgis_rs-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vgis_rs
-Version: 1.1.2
+Version: 1.1.3
 Summary: A libary for rs operator
 Home-page: https://github.com/gisfanmachel/vgisRs
 Author: gisfanmachel
 Author-email: gisfanmachel@gmail.com
 License: UNKNOWN
 Keywords: rs,setuptools,development
 Platform: UNKNOWN
```

### Comparing `vgis_rs-1.1.2/setup.py` & `vgis_rs-1.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 # Arguments marked as "Required" below must be included for upload to PyPI.
 # Fields marked as "Optional" may be commented out.
 
 setup(
 
     name="vgis_rs",  # Required 项目名称
-    version="1.1.2",  # Required 发布版本号
+    version="1.1.3",  # Required 发布版本号
     description="A libary for rs operator",  # Optional 项目简单描述
     long_description=long_description,  # Optional 详细描述
     long_description_content_type="text/markdown",  # 内容类型
     url="https://github.com/gisfanmachel/vgisRs",  # Optional github项目地址
     author="gisfanmachel",  # Optional 作者
     author_email="gisfanmachel@gmail.com",  # Optional 作者邮箱
     classifiers=[  # Optional 分类器通过对项目进行分类来帮助用户找到项目, 以下除了python版本其他的 不需要改动
```

### Comparing `vgis_rs-1.1.2/vgis_rs/rsTools.py` & `vgis_rs-1.1.3/vgis_rs/rsTools.py`

 * *Files 5% similar despite different names*

```diff
@@ -314,17 +314,21 @@
 
     @staticmethod
     # 用shp裁剪栅格文件
     # 需要gdal命令环境
     # 如果被裁切的影像没有坐标系，则裁切矢量也需要没有坐标系
     # 如果被裁切的影像有坐标系，则裁切矢量可以有也可以没有坐标系
     # 如果不是png或jpg,还需要生成pgw，jgw世界投影文件
-    def clip_raster_by_shape(input_raster_path, clip_shp_path, out_raster_path):
+    def clip_raster_by_shape(input_raster_path, clip_shp_path, out_raster_path, s_srs=None, t_srs=None):
         cmd_str = "gdalwarp -cutline {} -crop_to_cutline {} {}".format(clip_shp_path, input_raster_path,
                                                                        out_raster_path)
+        if s_srs is not None:
+            cmd_str+=" -s_srs {}".format(s_srs)
+        if t_srs is not None:
+            cmd_str+=" -t_srs {}".format(t_srs)
         print(cmd_str)
         os.system(cmd_str)
 
         # 针对不是tif的栅格文件，需要补充生成world投影文件
         file_pre_path, file_name = os.path.split(out_raster_path)
         shotname, suffix = os.path.splitext(file_name)
         if suffix.lower() != ".tif" or suffix.lower() != ".tiff" or suffix.lower() != ".geotiff":
```

### Comparing `vgis_rs-1.1.2/vgis_rs/tifTools.py` & `vgis_rs-1.1.3/vgis_rs/tifTools.py`

 * *Files identical despite different names*

### Comparing `vgis_rs-1.1.2/vgis_rs.egg-info/PKG-INFO` & `vgis_rs-1.1.3/vgis_rs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vgis-rs
-Version: 1.1.2
+Version: 1.1.3
 Summary: A libary for rs operator
 Home-page: https://github.com/gisfanmachel/vgisRs
 Author: gisfanmachel
 Author-email: gisfanmachel@gmail.com
 License: UNKNOWN
 Keywords: rs,setuptools,development
 Platform: UNKNOWN
```

