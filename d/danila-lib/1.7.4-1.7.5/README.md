# Comparing `tmp/danila-lib-1.7.4.tar.gz` & `tmp/danila-lib-1.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "danila-lib-1.7.4.tar", last modified: Wed May 22 10:13:41 2024, max compression
+gzip compressed data, was "danila-lib-1.7.5.tar", last modified: Wed May 22 11:33:03 2024, max compression
```

## Comparing `danila-lib-1.7.4.tar` & `danila-lib-1.7.5.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 10:13:41.249476 danila-lib-1.7.4/
--rw-rw-rw-   0        0        0     9615 2024-05-22 10:13:41.249476 danila-lib-1.7.4/PKG-INFO
--rw-rw-rw-   0        0        0     5060 2024-04-22 21:01:41.000000 danila-lib-1.7.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-22 10:13:40.655427 danila-lib-1.7.4/danila/
--rw-rw-rw-   0        0        0        0 2024-04-15 11:55:56.000000 danila-lib-1.7.4/danila/__init__.py
--rw-rw-rw-   0        0        0     2123 2024-05-22 05:28:12.000000 danila-lib-1.7.4/danila/danila.py
--rw-rw-rw-   0        0        0     9764 2024-05-22 08:43:39.000000 danila-lib-1.7.4/danila/danila_v1.py
--rw-rw-rw-   0        0        0    10182 2024-05-22 08:43:39.000000 danila-lib-1.7.4/danila/danila_v2.py
--rw-rw-rw-   0        0        0    10706 2024-05-22 08:43:39.000000 danila-lib-1.7.4/danila/danila_v3.py
--rw-rw-rw-   0        0        0    15320 2024-05-22 09:25:07.000000 danila-lib-1.7.4/danila/danila_v4.py
-drwxrwxrwx   0        0        0        0 2024-05-22 10:13:40.686670 danila-lib-1.7.4/danila_lib.egg-info/
--rw-rw-rw-   0        0        0     9615 2024-05-22 10:13:40.000000 danila-lib-1.7.4/danila_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      940 2024-05-22 10:13:40.000000 danila-lib-1.7.4/danila_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 10:13:40.000000 danila-lib-1.7.4/danila_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     1879 2024-05-22 10:13:40.000000 danila-lib-1.7.4/danila_lib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-22 10:13:40.000000 danila-lib-1.7.4/danila_lib.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-22 10:13:40.686670 danila-lib-1.7.4/data/
--rw-rw-rw-   0        0        0        0 2024-04-15 12:01:57.000000 danila-lib-1.7.4/data/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 10:13:40.968291 danila-lib-1.7.4/data/neuro/
--rw-rw-rw-   0        0        0     5722 2024-04-22 21:09:12.000000 danila-lib-1.7.4/data/neuro/Letters_recognize.py
--rw-rw-rw-   0        0        0     2754 2024-04-22 10:33:16.000000 danila-lib-1.7.4/data/neuro/Rama_classify_class.py
--rw-rw-rw-   0        0        0     2121 2024-05-22 08:48:35.000000 danila-lib-1.7.4/data/neuro/Rama_detect_class.py
--rw-rw-rw-   0        0        0     2614 2024-05-14 12:37:43.000000 danila-lib-1.7.4/data/neuro/Rama_prod_classify_class.py
--rw-rw-rw-   0        0        0     3143 2024-05-22 08:49:48.000000 danila-lib-1.7.4/data/neuro/Text_detect_class.py
--rw-rw-rw-   0        0        0        0 2024-04-15 12:02:04.000000 danila-lib-1.7.4/data/neuro/__init__.py
--rw-rw-rw-   0        0        0     6373 2024-05-06 15:05:03.000000 danila-lib-1.7.4/data/neuro/letters_in_image.py
--rw-rw-rw-   0        0        0      654 2024-05-22 10:13:34.000000 danila-lib-1.7.4/data/neuro/models.py
--rw-rw-rw-   0        0        0     2975 2024-05-14 11:04:15.000000 danila-lib-1.7.4/data/neuro/objs_in_image.py
--rw-rw-rw-   0        0        0     4390 2024-05-22 07:22:08.000000 danila-lib-1.7.4/data/neuro/text_recognize_yolo.py
-drwxrwxrwx   0        0        0        0 2024-05-22 10:13:41.249476 danila-lib-1.7.4/data/result/
--rw-rw-rw-   0        0        0       89 2023-11-28 06:30:22.000000 danila-lib-1.7.4/data/result/Class_im.py
--rw-rw-rw-   0        0        0      108 2023-12-12 16:53:34.000000 danila-lib-1.7.4/data/result/Class_text.py
--rw-rw-rw-   0        0        0     2811 2024-04-22 19:35:07.000000 danila-lib-1.7.4/data/result/Image_text_areas.py
--rw-rw-rw-   0        0        0      311 2024-04-22 18:52:56.000000 danila-lib-1.7.4/data/result/Label_area.py
--rw-rw-rw-   0        0        0      105 2024-05-14 11:34:55.000000 danila-lib-1.7.4/data/result/Rama_prod.py
--rw-rw-rw-   0        0        0     3233 2024-04-22 18:17:45.000000 danila-lib-1.7.4/data/result/Rect.py
--rw-rw-rw-   0        0        0      539 2024-04-22 18:52:56.000000 danila-lib-1.7.4/data/result/Text_area.py
--rw-rw-rw-   0        0        0      716 2024-04-22 10:33:16.000000 danila-lib-1.7.4/data/result/Yolo_label_rect.py
--rw-rw-rw-   0        0        0        0 2024-04-15 12:02:04.000000 danila-lib-1.7.4/data/result/__init__.py
--rw-rw-rw-   0        0        0      126 2024-05-14 11:04:15.000000 danila-lib-1.7.4/data/result/prod_classify_result.py
--rw-rw-rw-   0        0        0      122 2024-05-06 08:55:07.000000 danila-lib-1.7.4/data/result/word_compare_result.py
--rw-rw-rw-   0        0        0       42 2024-05-22 10:13:41.249476 danila-lib-1.7.4/setup.cfg
--rw-rw-rw-   0        0        0      983 2024-05-22 10:13:34.000000 danila-lib-1.7.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 11:33:03.024945 danila-lib-1.7.5/
+-rw-rw-rw-   0        0        0     9615 2024-05-22 11:33:03.024945 danila-lib-1.7.5/PKG-INFO
+-rw-rw-rw-   0        0        0     5060 2024-04-22 21:01:41.000000 danila-lib-1.7.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-22 11:33:02.711780 danila-lib-1.7.5/danila/
+-rw-rw-rw-   0        0        0        0 2024-04-15 11:55:56.000000 danila-lib-1.7.5/danila/__init__.py
+-rw-rw-rw-   0        0        0     2123 2024-05-22 05:28:12.000000 danila-lib-1.7.5/danila/danila.py
+-rw-rw-rw-   0        0        0     9764 2024-05-22 08:43:39.000000 danila-lib-1.7.5/danila/danila_v1.py
+-rw-rw-rw-   0        0        0    10182 2024-05-22 08:43:39.000000 danila-lib-1.7.5/danila/danila_v2.py
+-rw-rw-rw-   0        0        0    10706 2024-05-22 08:43:39.000000 danila-lib-1.7.5/danila/danila_v3.py
+-rw-rw-rw-   0        0        0    15682 2024-05-22 11:32:57.000000 danila-lib-1.7.5/danila/danila_v4.py
+drwxrwxrwx   0        0        0        0 2024-05-22 11:33:02.743023 danila-lib-1.7.5/danila_lib.egg-info/
+-rw-rw-rw-   0        0        0     9615 2024-05-22 11:33:02.000000 danila-lib-1.7.5/danila_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      940 2024-05-22 11:33:02.000000 danila-lib-1.7.5/danila_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 11:33:02.000000 danila-lib-1.7.5/danila_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     1879 2024-05-22 11:33:02.000000 danila-lib-1.7.5/danila_lib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-22 11:33:02.000000 danila-lib-1.7.5/danila_lib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-22 11:33:02.743023 danila-lib-1.7.5/data/
+-rw-rw-rw-   0        0        0        0 2024-04-15 12:01:57.000000 danila-lib-1.7.5/data/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 11:33:02.836747 danila-lib-1.7.5/data/neuro/
+-rw-rw-rw-   0        0        0     5722 2024-04-22 21:09:12.000000 danila-lib-1.7.5/data/neuro/Letters_recognize.py
+-rw-rw-rw-   0        0        0     2754 2024-04-22 10:33:16.000000 danila-lib-1.7.5/data/neuro/Rama_classify_class.py
+-rw-rw-rw-   0        0        0     2121 2024-05-22 08:48:35.000000 danila-lib-1.7.5/data/neuro/Rama_detect_class.py
+-rw-rw-rw-   0        0        0     2614 2024-05-14 12:37:43.000000 danila-lib-1.7.5/data/neuro/Rama_prod_classify_class.py
+-rw-rw-rw-   0        0        0     3143 2024-05-22 08:49:48.000000 danila-lib-1.7.5/data/neuro/Text_detect_class.py
+-rw-rw-rw-   0        0        0        0 2024-04-15 12:02:04.000000 danila-lib-1.7.5/data/neuro/__init__.py
+-rw-rw-rw-   0        0        0     6373 2024-05-06 15:05:03.000000 danila-lib-1.7.5/data/neuro/letters_in_image.py
+-rw-rw-rw-   0        0        0      654 2024-05-22 10:13:34.000000 danila-lib-1.7.5/data/neuro/models.py
+-rw-rw-rw-   0        0        0     2975 2024-05-14 11:04:15.000000 danila-lib-1.7.5/data/neuro/objs_in_image.py
+-rw-rw-rw-   0        0        0     4390 2024-05-22 07:22:08.000000 danila-lib-1.7.5/data/neuro/text_recognize_yolo.py
+drwxrwxrwx   0        0        0        0 2024-05-22 11:33:03.024945 danila-lib-1.7.5/data/result/
+-rw-rw-rw-   0        0        0       89 2023-11-28 06:30:22.000000 danila-lib-1.7.5/data/result/Class_im.py
+-rw-rw-rw-   0        0        0      108 2023-12-12 16:53:34.000000 danila-lib-1.7.5/data/result/Class_text.py
+-rw-rw-rw-   0        0        0     2811 2024-04-22 19:35:07.000000 danila-lib-1.7.5/data/result/Image_text_areas.py
+-rw-rw-rw-   0        0        0      311 2024-04-22 18:52:56.000000 danila-lib-1.7.5/data/result/Label_area.py
+-rw-rw-rw-   0        0        0      105 2024-05-14 11:34:55.000000 danila-lib-1.7.5/data/result/Rama_prod.py
+-rw-rw-rw-   0        0        0     3233 2024-04-22 18:17:45.000000 danila-lib-1.7.5/data/result/Rect.py
+-rw-rw-rw-   0        0        0      539 2024-04-22 18:52:56.000000 danila-lib-1.7.5/data/result/Text_area.py
+-rw-rw-rw-   0        0        0      716 2024-04-22 10:33:16.000000 danila-lib-1.7.5/data/result/Yolo_label_rect.py
+-rw-rw-rw-   0        0        0        0 2024-04-15 12:02:04.000000 danila-lib-1.7.5/data/result/__init__.py
+-rw-rw-rw-   0        0        0      126 2024-05-14 11:04:15.000000 danila-lib-1.7.5/data/result/prod_classify_result.py
+-rw-rw-rw-   0        0        0      122 2024-05-06 08:55:07.000000 danila-lib-1.7.5/data/result/word_compare_result.py
+-rw-rw-rw-   0        0        0       42 2024-05-22 11:33:03.024945 danila-lib-1.7.5/setup.cfg
+-rw-rw-rw-   0        0        0      983 2024-05-22 11:32:57.000000 danila-lib-1.7.5/setup.py
```

### Comparing `danila-lib-1.7.4/PKG-INFO` & `danila-lib-1.7.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: danila-lib
-Version: 1.7.4
+Version: 1.7.5
 Summary: This is the module for detecting and classifying text on rama pictures
 Home-page: https://github.com/Arseniy-Zhuck/danila_lib
 Author: arseniy_zhuck
 Author-email: arseniyzhuck@mail.ru
 Project-URL: GitHub, https://github.com/Arseniy-Zhuck/danila_lib
 Keywords: rama detect machine-learning computer-vision
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `danila-lib-1.7.4/README.md` & `danila-lib-1.7.5/README.md`

 * *Files identical despite different names*

