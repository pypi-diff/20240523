# Comparing `tmp/torch_model_manager-0.4.1.dev1.tar.gz` & `tmp/torch_model_manager-0.4.1.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_model_manager-0.4.1.dev1.tar", last modified: Thu May 23 12:37:15 2024, max compression
+gzip compressed data, was "torch_model_manager-0.4.1.dev2.tar", last modified: Thu May 23 12:41:00 2024, max compression
```

## Comparing `torch_model_manager-0.4.1.dev1.tar` & `torch_model_manager-0.4.1.dev2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-23 12:37:15.538599 torch_model_manager-0.4.1.dev1/
--rw-r--r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     9197 2024-05-23 12:37:15.538599 torch_model_manager-0.4.1.dev1/PKG-INFO
--rwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)     8105 2024-05-13 08:52:52.000000 torch_model_manager-0.4.1.dev1/README.md
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)       38 2024-05-23 12:37:15.538599 torch_model_manager-0.4.1.dev1/setup.cfg
--rwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)     2219 2024-05-23 12:37:13.000000 torch_model_manager-0.4.1.dev1/setup.py
-drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-23 12:37:15.534599 torch_model_manager-0.4.1.dev1/tests/
-drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-23 12:37:15.534599 torch_model_manager-0.4.1.dev1/tests/test_torch_model_manager/
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-13 08:52:52.000000 torch_model_manager-0.4.1.dev1/tests/test_torch_model_manager/__init__.py
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     2462 2024-05-13 08:52:52.000000 torch_model_manager-0.4.1.dev1/tests/test_torch_model_manager/test_torch_model_manager.py
-drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-23 12:37:15.534599 torch_model_manager-0.4.1.dev1/tests/test_utils/
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-13 08:52:52.000000 torch_model_manager-0.4.1.dev1/tests/test_utils/__init__.py
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     3018 2024-05-13 08:52:52.000000 torch_model_manager-0.4.1.dev1/tests/test_utils/test_helpers.py
-drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-23 12:37:15.538599 torch_model_manager-0.4.1.dev1/torch_model_manager/
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)      148 2024-05-22 10:34:37.000000 torch_model_manager-0.4.1.dev1/torch_model_manager/__init__.py
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)    32763 2024-05-23 09:59:17.000000 torch_model_manager-0.4.1.dev1/torch_model_manager/neptune_manager.py
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     1774 2024-05-13 09:13:42.000000 torch_model_manager-0.4.1.dev1/torch_model_manager/notebook_manager.py
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)    20684 2024-05-23 12:34:10.000000 torch_model_manager-0.4.1.dev1/torch_model_manager/segmentation_manager.py
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)    18831 2024-05-13 08:53:31.000000 torch_model_manager-0.4.1.dev1/torch_model_manager/torch_model_manager.py
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     2442 2024-05-13 08:53:31.000000 torch_model_manager-0.4.1.dev1/torch_model_manager/wandb_manager.py
-drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-23 12:37:15.538599 torch_model_manager-0.4.1.dev1/torch_model_manager.egg-info/
--rw-r--r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     9197 2024-05-23 12:37:15.000000 torch_model_manager-0.4.1.dev1/torch_model_manager.egg-info/PKG-INFO
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)      666 2024-05-23 12:37:15.000000 torch_model_manager-0.4.1.dev1/torch_model_manager.egg-info/SOURCES.txt
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)        1 2024-05-23 12:37:15.000000 torch_model_manager-0.4.1.dev1/torch_model_manager.egg-info/dependency_links.txt
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)      228 2024-05-23 12:37:15.000000 torch_model_manager-0.4.1.dev1/torch_model_manager.egg-info/requires.txt
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)       32 2024-05-23 12:37:15.000000 torch_model_manager-0.4.1.dev1/torch_model_manager.egg-info/top_level.txt
-drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-23 12:37:15.538599 torch_model_manager-0.4.1.dev1/utils/
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-13 08:52:52.000000 torch_model_manager-0.4.1.dev1/utils/__init__.py
--rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     9031 2024-05-22 10:54:34.000000 torch_model_manager-0.4.1.dev1/utils/helpers.py
+drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-23 12:41:00.001941 torch_model_manager-0.4.1.dev2/
+-rw-r--r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     9197 2024-05-23 12:41:00.001941 torch_model_manager-0.4.1.dev2/PKG-INFO
+-rwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)     8105 2024-05-13 08:52:52.000000 torch_model_manager-0.4.1.dev2/README.md
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)       38 2024-05-23 12:41:00.001941 torch_model_manager-0.4.1.dev2/setup.cfg
+-rwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)     2219 2024-05-23 12:40:57.000000 torch_model_manager-0.4.1.dev2/setup.py
+drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-23 12:40:59.993941 torch_model_manager-0.4.1.dev2/tests/
+drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-23 12:40:59.993941 torch_model_manager-0.4.1.dev2/tests/test_torch_model_manager/
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-13 08:52:52.000000 torch_model_manager-0.4.1.dev2/tests/test_torch_model_manager/__init__.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     2462 2024-05-13 08:52:52.000000 torch_model_manager-0.4.1.dev2/tests/test_torch_model_manager/test_torch_model_manager.py
+drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-23 12:40:59.997941 torch_model_manager-0.4.1.dev2/tests/test_utils/
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-13 08:52:52.000000 torch_model_manager-0.4.1.dev2/tests/test_utils/__init__.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     3018 2024-05-13 08:52:52.000000 torch_model_manager-0.4.1.dev2/tests/test_utils/test_helpers.py
+drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-23 12:40:59.997941 torch_model_manager-0.4.1.dev2/torch_model_manager/
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)      148 2024-05-22 10:34:37.000000 torch_model_manager-0.4.1.dev2/torch_model_manager/__init__.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)    32763 2024-05-23 09:59:17.000000 torch_model_manager-0.4.1.dev2/torch_model_manager/neptune_manager.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     1774 2024-05-13 09:13:42.000000 torch_model_manager-0.4.1.dev2/torch_model_manager/notebook_manager.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)    20547 2024-05-23 12:40:46.000000 torch_model_manager-0.4.1.dev2/torch_model_manager/segmentation_manager.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)    18831 2024-05-13 08:53:31.000000 torch_model_manager-0.4.1.dev2/torch_model_manager/torch_model_manager.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     2442 2024-05-13 08:53:31.000000 torch_model_manager-0.4.1.dev2/torch_model_manager/wandb_manager.py
+drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-23 12:41:00.001941 torch_model_manager-0.4.1.dev2/torch_model_manager.egg-info/
+-rw-r--r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     9197 2024-05-23 12:40:59.000000 torch_model_manager-0.4.1.dev2/torch_model_manager.egg-info/PKG-INFO
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)      666 2024-05-23 12:40:59.000000 torch_model_manager-0.4.1.dev2/torch_model_manager.egg-info/SOURCES.txt
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)        1 2024-05-23 12:40:59.000000 torch_model_manager-0.4.1.dev2/torch_model_manager.egg-info/dependency_links.txt
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)      228 2024-05-23 12:40:59.000000 torch_model_manager-0.4.1.dev2/torch_model_manager.egg-info/requires.txt
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)       32 2024-05-23 12:40:59.000000 torch_model_manager-0.4.1.dev2/torch_model_manager.egg-info/top_level.txt
+drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-23 12:41:00.001941 torch_model_manager-0.4.1.dev2/utils/
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-13 08:52:52.000000 torch_model_manager-0.4.1.dev2/utils/__init__.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     9031 2024-05-22 10:54:34.000000 torch_model_manager-0.4.1.dev2/utils/helpers.py
```

### Comparing `torch_model_manager-0.4.1.dev1/PKG-INFO` & `torch_model_manager-0.4.1.dev2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-model-manager
-Version: 0.4.1.dev1
+Version: 0.4.1.dev2
 Summary: A package for managing PyTorch models
 Home-page: https://github.com/Billal-MOKHTARI/torch-model-manager
 Author: Billal MOKHTARI
 Author-email: mokhtaribillal1@gmail.com
 Keywords: PyTorch,Deep Learning,Machine Learning,High Level Programming
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `torch_model_manager-0.4.1.dev1/README.md` & `torch_model_manager-0.4.1.dev2/README.md`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.1.dev1/setup.py` & `torch_model_manager-0.4.1.dev2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='torch-model-manager',
-    version='0.4.1.dev1',
+    version='0.4.1.dev2',
     description='A package for managing PyTorch models',
     author='Billal MOKHTARI',
     author_email='mokhtaribillal1@gmail.com',
     packages=find_packages(exclude=['tests', 
                                     'docs', 
                                     'build.sh', 
                                     'requirements.sh',
```

### Comparing `torch_model_manager-0.4.1.dev1/tests/test_torch_model_manager/test_torch_model_manager.py` & `torch_model_manager-0.4.1.dev2/tests/test_torch_model_manager/test_torch_model_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.1.dev1/tests/test_utils/test_helpers.py` & `torch_model_manager-0.4.1.dev2/tests/test_utils/test_helpers.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.1.dev1/torch_model_manager/neptune_manager.py` & `torch_model_manager-0.4.1.dev2/torch_model_manager/neptune_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.1.dev1/torch_model_manager/notebook_manager.py` & `torch_model_manager-0.4.1.dev2/torch_model_manager/notebook_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.1.dev1/torch_model_manager/segmentation_manager.py` & `torch_model_manager-0.4.1.dev2/torch_model_manager/segmentation_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,25 +75,24 @@
         Returns:
         - np.ndarray: Occurrence probability disjoint matrix with shape (num_classes, num_classes).
         """
         dataset_path = kwargs.get("dataset_path", None)
         classes = kwargs.get("classes", None)
         box_threshold = kwargs.get("box_threshold", 0.25)
         text_threshold = kwargs.get("text_threshold", 0.25)
-        nms_threshold = kwargs.get("nms_threshold", 0.8)
+
         agg = kwargs.get("agg", hmean)
         annotation_matrix_processing = kwargs.get("annotation_matrix_processing", None)
         annotation_matrix_processing_args = kwargs.get("annotation_matrix_processing_args", {})
         if apply_on_annotation_matrix:
             assert matrix is None, "Annotation matrix should not be provided."
             matrix = self.create_annotation_matrix(dataset_path=dataset_path, 
                                                    classes=classes, 
                                                    box_threshold=box_threshold, 
                                                    text_threshold=text_threshold,
-                                                   nms_threshold=nms_threshold, 
                                                    agg=agg,
                                                    run=run,
                                                    output_namespaces=output_namespaces)
         if annotation_matrix_processing is not None:
             matrix = annotation_matrix_processing(matrix, **annotation_matrix_processing_args)
 
         classes = matrix.columns
```

### Comparing `torch_model_manager-0.4.1.dev1/torch_model_manager/torch_model_manager.py` & `torch_model_manager-0.4.1.dev2/torch_model_manager/torch_model_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.1.dev1/torch_model_manager/wandb_manager.py` & `torch_model_manager-0.4.1.dev2/torch_model_manager/wandb_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.1.dev1/torch_model_manager.egg-info/PKG-INFO` & `torch_model_manager-0.4.1.dev2/torch_model_manager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-model-manager
-Version: 0.4.1.dev1
+Version: 0.4.1.dev2
 Summary: A package for managing PyTorch models
 Home-page: https://github.com/Billal-MOKHTARI/torch-model-manager
 Author: Billal MOKHTARI
 Author-email: mokhtaribillal1@gmail.com
 Keywords: PyTorch,Deep Learning,Machine Learning,High Level Programming
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `torch_model_manager-0.4.1.dev1/torch_model_manager.egg-info/SOURCES.txt` & `torch_model_manager-0.4.1.dev2/torch_model_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.4.1.dev1/utils/helpers.py` & `torch_model_manager-0.4.1.dev2/utils/helpers.py`

 * *Files identical despite different names*

