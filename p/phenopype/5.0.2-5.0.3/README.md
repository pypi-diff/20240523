# Comparing `tmp/phenopype-5.0.2.tar.gz` & `tmp/phenopype-5.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phenopype-5.0.2.tar", last modified: Fri May 17 03:00:24 2024, max compression
+gzip compressed data, was "phenopype-5.0.3.tar", last modified: Thu May 23 06:13:53 2024, max compression
```

## Comparing `phenopype-5.0.2.tar` & `phenopype-5.0.3.tar`

### file list

```diff
@@ -1,53 +1,51 @@
-drwxrwxrwx   0        0        0        0 2024-05-17 03:00:24.093351 phenopype-5.0.2/
--rw-rw-rw-   0        0        0     7815 2022-11-18 08:20:39.000000 phenopype-5.0.2/LICENSE
--rw-rw-rw-   0        0        0       28 2022-11-18 08:20:39.000000 phenopype-5.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0    15259 2024-05-17 03:00:24.090843 phenopype-5.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     4998 2023-11-15 10:03:26.000000 phenopype-5.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-17 03:00:23.922610 phenopype-5.0.2/_temp/
-drwxrwxrwx   0        0        0        0 2024-05-17 03:00:23.952684 phenopype-5.0.2/_temp/docs/
--rw-rw-rw-   0        0        0     3201 2022-05-03 09:06:29.000000 phenopype-5.0.2/_temp/docs/conf.py
-drwxrwxrwx   0        0        0        0 2024-05-17 03:00:23.923607 phenopype-5.0.2/_temp/tests/
-drwxrwxrwx   0        0        0        0 2024-05-17 03:00:23.957251 phenopype-5.0.2/_temp/tests/phenopype-tutorials-main/
--rw-rw-rw-   0        0        0     3104 2024-05-17 02:51:10.000000 phenopype-5.0.2/_temp/tests/phenopype-tutorials-main/conf.py
-drwxrwxrwx   0        0        0        0 2024-05-17 03:00:23.959248 phenopype-5.0.2/docs_source/
--rw-rw-rw-   0        0        0     1893 2024-05-16 22:54:42.000000 phenopype-5.0.2/docs_source/conf.py
-drwxrwxrwx   0        0        0        0 2024-05-17 03:00:23.980432 phenopype-5.0.2/phenopype/
--rw-rw-rw-   0        0        0      771 2024-05-17 02:47:12.000000 phenopype-5.0.2/phenopype/__init__.py
--rw-rw-rw-   0        0        0     5795 2024-05-16 22:54:42.000000 phenopype-5.0.2/phenopype/_vars.py
--rw-rw-rw-   0        0        0       23 2024-05-15 03:57:51.000000 phenopype-5.0.2/phenopype/_version.py
-drwxrwxrwx   0        0        0        0 2024-05-17 03:00:24.011932 phenopype-5.0.2/phenopype/assets/
--rw-rw-rw-   0        0        0    53700 2022-11-18 08:20:40.000000 phenopype-5.0.2/phenopype/assets/wc3_colours.html
--rw-rw-rw-   0        0        0      425 2024-05-16 22:54:42.000000 phenopype-5.0.2/phenopype/config.py
-drwxrwxrwx   0        0        0        0 2024-05-17 03:00:24.044821 phenopype-5.0.2/phenopype/core/
--rw-rw-rw-   0        0        0       79 2022-11-18 08:20:40.000000 phenopype-5.0.2/phenopype/core/__init__.py
--rw-rw-rw-   0        0        0    33750 2024-05-16 22:54:42.000000 phenopype-5.0.2/phenopype/core/export.py
--rw-rw-rw-   0        0        0    21663 2024-05-16 22:54:42.000000 phenopype-5.0.2/phenopype/core/measurement.py
--rw-rw-rw-   0        0        0    35985 2024-05-17 02:30:39.000000 phenopype-5.0.2/phenopype/core/preprocessing.py
--rw-rw-rw-   0        0        0    39404 2024-05-16 22:54:42.000000 phenopype-5.0.2/phenopype/core/segmentation.py
--rw-rw-rw-   0        0        0    31067 2024-05-16 22:54:42.000000 phenopype-5.0.2/phenopype/core/visualization.py
--rw-rw-rw-   0        0        0     2626 2024-05-16 22:54:42.000000 phenopype-5.0.2/phenopype/decorators.py
--rw-rw-rw-   0        0        0   129201 2024-05-17 02:42:25.000000 phenopype-5.0.2/phenopype/main.py
--rw-rw-rw-   0        0        0    32999 2024-05-16 22:54:42.000000 phenopype-5.0.2/phenopype/tracking.py
--rw-rw-rw-   0        0        0    10541 2024-05-16 23:21:09.000000 phenopype-5.0.2/phenopype/utils.py
--rw-rw-rw-   0        0        0   111464 2024-05-17 02:42:14.000000 phenopype-5.0.2/phenopype/utils_lowlevel.py
-drwxrwxrwx   0        0        0        0 2024-05-17 03:00:24.085859 phenopype-5.0.2/phenopype.egg-info/
--rw-rw-rw-   0        0        0    15259 2024-05-17 03:00:23.000000 phenopype-5.0.2/phenopype.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1031 2024-05-17 03:00:23.000000 phenopype-5.0.2/phenopype.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 03:00:23.000000 phenopype-5.0.2/phenopype.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      187 2024-05-17 03:00:23.000000 phenopype-5.0.2/phenopype.egg-info/requires.txt
--rw-rw-rw-   0        0        0       59 2024-05-17 03:00:23.000000 phenopype-5.0.2/phenopype.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1172 2024-05-17 02:55:37.000000 phenopype-5.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-17 03:00:24.093351 phenopype-5.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-17 03:00:24.081107 phenopype-5.0.2/tests/
--rw-rw-rw-   0        0        0        0 2022-11-18 08:20:40.000000 phenopype-5.0.2/tests/__init__.py
--rw-rw-rw-   0        0        0     7326 2024-05-16 22:54:42.000000 phenopype-5.0.2/tests/conftest.py
--rw-rw-rw-   0        0        0     3044 2024-05-16 22:54:42.000000 phenopype-5.0.2/tests/test_01_project.py
--rw-rw-rw-   0        0        0     3603 2024-05-16 22:54:42.000000 phenopype-5.0.2/tests/test_02_core_preprocessing.py
--rw-rw-rw-   0        0        0     2495 2024-05-16 22:54:42.000000 phenopype-5.0.2/tests/test_03_core_segmentation.py
--rw-rw-rw-   0        0        0     1577 2024-05-16 22:54:42.000000 phenopype-5.0.2/tests/test_04_core_measurement.py
--rw-rw-rw-   0        0        0     3867 2024-05-16 22:54:42.000000 phenopype-5.0.2/tests/test_05_core_visualization.py
--rw-rw-rw-   0        0        0     3640 2024-05-16 22:54:42.000000 phenopype-5.0.2/tests/test_06_core_export.py
--rw-rw-rw-   0        0        0     1609 2024-05-16 22:54:42.000000 phenopype-5.0.2/tests/test_07_pype.py
--rw-rw-rw-   0        0        0     3654 2023-11-15 10:03:26.000000 phenopype-5.0.2/tests/test_08_tracking.py
--rw-rw-rw-   0        0        0     1061 2024-05-17 02:50:37.000000 phenopype-5.0.2/tests/test_09_utils.py
--rw-rw-rw-   0        0        0      312 2022-11-18 08:20:40.000000 phenopype-5.0.2/tests/test_10_utils_lowlevel.py
+drwxrwxrwx   0        0        0        0 2024-05-23 06:13:53.260023 phenopype-5.0.3/
+-rw-rw-rw-   0        0        0     7815 2022-04-25 22:33:40.000000 phenopype-5.0.3/LICENSE
+-rw-rw-rw-   0        0        0       28 2023-10-10 22:30:43.000000 phenopype-5.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0    15259 2024-05-23 06:13:53.259023 phenopype-5.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4998 2023-10-10 22:30:43.000000 phenopype-5.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-23 06:13:53.208702 phenopype-5.0.3/_temp/
+drwxrwxrwx   0        0        0        0 2024-05-23 06:13:53.208702 phenopype-5.0.3/_temp/tests/
+drwxrwxrwx   0        0        0        0 2024-05-23 06:13:53.216703 phenopype-5.0.3/_temp/tests/phenopype-tutorials-main/
+-rw-rw-rw-   0        0        0     3104 2024-05-23 06:11:37.000000 phenopype-5.0.3/_temp/tests/phenopype-tutorials-main/conf.py
+drwxrwxrwx   0        0        0        0 2024-05-23 06:13:53.217703 phenopype-5.0.3/docs_source/
+-rw-rw-rw-   0        0        0     2105 2024-05-23 06:00:08.000000 phenopype-5.0.3/docs_source/conf.py
+drwxrwxrwx   0        0        0        0 2024-05-23 06:13:53.225713 phenopype-5.0.3/phenopype/
+-rw-rw-rw-   0        0        0      771 2024-05-23 06:00:08.000000 phenopype-5.0.3/phenopype/__init__.py
+-rw-rw-rw-   0        0        0     5794 2024-05-23 06:00:08.000000 phenopype-5.0.3/phenopype/_vars.py
+-rw-rw-rw-   0        0        0       23 2023-11-20 09:20:30.000000 phenopype-5.0.3/phenopype/_version.py
+drwxrwxrwx   0        0        0        0 2024-05-23 06:13:53.240032 phenopype-5.0.3/phenopype/assets/
+-rw-rw-rw-   0        0        0    53700 2023-10-10 22:30:43.000000 phenopype-5.0.3/phenopype/assets/wc3_colours.html
+-rw-rw-rw-   0        0        0      425 2024-05-15 15:11:34.000000 phenopype-5.0.3/phenopype/config.py
+drwxrwxrwx   0        0        0        0 2024-05-23 06:13:53.245024 phenopype-5.0.3/phenopype/core/
+-rw-rw-rw-   0        0        0       79 2024-04-14 20:07:18.000000 phenopype-5.0.3/phenopype/core/__init__.py
+-rw-rw-rw-   0        0        0    34022 2024-05-23 06:00:08.000000 phenopype-5.0.3/phenopype/core/export.py
+-rw-rw-rw-   0        0        0    21663 2024-05-15 15:10:11.000000 phenopype-5.0.3/phenopype/core/measurement.py
+-rw-rw-rw-   0        0        0    35985 2024-05-23 06:00:08.000000 phenopype-5.0.3/phenopype/core/preprocessing.py
+-rw-rw-rw-   0        0        0    39404 2024-05-16 15:29:59.000000 phenopype-5.0.3/phenopype/core/segmentation.py
+-rw-rw-rw-   0        0        0    31069 2024-05-23 06:00:08.000000 phenopype-5.0.3/phenopype/core/visualization.py
+-rw-rw-rw-   0        0        0     2626 2024-05-15 15:10:11.000000 phenopype-5.0.3/phenopype/decorators.py
+-rw-rw-rw-   0        0        0   129246 2024-05-23 06:00:08.000000 phenopype-5.0.3/phenopype/main.py
+-rw-rw-rw-   0        0        0    32999 2024-05-15 15:10:11.000000 phenopype-5.0.3/phenopype/tracking.py
+-rw-rw-rw-   0        0        0    10785 2024-05-23 06:00:08.000000 phenopype-5.0.3/phenopype/utils.py
+-rw-rw-rw-   0        0        0   111674 2024-05-23 06:00:08.000000 phenopype-5.0.3/phenopype/utils_lowlevel.py
+drwxrwxrwx   0        0        0        0 2024-05-23 06:13:53.257023 phenopype-5.0.3/phenopype.egg-info/
+-rw-rw-rw-   0        0        0    15259 2024-05-23 06:13:53.000000 phenopype-5.0.3/phenopype.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1012 2024-05-23 06:13:53.000000 phenopype-5.0.3/phenopype.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 06:13:53.000000 phenopype-5.0.3/phenopype.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      187 2024-05-23 06:13:53.000000 phenopype-5.0.3/phenopype.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       65 2024-05-23 06:13:53.000000 phenopype-5.0.3/phenopype.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1172 2024-05-23 06:02:31.000000 phenopype-5.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-23 06:13:53.260023 phenopype-5.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-23 06:13:53.256024 phenopype-5.0.3/tests/
+-rw-rw-rw-   0        0        0        0 2022-04-25 22:33:41.000000 phenopype-5.0.3/tests/__init__.py
+-rw-rw-rw-   0        0        0     7326 2024-05-15 15:10:11.000000 phenopype-5.0.3/tests/conftest.py
+-rw-rw-rw-   0        0        0     3044 2024-05-15 15:10:11.000000 phenopype-5.0.3/tests/test_01_project.py
+-rw-rw-rw-   0        0        0     3603 2024-05-15 15:10:11.000000 phenopype-5.0.3/tests/test_02_core_preprocessing.py
+-rw-rw-rw-   0        0        0     2495 2024-05-15 15:10:11.000000 phenopype-5.0.3/tests/test_03_core_segmentation.py
+-rw-rw-rw-   0        0        0     1577 2024-05-15 15:10:11.000000 phenopype-5.0.3/tests/test_04_core_measurement.py
+-rw-rw-rw-   0        0        0     3867 2024-05-15 15:10:11.000000 phenopype-5.0.3/tests/test_05_core_visualization.py
+-rw-rw-rw-   0        0        0     3640 2024-05-15 15:10:11.000000 phenopype-5.0.3/tests/test_06_core_export.py
+-rw-rw-rw-   0        0        0     1609 2024-05-15 15:10:11.000000 phenopype-5.0.3/tests/test_07_pype.py
+-rw-rw-rw-   0        0        0     3654 2023-10-10 22:30:43.000000 phenopype-5.0.3/tests/test_08_tracking.py
+-rw-rw-rw-   0        0        0     1061 2024-05-23 06:00:08.000000 phenopype-5.0.3/tests/test_09_utils.py
+-rw-rw-rw-   0        0        0      312 2022-04-25 22:33:41.000000 phenopype-5.0.3/tests/test_10_utils_lowlevel.py
```

### Comparing `phenopype-5.0.2/LICENSE` & `phenopype-5.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `phenopype-5.0.2/PKG-INFO` & `phenopype-5.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phenopype
-Version: 5.0.2
+Version: 5.0.3
 Summary: A phenotyping pipeline for python
 Author-email: Moritz Luerig <moritz.luerig@gmail.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `phenopype-5.0.2/README.md` & `phenopype-5.0.3/README.md`

 * *Files identical despite different names*

### Comparing `phenopype-5.0.2/_temp/tests/phenopype-tutorials-main/conf.py` & `phenopype-5.0.3/_temp/tests/phenopype-tutorials-main/conf.py`

 * *Files identical despite different names*

### Comparing `phenopype-5.0.2/docs_source/conf.py` & `phenopype-5.0.3/docs_source/conf.py`

 * *Files 19% similar despite different names*

```diff
@@ -34,16 +34,27 @@
 suppress_warnings = [
     'autosectionlabel.*',
     'mystnb.nbcell',
     'myst.header',
     'myst.strikethrough',
 ]
 myst_enable_extensions = [
-    'colon_fence',
-    'strikethrough',
+    "amsmath",
+    "attrs_inline",
+    "colon_fence",
+    "deflist",
+    "dollarmath",
+    "fieldlist",
+    "html_admonition",
+    "html_image",
+    "replacements",
+    "smartquotes",
+    "strikethrough",
+    "substitution",
+    "tasklist",
 ]
 
 myst_heading_anchors = 3
 nb_execution_mode = 'off'
 # nb_remove_code_outputs = True
 
 master_doc = 'index'
```

### Comparing `phenopype-5.0.2/phenopype/__init__.py` & `phenopype-5.0.3/phenopype/__init__.py`

 * *Files identical despite different names*

### Comparing `phenopype-5.0.2/phenopype/_vars.py` & `phenopype-5.0.3/phenopype/_vars.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 confirm_options = ["True", "true", "y", "yes", True]
 
 _default_label_colour = "red"
 _default_line_colour = "lime"
 _default_node_colour = "red"
 _default_point_colour = "red"
-_default_overlay_colour_left = "green"
+_default_overlay_colour_left = "lime"
 _default_overlay_colour_right = "red"
 
 
 default_filetypes = ["jpg", "JPG", "jpeg", "JPEG", "tif", "png", "bmp"]
 default_meta_data_fields = [
     "DateTimeOriginal",
     "Model",
```

### Comparing `phenopype-5.0.2/phenopype/assets/wc3_colours.html` & `phenopype-5.0.3/phenopype/assets/wc3_colours.html`

 * *Files identical despite different names*

### Comparing `phenopype-5.0.2/phenopype/core/export.py` & `phenopype-5.0.3/phenopype/core/export.py`

 * *Files 0% similar despite different names*

```diff
@@ -706,15 +706,31 @@
         annotations=annotations,
         annotation_type=annotation_type,
         annotation_id=annotation_id,
         kwargs=kwargs,
     )
 
     data = annotation["data"][annotation_type]
-
+    
+    # =============================================================================
+    # prep save
+    
+    ## add suffix 
+    if suffix is None:
+        suffix = ""
+    else:
+        suffix = "_" + suffix
+        
+    ## add extension
+    if "." not in ext:
+        ext = "." + ext
+        
+    # =============================================================================
+    # run
+    
     if which == "max":
         area = list()
         for idx, roi_coords in enumerate(data):
     
             if annotation_type == _vars._mask_type:
                 coords = ul._convert_tup_list_arr(roi_coords)[0]
             else:
@@ -825,39 +841,33 @@
         if background=="original":           
             pass
         else:
             if background=="transparent":           
                 roi_alpha = np.zeros((roi.shape[0], roi.shape[1], 4), dtype=np.uint8)
                 roi_alpha[:,:,0:3] = roi
                 roi_alpha[:, :, 3] = roi_mask
+                roi_canvas = roi_alpha
+                ext = ".png"
             else:
                 roi[roi_mask==0] = ul._get_bgr(background)
+                roi_canvas = roi
             roi = roi_canvas
                 
+                
         # =============================================================================
         ## resizing final ROI
         
         if max_dim:
             roi = utils.resize_image(roi, max_dim=max_dim)
             
         # =============================================================================
         ## saving          
                 
         if not kwargs.get("training_data"):
-            
-            ## add suffix 
-            if suffix is None:
-                suffix = ""
-            else:
-                suffix = "_" + suffix
-                
-            ## add extension
-            if "." not in ext:
-                ext = "." + ext
-                 
+                             
             ## add counter
             if counter:
                 roi_name = file_name + suffix + "_" + str(idx+1).zfill(3) + ext
             else:
                 roi_name = file_name + suffix + ext
```

### Comparing `phenopype-5.0.2/phenopype/core/measurement.py` & `phenopype-5.0.3/phenopype/core/measurement.py`

 * *Files identical despite different names*

### Comparing `phenopype-5.0.2/phenopype/core/preprocessing.py` & `phenopype-5.0.3/phenopype/core/preprocessing.py`

 * *Files identical despite different names*

### Comparing `phenopype-5.0.2/phenopype/core/segmentation.py` & `phenopype-5.0.3/phenopype/core/segmentation.py`

 * *Files identical despite different names*

### Comparing `phenopype-5.0.2/phenopype/core/visualization.py` & `phenopype-5.0.3/phenopype/core/visualization.py`

 * *Files 0% similar despite different names*

```diff
@@ -896,15 +896,15 @@
     Returns
     -------
     canvas : ndarray
         canvas for drawing
 
     """
 
-    if image.__class__.__name__ == "Container":
+    if image.__class__.__name__ == "_Container":
         
         ## method
         if canvas == "mod":
             image.canvas = copy.deepcopy(image.image)
             ul._print("- modifed image")
         elif canvas == "raw":
             image.canvas = copy.deepcopy(image.image_copy)
@@ -955,15 +955,15 @@
             
         if invert == True:
             canvas = cv2.bitwise_not(canvas)
             ul._print("- inverted image")
 
     ## check if colour
     if multi_channel:
-        if image.__class__.__name__ == "Container":
+        if image.__class__.__name__ == "_Container":
             if len(image.canvas.shape) < 3:
                 image.canvas = cv2.cvtColor(image.canvas, cv2.COLOR_GRAY2BGR)
         elif image.__class__.__name__ == "ndarray":
             if len(canvas.shape) < 3:
                 canvas = cv2.cvtColor(canvas, cv2.COLOR_GRAY2BGR)
                 
     return canvas
```

### Comparing `phenopype-5.0.2/phenopype/decorators.py` & `phenopype-5.0.3/phenopype/decorators.py`

 * *Files identical despite different names*

### Comparing `phenopype-5.0.2/phenopype/main.py` & `phenopype-5.0.3/phenopype/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -6367,1710 +6367,1712 @@
 00018de0: 2020 2066 6565 6462 6163 6b3d 5472 7565     feedback=True
 00018df0: 2c0d 0a20 2020 2020 2020 2061 7574 6f6c  ,..        autol
 00018e00: 6f61 643d 5472 7565 2c0d 0a20 2020 2020  oad=True,..     
 00018e10: 2020 2061 7574 6f73 6176 653d 5472 7565     autosave=True
 00018e20: 2c0d 0a20 2020 2020 2020 2061 7574 6f73  ,..        autos
 00018e30: 686f 773d 5472 7565 2c0d 0a20 2020 2020  how=True,..     
 00018e40: 2020 206c 6f67 5f6f 773d 4661 6c73 652c     log_ow=False,
-00018e50: 0d0a 2020 2020 2020 2020 636f 6e66 6967  ..        config
-00018e60: 5f70 6174 683d 4e6f 6e65 2c0d 0a20 2020  _path=None,..   
-00018e70: 2020 2020 2066 6978 5f6e 616d 6573 3d54       fix_names=T
-00018e80: 7275 652c 0d0a 2020 2020 2020 2020 6c6f  rue,..        lo
-00018e90: 6164 5f63 6f6e 746f 7572 733d 4661 6c73  ad_contours=Fals
-00018ea0: 652c 0d0a 2020 2020 2020 2020 7a6f 6f6d  e,..        zoom
-00018eb0: 5f6d 656d 6f72 793d 5472 7565 2c0d 0a20  _memory=True,.. 
-00018ec0: 2020 2020 2020 2064 6562 7567 3d46 616c         debug=Fal
-00018ed0: 7365 2c0d 0a20 2020 2020 2020 202a 2a6b  se,..        **k
-00018ee0: 7761 7267 730d 0a20 2020 2029 3a0d 0a0d  wargs..    ):...
-00018ef0: 0a20 2020 2020 2020 2023 203d 3d3d 3d3d  .        # =====
-00018f00: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00018f10: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00018e50: 0d0a 2020 2020 2020 2020 6469 725f 7061  ..        dir_pa
+00018e60: 7468 3d4e 6f6e 652c 0d0a 2020 2020 2020  th=None,..      
+00018e70: 2020 636f 6e66 6967 5f70 6174 683d 4e6f    config_path=No
+00018e80: 6e65 2c0d 0a20 2020 2020 2020 2066 6978  ne,..        fix
+00018e90: 5f6e 616d 6573 3d54 7275 652c 0d0a 2020  _names=True,..  
+00018ea0: 2020 2020 2020 6c6f 6164 5f63 6f6e 746f        load_conto
+00018eb0: 7572 733d 4661 6c73 652c 0d0a 2020 2020  urs=False,..    
+00018ec0: 2020 2020 7a6f 6f6d 5f6d 656d 6f72 793d      zoom_memory=
+00018ed0: 5472 7565 2c0d 0a20 2020 2020 2020 2064  True,..        d
+00018ee0: 6562 7567 3d46 616c 7365 2c0d 0a20 2020  ebug=False,..   
+00018ef0: 2020 2020 202a 2a6b 7761 7267 730d 0a20       **kwargs.. 
+00018f00: 2020 2029 3a0d 0a0d 0a20 2020 2020 2020     ):....       
+00018f10: 2023 203d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d   # =============
 00018f20: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 00018f30: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00018f40: 3d3d 3d3d 3d3d 3d3d 0d0a 2020 2020 2020  ========..      
-00018f50: 2020 2320 494e 4954 0d0a 0d0a 2020 2020    # INIT....    
-00018f60: 2020 2020 2323 206b 7761 7267 730d 0a20      ## kwargs.. 
-00018f70: 2020 2020 2020 2063 6f6e 6669 672e 7769         config.wi
-00018f80: 6e64 6f77 5f6d 696e 5f64 696d 203d 206b  ndow_min_dim = k
-00018f90: 7761 7267 732e 6765 7428 2277 696e 646f  wargs.get("windo
-00018fa0: 775f 6d61 785f 6469 6d22 2c20 636f 6e66  w_max_dim", conf
-00018fb0: 6967 2e77 696e 646f 775f 6d69 6e5f 6469  ig.window_min_di
-00018fc0: 6d29 0d0a 2020 2020 2020 2020 636f 6e66  m)..        conf
-00018fd0: 6967 2e77 696e 646f 775f 6d61 785f 6469  ig.window_max_di
-00018fe0: 6d20 3d20 6b77 6172 6773 2e67 6574 2822  m = kwargs.get("
-00018ff0: 7769 6e64 6f77 5f6d 6178 5f64 696d 222c  window_max_dim",
-00019000: 2063 6f6e 6669 672e 7769 6e64 6f77 5f6d   config.window_m
-00019010: 6178 5f64 696d 290d 0a20 2020 2020 2020  ax_dim)..       
-00019020: 2064 656c 6179 203d 206b 7761 7267 732e   delay = kwargs.
-00019030: 6765 7428 2264 656c 6179 222c 2031 3030  get("delay", 100
-00019040: 290d 0a20 2020 2020 2020 200d 0a20 2020  )..        ..   
-00019050: 2020 2020 2023 2320 666c 6167 730d 0a20       ## flags.. 
-00019060: 2020 2020 2020 2073 656c 662e 666c 6167         self.flag
-00019070: 7320 3d20 6d61 6b65 5f64 6174 6163 6c61  s = make_datacla
-00019080: 7373 280d 0a20 2020 2020 2020 2020 2020  ss(..           
-00019090: 2063 6c73 5f6e 616d 653d 2266 6c61 6773   cls_name="flags
-000190a0: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-000190b0: 6669 656c 6473 3d5b 0d0a 2020 2020 2020  fields=[..      
-000190c0: 2020 2020 2020 2020 2020 2822 6465 6275            ("debu
-000190d0: 6722 2c20 626f 6f6c 2c20 6465 6275 6729  g", bool, debug)
-000190e0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-000190f0: 2020 2028 2261 7574 6f6c 6f61 6422 2c20     ("autoload", 
-00019100: 626f 6f6c 2c20 6175 746f 6c6f 6164 292c  bool, autoload),
-00019110: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00019120: 2020 2822 6175 746f 7361 7665 222c 2062    ("autosave", b
-00019130: 6f6f 6c2c 2061 7574 6f73 6176 6529 2c0d  ool, autosave),.
-00019140: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00019150: 2028 2261 7574 6f73 686f 7722 2c20 626f   ("autoshow", bo
-00019160: 6f6c 2c20 6175 746f 7368 6f77 292c 0d0a  ol, autoshow),..
-00019170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019180: 2822 6665 6564 6261 636b 222c 2062 6f6f  ("feedback", boo
-00019190: 6c2c 2066 6565 6462 6163 6b29 2c0d 0a20  l, feedback),.. 
-000191a0: 2020 2020 2020 2020 2020 2020 2020 2028                 (
-000191b0: 2269 6e74 6572 6163 7469 7665 222c 2062  "interactive", b
-000191c0: 6f6f 6c2c 2069 6e74 6572 6163 7469 7665  ool, interactive
-000191d0: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
-000191e0: 2020 2020 2822 6669 785f 6e61 6d65 7322      ("fix_names"
-000191f0: 2c20 626f 6f6c 2c20 6669 785f 6e61 6d65  , bool, fix_name
-00019200: 7329 2c0d 0a20 2020 2020 2020 2020 2020  s),..           
-00019210: 2020 2020 2028 2273 6b69 7022 2c20 626f       ("skip", bo
-00019220: 6f6c 2c20 736b 6970 292c 0d0a 2020 2020  ol, skip),..    
-00019230: 2020 2020 2020 2020 2020 2020 2822 7a6f              ("zo
-00019240: 6f6d 5f6d 656d 6f72 7922 2c20 626f 6f6c  om_memory", bool
-00019250: 2c20 7a6f 6f6d 5f6d 656d 6f72 7929 2c0d  , zoom_memory),.
-00019260: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00019270: 2028 2264 7279 5f72 756e 222c 2062 6f6f   ("dry_run", boo
-00019280: 6c2c 206b 7761 7267 732e 6765 7428 2264  l, kwargs.get("d
-00019290: 7279 5f72 756e 222c 2046 616c 7365 2929  ry_run", False))
-000192a0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-000192b0: 2020 2028 2274 6572 6d69 6e61 7465 222c     ("terminate",
-000192c0: 2062 6f6f 6c2c 2046 616c 7365 292c 0d0a   bool, False),..
-000192d0: 2020 2020 2020 2020 2020 2020 5d2c 0d0a              ],..
-000192e0: 2020 2020 2020 2020 290d 0a20 2020 2020          )..     
-000192f0: 2020 200d 0a20 2020 2020 2020 2069 6620     ..        if 
-00019300: 7365 6c66 2e66 6c61 6773 2e64 6562 7567  self.flags.debug
-00019310: 3a0d 0a20 2020 2020 2020 2020 2020 200d  :..            .
-00019320: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00019330: 662e 7665 7262 6f73 6520 3d20 636f 6e66  f.verbose = conf
-00019340: 6967 2e76 6572 626f 7365 0d0a 2020 2020  ig.verbose..    
-00019350: 2020 2020 2020 2020 636f 6e66 6967 2e76          config.v
-00019360: 6572 626f 7365 203d 2054 7275 650d 0a20  erbose = True.. 
-00019370: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-00019380: 2020 2020 2069 6620 696d 6167 655f 7061       if image_pa
-00019390: 7468 2e5f 5f63 6c61 7373 5f5f 2e5f 5f6e  th.__class__.__n
-000193a0: 616d 655f 5f20 3d3d 2022 7374 7222 3a0d  ame__ == "str":.
-000193b0: 0a20 2020 2020 2020 2020 2020 2069 6d61  .            ima
-000193c0: 6765 5f70 6174 6820 3d20 6f73 2e70 6174  ge_path = os.pat
-000193d0: 682e 6162 7370 6174 6828 696d 6167 655f  h.abspath(image_
-000193e0: 7061 7468 290d 0a20 2020 2020 2020 2020  path)..         
-000193f0: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-00019400: 0a20 2020 2020 2020 2023 203d 3d3d 3d3d  .        # =====
-00019410: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00019420: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00019430: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00019440: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00019450: 3d3d 3d3d 3d3d 3d3d 0d0a 2020 2020 2020  ========..      
-00019460: 2020 2320 4c4f 4747 494e 470d 0a20 2020    # LOGGING..   
-00019470: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-00019480: 2020 2023 2320 7374 6172 7420 6c6f 6767     ## start logg
-00019490: 696e 670d 0a20 2020 2020 2020 2073 656c  ing..        sel
-000194a0: 662e 6c6f 6767 6572 203d 206c 6f67 6769  f.logger = loggi
-000194b0: 6e67 2e67 6574 4c6f 6767 6572 2829 0d0a  ng.getLogger()..
-000194c0: 2020 2020 2020 2020 7365 6c66 2e6c 6f67          self.log
-000194d0: 6765 722e 7365 744c 6576 656c 286c 6f67  ger.setLevel(log
-000194e0: 6769 6e67 2e49 4e46 4f29 0d0a 2020 2020  ging.INFO)..    
-000194f0: 2020 2020 6966 2028 7365 6c66 2e6c 6f67      if (self.log
-00019500: 6765 722e 6861 7348 616e 646c 6572 7328  ger.hasHandlers(
-00019510: 2929 3a0d 0a20 2020 2020 2020 2020 2020  )):..           
-00019520: 2073 656c 662e 6c6f 6767 6572 2e68 616e   self.logger.han
-00019530: 646c 6572 732e 636c 6561 7228 290d 0a20  dlers.clear().. 
-00019540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00019550: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-00019560: 2069 6620 7365 6c66 2e66 6c61 6773 2e66   if self.flags.f
-00019570: 6565 6462 6163 6b3a 0d0a 2020 2020 2020  eedback:..      
-00019580: 2020 2020 2020 7374 646f 7574 5f68 616e        stdout_han
-00019590: 646c 6572 203d 206c 6f67 6769 6e67 2e53  dler = logging.S
-000195a0: 7472 6561 6d48 616e 646c 6572 2873 7973  treamHandler(sys
-000195b0: 2e73 7464 6f75 7429 0d0a 2020 2020 2020  .stdout)..      
-000195c0: 2020 2020 2020 7374 646f 7574 5f68 616e        stdout_han
-000195d0: 646c 6572 2e73 6574 4c65 7665 6c28 6c6f  dler.setLevel(lo
-000195e0: 6767 696e 672e 4445 4255 4729 0d0a 2020  gging.DEBUG)..  
-000195f0: 2020 2020 2020 2020 2020 7374 646f 7574            stdout
-00019600: 5f66 6f72 6d61 7474 6572 203d 206c 6f67  _formatter = log
-00019610: 6769 6e67 2e46 6f72 6d61 7474 6572 2827  ging.Formatter('
-00019620: 2528 6173 6374 696d 6529 733a 2025 286d  %(asctime)s: %(m
-00019630: 6573 7361 6765 2973 272c 2022 2548 3a25  essage)s', "%H:%
-00019640: 4d3a 2553 2229 0d0a 2020 2020 2020 2020  M:%S")..        
-00019650: 2020 2020 7374 646f 7574 5f68 616e 646c      stdout_handl
-00019660: 6572 2e73 6574 466f 726d 6174 7465 7228  er.setFormatter(
-00019670: 7374 646f 7574 5f66 6f72 6d61 7474 6572  stdout_formatter
-00019680: 290d 0a20 2020 2020 2020 2020 2020 2073  )..            s
-00019690: 656c 662e 6c6f 6767 6572 2e61 6464 4861  elf.logger.addHa
-000196a0: 6e64 6c65 7228 7374 646f 7574 5f68 616e  ndler(stdout_han
-000196b0: 646c 6572 290d 0a0d 0a20 2020 2020 2020  dler)....       
-000196c0: 2023 2320 6c6f 6720 6669 6c65 0d0a 2020   ## log file..  
-000196d0: 2020 2020 2020 6966 206f 732e 7061 7468        if os.path
-000196e0: 2e69 7364 6972 2869 6d61 6765 5f70 6174  .isdir(image_pat
-000196f0: 6829 3a0d 0a20 2020 2020 2020 2020 2020  h):..           
-00019700: 206c 6f67 5f66 696c 655f 7061 7468 203d   log_file_path =
-00019710: 206f 732e 7061 7468 2e6a 6f69 6e28 696d   os.path.join(im
-00019720: 6167 655f 7061 7468 2c20 6622 7079 7065  age_path, f"pype
-00019730: 5f6c 6f67 735f 7b74 6167 7d2e 6c6f 6722  _logs_{tag}.log"
-00019740: 290d 0a20 2020 2020 2020 2065 6c69 6620  )..        elif 
-00019750: 6f73 2e70 6174 682e 6973 6669 6c65 2869  os.path.isfile(i
-00019760: 6d61 6765 5f70 6174 6829 3a0d 0a20 2020  mage_path):..   
-00019770: 2020 2020 2020 2020 206c 6f67 5f66 696c           log_fil
-00019780: 655f 7061 7468 203d 206f 732e 7061 7468  e_path = os.path
-00019790: 2e6a 6f69 6e28 6f73 2e70 6174 682e 6469  .join(os.path.di
-000197a0: 726e 616d 6528 696d 6167 655f 7061 7468  rname(image_path
-000197b0: 292c 2066 2270 7970 655f 6c6f 6773 5f7b  ), f"pype_logs_{
-000197c0: 7461 677d 2e6c 6f67 2229 0d0a 0d0a 2020  tag}.log")....  
-000197d0: 2020 2020 2020 6966 206f 732e 7061 7468        if os.path
-000197e0: 2e69 7366 696c 6528 6c6f 675f 6669 6c65  .isfile(log_file
-000197f0: 5f70 6174 6829 2061 6e64 206c 6f67 5f6f  _path) and log_o
-00019800: 773a 0d0a 2020 2020 2020 2020 2020 2020  w:..            
-00019810: 6f73 2e72 656d 6f76 6528 6c6f 675f 6669  os.remove(log_fi
-00019820: 6c65 5f70 6174 6829 0d0a 2020 2020 2020  le_path)..      
-00019830: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-00019840: 6669 6c65 5f68 616e 646c 6572 203d 206c  file_handler = l
-00019850: 6f67 6769 6e67 2e46 696c 6548 616e 646c  ogging.FileHandl
-00019860: 6572 286c 6f67 5f66 696c 655f 7061 7468  er(log_file_path
-00019870: 290d 0a20 2020 2020 2020 2066 696c 655f  )..        file_
-00019880: 6861 6e64 6c65 722e 7365 744c 6576 656c  handler.setLevel
-00019890: 286c 6f67 6769 6e67 2e49 4e46 4f29 0d0a  (logging.INFO)..
-000198a0: 2020 2020 2020 2020 6669 6c65 5f66 6f72          file_for
-000198b0: 6d61 7474 6572 203d 206c 6f67 6769 6e67  matter = logging
-000198c0: 2e46 6f72 6d61 7474 6572 2827 5b25 2861  .Formatter('[%(a
-000198d0: 7363 7469 6d65 2973 5d5b 2528 6c65 7665  sctime)s][%(leve
-000198e0: 6c6e 616d 6529 735d 2025 286d 6573 7361  lname)s] %(messa
-000198f0: 6765 2973 272c 2022 2559 2d25 6d2d 2564  ge)s', "%Y-%m-%d
-00019900: 2025 483a 254d 3a25 5322 290d 0a20 2020   %H:%M:%S")..   
-00019910: 2020 2020 2066 696c 655f 6861 6e64 6c65       file_handle
-00019920: 722e 7365 7446 6f72 6d61 7474 6572 2866  r.setFormatter(f
-00019930: 696c 655f 666f 726d 6174 7465 7229 0d0a  ile_formatter)..
-00019940: 2020 2020 2020 2020 7365 6c66 2e6c 6f67          self.log
-00019950: 6765 722e 6164 6448 616e 646c 6572 2866  ger.addHandler(f
-00019960: 696c 655f 6861 6e64 6c65 7229 0d0a 0d0a  ile_handler)....
-00019970: 2020 2020 2020 2020 2320 3d3d 3d3d 3d3d          # ======
-00019980: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00019990: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000199a0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000199b0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000199c0: 3d3d 3d3d 3d3d 3d0d 0a20 2020 2020 2020  =======..       
-000199d0: 2023 2043 4845 434b 5320 0d0a 0d0a 2020   # CHECKS ....  
-000199e0: 2020 2020 2020 2323 2063 6865 636b 206e        ## check n
-000199f0: 616d 652c 206c 6f61 6420 636f 6e74 6169  ame, load contai
-00019a00: 6e65 7220 616e 6420 636f 6e66 6967 0d0a  ner and config..
-00019a10: 2020 2020 2020 2020 756c 2e5f 6368 6563          ul._chec
-00019a20: 6b5f 7079 7065 5f74 6167 2874 6167 290d  k_pype_tag(tag).
-00019a30: 0a20 2020 2020 2020 2073 656c 662e 5f6c  .        self._l
-00019a40: 6f61 645f 636f 6e74 6169 6e65 7228 696d  oad_container(im
-00019a50: 6167 655f 7061 7468 3d69 6d61 6765 5f70  age_path=image_p
-00019a60: 6174 682c 2074 6167 3d74 6167 290d 0a20  ath, tag=tag).. 
-00019a70: 2020 2020 2020 2073 656c 662e 5f6c 6f61         self._loa
-00019a80: 645f 636f 6e66 6967 2869 6d61 6765 5f70  d_config(image_p
-00019a90: 6174 683d 696d 6167 655f 7061 7468 2c20  ath=image_path, 
-00019aa0: 7461 673d 7461 672c 2063 6f6e 6669 675f  tag=tag, config_
-00019ab0: 7061 7468 3d63 6f6e 6669 675f 7061 7468  path=config_path
-00019ac0: 290d 0a0d 0a20 2020 2020 2020 2023 2063  )....        # c
-00019ad0: 6865 636b 2076 6572 7369 6f6e 2c20 6c6f  heck version, lo
-00019ae0: 6164 2063 6f6e 7461 696e 6572 2061 6e64  ad container and
-00019af0: 2063 6f6e 6669 670d 0a20 2020 2020 2020   config..       
-00019b00: 2069 6620 7365 6c66 2e66 6c61 6773 2e64   if self.flags.d
-00019b10: 7279 5f72 756e 3a0d 0a20 2020 2020 2020  ry_run:..       
-00019b20: 2020 2020 2073 656c 662e 5f6c 6f61 645f       self._load_
-00019b30: 636f 6e66 6967 2869 6d61 6765 5f70 6174  config(image_pat
-00019b40: 682c 2074 6167 2c20 636f 6e66 6967 5f70  h, tag, config_p
-00019b50: 6174 6829 0d0a 2020 2020 2020 2020 2020  ath)..          
-00019b60: 2020 7365 6c66 2e5f 6974 6572 6174 6528    self._iterate(
-00019b70: 616e 6e6f 7461 7469 6f6e 733d 636f 7079  annotations=copy
-00019b80: 2e64 6565 7063 6f70 7928 5f76 6172 732e  .deepcopy(_vars.
-00019b90: 5f61 6e6e 6f74 6174 696f 6e5f 7479 7065  _annotation_type
-00019ba0: 7329 2c0d 0a20 2020 2020 2020 2020 2020  s),..           
-00019bb0: 2020 2020 2020 2020 2020 2065 7865 6375             execu
-00019bc0: 7465 3d46 616c 7365 2c20 6175 746f 7368  te=False, autosh
-00019bd0: 6f77 3d46 616c 7365 2c20 6665 6564 6261  ow=False, feedba
-00019be0: 636b 3d54 7275 6529 0d0a 2020 2020 2020  ck=True)..      
-00019bf0: 2020 2020 2020 7265 7475 726e 0d0a 0d0a        return....
-00019c00: 2020 2020 2020 2020 2323 2063 6865 636b          ## check
-00019c10: 2077 6865 7468 6572 2064 6972 6563 746f   whether directo
-00019c20: 7279 2069 7320 736b 6970 7065 640d 0a20  ry is skipped.. 
-00019c30: 2020 2020 2020 2069 6620 7365 6c66 2e66         if self.f
-00019c40: 6c61 6773 2e73 6b69 703a 0d0a 2020 2020  lags.skip:..    
-00019c50: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00019c60: 5f63 6865 636b 5f64 6972 6563 746f 7279  _check_directory
-00019c70: 5f73 6b69 7028 0d0a 2020 2020 2020 2020  _skip(..        
-00019c80: 2020 2020 2020 2020 7461 673d 7461 672c          tag=tag,
-00019c90: 2073 6b69 705f 7061 7474 6572 6e3d 736b   skip_pattern=sk
-00019ca0: 6970 2c20 6469 725f 7061 7468 3d73 656c  ip, dir_path=sel
-00019cb0: 662e 636f 6e74 6169 6e65 722e 6469 725f  f.container.dir_
-00019cc0: 7061 7468 0d0a 2020 2020 2020 2020 2020  path..          
-00019cd0: 2020 293a 0d0a 2020 2020 2020 2020 2020    ):..          
-00019ce0: 2020 2020 2020 7265 7475 726e 0d0a 2020        return..  
-00019cf0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-00019d00: 2020 2020 2320 3d3d 3d3d 3d3d 3d3d 3d3d      # ==========
-00019d10: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00019d20: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00019d30: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00019d40: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00019d50: 3d3d 3d0d 0a20 2020 2020 2020 2023 2046  ===..        # F
-00019d60: 4545 4442 4143 4b20 0d0a 2020 2020 2020  EEDBACK ..      
-00019d70: 2020 0d0a 2020 2020 2020 2020 7374 6172    ..        star
-00019d80: 7475 705f 6d73 675f 6c69 7374 203d 205b  tup_msg_list = [
-00019d90: 5d0d 0a20 2020 2020 2020 2073 7461 7274  ]..        start
-00019da0: 7570 5f6d 7367 5f6c 6973 742e 6170 7065  up_msg_list.appe
-00019db0: 6e64 2875 6c2e 5f70 7072 696e 745f 6669  nd(ul._pprint_fi
-00019dc0: 6c6c 5f68 6261 7228 7365 6c66 2e63 6f6e  ll_hbar(self.con
-00019dd0: 7461 696e 6572 2e69 6d61 6765 5f6e 616d  tainer.image_nam
-00019de0: 652c 2073 796d 626f 6c3d 223d 222c 2072  e, symbol="=", r
-00019df0: 6574 3d54 7275 6529 290d 0a20 2020 2020  et=True))..     
-00019e00: 2020 2073 656c 662e 5f6c 6f67 2822 696e     self._log("in
-00019e10: 666f 222c 2073 7461 7274 7570 5f6d 7367  fo", startup_msg
-00019e20: 5f6c 6973 742c 2030 2c20 7061 7373 7468  _list, 0, passth
-00019e30: 726f 7567 683d 5472 7565 290d 0a20 2020  rough=True)..   
-00019e40: 2020 2020 200d 0a20 2020 2020 2020 2023       ..        #
-00019e50: 203d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d   ===============
-00019e60: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00019e70: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00019e80: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00019e90: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 0d0a  ==============..
-00019ea0: 0d0a 2020 2020 2020 2020 2323 206c 6f61  ..        ## loa
-00019eb0: 6420 6578 6973 7469 6e67 2061 6e6e 6f74  d existing annot
-00019ec0: 6174 696f 6e73 2074 6872 6f75 6768 2063  ations through c
-00019ed0: 6f6e 7461 696e 6572 0d0a 2020 2020 2020  ontainer..      
-00019ee0: 2020 6966 2073 656c 662e 666c 6167 732e    if self.flags.
-00019ef0: 6175 746f 6c6f 6164 3a0d 0a20 2020 2020  autoload:..     
-00019f00: 2020 2020 2020 2073 656c 662e 5f6c 6f67         self._log
-00019f10: 2822 696e 666f 222c 2022 5079 7065 3a20  ("info", "Pype: 
-00019f20: 4155 544f 4c4f 4144 222c 2030 290d 0a20  AUTOLOAD", 0).. 
-00019f30: 2020 2020 2020 2020 2020 2077 6974 6820             with 
-00019f40: 696f 2e53 7472 696e 6749 4f28 2920 6173  io.StringIO() as
-00019f50: 2062 7566 6665 722c 2072 6564 6972 6563   buffer, redirec
-00019f60: 745f 7374 646f 7574 2862 7566 6665 7229  t_stdout(buffer)
-00019f70: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-00019f80: 2020 2073 656c 662e 636f 6e74 6169 6e65     self.containe
-00019f90: 722e 5f6c 6f61 6428 636f 6e74 6f75 7273  r._load(contours
-00019fa0: 3d6c 6f61 645f 636f 6e74 6f75 7273 290d  =load_contours).
-00019fb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00019fc0: 2073 7464 6f75 7420 3d20 6275 6666 6572   stdout = buffer
-00019fd0: 2e67 6574 7661 6c75 6528 290d 0a20 2020  .getvalue()..   
-00019fe0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00019ff0: 662e 5f6c 6f67 2822 696e 666f 222c 2073  f._log("info", s
-0001a000: 7464 6f75 742c 2031 290d 0a0d 0a20 2020  tdout, 1)....   
-0001a010: 2020 2020 2023 2320 6368 6563 6b20 7079       ## check py
-0001a020: 7065 2063 6f6e 6669 6720 666f 7220 616e  pe config for an
-0001a030: 6e6f 7461 7469 6f6e 730d 0a20 2020 2020  notations..     
-0001a040: 2020 2073 656c 662e 5f69 7465 7261 7465     self._iterate
-0001a050: 280d 0a20 2020 2020 2020 2020 2020 2061  (..            a
-0001a060: 6e6e 6f74 6174 696f 6e73 3d73 656c 662e  nnotations=self.
-0001a070: 636f 6e74 6169 6e65 722e 616e 6e6f 7461  container.annota
-0001a080: 7469 6f6e 732c 0d0a 2020 2020 2020 2020  tions,..        
-0001a090: 2020 2020 6578 6563 7574 653d 4661 6c73      execute=Fals
-0001a0a0: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
-0001a0b0: 6175 746f 7368 6f77 3d46 616c 7365 2c0d  autoshow=False,.
-0001a0c0: 0a20 2020 2020 2020 2020 2020 2069 6e74  .            int
-0001a0d0: 6572 6163 7469 7665 3d46 616c 7365 2c0d  eractive=False,.
-0001a0e0: 0a20 2020 2020 2020 2029 0d0a 0d0a 2020  .        )....  
-0001a0f0: 2020 2020 2020 2323 2066 696e 616c 2063        ## final c
-0001a100: 6865 636b 2062 6566 6f72 6520 7374 6172  heck before star
-0001a110: 7469 6e67 2070 7970 650d 0a20 2020 2020  ting pype..     
-0001a120: 2020 2073 656c 662e 5f63 6865 636b 5f66     self._check_f
-0001a130: 696e 616c 2829 0d0a 2020 2020 2020 2020  inal()..        
-0001a140: 0d0a 2020 2020 2020 2020 2323 2074 7572  ..        ## tur
-0001a150: 6e20 6f66 6620 6175 7473 686f 7720 616e  n off autshow an
-0001a160: 6420 6669 6c65 206d 6f6e 6974 6f72 2069  d file monitor i
-0001a170: 6e20 6e6f 6e2d 696e 7465 7261 6374 6976  n non-interactiv
-0001a180: 6520 6d6f 6465 0d0a 2020 2020 2020 2020  e mode..        
-0001a190: 6966 2073 656c 662e 666c 6167 732e 696e  if self.flags.in
-0001a1a0: 7465 7261 6374 6976 653a 0d0a 2020 2020  teractive:..    
-0001a1b0: 2020 2020 2020 2020 7365 6c66 2e5f 7374          self._st
-0001a1c0: 6172 745f 6669 6c65 5f6d 6f6e 6974 6f72  art_file_monitor
-0001a1d0: 2864 656c 6179 3d64 656c 6179 290d 0a20  (delay=delay).. 
-0001a1e0: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
-0001a1f0: 2020 2020 2020 2020 2020 7365 6c66 2e66            self.f
-0001a200: 6c61 6773 2e61 7574 6f73 686f 7720 3d20  lags.autoshow = 
-0001a210: 4661 6c73 650d 0a20 2020 2020 2020 2020  False..         
-0001a220: 2020 200d 0a20 2020 2020 2020 2023 2320     ..        ## 
-0001a230: 636c 6561 7220 6f6c 6420 7a6f 6f6d 206d  clear old zoom m
-0001a240: 656d 6f72 790d 0a20 2020 2020 2020 2063  emory..        c
-0001a250: 6f6e 6669 672e 6775 695f 7a6f 6f6d 5f63  onfig.gui_zoom_c
-0001a260: 6f6e 6669 6720 3d20 4e6f 6e65 0d0a 0d0a  onfig = None....
-0001a270: 2020 2020 2020 2020 2320 3d3d 3d3d 3d3d          # ======
-0001a280: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0001a290: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0001a2a0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0001a2b0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0001a2c0: 3d3d 3d3d 3d3d 3d0d 0a20 2020 2020 2020  =======..       
-0001a2d0: 2023 2050 5950 4520 4c4f 4f50 0d0a 0d0a   # PYPE LOOP....
-0001a2e0: 2020 2020 2020 2020 2323 2072 756e 2070          ## run p
-0001a2f0: 7970 650d 0a20 2020 2020 2020 2077 6869  ype..        whi
-0001a300: 6c65 2054 7275 653a 0d0a 0d0a 2020 2020  le True:....    
-0001a310: 2020 2020 2020 2020 2323 2070 7970 6520          ## pype 
-0001a320: 7265 7374 6172 7420 666c 6167 0d0a 2020  restart flag..  
-0001a330: 2020 2020 2020 2020 2020 636f 6e66 6967            config
-0001a340: 2e70 7970 655f 7265 7374 6172 7420 3d20  .pype_restart = 
-0001a350: 4661 6c73 650d 0a0d 0a20 2020 2020 2020  False....       
-0001a360: 2020 2020 2023 2320 7265 6672 6573 6820       ## refresh 
-0001a370: 636f 6e66 6967 0d0a 2020 2020 2020 2020  config..        
-0001a380: 2020 2020 6966 2073 656c 662e 666c 6167      if self.flag
-0001a390: 732e 696e 7465 7261 6374 6976 653a 0d0a  s.interactive:..
-0001a3a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001a3b0: 2020 2323 2074 6f20 7374 6f70 2069 6e66    ## to stop inf
-0001a3c0: 696e 6974 6520 6c6f 6f70 2077 6974 686f  inite loop witho
-0001a3d0: 7574 206f 7065 6e69 6e67 206e 6577 2077  ut opening new w
-0001a3e0: 696e 646f 770d 0a20 2020 2020 2020 2020  indow..         
-0001a3f0: 2020 2020 2020 2069 6620 6e6f 7420 7365         if not se
-0001a400: 6c66 2e59 464d 2e63 6f6e 7465 6e74 3a0d  lf.YFM.content:.
-0001a410: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001a420: 2020 2020 2073 656c 662e 5f6c 6f67 2822       self._log("
-0001a430: 6465 6275 6722 2c20 2250 7970 653a 2053  debug", "Pype: S
-0001a440: 5449 4c4c 2055 5044 4154 494e 4720 434f  TILL UPDATING CO
-0001a450: 4e46 4947 2028 6e6f 2063 6f6e 6669 6729  NFIG (no config)
-0001a460: 222c 2030 290d 0a20 2020 2020 2020 2020  ", 0)..         
-0001a470: 2020 2020 2020 2020 2020 2063 7632 2e64             cv2.d
-0001a480: 6573 7472 6f79 5769 6e64 6f77 2822 7068  estroyWindow("ph
-0001a490: 656e 6f70 7970 6522 290d 0a20 2020 2020  enopype")..     
-0001a4a0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-0001a4b0: 696d 652e 736c 6565 7028 3129 0d0a 2020  ime.sleep(1)..  
-0001a4c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a4d0: 2020 7365 6c66 2e59 464d 2e5f 7374 6f70    self.YFM._stop
-0001a4e0: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
-0001a4f0: 2020 2020 2020 2020 7365 6c66 2e5f 7374          self._st
-0001a500: 6172 745f 6669 6c65 5f6d 6f6e 6974 6f72  art_file_monitor
-0001a510: 2864 656c 6179 3d64 656c 6179 290d 0a20  (delay=delay).. 
-0001a520: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a530: 2020 2063 6f6e 7469 6e75 650d 0a0d 0a20     continue.... 
-0001a540: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0001a550: 656c 662e 636f 6e66 6967 203d 2063 6f70  elf.config = cop
-0001a560: 792e 6465 6570 636f 7079 2873 656c 662e  y.deepcopy(self.
-0001a570: 5946 4d2e 636f 6e74 656e 7429 0d0a 0d0a  YFM.content)....
-0001a580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a590: 6966 206e 6f74 2073 656c 662e 636f 6e66  if not self.conf
-0001a5a0: 6967 3a0d 0a20 2020 2020 2020 2020 2020  ig:..           
-0001a5b0: 2020 2020 2020 2020 2073 656c 662e 5f6c           self._l
-0001a5c0: 6f67 2822 6465 6275 6722 2c20 2250 7970  og("debug", "Pyp
-0001a5d0: 653a 2053 5449 4c4c 2055 5044 4154 494e  e: STILL UPDATIN
-0001a5e0: 4720 434f 4e46 4947 2028 6e6f 2063 6f6e  G CONFIG (no con
-0001a5f0: 6669 6729 222c 2030 290d 0a20 2020 2020  fig)", 0)..     
-0001a600: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-0001a610: 6f6e 7469 6e75 650d 0a0d 0a20 2020 2020  ontinue....     
-0001a620: 2020 2020 2020 2023 2320 7275 6e20 7079         ## run py
-0001a630: 7065 2063 6f6e 6669 6720 696e 2073 6571  pe config in seq
-0001a640: 7565 6e63 650d 0a20 2020 2020 2020 2020  uence..         
-0001a650: 2020 2073 656c 662e 5f69 7465 7261 7465     self._iterate
-0001a660: 280d 0a20 2020 2020 2020 2020 2020 2020  (..             
-0001a670: 2020 2061 6e6e 6f74 6174 696f 6e73 3d73     annotations=s
-0001a680: 656c 662e 636f 6e74 6169 6e65 722e 616e  elf.container.an
-0001a690: 6e6f 7461 7469 6f6e 732c 0d0a 2020 2020  notations,..    
-0001a6a0: 2020 2020 2020 2020 2020 2020 696e 7465              inte
-0001a6b0: 7261 6374 6976 653d 7365 6c66 2e66 6c61  ractive=self.fla
-0001a6c0: 6773 2e69 6e74 6572 6163 7469 7665 2c0d  gs.interactive,.
-0001a6d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001a6e0: 2061 7574 6f73 686f 773d 7365 6c66 2e66   autoshow=self.f
-0001a6f0: 6c61 6773 2e61 7574 6f73 686f 772c 0d0a  lags.autoshow,..
-0001a700: 2020 2020 2020 2020 2020 2020 290d 0a0d              )...
-0001a710: 0a20 2020 2020 2020 2020 2020 2023 2320  .            ## 
-0001a720: 7465 726d 696e 6174 6520 2620 636c 6561  terminate & clea
-0001a730: 6e75 700d 0a20 2020 2020 2020 2020 2020  nup..           
-0001a740: 2069 6620 7365 6c66 2e66 6c61 6773 2e69   if self.flags.i
-0001a750: 6e74 6572 6163 7469 7665 3a0d 0a20 2020  nteractive:..   
-0001a760: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-0001a770: 7365 6c66 2e66 6c61 6773 2e74 6572 6d69  self.flags.termi
-0001a780: 6e61 7465 3a0d 0a20 2020 2020 2020 2020  nate:..         
-0001a790: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-0001a7a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a7b0: 2023 2320 7374 6f70 6520 6669 6c65 206d   ## stope file m
-0001a7c0: 6f6e 6974 6f72 696e 670d 0a20 2020 2020  onitoring..     
-0001a7d0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0001a7e0: 6620 6861 7361 7474 7228 7365 6c66 2c20  f hasattr(self, 
-0001a7f0: 2259 464d 2229 3a0d 0a20 2020 2020 2020  "YFM"):..       
-0001a800: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a810: 2073 656c 662e 5946 4d2e 5f73 746f 7028   self.YFM._stop(
-0001a820: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-0001a830: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-0001a840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a850: 2023 2320 7265 7365 7420 7a6f 6f6d 2073   ## reset zoom s
-0001a860: 6574 7469 6e67 730d 0a20 2020 2020 2020  ettings..       
-0001a870: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-0001a880: 6e6f 7420 7365 6c66 2e66 6c61 6773 2e7a  not self.flags.z
-0001a890: 6f6f 6d5f 6d65 6d6f 7279 3a0d 0a20 2020  oom_memory:..   
-0001a8a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a8b0: 2020 2020 2063 6f6e 6669 672e 6775 695f       config.gui_
-0001a8c0: 7a6f 6f6d 5f63 6f6e 6669 6720 3d20 4e6f  zoom_config = No
-0001a8d0: 6e65 0d0a 2020 2020 2020 2020 2020 2020  ne..            
-0001a8e0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-0001a8f0: 2020 2020 2020 2020 2020 2020 2020 2323                ##
-0001a900: 2061 6464 200d 0a20 2020 2020 2020 2020   add ..         
-0001a910: 2020 2020 2020 2020 2020 2069 6620 2263             if "c
-0001a920: 6f6e 6669 675f 696e 666f 2220 696e 2073  onfig_info" in s
-0001a930: 656c 662e 636f 6e66 6967 3a0d 0a20 2020  elf.config:..   
-0001a940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001a950: 2020 2020 2073 656c 662e 636f 6e66 6967       self.config
-0001a960: 5b22 636f 6e66 6967 5f69 6e66 6f22 5d5b  ["config_info"][
-0001a970: 2264 6174 655f 6c61 7374 5f6d 6f64 6966  "date_last_modif
-0001a980: 6965 6422 5d20 3d20 6461 7465 7469 6d65  ied"] = datetime
-0001a990: 2e74 6f64 6179 2829 2e73 7472 6674 696d  .today().strftim
-0001a9a0: 6528 5f76 6172 732e 7374 7266 7469 6d65  e(_vars.strftime
-0001a9b0: 5f66 6f72 6d61 7429 0d0a 2020 2020 2020  _format)..      
-0001a9c0: 2020 2020 2020 2020 2020 2020 2020 756c                ul
-0001a9d0: 2e5f 7361 7665 5f79 616d 6c28 7365 6c66  ._save_yaml(self
-0001a9e0: 2e63 6f6e 6669 672c 2073 656c 662e 636f  .config, self.co
-0001a9f0: 6e66 6967 5f70 6174 6829 0d0a 2020 2020  nfig_path)..    
-0001aa00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001aa10: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-0001aa20: 2020 2020 2020 2020 2020 2323 2066 6565            ## fee
-0001aa30: 6462 6163 6b0d 0a20 2020 2020 2020 2020  dback..         
-0001aa40: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0001aa50: 5f6c 6f67 2822 696e 666f 222c 2022 5079  _log("info", "Py
-0001aa60: 7065 3a20 5445 524d 494e 4154 4522 2c20  pe: TERMINATE", 
-0001aa70: 3029 0d0a 2020 2020 2020 2020 2020 2020  0)..            
-0001aa80: 2020 2020 2020 2020 6272 6561 6b0d 0a20          break.. 
-0001aa90: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-0001aaa0: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
-0001aab0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-0001aac0: 2020 2020 6272 6561 6b0d 0a20 2020 2020      break..     
-0001aad0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
-0001aae0: 2023 203d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d   # =============
-0001aaf0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0001ab00: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0001ab10: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0001ab20: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0001ab30: 0d0a 2020 2020 2020 2020 2323 2061 7574  ..        ## aut
-0001ab40: 6f73 6176 650d 0a20 2020 2020 2020 2069  osave..        i
-0001ab50: 6620 7365 6c66 2e66 6c61 6773 2e61 7574  f self.flags.aut
-0001ab60: 6f73 6176 6520 616e 6420 7365 6c66 2e66  osave and self.f
-0001ab70: 6c61 6773 2e74 6572 6d69 6e61 7465 3a0d  lags.terminate:.
-0001ab80: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0001ab90: 662e 5f6c 6f67 2822 696e 666f 222c 2022  f._log("info", "
-0001aba0: 5079 7065 3a20 4155 544f 5341 5645 222c  Pype: AUTOSAVE",
-0001abb0: 2030 290d 0a20 2020 2020 2020 2020 2020   0)..           
-0001abc0: 2069 6620 2265 7870 6f72 7422 206e 6f74   if "export" not
-0001abd0: 2069 6e20 7365 6c66 2e63 6f6e 6669 675f   in self.config_
-0001abe0: 7061 7273 6564 5f66 6c61 7474 656e 6564  parsed_flattened
-0001abf0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-0001ac00: 2020 2065 7870 6f72 745f 6c69 7374 203d     export_list =
-0001ac10: 205b 5d0d 0a20 2020 2020 2020 2020 2020   []..           
-0001ac20: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
-0001ac30: 2020 2020 2020 2020 6578 706f 7274 5f6c          export_l
-0001ac40: 6973 7420 3d20 7365 6c66 2e63 6f6e 6669  ist = self.confi
-0001ac50: 675f 7061 7273 6564 5f66 6c61 7474 656e  g_parsed_flatten
-0001ac60: 6564 5b22 6578 706f 7274 225d 0d0a 2020  ed["export"]..  
-0001ac70: 2020 2020 2020 2020 2020 7769 7468 2069            with i
-0001ac80: 6f2e 5374 7269 6e67 494f 2829 2061 7320  o.StringIO() as 
-0001ac90: 6275 6666 6572 2c20 7265 6469 7265 6374  buffer, redirect
-0001aca0: 5f73 7464 6f75 7428 6275 6666 6572 293a  _stdout(buffer):
-0001acb0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001acc0: 2020 7365 6c66 2e63 6f6e 7461 696e 6572    self.container
-0001acd0: 2e5f 7361 7665 2865 7870 6f72 745f 6c69  ._save(export_li
-0001ace0: 7374 3d65 7870 6f72 745f 6c69 7374 290d  st=export_list).
-0001acf0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001ad00: 2073 7464 6f75 7420 3d20 6275 6666 6572   stdout = buffer
-0001ad10: 2e67 6574 7661 6c75 6528 290d 0a20 2020  .getvalue()..   
-0001ad20: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0001ad30: 662e 5f6c 6f67 2822 696e 666f 222c 2073  f._log("info", s
-0001ad40: 7464 6f75 742c 2031 290d 0a20 2020 2020  tdout, 1)..     
-0001ad50: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-0001ad60: 2020 2020 2023 203d 3d3d 3d3d 3d3d 3d3d       # =========
-0001ad70: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0001ad80: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0001ad90: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0001ada0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0001adb0: 3d3d 3d3d 0d0a 2020 2020 2020 2020 2320  ====..        # 
-0001adc0: 4645 4544 4241 434b 200d 0a20 2020 2020  FEEDBACK ..     
-0001add0: 2020 200d 0a20 2020 2020 2020 2073 7461     ..        sta
-0001ade0: 7274 7570 5f6d 7367 5f6c 6973 7420 3d20  rtup_msg_list = 
-0001adf0: 5b5d 0d0a 2020 2020 2020 2020 7374 6172  []..        star
-0001ae00: 7475 705f 6d73 675f 6c69 7374 2e61 7070  tup_msg_list.app
-0001ae10: 656e 6428 756c 2e5f 7070 7269 6e74 5f66  end(ul._pprint_f
-0001ae20: 696c 6c5f 6862 6172 2822 454e 4422 2c20  ill_hbar("END", 
-0001ae30: 7379 6d62 6f6c 3d22 3d22 2c20 7265 743d  symbol="=", ret=
-0001ae40: 5472 7565 2929 0d0a 2020 2020 2020 2020  True))..        
-0001ae50: 7365 6c66 2e5f 6c6f 6728 2269 6e66 6f22  self._log("info"
-0001ae60: 2c20 7374 6172 7475 705f 6d73 675f 6c69  , startup_msg_li
-0001ae70: 7374 2c20 3029 0d0a 2020 2020 2020 2020  st, 0)..        
-0001ae80: 0d0a 2020 2020 2020 2020 2320 3d3d 3d3d  ..        # ====
-0001ae90: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0001aea0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0001aeb0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0001aec0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0001aed0: 3d3d 3d3d 3d3d 3d3d 3d0d 0a0d 0a20 2020  =========....   
-0001aee0: 2020 2020 2023 2320 656e 6420 6c6f 6767       ## end logg
-0001aef0: 696e 670d 0a20 2020 2020 2020 206c 6f67  ing..        log
-0001af00: 6769 6e67 2e73 6875 7464 6f77 6e28 290d  ging.shutdown().
-0001af10: 0a20 2020 2020 2020 200d 0a20 2020 2020  .        ..     
-0001af20: 2020 2069 6620 7365 6c66 2e66 6c61 6773     if self.flags
-0001af30: 2e64 6562 7567 3a0d 0a20 2020 2020 2020  .debug:..       
-0001af40: 2020 2020 2063 6f6e 6669 672e 7665 7262       config.verb
-0001af50: 6f73 6520 3d20 7365 6c66 2e76 6572 626f  ose = self.verbo
-0001af60: 7365 0d0a 0d0a 0d0a 2020 2020 6465 6620  se......    def 
-0001af70: 5f6c 6f61 645f 636f 6e74 6169 6e65 7228  _load_container(
-0001af80: 7365 6c66 2c20 696d 6167 655f 7061 7468  self, image_path
-0001af90: 2c20 7461 6729 3a0d 0a20 2020 2020 2020  , tag):..       
-0001afa0: 2069 6620 696d 6167 655f 7061 7468 2e5f   if image_path._
-0001afb0: 5f63 6c61 7373 5f5f 2e5f 5f6e 616d 655f  _class__.__name_
-0001afc0: 5f20 3d3d 2022 7374 7222 3a0d 0a20 2020  _ == "str":..   
-0001afd0: 2020 2020 2020 2020 2069 6620 6f73 2e70           if os.p
-0001afe0: 6174 682e 6973 6669 6c65 2869 6d61 6765  ath.isfile(image
-0001aff0: 5f70 6174 6829 3a0d 0a20 2020 2020 2020  _path):..       
-0001b000: 2020 2020 2020 2020 2069 6d61 6765 203d           image =
-0001b010: 2075 7469 6c73 2e6c 6f61 645f 696d 6167   utils.load_imag
-0001b020: 6528 696d 6167 655f 7061 7468 290d 0a20  e(image_path).. 
-0001b030: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-0001b040: 6972 5f70 6174 6820 3d20 6f73 2e70 6174  ir_path = os.pat
-0001b050: 682e 6469 726e 616d 6528 696d 6167 655f  h.dirname(image_
-0001b060: 7061 7468 290d 0a20 2020 2020 2020 2020  path)..         
-0001b070: 2020 2020 2020 2073 656c 662e 636f 6e74         self.cont
-0001b080: 6169 6e65 7220 3d20 756c 2e5f 436f 6e74  ainer = ul._Cont
-0001b090: 6169 6e65 7228 0d0a 2020 2020 2020 2020  ainer(..        
-0001b0a0: 2020 2020 2020 2020 2020 2020 696d 6167              imag
-0001b0b0: 653d 696d 6167 652c 0d0a 2020 2020 2020  e=image,..      
-0001b0c0: 2020 2020 2020 2020 2020 2020 2020 6469                di
-0001b0d0: 725f 7061 7468 3d64 6972 5f70 6174 682c  r_path=dir_path,
-0001b0e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001b0f0: 2020 2020 2020 7461 673d 7461 672c 0d0a        tag=tag,..
-0001b100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b110: 2020 2020 6669 6c65 5f70 7265 6669 783d      file_prefix=
-0001b120: 6f73 2e70 6174 682e 7370 6c69 7465 7874  os.path.splitext
-0001b130: 286f 732e 7061 7468 2e62 6173 656e 616d  (os.path.basenam
-0001b140: 6528 696d 6167 655f 7061 7468 2929 5b30  e(image_path))[0
-0001b150: 5d2c 0d0a 2020 2020 2020 2020 2020 2020  ],..            
-0001b160: 2020 2020 2020 2020 6669 6c65 5f73 7566          file_suf
-0001b170: 6669 783d 7461 672c 0d0a 2020 2020 2020  fix=tag,..      
-0001b180: 2020 2020 2020 2020 2020 2020 2020 696d                im
-0001b190: 6167 655f 6e61 6d65 3d6f 732e 7061 7468  age_name=os.path
-0001b1a0: 2e62 6173 656e 616d 6528 696d 6167 655f  .basename(image_
-0001b1b0: 7061 7468 292c 0d0a 2020 2020 2020 2020  path),..        
-0001b1c0: 2020 2020 2020 2020 290d 0a20 2020 2020          )..     
-0001b1d0: 2020 2020 2020 2065 6c69 6620 6f73 2e70         elif os.p
-0001b1e0: 6174 682e 6973 6469 7228 696d 6167 655f  ath.isdir(image_
-0001b1f0: 7061 7468 293a 0d0a 2020 2020 2020 2020  path):..        
-0001b200: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
-0001b210: 7461 696e 6572 203d 2075 6c2e 5f6c 6f61  tainer = ul._loa
-0001b220: 645f 7072 6f6a 6563 745f 696d 6167 655f  d_project_image_
-0001b230: 6469 7265 6374 6f72 7928 0d0a 2020 2020  directory(..    
-0001b240: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b250: 6469 725f 7061 7468 3d69 6d61 6765 5f70  dir_path=image_p
-0001b260: 6174 682c 2074 6167 3d74 6167 2c0d 0a20  ath, tag=tag,.. 
-0001b270: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-0001b280: 0d0a 2020 2020 2020 2020 2020 2020 656c  ..            el
-0001b290: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
-0001b2a0: 2020 2020 2072 6169 7365 2046 696c 654e       raise FileN
-0001b2b0: 6f74 466f 756e 6445 7272 6f72 280d 0a20  otFoundError(.. 
-0001b2c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b2d0: 2020 2027 436f 756c 6420 6e6f 7420 6669     'Could not fi
-0001b2e0: 6e64 2069 6d61 6765 206f 7220 696d 6167  nd image or imag
-0001b2f0: 6520 6469 7265 6374 6f72 793a 2022 7b7d  e directory: "{}
-0001b300: 2227 2e66 6f72 6d61 7428 0d0a 2020 2020  "'.format(..    
-0001b310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001b320: 2020 2020 6f73 2e70 6174 682e 6469 726e      os.path.dirn
-0001b330: 616d 6528 696d 6167 655f 7061 7468 290d  ame(image_path).
-0001b340: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001b350: 2020 2020 2029 0d0a 2020 2020 2020 2020       )..        
-0001b360: 2020 2020 2020 2020 290d 0a20 2020 2020          )..     
-0001b370: 2020 2065 6c69 6620 696d 6167 655f 7061     elif image_pa
-0001b380: 7468 2e5f 5f63 6c61 7373 5f5f 2e5f 5f6e  th.__class__.__n
-0001b390: 616d 655f 5f20 3d3d 2022 436f 6e74 6169  ame__ == "Contai
-0001b3a0: 6e65 7222 3a0d 0a20 2020 2020 2020 2020  ner":..         
-0001b3b0: 2020 2073 656c 662e 636f 6e74 6169 6e65     self.containe
-0001b3c0: 7220 3d20 636f 7079 2e64 6565 7063 6f70  r = copy.deepcop
-0001b3d0: 7928 696d 6167 655f 7061 7468 290d 0a20  y(image_path).. 
-0001b3e0: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
-0001b3f0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-0001b400: 5479 7065 4572 726f 7228 2249 6e76 616c  TypeError("Inval
-0001b410: 6964 2069 6e70 7574 2066 6f72 2069 6d61  id input for ima
-0001b420: 6765 2070 6174 6820 2873 7472 2072 6571  ge path (str req
-0001b430: 7569 7265 6429 2229 0d0a 0d0a 2020 2020  uired)")....    
-0001b440: 6465 6620 5f6c 6f61 645f 636f 6e66 6967  def _load_config
-0001b450: 2873 656c 662c 2069 6d61 6765 5f70 6174  (self, image_pat
-0001b460: 682c 2074 6167 2c20 636f 6e66 6967 5f70  h, tag, config_p
-0001b470: 6174 6829 3a0d 0a0d 0a20 2020 2020 2020  ath):....       
-0001b480: 2069 6620 636f 6e66 6967 5f70 6174 682e   if config_path.
-0001b490: 5f5f 636c 6173 735f 5f2e 5f5f 6e61 6d65  __class__.__name
-0001b4a0: 5f5f 203d 3d20 224e 6f6e 6554 7970 6522  __ == "NoneType"
-0001b4b0: 3a0d 0a20 2020 2020 2020 2020 2020 2069  :..            i
-0001b4c0: 6620 6f73 2e70 6174 682e 6973 6669 6c65  f os.path.isfile
-0001b4d0: 2869 6d61 6765 5f70 6174 6829 3a0d 0a20  (image_path):.. 
-0001b4e0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0001b4f0: 6d61 6765 5f6e 616d 655f 7374 656d 203d  mage_name_stem =
-0001b500: 206f 732e 7061 7468 2e73 706c 6974 6578   os.path.splitex
-0001b510: 7428 6f73 2e70 6174 682e 6261 7365 6e61  t(os.path.basena
-0001b520: 6d65 2869 6d61 6765 5f70 6174 6829 295b  me(image_path))[
-0001b530: 305d 0d0a 2020 2020 2020 2020 2020 2020  0]..            
-0001b540: 2020 2020 7072 6570 656e 6420 3d20 696d      prepend = im
-0001b550: 6167 655f 6e61 6d65 5f73 7465 6d20 2b20  age_name_stem + 
-0001b560: 225f 220d 0a20 2020 2020 2020 2020 2020  "_"..           
-0001b570: 2065 6c69 6620 6f73 2e70 6174 682e 6973   elif os.path.is
-0001b580: 6469 7228 696d 6167 655f 7061 7468 293a  dir(image_path):
-0001b590: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001b5a0: 2020 7072 6570 656e 6420 3d20 2222 0d0a    prepend = ""..
-0001b5b0: 0d0a 2020 2020 2020 2020 2020 2020 2323  ..            ##
-0001b5c0: 2067 656e 6572 6174 6520 636f 6e66 6967   generate config
-0001b5d0: 2070 6174 6820 6672 6f6d 2069 6d61 6765   path from image
-0001b5e0: 2066 696c 6520 6f72 2064 6972 6563 746f   file or directo
-0001b5f0: 7279 2028 7072 6f6a 6563 7429 0d0a 2020  ry (project)..  
-0001b600: 2020 2020 2020 2020 2020 636f 6e66 6967            config
-0001b610: 5f6e 616d 6520 3d20 7072 6570 656e 6420  _name = prepend 
-0001b620: 2b20 2270 7970 655f 636f 6e66 6967 5f22  + "pype_config_"
-0001b630: 202b 2074 6167 202b 2022 2e79 616d 6c22   + tag + ".yaml"
-0001b640: 0d0a 2020 2020 2020 2020 2020 2020 636f  ..            co
-0001b650: 6e66 6967 5f70 6174 6820 3d20 6f73 2e70  nfig_path = os.p
-0001b660: 6174 682e 6a6f 696e 2873 656c 662e 636f  ath.join(self.co
-0001b670: 6e74 6169 6e65 722e 6469 725f 7061 7468  ntainer.dir_path
-0001b680: 2c20 636f 6e66 6967 5f6e 616d 6529 0d0a  , config_name)..
-0001b690: 0d0a 2020 2020 2020 2020 2323 206c 6f61  ..        ## loa
-0001b6a0: 6420 636f 6e66 6967 2066 726f 6d20 636f  d config from co
-0001b6b0: 6e66 6967 2070 6174 680d 0a20 2020 2020  nfig path..     
-0001b6c0: 2020 2065 6c69 6620 636f 6e66 6967 5f70     elif config_p
-0001b6d0: 6174 682e 5f5f 636c 6173 735f 5f2e 5f5f  ath.__class__.__
-0001b6e0: 6e61 6d65 5f5f 203d 3d20 2273 7472 223a  name__ == "str":
-0001b6f0: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-0001b700: 206f 732e 7061 7468 2e69 7366 696c 6528   os.path.isfile(
-0001b710: 636f 6e66 6967 5f70 6174 6829 3a0d 0a20  config_path):.. 
-0001b720: 2020 2020 2020 2020 2020 2020 2020 2070                 p
-0001b730: 6173 730d 0a20 2020 2020 2020 2020 2020  ass..           
-0001b740: 2023 2065 6c73 653a 0d0a 2020 2020 2020   # else:..      
-0001b750: 2020 2020 2020 2320 2020 2020 7261 6973        #     rais
-0001b760: 6520 4669 6c65 4e6f 7446 6f75 6e64 4572  e FileNotFoundEr
-0001b770: 726f 7228 0d0a 2020 2020 2020 2020 2020  ror(..          
-0001b780: 2020 2320 2020 2020 2020 2020 2243 6f75    #         "Cou
-0001b790: 6c64 206e 6f74 2072 6561 6420 636f 6e66  ld not read conf
-0001b7a0: 6967 2066 696c 6520 6672 6f6d 2073 7065  ig file from spe
-0001b7b0: 6369 6669 6564 2063 6f6e 6669 675f 7061  cified config_pa
-0001b7c0: 7468 3a20 5c22 7b7d 5c22 222e 666f 726d  th: \"{}\"".form
-0001b7d0: 6174 2863 6f6e 6669 675f 7061 7468 2929  at(config_path))
-0001b7e0: 0d0a 0d0a 2020 2020 2020 2020 6966 206f  ....        if o
-0001b7f0: 732e 7061 7468 2e69 7366 696c 6528 636f  s.path.isfile(co
-0001b800: 6e66 6967 5f70 6174 6829 3a0d 0a20 2020  nfig_path):..   
-0001b810: 2020 2020 2020 2020 2073 656c 662e 636f           self.co
-0001b820: 6e66 6967 203d 2075 6c2e 5f6c 6f61 645f  nfig = ul._load_
-0001b830: 7961 6d6c 2863 6f6e 6669 675f 7061 7468  yaml(config_path
-0001b840: 290d 0a20 2020 2020 2020 2020 2020 2073  )..            s
-0001b850: 656c 662e 636f 6e66 6967 5f70 6174 6820  elf.config_path 
-0001b860: 3d20 636f 6e66 6967 5f70 6174 680d 0a20  = config_path.. 
-0001b870: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
-0001b880: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-0001b890: 4669 6c65 4e6f 7446 6f75 6e64 4572 726f  FileNotFoundErro
-0001b8a0: 7228 0d0a 2020 2020 2020 2020 2020 2020  r(..            
-0001b8b0: 2020 2020 2743 6f75 6c64 206e 6f74 2066      'Could not f
-0001b8c0: 696e 6420 636f 6e66 6967 2066 696c 6520  ind config file 
-0001b8d0: 227b 7d22 2069 6e20 696d 6167 6520 6469  "{}" in image di
-0001b8e0: 7265 6374 6f72 793a 2022 7b7d 2227 2e66  rectory: "{}"'.f
-0001b8f0: 6f72 6d61 7428 0d0a 2020 2020 2020 2020  ormat(..        
-0001b900: 2020 2020 2020 2020 2020 2020 636f 6e66              conf
-0001b910: 6967 5f6e 616d 652c 206f 732e 7061 7468  ig_name, os.path
-0001b920: 2e64 6972 6e61 6d65 2869 6d61 6765 5f70  .dirname(image_p
-0001b930: 6174 6829 0d0a 2020 2020 2020 2020 2020  ath)..          
-0001b940: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
-0001b950: 2020 2020 2029 0d0a 0d0a 2020 2020 6465       )....    de
-0001b960: 6620 5f73 7461 7274 5f66 696c 655f 6d6f  f _start_file_mo
-0001b970: 6e69 746f 7228 7365 6c66 2c20 6465 6c61  nitor(self, dela
-0001b980: 7929 3a0d 0a0d 0a20 2020 2020 2020 2069  y):....        i
-0001b990: 6620 706c 6174 666f 726d 2e73 7973 7465  f platform.syste
-0001b9a0: 6d28 2920 3d3d 2022 4461 7277 696e 223a  m() == "Darwin":
-0001b9b0: 2020 2320 6d61 634f 530d 0a20 2020 2020    # macOS..     
-0001b9c0: 2020 2020 2020 2073 7562 7072 6f63 6573         subproces
-0001b9d0: 732e 6361 6c6c 2828 226f 7065 6e22 2c20  s.call(("open", 
-0001b9e0: 7365 6c66 2e63 6f6e 6669 675f 7061 7468  self.config_path
-0001b9f0: 2929 0d0a 2020 2020 2020 2020 656c 6966  ))..        elif
-0001ba00: 2070 6c61 7466 6f72 6d2e 7379 7374 656d   platform.system
-0001ba10: 2829 203d 3d20 2257 696e 646f 7773 223a  () == "Windows":
-0001ba20: 2020 2320 5769 6e64 6f77 730d 0a20 2020    # Windows..   
-0001ba30: 2020 2020 2020 2020 206f 732e 7374 6172           os.star
-0001ba40: 7466 696c 6528 6f73 2e70 6174 682e 6e6f  tfile(os.path.no
-0001ba50: 726d 7061 7468 2873 656c 662e 636f 6e66  rmpath(self.conf
-0001ba60: 6967 5f70 6174 6829 290d 0a20 2020 2020  ig_path))..     
-0001ba70: 2020 2065 6c73 653a 2020 2320 6c69 6e75     else:  # linu
-0001ba80: 7820 7661 7269 616e 7473 0d0a 2020 2020  x variants..    
-0001ba90: 2020 2020 2020 2020 7375 6270 726f 6365          subproce
-0001baa0: 7373 2e63 616c 6c28 2822 7864 672d 6f70  ss.call(("xdg-op
-0001bab0: 656e 222c 2073 656c 662e 636f 6e66 6967  en", self.config
-0001bac0: 5f70 6174 6829 290d 0a0d 0a20 2020 2020  _path))....     
-0001bad0: 2020 2073 656c 662e 5946 4d20 3d20 756c     self.YFM = ul
-0001bae0: 2e5f 5961 6d6c 4669 6c65 4d6f 6e69 746f  ._YamlFileMonito
-0001baf0: 7228 7365 6c66 2e63 6f6e 6669 675f 7061  r(self.config_pa
-0001bb00: 7468 2c20 6465 6c61 7929 0d0a 2020 2020  th, delay)..    
-0001bb10: 2020 2020 7365 6c66 2e5f 6c6f 6728 2264      self._log("d
-0001bb20: 6562 7567 222c 2022 5079 7065 3a20 7374  ebug", "Pype: st
-0001bb30: 6172 7469 6e67 2063 6f6e 6669 6720 6669  arting config fi
-0001bb40: 6c65 206d 6f6e 6974 6f72 222c 2030 290d  le monitor", 0).
-0001bb50: 0a0d 0a20 2020 2064 6566 205f 6368 6563  ...    def _chec
-0001bb60: 6b5f 6469 7265 6374 6f72 795f 736b 6970  k_directory_skip
-0001bb70: 2873 656c 662c 2074 6167 2c20 736b 6970  (self, tag, skip
-0001bb80: 5f70 6174 7465 726e 2c20 6469 725f 7061  _pattern, dir_pa
-0001bb90: 7468 293a 0d0a 0d0a 2020 2020 2020 2020  th):....        
-0001bba0: 2323 2073 6b69 7020 6469 7265 6374 6f72  ## skip director
-0001bbb0: 6965 7320 7468 6174 2061 6c72 6561 6479  ies that already
-0001bbc0: 2063 6f6e 7461 696e 2073 7065 6369 6669   contain specifi
-0001bbd0: 6564 2066 696c 6573 0d0a 2020 2020 2020  ed files..      
-0001bbe0: 2020 6966 2073 6b69 705f 7061 7474 6572    if skip_patter
-0001bbf0: 6e2e 5f5f 636c 6173 735f 5f2e 5f5f 6e61  n.__class__.__na
-0001bc00: 6d65 5f5f 203d 3d20 2273 7472 223a 0d0a  me__ == "str":..
-0001bc10: 2020 2020 2020 2020 2020 2020 736b 6970              skip
-0001bc20: 5f70 6174 7465 726e 203d 205b 736b 6970  _pattern = [skip
-0001bc30: 5f70 6174 7465 726e 5d0d 0a20 2020 2020  _pattern]..     
-0001bc40: 2020 2065 6c69 6620 736b 6970 5f70 6174     elif skip_pat
-0001bc50: 7465 726e 2e5f 5f63 6c61 7373 5f5f 2e5f  tern.__class__._
-0001bc60: 5f6e 616d 655f 5f20 3d3d 2022 626f 6f6c  _name__ == "bool
-0001bc70: 223a 0d0a 2020 2020 2020 2020 2020 2020  ":..            
-0001bc80: 736b 6970 5f70 6174 7465 726e 203d 205b  skip_pattern = [
-0001bc90: 2222 5d0d 0a20 2020 2020 2020 2065 6c69  ""]..        eli
-0001bca0: 6620 736b 6970 5f70 6174 7465 726e 2e5f  f skip_pattern._
-0001bcb0: 5f63 6c61 7373 5f5f 2e5f 5f6e 616d 655f  _class__.__name_
-0001bcc0: 5f20 696e 205b 226c 6973 7422 2c20 2243  _ in ["list", "C
-0001bcd0: 6f6d 6d65 6e74 6564 5365 7122 5d3a 0d0a  ommentedSeq"]:..
-0001bce0: 2020 2020 2020 2020 2020 2020 736b 6970              skip
-0001bcf0: 5f70 6174 7465 726e 203d 2073 6b69 705f  _pattern = skip_
-0001bd00: 7061 7474 6572 6e0d 0a0d 0a20 2020 2020  pattern....     
-0001bd10: 2020 2066 696c 655f 7061 7474 6572 6e20     file_pattern 
-0001bd20: 3d20 5b5d 0d0a 2020 2020 2020 2020 666f  = []..        fo
-0001bd30: 7220 7061 7474 6572 6e20 696e 2073 6b69  r pattern in ski
-0001bd40: 705f 7061 7474 6572 6e3a 0d0a 2020 2020  p_pattern:..    
-0001bd50: 2020 2020 2020 2020 6669 6c65 5f70 6174          file_pat
-0001bd60: 7465 726e 2e61 7070 656e 6428 7061 7474  tern.append(patt
-0001bd70: 6572 6e20 2b20 225f 2220 2b20 7461 6729  ern + "_" + tag)
-0001bd80: 0d0a 0d0a 2020 2020 2020 2020 6669 6c65  ....        file
-0001bd90: 7061 7468 732c 2064 7570 6c69 6361 7465  paths, duplicate
-0001bda0: 7320 3d20 756c 2e5f 6669 6c65 5f77 616c  s = ul._file_wal
-0001bdb0: 6b65 7228 0d0a 2020 2020 2020 2020 2020  ker(..          
-0001bdc0: 2020 6469 725f 7061 7468 2c0d 0a20 2020    dir_path,..   
-0001bdd0: 2020 2020 2020 2020 2069 6e63 6c75 6465           include
-0001bde0: 3d66 696c 655f 7061 7474 6572 6e2c 0d0a  =file_pattern,..
-0001bdf0: 2020 2020 2020 2020 2020 2020 696e 636c              incl
-0001be00: 7564 655f 616c 6c3d 4661 6c73 652c 0d0a  ude_all=False,..
-0001be10: 2020 2020 2020 2020 2020 2020 6578 636c              excl
-0001be20: 7564 653d 5b22 7079 7065 5f63 6f6e 6669  ude=["pype_confi
-0001be30: 6722 2c20 2261 7474 7269 6275 7465 7322  g", "attributes"
-0001be40: 5d2c 0d0a 2020 2020 2020 2020 2020 2020  ],..            
-0001be50: 7079 7065 5f6d 6f64 653d 5472 7565 2c0d  pype_mode=True,.
-0001be60: 0a20 2020 2020 2020 2029 0d0a 0d0a 2020  .        )....  
-0001be70: 2020 2020 2020 6966 206c 656e 2866 696c        if len(fil
-0001be80: 6570 6174 6873 2920 3e20 303a 0d0a 2020  epaths) > 0:..  
-0001be90: 2020 2020 2020 2020 2020 6669 6c65 7320            files 
-0001bea0: 3d20 5b5d 0d0a 2020 2020 2020 2020 2020  = []..          
-0001beb0: 2020 666f 7220 6669 6c65 2069 6e20 6669    for file in fi
-0001bec0: 6c65 7061 7468 733a 0d0a 2020 2020 2020  lepaths:..      
-0001bed0: 2020 2020 2020 2020 2020 6669 6c65 732e            files.
-0001bee0: 6170 7065 6e64 286f 732e 7061 7468 2e62  append(os.path.b
-0001bef0: 6173 656e 616d 6528 6669 6c65 2929 0d0a  asename(file))..
-0001bf00: 2020 2020 2020 2020 2020 2020 7072 696e              prin
-0001bf10: 7428 275c 6e46 6f75 6e64 2065 7869 7374  t('\nFound exist
-0001bf20: 696e 6720 6669 6c65 7320 7b7d 202d 2073  ing files {} - s
-0001bf30: 6b69 7070 6564 5c6e 272e 666f 726d 6174  kipped\n'.format
-0001bf40: 2828 2a66 696c 6573 2c29 2929 0d0a 2020  ((*files,)))..  
-0001bf50: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0001bf60: 2054 7275 650d 0a20 2020 2020 2020 2065   True..        e
-0001bf70: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
-0001bf80: 2020 7265 7475 726e 2046 616c 7365 0d0a    return False..
-0001bf90: 0d0a 2020 2020 6465 6620 5f63 6865 636b  ..    def _check
-0001bfa0: 5f66 696e 616c 2873 656c 6629 3a0d 0a0d  _final(self):...
-0001bfb0: 0a20 2020 2020 2020 2023 2320 6368 6563  .        ## chec
-0001bfc0: 6b20 636f 6d70 6f6e 656e 7473 2062 6566  k components bef
-0001bfd0: 6f72 6520 7374 6172 7469 6e67 2070 7970  ore starting pyp
-0001bfe0: 6520 746f 2073 6565 2069 6620 736f 6d65  e to see if some
-0001bff0: 7468 696e 6720 7765 6e74 2077 726f 6e67  thing went wrong
-0001c000: 0d0a 2020 2020 2020 2020 6966 2028 0d0a  ..        if (..
-0001c010: 2020 2020 2020 2020 2020 2020 6e6f 7420              not 
-0001c020: 6861 7361 7474 7228 7365 6c66 2e63 6f6e  hasattr(self.con
-0001c030: 7461 696e 6572 2c20 2269 6d61 6765 2229  tainer, "image")
-0001c040: 0d0a 2020 2020 2020 2020 2020 2020 6f72  ..            or
-0001c050: 2073 656c 662e 636f 6e74 6169 6e65 722e   self.container.
-0001c060: 696d 6167 652e 5f5f 636c 6173 735f 5f2e  image.__class__.
-0001c070: 5f5f 6e61 6d65 5f5f 203d 3d20 224e 6f6e  __name__ == "Non
-0001c080: 6554 7970 6522 0d0a 2020 2020 2020 2020  eType"..        
-0001c090: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-0001c0a0: 7261 6973 6520 4174 7472 6962 7574 6545  raise AttributeE
-0001c0b0: 7272 6f72 2822 4e6f 2069 6d61 6765 2077  rror("No image w
-0001c0c0: 6173 206c 6f61 6465 6422 290d 0a20 2020  as loaded")..   
-0001c0d0: 2020 2020 2020 2020 2072 6574 7572 6e0d           return.
-0001c0e0: 0a20 2020 2020 2020 2069 6620 280d 0a20  .        if (.. 
-0001c0f0: 2020 2020 2020 2020 2020 206e 6f74 2068             not h
-0001c100: 6173 6174 7472 2873 656c 662e 636f 6e74  asattr(self.cont
-0001c110: 6169 6e65 722c 2022 6469 725f 7061 7468  ainer, "dir_path
-0001c120: 2229 0d0a 2020 2020 2020 2020 2020 2020  ")..            
-0001c130: 6f72 2073 656c 662e 636f 6e74 6169 6e65  or self.containe
-0001c140: 722e 6469 725f 7061 7468 2e5f 5f63 6c61  r.dir_path.__cla
-0001c150: 7373 5f5f 2e5f 5f6e 616d 655f 5f20 3d3d  ss__.__name__ ==
-0001c160: 2022 4e6f 6e65 5479 7065 220d 0a20 2020   "NoneType"..   
-0001c170: 2020 2020 2029 3a0d 0a20 2020 2020 2020       ):..       
-0001c180: 2020 2020 2072 6169 7365 2041 7474 7269       raise Attri
-0001c190: 6275 7465 4572 726f 7228 2243 6f75 6c64  buteError("Could
-0001c1a0: 206e 6f74 2064 6574 6572 6d69 6e65 2064   not determine d
-0001c1b0: 6972 5f70 6174 6820 746f 2073 6176 6520  ir_path to save 
-0001c1c0: 6f75 7470 7574 2e22 290d 0a20 2020 2020  output.")..     
-0001c1d0: 2020 2020 2020 2072 6574 7572 6e0d 0a20         return.. 
-0001c1e0: 2020 2020 2020 2069 6620 6e6f 7420 6861         if not ha
-0001c1f0: 7361 7474 7228 7365 6c66 2c20 2263 6f6e  sattr(self, "con
-0001c200: 6669 6722 2920 6f72 2073 656c 662e 636f  fig") or self.co
-0001c210: 6e66 6967 2e5f 5f63 6c61 7373 5f5f 2e5f  nfig.__class__._
-0001c220: 5f6e 616d 655f 5f20 3d3d 2022 4e6f 6e65  _name__ == "None
-0001c230: 5479 7065 223a 0d0a 2020 2020 2020 2020  Type":..        
-0001c240: 2020 2020 7261 6973 6520 4174 7472 6962      raise Attrib
-0001c250: 7574 6545 7272 6f72 280d 0a20 2020 2020  uteError(..     
-0001c260: 2020 2020 2020 2020 2020 2022 4e6f 2063             "No c
-0001c270: 6f6e 6669 6720 6669 6c65 2077 6173 2070  onfig file was p
-0001c280: 726f 7669 6465 6420 6f72 206c 6f61 6469  rovided or loadi
-0001c290: 6e67 2063 6f6e 6669 6720 6469 6420 6e6f  ng config did no
-0001c2a0: 7420 7375 6363 6565 642e 220d 0a20 2020  t succeed."..   
-0001c2b0: 2020 2020 2020 2020 2029 0d0a 2020 2020           )..    
-0001c2c0: 2020 2020 2020 2020 7265 7475 726e 0d0a          return..
-0001c2d0: 2020 2020 2020 2020 0d0a 2020 2020 6465          ..    de
-0001c2e0: 6620 5f6c 6f67 2873 656c 662c 206c 766c  f _log(self, lvl
-0001c2f0: 2c20 6d65 7373 6167 6573 2c20 696e 643d  , messages, ind=
-0001c300: 302c 2070 6173 7374 6872 6f75 6768 3d46  0, passthrough=F
-0001c310: 616c 7365 293a 0d0a 2020 2020 2020 2020  alse):..        
-0001c320: 0d0a 2020 2020 2020 2020 2222 2241 6464  ..        """Add
-0001c330: 2061 206d 6573 7361 6765 2074 6f20 6120   a message to a 
-0001c340: 6c6f 6767 696e 6720 6f62 6a65 6374 2e0d  logging object..
-0001c350: 0a0d 0a20 2020 2020 2020 2050 6172 616d  ...        Param
-0001c360: 6574 6572 733a 0d0a 2020 2020 2020 2020  eters:..        
-0001c370: 6c6f 6767 696e 6720 286c 6f67 6769 6e67  logging (logging
-0001c380: 2e4c 6f67 6765 7229 3a20 5468 6520 6c6f  .Logger): The lo
-0001c390: 6767 696e 6720 6f62 6a65 6374 2074 6f20  gging object to 
-0001c3a0: 6164 6420 7468 6520 6d65 7373 6167 6520  add the message 
-0001c3b0: 746f 2e0d 0a20 2020 2020 2020 206d 6573  to...        mes
-0001c3c0: 7361 6765 2028 7374 7229 3a20 5468 6520  sage (str): The 
-0001c3d0: 6d65 7373 6167 6520 746f 2062 6520 6c6f  message to be lo
-0001c3e0: 6767 6564 2e0d 0a0d 0a20 2020 2020 2020  gged.....       
-0001c3f0: 2022 2222 0d0a 0d0a 2020 2020 2020 2020   """....        
-0001c400: 6966 2069 7369 6e73 7461 6e63 6528 6d65  if isinstance(me
-0001c410: 7373 6167 6573 2c20 7374 7229 3a0d 0a20  ssages, str):.. 
-0001c420: 2020 2020 2020 2020 2020 206d 6573 7361             messa
-0001c430: 6765 735f 6c69 7374 203d 206d 6573 7361  ges_list = messa
-0001c440: 6765 732e 7370 6c69 7428 225c 6e22 290d  ges.split("\n").
-0001c450: 0a20 2020 2020 2020 2065 6c69 6620 6973  .        elif is
-0001c460: 696e 7374 616e 6365 286d 6573 7361 6765  instance(message
-0001c470: 732c 206c 6973 7429 3a0d 0a20 2020 2020  s, list):..     
-0001c480: 2020 2020 2020 206d 6573 7361 6765 735f         messages_
-0001c490: 6c69 7374 203d 206d 6573 7361 6765 730d  list = messages.
-0001c4a0: 0a20 2020 2020 2020 2020 2020 200d 0a20  .            .. 
-0001c4b0: 2020 2020 2020 2066 6f72 206d 6573 7361         for messa
-0001c4c0: 6765 2069 6e20 6d65 7373 6167 6573 5f6c  ge in messages_l
-0001c4d0: 6973 743a 0d0a 2020 2020 2020 2020 2020  ist:..          
-0001c4e0: 2020 6966 206e 6f74 206d 6573 7361 6765    if not message
-0001c4f0: 203d 3d20 2222 3a0d 0a20 2020 2020 2020   == "":..       
-0001c500: 2020 2020 2020 2020 2069 6620 6d65 7373           if mess
-0001c510: 6167 652e 656e 6473 7769 7468 2822 5c6e  age.endswith("\n
-0001c520: 2229 3a0d 0a20 2020 2020 2020 2020 2020  "):..           
-0001c530: 2020 2020 2020 2020 206d 6573 7361 6765           message
-0001c540: 203d 206d 6573 7361 6765 5b3a 2d32 5d0d   = message[:-2].
-0001c550: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001c560: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-0001c570: 2020 206d 6573 7361 6765 203d 2028 2220     message = (" 
-0001c580: 2020 2022 202a 2069 6e64 2920 2b20 6d65     " * ind) + me
-0001c590: 7373 6167 650d 0a20 2020 2020 2020 2020  ssage..         
-0001c5a0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
-0001c5b0: 2020 2020 2069 6620 6c76 6c20 3d3d 2022       if lvl == "
-0001c5c0: 6465 6275 6722 3a0d 0a20 2020 2020 2020  debug":..       
-0001c5d0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0001c5e0: 662e 6c6f 6767 6572 2e64 6562 7567 286d  f.logger.debug(m
-0001c5f0: 6573 7361 6765 290d 0a20 2020 2020 2020  essage)..       
-0001c600: 2020 2020 2020 2020 2065 6c69 6620 6c76           elif lv
-0001c610: 6c20 3d3d 2022 696e 666f 223a 0d0a 2020  l == "info":..  
-0001c620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c630: 2020 7365 6c66 2e6c 6f67 6765 722e 696e    self.logger.in
-0001c640: 666f 286d 6573 7361 6765 290d 0a20 2020  fo(message)..   
-0001c650: 2020 2020 2020 2020 2020 2020 2065 6c69               eli
-0001c660: 6620 6c76 6c20 3d3d 2022 7761 726e 696e  f lvl == "warnin
-0001c670: 6722 3a0d 0a20 2020 2020 2020 2020 2020  g":..           
-0001c680: 2020 2020 2020 2020 2073 656c 662e 6c6f           self.lo
-0001c690: 6767 6572 2e77 6172 6e69 6e67 286d 6573  gger.warning(mes
-0001c6a0: 7361 6765 290d 0a20 2020 2020 2020 2020  sage)..         
-0001c6b0: 2020 2020 2020 2065 6c69 6620 6c76 6c20         elif lvl 
-0001c6c0: 3d3d 2022 6572 726f 7222 3a0d 0a20 2020  == "error":..   
-0001c6d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001c6e0: 2073 656c 662e 6c6f 6767 6572 2e65 7272   self.logger.err
-0001c6f0: 6f72 286d 6573 7361 6765 290d 0a20 2020  or(message)..   
-0001c700: 2020 2020 2020 2020 2020 2020 2065 6c69               eli
-0001c710: 6620 6c76 6c20 3d3d 2022 6372 6974 6963  f lvl == "critic
-0001c720: 616c 223a 0d0a 2020 2020 2020 2020 2020  al":..          
-0001c730: 2020 2020 2020 2020 2020 7365 6c66 2e6c            self.l
-0001c740: 6f67 6765 722e 6372 6974 6963 616c 286d  ogger.critical(m
-0001c750: 6573 7361 6765 290d 0a20 2020 2020 2020  essage)..       
-0001c760: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
-0001c770: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0001c780: 6620 7365 6c66 2e66 6c61 6773 2e66 6565  f self.flags.fee
-0001c790: 6462 6163 6b3d 3d46 616c 7365 2061 6e64  dback==False and
-0001c7a0: 2070 6173 7374 6872 6f75 6768 3d3d 5472   passthrough==Tr
-0001c7b0: 7565 3a0d 0a20 2020 2020 2020 2020 2020  ue:..           
-0001c7c0: 2020 2020 2020 2020 2068 6d20 3d20 6461           hm = da
-0001c7d0: 7465 7469 6d65 2e74 6f64 6179 2829 2e73  tetime.today().s
-0001c7e0: 7472 6674 696d 6528 2225 483a 254d 3a25  trftime("%H:%M:%
-0001c7f0: 5322 290d 0a20 2020 2020 2020 2020 2020  S")..           
-0001c800: 2020 2020 2020 2020 2070 7269 6e74 2868           print(h
-0001c810: 6d20 2b20 223a 2022 202b 206d 6573 7361  m + ": " + messa
-0001c820: 6765 290d 0a0d 0a0d 0a20 2020 2064 6566  ge)......    def
-0001c830: 205f 6974 6572 6174 6528 0d0a 2020 2020   _iterate(..    
-0001c840: 2020 2020 7365 6c66 2c20 0d0a 2020 2020      self, ..    
-0001c850: 2020 2020 616e 6e6f 7461 7469 6f6e 732c      annotations,
-0001c860: 200d 0a20 2020 2020 2020 2065 7865 6375   ..        execu
-0001c870: 7465 3d54 7275 652c 200d 0a20 2020 2020  te=True, ..     
-0001c880: 2020 2061 7574 6f73 686f 773d 5472 7565     autoshow=True
-0001c890: 2c20 0d0a 2020 2020 2020 2020 696e 7465  , ..        inte
-0001c8a0: 7261 6374 6976 653d 5472 7565 2c0d 0a20  ractive=True,.. 
-0001c8b0: 2020 2029 3a0d 0a0d 0a20 2020 2020 2020     ):....       
-0001c8c0: 2066 6c61 6773 203d 206d 616b 655f 6461   flags = make_da
-0001c8d0: 7461 636c 6173 7328 0d0a 2020 2020 2020  taclass(..      
-0001c8e0: 2020 2020 2020 636c 735f 6e61 6d65 3d22        cls_name="
-0001c8f0: 666c 6167 7322 2c0d 0a20 2020 2020 2020  flags",..       
-0001c900: 2020 2020 2066 6965 6c64 733d 5b0d 0a20       fields=[.. 
-0001c910: 2020 2020 2020 2020 2020 2020 2020 2028                 (
-0001c920: 2265 7865 6375 7465 222c 2062 6f6f 6c2c  "execute", bool,
-0001c930: 2065 7865 6375 7465 292c 0d0a 2020 2020   execute),..    
-0001c940: 2020 2020 2020 2020 2020 2020 2822 6175              ("au
-0001c950: 746f 7368 6f77 222c 2062 6f6f 6c2c 2061  toshow", bool, a
-0001c960: 7574 6f73 686f 7729 2c0d 0a20 2020 2020  utoshow),..     
-0001c970: 2020 2020 2020 2020 2020 2028 2269 6e74             ("int
-0001c980: 6572 6163 7469 7665 222c 2062 6f6f 6c2c  eractive", bool,
-0001c990: 2069 6e74 6572 6163 7469 7665 292c 0d0a   interactive),..
-0001c9a0: 2020 2020 2020 2020 2020 2020 5d2c 0d0a              ],..
-0001c9b0: 2020 2020 2020 2020 290d 0a0d 0a20 2020          )....   
-0001c9c0: 2020 2020 2023 203d 3d3d 3d3d 3d3d 3d3d       # =========
-0001c9d0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0001c9e0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0001c9f0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00018f40: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00018f50: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00018f60: 0d0a 2020 2020 2020 2020 2320 494e 4954  ..        # INIT
+00018f70: 0d0a 0d0a 2020 2020 2020 2020 2323 206b  ....        ## k
+00018f80: 7761 7267 730d 0a20 2020 2020 2020 2063  wargs..        c
+00018f90: 6f6e 6669 672e 7769 6e64 6f77 5f6d 696e  onfig.window_min
+00018fa0: 5f64 696d 203d 206b 7761 7267 732e 6765  _dim = kwargs.ge
+00018fb0: 7428 2277 696e 646f 775f 6d61 785f 6469  t("window_max_di
+00018fc0: 6d22 2c20 636f 6e66 6967 2e77 696e 646f  m", config.windo
+00018fd0: 775f 6d69 6e5f 6469 6d29 0d0a 2020 2020  w_min_dim)..    
+00018fe0: 2020 2020 636f 6e66 6967 2e77 696e 646f      config.windo
+00018ff0: 775f 6d61 785f 6469 6d20 3d20 6b77 6172  w_max_dim = kwar
+00019000: 6773 2e67 6574 2822 7769 6e64 6f77 5f6d  gs.get("window_m
+00019010: 6178 5f64 696d 222c 2063 6f6e 6669 672e  ax_dim", config.
+00019020: 7769 6e64 6f77 5f6d 6178 5f64 696d 290d  window_max_dim).
+00019030: 0a20 2020 2020 2020 2064 656c 6179 203d  .        delay =
+00019040: 206b 7761 7267 732e 6765 7428 2264 656c   kwargs.get("del
+00019050: 6179 222c 2031 3030 290d 0a20 2020 2020  ay", 100)..     
+00019060: 2020 200d 0a20 2020 2020 2020 2023 2320     ..        ## 
+00019070: 666c 6167 730d 0a20 2020 2020 2020 2073  flags..        s
+00019080: 656c 662e 666c 6167 7320 3d20 6d61 6b65  elf.flags = make
+00019090: 5f64 6174 6163 6c61 7373 280d 0a20 2020  _dataclass(..   
+000190a0: 2020 2020 2020 2020 2063 6c73 5f6e 616d           cls_nam
+000190b0: 653d 2266 6c61 6773 222c 0d0a 2020 2020  e="flags",..    
+000190c0: 2020 2020 2020 2020 6669 656c 6473 3d5b          fields=[
+000190d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000190e0: 2020 2822 6465 6275 6722 2c20 626f 6f6c    ("debug", bool
+000190f0: 2c20 6465 6275 6729 2c0d 0a20 2020 2020  , debug),..     
+00019100: 2020 2020 2020 2020 2020 2028 2261 7574             ("aut
+00019110: 6f6c 6f61 6422 2c20 626f 6f6c 2c20 6175  oload", bool, au
+00019120: 746f 6c6f 6164 292c 0d0a 2020 2020 2020  toload),..      
+00019130: 2020 2020 2020 2020 2020 2822 6175 746f            ("auto
+00019140: 7361 7665 222c 2062 6f6f 6c2c 2061 7574  save", bool, aut
+00019150: 6f73 6176 6529 2c0d 0a20 2020 2020 2020  osave),..       
+00019160: 2020 2020 2020 2020 2028 2261 7574 6f73           ("autos
+00019170: 686f 7722 2c20 626f 6f6c 2c20 6175 746f  how", bool, auto
+00019180: 7368 6f77 292c 0d0a 2020 2020 2020 2020  show),..        
+00019190: 2020 2020 2020 2020 2822 6665 6564 6261          ("feedba
+000191a0: 636b 222c 2062 6f6f 6c2c 2066 6565 6462  ck", bool, feedb
+000191b0: 6163 6b29 2c0d 0a20 2020 2020 2020 2020  ack),..         
+000191c0: 2020 2020 2020 2028 2269 6e74 6572 6163         ("interac
+000191d0: 7469 7665 222c 2062 6f6f 6c2c 2069 6e74  tive", bool, int
+000191e0: 6572 6163 7469 7665 292c 0d0a 2020 2020  eractive),..    
+000191f0: 2020 2020 2020 2020 2020 2020 2822 6669              ("fi
+00019200: 785f 6e61 6d65 7322 2c20 626f 6f6c 2c20  x_names", bool, 
+00019210: 6669 785f 6e61 6d65 7329 2c0d 0a20 2020  fix_names),..   
+00019220: 2020 2020 2020 2020 2020 2020 2028 2273               ("s
+00019230: 6b69 7022 2c20 626f 6f6c 2c20 736b 6970  kip", bool, skip
+00019240: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
+00019250: 2020 2020 2822 7a6f 6f6d 5f6d 656d 6f72      ("zoom_memor
+00019260: 7922 2c20 626f 6f6c 2c20 7a6f 6f6d 5f6d  y", bool, zoom_m
+00019270: 656d 6f72 7929 2c0d 0a20 2020 2020 2020  emory),..       
+00019280: 2020 2020 2020 2020 2028 2264 7279 5f72           ("dry_r
+00019290: 756e 222c 2062 6f6f 6c2c 206b 7761 7267  un", bool, kwarg
+000192a0: 732e 6765 7428 2264 7279 5f72 756e 222c  s.get("dry_run",
+000192b0: 2046 616c 7365 2929 2c0d 0a20 2020 2020   False)),..     
+000192c0: 2020 2020 2020 2020 2020 2028 2274 6572             ("ter
+000192d0: 6d69 6e61 7465 222c 2062 6f6f 6c2c 2046  minate", bool, F
+000192e0: 616c 7365 292c 0d0a 2020 2020 2020 2020  alse),..        
+000192f0: 2020 2020 5d2c 0d0a 2020 2020 2020 2020      ],..        
+00019300: 290d 0a20 2020 2020 2020 200d 0a20 2020  )..        ..   
+00019310: 2020 2020 2069 6620 7365 6c66 2e66 6c61       if self.fla
+00019320: 6773 2e64 6562 7567 3a0d 0a20 2020 2020  gs.debug:..     
+00019330: 2020 2020 2020 2073 656c 662e 7665 7262         self.verb
+00019340: 6f73 6520 3d20 636f 6e66 6967 2e76 6572  ose = config.ver
+00019350: 626f 7365 0d0a 2020 2020 2020 2020 2020  bose..          
+00019360: 2020 636f 6e66 6967 2e76 6572 626f 7365    config.verbose
+00019370: 203d 2054 7275 650d 0a20 2020 2020 2020   = True..       
+00019380: 2020 2020 200d 0a20 2020 2020 2020 2069       ..        i
+00019390: 6620 696d 6167 655f 7061 7468 2e5f 5f63  f image_path.__c
+000193a0: 6c61 7373 5f5f 2e5f 5f6e 616d 655f 5f20  lass__.__name__ 
+000193b0: 3d3d 2022 7374 7222 3a0d 0a20 2020 2020  == "str":..     
+000193c0: 2020 2020 2020 2069 6d61 6765 5f70 6174         image_pat
+000193d0: 6820 3d20 6f73 2e70 6174 682e 6162 7370  h = os.path.absp
+000193e0: 6174 6828 696d 6167 655f 7061 7468 290d  ath(image_path).
+000193f0: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
+00019400: 6469 725f 7061 7468 3a0d 0a20 2020 2020  dir_path:..     
+00019410: 2020 2020 2020 2064 6972 5f70 6174 6820         dir_path 
+00019420: 3d20 6f73 2e70 6174 682e 6469 726e 616d  = os.path.dirnam
+00019430: 6528 696d 6167 655f 7061 7468 290d 0a0d  e(image_path)...
+00019440: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00019450: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+00019460: 2020 2023 203d 3d3d 3d3d 3d3d 3d3d 3d3d     # ===========
+00019470: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00019480: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00019490: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000194a0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000194b0: 3d3d 0d0a 2020 2020 2020 2020 2320 4c4f  ==..        # LO
+000194c0: 4747 494e 470d 0a20 2020 2020 2020 2020  GGING..         
+000194d0: 2020 200d 0a20 2020 2020 2020 2023 2320     ..        ## 
+000194e0: 7374 6172 7420 6c6f 6767 696e 670d 0a20  start logging.. 
+000194f0: 2020 2020 2020 2073 656c 662e 6c6f 6767         self.logg
+00019500: 6572 203d 206c 6f67 6769 6e67 2e67 6574  er = logging.get
+00019510: 4c6f 6767 6572 2829 0d0a 2020 2020 2020  Logger()..      
+00019520: 2020 7365 6c66 2e6c 6f67 6765 722e 7365    self.logger.se
+00019530: 744c 6576 656c 286c 6f67 6769 6e67 2e49  tLevel(logging.I
+00019540: 4e46 4f29 0d0a 2020 2020 2020 2020 6966  NFO)..        if
+00019550: 2028 7365 6c66 2e6c 6f67 6765 722e 6861   (self.logger.ha
+00019560: 7348 616e 646c 6572 7328 2929 3a0d 0a20  sHandlers()):.. 
+00019570: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00019580: 6c6f 6767 6572 2e68 616e 646c 6572 732e  logger.handlers.
+00019590: 636c 6561 7228 290d 0a20 2020 2020 2020  clear()..       
+000195a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000195b0: 200d 0a20 2020 2020 2020 2069 6620 7365   ..        if se
+000195c0: 6c66 2e66 6c61 6773 2e66 6565 6462 6163  lf.flags.feedbac
+000195d0: 6b3a 0d0a 2020 2020 2020 2020 2020 2020  k:..            
+000195e0: 7374 646f 7574 5f68 616e 646c 6572 203d  stdout_handler =
+000195f0: 206c 6f67 6769 6e67 2e53 7472 6561 6d48   logging.StreamH
+00019600: 616e 646c 6572 2873 7973 2e73 7464 6f75  andler(sys.stdou
+00019610: 7429 0d0a 2020 2020 2020 2020 2020 2020  t)..            
+00019620: 7374 646f 7574 5f68 616e 646c 6572 2e73  stdout_handler.s
+00019630: 6574 4c65 7665 6c28 6c6f 6767 696e 672e  etLevel(logging.
+00019640: 4445 4255 4729 0d0a 2020 2020 2020 2020  DEBUG)..        
+00019650: 2020 2020 7374 646f 7574 5f66 6f72 6d61      stdout_forma
+00019660: 7474 6572 203d 206c 6f67 6769 6e67 2e46  tter = logging.F
+00019670: 6f72 6d61 7474 6572 2827 2528 6173 6374  ormatter('%(asct
+00019680: 696d 6529 733a 2025 286d 6573 7361 6765  ime)s: %(message
+00019690: 2973 272c 2022 2548 3a25 4d3a 2553 2229  )s', "%H:%M:%S")
+000196a0: 0d0a 2020 2020 2020 2020 2020 2020 7374  ..            st
+000196b0: 646f 7574 5f68 616e 646c 6572 2e73 6574  dout_handler.set
+000196c0: 466f 726d 6174 7465 7228 7374 646f 7574  Formatter(stdout
+000196d0: 5f66 6f72 6d61 7474 6572 290d 0a20 2020  _formatter)..   
+000196e0: 2020 2020 2020 2020 2073 656c 662e 6c6f           self.lo
+000196f0: 6767 6572 2e61 6464 4861 6e64 6c65 7228  gger.addHandler(
+00019700: 7374 646f 7574 5f68 616e 646c 6572 290d  stdout_handler).
+00019710: 0a0d 0a20 2020 2020 2020 2023 2320 6c6f  ...        ## lo
+00019720: 6720 6669 6c65 0d0a 2020 2020 2020 2020  g file..        
+00019730: 6966 206f 732e 7061 7468 2e69 7364 6972  if os.path.isdir
+00019740: 2869 6d61 6765 5f70 6174 6829 3a0d 0a20  (image_path):.. 
+00019750: 2020 2020 2020 2020 2020 206c 6f67 5f66             log_f
+00019760: 696c 655f 7061 7468 203d 206f 732e 7061  ile_path = os.pa
+00019770: 7468 2e6a 6f69 6e28 696d 6167 655f 7061  th.join(image_pa
+00019780: 7468 2c20 6622 7079 7065 5f6c 6f67 735f  th, f"pype_logs_
+00019790: 7b74 6167 7d2e 6c6f 6722 290d 0a20 2020  {tag}.log")..   
+000197a0: 2020 2020 2065 6c69 6620 6f73 2e70 6174       elif os.pat
+000197b0: 682e 6973 6669 6c65 2869 6d61 6765 5f70  h.isfile(image_p
+000197c0: 6174 6829 3a0d 0a20 2020 2020 2020 2020  ath):..         
+000197d0: 2020 206c 6f67 5f66 696c 655f 7061 7468     log_file_path
+000197e0: 203d 206f 732e 7061 7468 2e6a 6f69 6e28   = os.path.join(
+000197f0: 6469 725f 7061 7468 2c20 6622 7079 7065  dir_path, f"pype
+00019800: 5f6c 6f67 735f 7b74 6167 7d2e 6c6f 6722  _logs_{tag}.log"
+00019810: 290d 0a0d 0a20 2020 2020 2020 2069 6620  )....        if 
+00019820: 6f73 2e70 6174 682e 6973 6669 6c65 286c  os.path.isfile(l
+00019830: 6f67 5f66 696c 655f 7061 7468 2920 616e  og_file_path) an
+00019840: 6420 6c6f 675f 6f77 3a0d 0a20 2020 2020  d log_ow:..     
+00019850: 2020 2020 2020 206f 732e 7265 6d6f 7665         os.remove
+00019860: 286c 6f67 5f66 696c 655f 7061 7468 290d  (log_file_path).
+00019870: 0a20 2020 2020 2020 2020 2020 200d 0a20  .            .. 
+00019880: 2020 2020 2020 2066 696c 655f 6861 6e64         file_hand
+00019890: 6c65 7220 3d20 6c6f 6767 696e 672e 4669  ler = logging.Fi
+000198a0: 6c65 4861 6e64 6c65 7228 6c6f 675f 6669  leHandler(log_fi
+000198b0: 6c65 5f70 6174 6829 0d0a 2020 2020 2020  le_path)..      
+000198c0: 2020 6669 6c65 5f68 616e 646c 6572 2e73    file_handler.s
+000198d0: 6574 4c65 7665 6c28 6c6f 6767 696e 672e  etLevel(logging.
+000198e0: 494e 464f 290d 0a20 2020 2020 2020 2066  INFO)..        f
+000198f0: 696c 655f 666f 726d 6174 7465 7220 3d20  ile_formatter = 
+00019900: 6c6f 6767 696e 672e 466f 726d 6174 7465  logging.Formatte
+00019910: 7228 275b 2528 6173 6374 696d 6529 735d  r('[%(asctime)s]
+00019920: 5b25 286c 6576 656c 6e61 6d65 2973 5d20  [%(levelname)s] 
+00019930: 2528 6d65 7373 6167 6529 7327 2c20 2225  %(message)s', "%
+00019940: 592d 256d 2d25 6420 2548 3a25 4d3a 2553  Y-%m-%d %H:%M:%S
+00019950: 2229 0d0a 2020 2020 2020 2020 6669 6c65  ")..        file
+00019960: 5f68 616e 646c 6572 2e73 6574 466f 726d  _handler.setForm
+00019970: 6174 7465 7228 6669 6c65 5f66 6f72 6d61  atter(file_forma
+00019980: 7474 6572 290d 0a20 2020 2020 2020 2073  tter)..        s
+00019990: 656c 662e 6c6f 6767 6572 2e61 6464 4861  elf.logger.addHa
+000199a0: 6e64 6c65 7228 6669 6c65 5f68 616e 646c  ndler(file_handl
+000199b0: 6572 290d 0a0d 0a20 2020 2020 2020 2023  er)....        #
+000199c0: 203d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d   ===============
+000199d0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000199e0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+000199f0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00019a00: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 0d0a  ==============..
+00019a10: 2020 2020 2020 2020 2320 4348 4543 4b53          # CHECKS
+00019a20: 200d 0a0d 0a20 2020 2020 2020 2023 2320   ....        ## 
+00019a30: 6368 6563 6b20 6e61 6d65 2c20 6c6f 6164  check name, load
+00019a40: 2063 6f6e 7461 696e 6572 2061 6e64 2063   container and c
+00019a50: 6f6e 6669 670d 0a20 2020 2020 2020 2075  onfig..        u
+00019a60: 6c2e 5f63 6865 636b 5f70 7970 655f 7461  l._check_pype_ta
+00019a70: 6728 7461 6729 0d0a 2020 2020 2020 2020  g(tag)..        
+00019a80: 7365 6c66 2e5f 6c6f 6164 5f63 6f6e 7461  self._load_conta
+00019a90: 696e 6572 2869 6d61 6765 5f70 6174 683d  iner(image_path=
+00019aa0: 696d 6167 655f 7061 7468 2c20 6469 725f  image_path, dir_
+00019ab0: 7061 7468 3d64 6972 5f70 6174 682c 2074  path=dir_path, t
+00019ac0: 6167 3d74 6167 290d 0a20 2020 2020 2020  ag=tag)..       
+00019ad0: 2073 656c 662e 5f6c 6f61 645f 636f 6e66   self._load_conf
+00019ae0: 6967 2869 6d61 6765 5f70 6174 683d 696d  ig(image_path=im
+00019af0: 6167 655f 7061 7468 2c20 7461 673d 7461  age_path, tag=ta
+00019b00: 672c 2063 6f6e 6669 675f 7061 7468 3d63  g, config_path=c
+00019b10: 6f6e 6669 675f 7061 7468 290d 0a0d 0a20  onfig_path).... 
+00019b20: 2020 2020 2020 2023 2063 6865 636b 2076         # check v
+00019b30: 6572 7369 6f6e 2c20 6c6f 6164 2063 6f6e  ersion, load con
+00019b40: 7461 696e 6572 2061 6e64 2063 6f6e 6669  tainer and confi
+00019b50: 670d 0a20 2020 2020 2020 2069 6620 7365  g..        if se
+00019b60: 6c66 2e66 6c61 6773 2e64 7279 5f72 756e  lf.flags.dry_run
+00019b70: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
+00019b80: 656c 662e 5f6c 6f61 645f 636f 6e66 6967  elf._load_config
+00019b90: 2869 6d61 6765 5f70 6174 682c 2074 6167  (image_path, tag
+00019ba0: 2c20 636f 6e66 6967 5f70 6174 6829 0d0a  , config_path)..
+00019bb0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00019bc0: 2e5f 6974 6572 6174 6528 616e 6e6f 7461  ._iterate(annota
+00019bd0: 7469 6f6e 733d 636f 7079 2e64 6565 7063  tions=copy.deepc
+00019be0: 6f70 7928 5f76 6172 732e 5f61 6e6e 6f74  opy(_vars._annot
+00019bf0: 6174 696f 6e5f 7479 7065 7329 2c0d 0a20  ation_types),.. 
+00019c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019c10: 2020 2020 2065 7865 6375 7465 3d46 616c       execute=Fal
+00019c20: 7365 2c20 6175 746f 7368 6f77 3d46 616c  se, autoshow=Fal
+00019c30: 7365 2c20 6665 6564 6261 636b 3d54 7275  se, feedback=Tru
+00019c40: 6529 0d0a 2020 2020 2020 2020 2020 2020  e)..            
+00019c50: 7265 7475 726e 0d0a 0d0a 2020 2020 2020  return....      
+00019c60: 2020 2323 2063 6865 636b 2077 6865 7468    ## check wheth
+00019c70: 6572 2064 6972 6563 746f 7279 2069 7320  er directory is 
+00019c80: 736b 6970 7065 640d 0a20 2020 2020 2020  skipped..       
+00019c90: 2069 6620 7365 6c66 2e66 6c61 6773 2e73   if self.flags.s
+00019ca0: 6b69 703a 0d0a 2020 2020 2020 2020 2020  kip:..          
+00019cb0: 2020 6966 2073 656c 662e 5f63 6865 636b    if self._check
+00019cc0: 5f64 6972 6563 746f 7279 5f73 6b69 7028  _directory_skip(
+00019cd0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00019ce0: 2020 7461 673d 7461 672c 2073 6b69 705f    tag=tag, skip_
+00019cf0: 7061 7474 6572 6e3d 736b 6970 2c20 6469  pattern=skip, di
+00019d00: 725f 7061 7468 3d73 656c 662e 636f 6e74  r_path=self.cont
+00019d10: 6169 6e65 722e 6469 725f 7061 7468 0d0a  ainer.dir_path..
+00019d20: 2020 2020 2020 2020 2020 2020 293a 0d0a              ):..
+00019d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00019d40: 7265 7475 726e 0d0a 2020 2020 2020 2020  return..        
+00019d50: 2020 2020 0d0a 2020 2020 2020 2020 2320      ..        # 
+00019d60: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00019d70: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00019d80: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00019d90: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00019da0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d0d 0a20  =============.. 
+00019db0: 2020 2020 2020 2023 2046 4545 4442 4143         # FEEDBAC
+00019dc0: 4b20 0d0a 2020 2020 2020 2020 0d0a 2020  K ..        ..  
+00019dd0: 2020 2020 2020 7374 6172 7475 705f 6d73        startup_ms
+00019de0: 675f 6c69 7374 203d 205b 5d0d 0a20 2020  g_list = []..   
+00019df0: 2020 2020 2073 7461 7274 7570 5f6d 7367       startup_msg
+00019e00: 5f6c 6973 742e 6170 7065 6e64 2875 6c2e  _list.append(ul.
+00019e10: 5f70 7072 696e 745f 6669 6c6c 5f68 6261  _pprint_fill_hba
+00019e20: 7228 7365 6c66 2e63 6f6e 7461 696e 6572  r(self.container
+00019e30: 2e69 6d61 6765 5f6e 616d 652c 2073 796d  .image_name, sym
+00019e40: 626f 6c3d 223d 222c 2072 6574 3d54 7275  bol="=", ret=Tru
+00019e50: 6529 290d 0a20 2020 2020 2020 2073 656c  e))..        sel
+00019e60: 662e 5f6c 6f67 2822 696e 666f 222c 2073  f._log("info", s
+00019e70: 7461 7274 7570 5f6d 7367 5f6c 6973 742c  tartup_msg_list,
+00019e80: 2030 2c20 7061 7373 7468 726f 7567 683d   0, passthrough=
+00019e90: 5472 7565 290d 0a20 2020 2020 2020 200d  True)..        .
+00019ea0: 0a20 2020 2020 2020 2023 203d 3d3d 3d3d  .        # =====
+00019eb0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00019ec0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00019ed0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00019ee0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00019ef0: 3d3d 3d3d 3d3d 3d3d 0d0a 0d0a 2020 2020  ========....    
+00019f00: 2020 2020 2323 206c 6f61 6420 6578 6973      ## load exis
+00019f10: 7469 6e67 2061 6e6e 6f74 6174 696f 6e73  ting annotations
+00019f20: 2074 6872 6f75 6768 2063 6f6e 7461 696e   through contain
+00019f30: 6572 0d0a 2020 2020 2020 2020 6966 2073  er..        if s
+00019f40: 656c 662e 666c 6167 732e 6175 746f 6c6f  elf.flags.autolo
+00019f50: 6164 3a0d 0a20 2020 2020 2020 2020 2020  ad:..           
+00019f60: 2073 656c 662e 5f6c 6f67 2822 696e 666f   self._log("info
+00019f70: 222c 2022 5079 7065 3a20 4155 544f 4c4f  ", "Pype: AUTOLO
+00019f80: 4144 222c 2030 290d 0a20 2020 2020 2020  AD", 0)..       
+00019f90: 2020 2020 2077 6974 6820 696f 2e53 7472       with io.Str
+00019fa0: 696e 6749 4f28 2920 6173 2062 7566 6665  ingIO() as buffe
+00019fb0: 722c 2072 6564 6972 6563 745f 7374 646f  r, redirect_stdo
+00019fc0: 7574 2862 7566 6665 7229 3a0d 0a20 2020  ut(buffer):..   
+00019fd0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
+00019fe0: 662e 636f 6e74 6169 6e65 722e 5f6c 6f61  f.container._loa
+00019ff0: 6428 636f 6e74 6f75 7273 3d6c 6f61 645f  d(contours=load_
+0001a000: 636f 6e74 6f75 7273 290d 0a20 2020 2020  contours)..     
+0001a010: 2020 2020 2020 2020 2020 2073 7464 6f75             stdou
+0001a020: 7420 3d20 6275 6666 6572 2e67 6574 7661  t = buffer.getva
+0001a030: 6c75 6528 290d 0a20 2020 2020 2020 2020  lue()..         
+0001a040: 2020 2020 2020 2073 656c 662e 5f6c 6f67         self._log
+0001a050: 2822 696e 666f 222c 2073 7464 6f75 742c  ("info", stdout,
+0001a060: 2031 290d 0a0d 0a20 2020 2020 2020 2023   1)....        #
+0001a070: 2320 6368 6563 6b20 7079 7065 2063 6f6e  # check pype con
+0001a080: 6669 6720 666f 7220 616e 6e6f 7461 7469  fig for annotati
+0001a090: 6f6e 730d 0a20 2020 2020 2020 2073 656c  ons..        sel
+0001a0a0: 662e 5f69 7465 7261 7465 280d 0a20 2020  f._iterate(..   
+0001a0b0: 2020 2020 2020 2020 2061 6e6e 6f74 6174           annotat
+0001a0c0: 696f 6e73 3d73 656c 662e 636f 6e74 6169  ions=self.contai
+0001a0d0: 6e65 722e 616e 6e6f 7461 7469 6f6e 732c  ner.annotations,
+0001a0e0: 0d0a 2020 2020 2020 2020 2020 2020 6578  ..            ex
+0001a0f0: 6563 7574 653d 4661 6c73 652c 0d0a 2020  ecute=False,..  
+0001a100: 2020 2020 2020 2020 2020 6175 746f 7368            autosh
+0001a110: 6f77 3d46 616c 7365 2c0d 0a20 2020 2020  ow=False,..     
+0001a120: 2020 2020 2020 2069 6e74 6572 6163 7469         interacti
+0001a130: 7665 3d46 616c 7365 2c0d 0a20 2020 2020  ve=False,..     
+0001a140: 2020 2029 0d0a 0d0a 2020 2020 2020 2020     )....        
+0001a150: 2323 2066 696e 616c 2063 6865 636b 2062  ## final check b
+0001a160: 6566 6f72 6520 7374 6172 7469 6e67 2070  efore starting p
+0001a170: 7970 650d 0a20 2020 2020 2020 2073 656c  ype..        sel
+0001a180: 662e 5f63 6865 636b 5f66 696e 616c 2829  f._check_final()
+0001a190: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
+0001a1a0: 2020 2020 2323 2074 7572 6e20 6f66 6620      ## turn off 
+0001a1b0: 6175 7473 686f 7720 616e 6420 6669 6c65  autshow and file
+0001a1c0: 206d 6f6e 6974 6f72 2069 6e20 6e6f 6e2d   monitor in non-
+0001a1d0: 696e 7465 7261 6374 6976 6520 6d6f 6465  interactive mode
+0001a1e0: 0d0a 2020 2020 2020 2020 6966 2073 656c  ..        if sel
+0001a1f0: 662e 666c 6167 732e 696e 7465 7261 6374  f.flags.interact
+0001a200: 6976 653a 0d0a 2020 2020 2020 2020 2020  ive:..          
+0001a210: 2020 7365 6c66 2e5f 7374 6172 745f 6669    self._start_fi
+0001a220: 6c65 5f6d 6f6e 6974 6f72 2864 656c 6179  le_monitor(delay
+0001a230: 3d64 656c 6179 290d 0a20 2020 2020 2020  =delay)..       
+0001a240: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
+0001a250: 2020 2020 7365 6c66 2e66 6c61 6773 2e61      self.flags.a
+0001a260: 7574 6f73 686f 7720 3d20 4661 6c73 650d  utoshow = False.
+0001a270: 0a20 2020 2020 2020 2020 2020 200d 0a20  .            .. 
+0001a280: 2020 2020 2020 2023 2320 636c 6561 7220         ## clear 
+0001a290: 6f6c 6420 7a6f 6f6d 206d 656d 6f72 790d  old zoom memory.
+0001a2a0: 0a20 2020 2020 2020 2063 6f6e 6669 672e  .        config.
+0001a2b0: 6775 695f 7a6f 6f6d 5f63 6f6e 6669 6720  gui_zoom_config 
+0001a2c0: 3d20 4e6f 6e65 0d0a 0d0a 2020 2020 2020  = None....      
+0001a2d0: 2020 2320 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d    # ============
+0001a2e0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0001a2f0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0001a300: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0001a310: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0001a320: 3d0d 0a20 2020 2020 2020 2023 2050 5950  =..        # PYP
+0001a330: 4520 4c4f 4f50 0d0a 0d0a 2020 2020 2020  E LOOP....      
+0001a340: 2020 2323 2072 756e 2070 7970 650d 0a20    ## run pype.. 
+0001a350: 2020 2020 2020 2077 6869 6c65 2054 7275         while Tru
+0001a360: 653a 0d0a 0d0a 2020 2020 2020 2020 2020  e:....          
+0001a370: 2020 2323 2070 7970 6520 7265 7374 6172    ## pype restar
+0001a380: 7420 666c 6167 0d0a 2020 2020 2020 2020  t flag..        
+0001a390: 2020 2020 636f 6e66 6967 2e70 7970 655f      config.pype_
+0001a3a0: 7265 7374 6172 7420 3d20 4661 6c73 650d  restart = False.
+0001a3b0: 0a0d 0a20 2020 2020 2020 2020 2020 2023  ...            #
+0001a3c0: 2320 7265 6672 6573 6820 636f 6e66 6967  # refresh config
+0001a3d0: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+0001a3e0: 2073 656c 662e 666c 6167 732e 696e 7465   self.flags.inte
+0001a3f0: 7261 6374 6976 653a 0d0a 0d0a 2020 2020  ractive:....    
+0001a400: 2020 2020 2020 2020 2020 2020 2323 2074              ## t
+0001a410: 6f20 7374 6f70 2069 6e66 696e 6974 6520  o stop infinite 
+0001a420: 6c6f 6f70 2077 6974 686f 7574 206f 7065  loop without ope
+0001a430: 6e69 6e67 206e 6577 2077 696e 646f 770d  ning new window.
+0001a440: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001a450: 2069 6620 6e6f 7420 7365 6c66 2e59 464d   if not self.YFM
+0001a460: 2e63 6f6e 7465 6e74 3a0d 0a20 2020 2020  .content:..     
+0001a470: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0001a480: 656c 662e 5f6c 6f67 2822 6465 6275 6722  elf._log("debug"
+0001a490: 2c20 2250 7970 653a 2053 5449 4c4c 2055  , "Pype: STILL U
+0001a4a0: 5044 4154 494e 4720 434f 4e46 4947 2028  PDATING CONFIG (
+0001a4b0: 6e6f 2063 6f6e 6669 6729 222c 2030 290d  no config)", 0).
+0001a4c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001a4d0: 2020 2020 2063 7632 2e64 6573 7472 6f79       cv2.destroy
+0001a4e0: 5769 6e64 6f77 2822 7068 656e 6f70 7970  Window("phenopyp
+0001a4f0: 6522 290d 0a20 2020 2020 2020 2020 2020  e")..           
+0001a500: 2020 2020 2020 2020 2074 696d 652e 736c           time.sl
+0001a510: 6565 7028 3129 0d0a 2020 2020 2020 2020  eep(1)..        
+0001a520: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0001a530: 2e59 464d 2e5f 7374 6f70 2829 0d0a 2020  .YFM._stop()..  
+0001a540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a550: 2020 7365 6c66 2e5f 7374 6172 745f 6669    self._start_fi
+0001a560: 6c65 5f6d 6f6e 6974 6f72 2864 656c 6179  le_monitor(delay
+0001a570: 3d64 656c 6179 290d 0a20 2020 2020 2020  =delay)..       
+0001a580: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
+0001a590: 7469 6e75 650d 0a0d 0a20 2020 2020 2020  tinue....       
+0001a5a0: 2020 2020 2020 2020 2073 656c 662e 636f           self.co
+0001a5b0: 6e66 6967 203d 2063 6f70 792e 6465 6570  nfig = copy.deep
+0001a5c0: 636f 7079 2873 656c 662e 5946 4d2e 636f  copy(self.YFM.co
+0001a5d0: 6e74 656e 7429 0d0a 0d0a 2020 2020 2020  ntent)....      
+0001a5e0: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
+0001a5f0: 2073 656c 662e 636f 6e66 6967 3a0d 0a20   self.config:.. 
+0001a600: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a610: 2020 2073 656c 662e 5f6c 6f67 2822 6465     self._log("de
+0001a620: 6275 6722 2c20 2250 7970 653a 2053 5449  bug", "Pype: STI
+0001a630: 4c4c 2055 5044 4154 494e 4720 434f 4e46  LL UPDATING CONF
+0001a640: 4947 2028 6e6f 2063 6f6e 6669 6729 222c  IG (no config)",
+0001a650: 2030 290d 0a20 2020 2020 2020 2020 2020   0)..           
+0001a660: 2020 2020 2020 2020 2063 6f6e 7469 6e75           continu
+0001a670: 650d 0a0d 0a20 2020 2020 2020 2020 2020  e....           
+0001a680: 2023 2320 7275 6e20 7079 7065 2063 6f6e   ## run pype con
+0001a690: 6669 6720 696e 2073 6571 7565 6e63 650d  fig in sequence.
+0001a6a0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0001a6b0: 662e 5f69 7465 7261 7465 280d 0a20 2020  f._iterate(..   
+0001a6c0: 2020 2020 2020 2020 2020 2020 2061 6e6e               ann
+0001a6d0: 6f74 6174 696f 6e73 3d73 656c 662e 636f  otations=self.co
+0001a6e0: 6e74 6169 6e65 722e 616e 6e6f 7461 7469  ntainer.annotati
+0001a6f0: 6f6e 732c 0d0a 2020 2020 2020 2020 2020  ons,..          
+0001a700: 2020 2020 2020 696e 7465 7261 6374 6976        interactiv
+0001a710: 653d 7365 6c66 2e66 6c61 6773 2e69 6e74  e=self.flags.int
+0001a720: 6572 6163 7469 7665 2c0d 0a20 2020 2020  eractive,..     
+0001a730: 2020 2020 2020 2020 2020 2061 7574 6f73             autos
+0001a740: 686f 773d 7365 6c66 2e66 6c61 6773 2e61  how=self.flags.a
+0001a750: 7574 6f73 686f 772c 0d0a 2020 2020 2020  utoshow,..      
+0001a760: 2020 2020 2020 290d 0a0d 0a20 2020 2020        )....     
+0001a770: 2020 2020 2020 2023 2320 7465 726d 696e         ## termin
+0001a780: 6174 6520 2620 636c 6561 6e75 700d 0a20  ate & cleanup.. 
+0001a790: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+0001a7a0: 6c66 2e66 6c61 6773 2e69 6e74 6572 6163  lf.flags.interac
+0001a7b0: 7469 7665 3a0d 0a20 2020 2020 2020 2020  tive:..         
+0001a7c0: 2020 2020 2020 2069 6620 7365 6c66 2e66         if self.f
+0001a7d0: 6c61 6773 2e74 6572 6d69 6e61 7465 3a0d  lags.terminate:.
+0001a7e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001a7f0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+0001a800: 2020 2020 2020 2020 2020 2023 2320 7374             ## st
+0001a810: 6f70 6520 6669 6c65 206d 6f6e 6974 6f72  ope file monitor
+0001a820: 696e 670d 0a20 2020 2020 2020 2020 2020  ing..           
+0001a830: 2020 2020 2020 2020 2069 6620 6861 7361           if hasa
+0001a840: 7474 7228 7365 6c66 2c20 2259 464d 2229  ttr(self, "YFM")
+0001a850: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+0001a860: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0001a870: 5946 4d2e 5f73 746f 7028 290d 0a20 2020  YFM._stop()..   
+0001a880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a890: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
+0001a8a0: 2020 2020 2020 2020 2020 2023 2320 7265             ## re
+0001a8b0: 7365 7420 7a6f 6f6d 2073 6574 7469 6e67  set zoom setting
+0001a8c0: 730d 0a20 2020 2020 2020 2020 2020 2020  s..             
+0001a8d0: 2020 2020 2020 2069 6620 6e6f 7420 7365         if not se
+0001a8e0: 6c66 2e66 6c61 6773 2e7a 6f6f 6d5f 6d65  lf.flags.zoom_me
+0001a8f0: 6d6f 7279 3a0d 0a20 2020 2020 2020 2020  mory:..         
+0001a900: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+0001a910: 6f6e 6669 672e 6775 695f 7a6f 6f6d 5f63  onfig.gui_zoom_c
+0001a920: 6f6e 6669 6720 3d20 4e6f 6e65 0d0a 2020  onfig = None..  
+0001a930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001a940: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+0001a950: 2020 2020 2020 2020 2323 2061 6464 200d          ## add .
+0001a960: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001a970: 2020 2020 2069 6620 2263 6f6e 6669 675f       if "config_
+0001a980: 696e 666f 2220 696e 2073 656c 662e 636f  info" in self.co
+0001a990: 6e66 6967 3a0d 0a20 2020 2020 2020 2020  nfig:..         
+0001a9a0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0001a9b0: 656c 662e 636f 6e66 6967 5b22 636f 6e66  elf.config["conf
+0001a9c0: 6967 5f69 6e66 6f22 5d5b 2264 6174 655f  ig_info"]["date_
+0001a9d0: 6c61 7374 5f6d 6f64 6966 6965 6422 5d20  last_modified"] 
+0001a9e0: 3d20 6461 7465 7469 6d65 2e74 6f64 6179  = datetime.today
+0001a9f0: 2829 2e73 7472 6674 696d 6528 5f76 6172  ().strftime(_var
+0001aa00: 732e 7374 7266 7469 6d65 5f66 6f72 6d61  s.strftime_forma
+0001aa10: 7429 0d0a 2020 2020 2020 2020 2020 2020  t)..            
+0001aa20: 2020 2020 2020 2020 756c 2e5f 7361 7665          ul._save
+0001aa30: 5f79 616d 6c28 7365 6c66 2e63 6f6e 6669  _yaml(self.confi
+0001aa40: 672c 2073 656c 662e 636f 6e66 6967 5f70  g, self.config_p
+0001aa50: 6174 6829 0d0a 2020 2020 2020 2020 2020  ath)..          
+0001aa60: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+0001aa70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001aa80: 2020 2020 2323 2066 6565 6462 6163 6b0d      ## feedback.
+0001aa90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001aaa0: 2020 2020 2073 656c 662e 5f6c 6f67 2822       self._log("
+0001aab0: 696e 666f 222c 2022 5079 7065 3a20 5445  info", "Pype: TE
+0001aac0: 524d 494e 4154 4522 2c20 3029 0d0a 2020  RMINATE", 0)..  
+0001aad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001aae0: 2020 6272 6561 6b0d 0a20 2020 2020 2020    break..       
+0001aaf0: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+0001ab00: 2020 2020 2020 2065 6c73 653a 0d0a 2020         else:..  
+0001ab10: 2020 2020 2020 2020 2020 2020 2020 6272                br
+0001ab20: 6561 6b0d 0a20 2020 2020 2020 2020 2020  eak..           
+0001ab30: 200d 0a20 2020 2020 2020 2023 203d 3d3d   ..        # ===
+0001ab40: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0001ab50: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0001ab60: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0001ab70: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0001ab80: 3d3d 3d3d 3d3d 3d3d 3d3d 0d0a 2020 2020  ==========..    
+0001ab90: 2020 2020 2323 2061 7574 6f73 6176 650d      ## autosave.
+0001aba0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+0001abb0: 2e66 6c61 6773 2e61 7574 6f73 6176 6520  .flags.autosave 
+0001abc0: 616e 6420 7365 6c66 2e66 6c61 6773 2e74  and self.flags.t
+0001abd0: 6572 6d69 6e61 7465 3a0d 0a20 2020 2020  erminate:..     
+0001abe0: 2020 2020 2020 2073 656c 662e 5f6c 6f67         self._log
+0001abf0: 2822 696e 666f 222c 2022 5079 7065 3a20  ("info", "Pype: 
+0001ac00: 4155 544f 5341 5645 222c 2030 290d 0a20  AUTOSAVE", 0).. 
+0001ac10: 2020 2020 2020 2020 2020 2069 6620 2265             if "e
+0001ac20: 7870 6f72 7422 206e 6f74 2069 6e20 7365  xport" not in se
+0001ac30: 6c66 2e63 6f6e 6669 675f 7061 7273 6564  lf.config_parsed
+0001ac40: 5f66 6c61 7474 656e 6564 3a0d 0a20 2020  _flattened:..   
+0001ac50: 2020 2020 2020 2020 2020 2020 2065 7870               exp
+0001ac60: 6f72 745f 6c69 7374 203d 205b 5d0d 0a20  ort_list = [].. 
+0001ac70: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+0001ac80: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001ac90: 2020 6578 706f 7274 5f6c 6973 7420 3d20    export_list = 
+0001aca0: 7365 6c66 2e63 6f6e 6669 675f 7061 7273  self.config_pars
+0001acb0: 6564 5f66 6c61 7474 656e 6564 5b22 6578  ed_flattened["ex
+0001acc0: 706f 7274 225d 0d0a 2020 2020 2020 2020  port"]..        
+0001acd0: 2020 2020 7769 7468 2069 6f2e 5374 7269      with io.Stri
+0001ace0: 6e67 494f 2829 2061 7320 6275 6666 6572  ngIO() as buffer
+0001acf0: 2c20 7265 6469 7265 6374 5f73 7464 6f75  , redirect_stdou
+0001ad00: 7428 6275 6666 6572 293a 0d0a 2020 2020  t(buffer):..    
+0001ad10: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0001ad20: 2e63 6f6e 7461 696e 6572 2e5f 7361 7665  .container._save
+0001ad30: 2865 7870 6f72 745f 6c69 7374 3d65 7870  (export_list=exp
+0001ad40: 6f72 745f 6c69 7374 290d 0a20 2020 2020  ort_list)..     
+0001ad50: 2020 2020 2020 2020 2020 2073 7464 6f75             stdou
+0001ad60: 7420 3d20 6275 6666 6572 2e67 6574 7661  t = buffer.getva
+0001ad70: 6c75 6528 290d 0a20 2020 2020 2020 2020  lue()..         
+0001ad80: 2020 2020 2020 2073 656c 662e 5f6c 6f67         self._log
+0001ad90: 2822 696e 666f 222c 2073 7464 6f75 742c  ("info", stdout,
+0001ada0: 2031 290d 0a20 2020 2020 2020 2020 2020   1)..           
+0001adb0: 2020 2020 200d 0a20 2020 2020 2020 2023       ..        #
+0001adc0: 203d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d   ===============
+0001add0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0001ade0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0001adf0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0001ae00: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 0d0a  ==============..
+0001ae10: 2020 2020 2020 2020 2320 4645 4544 4241          # FEEDBA
+0001ae20: 434b 200d 0a20 2020 2020 2020 200d 0a20  CK ..        .. 
+0001ae30: 2020 2020 2020 2073 7461 7274 7570 5f6d         startup_m
+0001ae40: 7367 5f6c 6973 7420 3d20 5b5d 0d0a 2020  sg_list = []..  
+0001ae50: 2020 2020 2020 7374 6172 7475 705f 6d73        startup_ms
+0001ae60: 675f 6c69 7374 2e61 7070 656e 6428 756c  g_list.append(ul
+0001ae70: 2e5f 7070 7269 6e74 5f66 696c 6c5f 6862  ._pprint_fill_hb
+0001ae80: 6172 2822 454e 4422 2c20 7379 6d62 6f6c  ar("END", symbol
+0001ae90: 3d22 3d22 2c20 7265 743d 5472 7565 2929  ="=", ret=True))
+0001aea0: 0d0a 2020 2020 2020 2020 7365 6c66 2e5f  ..        self._
+0001aeb0: 6c6f 6728 2269 6e66 6f22 2c20 7374 6172  log("info", star
+0001aec0: 7475 705f 6d73 675f 6c69 7374 2c20 3029  tup_msg_list, 0)
+0001aed0: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
+0001aee0: 2020 2020 2320 3d3d 3d3d 3d3d 3d3d 3d3d      # ==========
+0001aef0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0001af00: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0001af10: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0001af20: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0001af30: 3d3d 3d0d 0a0d 0a20 2020 2020 2020 2023  ===....        #
+0001af40: 2320 656e 6420 6c6f 6767 696e 670d 0a20  # end logging.. 
+0001af50: 2020 2020 2020 206c 6f67 6769 6e67 2e73         logging.s
+0001af60: 6875 7464 6f77 6e28 290d 0a20 2020 2020  hutdown()..     
+0001af70: 2020 200d 0a20 2020 2020 2020 2069 6620     ..        if 
+0001af80: 7365 6c66 2e66 6c61 6773 2e64 6562 7567  self.flags.debug
+0001af90: 3a0d 0a20 2020 2020 2020 2020 2020 2063  :..            c
+0001afa0: 6f6e 6669 672e 7665 7262 6f73 6520 3d20  onfig.verbose = 
+0001afb0: 7365 6c66 2e76 6572 626f 7365 0d0a 0d0a  self.verbose....
+0001afc0: 0d0a 2020 2020 6465 6620 5f6c 6f61 645f  ..    def _load_
+0001afd0: 636f 6e74 6169 6e65 7228 7365 6c66 2c20  container(self, 
+0001afe0: 696d 6167 655f 7061 7468 2c20 6469 725f  image_path, dir_
+0001aff0: 7061 7468 2c20 7461 6729 3a0d 0a20 2020  path, tag):..   
+0001b000: 2020 2020 2069 6620 696d 6167 655f 7061       if image_pa
+0001b010: 7468 2e5f 5f63 6c61 7373 5f5f 2e5f 5f6e  th.__class__.__n
+0001b020: 616d 655f 5f20 3d3d 2022 7374 7222 3a0d  ame__ == "str":.
+0001b030: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0001b040: 6f73 2e70 6174 682e 6973 6669 6c65 2869  os.path.isfile(i
+0001b050: 6d61 6765 5f70 6174 6829 3a0d 0a20 2020  mage_path):..   
+0001b060: 2020 2020 2020 2020 2020 2020 2069 6d61               ima
+0001b070: 6765 203d 2075 7469 6c73 2e6c 6f61 645f  ge = utils.load_
+0001b080: 696d 6167 6528 696d 6167 655f 7061 7468  image(image_path
+0001b090: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+0001b0a0: 2020 2073 656c 662e 636f 6e74 6169 6e65     self.containe
+0001b0b0: 7220 3d20 756c 2e5f 436f 6e74 6169 6e65  r = ul._Containe
+0001b0c0: 7228 0d0a 2020 2020 2020 2020 2020 2020  r(..            
+0001b0d0: 2020 2020 2020 2020 696d 6167 653d 696d          image=im
+0001b0e0: 6167 652c 0d0a 2020 2020 2020 2020 2020  age,..          
+0001b0f0: 2020 2020 2020 2020 2020 6469 725f 7061            dir_pa
+0001b100: 7468 3d64 6972 5f70 6174 682c 0d0a 2020  th=dir_path,..  
+0001b110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b120: 2020 7461 673d 7461 672c 0d0a 2020 2020    tag=tag,..    
+0001b130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b140: 6669 6c65 5f70 7265 6669 783d 6f73 2e70  file_prefix=os.p
+0001b150: 6174 682e 7370 6c69 7465 7874 286f 732e  ath.splitext(os.
+0001b160: 7061 7468 2e62 6173 656e 616d 6528 696d  path.basename(im
+0001b170: 6167 655f 7061 7468 2929 5b30 5d2c 0d0a  age_path))[0],..
+0001b180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b190: 2020 2020 6669 6c65 5f73 7566 6669 783d      file_suffix=
+0001b1a0: 7461 672c 0d0a 2020 2020 2020 2020 2020  tag,..          
+0001b1b0: 2020 2020 2020 2020 2020 696d 6167 655f            image_
+0001b1c0: 6e61 6d65 3d6f 732e 7061 7468 2e62 6173  name=os.path.bas
+0001b1d0: 656e 616d 6528 696d 6167 655f 7061 7468  ename(image_path
+0001b1e0: 292c 0d0a 2020 2020 2020 2020 2020 2020  ),..            
+0001b1f0: 2020 2020 290d 0a20 2020 2020 2020 2020      )..         
+0001b200: 2020 2065 6c69 6620 6f73 2e70 6174 682e     elif os.path.
+0001b210: 6973 6469 7228 696d 6167 655f 7061 7468  isdir(image_path
+0001b220: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+0001b230: 2020 2020 7365 6c66 2e63 6f6e 7461 696e      self.contain
+0001b240: 6572 203d 2075 6c2e 5f6c 6f61 645f 7072  er = ul._load_pr
+0001b250: 6f6a 6563 745f 696d 6167 655f 6469 7265  oject_image_dire
+0001b260: 6374 6f72 7928 0d0a 2020 2020 2020 2020  ctory(..        
+0001b270: 2020 2020 2020 2020 2020 2020 6469 725f              dir_
+0001b280: 7061 7468 3d69 6d61 6765 5f70 6174 682c  path=image_path,
+0001b290: 2074 6167 3d74 6167 2c0d 0a20 2020 2020   tag=tag,..     
+0001b2a0: 2020 2020 2020 2020 2020 2029 0d0a 2020             )..  
+0001b2b0: 2020 2020 2020 2020 2020 656c 7365 3a0d            else:.
+0001b2c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001b2d0: 2072 6169 7365 2046 696c 654e 6f74 466f   raise FileNotFo
+0001b2e0: 756e 6445 7272 6f72 280d 0a20 2020 2020  undError(..     
+0001b2f0: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+0001b300: 436f 756c 6420 6e6f 7420 6669 6e64 2069  Could not find i
+0001b310: 6d61 6765 206f 7220 696d 6167 6520 6469  mage or image di
+0001b320: 7265 6374 6f72 793a 2022 7b7d 2227 2e66  rectory: "{}"'.f
+0001b330: 6f72 6d61 7428 0d0a 2020 2020 2020 2020  ormat(..        
+0001b340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b350: 6f73 2e70 6174 682e 6469 726e 616d 6528  os.path.dirname(
+0001b360: 696d 6167 655f 7061 7468 290d 0a20 2020  image_path)..   
+0001b370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001b380: 2029 0d0a 2020 2020 2020 2020 2020 2020   )..            
+0001b390: 2020 2020 290d 0a20 2020 2020 2020 2065      )..        e
+0001b3a0: 6c69 6620 696d 6167 655f 7061 7468 2e5f  lif image_path._
+0001b3b0: 5f63 6c61 7373 5f5f 2e5f 5f6e 616d 655f  _class__.__name_
+0001b3c0: 5f20 3d3d 2022 5f43 6f6e 7461 696e 6572  _ == "_Container
+0001b3d0: 223a 0d0a 2020 2020 2020 2020 2020 2020  ":..            
+0001b3e0: 7365 6c66 2e63 6f6e 7461 696e 6572 203d  self.container =
+0001b3f0: 2063 6f70 792e 6465 6570 636f 7079 2869   copy.deepcopy(i
+0001b400: 6d61 6765 5f70 6174 6829 0d0a 2020 2020  mage_path)..    
+0001b410: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
+0001b420: 2020 2020 2020 2072 6169 7365 2054 7970         raise Typ
+0001b430: 6545 7272 6f72 2822 496e 7661 6c69 6420  eError("Invalid 
+0001b440: 696e 7075 7420 666f 7220 696d 6167 6520  input for image 
+0001b450: 7061 7468 2028 7374 7220 7265 7175 6972  path (str requir
+0001b460: 6564 2922 290d 0a0d 0a20 2020 2064 6566  ed)")....    def
+0001b470: 205f 6c6f 6164 5f63 6f6e 6669 6728 7365   _load_config(se
+0001b480: 6c66 2c20 696d 6167 655f 7061 7468 2c20  lf, image_path, 
+0001b490: 7461 672c 2063 6f6e 6669 675f 7061 7468  tag, config_path
+0001b4a0: 293a 0d0a 0d0a 2020 2020 2020 2020 6966  ):....        if
+0001b4b0: 2063 6f6e 6669 675f 7061 7468 2e5f 5f63   config_path.__c
+0001b4c0: 6c61 7373 5f5f 2e5f 5f6e 616d 655f 5f20  lass__.__name__ 
+0001b4d0: 3d3d 2022 4e6f 6e65 5479 7065 223a 0d0a  == "NoneType":..
+0001b4e0: 2020 2020 2020 2020 2020 2020 6966 206f              if o
+0001b4f0: 732e 7061 7468 2e69 7366 696c 6528 696d  s.path.isfile(im
+0001b500: 6167 655f 7061 7468 293a 0d0a 2020 2020  age_path):..    
+0001b510: 2020 2020 2020 2020 2020 2020 696d 6167              imag
+0001b520: 655f 6e61 6d65 5f73 7465 6d20 3d20 6f73  e_name_stem = os
+0001b530: 2e70 6174 682e 7370 6c69 7465 7874 286f  .path.splitext(o
+0001b540: 732e 7061 7468 2e62 6173 656e 616d 6528  s.path.basename(
+0001b550: 696d 6167 655f 7061 7468 2929 5b30 5d0d  image_path))[0].
+0001b560: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001b570: 2070 7265 7065 6e64 203d 2069 6d61 6765   prepend = image
+0001b580: 5f6e 616d 655f 7374 656d 202b 2022 5f22  _name_stem + "_"
+0001b590: 0d0a 2020 2020 2020 2020 2020 2020 656c  ..            el
+0001b5a0: 6966 206f 732e 7061 7468 2e69 7364 6972  if os.path.isdir
+0001b5b0: 2869 6d61 6765 5f70 6174 6829 3a0d 0a20  (image_path):.. 
+0001b5c0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+0001b5d0: 7265 7065 6e64 203d 2022 220d 0a0d 0a20  repend = "".... 
+0001b5e0: 2020 2020 2020 2020 2020 2023 2320 6765             ## ge
+0001b5f0: 6e65 7261 7465 2063 6f6e 6669 6720 7061  nerate config pa
+0001b600: 7468 2066 726f 6d20 696d 6167 6520 6669  th from image fi
+0001b610: 6c65 206f 7220 6469 7265 6374 6f72 7920  le or directory 
+0001b620: 2870 726f 6a65 6374 290d 0a20 2020 2020  (project)..     
+0001b630: 2020 2020 2020 2063 6f6e 6669 675f 6e61         config_na
+0001b640: 6d65 203d 2070 7265 7065 6e64 202b 2022  me = prepend + "
+0001b650: 7079 7065 5f63 6f6e 6669 675f 2220 2b20  pype_config_" + 
+0001b660: 7461 6720 2b20 222e 7961 6d6c 220d 0a20  tag + ".yaml".. 
+0001b670: 2020 2020 2020 2020 2020 2063 6f6e 6669             confi
+0001b680: 675f 7061 7468 203d 206f 732e 7061 7468  g_path = os.path
+0001b690: 2e6a 6f69 6e28 7365 6c66 2e63 6f6e 7461  .join(self.conta
+0001b6a0: 696e 6572 2e64 6972 5f70 6174 682c 2063  iner.dir_path, c
+0001b6b0: 6f6e 6669 675f 6e61 6d65 290d 0a0d 0a20  onfig_name).... 
+0001b6c0: 2020 2020 2020 2023 2320 6c6f 6164 2063         ## load c
+0001b6d0: 6f6e 6669 6720 6672 6f6d 2063 6f6e 6669  onfig from confi
+0001b6e0: 6720 7061 7468 0d0a 2020 2020 2020 2020  g path..        
+0001b6f0: 656c 6966 2063 6f6e 6669 675f 7061 7468  elif config_path
+0001b700: 2e5f 5f63 6c61 7373 5f5f 2e5f 5f6e 616d  .__class__.__nam
+0001b710: 655f 5f20 3d3d 2022 7374 7222 3a0d 0a20  e__ == "str":.. 
+0001b720: 2020 2020 2020 2020 2020 2069 6620 6f73             if os
+0001b730: 2e70 6174 682e 6973 6669 6c65 2863 6f6e  .path.isfile(con
+0001b740: 6669 675f 7061 7468 293a 0d0a 2020 2020  fig_path):..    
+0001b750: 2020 2020 2020 2020 2020 2020 7061 7373              pass
+0001b760: 0d0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
+0001b770: 656c 7365 3a0d 0a20 2020 2020 2020 2020  else:..         
+0001b780: 2020 2023 2020 2020 2072 6169 7365 2046     #     raise F
+0001b790: 696c 654e 6f74 466f 756e 6445 7272 6f72  ileNotFoundError
+0001b7a0: 280d 0a20 2020 2020 2020 2020 2020 2023  (..            #
+0001b7b0: 2020 2020 2020 2020 2022 436f 756c 6420           "Could 
+0001b7c0: 6e6f 7420 7265 6164 2063 6f6e 6669 6720  not read config 
+0001b7d0: 6669 6c65 2066 726f 6d20 7370 6563 6966  file from specif
+0001b7e0: 6965 6420 636f 6e66 6967 5f70 6174 683a  ied config_path:
+0001b7f0: 205c 227b 7d5c 2222 2e66 6f72 6d61 7428   \"{}\"".format(
+0001b800: 636f 6e66 6967 5f70 6174 6829 290d 0a0d  config_path))...
+0001b810: 0a20 2020 2020 2020 2069 6620 6f73 2e70  .        if os.p
+0001b820: 6174 682e 6973 6669 6c65 2863 6f6e 6669  ath.isfile(confi
+0001b830: 675f 7061 7468 293a 0d0a 2020 2020 2020  g_path):..      
+0001b840: 2020 2020 2020 7365 6c66 2e63 6f6e 6669        self.confi
+0001b850: 6720 3d20 756c 2e5f 6c6f 6164 5f79 616d  g = ul._load_yam
+0001b860: 6c28 636f 6e66 6967 5f70 6174 6829 0d0a  l(config_path)..
+0001b870: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0001b880: 2e63 6f6e 6669 675f 7061 7468 203d 2063  .config_path = c
+0001b890: 6f6e 6669 675f 7061 7468 0d0a 2020 2020  onfig_path..    
+0001b8a0: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
+0001b8b0: 2020 2020 2020 2072 6169 7365 2046 696c         raise Fil
+0001b8c0: 654e 6f74 466f 756e 6445 7272 6f72 280d  eNotFoundError(.
+0001b8d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001b8e0: 2027 436f 756c 6420 6e6f 7420 6669 6e64   'Could not find
+0001b8f0: 2063 6f6e 6669 6720 6669 6c65 2022 7b7d   config file "{}
+0001b900: 2220 696e 2069 6d61 6765 2064 6972 6563  " in image direc
+0001b910: 746f 7279 3a20 227b 7d22 272e 666f 726d  tory: "{}"'.form
+0001b920: 6174 280d 0a20 2020 2020 2020 2020 2020  at(..           
+0001b930: 2020 2020 2020 2020 2063 6f6e 6669 675f           config_
+0001b940: 6e61 6d65 2c20 6f73 2e70 6174 682e 6469  name, os.path.di
+0001b950: 726e 616d 6528 696d 6167 655f 7061 7468  rname(image_path
+0001b960: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+0001b970: 2020 2029 0d0a 2020 2020 2020 2020 2020     )..          
+0001b980: 2020 290d 0a0d 0a20 2020 2064 6566 205f    )....    def _
+0001b990: 7374 6172 745f 6669 6c65 5f6d 6f6e 6974  start_file_monit
+0001b9a0: 6f72 2873 656c 662c 2064 656c 6179 293a  or(self, delay):
+0001b9b0: 0d0a 0d0a 2020 2020 2020 2020 6966 2070  ....        if p
+0001b9c0: 6c61 7466 6f72 6d2e 7379 7374 656d 2829  latform.system()
+0001b9d0: 203d 3d20 2244 6172 7769 6e22 3a20 2023   == "Darwin":  #
+0001b9e0: 206d 6163 4f53 0d0a 2020 2020 2020 2020   macOS..        
+0001b9f0: 2020 2020 7375 6270 726f 6365 7373 2e63      subprocess.c
+0001ba00: 616c 6c28 2822 6f70 656e 222c 2073 656c  all(("open", sel
+0001ba10: 662e 636f 6e66 6967 5f70 6174 6829 290d  f.config_path)).
+0001ba20: 0a20 2020 2020 2020 2065 6c69 6620 706c  .        elif pl
+0001ba30: 6174 666f 726d 2e73 7973 7465 6d28 2920  atform.system() 
+0001ba40: 3d3d 2022 5769 6e64 6f77 7322 3a20 2023  == "Windows":  #
+0001ba50: 2057 696e 646f 7773 0d0a 2020 2020 2020   Windows..      
+0001ba60: 2020 2020 2020 6f73 2e73 7461 7274 6669        os.startfi
+0001ba70: 6c65 286f 732e 7061 7468 2e6e 6f72 6d70  le(os.path.normp
+0001ba80: 6174 6828 7365 6c66 2e63 6f6e 6669 675f  ath(self.config_
+0001ba90: 7061 7468 2929 0d0a 2020 2020 2020 2020  path))..        
+0001baa0: 656c 7365 3a20 2023 206c 696e 7578 2076  else:  # linux v
+0001bab0: 6172 6961 6e74 730d 0a20 2020 2020 2020  ariants..       
+0001bac0: 2020 2020 2073 7562 7072 6f63 6573 732e       subprocess.
+0001bad0: 6361 6c6c 2828 2278 6467 2d6f 7065 6e22  call(("xdg-open"
+0001bae0: 2c20 7365 6c66 2e63 6f6e 6669 675f 7061  , self.config_pa
+0001baf0: 7468 2929 0d0a 0d0a 2020 2020 2020 2020  th))....        
+0001bb00: 7365 6c66 2e59 464d 203d 2075 6c2e 5f59  self.YFM = ul._Y
+0001bb10: 616d 6c46 696c 654d 6f6e 6974 6f72 2873  amlFileMonitor(s
+0001bb20: 656c 662e 636f 6e66 6967 5f70 6174 682c  elf.config_path,
+0001bb30: 2064 656c 6179 290d 0a20 2020 2020 2020   delay)..       
+0001bb40: 2073 656c 662e 5f6c 6f67 2822 6465 6275   self._log("debu
+0001bb50: 6722 2c20 2250 7970 653a 2073 7461 7274  g", "Pype: start
+0001bb60: 696e 6720 636f 6e66 6967 2066 696c 6520  ing config file 
+0001bb70: 6d6f 6e69 746f 7222 2c20 3029 0d0a 0d0a  monitor", 0)....
+0001bb80: 2020 2020 6465 6620 5f63 6865 636b 5f64      def _check_d
+0001bb90: 6972 6563 746f 7279 5f73 6b69 7028 7365  irectory_skip(se
+0001bba0: 6c66 2c20 7461 672c 2073 6b69 705f 7061  lf, tag, skip_pa
+0001bbb0: 7474 6572 6e2c 2064 6972 5f70 6174 6829  ttern, dir_path)
+0001bbc0: 3a0d 0a0d 0a20 2020 2020 2020 2023 2320  :....        ## 
+0001bbd0: 736b 6970 2064 6972 6563 746f 7269 6573  skip directories
+0001bbe0: 2074 6861 7420 616c 7265 6164 7920 636f   that already co
+0001bbf0: 6e74 6169 6e20 7370 6563 6966 6965 6420  ntain specified 
+0001bc00: 6669 6c65 730d 0a20 2020 2020 2020 2069  files..        i
+0001bc10: 6620 736b 6970 5f70 6174 7465 726e 2e5f  f skip_pattern._
+0001bc20: 5f63 6c61 7373 5f5f 2e5f 5f6e 616d 655f  _class__.__name_
+0001bc30: 5f20 3d3d 2022 7374 7222 3a0d 0a20 2020  _ == "str":..   
+0001bc40: 2020 2020 2020 2020 2073 6b69 705f 7061           skip_pa
+0001bc50: 7474 6572 6e20 3d20 5b73 6b69 705f 7061  ttern = [skip_pa
+0001bc60: 7474 6572 6e5d 0d0a 2020 2020 2020 2020  ttern]..        
+0001bc70: 656c 6966 2073 6b69 705f 7061 7474 6572  elif skip_patter
+0001bc80: 6e2e 5f5f 636c 6173 735f 5f2e 5f5f 6e61  n.__class__.__na
+0001bc90: 6d65 5f5f 203d 3d20 2262 6f6f 6c22 3a0d  me__ == "bool":.
+0001bca0: 0a20 2020 2020 2020 2020 2020 2073 6b69  .            ski
+0001bcb0: 705f 7061 7474 6572 6e20 3d20 5b22 225d  p_pattern = [""]
+0001bcc0: 0d0a 2020 2020 2020 2020 656c 6966 2073  ..        elif s
+0001bcd0: 6b69 705f 7061 7474 6572 6e2e 5f5f 636c  kip_pattern.__cl
+0001bce0: 6173 735f 5f2e 5f5f 6e61 6d65 5f5f 2069  ass__.__name__ i
+0001bcf0: 6e20 5b22 6c69 7374 222c 2022 436f 6d6d  n ["list", "Comm
+0001bd00: 656e 7465 6453 6571 225d 3a0d 0a20 2020  entedSeq"]:..   
+0001bd10: 2020 2020 2020 2020 2073 6b69 705f 7061           skip_pa
+0001bd20: 7474 6572 6e20 3d20 736b 6970 5f70 6174  ttern = skip_pat
+0001bd30: 7465 726e 0d0a 0d0a 2020 2020 2020 2020  tern....        
+0001bd40: 6669 6c65 5f70 6174 7465 726e 203d 205b  file_pattern = [
+0001bd50: 5d0d 0a20 2020 2020 2020 2066 6f72 2070  ]..        for p
+0001bd60: 6174 7465 726e 2069 6e20 736b 6970 5f70  attern in skip_p
+0001bd70: 6174 7465 726e 3a0d 0a20 2020 2020 2020  attern:..       
+0001bd80: 2020 2020 2066 696c 655f 7061 7474 6572       file_patter
+0001bd90: 6e2e 6170 7065 6e64 2870 6174 7465 726e  n.append(pattern
+0001bda0: 202b 2022 5f22 202b 2074 6167 290d 0a0d   + "_" + tag)...
+0001bdb0: 0a20 2020 2020 2020 2066 696c 6570 6174  .        filepat
+0001bdc0: 6873 2c20 6475 706c 6963 6174 6573 203d  hs, duplicates =
+0001bdd0: 2075 6c2e 5f66 696c 655f 7761 6c6b 6572   ul._file_walker
+0001bde0: 280d 0a20 2020 2020 2020 2020 2020 2064  (..            d
+0001bdf0: 6972 5f70 6174 682c 0d0a 2020 2020 2020  ir_path,..      
+0001be00: 2020 2020 2020 696e 636c 7564 653d 6669        include=fi
+0001be10: 6c65 5f70 6174 7465 726e 2c0d 0a20 2020  le_pattern,..   
+0001be20: 2020 2020 2020 2020 2069 6e63 6c75 6465           include
+0001be30: 5f61 6c6c 3d46 616c 7365 2c0d 0a20 2020  _all=False,..   
+0001be40: 2020 2020 2020 2020 2065 7863 6c75 6465           exclude
+0001be50: 3d5b 2270 7970 655f 636f 6e66 6967 222c  =["pype_config",
+0001be60: 2022 6174 7472 6962 7574 6573 225d 2c0d   "attributes"],.
+0001be70: 0a20 2020 2020 2020 2020 2020 2070 7970  .            pyp
+0001be80: 655f 6d6f 6465 3d54 7275 652c 0d0a 2020  e_mode=True,..  
+0001be90: 2020 2020 2020 290d 0a0d 0a20 2020 2020        )....     
+0001bea0: 2020 2069 6620 6c65 6e28 6669 6c65 7061     if len(filepa
+0001beb0: 7468 7329 203e 2030 3a0d 0a20 2020 2020  ths) > 0:..     
+0001bec0: 2020 2020 2020 2066 696c 6573 203d 205b         files = [
+0001bed0: 5d0d 0a20 2020 2020 2020 2020 2020 2066  ]..            f
+0001bee0: 6f72 2066 696c 6520 696e 2066 696c 6570  or file in filep
+0001bef0: 6174 6873 3a0d 0a20 2020 2020 2020 2020  aths:..         
+0001bf00: 2020 2020 2020 2066 696c 6573 2e61 7070         files.app
+0001bf10: 656e 6428 6f73 2e70 6174 682e 6261 7365  end(os.path.base
+0001bf20: 6e61 6d65 2866 696c 6529 290d 0a20 2020  name(file))..   
+0001bf30: 2020 2020 2020 2020 2070 7269 6e74 2827           print('
+0001bf40: 5c6e 466f 756e 6420 6578 6973 7469 6e67  \nFound existing
+0001bf50: 2066 696c 6573 207b 7d20 2d20 736b 6970   files {} - skip
+0001bf60: 7065 645c 6e27 2e66 6f72 6d61 7428 282a  ped\n'.format((*
+0001bf70: 6669 6c65 732c 2929 290d 0a20 2020 2020  files,)))..     
+0001bf80: 2020 2020 2020 2072 6574 7572 6e20 5472         return Tr
+0001bf90: 7565 0d0a 2020 2020 2020 2020 656c 7365  ue..        else
+0001bfa0: 3a0d 0a20 2020 2020 2020 2020 2020 2072  :..            r
+0001bfb0: 6574 7572 6e20 4661 6c73 650d 0a0d 0a20  eturn False.... 
+0001bfc0: 2020 2064 6566 205f 6368 6563 6b5f 6669     def _check_fi
+0001bfd0: 6e61 6c28 7365 6c66 293a 0d0a 0d0a 2020  nal(self):....  
+0001bfe0: 2020 2020 2020 2323 2063 6865 636b 2063        ## check c
+0001bff0: 6f6d 706f 6e65 6e74 7320 6265 666f 7265  omponents before
+0001c000: 2073 7461 7274 696e 6720 7079 7065 2074   starting pype t
+0001c010: 6f20 7365 6520 6966 2073 6f6d 6574 6869  o see if somethi
+0001c020: 6e67 2077 656e 7420 7772 6f6e 670d 0a20  ng went wrong.. 
+0001c030: 2020 2020 2020 2069 6620 280d 0a20 2020         if (..   
+0001c040: 2020 2020 2020 2020 206e 6f74 2068 6173           not has
+0001c050: 6174 7472 2873 656c 662e 636f 6e74 6169  attr(self.contai
+0001c060: 6e65 722c 2022 696d 6167 6522 290d 0a20  ner, "image").. 
+0001c070: 2020 2020 2020 2020 2020 206f 7220 7365             or se
+0001c080: 6c66 2e63 6f6e 7461 696e 6572 2e69 6d61  lf.container.ima
+0001c090: 6765 2e5f 5f63 6c61 7373 5f5f 2e5f 5f6e  ge.__class__.__n
+0001c0a0: 616d 655f 5f20 3d3d 2022 4e6f 6e65 5479  ame__ == "NoneTy
+0001c0b0: 7065 220d 0a20 2020 2020 2020 2029 3a0d  pe"..        ):.
+0001c0c0: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
+0001c0d0: 7365 2041 7474 7269 6275 7465 4572 726f  se AttributeErro
+0001c0e0: 7228 224e 6f20 696d 6167 6520 7761 7320  r("No image was 
+0001c0f0: 6c6f 6164 6564 2229 0d0a 2020 2020 2020  loaded")..      
+0001c100: 2020 2020 2020 7265 7475 726e 0d0a 2020        return..  
+0001c110: 2020 2020 2020 6966 2028 0d0a 2020 2020        if (..    
+0001c120: 2020 2020 2020 2020 6e6f 7420 6861 7361          not hasa
+0001c130: 7474 7228 7365 6c66 2e63 6f6e 7461 696e  ttr(self.contain
+0001c140: 6572 2c20 2264 6972 5f70 6174 6822 290d  er, "dir_path").
+0001c150: 0a20 2020 2020 2020 2020 2020 206f 7220  .            or 
+0001c160: 7365 6c66 2e63 6f6e 7461 696e 6572 2e64  self.container.d
+0001c170: 6972 5f70 6174 682e 5f5f 636c 6173 735f  ir_path.__class_
+0001c180: 5f2e 5f5f 6e61 6d65 5f5f 203d 3d20 224e  _.__name__ == "N
+0001c190: 6f6e 6554 7970 6522 0d0a 2020 2020 2020  oneType"..      
+0001c1a0: 2020 293a 0d0a 2020 2020 2020 2020 2020    ):..          
+0001c1b0: 2020 7261 6973 6520 4174 7472 6962 7574    raise Attribut
+0001c1c0: 6545 7272 6f72 2822 436f 756c 6420 6e6f  eError("Could no
+0001c1d0: 7420 6465 7465 726d 696e 6520 6469 725f  t determine dir_
+0001c1e0: 7061 7468 2074 6f20 7361 7665 206f 7574  path to save out
+0001c1f0: 7075 742e 2229 0d0a 2020 2020 2020 2020  put.")..        
+0001c200: 2020 2020 7265 7475 726e 0d0a 2020 2020      return..    
+0001c210: 2020 2020 6966 206e 6f74 2068 6173 6174      if not hasat
+0001c220: 7472 2873 656c 662c 2022 636f 6e66 6967  tr(self, "config
+0001c230: 2229 206f 7220 7365 6c66 2e63 6f6e 6669  ") or self.confi
+0001c240: 672e 5f5f 636c 6173 735f 5f2e 5f5f 6e61  g.__class__.__na
+0001c250: 6d65 5f5f 203d 3d20 224e 6f6e 6554 7970  me__ == "NoneTyp
+0001c260: 6522 3a0d 0a20 2020 2020 2020 2020 2020  e":..           
+0001c270: 2072 6169 7365 2041 7474 7269 6275 7465   raise Attribute
+0001c280: 4572 726f 7228 0d0a 2020 2020 2020 2020  Error(..        
+0001c290: 2020 2020 2020 2020 224e 6f20 636f 6e66          "No conf
+0001c2a0: 6967 2066 696c 6520 7761 7320 7072 6f76  ig file was prov
+0001c2b0: 6964 6564 206f 7220 6c6f 6164 696e 6720  ided or loading 
+0001c2c0: 636f 6e66 6967 2064 6964 206e 6f74 2073  config did not s
+0001c2d0: 7563 6365 6564 2e22 0d0a 2020 2020 2020  ucceed."..      
+0001c2e0: 2020 2020 2020 290d 0a20 2020 2020 2020        )..       
+0001c2f0: 2020 2020 2072 6574 7572 6e0d 0a20 2020       return..   
+0001c300: 2020 2020 200d 0a20 2020 2064 6566 205f       ..    def _
+0001c310: 6c6f 6728 7365 6c66 2c20 6c76 6c2c 206d  log(self, lvl, m
+0001c320: 6573 7361 6765 732c 2069 6e64 3d30 2c20  essages, ind=0, 
+0001c330: 7061 7373 7468 726f 7567 683d 4661 6c73  passthrough=Fals
+0001c340: 6529 3a0d 0a20 2020 2020 2020 200d 0a20  e):..        .. 
+0001c350: 2020 2020 2020 2022 2222 4164 6420 6120         """Add a 
+0001c360: 6d65 7373 6167 6520 746f 2061 206c 6f67  message to a log
+0001c370: 6769 6e67 206f 626a 6563 742e 0d0a 0d0a  ging object.....
+0001c380: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
+0001c390: 7273 3a0d 0a20 2020 2020 2020 206c 6f67  rs:..        log
+0001c3a0: 6769 6e67 2028 6c6f 6767 696e 672e 4c6f  ging (logging.Lo
+0001c3b0: 6767 6572 293a 2054 6865 206c 6f67 6769  gger): The loggi
+0001c3c0: 6e67 206f 626a 6563 7420 746f 2061 6464  ng object to add
+0001c3d0: 2074 6865 206d 6573 7361 6765 2074 6f2e   the message to.
+0001c3e0: 0d0a 2020 2020 2020 2020 6d65 7373 6167  ..        messag
+0001c3f0: 6520 2873 7472 293a 2054 6865 206d 6573  e (str): The mes
+0001c400: 7361 6765 2074 6f20 6265 206c 6f67 6765  sage to be logge
+0001c410: 642e 0d0a 0d0a 2020 2020 2020 2020 2222  d.....        ""
+0001c420: 220d 0a0d 0a20 2020 2020 2020 2069 6620  "....        if 
+0001c430: 6973 696e 7374 616e 6365 286d 6573 7361  isinstance(messa
+0001c440: 6765 732c 2073 7472 293a 0d0a 2020 2020  ges, str):..    
+0001c450: 2020 2020 2020 2020 6d65 7373 6167 6573          messages
+0001c460: 5f6c 6973 7420 3d20 6d65 7373 6167 6573  _list = messages
+0001c470: 2e73 706c 6974 2822 5c6e 2229 0d0a 2020  .split("\n")..  
+0001c480: 2020 2020 2020 656c 6966 2069 7369 6e73        elif isins
+0001c490: 7461 6e63 6528 6d65 7373 6167 6573 2c20  tance(messages, 
+0001c4a0: 6c69 7374 293a 0d0a 2020 2020 2020 2020  list):..        
+0001c4b0: 2020 2020 6d65 7373 6167 6573 5f6c 6973      messages_lis
+0001c4c0: 7420 3d20 6d65 7373 6167 6573 0d0a 2020  t = messages..  
+0001c4d0: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+0001c4e0: 2020 2020 666f 7220 6d65 7373 6167 6520      for message 
+0001c4f0: 696e 206d 6573 7361 6765 735f 6c69 7374  in messages_list
+0001c500: 3a0d 0a20 2020 2020 2020 2020 2020 2069  :..            i
+0001c510: 6620 6e6f 7420 6d65 7373 6167 6520 3d3d  f not message ==
+0001c520: 2022 223a 0d0a 2020 2020 2020 2020 2020   "":..          
+0001c530: 2020 2020 2020 6966 206d 6573 7361 6765        if message
+0001c540: 2e65 6e64 7377 6974 6828 225c 6e22 293a  .endswith("\n"):
+0001c550: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001c560: 2020 2020 2020 6d65 7373 6167 6520 3d20        message = 
+0001c570: 6d65 7373 6167 655b 3a2d 325d 0d0a 2020  message[:-2]..  
+0001c580: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+0001c590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001c5a0: 6d65 7373 6167 6520 3d20 2822 2020 2020  message = ("    
+0001c5b0: 2220 2a20 696e 6429 202b 206d 6573 7361  " * ind) + messa
+0001c5c0: 6765 0d0a 2020 2020 2020 2020 2020 2020  ge..            
+0001c5d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001c5e0: 2020 6966 206c 766c 203d 3d20 2264 6562    if lvl == "deb
+0001c5f0: 7567 223a 0d0a 2020 2020 2020 2020 2020  ug":..          
+0001c600: 2020 2020 2020 2020 2020 7365 6c66 2e6c            self.l
+0001c610: 6f67 6765 722e 6465 6275 6728 6d65 7373  ogger.debug(mess
+0001c620: 6167 6529 0d0a 2020 2020 2020 2020 2020  age)..          
+0001c630: 2020 2020 2020 656c 6966 206c 766c 203d        elif lvl =
+0001c640: 3d20 2269 6e66 6f22 3a0d 0a20 2020 2020  = "info":..     
+0001c650: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0001c660: 656c 662e 6c6f 6767 6572 2e69 6e66 6f28  elf.logger.info(
+0001c670: 6d65 7373 6167 6529 0d0a 2020 2020 2020  message)..      
+0001c680: 2020 2020 2020 2020 2020 656c 6966 206c            elif l
+0001c690: 766c 203d 3d20 2277 6172 6e69 6e67 223a  vl == "warning":
+0001c6a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001c6b0: 2020 2020 2020 7365 6c66 2e6c 6f67 6765        self.logge
+0001c6c0: 722e 7761 726e 696e 6728 6d65 7373 6167  r.warning(messag
+0001c6d0: 6529 0d0a 2020 2020 2020 2020 2020 2020  e)..            
+0001c6e0: 2020 2020 656c 6966 206c 766c 203d 3d20      elif lvl == 
+0001c6f0: 2265 7272 6f72 223a 0d0a 2020 2020 2020  "error":..      
+0001c700: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0001c710: 6c66 2e6c 6f67 6765 722e 6572 726f 7228  lf.logger.error(
+0001c720: 6d65 7373 6167 6529 0d0a 2020 2020 2020  message)..      
+0001c730: 2020 2020 2020 2020 2020 656c 6966 206c            elif l
+0001c740: 766c 203d 3d20 2263 7269 7469 6361 6c22  vl == "critical"
+0001c750: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+0001c760: 2020 2020 2020 2073 656c 662e 6c6f 6767         self.logg
+0001c770: 6572 2e63 7269 7469 6361 6c28 6d65 7373  er.critical(mess
+0001c780: 6167 6529 0d0a 2020 2020 2020 2020 2020  age)..          
+0001c790: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+0001c7a0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
+0001c7b0: 656c 662e 666c 6167 732e 6665 6564 6261  elf.flags.feedba
+0001c7c0: 636b 3d3d 4661 6c73 6520 616e 6420 7061  ck==False and pa
+0001c7d0: 7373 7468 726f 7567 683d 3d54 7275 653a  ssthrough==True:
+0001c7e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001c7f0: 2020 2020 2020 686d 203d 2064 6174 6574        hm = datet
+0001c800: 696d 652e 746f 6461 7928 292e 7374 7266  ime.today().strf
+0001c810: 7469 6d65 2822 2548 3a25 4d3a 2553 2229  time("%H:%M:%S")
+0001c820: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001c830: 2020 2020 2020 7072 696e 7428 686d 202b        print(hm +
+0001c840: 2022 3a20 2220 2b20 6d65 7373 6167 6529   ": " + message)
+0001c850: 0d0a 0d0a 0d0a 2020 2020 6465 6620 5f69  ......    def _i
+0001c860: 7465 7261 7465 280d 0a20 2020 2020 2020  terate(..       
+0001c870: 2073 656c 662c 200d 0a20 2020 2020 2020   self, ..       
+0001c880: 2061 6e6e 6f74 6174 696f 6e73 2c20 0d0a   annotations, ..
+0001c890: 2020 2020 2020 2020 6578 6563 7574 653d          execute=
+0001c8a0: 5472 7565 2c20 0d0a 2020 2020 2020 2020  True, ..        
+0001c8b0: 6175 746f 7368 6f77 3d54 7275 652c 200d  autoshow=True, .
+0001c8c0: 0a20 2020 2020 2020 2069 6e74 6572 6163  .        interac
+0001c8d0: 7469 7665 3d54 7275 652c 0d0a 2020 2020  tive=True,..    
+0001c8e0: 293a 0d0a 0d0a 2020 2020 2020 2020 666c  ):....        fl
+0001c8f0: 6167 7320 3d20 6d61 6b65 5f64 6174 6163  ags = make_datac
+0001c900: 6c61 7373 280d 0a20 2020 2020 2020 2020  lass(..         
+0001c910: 2020 2063 6c73 5f6e 616d 653d 2266 6c61     cls_name="fla
+0001c920: 6773 222c 0d0a 2020 2020 2020 2020 2020  gs",..          
+0001c930: 2020 6669 656c 6473 3d5b 0d0a 2020 2020    fields=[..    
+0001c940: 2020 2020 2020 2020 2020 2020 2822 6578              ("ex
+0001c950: 6563 7574 6522 2c20 626f 6f6c 2c20 6578  ecute", bool, ex
+0001c960: 6563 7574 6529 2c0d 0a20 2020 2020 2020  ecute),..       
+0001c970: 2020 2020 2020 2020 2028 2261 7574 6f73           ("autos
+0001c980: 686f 7722 2c20 626f 6f6c 2c20 6175 746f  how", bool, auto
+0001c990: 7368 6f77 292c 0d0a 2020 2020 2020 2020  show),..        
+0001c9a0: 2020 2020 2020 2020 2822 696e 7465 7261          ("intera
+0001c9b0: 6374 6976 6522 2c20 626f 6f6c 2c20 696e  ctive", bool, in
+0001c9c0: 7465 7261 6374 6976 6529 2c0d 0a20 2020  teractive),..   
+0001c9d0: 2020 2020 2020 2020 205d 2c0d 0a20 2020           ],..   
+0001c9e0: 2020 2020 2029 0d0a 0d0a 2020 2020 2020       )....      
+0001c9f0: 2020 2320 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d    # ============
 0001ca00: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0001ca10: 3d3d 3d3d 0d0a 2020 2020 2020 2020 2320  ====..        # 
-0001ca20: 4645 4544 4241 434b 200d 0a20 2020 2020  FEEDBACK ..     
-0001ca30: 2020 200d 0a20 2020 2020 2020 2069 6620     ..        if 
-0001ca40: 666c 6167 732e 6578 6563 7574 6520 616e  flags.execute an
-0001ca50: 6420 6e6f 7420 7365 6c66 2e66 6c61 6773  d not self.flags
-0001ca60: 2e64 7279 5f72 756e 3a0d 0a20 2020 2020  .dry_run:..     
-0001ca70: 2020 2020 2020 206e 6577 5f70 7970 655f         new_pype_
-0001ca80: 6d73 6720 3d20 756c 2e5f 7070 7269 6e74  msg = ul._pprint
-0001ca90: 5f66 696c 6c5f 6862 6172 2822 7c20 6e65  _fill_hbar("| ne
-0001caa0: 7720 7079 7065 2069 7465 7261 7469 6f6e  w pype iteration
-0001cab0: 207c 222c 2072 6574 3d54 7275 6529 0d0a   |", ret=True)..
-0001cac0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0001cad0: 2e5f 6c6f 6728 2269 6e66 6f22 2c20 6e65  ._log("info", ne
-0001cae0: 775f 7079 7065 5f6d 7367 2c20 3029 200d  w_pype_msg, 0) .
-0001caf0: 0a20 2020 2020 2020 2020 2020 200d 0a20  .            .. 
-0001cb00: 2020 2020 2020 2023 203d 3d3d 3d3d 3d3d         # =======
-0001cb10: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0001cb20: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0001cb30: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0001ca10: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0001ca20: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0001ca30: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0001ca40: 3d0d 0a20 2020 2020 2020 2023 2046 4545  =..        # FEE
+0001ca50: 4442 4143 4b20 0d0a 2020 2020 2020 2020  DBACK ..        
+0001ca60: 0d0a 2020 2020 2020 2020 6966 2066 6c61  ..        if fla
+0001ca70: 6773 2e65 7865 6375 7465 2061 6e64 206e  gs.execute and n
+0001ca80: 6f74 2073 656c 662e 666c 6167 732e 6472  ot self.flags.dr
+0001ca90: 795f 7275 6e3a 0d0a 2020 2020 2020 2020  y_run:..        
+0001caa0: 2020 2020 6e65 775f 7079 7065 5f6d 7367      new_pype_msg
+0001cab0: 203d 2075 6c2e 5f70 7072 696e 745f 6669   = ul._pprint_fi
+0001cac0: 6c6c 5f68 6261 7228 227c 206e 6577 2070  ll_hbar("| new p
+0001cad0: 7970 6520 6974 6572 6174 696f 6e20 7c22  ype iteration |"
+0001cae0: 2c20 7265 743d 5472 7565 290d 0a20 2020  , ret=True)..   
+0001caf0: 2020 2020 2020 2020 2073 656c 662e 5f6c           self._l
+0001cb00: 6f67 2822 696e 666f 222c 206e 6577 5f70  og("info", new_p
+0001cb10: 7970 655f 6d73 672c 2030 2920 0d0a 2020  ype_msg, 0) ..  
+0001cb20: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+0001cb30: 2020 2020 2320 3d3d 3d3d 3d3d 3d3d 3d3d      # ==========
 0001cb40: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0001cb50: 3d3d 3d3d 3d3d 0d0a 0d0a 2020 2020 2020  ======....      
-0001cb60: 2020 2320 7265 7365 7420 7661 6c75 6573    # reset values
-0001cb70: 0d0a 2020 2020 2020 2020 6966 206e 6f74  ..        if not
-0001cb80: 2073 656c 662e 666c 6167 732e 6472 795f   self.flags.dry_
-0001cb90: 7275 6e3a 0d0a 2020 2020 2020 2020 2020  run:..          
-0001cba0: 2020 7365 6c66 2e63 6f6e 7461 696e 6572    self.container
-0001cbb0: 2e5f 7265 7365 7428 290d 0a20 2020 2020  ._reset()..     
-0001cbc0: 2020 2061 6e6e 6f74 6174 696f 6e5f 636f     annotation_co
-0001cbd0: 756e 7465 7220 3d20 6469 6374 2e66 726f  unter = dict.fro
-0001cbe0: 6d6b 6579 7328 5f76 6172 732e 5f61 6e6e  mkeys(_vars._ann
-0001cbf0: 6f74 6174 696f 6e5f 7479 7065 732c 202d  otation_types, -
-0001cc00: 3129 0d0a 0d0a 2020 2020 2020 2020 2323  1)....        ##
-0001cc10: 2061 7070 6c79 2070 7970 653a 206c 6f6f   apply pype: loo
-0001cc20: 7020 7468 726f 7567 6820 7374 6570 7320  p through steps 
-0001cc30: 616e 6420 636f 6e74 6169 6e65 6420 6d65  and contained me
-0001cc40: 7468 6f64 730d 0a20 2020 2020 2020 2073  thods..        s
-0001cc50: 7465 705f 6c69 7374 203d 2073 656c 662e  tep_list = self.
-0001cc60: 636f 6e66 6967 5b22 7072 6f63 6573 7369  config["processi
-0001cc70: 6e67 5f73 7465 7073 225d 0d0a 2020 2020  ng_steps"]..    
-0001cc80: 2020 2020 7365 6c66 2e63 6f6e 6669 675f      self.config_
-0001cc90: 7570 6461 7465 6420 3d20 636f 7079 2e64  updated = copy.d
-0001cca0: 6565 7063 6f70 7928 7365 6c66 2e63 6f6e  eepcopy(self.con
-0001ccb0: 6669 6729 0d0a 2020 2020 2020 2020 7365  fig)..        se
-0001ccc0: 6c66 2e63 6f6e 6669 675f 7061 7273 6564  lf.config_parsed
-0001ccd0: 5f66 6c61 7474 656e 6564 203d 207b 7d0d  _flattened = {}.
-0001cce0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001ccf0: 200d 0a20 2020 2020 2020 2066 6f72 2073   ..        for s
-0001cd00: 7465 705f 6964 782c 2073 7465 7020 696e  tep_idx, step in
-0001cd10: 2065 6e75 6d65 7261 7465 2873 7465 705f   enumerate(step_
-0001cd20: 6c69 7374 293a 0d0a 0d0a 2020 2020 2020  list):....      
-0001cd30: 2020 2020 2020 2320 3d3d 3d3d 3d3d 3d3d        # ========
-0001cd40: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0001cd50: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0001cd60: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0001cb50: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0001cb60: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0001cb70: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0001cb80: 3d3d 3d0d 0a0d 0a20 2020 2020 2020 2023  ===....        #
+0001cb90: 2072 6573 6574 2076 616c 7565 730d 0a20   reset values.. 
+0001cba0: 2020 2020 2020 2069 6620 6e6f 7420 7365         if not se
+0001cbb0: 6c66 2e66 6c61 6773 2e64 7279 5f72 756e  lf.flags.dry_run
+0001cbc0: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
+0001cbd0: 656c 662e 636f 6e74 6169 6e65 722e 5f72  elf.container._r
+0001cbe0: 6573 6574 2829 0d0a 2020 2020 2020 2020  eset()..        
+0001cbf0: 616e 6e6f 7461 7469 6f6e 5f63 6f75 6e74  annotation_count
+0001cc00: 6572 203d 2064 6963 742e 6672 6f6d 6b65  er = dict.fromke
+0001cc10: 7973 285f 7661 7273 2e5f 616e 6e6f 7461  ys(_vars._annota
+0001cc20: 7469 6f6e 5f74 7970 6573 2c20 2d31 290d  tion_types, -1).
+0001cc30: 0a0d 0a20 2020 2020 2020 2023 2320 6170  ...        ## ap
+0001cc40: 706c 7920 7079 7065 3a20 6c6f 6f70 2074  ply pype: loop t
+0001cc50: 6872 6f75 6768 2073 7465 7073 2061 6e64  hrough steps and
+0001cc60: 2063 6f6e 7461 696e 6564 206d 6574 686f   contained metho
+0001cc70: 6473 0d0a 2020 2020 2020 2020 7374 6570  ds..        step
+0001cc80: 5f6c 6973 7420 3d20 7365 6c66 2e63 6f6e  _list = self.con
+0001cc90: 6669 675b 2270 726f 6365 7373 696e 675f  fig["processing_
+0001cca0: 7374 6570 7322 5d0d 0a20 2020 2020 2020  steps"]..       
+0001ccb0: 2073 656c 662e 636f 6e66 6967 5f75 7064   self.config_upd
+0001ccc0: 6174 6564 203d 2063 6f70 792e 6465 6570  ated = copy.deep
+0001ccd0: 636f 7079 2873 656c 662e 636f 6e66 6967  copy(self.config
+0001cce0: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+0001ccf0: 636f 6e66 6967 5f70 6172 7365 645f 666c  config_parsed_fl
+0001cd00: 6174 7465 6e65 6420 3d20 7b7d 0d0a 2020  attened = {}..  
+0001cd10: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+0001cd20: 2020 2020 2020 2020 666f 7220 7374 6570          for step
+0001cd30: 5f69 6478 2c20 7374 6570 2069 6e20 656e  _idx, step in en
+0001cd40: 756d 6572 6174 6528 7374 6570 5f6c 6973  umerate(step_lis
+0001cd50: 7429 3a0d 0a0d 0a20 2020 2020 2020 2020  t):....         
+0001cd60: 2020 2023 203d 3d3d 3d3d 3d3d 3d3d 3d3d     # ===========
 0001cd70: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0001cd80: 3d3d 3d3d 3d0d 0a20 2020 2020 2020 2020  =====..         
-0001cd90: 2020 2023 2053 5445 500d 0a20 2020 2020     # STEP..     
-0001cda0: 2020 2020 2020 2023 203d 3d3d 3d3d 3d3d         # =======
-0001cdb0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0001cdc0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0001cdd0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0001cd80: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0001cd90: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0001cda0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0001cdb0: 3d3d 0d0a 2020 2020 2020 2020 2020 2020  ==..            
+0001cdc0: 2320 5354 4550 0d0a 2020 2020 2020 2020  # STEP..        
+0001cdd0: 2020 2020 2320 3d3d 3d3d 3d3d 3d3d 3d3d      # ==========
 0001cde0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0001cdf0: 3d3d 3d3d 3d3d 0d0a 0d0a 2020 2020 2020  ======....      
-0001ce00: 2020 2020 2020 6966 2073 7465 702e 5f5f        if step.__
-0001ce10: 636c 6173 735f 5f2e 5f5f 6e61 6d65 5f5f  class__.__name__
-0001ce20: 203d 3d20 2273 7472 223a 0d0a 2020 2020   == "str":..    
-0001ce30: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
-0001ce40: 696e 7565 0d0a 0d0a 2020 2020 2020 2020  inue....        
-0001ce50: 2020 2020 2323 2067 6574 2073 7465 7020      ## get step 
-0001ce60: 6e61 6d65 0d0a 2020 2020 2020 2020 2020  name..          
-0001ce70: 2020 7374 6570 5f6e 616d 6520 3d20 6c69    step_name = li
-0001ce80: 7374 2864 6963 7428 7374 6570 292e 6b65  st(dict(step).ke
-0001ce90: 7973 2829 295b 305d 0d0a 2020 2020 2020  ys())[0]..      
-0001cea0: 2020 2020 2020 6d65 7468 6f64 5f6c 6973        method_lis
-0001ceb0: 7420 3d20 6c69 7374 2864 6963 7428 7374  t = list(dict(st
-0001cec0: 6570 292e 7661 6c75 6573 2829 295b 305d  ep).values())[0]
-0001ced0: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
-0001cee0: 6c66 2e63 6f6e 6669 675f 7061 7273 6564  lf.config_parsed
-0001cef0: 5f66 6c61 7474 656e 6564 5b73 7465 705f  _flattened[step_
-0001cf00: 6e61 6d65 5d20 3d20 5b5d 0d0a 0d0a 2020  name] = []....  
-0001cf10: 2020 2020 2020 2020 2020 6966 206d 6574            if met
-0001cf20: 686f 645f 6c69 7374 2e5f 5f63 6c61 7373  hod_list.__class
-0001cf30: 5f5f 2e5f 5f6e 616d 655f 5f20 3d3d 2022  __.__name__ == "
-0001cf40: 4e6f 6e65 5479 7065 223a 0d0a 2020 2020  NoneType":..    
-0001cf50: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
-0001cf60: 696e 7565 0d0a 0d0a 2020 2020 2020 2020  inue....        
-0001cf70: 2020 2020 2323 2070 7269 6e74 2063 7572      ## print cur
-0001cf80: 7265 6e74 2073 7465 700d 0a20 2020 2020  rent step..     
-0001cf90: 2020 2020 2020 2069 6620 666c 6167 732e         if flags.
-0001cfa0: 6578 6563 7574 653a 0d0a 2020 2020 2020  execute:..      
-0001cfb0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-0001cfc0: 6c6f 6728 2269 6e66 6f22 2c20 7374 6570  log("info", step
-0001cfd0: 5f6e 616d 652c 2030 290d 0a0d 0a20 2020  _name, 0)....   
-0001cfe0: 2020 2020 2020 2020 2069 6620 7374 6570           if step
-0001cff0: 5f6e 616d 6520 3d3d 2022 7669 7375 616c  _name == "visual
-0001d000: 697a 6174 696f 6e22 2061 6e64 2066 6c61  ization" and fla
-0001d010: 6773 2e65 7865 6375 7465 3a0d 0a0d 0a20  gs.execute:.... 
-0001d020: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-0001d030: 2320 6368 6563 6b20 6966 2063 616e 7661  # check if canva
-0001d040: 7320 6973 2073 656c 6563 7465 642c 2061  s is selected, a
-0001d050: 6e64 206f 7468 6572 7769 7365 2065 7865  nd otherwise exe
-0001d060: 6375 7465 2077 6974 6820 6465 6661 756c  cute with defaul
-0001d070: 7420 7661 6c75 6573 0d0a 2020 2020 2020  t values..      
-0001d080: 2020 2020 2020 2020 2020 6368 6563 6b5f            check_
-0001d090: 6c69 7374 203d 205b 0d0a 2020 2020 2020  list = [..      
-0001d0a0: 2020 2020 2020 2020 2020 2020 2020 6c69                li
-0001d0b0: 7374 2864 6963 7428 6929 2e6b 6579 7328  st(dict(i).keys(
-0001d0c0: 2929 5b30 5d20 6966 206e 6f74 2069 7369  ))[0] if not isi
-0001d0d0: 6e73 7461 6e63 6528 692c 2073 7472 2920  nstance(i, str) 
-0001d0e0: 656c 7365 2069 0d0a 2020 2020 2020 2020  else i..        
-0001d0f0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-0001d100: 6920 696e 206d 6574 686f 645f 6c69 7374  i in method_list
-0001d110: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001d120: 2020 5d0d 0a20 2020 2020 2020 2020 2020    ]..           
-0001d130: 2020 2020 2069 6620 280d 0a20 2020 2020       if (..     
-0001d140: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0001d150: 656c 662e 636f 6e74 6169 6e65 722e 6361  elf.container.ca
-0001d160: 6e76 6173 2e5f 5f63 6c61 7373 5f5f 2e5f  nvas.__class__._
-0001d170: 5f6e 616d 655f 5f20 3d3d 2022 4e6f 6e65  _name__ == "None
-0001d180: 5479 7065 220d 0a20 2020 2020 2020 2020  Type"..         
-0001d190: 2020 2020 2020 2020 2020 2061 6e64 206e             and n
-0001d1a0: 6f74 2022 7365 6c65 6374 5f63 616e 7661  ot "select_canva
-0001d1b0: 7322 2069 6e20 6368 6563 6b5f 6c69 7374  s" in check_list
-0001d1c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001d1d0: 2020 293a 0d0a 2020 2020 2020 2020 2020    ):..          
-0001d1e0: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
-0001d1f0: 6f6e 7461 696e 6572 2e5f 7275 6e28 2273  ontainer._run("s
-0001d200: 656c 6563 745f 6361 6e76 6173 2229 0d0a  elect_canvas")..
-0001d210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d220: 2020 2020 6966 2066 6c61 6773 2e69 6e74      if flags.int
-0001d230: 6572 6163 7469 7665 2061 6e64 2066 6c61  eractive and fla
-0001d240: 6773 2e61 7574 6f73 686f 773a 0d0a 2020  gs.autoshow:..  
-0001d250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d260: 2020 2020 2020 7365 6c66 2e5f 6c6f 6728        self._log(
-0001d270: 2269 6e66 6f22 2c20 2273 656c 6563 745f  "info", "select_
-0001d280: 6361 6e76 6173 2028 4445 4641 554c 5429  canvas (DEFAULT)
-0001d290: 222c 2031 290d 0a20 2020 2020 2020 2020  ", 1)..         
-0001d2a0: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-0001d2b0: 0a20 2020 2020 2020 2020 2020 2023 2320  .            ## 
-0001d2c0: 6974 6572 6174 6520 7468 726f 7567 6820  iterate through 
-0001d2d0: 7374 6570 206c 6973 740d 0a20 2020 2020  step list..     
-0001d2e0: 2020 2020 2020 2066 6f72 206d 6574 686f         for metho
-0001d2f0: 645f 6964 782c 206d 6574 686f 6420 696e  d_idx, method in
-0001d300: 2065 6e75 6d65 7261 7465 286d 6574 686f   enumerate(metho
-0001d310: 645f 6c69 7374 293a 0d0a 0d0a 2020 2020  d_list):....    
-0001d320: 2020 2020 2020 2020 2020 2020 2320 3d3d              # ==
-0001d330: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0001d340: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0001d350: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0001cdf0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0001ce00: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0001ce10: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0001ce20: 3d3d 3d0d 0a0d 0a20 2020 2020 2020 2020  ===....         
+0001ce30: 2020 2069 6620 7374 6570 2e5f 5f63 6c61     if step.__cla
+0001ce40: 7373 5f5f 2e5f 5f6e 616d 655f 5f20 3d3d  ss__.__name__ ==
+0001ce50: 2022 7374 7222 3a0d 0a20 2020 2020 2020   "str":..       
+0001ce60: 2020 2020 2020 2020 2063 6f6e 7469 6e75           continu
+0001ce70: 650d 0a0d 0a20 2020 2020 2020 2020 2020  e....           
+0001ce80: 2023 2320 6765 7420 7374 6570 206e 616d   ## get step nam
+0001ce90: 650d 0a20 2020 2020 2020 2020 2020 2073  e..            s
+0001cea0: 7465 705f 6e61 6d65 203d 206c 6973 7428  tep_name = list(
+0001ceb0: 6469 6374 2873 7465 7029 2e6b 6579 7328  dict(step).keys(
+0001cec0: 2929 5b30 5d0d 0a20 2020 2020 2020 2020  ))[0]..         
+0001ced0: 2020 206d 6574 686f 645f 6c69 7374 203d     method_list =
+0001cee0: 206c 6973 7428 6469 6374 2873 7465 7029   list(dict(step)
+0001cef0: 2e76 616c 7565 7328 2929 5b30 5d0d 0a20  .values())[0].. 
+0001cf00: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+0001cf10: 636f 6e66 6967 5f70 6172 7365 645f 666c  config_parsed_fl
+0001cf20: 6174 7465 6e65 645b 7374 6570 5f6e 616d  attened[step_nam
+0001cf30: 655d 203d 205b 5d0d 0a0d 0a20 2020 2020  e] = []....     
+0001cf40: 2020 2020 2020 2069 6620 6d65 7468 6f64         if method
+0001cf50: 5f6c 6973 742e 5f5f 636c 6173 735f 5f2e  _list.__class__.
+0001cf60: 5f5f 6e61 6d65 5f5f 203d 3d20 224e 6f6e  __name__ == "Non
+0001cf70: 6554 7970 6522 3a0d 0a20 2020 2020 2020  eType":..       
+0001cf80: 2020 2020 2020 2020 2063 6f6e 7469 6e75           continu
+0001cf90: 650d 0a0d 0a20 2020 2020 2020 2020 2020  e....           
+0001cfa0: 2023 2320 7072 696e 7420 6375 7272 656e   ## print curren
+0001cfb0: 7420 7374 6570 0d0a 2020 2020 2020 2020  t step..        
+0001cfc0: 2020 2020 6966 2066 6c61 6773 2e65 7865      if flags.exe
+0001cfd0: 6375 7465 3a0d 0a20 2020 2020 2020 2020  cute:..         
+0001cfe0: 2020 2020 2020 2073 656c 662e 5f6c 6f67         self._log
+0001cff0: 2822 696e 666f 222c 2073 7465 705f 6e61  ("info", step_na
+0001d000: 6d65 2c20 3029 0d0a 0d0a 2020 2020 2020  me, 0)....      
+0001d010: 2020 2020 2020 6966 2073 7465 705f 6e61        if step_na
+0001d020: 6d65 203d 3d20 2276 6973 7561 6c69 7a61  me == "visualiza
+0001d030: 7469 6f6e 2220 616e 6420 666c 6167 732e  tion" and flags.
+0001d040: 6578 6563 7574 653a 0d0a 0d0a 2020 2020  execute:....    
+0001d050: 2020 2020 2020 2020 2020 2020 2323 2063              ## c
+0001d060: 6865 636b 2069 6620 6361 6e76 6173 2069  heck if canvas i
+0001d070: 7320 7365 6c65 6374 6564 2c20 616e 6420  s selected, and 
+0001d080: 6f74 6865 7277 6973 6520 6578 6563 7574  otherwise execut
+0001d090: 6520 7769 7468 2064 6566 6175 6c74 2076  e with default v
+0001d0a0: 616c 7565 730d 0a20 2020 2020 2020 2020  alues..         
+0001d0b0: 2020 2020 2020 2063 6865 636b 5f6c 6973         check_lis
+0001d0c0: 7420 3d20 5b0d 0a20 2020 2020 2020 2020  t = [..         
+0001d0d0: 2020 2020 2020 2020 2020 206c 6973 7428             list(
+0001d0e0: 6469 6374 2869 292e 6b65 7973 2829 295b  dict(i).keys())[
+0001d0f0: 305d 2069 6620 6e6f 7420 6973 696e 7374  0] if not isinst
+0001d100: 616e 6365 2869 2c20 7374 7229 2065 6c73  ance(i, str) els
+0001d110: 6520 690d 0a20 2020 2020 2020 2020 2020  e i..           
+0001d120: 2020 2020 2020 2020 2066 6f72 2069 2069           for i i
+0001d130: 6e20 6d65 7468 6f64 5f6c 6973 740d 0a20  n method_list.. 
+0001d140: 2020 2020 2020 2020 2020 2020 2020 205d                 ]
+0001d150: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001d160: 2020 6966 2028 0d0a 2020 2020 2020 2020    if (..        
+0001d170: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0001d180: 2e63 6f6e 7461 696e 6572 2e63 616e 7661  .container.canva
+0001d190: 732e 5f5f 636c 6173 735f 5f2e 5f5f 6e61  s.__class__.__na
+0001d1a0: 6d65 5f5f 203d 3d20 224e 6f6e 6554 7970  me__ == "NoneTyp
+0001d1b0: 6522 0d0a 2020 2020 2020 2020 2020 2020  e"..            
+0001d1c0: 2020 2020 2020 2020 616e 6420 6e6f 7420          and not 
+0001d1d0: 2273 656c 6563 745f 6361 6e76 6173 2220  "select_canvas" 
+0001d1e0: 696e 2063 6865 636b 5f6c 6973 740d 0a20  in check_list.. 
+0001d1f0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+0001d200: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+0001d210: 2020 2020 2020 2073 656c 662e 636f 6e74         self.cont
+0001d220: 6169 6e65 722e 5f72 756e 2822 7365 6c65  ainer._run("sele
+0001d230: 6374 5f63 616e 7661 7322 290d 0a20 2020  ct_canvas")..   
+0001d240: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d250: 2069 6620 666c 6167 732e 696e 7465 7261   if flags.intera
+0001d260: 6374 6976 6520 616e 6420 666c 6167 732e  ctive and flags.
+0001d270: 6175 746f 7368 6f77 3a0d 0a20 2020 2020  autoshow:..     
+0001d280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d290: 2020 2073 656c 662e 5f6c 6f67 2822 696e     self._log("in
+0001d2a0: 666f 222c 2022 7365 6c65 6374 5f63 616e  fo", "select_can
+0001d2b0: 7661 7320 2844 4546 4155 4c54 2922 2c20  vas (DEFAULT)", 
+0001d2c0: 3129 0d0a 2020 2020 2020 2020 2020 2020  1)..            
+0001d2d0: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+0001d2e0: 2020 2020 2020 2020 2020 2323 2069 7465            ## ite
+0001d2f0: 7261 7465 2074 6872 6f75 6768 2073 7465  rate through ste
+0001d300: 7020 6c69 7374 0d0a 2020 2020 2020 2020  p list..        
+0001d310: 2020 2020 666f 7220 6d65 7468 6f64 5f69      for method_i
+0001d320: 6478 2c20 6d65 7468 6f64 2069 6e20 656e  dx, method in en
+0001d330: 756d 6572 6174 6528 6d65 7468 6f64 5f6c  umerate(method_l
+0001d340: 6973 7429 3a0d 0a0d 0a20 2020 2020 2020  ist):....       
+0001d350: 2020 2020 2020 2020 2023 203d 3d3d 3d3d           # =====
 0001d360: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0001d370: 3d3d 3d3d 3d3d 3d3d 3d3d 3d0d 0a20 2020  ===========..   
-0001d380: 2020 2020 2020 2020 2020 2020 2023 204d               # M
-0001d390: 4554 484f 4420 2f20 4558 5452 4143 5449  ETHOD / EXTRACTI
-0001d3a0: 4f4e 2041 4e44 2043 4845 434b 0d0a 2020  ON AND CHECK..  
-0001d3b0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-0001d3c0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0001d3d0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0001d3e0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0001d370: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0001d380: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0001d390: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0001d3a0: 3d3d 3d3d 3d3d 3d3d 0d0a 2020 2020 2020  ========..      
+0001d3b0: 2020 2020 2020 2020 2020 2320 4d45 5448            # METH
+0001d3c0: 4f44 202f 2045 5854 5241 4354 494f 4e20  OD / EXTRACTION 
+0001d3d0: 414e 4420 4348 4543 4b0d 0a20 2020 2020  AND CHECK..     
+0001d3e0: 2020 2020 2020 2020 2020 2023 203d 3d3d             # ===
 0001d3f0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0001d400: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d0d 0a0d  =============...
-0001d410: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001d420: 2023 2320 666f 726d 6174 206d 6574 686f   ## format metho
-0001d430: 6420 6e61 6d65 2061 6e64 2061 7267 756d  d name and argum
-0001d440: 656e 7473 0d0a 2020 2020 2020 2020 2020  ents..          
-0001d450: 2020 2020 2020 6966 2069 7369 6e73 7461        if isinsta
-0001d460: 6e63 6528 6d65 7468 6f64 2c20 2864 6963  nce(method, (dic
-0001d470: 742c 204f 7264 6572 6564 4469 6374 2c20  t, OrderedDict, 
-0001d480: 436f 6d6d 656e 7465 644d 6170 2929 3a0d  CommentedMap)):.
-0001d490: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001d4a0: 2020 2020 206d 6574 686f 6420 3d20 6469       method = di
-0001d4b0: 6374 286d 6574 686f 6429 0d0a 2020 2020  ct(method)..    
+0001d400: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0001d410: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0001d420: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0001d430: 3d3d 3d3d 3d3d 3d3d 3d3d 0d0a 0d0a 2020  ==========....  
+0001d440: 2020 2020 2020 2020 2020 2020 2020 2323                ##
+0001d450: 2066 6f72 6d61 7420 6d65 7468 6f64 206e   format method n
+0001d460: 616d 6520 616e 6420 6172 6775 6d65 6e74  ame and argument
+0001d470: 730d 0a20 2020 2020 2020 2020 2020 2020  s..             
+0001d480: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
+0001d490: 286d 6574 686f 642c 2028 6469 6374 2c20  (method, (dict, 
+0001d4a0: 4f72 6465 7265 6444 6963 742c 2043 6f6d  OrderedDict, Com
+0001d4b0: 6d65 6e74 6564 4d61 7029 293a 0d0a 2020  mentedMap)):..  
 0001d4c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d4d0: 6d65 7468 6f64 5f6e 616d 6520 3d20 6e65  method_name = ne
-0001d4e0: 7874 2869 7465 7228 6d65 7468 6f64 2929  xt(iter(method))
-0001d4f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001d500: 2020 2020 2020 6d65 7468 6f64 5f61 7267        method_arg
-0001d510: 7320 3d20 6469 6374 286d 6574 686f 645b  s = dict(method[
-0001d520: 6d65 7468 6f64 5f6e 616d 655d 2920 6966  method_name]) if
-0001d530: 206d 6574 686f 645b 6d65 7468 6f64 5f6e   method[method_n
-0001d540: 616d 655d 2069 7320 6e6f 7420 4e6f 6e65  ame] is not None
-0001d550: 2065 6c73 6520 7b7d 0d0a 2020 2020 2020   else {}..      
-0001d560: 2020 2020 2020 2020 2020 656c 6966 2069            elif i
-0001d570: 7369 6e73 7461 6e63 6528 6d65 7468 6f64  sinstance(method
-0001d580: 2c20 7374 7229 3a0d 0a20 2020 2020 2020  , str):..       
-0001d590: 2020 2020 2020 2020 2020 2020 206d 6574               met
-0001d5a0: 686f 645f 6e61 6d65 203d 206d 6574 686f  hod_name = metho
-0001d5b0: 640d 0a20 2020 2020 2020 2020 2020 2020  d..             
-0001d5c0: 2020 2020 2020 206d 6574 686f 645f 6172         method_ar
-0001d5d0: 6773 203d 207b 7d0d 0a20 2020 2020 2020  gs = {}..       
-0001d5e0: 2020 2020 2020 2020 2020 2020 200d 0a20               .. 
-0001d5f0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-0001d600: 2320 6665 6564 6261 636b 202d 2063 6865  # feedback - che
-0001d610: 636b 2069 6620 6d65 7468 6f64 2065 7869  ck if method exi
-0001d620: 7374 730d 0a20 2020 2020 2020 2020 2020  sts..           
-0001d630: 2020 2020 2069 6620 666c 6167 732e 6578       if flags.ex
-0001d640: 6563 7574 653a 0d0a 2020 2020 2020 2020  ecute:..        
-0001d650: 2020 2020 2020 2020 2020 2020 6966 2068              if h
-0001d660: 6173 6174 7472 2865 7661 6c28 2263 6f72  asattr(eval("cor
-0001d670: 652e 222b 2073 7465 705f 6e61 6d65 292c  e."+ step_name),
-0001d680: 206d 6574 686f 645f 6e61 6d65 2920 6f72   method_name) or
-0001d690: 2068 6173 6174 7472 2865 7661 6c28 2270   hasattr(eval("p
-0001d6a0: 6c75 6769 6e73 2e22 2b20 7374 6570 5f6e  lugins."+ step_n
-0001d6b0: 616d 6529 2c20 6d65 7468 6f64 5f6e 616d  ame), method_nam
-0001d6c0: 6529 3a0d 0a20 2020 2020 2020 2020 2020  e):..           
-0001d6d0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0001d6e0: 662e 636f 6e66 6967 5f70 6172 7365 645f  f.config_parsed_
-0001d6f0: 666c 6174 7465 6e65 645b 7374 6570 5f6e  flattened[step_n
-0001d700: 616d 655d 2e61 7070 656e 6428 6d65 7468  ame].append(meth
-0001d710: 6f64 5f6e 616d 6529 0d0a 2020 2020 2020  od_name)..      
-0001d720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d730: 2020 7365 6c66 2e5f 6c6f 6728 2269 6e66    self._log("inf
-0001d740: 6f22 2c20 6d65 7468 6f64 5f6e 616d 652c  o", method_name,
-0001d750: 2031 290d 0a20 2020 2020 2020 2020 2020   1)..           
-0001d760: 2020 2020 2020 2020 2065 6c73 653a 2020           else:  
-0001d770: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
-0001d780: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-0001d790: 656c 662e 666c 6167 732e 6669 785f 6e61  elf.flags.fix_na
-0001d7a0: 6d65 7320 616e 6420 6d65 7468 6f64 5f6e  mes and method_n
-0001d7b0: 616d 6520 696e 205f 7661 7273 2e5f 6c65  ame in _vars._le
-0001d7c0: 6761 6379 5f6e 616d 6573 5b73 7465 705f  gacy_names[step_
-0001d7d0: 6e61 6d65 5d3a 0d0a 2020 2020 2020 2020  name]:..        
-0001d7e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d7f0: 2020 2020 6d65 7468 6f64 5f6e 616d 655f      method_name_
-0001d800: 7570 6461 7465 6420 3d20 5f76 6172 732e  updated = _vars.
-0001d810: 5f6c 6567 6163 795f 6e61 6d65 735b 7374  _legacy_names[st
-0001d820: 6570 5f6e 616d 655d 5b0d 0a20 2020 2020  ep_name][..     
-0001d830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d840: 2020 2020 2020 2020 2020 206d 6574 686f             metho
-0001d850: 645f 6e61 6d65 0d0a 2020 2020 2020 2020  d_name..        
+0001d4d0: 2020 6d65 7468 6f64 203d 2064 6963 7428    method = dict(
+0001d4e0: 6d65 7468 6f64 290d 0a20 2020 2020 2020  method)..       
+0001d4f0: 2020 2020 2020 2020 2020 2020 206d 6574               met
+0001d500: 686f 645f 6e61 6d65 203d 206e 6578 7428  hod_name = next(
+0001d510: 6974 6572 286d 6574 686f 6429 290d 0a20  iter(method)).. 
+0001d520: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d530: 2020 206d 6574 686f 645f 6172 6773 203d     method_args =
+0001d540: 2064 6963 7428 6d65 7468 6f64 5b6d 6574   dict(method[met
+0001d550: 686f 645f 6e61 6d65 5d29 2069 6620 6d65  hod_name]) if me
+0001d560: 7468 6f64 5b6d 6574 686f 645f 6e61 6d65  thod[method_name
+0001d570: 5d20 6973 206e 6f74 204e 6f6e 6520 656c  ] is not None el
+0001d580: 7365 207b 7d0d 0a20 2020 2020 2020 2020  se {}..         
+0001d590: 2020 2020 2020 2065 6c69 6620 6973 696e         elif isin
+0001d5a0: 7374 616e 6365 286d 6574 686f 642c 2073  stance(method, s
+0001d5b0: 7472 293a 0d0a 2020 2020 2020 2020 2020  tr):..          
+0001d5c0: 2020 2020 2020 2020 2020 6d65 7468 6f64            method
+0001d5d0: 5f6e 616d 6520 3d20 6d65 7468 6f64 0d0a  _name = method..
+0001d5e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d5f0: 2020 2020 6d65 7468 6f64 5f61 7267 7320      method_args 
+0001d600: 3d20 7b7d 0d0a 2020 2020 2020 2020 2020  = {}..          
+0001d610: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
+0001d620: 2020 2020 2020 2020 2020 2020 2323 2066              ## f
+0001d630: 6565 6462 6163 6b20 2d20 6368 6563 6b20  eedback - check 
+0001d640: 6966 206d 6574 686f 6420 6578 6973 7473  if method exists
+0001d650: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001d660: 2020 6966 2066 6c61 6773 2e65 7865 6375    if flags.execu
+0001d670: 7465 3a0d 0a20 2020 2020 2020 2020 2020  te:..           
+0001d680: 2020 2020 2020 2020 2069 6620 6861 7361           if hasa
+0001d690: 7474 7228 6576 616c 2822 636f 7265 2e22  ttr(eval("core."
+0001d6a0: 2b20 7374 6570 5f6e 616d 6529 2c20 6d65  + step_name), me
+0001d6b0: 7468 6f64 5f6e 616d 6529 206f 7220 6861  thod_name) or ha
+0001d6c0: 7361 7474 7228 6576 616c 2822 706c 7567  sattr(eval("plug
+0001d6d0: 696e 732e 222b 2073 7465 705f 6e61 6d65  ins."+ step_name
+0001d6e0: 292c 206d 6574 686f 645f 6e61 6d65 293a  ), method_name):
+0001d6f0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001d700: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+0001d710: 6f6e 6669 675f 7061 7273 6564 5f66 6c61  onfig_parsed_fla
+0001d720: 7474 656e 6564 5b73 7465 705f 6e61 6d65  ttened[step_name
+0001d730: 5d2e 6170 7065 6e64 286d 6574 686f 645f  ].append(method_
+0001d740: 6e61 6d65 290d 0a20 2020 2020 2020 2020  name)..         
+0001d750: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0001d760: 656c 662e 5f6c 6f67 2822 696e 666f 222c  elf._log("info",
+0001d770: 206d 6574 686f 645f 6e61 6d65 2c20 3129   method_name, 1)
+0001d780: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001d790: 2020 2020 2020 656c 7365 3a20 2020 200d        else:    .
+0001d7a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001d7b0: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+0001d7c0: 2e66 6c61 6773 2e66 6978 5f6e 616d 6573  .flags.fix_names
+0001d7d0: 2061 6e64 206d 6574 686f 645f 6e61 6d65   and method_name
+0001d7e0: 2069 6e20 5f76 6172 732e 5f6c 6567 6163   in _vars._legac
+0001d7f0: 795f 6e61 6d65 735b 7374 6570 5f6e 616d  y_names[step_nam
+0001d800: 655d 3a0d 0a20 2020 2020 2020 2020 2020  e]:..           
+0001d810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d820: 206d 6574 686f 645f 6e61 6d65 5f75 7064   method_name_upd
+0001d830: 6174 6564 203d 205f 7661 7273 2e5f 6c65  ated = _vars._le
+0001d840: 6761 6379 5f6e 616d 6573 5b73 7465 705f  gacy_names[step_
+0001d850: 6e61 6d65 5d5b 0d0a 2020 2020 2020 2020  name][..        
 0001d860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d870: 2020 2020 5d0d 0a20 2020 2020 2020 2020      ]..         
-0001d880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d890: 2020 2073 656c 662e 636f 6e66 6967 5f75     self.config_u
-0001d8a0: 7064 6174 6564 5b22 7072 6f63 6573 7369  pdated["processi
-0001d8b0: 6e67 5f73 7465 7073 225d 5b73 7465 705f  ng_steps"][step_
-0001d8c0: 6964 785d 5b73 7465 705f 6e61 6d65 5d5b  idx][step_name][
-0001d8d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001d8e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d8f0: 2020 6d65 7468 6f64 5f69 6478 0d0a 2020    method_idx..  
+0001d870: 2020 2020 2020 2020 6d65 7468 6f64 5f6e          method_n
+0001d880: 616d 650d 0a20 2020 2020 2020 2020 2020  ame..           
+0001d890: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d8a0: 205d 0d0a 2020 2020 2020 2020 2020 2020   ]..            
+0001d8b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d8c0: 7365 6c66 2e63 6f6e 6669 675f 7570 6461  self.config_upda
+0001d8d0: 7465 645b 2270 726f 6365 7373 696e 675f  ted["processing_
+0001d8e0: 7374 6570 7322 5d5b 7374 6570 5f69 6478  steps"][step_idx
+0001d8f0: 5d5b 7374 6570 5f6e 616d 655d 5b0d 0a20  ][step_name][.. 
 0001d900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001d910: 2020 2020 2020 2020 2020 5d20 3d20 7b6d            ] = {m
-0001d920: 6574 686f 645f 6e61 6d65 5f75 7064 6174  ethod_name_updat
-0001d930: 6564 3a20 6d65 7468 6f64 5f61 7267 737d  ed: method_args}
-0001d940: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001d950: 2020 2020 2020 2020 2020 2020 2020 6d65                me
-0001d960: 7468 6f64 5f6e 616d 6520 3d20 6d65 7468  thod_name = meth
-0001d970: 6f64 5f6e 616d 655f 7570 6461 7465 640d  od_name_updated.
-0001d980: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001d990: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0001d9a0: 662e 5f6c 6f67 2822 696e 666f 222c 2066  f._log("info", f
-0001d9b0: 227b 6d65 7468 6f64 5f6e 616d 657d 2064  "{method_name} d
-0001d9c0: 6f65 7320 6e6f 7420 6578 6973 7420 696e  oes not exist in
-0001d9d0: 2070 6865 6e6f 7079 7065 2e7b 7374 6570   phenopype.{step
-0001d9e0: 5f6e 616d 657d 202d 2075 7064 6174 6564  _name} - updated
-0001d9f0: 206d 6574 686f 6420 6e61 6d65 2074 6f20   method name to 
-0001da00: 7b6d 6574 686f 645f 6e61 6d65 5f75 7064  {method_name_upd
-0001da10: 6174 6564 7d22 2c20 3129 0d0a 2020 2020  ated}", 1)..    
-0001da20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001da30: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
-0001da40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001da50: 2020 2020 2020 2065 7272 6f72 5f6d 7367         error_msg
-0001da60: 203d 2020 6622 7b6d 6574 686f 645f 6e61   =  f"{method_na
-0001da70: 6d65 7d20 646f 6573 206e 6f74 2065 7869  me} does not exi
-0001da80: 7374 2069 6e20 7068 656e 6f70 7970 652e  st in phenopype.
-0001da90: 636f 7265 2e7b 7374 6570 5f6e 616d 657d  core.{step_name}
-0001daa0: 206f 7220 7068 656e 6f70 7970 655f 706c   or phenopype_pl
-0001dab0: 7567 696e 732e 7b73 7465 705f 6e61 6d65  ugins.{step_name
-0001dac0: 7d20 6d6f 6475 6c65 732e 220d 0a20 2020  } modules."..   
-0001dad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001dae0: 2020 2020 2020 2020 2073 656c 662e 5f6c           self._l
-0001daf0: 6f67 2822 6572 726f 7222 2c20 6572 726f  og("error", erro
-0001db00: 725f 6d73 672c 2031 290d 0a20 2020 2020  r_msg, 1)..     
-0001db10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001db20: 2020 2020 2020 2072 6169 7365 204e 616d         raise Nam
-0001db30: 6545 7272 6f72 2865 7272 6f72 5f6d 7367  eError(error_msg
-0001db40: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-0001db50: 2020 2020 2020 2020 2020 2020 2020 200d                 .
-0001db60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001db70: 2023 203d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d   # =============
-0001db80: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0001db90: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0001d910: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+0001d920: 6574 686f 645f 6964 780d 0a20 2020 2020  ethod_idx..     
+0001d930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d940: 2020 2020 2020 205d 203d 207b 6d65 7468         ] = {meth
+0001d950: 6f64 5f6e 616d 655f 7570 6461 7465 643a  od_name_updated:
+0001d960: 206d 6574 686f 645f 6172 6773 7d0d 0a20   method_args}.. 
+0001d970: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d980: 2020 2020 2020 2020 2020 206d 6574 686f             metho
+0001d990: 645f 6e61 6d65 203d 206d 6574 686f 645f  d_name = method_
+0001d9a0: 6e61 6d65 5f75 7064 6174 6564 0d0a 2020  name_updated..  
+0001d9b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001d9c0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
+0001d9d0: 6c6f 6728 2269 6e66 6f22 2c20 6622 7b6d  log("info", f"{m
+0001d9e0: 6574 686f 645f 6e61 6d65 7d20 646f 6573  ethod_name} does
+0001d9f0: 206e 6f74 2065 7869 7374 2069 6e20 7068   not exist in ph
+0001da00: 656e 6f70 7970 652e 7b73 7465 705f 6e61  enopype.{step_na
+0001da10: 6d65 7d20 2d20 7570 6461 7465 6420 6d65  me} - updated me
+0001da20: 7468 6f64 206e 616d 6520 746f 207b 6d65  thod name to {me
+0001da30: 7468 6f64 5f6e 616d 655f 7570 6461 7465  thod_name_update
+0001da40: 647d 222c 2031 290d 0a20 2020 2020 2020  d}", 1)..       
+0001da50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001da60: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
+0001da70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001da80: 2020 2020 6572 726f 725f 6d73 6720 3d20      error_msg = 
+0001da90: 2066 227b 6d65 7468 6f64 5f6e 616d 657d   f"{method_name}
+0001daa0: 2064 6f65 7320 6e6f 7420 6578 6973 7420   does not exist 
+0001dab0: 696e 2070 6865 6e6f 7079 7065 2e63 6f72  in phenopype.cor
+0001dac0: 652e 7b73 7465 705f 6e61 6d65 7d20 6f72  e.{step_name} or
+0001dad0: 2070 6865 6e6f 7079 7065 5f70 6c75 6769   phenopype_plugi
+0001dae0: 6e73 2e7b 7374 6570 5f6e 616d 657d 206d  ns.{step_name} m
+0001daf0: 6f64 756c 6573 2e22 0d0a 2020 2020 2020  odules."..      
+0001db00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001db10: 2020 2020 2020 7365 6c66 2e5f 6c6f 6728        self._log(
+0001db20: 2265 7272 6f72 222c 2065 7272 6f72 5f6d  "error", error_m
+0001db30: 7367 2c20 3129 0d0a 2020 2020 2020 2020  sg, 1)..        
+0001db40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001db50: 2020 2020 7261 6973 6520 4e61 6d65 4572      raise NameEr
+0001db60: 726f 7228 6572 726f 725f 6d73 6729 0d0a  ror(error_msg)..
+0001db70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001db80: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
+0001db90: 2020 2020 2020 2020 2020 2020 2020 2320                # 
 0001dba0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 0001dbb0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0001dbc0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001dbd0: 2020 2320 4d45 5448 4f44 202f 2041 4e4e    # METHOD / ANN
-0001dbe0: 4f54 4154 494f 4e0d 0a20 2020 2020 2020  OTATION..       
-0001dbf0: 2020 2020 2020 2020 2023 203d 3d3d 3d3d           # =====
-0001dc00: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0001dc10: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0001dc20: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0001dbc0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0001dbd0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0001dbe0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d0d 0a20  =============.. 
+0001dbf0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+0001dc00: 204d 4554 484f 4420 2f20 414e 4e4f 5441   METHOD / ANNOTA
+0001dc10: 5449 4f4e 0d0a 2020 2020 2020 2020 2020  TION..          
+0001dc20: 2020 2020 2020 2320 3d3d 3d3d 3d3d 3d3d        # ========
 0001dc30: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0001dc40: 3d3d 3d3d 3d3d 3d3d 0d0a 2020 2020 2020  ========..      
-0001dc50: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-0001dc60: 2020 2020 2020 2020 2020 2020 6966 206d              if m
-0001dc70: 6574 686f 645f 6e61 6d65 2069 6e20 6c69  ethod_name in li
-0001dc80: 7374 285f 7661 7273 2e5f 616e 6e6f 7461  st(_vars._annota
-0001dc90: 7469 6f6e 5f66 756e 6374 696f 6e73 2e6b  tion_functions.k
-0001dca0: 6579 7328 2929 202b 205b 2263 6f6e 7665  eys()) + ["conve
-0001dcb0: 7274 5f61 6e6e 6f74 6174 696f 6e22 5d3a  rt_annotation"]:
-0001dcc0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001dcd0: 2020 2020 2020 6966 2022 414e 4e4f 5441        if "ANNOTA
-0001dce0: 5449 4f4e 2220 696e 206d 6574 686f 645f  TION" in method_
-0001dcf0: 6172 6773 3a0d 0a20 2020 2020 2020 2020  args:..         
-0001dd00: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-0001dd10: 6e6e 6f74 6174 696f 6e5f 6172 6773 203d  nnotation_args =
-0001dd20: 2064 6963 7428 6d65 7468 6f64 5f61 7267   dict(method_arg
-0001dd30: 735b 2241 4e4e 4f54 4154 494f 4e22 5d29  s["ANNOTATION"])
-0001dd40: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001dd50: 2020 2020 2020 2020 2020 6465 6c20 6d65            del me
-0001dd60: 7468 6f64 5f61 7267 735b 2241 4e4e 4f54  thod_args["ANNOT
-0001dd70: 4154 494f 4e22 5d0d 0a20 2020 2020 2020  ATION"]..       
-0001dd80: 2020 2020 2020 2020 2020 2020 2065 6c73               els
-0001dd90: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-0001dda0: 2020 2020 2020 2020 2020 2020 616e 6e6f              anno
-0001ddb0: 7461 7469 6f6e 5f61 7267 7320 3d20 7b7d  tation_args = {}
-0001ddc0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001ddd0: 2020 2020 2020 2020 2020 6d65 7468 6f64            method
-0001dde0: 5f61 7267 7320 3d20 6469 6374 286d 6574  _args = dict(met
-0001ddf0: 686f 645f 6172 6773 290d 0a20 2020 2020  hod_args)..     
-0001de00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001de10: 2020 2073 656c 662e 5f6c 6f67 2822 6465     self._log("de
-0001de20: 6275 6722 2c20 2250 7970 653a 2041 6464  bug", "Pype: Add
-0001de30: 2061 6e6e 6f74 6174 696f 6e20 636f 6e74   annotation cont
-0001de40: 726f 6c20 6172 6773 222c 2030 290d 0a0d  rol args", 0)...
-0001de50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001de60: 2023 2320 616e 6e6f 7461 7469 6f6e 2070   ## annotation p
-0001de70: 6172 616d 730d 0a20 2020 2020 2020 2020  arams..         
-0001de80: 2020 2020 2020 2069 6620 6d65 7468 6f64         if method
-0001de90: 5f6e 616d 6520 696e 205f 7661 7273 2e5f  _name in _vars._
-0001dea0: 616e 6e6f 7461 7469 6f6e 5f66 756e 6374  annotation_funct
-0001deb0: 696f 6e73 3a0d 0a0d 0a20 2020 2020 2020  ions:....       
-0001dec0: 2020 2020 2020 2020 2020 2020 2061 6e6e               ann
-0001ded0: 6f74 6174 696f 6e5f 636f 756e 7465 725b  otation_counter[
-0001dee0: 5f76 6172 732e 5f61 6e6e 6f74 6174 696f  _vars._annotatio
-0001def0: 6e5f 6675 6e63 7469 6f6e 735b 6d65 7468  n_functions[meth
-0001df00: 6f64 5f6e 616d 655d 5d20 2b3d 2031 0d0a  od_name]] += 1..
-0001df10: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001df20: 2020 2020 2020 6966 206e 6f74 2022 7479        if not "ty
-0001df30: 7065 2220 696e 2061 6e6e 6f74 6174 696f  pe" in annotatio
-0001df40: 6e5f 6172 6773 3a0d 0a20 2020 2020 2020  n_args:..       
-0001df50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001df60: 2061 6e6e 6f74 6174 696f 6e5f 6172 6773   annotation_args
-0001df70: 2e75 7064 6174 6528 7b22 7479 7065 223a  .update({"type":
-0001df80: 205f 7661 7273 2e5f 616e 6e6f 7461 7469   _vars._annotati
-0001df90: 6f6e 5f66 756e 6374 696f 6e73 5b6d 6574  on_functions[met
-0001dfa0: 686f 645f 6e61 6d65 5d7d 290d 0a20 2020  hod_name]})..   
-0001dfb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001dfc0: 2069 6620 6e6f 7420 2269 6422 2069 6e20   if not "id" in 
-0001dfd0: 616e 6e6f 7461 7469 6f6e 5f61 7267 733a  annotation_args:
-0001dfe0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001dff0: 2020 2020 2020 2020 2020 616e 6e6f 7461            annota
-0001e000: 7469 6f6e 5f61 7267 732e 7570 6461 7465  tion_args.update
-0001e010: 287b 2269 6422 3a20 7374 7269 6e67 2e61  ({"id": string.a
-0001e020: 7363 6969 5f6c 6f77 6572 6361 7365 5b61  scii_lowercase[a
-0001e030: 6e6e 6f74 6174 696f 6e5f 636f 756e 7465  nnotation_counte
-0001e040: 725b 5f76 6172 732e 5f61 6e6e 6f74 6174  r[_vars._annotat
-0001e050: 696f 6e5f 6675 6e63 7469 6f6e 735b 6d65  ion_functions[me
-0001e060: 7468 6f64 5f6e 616d 655d 5d5d 7d29 0d0a  thod_name]]]})..
-0001e070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e080: 2020 2020 6966 206e 6f74 2022 6564 6974      if not "edit
-0001e090: 2220 696e 2061 6e6e 6f74 6174 696f 6e5f  " in annotation_
-0001e0a0: 6172 6773 3a0d 0a20 2020 2020 2020 2020  args:..         
-0001e0b0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-0001e0c0: 6e6e 6f74 6174 696f 6e5f 6172 6773 2e75  nnotation_args.u
-0001e0d0: 7064 6174 6528 7b22 6564 6974 223a 2022  pdate({"edit": "
-0001e0e0: 6f76 6572 7772 6974 6522 2069 6620 6d65  overwrite" if me
-0001e0f0: 7468 6f64 5f6e 616d 6520 696e 205b 0d0a  thod_name in [..
-0001e100: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e120: 2020 2020 2263 6f6e 746f 7572 5f74 6f5f      "contour_to_
-0001e130: 6d61 736b 222c 0d0a 2020 2020 2020 2020  mask",..        
+0001dc40: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0001dc50: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0001dc60: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0001dc70: 3d3d 3d3d 3d0d 0a20 2020 2020 2020 2020  =====..         
+0001dc80: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+0001dc90: 2020 2020 2020 2020 2069 6620 6d65 7468           if meth
+0001dca0: 6f64 5f6e 616d 6520 696e 206c 6973 7428  od_name in list(
+0001dcb0: 5f76 6172 732e 5f61 6e6e 6f74 6174 696f  _vars._annotatio
+0001dcc0: 6e5f 6675 6e63 7469 6f6e 732e 6b65 7973  n_functions.keys
+0001dcd0: 2829 2920 2b20 5b22 636f 6e76 6572 745f  ()) + ["convert_
+0001dce0: 616e 6e6f 7461 7469 6f6e 225d 3a0d 0a20  annotation"]:.. 
+0001dcf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001dd00: 2020 2069 6620 2241 4e4e 4f54 4154 494f     if "ANNOTATIO
+0001dd10: 4e22 2069 6e20 6d65 7468 6f64 5f61 7267  N" in method_arg
+0001dd20: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
+0001dd30: 2020 2020 2020 2020 2020 2020 616e 6e6f              anno
+0001dd40: 7461 7469 6f6e 5f61 7267 7320 3d20 6469  tation_args = di
+0001dd50: 6374 286d 6574 686f 645f 6172 6773 5b22  ct(method_args["
+0001dd60: 414e 4e4f 5441 5449 4f4e 225d 290d 0a20  ANNOTATION"]).. 
+0001dd70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001dd80: 2020 2020 2020 2064 656c 206d 6574 686f         del metho
+0001dd90: 645f 6172 6773 5b22 414e 4e4f 5441 5449  d_args["ANNOTATI
+0001dda0: 4f4e 225d 0d0a 2020 2020 2020 2020 2020  ON"]..          
+0001ddb0: 2020 2020 2020 2020 2020 656c 7365 3a0d            else:.
+0001ddc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001ddd0: 2020 2020 2020 2020 2061 6e6e 6f74 6174           annotat
+0001dde0: 696f 6e5f 6172 6773 203d 207b 7d0d 0a20  ion_args = {}.. 
+0001ddf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001de00: 2020 2020 2020 206d 6574 686f 645f 6172         method_ar
+0001de10: 6773 203d 2064 6963 7428 6d65 7468 6f64  gs = dict(method
+0001de20: 5f61 7267 7329 0d0a 2020 2020 2020 2020  _args)..        
+0001de30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001de40: 7365 6c66 2e5f 6c6f 6728 2264 6562 7567  self._log("debug
+0001de50: 222c 2022 5079 7065 3a20 4164 6420 616e  ", "Pype: Add an
+0001de60: 6e6f 7461 7469 6f6e 2063 6f6e 7472 6f6c  notation control
+0001de70: 2061 7267 7322 2c20 3029 0d0a 0d0a 2020   args", 0)....  
+0001de80: 2020 2020 2020 2020 2020 2020 2020 2323                ##
+0001de90: 2061 6e6e 6f74 6174 696f 6e20 7061 7261   annotation para
+0001dea0: 6d73 0d0a 2020 2020 2020 2020 2020 2020  ms..            
+0001deb0: 2020 2020 6966 206d 6574 686f 645f 6e61      if method_na
+0001dec0: 6d65 2069 6e20 5f76 6172 732e 5f61 6e6e  me in _vars._ann
+0001ded0: 6f74 6174 696f 6e5f 6675 6e63 7469 6f6e  otation_function
+0001dee0: 733a 0d0a 0d0a 2020 2020 2020 2020 2020  s:....          
+0001def0: 2020 2020 2020 2020 2020 616e 6e6f 7461            annota
+0001df00: 7469 6f6e 5f63 6f75 6e74 6572 5b5f 7661  tion_counter[_va
+0001df10: 7273 2e5f 616e 6e6f 7461 7469 6f6e 5f66  rs._annotation_f
+0001df20: 756e 6374 696f 6e73 5b6d 6574 686f 645f  unctions[method_
+0001df30: 6e61 6d65 5d5d 202b 3d20 310d 0a0d 0a20  name]] += 1.... 
+0001df40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001df50: 2020 2069 6620 6e6f 7420 2274 7970 6522     if not "type"
+0001df60: 2069 6e20 616e 6e6f 7461 7469 6f6e 5f61   in annotation_a
+0001df70: 7267 733a 0d0a 2020 2020 2020 2020 2020  rgs:..          
+0001df80: 2020 2020 2020 2020 2020 2020 2020 616e                an
+0001df90: 6e6f 7461 7469 6f6e 5f61 7267 732e 7570  notation_args.up
+0001dfa0: 6461 7465 287b 2274 7970 6522 3a20 5f76  date({"type": _v
+0001dfb0: 6172 732e 5f61 6e6e 6f74 6174 696f 6e5f  ars._annotation_
+0001dfc0: 6675 6e63 7469 6f6e 735b 6d65 7468 6f64  functions[method
+0001dfd0: 5f6e 616d 655d 7d29 0d0a 2020 2020 2020  _name]})..      
+0001dfe0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+0001dff0: 206e 6f74 2022 6964 2220 696e 2061 6e6e   not "id" in ann
+0001e000: 6f74 6174 696f 6e5f 6172 6773 3a0d 0a20  otation_args:.. 
+0001e010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e020: 2020 2020 2020 2061 6e6e 6f74 6174 696f         annotatio
+0001e030: 6e5f 6172 6773 2e75 7064 6174 6528 7b22  n_args.update({"
+0001e040: 6964 223a 2073 7472 696e 672e 6173 6369  id": string.asci
+0001e050: 695f 6c6f 7765 7263 6173 655b 616e 6e6f  i_lowercase[anno
+0001e060: 7461 7469 6f6e 5f63 6f75 6e74 6572 5b5f  tation_counter[_
+0001e070: 7661 7273 2e5f 616e 6e6f 7461 7469 6f6e  vars._annotation
+0001e080: 5f66 756e 6374 696f 6e73 5b6d 6574 686f  _functions[metho
+0001e090: 645f 6e61 6d65 5d5d 5d7d 290d 0a20 2020  d_name]]]})..   
+0001e0a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e0b0: 2069 6620 6e6f 7420 2265 6469 7422 2069   if not "edit" i
+0001e0c0: 6e20 616e 6e6f 7461 7469 6f6e 5f61 7267  n annotation_arg
+0001e0d0: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
+0001e0e0: 2020 2020 2020 2020 2020 2020 616e 6e6f              anno
+0001e0f0: 7461 7469 6f6e 5f61 7267 732e 7570 6461  tation_args.upda
+0001e100: 7465 287b 2265 6469 7422 3a20 226f 7665  te({"edit": "ove
+0001e110: 7277 7269 7465 2220 6966 206d 6574 686f  rwrite" if metho
+0001e120: 645f 6e61 6d65 2069 6e20 5b0d 0a20 2020  d_name in [..   
+0001e130: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0001e140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e150: 2020 2020 2020 2020 2020 2020 2264 6574              "det
-0001e160: 6563 745f 636f 6e74 6f75 7222 2c0d 0a20  ect_contour",.. 
+0001e150: 2022 636f 6e74 6f75 725f 746f 5f6d 6173   "contour_to_mas
+0001e160: 6b22 2c0d 0a20 2020 2020 2020 2020 2020  k",..           
 0001e170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e190: 2020 2022 6465 7465 6374 5f6d 6173 6b22     "detect_mask"
-0001e1a0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+0001e180: 2020 2020 2020 2020 2022 6465 7465 6374           "detect
+0001e190: 5f63 6f6e 746f 7572 222c 0d0a 2020 2020  _contour",..    
+0001e1a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0001e1b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e1c0: 2020 2020 2020 2022 636f 6d70 7574 655f         "compute_
-0001e1d0: 7368 6170 655f 6665 6174 7572 6573 222c  shape_features",
-0001e1e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001e1f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e200: 2020 2020 2020 2263 6f6d 7075 7465 5f74        "compute_t
-0001e210: 6578 7475 7265 5f66 6561 7475 7265 7322  exture_features"
-0001e220: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-0001e230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e240: 2020 2020 2020 2022 6465 7465 6374 5f73         "detect_s
-0001e250: 6b65 6c65 746f 6e22 2c0d 0a20 2020 2020  keleton",..     
+0001e1c0: 2264 6574 6563 745f 6d61 736b 222c 0d0a  "detect_mask",..
+0001e1d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e1e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e1f0: 2020 2020 2263 6f6d 7075 7465 5f73 6861      "compute_sha
+0001e200: 7065 5f66 6561 7475 7265 7322 2c0d 0a20  pe_features",.. 
+0001e210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e230: 2020 2022 636f 6d70 7574 655f 7465 7874     "compute_text
+0001e240: 7572 655f 6665 6174 7572 6573 222c 0d0a  ure_features",..
+0001e250: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0001e260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e270: 2020 2020 2020 2020 2020 205d 2065 6c73             ] els
-0001e280: 6520 4661 6c73 6520 7d29 0d0a 0d0a 0d0a  e False })......
+0001e270: 2020 2020 2264 6574 6563 745f 736b 656c      "detect_skel
+0001e280: 6574 6f6e 222c 0d0a 2020 2020 2020 2020  eton",..        
 0001e290: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e2a0: 656c 6966 206d 6574 686f 645f 6e61 6d65  elif method_name
-0001e2b0: 2069 6e20 5b22 636f 6e76 6572 745f 616e   in ["convert_an
-0001e2c0: 6e6f 7461 7469 6f6e 225d 3a0d 0a20 2020  notation"]:..   
-0001e2d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e2e0: 2074 7279 3a0d 0a20 2020 2020 2020 2020   try:..         
-0001e2f0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-0001e300: 6e6e 6f74 6174 696f 6e5f 7479 7065 203d  nnotation_type =
-0001e310: 206d 6574 686f 645f 6172 6773 5b22 616e   method_args["an
-0001e320: 6e6f 7461 7469 6f6e 5f74 7970 655f 6e65  notation_type_ne
-0001e330: 7722 5d0d 0a20 2020 2020 2020 2020 2020  w"]..           
-0001e340: 2020 2020 2020 2020 2020 2020 2061 6e6e               ann
-0001e350: 6f74 6174 696f 6e5f 6964 203d 206d 6574  otation_id = met
-0001e360: 686f 645f 6172 6773 5b22 616e 6e6f 7461  hod_args["annota
-0001e370: 7469 6f6e 5f69 645f 6e65 7722 5d0d 0a20  tion_id_new"].. 
-0001e380: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e390: 2020 2020 2020 2061 6e6e 6f74 6174 696f         annotatio
-0001e3a0: 6e5f 6172 6773 2e75 7064 6174 6528 7b22  n_args.update({"
-0001e3b0: 7479 7065 223a 616e 6e6f 7461 7469 6f6e  type":annotation
-0001e3c0: 5f74 7970 652c 2022 6964 223a 616e 6e6f  _type, "id":anno
-0001e3d0: 7461 7469 6f6e 5f69 642c 2022 6564 6974  tation_id, "edit
-0001e3e0: 223a 226f 7665 7277 7269 7465 227d 290d  ":"overwrite"}).
-0001e3f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001e400: 2020 2020 2065 7863 6570 7420 4b65 7945       except KeyE
-0001e410: 7272 6f72 3a0d 0a20 2020 2020 2020 2020  rror:..         
-0001e420: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0001e430: 656c 662e 5f6c 6f67 2822 6572 726f 7222  elf._log("error"
-0001e440: 2c20 2250 7970 653a 204d 6973 7369 6e67  , "Pype: Missing
-0001e450: 2061 7267 756d 656e 7473 2066 6f72 2061   arguments for a
-0001e460: 6e6e 6f74 6174 696f 6e20 636f 6e76 6572  nnotation conver
-0001e470: 7369 6f6e 222c 2030 290d 0a0d 0a20 2020  sion", 0)....   
-0001e480: 2020 2020 2020 2020 2020 2020 2065 6c73               els
-0001e490: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-0001e4a0: 2020 2020 2020 2020 616e 6e6f 7461 7469          annotati
-0001e4b0: 6f6e 5f61 7267 7320 3d20 7b7d 0d0a 0d0a  on_args = {}....
-0001e4c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e4d0: 2323 2063 7265 6174 6520 414e 4e4f 5441  ## create ANNOTA
-0001e4e0: 5449 4f4e 2073 7472 696e 6720 616e 6420  TION string and 
-0001e4f0: 6164 6420 746f 2063 6f6e 6669 670d 0a20  add to config.. 
-0001e500: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0001e510: 6620 616e 6e6f 7461 7469 6f6e 5f61 7267  f annotation_arg
-0001e520: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
-0001e530: 2020 2020 2020 2020 616e 6e6f 7461 7469          annotati
-0001e540: 6f6e 5f61 7267 7320 3d20 756c 2e5f 7961  on_args = ul._ya
-0001e550: 6d6c 5f66 6c6f 775f 7374 796c 6528 616e  ml_flow_style(an
-0001e560: 6e6f 7461 7469 6f6e 5f61 7267 7329 0d0a  notation_args)..
-0001e570: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e580: 2020 2020 6d65 7468 6f64 5f61 7267 735f      method_args_
-0001e590: 7570 6461 7465 6420 3d20 7b22 414e 4e4f  updated = {"ANNO
-0001e5a0: 5441 5449 4f4e 223a 2061 6e6e 6f74 6174  TATION": annotat
-0001e5b0: 696f 6e5f 6172 6773 7d0d 0a20 2020 2020  ion_args}..     
-0001e5c0: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-0001e5d0: 6574 686f 645f 6172 6773 5f75 7064 6174  ethod_args_updat
-0001e5e0: 6564 2e75 7064 6174 6528 6d65 7468 6f64  ed.update(method
-0001e5f0: 5f61 7267 7329 0d0a 2020 2020 2020 2020  _args)..        
-0001e600: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0001e610: 2e63 6f6e 6669 675f 7570 6461 7465 645b  .config_updated[
-0001e620: 2270 726f 6365 7373 696e 675f 7374 6570  "processing_step
-0001e630: 7322 5d5b 7374 6570 5f69 6478 5d5b 7374  s"][step_idx][st
-0001e640: 6570 5f6e 616d 655d 5b6d 6574 686f 645f  ep_name][method_
-0001e650: 6964 785d 203d 207b 6d65 7468 6f64 5f6e  idx] = {method_n
-0001e660: 616d 653a 206d 6574 686f 645f 6172 6773  ame: method_args
-0001e670: 5f75 7064 6174 6564 7d0d 0a0d 0a20 2020  _updated}....   
-0001e680: 2020 2020 2020 2020 2020 2020 2023 203d               # =
-0001e690: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0001e6a0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0001e6b0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0001e2a0: 2020 2020 2020 2020 5d20 656c 7365 2046          ] else F
+0001e2b0: 616c 7365 207d 290d 0a0d 0a0d 0a20 2020  alse })......   
+0001e2c0: 2020 2020 2020 2020 2020 2020 2065 6c69               eli
+0001e2d0: 6620 6d65 7468 6f64 5f6e 616d 6520 696e  f method_name in
+0001e2e0: 205b 2263 6f6e 7665 7274 5f61 6e6e 6f74   ["convert_annot
+0001e2f0: 6174 696f 6e22 5d3a 0d0a 2020 2020 2020  ation"]:..      
+0001e300: 2020 2020 2020 2020 2020 2020 2020 7472                tr
+0001e310: 793a 0d0a 2020 2020 2020 2020 2020 2020  y:..            
+0001e320: 2020 2020 2020 2020 2020 2020 616e 6e6f              anno
+0001e330: 7461 7469 6f6e 5f74 7970 6520 3d20 6d65  tation_type = me
+0001e340: 7468 6f64 5f61 7267 735b 2261 6e6e 6f74  thod_args["annot
+0001e350: 6174 696f 6e5f 7479 7065 5f6e 6577 225d  ation_type_new"]
+0001e360: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001e370: 2020 2020 2020 2020 2020 616e 6e6f 7461            annota
+0001e380: 7469 6f6e 5f69 6420 3d20 6d65 7468 6f64  tion_id = method
+0001e390: 5f61 7267 735b 2261 6e6e 6f74 6174 696f  _args["annotatio
+0001e3a0: 6e5f 6964 5f6e 6577 225d 0d0a 2020 2020  n_id_new"]..    
+0001e3b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e3c0: 2020 2020 616e 6e6f 7461 7469 6f6e 5f61      annotation_a
+0001e3d0: 7267 732e 7570 6461 7465 287b 2274 7970  rgs.update({"typ
+0001e3e0: 6522 3a61 6e6e 6f74 6174 696f 6e5f 7479  e":annotation_ty
+0001e3f0: 7065 2c20 2269 6422 3a61 6e6e 6f74 6174  pe, "id":annotat
+0001e400: 696f 6e5f 6964 2c20 2265 6469 7422 3a22  ion_id, "edit":"
+0001e410: 6f76 6572 7772 6974 6522 7d29 0d0a 2020  overwrite"})..  
+0001e420: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e430: 2020 6578 6365 7074 204b 6579 4572 726f    except KeyErro
+0001e440: 723a 0d0a 2020 2020 2020 2020 2020 2020  r:..            
+0001e450: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0001e460: 2e5f 6c6f 6728 2265 7272 6f72 222c 2022  ._log("error", "
+0001e470: 5079 7065 3a20 4d69 7373 696e 6720 6172  Pype: Missing ar
+0001e480: 6775 6d65 6e74 7320 666f 7220 616e 6e6f  guments for anno
+0001e490: 7461 7469 6f6e 2063 6f6e 7665 7273 696f  tation conversio
+0001e4a0: 6e22 2c20 3029 0d0a 0d0a 2020 2020 2020  n", 0)....      
+0001e4b0: 2020 2020 2020 2020 2020 656c 7365 3a0d            else:.
+0001e4c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001e4d0: 2020 2020 2061 6e6e 6f74 6174 696f 6e5f       annotation_
+0001e4e0: 6172 6773 203d 207b 7d0d 0a0d 0a20 2020  args = {}....   
+0001e4f0: 2020 2020 2020 2020 2020 2020 2023 2320               ## 
+0001e500: 6372 6561 7465 2041 4e4e 4f54 4154 494f  create ANNOTATIO
+0001e510: 4e20 7374 7269 6e67 2061 6e64 2061 6464  N string and add
+0001e520: 2074 6f20 636f 6e66 6967 0d0a 2020 2020   to config..    
+0001e530: 2020 2020 2020 2020 2020 2020 6966 2061              if a
+0001e540: 6e6e 6f74 6174 696f 6e5f 6172 6773 3a0d  nnotation_args:.
+0001e550: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001e560: 2020 2020 2061 6e6e 6f74 6174 696f 6e5f       annotation_
+0001e570: 6172 6773 203d 2075 6c2e 5f79 616d 6c5f  args = ul._yaml_
+0001e580: 666c 6f77 5f73 7479 6c65 2861 6e6e 6f74  flow_style(annot
+0001e590: 6174 696f 6e5f 6172 6773 290d 0a20 2020  ation_args)..   
+0001e5a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e5b0: 206d 6574 686f 645f 6172 6773 5f75 7064   method_args_upd
+0001e5c0: 6174 6564 203d 207b 2241 4e4e 4f54 4154  ated = {"ANNOTAT
+0001e5d0: 494f 4e22 3a20 616e 6e6f 7461 7469 6f6e  ION": annotation
+0001e5e0: 5f61 7267 737d 0d0a 2020 2020 2020 2020  _args}..        
+0001e5f0: 2020 2020 2020 2020 2020 2020 6d65 7468              meth
+0001e600: 6f64 5f61 7267 735f 7570 6461 7465 642e  od_args_updated.
+0001e610: 7570 6461 7465 286d 6574 686f 645f 6172  update(method_ar
+0001e620: 6773 290d 0a20 2020 2020 2020 2020 2020  gs)..           
+0001e630: 2020 2020 2020 2020 2073 656c 662e 636f           self.co
+0001e640: 6e66 6967 5f75 7064 6174 6564 5b22 7072  nfig_updated["pr
+0001e650: 6f63 6573 7369 6e67 5f73 7465 7073 225d  ocessing_steps"]
+0001e660: 5b73 7465 705f 6964 785d 5b73 7465 705f  [step_idx][step_
+0001e670: 6e61 6d65 5d5b 6d65 7468 6f64 5f69 6478  name][method_idx
+0001e680: 5d20 3d20 7b6d 6574 686f 645f 6e61 6d65  ] = {method_name
+0001e690: 3a20 6d65 7468 6f64 5f61 7267 735f 7570  : method_args_up
+0001e6a0: 6461 7465 647d 0d0a 0d0a 2020 2020 2020  dated}....      
+0001e6b0: 2020 2020 2020 2020 2020 2320 3d3d 3d3d            # ====
 0001e6c0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0001e6d0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 0d0a 2020  ============..  
-0001e6e0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-0001e6f0: 4d45 5448 4f44 202f 2045 5845 4355 5445  METHOD / EXECUTE
-0001e700: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001e710: 2020 2320 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d    # ============
-0001e720: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0001e730: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0001e740: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0001e6d0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0001e6e0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0001e6f0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0001e700: 3d3d 3d3d 3d3d 3d3d 3d0d 0a20 2020 2020  =========..     
+0001e710: 2020 2020 2020 2020 2020 2023 204d 4554             # MET
+0001e720: 484f 4420 2f20 4558 4543 5554 450d 0a20  HOD / EXECUTE.. 
+0001e730: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+0001e740: 203d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d   ===============
 0001e750: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0001e760: 3d0d 0a0d 0a20 2020 2020 2020 2020 2020  =....           
-0001e770: 2020 2020 2023 2320 7275 6e20 6d65 7468       ## run meth
-0001e780: 6f64 2077 6974 6820 6572 726f 7220 6861  od with error ha
-0001e790: 6e64 6c69 6e67 0d0a 2020 2020 2020 2020  ndling..        
-0001e7a0: 2020 2020 2020 2020 6966 2066 6c61 6773          if flags
-0001e7b0: 2e65 7865 6375 7465 3a0d 0a20 2020 2020  .execute:..     
-0001e7c0: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
-0001e7d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e7e0: 2023 2320 6f70 656e 2062 7566 6665 720d   ## open buffer.
-0001e7f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001e800: 2020 2020 2062 7566 6665 7220 3d20 696f       buffer = io
-0001e810: 2e53 7472 696e 6749 4f28 290d 0a20 2020  .StringIO()..   
+0001e760: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0001e770: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0001e780: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 0d0a  ==============..
+0001e790: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001e7a0: 2020 2323 2072 756e 206d 6574 686f 6420    ## run method 
+0001e7b0: 7769 7468 2065 7272 6f72 2068 616e 646c  with error handl
+0001e7c0: 696e 670d 0a20 2020 2020 2020 2020 2020  ing..           
+0001e7d0: 2020 2020 2069 6620 666c 6167 732e 6578       if flags.ex
+0001e7e0: 6563 7574 653a 0d0a 2020 2020 2020 2020  ecute:..        
+0001e7f0: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+0001e800: 2020 2020 2020 2020 2020 2020 2020 2323                ##
+0001e810: 206f 7065 6e20 6275 6666 6572 0d0a 2020   open buffer..  
 0001e820: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e830: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
-0001e840: 2020 2020 2020 2023 2320 736f 6d65 2066         ## some f
-0001e850: 756e 6374 696f 6e20 7370 6563 6966 6963  unction specific
-0001e860: 2073 7769 7463 6865 730d 0a20 2020 2020   switches..     
-0001e870: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-0001e880: 6574 686f 645f 6172 6773 5b22 696e 7465  ethod_args["inte
-0001e890: 7261 6374 6976 6522 5d20 3d20 666c 6167  ractive"] = flag
-0001e8a0: 732e 696e 7465 7261 6374 6976 6520 2020  s.interactive   
-0001e8b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e8c0: 2020 2020 200d 0a20 2020 2020 2020 2020       ..         
-0001e8d0: 2020 2020 2020 2020 2020 206d 6574 686f             metho
-0001e8e0: 645f 6172 6773 5b22 7a6f 6f6d 5f6d 656d  d_args["zoom_mem
-0001e8f0: 6f72 7922 5d20 3d20 7365 6c66 2e66 6c61  ory"] = self.fla
-0001e900: 6773 2e7a 6f6f 6d5f 6d65 6d6f 7279 2020  gs.zoom_memory  
-0001e910: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-0001e920: 2020 2020 2020 2020 2020 2020 2020 206d                 m
-0001e930: 6574 686f 645f 6172 6773 5b22 7471 646d  ethod_args["tqdm
-0001e940: 5f6f 6666 225d 203d 206e 6f74 2073 656c  _off"] = not sel
-0001e950: 662e 666c 6167 732e 6665 6564 6261 636b  f.flags.feedback
-0001e960: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0001e970: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
-0001e980: 2020 2020 2020 2020 2020 2020 2323 2065              ## e
-0001e990: 7863 6563 7574 6520 616e 6420 6361 7074  xcecute and capt
-0001e9a0: 7572 6520 7374 646f 7574 0d0a 2020 2020  ure stdout..    
-0001e9b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001e9c0: 7472 793a 0d0a 2020 2020 2020 2020 2020  try:..          
-0001e9d0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-0001e9e0: 206e 6f74 2073 656c 662e 666c 6167 732e   not self.flags.
-0001e9f0: 6465 6275 673a 0d0a 2020 2020 2020 2020  debug:..        
-0001ea00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ea10: 2020 2020 7769 7468 2072 6564 6972 6563      with redirec
-0001ea20: 745f 7374 646f 7574 2862 7566 6665 7229  t_stdout(buffer)
-0001ea30: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-0001ea40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ea50: 2020 2073 656c 662e 636f 6e74 6169 6e65     self.containe
-0001ea60: 722e 5f72 756e 280d 0a20 2020 2020 2020  r._run(..       
+0001e830: 2020 6275 6666 6572 203d 2069 6f2e 5374    buffer = io.St
+0001e840: 7269 6e67 494f 2829 0d0a 2020 2020 2020  ringIO()..      
+0001e850: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+0001e860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e870: 2020 2020 2323 2073 6f6d 6520 6675 6e63      ## some func
+0001e880: 7469 6f6e 2073 7065 6369 6669 6320 7377  tion specific sw
+0001e890: 6974 6368 6573 0d0a 2020 2020 2020 2020  itches..        
+0001e8a0: 2020 2020 2020 2020 2020 2020 6d65 7468              meth
+0001e8b0: 6f64 5f61 7267 735b 2269 6e74 6572 6163  od_args["interac
+0001e8c0: 7469 7665 225d 203d 2066 6c61 6773 2e69  tive"] = flags.i
+0001e8d0: 6e74 6572 6163 7469 7665 2020 2020 2020  nteractive      
+0001e8e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e8f0: 2020 0d0a 2020 2020 2020 2020 2020 2020    ..            
+0001e900: 2020 2020 2020 2020 6d65 7468 6f64 5f61          method_a
+0001e910: 7267 735b 227a 6f6f 6d5f 6d65 6d6f 7279  rgs["zoom_memory
+0001e920: 225d 203d 2073 656c 662e 666c 6167 732e  "] = self.flags.
+0001e930: 7a6f 6f6d 5f6d 656d 6f72 7920 2020 2020  zoom_memory     
+0001e940: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+0001e950: 2020 2020 2020 2020 2020 2020 6d65 7468              meth
+0001e960: 6f64 5f61 7267 735b 2274 7164 6d5f 6f66  od_args["tqdm_of
+0001e970: 6622 5d20 3d20 6e6f 7420 7365 6c66 2e66  f"] = not self.f
+0001e980: 6c61 6773 2e66 6565 6462 6163 6b0d 0a20  lags.feedback.. 
+0001e990: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001e9a0: 2020 200d 0a20 2020 2020 2020 2020 2020     ..           
+0001e9b0: 2020 2020 2020 2020 2023 2320 6578 6365           ## exce
+0001e9c0: 6375 7465 2061 6e64 2063 6170 7475 7265  cute and capture
+0001e9d0: 2073 7464 6f75 740d 0a20 2020 2020 2020   stdout..       
+0001e9e0: 2020 2020 2020 2020 2020 2020 2074 7279               try
+0001e9f0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
+0001ea00: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
+0001ea10: 7420 7365 6c66 2e66 6c61 6773 2e64 6562  t self.flags.deb
+0001ea20: 7567 3a0d 0a20 2020 2020 2020 2020 2020  ug:..           
+0001ea30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ea40: 2077 6974 6820 7265 6469 7265 6374 5f73   with redirect_s
+0001ea50: 7464 6f75 7428 6275 6666 6572 293a 0d0a  tdout(buffer):..
+0001ea60: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0001ea70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ea80: 2020 2020 2020 2020 2020 2020 2066 756e               fun
-0001ea90: 3d6d 6574 686f 645f 6e61 6d65 2c0d 0a20  =method_name,.. 
+0001ea80: 7365 6c66 2e63 6f6e 7461 696e 6572 2e5f  self.container._
+0001ea90: 7275 6e28 0d0a 2020 2020 2020 2020 2020  run(..          
 0001eaa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001eab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001eac0: 2020 2066 756e 5f6b 7761 7267 733d 6d65     fun_kwargs=me
-0001ead0: 7468 6f64 5f61 7267 732c 0d0a 2020 2020  thod_args,..    
+0001eab0: 2020 2020 2020 2020 2020 6675 6e3d 6d65            fun=me
+0001eac0: 7468 6f64 5f6e 616d 652c 0d0a 2020 2020  thod_name,..    
+0001ead0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0001eae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001eaf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001eb00: 616e 6e6f 7461 7469 6f6e 5f6b 7761 7267  annotation_kwarg
-0001eb10: 733d 616e 6e6f 7461 7469 6f6e 5f61 7267  s=annotation_arg
-0001eb20: 732c 0d0a 2020 2020 2020 2020 2020 2020  s,..            
-0001eb30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001eb40: 2020 2020 2020 2020 616e 6e6f 7461 7469          annotati
-0001eb50: 6f6e 5f63 6f75 6e74 6572 3d61 6e6e 6f74  on_counter=annot
-0001eb60: 6174 696f 6e5f 636f 756e 7465 722c 0d0a  ation_counter,..
-0001eb70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001eb80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001eb90: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+0001eaf0: 6675 6e5f 6b77 6172 6773 3d6d 6574 686f  fun_kwargs=metho
+0001eb00: 645f 6172 6773 2c0d 0a20 2020 2020 2020  d_args,..       
+0001eb10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001eb20: 2020 2020 2020 2020 2020 2020 2061 6e6e               ann
+0001eb30: 6f74 6174 696f 6e5f 6b77 6172 6773 3d61  otation_kwargs=a
+0001eb40: 6e6e 6f74 6174 696f 6e5f 6172 6773 2c0d  nnotation_args,.
+0001eb50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001eb60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001eb70: 2020 2020 2061 6e6e 6f74 6174 696f 6e5f       annotation_
+0001eb80: 636f 756e 7465 723d 616e 6e6f 7461 7469  counter=annotati
+0001eb90: 6f6e 5f63 6f75 6e74 6572 2c0d 0a20 2020  on_counter,..   
 0001eba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ebb0: 2020 2073 7464 6f75 7420 3d20 6275 6666     stdout = buff
-0001ebc0: 6572 2e67 6574 7661 6c75 6528 290d 0a20  er.getvalue().. 
+0001ebb0: 2020 2020 2020 2020 2020 2020 2029 0d0a               )..
+0001ebc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0001ebd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ebe0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0001ebf0: 656c 662e 5f6c 6f67 2822 696e 666f 222c  elf._log("info",
-0001ec00: 2073 7464 6f75 742c 2032 290d 0a20 2020   stdout, 2)..   
-0001ec10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ec20: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
-0001ec30: 6669 672e 6c61 7374 5f70 7269 6e74 5f6d  fig.last_print_m
-0001ec40: 7367 203d 2022 220d 0a20 2020 2020 2020  sg = ""..       
-0001ec50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ec60: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
-0001ec70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ec80: 2020 2020 7365 6c66 2e63 6f6e 7461 696e      self.contain
-0001ec90: 6572 2e5f 7275 6e28 0d0a 2020 2020 2020  er._run(..      
+0001ebe0: 7374 646f 7574 203d 2062 7566 6665 722e  stdout = buffer.
+0001ebf0: 6765 7476 616c 7565 2829 0d0a 2020 2020  getvalue()..    
+0001ec00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ec10: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0001ec20: 2e5f 6c6f 6728 2269 6e66 6f22 2c20 7374  ._log("info", st
+0001ec30: 646f 7574 2c20 3229 0d0a 2020 2020 2020  dout, 2)..      
+0001ec40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ec50: 2020 2020 2020 2020 2020 636f 6e66 6967            config
+0001ec60: 2e6c 6173 745f 7072 696e 745f 6d73 6720  .last_print_msg 
+0001ec70: 3d20 2222 0d0a 2020 2020 2020 2020 2020  = ""..          
+0001ec80: 2020 2020 2020 2020 2020 2020 2020 656c                el
+0001ec90: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
 0001eca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ecb0: 2020 2020 2020 2020 2020 6675 6e3d 6d65            fun=me
-0001ecc0: 7468 6f64 5f6e 616d 652c 0d0a 2020 2020  thod_name,..    
+0001ecb0: 2073 656c 662e 636f 6e74 6169 6e65 722e   self.container.
+0001ecc0: 5f72 756e 280d 0a20 2020 2020 2020 2020  _run(..         
 0001ecd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ece0: 2020 2020 2020 2020 2020 2020 6675 6e5f              fun_
-0001ecf0: 6b77 6172 6773 3d6d 6574 686f 645f 6172  kwargs=method_ar
-0001ed00: 6773 2c0d 0a20 2020 2020 2020 2020 2020  gs,..           
-0001ed10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ed20: 2020 2020 2061 6e6e 6f74 6174 696f 6e5f       annotation_
-0001ed30: 6b77 6172 6773 3d61 6e6e 6f74 6174 696f  kwargs=annotatio
-0001ed40: 6e5f 6172 6773 2c0d 0a20 2020 2020 2020  n_args,..       
-0001ed50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ed60: 2020 2020 2020 2020 2061 6e6e 6f74 6174           annotat
-0001ed70: 696f 6e5f 636f 756e 7465 723d 616e 6e6f  ion_counter=anno
-0001ed80: 7461 7469 6f6e 5f63 6f75 6e74 6572 2c0d  tation_counter,.
-0001ed90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001eda0: 2020 2020 2020 2020 2020 2020 2029 0d0a               )..
-0001edb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001edc0: 2020 2020 6578 6365 7074 2045 7863 6570      except Excep
-0001edd0: 7469 6f6e 2061 7320 6578 3a0d 0a20 2020  tion as ex:..   
+0001ece0: 2020 2020 2020 2066 756e 3d6d 6574 686f         fun=metho
+0001ecf0: 645f 6e61 6d65 2c0d 0a20 2020 2020 2020  d_name,..       
+0001ed00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ed10: 2020 2020 2020 2020 2066 756e 5f6b 7761           fun_kwa
+0001ed20: 7267 733d 6d65 7468 6f64 5f61 7267 732c  rgs=method_args,
+0001ed30: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001ed40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ed50: 2020 616e 6e6f 7461 7469 6f6e 5f6b 7761    annotation_kwa
+0001ed60: 7267 733d 616e 6e6f 7461 7469 6f6e 5f61  rgs=annotation_a
+0001ed70: 7267 732c 0d0a 2020 2020 2020 2020 2020  rgs,..          
+0001ed80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ed90: 2020 2020 2020 616e 6e6f 7461 7469 6f6e        annotation
+0001eda0: 5f63 6f75 6e74 6572 3d61 6e6e 6f74 6174  _counter=annotat
+0001edb0: 696f 6e5f 636f 756e 7465 722c 0d0a 2020  ion_counter,..  
+0001edc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001edd0: 2020 2020 2020 2020 2020 290d 0a20 2020            )..   
 0001ede0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001edf0: 2020 2020 2070 7269 6e74 2862 7566 6665       print(buffe
-0001ee00: 722e 6765 7476 616c 7565 2829 290d 0a20  r.getvalue()).. 
+0001edf0: 2065 7863 6570 7420 4578 6365 7074 696f   except Exceptio
+0001ee00: 6e20 6173 2065 783a 0d0a 2020 2020 2020  n as ex:..      
 0001ee10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ee20: 2020 2020 2020 2065 7272 6f72 5f6d 7367         error_msg
-0001ee30: 203d 2020 6622 7b73 7465 705f 6e61 6d65   =  f"{step_name
-0001ee40: 7d2e 7b6d 6574 686f 645f 6e61 6d65 7d3a  }.{method_name}:
-0001ee50: 207b 7374 7228 6578 2e5f 5f63 6c61 7373   {str(ex.__class
-0001ee60: 5f5f 2e5f 5f6e 616d 655f 5f29 7d20 2d20  __.__name__)} - 
-0001ee70: 7b65 787d 220d 0a20 2020 2020 2020 2020  {ex}"..         
-0001ee80: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0001ee90: 656c 662e 5f6c 6f67 2822 6572 726f 7222  elf._log("error"
-0001eea0: 2c20 6572 726f 725f 6d73 672c 2031 290d  , error_msg, 1).
-0001eeb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001eec0: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
-0001eed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001eee0: 2020 2023 2320 636c 6561 6e75 700d 0a20     ## cleanup.. 
-0001eef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ef00: 2020 2020 2020 2069 6620 7365 6c66 2e66         if self.f
-0001ef10: 6c61 6773 2e64 6562 7567 3a0d 0a20 2020  lags.debug:..   
+0001ee20: 2020 7072 696e 7428 6275 6666 6572 2e67    print(buffer.g
+0001ee30: 6574 7661 6c75 6528 2929 0d0a 2020 2020  etvalue())..    
+0001ee40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ee50: 2020 2020 6572 726f 725f 6d73 6720 3d20      error_msg = 
+0001ee60: 2066 227b 7374 6570 5f6e 616d 657d 2e7b   f"{step_name}.{
+0001ee70: 6d65 7468 6f64 5f6e 616d 657d 3a20 7b73  method_name}: {s
+0001ee80: 7472 2865 782e 5f5f 636c 6173 735f 5f2e  tr(ex.__class__.
+0001ee90: 5f5f 6e61 6d65 5f5f 297d 202d 207b 6578  __name__)} - {ex
+0001eea0: 7d22 0d0a 2020 2020 2020 2020 2020 2020  }"..            
+0001eeb0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0001eec0: 2e5f 6c6f 6728 2265 7272 6f72 222c 2065  ._log("error", e
+0001eed0: 7272 6f72 5f6d 7367 2c20 3129 0d0a 2020  rror_msg, 1)..  
+0001eee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001eef0: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+0001ef00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ef10: 2323 2063 6c65 616e 7570 0d0a 2020 2020  ## cleanup..    
 0001ef20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ef30: 2020 2020 2020 2020 2063 6f6e 6669 672e           config.
-0001ef40: 7665 7262 6f73 6520 3d20 7365 6c66 2e76  verbose = self.v
-0001ef50: 6572 626f 7365 0d0a 2020 2020 2020 2020  erbose..        
-0001ef60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ef70: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-0001ef80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001ef90: 2020 2323 2072 6169 7365 2065 7272 6f72    ## raise error
-0001efa0: 2061 6e64 2065 6e64 0d0a 2020 2020 2020   and end..      
-0001efb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001efc0: 2020 2020 2020 7261 6973 650d 0a0d 0a0d        raise.....
-0001efd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001efe0: 2020 2020 2023 2320 6368 6563 6b20 666f       ## check fo
-0001eff0: 7220 7079 7065 2d72 6573 7461 7274 2061  r pype-restart a
-0001f000: 6674 6572 2063 6f6e 6669 6720 6368 616e  fter config chan
-0001f010: 6765 0d0a 2020 2020 2020 2020 2020 2020  ge..            
-0001f020: 2020 2020 2020 2020 6966 2063 6f6e 6669          if confi
-0001f030: 672e 7079 7065 5f72 6573 7461 7274 3a0d  g.pype_restart:.
+0001ef30: 2020 2020 6966 2073 656c 662e 666c 6167      if self.flag
+0001ef40: 732e 6465 6275 673a 0d0a 2020 2020 2020  s.debug:..      
+0001ef50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001ef60: 2020 2020 2020 636f 6e66 6967 2e76 6572        config.ver
+0001ef70: 626f 7365 203d 2073 656c 662e 7665 7262  bose = self.verb
+0001ef80: 6f73 650d 0a20 2020 2020 2020 2020 2020  ose..           
+0001ef90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001efa0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+0001efb0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+0001efc0: 2320 7261 6973 6520 6572 726f 7220 616e  # raise error an
+0001efd0: 6420 656e 640d 0a20 2020 2020 2020 2020  d end..         
+0001efe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001eff0: 2020 2072 6169 7365 0d0a 0d0a 0d0a 2020     raise......  
+0001f000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f010: 2020 2323 2063 6865 636b 2066 6f72 2070    ## check for p
+0001f020: 7970 652d 7265 7374 6172 7420 6166 7465  ype-restart afte
+0001f030: 7220 636f 6e66 6967 2063 6861 6e67 650d  r config change.
 0001f040: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001f050: 2020 2020 2020 2020 2073 656c 662e 5f6c           self._l
-0001f060: 6f67 2822 6465 6275 6722 2c20 2250 7970  og("debug", "Pyp
-0001f070: 653a 2072 6573 7461 7274 222c 2030 290d  e: restart", 0).
-0001f080: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001f090: 2020 2020 2020 2020 2072 6574 7572 6e0d           return.
-0001f0a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001f0b0: 2020 2020 200d 0a20 2020 2020 2020 2023       ..        #
-0001f0c0: 2073 7973 2e73 7464 6f75 7420 3d20 7365   sys.stdout = se
-0001f0d0: 6c66 2e6f 6c64 5f73 7464 6f75 740d 0a0d  lf.old_stdout...
-0001f0e0: 0a20 2020 2020 2020 2023 203d 3d3d 3d3d  .        # =====
-0001f0f0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0001f100: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0001f110: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0001f050: 2020 2020 2069 6620 636f 6e66 6967 2e70       if config.p
+0001f060: 7970 655f 7265 7374 6172 743a 0d0a 2020  ype_restart:..  
+0001f070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f080: 2020 2020 2020 7365 6c66 2e5f 6c6f 6728        self._log(
+0001f090: 2264 6562 7567 222c 2022 5079 7065 3a20  "debug", "Pype: 
+0001f0a0: 7265 7374 6172 7422 2c20 3029 0d0a 2020  restart", 0)..  
+0001f0b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f0c0: 2020 2020 2020 7265 7475 726e 0d0a 2020        return..  
+0001f0d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f0e0: 2020 0d0a 2020 2020 2020 2020 2320 7379    ..        # sy
+0001f0f0: 732e 7374 646f 7574 203d 2073 656c 662e  s.stdout = self.
+0001f100: 6f6c 645f 7374 646f 7574 0d0a 0d0a 2020  old_stdout....  
+0001f110: 2020 2020 2020 2320 3d3d 3d3d 3d3d 3d3d        # ========
 0001f120: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0001f130: 3d3d 3d3d 3d3d 3d3d 0d0a 2020 2020 2020  ========..      
-0001f140: 2020 2320 434f 4e46 4947 2d55 5044 4154    # CONFIG-UPDAT
-0001f150: 4520 414e 4420 4155 544f 5348 4f57 2028  E AND AUTOSHOW (
-0001f160: 6f70 7469 6f6e 616c 290d 0a20 2020 2020  optional)..     
-0001f170: 2020 2023 203d 3d3d 3d3d 3d3d 3d3d 3d3d     # ===========
-0001f180: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0001f190: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0001f1a0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0001f130: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0001f140: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0001f150: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0001f160: 3d3d 3d3d 3d0d 0a20 2020 2020 2020 2023  =====..        #
+0001f170: 2043 4f4e 4649 472d 5550 4441 5445 2041   CONFIG-UPDATE A
+0001f180: 4e44 2041 5554 4f53 484f 5720 286f 7074  ND AUTOSHOW (opt
+0001f190: 696f 6e61 6c29 0d0a 2020 2020 2020 2020  ional)..        
+0001f1a0: 2320 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  # ==============
 0001f1b0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0001f1c0: 3d3d 0d0a 0d0a 2020 2020 2020 2020 6966  ==....        if
-0001f1d0: 206e 6f74 2073 656c 662e 636f 6e66 6967   not self.config
-0001f1e0: 5f75 7064 6174 6564 203d 3d20 7365 6c66  _updated == self
-0001f1f0: 2e63 6f6e 6669 673a 0d0a 2020 2020 2020  .config:..      
-0001f200: 2020 2020 2020 756c 2e5f 7361 7665 5f79        ul._save_y
-0001f210: 616d 6c28 7365 6c66 2e63 6f6e 6669 675f  aml(self.config_
-0001f220: 7570 6461 7465 642c 2073 656c 662e 636f  updated, self.co
-0001f230: 6e66 6967 5f70 6174 6829 0d0a 2020 2020  nfig_path)..    
-0001f240: 2020 2020 2020 2020 7365 6c66 2e5f 6c6f          self._lo
-0001f250: 6728 2264 6562 7567 222c 2022 5079 7065  g("debug", "Pype
-0001f260: 3a20 5570 6461 7469 6e67 2063 6f6e 6669  : Updating confi
-0001f270: 673b 2061 7070 6c79 696e 6720 7374 6167  g; applying stag
-0001f280: 6564 2063 6861 6e67 6573 222c 2030 290d  ed changes", 0).
-0001f290: 0a0d 0a20 2020 2020 2020 2069 6620 666c  ...        if fl
-0001f2a0: 6167 732e 6175 746f 7368 6f77 2061 6e64  ags.autoshow and
-0001f2b0: 2066 6c61 6773 2e65 7865 6375 7465 3a0d   flags.execute:.
-0001f2c0: 0a20 2020 2020 2020 2020 2020 2074 7279  .            try
-0001f2d0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-0001f2e0: 2020 2073 656c 662e 5f6c 6f67 2822 696e     self._log("in
-0001f2f0: 666f 222c 2022 5079 7065 3a20 4155 544f  fo", "Pype: AUTO
-0001f300: 5348 4f57 222c 2030 290d 0a20 2020 2020  SHOW", 0)..     
-0001f310: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-0001f320: 6c66 2e63 6f6e 7461 696e 6572 2e63 616e  lf.container.can
-0001f330: 7661 732e 5f5f 636c 6173 735f 5f2e 5f5f  vas.__class__.__
-0001f340: 6e61 6d65 5f5f 203d 3d20 224e 6f6e 6554  name__ == "NoneT
-0001f350: 7970 6522 3a0d 0a20 2020 2020 2020 2020  ype":..         
-0001f360: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0001f370: 636f 6e74 6169 6e65 722e 5f72 756e 2866  container._run(f
-0001f380: 756e 3d22 7365 6c65 6374 5f63 616e 7661  un="select_canva
-0001f390: 7322 290d 0a20 2020 2020 2020 2020 2020  s")..           
-0001f3a0: 2020 2020 2020 2020 2073 656c 662e 5f6c           self._l
-0001f3b0: 6f67 2822 696e 666f 222c 2022 7365 6c65  og("info", "sele
-0001f3c0: 6374 5f63 616e 7661 7322 2c20 3129 0d0a  ct_canvas", 1)..
-0001f3d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f3e0: 2020 2020 2020 2020 2020 2020 0d0a 2020              ..  
-0001f3f0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-0001f400: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0001f410: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0001f420: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0001f1c0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0001f1d0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0001f1e0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d0d  ===============.
+0001f1f0: 0a0d 0a20 2020 2020 2020 2069 6620 6e6f  ...        if no
+0001f200: 7420 7365 6c66 2e63 6f6e 6669 675f 7570  t self.config_up
+0001f210: 6461 7465 6420 3d3d 2073 656c 662e 636f  dated == self.co
+0001f220: 6e66 6967 3a0d 0a20 2020 2020 2020 2020  nfig:..         
+0001f230: 2020 2075 6c2e 5f73 6176 655f 7961 6d6c     ul._save_yaml
+0001f240: 2873 656c 662e 636f 6e66 6967 5f75 7064  (self.config_upd
+0001f250: 6174 6564 2c20 7365 6c66 2e63 6f6e 6669  ated, self.confi
+0001f260: 675f 7061 7468 290d 0a20 2020 2020 2020  g_path)..       
+0001f270: 2020 2020 2073 656c 662e 5f6c 6f67 2822       self._log("
+0001f280: 6465 6275 6722 2c20 2250 7970 653a 2055  debug", "Pype: U
+0001f290: 7064 6174 696e 6720 636f 6e66 6967 3b20  pdating config; 
+0001f2a0: 6170 706c 7969 6e67 2073 7461 6765 6420  applying staged 
+0001f2b0: 6368 616e 6765 7322 2c20 3029 0d0a 0d0a  changes", 0)....
+0001f2c0: 2020 2020 2020 2020 6966 2066 6c61 6773          if flags
+0001f2d0: 2e61 7574 6f73 686f 7720 616e 6420 666c  .autoshow and fl
+0001f2e0: 6167 732e 6578 6563 7574 653a 0d0a 2020  ags.execute:..  
+0001f2f0: 2020 2020 2020 2020 2020 7472 793a 0d0a            try:..
+0001f300: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f310: 7365 6c66 2e5f 6c6f 6728 2269 6e66 6f22  self._log("info"
+0001f320: 2c20 2250 7970 653a 2041 5554 4f53 484f  , "Pype: AUTOSHO
+0001f330: 5722 2c20 3029 0d0a 2020 2020 2020 2020  W", 0)..        
+0001f340: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0001f350: 636f 6e74 6169 6e65 722e 6361 6e76 6173  container.canvas
+0001f360: 2e5f 5f63 6c61 7373 5f5f 2e5f 5f6e 616d  .__class__.__nam
+0001f370: 655f 5f20 3d3d 2022 4e6f 6e65 5479 7065  e__ == "NoneType
+0001f380: 223a 0d0a 2020 2020 2020 2020 2020 2020  ":..            
+0001f390: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
+0001f3a0: 7461 696e 6572 2e5f 7275 6e28 6675 6e3d  tainer._run(fun=
+0001f3b0: 2273 656c 6563 745f 6361 6e76 6173 2229  "select_canvas")
+0001f3c0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0001f3d0: 2020 2020 2020 7365 6c66 2e5f 6c6f 6728        self._log(
+0001f3e0: 2269 6e66 6f22 2c20 2273 656c 6563 745f  "info", "select_
+0001f3f0: 6361 6e76 6173 222c 2031 290d 0a20 2020  canvas", 1)..   
+0001f400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0001f410: 2020 2020 2020 2020 200d 0a20 2020 2020           ..     
+0001f420: 2020 2020 2020 2020 2020 2023 203d 3d3d             # ===
 0001f430: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0001f440: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d0d 0a20  =============.. 
-0001f450: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-0001f460: 2046 4545 4442 4143 4b20 0d0a 2020 2020   FEEDBACK ..    
-0001f470: 2020 2020 0d0a 2020 2020 2020 2020 2020      ..          
-0001f480: 2020 2020 2020 636c 6f73 696e 675f 6d73        closing_ms
-0001f490: 675f 6c69 7374 203d 205b 5d0d 0a20 2020  g_list = []..   
-0001f4a0: 2020 2020 2020 2020 2020 2020 2063 6c6f               clo
-0001f4b0: 7369 6e67 5f6d 7367 5f6c 6973 742e 6170  sing_msg_list.ap
-0001f4c0: 7065 6e64 2820 756c 2e5f 7070 7269 6e74  pend( ul._pprint
-0001f4d0: 5f66 696c 6c5f 6862 6172 2822 7c20 6669  _fill_hbar("| fi
-0001f4e0: 6e69 7368 6564 2070 7970 6520 6974 6572  nished pype iter
-0001f4f0: 6174 696f 6e20 7c22 2c20 7265 743d 5472  ation |", ret=Tr
-0001f500: 7565 2929 0d0a 2020 2020 2020 2020 2020  ue))..          
-0001f510: 2020 2020 2020 6966 2066 6c61 6773 2e61        if flags.a
-0001f520: 7574 6f73 686f 773a 0d0a 2020 2020 2020  utoshow:..      
-0001f530: 2020 2020 2020 2020 2020 2020 2020 636c                cl
-0001f540: 6f73 696e 675f 6d73 675f 6c69 7374 2e61  osing_msg_list.a
-0001f550: 7070 656e 6428 2075 6c2e 5f70 7072 696e  ppend( ul._pprin
-0001f560: 745f 6669 6c6c 5f68 6261 7228 2228 456e  t_fill_hbar("(En
-0001f570: 6420 7769 7468 2043 7472 6c2b 456e 7465  d with Ctrl+Ente
-0001f580: 7220 6f72 2072 652d 7275 6e20 7769 7468  r or re-run with
-0001f590: 2045 6e74 6572 2922 2c20 7265 743d 5472   Enter)", ret=Tr
-0001f5a0: 7565 2929 0d0a 2020 2020 2020 2020 2020  ue))..          
-0001f5b0: 2020 2020 2020 7365 6c66 2e5f 6c6f 6728        self._log(
-0001f5c0: 2269 6e66 6f22 2c20 636c 6f73 696e 675f  "info", closing_
-0001f5d0: 6d73 675f 6c69 7374 2c20 3029 0d0a 2020  msg_list, 0)..  
-0001f5e0: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
-0001f5f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0001f600: 2320 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  # ==============
-0001f610: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0001f620: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0001f440: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0001f450: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0001f460: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0001f470: 3d3d 3d3d 3d3d 3d3d 3d3d 0d0a 2020 2020  ==========..    
+0001f480: 2020 2020 2020 2020 2020 2020 2320 4645              # FE
+0001f490: 4544 4241 434b 200d 0a20 2020 2020 2020  EDBACK ..       
+0001f4a0: 200d 0a20 2020 2020 2020 2020 2020 2020   ..             
+0001f4b0: 2020 2063 6c6f 7369 6e67 5f6d 7367 5f6c     closing_msg_l
+0001f4c0: 6973 7420 3d20 5b5d 0d0a 2020 2020 2020  ist = []..      
+0001f4d0: 2020 2020 2020 2020 2020 636c 6f73 696e            closin
+0001f4e0: 675f 6d73 675f 6c69 7374 2e61 7070 656e  g_msg_list.appen
+0001f4f0: 6428 2075 6c2e 5f70 7072 696e 745f 6669  d( ul._pprint_fi
+0001f500: 6c6c 5f68 6261 7228 227c 2066 696e 6973  ll_hbar("| finis
+0001f510: 6865 6420 7079 7065 2069 7465 7261 7469  hed pype iterati
+0001f520: 6f6e 207c 222c 2072 6574 3d54 7275 6529  on |", ret=True)
+0001f530: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+0001f540: 2020 2069 6620 666c 6167 732e 6175 746f     if flags.auto
+0001f550: 7368 6f77 3a0d 0a20 2020 2020 2020 2020  show:..         
+0001f560: 2020 2020 2020 2020 2020 2063 6c6f 7369             closi
+0001f570: 6e67 5f6d 7367 5f6c 6973 742e 6170 7065  ng_msg_list.appe
+0001f580: 6e64 2820 756c 2e5f 7070 7269 6e74 5f66  nd( ul._pprint_f
+0001f590: 696c 6c5f 6862 6172 2822 2845 6e64 2077  ill_hbar("(End w
+0001f5a0: 6974 6820 4374 726c 2b45 6e74 6572 206f  ith Ctrl+Enter o
+0001f5b0: 7220 7265 2d72 756e 2077 6974 6820 456e  r re-run with En
+0001f5c0: 7465 7229 222c 2072 6574 3d54 7275 6529  ter)", ret=True)
+0001f5d0: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
+0001f5e0: 2020 2073 656c 662e 5f6c 6f67 2822 696e     self._log("in
+0001f5f0: 666f 222c 2063 6c6f 7369 6e67 5f6d 7367  fo", closing_msg
+0001f600: 5f6c 6973 742c 2030 290d 0a20 2020 2020  _list, 0)..     
+0001f610: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+0001f620: 2020 2020 2020 2020 2020 2020 2023 203d               # =
 0001f630: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-0001f640: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d0d  ===============.
-0001f650: 0a20 2020 2020 2020 200d 0a20 2020 2020  .        ..     
-0001f660: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-0001f670: 6775 6920 3d20 756c 2e5f 4755 4928 7365  gui = ul._GUI(se
-0001f680: 6c66 2e63 6f6e 7461 696e 6572 2e63 616e  lf.container.can
-0001f690: 7661 732c 207a 6f6f 6d5f 6d65 6d6f 7279  vas, zoom_memory
-0001f6a0: 3d73 656c 662e 666c 6167 732e 7a6f 6f6d  =self.flags.zoom
-0001f6b0: 5f6d 656d 6f72 792c 2070 7970 655f 6d6f  _memory, pype_mo
-0001f6c0: 6465 3d54 7275 6529 0d0a 2020 2020 2020  de=True)..      
-0001f6d0: 2020 2020 2020 2020 2020 7365 6c66 2e66            self.f
-0001f6e0: 6c61 6773 2e74 6572 6d69 6e61 7465 203d  lags.terminate =
-0001f6f0: 2073 656c 662e 6775 692e 666c 6167 732e   self.gui.flags.
-0001f700: 656e 645f 7079 7065 0d0a 2020 2020 2020  end_pype..      
-0001f710: 2020 2020 2020 2020 2020 0d0a 2020 2020            ..    
-0001f720: 2020 2020 2020 2020 6578 6365 7074 2045          except E
-0001f730: 7863 6570 7469 6f6e 2061 7320 6578 3a0d  xception as ex:.
-0001f740: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001f750: 2065 7272 6f72 5f6d 7367 203d 2020 6622   error_msg =  f"
-0001f760: 5079 7065 3a20 4155 5453 484f 5720 7b73  Pype: AUTSHOW {s
-0001f770: 7472 2865 782e 5f5f 636c 6173 735f 5f2e  tr(ex.__class__.
-0001f780: 5f5f 6e61 6d65 5f5f 297d 202d 207b 6578  __name__)} - {ex
-0001f790: 7d22 0d0a 2020 2020 2020 2020 2020 2020  }"..            
-0001f7a0: 2020 2020 7365 6c66 2e5f 6c6f 6728 2265      self._log("e
-0001f7b0: 7272 6f72 222c 2065 7272 6f72 5f6d 7367  rror", error_msg
-0001f7c0: 2c20 3129 0d0a 2020 2020 2020 2020 656c  , 1)..        el
-0001f7d0: 7365 3a0d 0a20 2020 2020 2020 2020 2020  se:..           
-0001f7e0: 2069 6620 666c 6167 732e 6578 6563 7574   if flags.execut
-0001f7f0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-0001f800: 2020 2020 636c 6f73 696e 675f 6d73 6720      closing_msg 
-0001f810: 3d20 756c 2e5f 7070 7269 6e74 5f66 696c  = ul._pprint_fil
-0001f820: 6c5f 6862 6172 2822 7c20 6669 6e69 7368  l_hbar("| finish
-0001f830: 6564 2070 7970 6520 6974 6572 6174 696f  ed pype iteratio
-0001f840: 6e20 7c22 2c20 7265 743d 5472 7565 290d  n |", ret=True).
-0001f850: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0001f860: 2073 656c 662e 5f6c 6f67 2822 696e 666f   self._log("info
-0001f870: 222c 2063 6c6f 7369 6e67 5f6d 7367 2c20  ", closing_msg, 
-0001f880: 3029 0d0a 2020 2020 2020 2020 2020 2020  0)..            
-0001f890: 2020 2020 7365 6c66 2e66 6c61 6773 2e74      self.flags.t
-0001f8a0: 6572 6d69 6e61 7465 203d 2054 7275 650d  erminate = True.
-0001f8b0: 0a                                       .
+0001f640: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0001f650: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0001f660: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+0001f670: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 0d0a 2020  ============..  
+0001f680: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+0001f690: 2020 2020 2020 2020 7365 6c66 2e67 7569          self.gui
+0001f6a0: 203d 2075 6c2e 5f47 5549 2873 656c 662e   = ul._GUI(self.
+0001f6b0: 636f 6e74 6169 6e65 722e 6361 6e76 6173  container.canvas
+0001f6c0: 2c20 7a6f 6f6d 5f6d 656d 6f72 793d 7365  , zoom_memory=se
+0001f6d0: 6c66 2e66 6c61 6773 2e7a 6f6f 6d5f 6d65  lf.flags.zoom_me
+0001f6e0: 6d6f 7279 2c20 7079 7065 5f6d 6f64 653d  mory, pype_mode=
+0001f6f0: 5472 7565 290d 0a20 2020 2020 2020 2020  True)..         
+0001f700: 2020 2020 2020 2073 656c 662e 666c 6167         self.flag
+0001f710: 732e 7465 726d 696e 6174 6520 3d20 7365  s.terminate = se
+0001f720: 6c66 2e67 7569 2e66 6c61 6773 2e65 6e64  lf.gui.flags.end
+0001f730: 5f70 7970 650d 0a20 2020 2020 2020 2020  _pype..         
+0001f740: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+0001f750: 2020 2020 2065 7863 6570 7420 4578 6365       except Exce
+0001f760: 7074 696f 6e20 6173 2065 783a 0d0a 2020  ption as ex:..  
+0001f770: 2020 2020 2020 2020 2020 2020 2020 6572                er
+0001f780: 726f 725f 6d73 6720 3d20 2066 2250 7970  ror_msg =  f"Pyp
+0001f790: 653a 2041 5554 5348 4f57 207b 7374 7228  e: AUTSHOW {str(
+0001f7a0: 6578 2e5f 5f63 6c61 7373 5f5f 2e5f 5f6e  ex.__class__.__n
+0001f7b0: 616d 655f 5f29 7d20 2d20 7b65 787d 220d  ame__)} - {ex}".
+0001f7c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001f7d0: 2073 656c 662e 5f6c 6f67 2822 6572 726f   self._log("erro
+0001f7e0: 7222 2c20 6572 726f 725f 6d73 672c 2031  r", error_msg, 1
+0001f7f0: 290d 0a20 2020 2020 2020 2065 6c73 653a  )..        else:
+0001f800: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+0001f810: 2066 6c61 6773 2e65 7865 6375 7465 3a0d   flags.execute:.
+0001f820: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001f830: 2063 6c6f 7369 6e67 5f6d 7367 203d 2075   closing_msg = u
+0001f840: 6c2e 5f70 7072 696e 745f 6669 6c6c 5f68  l._pprint_fill_h
+0001f850: 6261 7228 227c 2066 696e 6973 6865 6420  bar("| finished 
+0001f860: 7079 7065 2069 7465 7261 7469 6f6e 207c  pype iteration |
+0001f870: 222c 2072 6574 3d54 7275 6529 0d0a 2020  ", ret=True)..  
+0001f880: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0001f890: 6c66 2e5f 6c6f 6728 2269 6e66 6f22 2c20  lf._log("info", 
+0001f8a0: 636c 6f73 696e 675f 6d73 672c 2030 290d  closing_msg, 0).
+0001f8b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0001f8c0: 2073 656c 662e 666c 6167 732e 7465 726d   self.flags.term
+0001f8d0: 696e 6174 6520 3d20 5472 7565 0d0a       inate = True..
```

### Comparing `phenopype-5.0.2/phenopype/tracking.py` & `phenopype-5.0.3/phenopype/tracking.py`

 * *Files identical despite different names*

### Comparing `phenopype-5.0.2/phenopype/utils.py` & `phenopype-5.0.3/phenopype/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,16 +58,21 @@
                 if flags.mode == "unchanged":
                     image = cv2.imread(path, cv2.IMREAD_UNCHANGED)
                 elif flags.mode == "colour":
                     image = cv2.imread(path, cv2.IMREAD_COLOR)
                 elif flags.mode == "gray":
                     image = cv2.imread(path, cv2.IMREAD_GRAYSCALE)
                 elif flags.mode == "rgb":
-                    image = cv2.imread(path)
-                    image = cv2.cvtColor(image, cv2.COLOR_BGR2RGB)
+                    image = cv2.imread(path, cv2.IMREAD_UNCHANGED)
+                    if image.shape[2] == 4:
+                        b, g, r, a = cv2.split(image)
+                        image = cv2.merge((r, g, b, a))
+                    else:
+                        b, g, r = cv2.split(image)
+                        image = cv2.merge((r, g, b))
             else:
                 ul._print(
                     'Invalid file extension "{}" - could not load image:\n'.format(ext)
                 )
                 return
         elif os.path.isdir(path):
             image = ul._load_project_image_directory(
```

### Comparing `phenopype-5.0.2/phenopype/utils_lowlevel.py` & `phenopype-5.0.3/phenopype/utils_lowlevel.py`

 * *Files 0% similar despite different names*

```diff
@@ -348,16 +348,16 @@
             core.export.save_canvas(
                 self.canvas,
                 dir_path=self.dir_path,
                 **kwargs_function,
             )
         if fun == "save_ROI":
             if not "file_name" in kwargs_function:
-                ext = kwargs_function.get("ext", ".jpg")
-                kwargs_function["file_name"] = self._construct_file_name("roi", ext)
+                kwargs_function["file_name"] = self._construct_file_name(
+                    self.image_name, "png")
             if not "dir_path" in kwargs_function:
                 kwargs_function["dir_path"] = os.path.join(self.dir_path, "ROI")
                 if not os.path.isdir(kwargs_function["dir_path"]):
                     os.makedirs(kwargs_function["dir_path"])
             core.export.save_ROI(
                 self.image_copy,
                 **kwargs_function,
@@ -573,17 +573,14 @@
         self._initialize_settings(tool, interactive, kwargs)
         
         ## initialize canvas (load previous zoom, mount, etc.)
         self._initialize_canvas()     
         
         ## prepare GUI for the evebtual use of certain tools (comment and drawing)
         self._prepare_tools(kwargs)
-        
-
-
 
         ## RUN: load tools and allow for user input
         if self.settings.interactive:
 
             cv2.namedWindow(
                 self.settings.window_name, _vars.opencv_window_flags[self.settings.window_aspect]
             )
@@ -842,36 +839,40 @@
                 self.settings.label_size,
                 self.settings.label_colour,
                 self.settings.label_width,
                 cv2.LINE_AA,
             )
 
         if self.tool == "draw":
+            self.settings.line_width_draw = copy.deepcopy(self.settings.line_width)
             if len(self.data[_vars._contour_type]) > 0:
+                ## draw contours if they're there
                 if len(self.image.shape) == 2:
                     self.image = cv2.cvtColor(self.image, cv2.COLOR_GRAY2BGR)
                 self.image_bin = np.zeros(self.image.shape[0:2], dtype=np.uint8)
                 self.image_bin_copy = copy.deepcopy(self.image_bin)
                 for contour in self.data[_vars._contour_type]:
                     cv2.drawContours(
                         image=self.image_bin,
                         contours=[contour],
                         contourIdx=0,
                         thickness=-1,
                         color=255,
                         maxLevel=3,
                         offset=(0, 0),
                     )
+                ## initial pass
+                self._canvas_renew()
                 self._canvas_draw(
-                    tool="line_bin", 
-                    coord_list=self.data[_vars._sequence_type],
+                    tool="line_bin", coord_list=self.data[_vars._sequence_type]
                 )
                 self._canvas_blend()
                 self._canvas_draw_contours()
-                    
+                self._canvas_mount()
+                
             else:
                 print("Could not find contours to edit - check annotations.")
                 return
             
         if self.tool in ["rectangle", "polygon", "polyline", "draw"]:
             self._canvas_draw(
                 tool="line", 
@@ -1317,15 +1318,15 @@
         if event == cv2.EVENT_LBUTTONUP or event == cv2.EVENT_RBUTTONUP:
             self.flags.drawing = False
             self.canvas = copy.deepcopy(self.canvas_copy)
             self.data[_vars._sequence_type].append(
                 [
                     self.data[_vars._coord_type],
                     self.colour_current_bin,
-                    int(self.settings.line_width * self.zoom.global_fx),
+                    int(self.settings.line_width_draw * self.zoom.global_fx),
                 ]
             )
             self.data[_vars._coord_type] = []
 
             ## draw all segments
             self._canvas_renew()
             self._canvas_draw(
@@ -1346,39 +1347,39 @@
 
             ## draw onto canvas for immediate feedback
             cv2.line(
                 self.canvas,
                 (self.ix, self.iy),
                 (x, y),
                 self.colour_current,
-                self.settings.line_width,
+                self.settings.line_width_draw,
             )
             self.ix, self.iy = x, y
             cv2.imshow(self.settings.window_name, self.canvas)
 
         if self.keypress == 9 and event == cv2.EVENT_MOUSEWHEEL:
             if flags > 1:
                 self.line_width_orig += 1
             if flags < 1 and self.line_width_orig > 1:
                 self.line_width_orig -= 1
 
             self.canvas = copy.deepcopy(self.canvas_copy)
-            self.settings.line_width = int(
+            self.settings.line_width_draw = int(
                 self.line_width_orig
                 / ((self.zoom.x2 - self.zoom.x1) / self.image_width)
             )
             cv2.line(
-                self.canvas, (x, y), (x, y), _get_bgr("black"), self.settings.line_width
+                self.canvas, (x, y), (x, y), _get_bgr("black"), self.settings.line_width_draw
             )
             cv2.line(
                 self.canvas,
                 (x, y),
                 (x, y),
                 _get_bgr("white"),
-                max(self.settings.line_width - 5, 1),
+                max(self.settings.line_width_draw - 5, 1),
             )
             cv2.imshow(self.settings.window_name, self.canvas)
 
     def _canvas_blend(self):
 
         ## create coloured overlay from binary image
         self.colour_mask = copy.deepcopy(self.image_bin_copy)
@@ -1544,15 +1545,15 @@
         )
 
         ## update canvas
         self._canvas_mount(refresh=False)
 
         ## adjust brush size
         if self.tool == "draw":
-            self.settings.line_width = int(
+            self.settings.line_width_draw = int(
                 self.line_width_orig
                 / ((self.zoom.x2 - self.zoom.x1) / self.image_width)
             )
             
         ## redraw input
         if self.tool in ["comment", "labelling"]:
             y_pos, x_pos = self.settings.label_position
```

### Comparing `phenopype-5.0.2/phenopype.egg-info/PKG-INFO` & `phenopype-5.0.3/phenopype.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phenopype
-Version: 5.0.2
+Version: 5.0.3
 Summary: A phenotyping pipeline for python
 Author-email: Moritz Luerig <moritz.luerig@gmail.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `phenopype-5.0.2/phenopype.egg-info/SOURCES.txt` & `phenopype-5.0.3/phenopype.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
-_temp/docs/conf.py
 _temp/tests/phenopype-tutorials-main/conf.py
 docs_source/conf.py
 phenopype/__init__.py
 phenopype/_vars.py
 phenopype/_version.py
 phenopype/config.py
 phenopype/decorators.py
```

### Comparing `phenopype-5.0.2/pyproject.toml` & `phenopype-5.0.3/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 00000010: 7265 7175 6972 6573 203d 205b 2273 6574  requires = ["set
 00000020: 7570 746f 6f6c 7322 5d0d 0a62 7569 6c64  uptools"]..build
 00000030: 2d62 6163 6b65 6e64 203d 2022 7365 7475  -backend = "setu
 00000040: 7074 6f6f 6c73 2e62 7569 6c64 5f6d 6574  ptools.build_met
 00000050: 6122 0d0a 0d0a 5b70 726f 6a65 6374 5d0d  a"....[project].
 00000060: 0a6e 616d 6520 3d20 2270 6865 6e6f 7079  .name = "phenopy
 00000070: 7065 220d 0a76 6572 7369 6f6e 203d 2022  pe"..version = "
-00000080: 352e 302e 3222 2020 0d0a 6465 7363 7269  5.0.2"  ..descri
+00000080: 352e 302e 3322 2020 0d0a 6465 7363 7269  5.0.3"  ..descri
 00000090: 7074 696f 6e20 3d20 2241 2070 6865 6e6f  ption = "A pheno
 000000a0: 7479 7069 6e67 2070 6970 656c 696e 6520  typing pipeline 
 000000b0: 666f 7220 7079 7468 6f6e 220d 0a72 6561  for python"..rea
 000000c0: 646d 6520 3d20 2252 4541 444d 452e 6d64  dme = "README.md
 000000d0: 220d 0a61 7574 686f 7273 203d 205b 0d0a  "..authors = [..
 000000e0: 2020 2020 7b6e 616d 6520 3d20 224d 6f72      {name = "Mor
 000000f0: 6974 7a20 4c75 6572 6967 222c 2065 6d61  itz Luerig", ema
```

### Comparing `phenopype-5.0.2/tests/conftest.py` & `phenopype-5.0.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `phenopype-5.0.2/tests/test_01_project.py` & `phenopype-5.0.3/tests/test_01_project.py`

 * *Files identical despite different names*

### Comparing `phenopype-5.0.2/tests/test_02_core_preprocessing.py` & `phenopype-5.0.3/tests/test_02_core_preprocessing.py`

 * *Files identical despite different names*

### Comparing `phenopype-5.0.2/tests/test_03_core_segmentation.py` & `phenopype-5.0.3/tests/test_03_core_segmentation.py`

 * *Files identical despite different names*

### Comparing `phenopype-5.0.2/tests/test_04_core_measurement.py` & `phenopype-5.0.3/tests/test_04_core_measurement.py`

 * *Files identical despite different names*

### Comparing `phenopype-5.0.2/tests/test_05_core_visualization.py` & `phenopype-5.0.3/tests/test_05_core_visualization.py`

 * *Files identical despite different names*

### Comparing `phenopype-5.0.2/tests/test_06_core_export.py` & `phenopype-5.0.3/tests/test_06_core_export.py`

 * *Files identical despite different names*

### Comparing `phenopype-5.0.2/tests/test_07_pype.py` & `phenopype-5.0.3/tests/test_07_pype.py`

 * *Files identical despite different names*

### Comparing `phenopype-5.0.2/tests/test_08_tracking.py` & `phenopype-5.0.3/tests/test_08_tracking.py`

 * *Files identical despite different names*

### Comparing `phenopype-5.0.2/tests/test_09_utils.py` & `phenopype-5.0.3/tests/test_09_utils.py`

 * *Files identical despite different names*