### Comparing `danila-lib-1.7.4/danila/danila.py` & `danila-lib-1.7.5/danila/danila.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.7.4/danila/danila_v1.py` & `danila-lib-1.7.5/danila/danila_v1.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.7.4/danila/danila_v2.py` & `danila-lib-1.7.5/danila/danila_v2.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.7.4/danila/danila_v3.py` & `danila-lib-1.7.5/danila/danila_v3.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.7.4/danila/danila_v4.py` & `danila-lib-1.7.5/danila/danila_v4.py`

 * *Files 2% similar despite different names*

```diff
@@ -207,15 +207,18 @@
                     label_area_max = self.text_recognize_ruzhimmash_model.work_image_cut(image_text_areas, img_cut, 5, 64, 128,
                                                                               4, 64, 128, 2, 64, 64)
                     if len(label_area_max.labels[Class_text.number]) == 5:
                         res_labels['number'] = label_area_max.labels[Class_text.number]
                     else:
                         res_labels['number'] = label_area.labels[Class_text.number]
             res_labels['prod'] = '1275'
-            res_labels['year'] = label_area.labels[Class_text.year]
+            if (len(label_area.labels[Class_text.year]) == 2) and (int(label_area.labels[Class_text.year]) < 25):
+                res_labels['year'] = label_area.labels[Class_text.year]
+            else:
+                res_labels['year'] = '23'
             return res_labels
         else:
             rect = self.rama_no_spring_detect_model.rama_detect(initial_image_path)
             if rect is None:
                 return {"result" : "no_rama"}
             img_cut = img[rect.ymin:rect.ymax, rect.xmin:rect.xmax]
             img_cut_path = 'cut_img.jpg'
@@ -251,9 +254,12 @@
                     label_area_max = self.text_recognize_begickaya_model.work_image_cut(image_text_areas, img_cut, 5, 64, 128,
                                                                               4, 64, 128, 2, 64, 64)
                     if len(label_area_max.labels[Class_text.number]) == 6:
                         res_labels['number'] = label_area_max.labels[Class_text.number]
                     else:
                         res_labels['number'] = label_area.labels[Class_text.number]
             res_labels['prod'] = '12'
-            res_labels['year'] = label_area.labels[Class_text.year]
+            if (len(label_area.labels[Class_text.year]) == 2) and (int(label_area.labels[Class_text.year]) < 25):
+                res_labels['year'] = label_area.labels[Class_text.year]
+            else:
+                res_labels['year'] = '23'
             return res_labels
```

