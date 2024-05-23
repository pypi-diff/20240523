# Comparing `tmp/torch_model_manager-0.4.0.dev8.tar.gz` & `tmp/torch_model_manager-0.4.0.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_model_manager-0.4.0.dev8.tar", last modified: Wed May 22 13:29:51 2024, max compression
+gzip compressed data, was "torch_model_manager-0.4.0.dev9.tar", last modified: Thu May 23 07:07:21 2024, max compression
```

## Comparing `torch_model_manager-0.4.0.dev8.tar` & `torch_model_manager-0.4.0.dev9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-22 13:29:51.728508 torch_model_manager-0.4.0.dev8/
--rw-r--r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     9197 2024-05-22 13:29:51.728508 torch_model_manager-0.4.0.dev8/PKG-INFO
--rwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)     8105 2024-05-13 08:52:52.000000 torch_model_manager-0.4.0.dev8/README.md
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)       38 2024-05-22 13:29:51.728508 torch_model_manager-0.4.0.dev8/setup.cfg
--rwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)     2219 2024-05-22 13:29:49.000000 torch_model_manager-0.4.0.dev8/setup.py
-drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-22 13:29:51.724508 torch_model_manager-0.4.0.dev8/tests/
-drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-22 13:29:51.724508 torch_model_manager-0.4.0.dev8/tests/test_torch_model_manager/
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-13 08:52:52.000000 torch_model_manager-0.4.0.dev8/tests/test_torch_model_manager/__init__.py
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     2462 2024-05-13 08:52:52.000000 torch_model_manager-0.4.0.dev8/tests/test_torch_model_manager/test_torch_model_manager.py
-drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-22 13:29:51.724508 torch_model_manager-0.4.0.dev8/tests/test_utils/
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-13 08:52:52.000000 torch_model_manager-0.4.0.dev8/tests/test_utils/__init__.py
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     3018 2024-05-13 08:52:52.000000 torch_model_manager-0.4.0.dev8/tests/test_utils/test_helpers.py
-drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-22 13:29:51.728508 torch_model_manager-0.4.0.dev8/torch_model_manager/
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)      148 2024-05-22 10:34:37.000000 torch_model_manager-0.4.0.dev8/torch_model_manager/__init__.py
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)    32749 2024-05-17 13:07:00.000000 torch_model_manager-0.4.0.dev8/torch_model_manager/neptune_manager.py
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     1774 2024-05-13 09:13:42.000000 torch_model_manager-0.4.0.dev8/torch_model_manager/notebook_manager.py
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)    14036 2024-05-22 13:29:32.000000 torch_model_manager-0.4.0.dev8/torch_model_manager/segmentation_manager.py
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)    18831 2024-05-13 08:53:31.000000 torch_model_manager-0.4.0.dev8/torch_model_manager/torch_model_manager.py
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     2442 2024-05-13 08:53:31.000000 torch_model_manager-0.4.0.dev8/torch_model_manager/wandb_manager.py
-drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-22 13:29:51.728508 torch_model_manager-0.4.0.dev8/torch_model_manager.egg-info/
--rw-r--r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     9197 2024-05-22 13:29:51.000000 torch_model_manager-0.4.0.dev8/torch_model_manager.egg-info/PKG-INFO
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)      666 2024-05-22 13:29:51.000000 torch_model_manager-0.4.0.dev8/torch_model_manager.egg-info/SOURCES.txt
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)        1 2024-05-22 13:29:51.000000 torch_model_manager-0.4.0.dev8/torch_model_manager.egg-info/dependency_links.txt
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)      228 2024-05-22 13:29:51.000000 torch_model_manager-0.4.0.dev8/torch_model_manager.egg-info/requires.txt
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)       32 2024-05-22 13:29:51.000000 torch_model_manager-0.4.0.dev8/torch_model_manager.egg-info/top_level.txt
-drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-22 13:29:51.728508 torch_model_manager-0.4.0.dev8/utils/
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-13 08:52:52.000000 torch_model_manager-0.4.0.dev8/utils/__init__.py
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     9031 2024-05-22 10:54:34.000000 torch_model_manager-0.4.0.dev8/utils/helpers.py
+drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-23 07:07:21.106859 torch_model_manager-0.4.0.dev9/
+-rw-r--r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     9197 2024-05-23 07:07:21.106859 torch_model_manager-0.4.0.dev9/PKG-INFO
+-rwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)     8105 2024-05-13 08:52:52.000000 torch_model_manager-0.4.0.dev9/README.md
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)       38 2024-05-23 07:07:21.106859 torch_model_manager-0.4.0.dev9/setup.cfg
+-rwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)     2219 2024-05-23 07:07:19.000000 torch_model_manager-0.4.0.dev9/setup.py
+drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-23 07:07:21.098859 torch_model_manager-0.4.0.dev9/tests/
+drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-23 07:07:21.102859 torch_model_manager-0.4.0.dev9/tests/test_torch_model_manager/
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-13 08:52:52.000000 torch_model_manager-0.4.0.dev9/tests/test_torch_model_manager/__init__.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     2462 2024-05-13 08:52:52.000000 torch_model_manager-0.4.0.dev9/tests/test_torch_model_manager/test_torch_model_manager.py
+drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-23 07:07:21.102859 torch_model_manager-0.4.0.dev9/tests/test_utils/
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-13 08:52:52.000000 torch_model_manager-0.4.0.dev9/tests/test_utils/__init__.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     3018 2024-05-13 08:52:52.000000 torch_model_manager-0.4.0.dev9/tests/test_utils/test_helpers.py
+drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-23 07:07:21.102859 torch_model_manager-0.4.0.dev9/torch_model_manager/
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)      148 2024-05-22 10:34:37.000000 torch_model_manager-0.4.0.dev9/torch_model_manager/__init__.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)    32749 2024-05-17 13:07:00.000000 torch_model_manager-0.4.0.dev9/torch_model_manager/neptune_manager.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     1774 2024-05-13 09:13:42.000000 torch_model_manager-0.4.0.dev9/torch_model_manager/notebook_manager.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)    14009 2024-05-23 07:06:52.000000 torch_model_manager-0.4.0.dev9/torch_model_manager/segmentation_manager.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)    18831 2024-05-13 08:53:31.000000 torch_model_manager-0.4.0.dev9/torch_model_manager/torch_model_manager.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     2442 2024-05-13 08:53:31.000000 torch_model_manager-0.4.0.dev9/torch_model_manager/wandb_manager.py
+drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-23 07:07:21.106859 torch_model_manager-0.4.0.dev9/torch_model_manager.egg-info/
+-rw-r--r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     9197 2024-05-23 07:07:21.000000 torch_model_manager-0.4.0.dev9/torch_model_manager.egg-info/PKG-INFO
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)      666 2024-05-23 07:07:21.000000 torch_model_manager-0.4.0.dev9/torch_model_manager.egg-info/SOURCES.txt
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)        1 2024-05-23 07:07:21.000000 torch_model_manager-0.4.0.dev9/torch_model_manager.egg-info/dependency_links.txt
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)      228 2024-05-23 07:07:21.000000 torch_model_manager-0.4.0.dev9/torch_model_manager.egg-info/requires.txt
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)       32 2024-05-23 07:07:21.000000 torch_model_manager-0.4.0.dev9/torch_model_manager.egg-info/top_level.txt
+drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-23 07:07:21.106859 torch_model_manager-0.4.0.dev9/utils/
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-13 08:52:52.000000 torch_model_manager-0.4.0.dev9/utils/__init__.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     9031 2024-05-22 10:54:34.000000 torch_model_manager-0.4.0.dev9/utils/helpers.py
```

### Comparing `torch_model_manager-0.4.0.dev8/PKG-INFO` & `torch_model_manager-0.4.0.dev9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-model-manager
-Version: 0.4.0.dev8
+Version: 0.4.0.dev9
 Summary: A package for managing PyTorch models
 Home-page: https://github.com/Billal-MOKHTARI/torch-model-manager
 Author: Billal MOKHTARI
 Author-email: mokhtaribillal1@gmail.com
 Keywords: PyTorch,Deep Learning,Machine Learning,High Level Programming
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `torch_model_manager-0.4.0.dev8/README.md` & `torch_model_manager-0.4.0.dev9/README.md`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.0.dev8/setup.py` & `torch_model_manager-0.4.0.dev9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='torch-model-manager',
-    version='0.4.0.dev8',
+    version='0.4.0.dev9',
     description='A package for managing PyTorch models',
     author='Billal MOKHTARI',
     author_email='mokhtaribillal1@gmail.com',
     packages=find_packages(exclude=['tests', 
                                     'docs', 
                                     'build.sh', 
                                     'requirements.sh',
```

### Comparing `torch_model_manager-0.4.0.dev8/tests/test_torch_model_manager/test_torch_model_manager.py` & `torch_model_manager-0.4.0.dev9/tests/test_torch_model_manager/test_torch_model_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.0.dev8/tests/test_utils/test_helpers.py` & `torch_model_manager-0.4.0.dev9/tests/test_utils/test_helpers.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.0.dev8/torch_model_manager/neptune_manager.py` & `torch_model_manager-0.4.0.dev9/torch_model_manager/neptune_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.0.dev8/torch_model_manager/notebook_manager.py` & `torch_model_manager-0.4.0.dev9/torch_model_manager/notebook_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.0.dev8/torch_model_manager/segmentation_manager.py` & `torch_model_manager-0.4.0.dev9/torch_model_manager/segmentation_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -195,20 +195,20 @@
 
     def grounding_sam(self, source_image_path, classes, box_threshold=0.25, text_threshold=0.25, nms_threshold=0.8, output_path=None):
         # Load image
         image = self.load_image(source_image_path)
 
         # Detect objects
         detections = self.detect_objects(image, classes, box_threshold, text_threshold)
-
         # Apply NMS
         detections = self.nms(detections, nms_threshold)
 
         # Convert detections to masks
         detections.mask = self.segment(cv2.cvtColor(image, cv2.COLOR_BGR2RGB), detections.xyxy)
+  
 
         # Annotate image with segmented masks
         annotated_image = self.annotate_image(image, detections, classes)
 
         if output_path is not None:
             self.save_image(annotated_image, output_path)
 
@@ -255,15 +255,14 @@
         annotation_matrix = pd.DataFrame(data=np.zeros((len(image_ids), len(classes))), index=image_ids, columns=classes)
 
         for image_name in tqdm(image_ids, desc="Creating annotation matrix", unit="image"):
             image_path = os.path.join(dataset_path, image_name)
 
             # Apply the grounding SAM pipeline
             detections = self.grounding_sam(image_path, classes, box_threshold=box_threshold, text_threshold=text_threshold, nms_threshold=nms_threshold)
-
             # Calculate the harmonic mean of confidences
             confidences = detections.confidence
             class_ids = [classes[id] for id in detections.class_id]
             harmonic_means = self.aggregator(class_ids, confidences, agg=agg)
             annotation_matrix.loc[image_name, harmonic_means[:, 0]] = harmonic_means[:, 1]
 
         return annotation_matrix
@@ -312,15 +311,15 @@
 
         return tensor, matrix.index, classes
     
     
     def save_image(self, image, path):
         cv2.imwrite(path, image)
         
-# # Example usage
+# # # Example usage
 # if __name__ == "__main__":
 #     SOURCE_IMAGE_PATH = "G0041951.JPG"
 #     CLASSES = ["person", "banner", "finger", "hand", "foot", "glasses", "desert", "sky", "clouds"]
 #     BOX_THRESHOLD = 0.3
 #     TEXT_THRESHOLD = 0.25
 #     NMS_THRESHOLD = 0.3
 
@@ -334,8 +333,8 @@
 #     annotation_matrix = manager.occ_proba_disjoint_tensor(matrix = None, 
 #                                                           apply_on_annotation_matrix=True, 
 #                                                           dataset_path=dataset_path, 
 #                                                           classes=CLASSES, 
 #                                                           box_threshold=BOX_THRESHOLD, 
 #                                                           text_threshold=TEXT_THRESHOLD, 
 #                                                           nms_threshold=NMS_THRESHOLD)
-#     print(annotation_matrix)
+
```

### Comparing `torch_model_manager-0.4.0.dev8/torch_model_manager/torch_model_manager.py` & `torch_model_manager-0.4.0.dev9/torch_model_manager/torch_model_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.0.dev8/torch_model_manager/wandb_manager.py` & `torch_model_manager-0.4.0.dev9/torch_model_manager/wandb_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.0.dev8/torch_model_manager.egg-info/PKG-INFO` & `torch_model_manager-0.4.0.dev9/torch_model_manager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-model-manager
-Version: 0.4.0.dev8
+Version: 0.4.0.dev9
 Summary: A package for managing PyTorch models
 Home-page: https://github.com/Billal-MOKHTARI/torch-model-manager
 Author: Billal MOKHTARI
 Author-email: mokhtaribillal1@gmail.com
 Keywords: PyTorch,Deep Learning,Machine Learning,High Level Programming
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `torch_model_manager-0.4.0.dev8/torch_model_manager.egg-info/SOURCES.txt` & `torch_model_manager-0.4.0.dev9/torch_model_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.0.dev8/utils/helpers.py` & `torch_model_manager-0.4.0.dev9/utils/helpers.py`

 * *Files identical despite different names*