### Comparing `danila-lib-1.7.4/danila_lib.egg-info/PKG-INFO` & `danila-lib-1.7.5/danila_lib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: danila-lib
-Version: 1.7.4
+Version: 1.7.5
 Summary: This is the module for detecting and classifying text on rama pictures
 Home-page: https://github.com/Arseniy-Zhuck/danila_lib
 Author: arseniy_zhuck
 Author-email: arseniyzhuck@mail.ru
 Project-URL: GitHub, https://github.com/Arseniy-Zhuck/danila_lib
 Keywords: rama detect machine-learning computer-vision
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `danila-lib-1.7.4/danila_lib.egg-info/SOURCES.txt` & `danila-lib-1.7.5/danila_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `danila-lib-1.7.4/danila_lib.egg-info/requires.txt` & `danila-lib-1.7.5/danila_lib.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `danila-lib-1.7.4/data/neuro/Letters_recognize.py` & `danila-lib-1.7.5/data/neuro/Letters_recognize.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.7.4/data/neuro/Rama_classify_class.py` & `danila-lib-1.7.5/data/neuro/Rama_classify_class.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.7.4/data/neuro/Rama_detect_class.py` & `danila-lib-1.7.5/data/neuro/Rama_detect_class.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.7.4/data/neuro/Rama_prod_classify_class.py` & `danila-lib-1.7.5/data/neuro/Rama_prod_classify_class.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.7.4/data/neuro/Text_detect_class.py` & `danila-lib-1.7.5/data/neuro/Text_detect_class.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.7.4/data/neuro/letters_in_image.py` & `danila-lib-1.7.5/data/neuro/letters_in_image.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.7.4/data/neuro/models.py` & `danila-lib-1.7.5/data/neuro/models.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.7.4/data/neuro/objs_in_image.py` & `danila-lib-1.7.5/data/neuro/objs_in_image.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.7.4/data/neuro/text_recognize_yolo.py` & `danila-lib-1.7.5/data/neuro/text_recognize_yolo.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.7.4/data/result/Image_text_areas.py` & `danila-lib-1.7.5/data/result/Image_text_areas.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.7.4/data/result/Rect.py` & `danila-lib-1.7.5/data/result/Rect.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.7.4/data/result/Text_area.py` & `danila-lib-1.7.5/data/result/Text_area.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.7.4/data/result/Yolo_label_rect.py` & `danila-lib-1.7.5/data/result/Yolo_label_rect.py`

 * *Files identical despite different names*

### Comparing `danila-lib-1.7.4/setup.py` & `danila-lib-1.7.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
   with open('requirements.txt', 'r') as f:
     a = f.read()
   b = a.split()
   return b
 
 setup(
   name='danila-lib',
-  version='1.7.4',
+  version='1.7.5',
   author='arseniy_zhuck',
   author_email='arseniyzhuck@mail.ru',
   description='This is the module for detecting and classifying text on rama pictures',
   long_description=readme(),
   long_description_content_type='text/markdown',
   url='https://github.com/Arseniy-Zhuck/danila_lib',
   packages=find_packages(),
```

