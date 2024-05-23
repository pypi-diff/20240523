# Comparing `tmp/neuroweave-0.0.4.tar.gz` & `tmp/neuroweave-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuroweave-0.0.4.tar", last modified: Thu May 23 17:56:50 2024, max compression
+gzip compressed data, was "neuroweave-0.0.5.tar", last modified: Thu May 23 18:07:11 2024, max compression
```

## Comparing `neuroweave-0.0.4.tar` & `neuroweave-0.0.5.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 17:56:50.159268 neuroweave-0.0.4/
--rw-rw-rw-   0        0        0     1088 2024-04-25 14:13:00.000000 neuroweave-0.0.4/LICENSE
--rw-rw-rw-   0        0        0     5677 2024-05-23 17:56:50.157159 neuroweave-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     4339 2024-05-23 11:36:09.000000 neuroweave-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-23 17:56:50.155090 neuroweave-0.0.4/neuroweave.egg-info/
--rw-rw-rw-   0        0        0     5677 2024-05-23 17:56:50.000000 neuroweave-0.0.4/neuroweave.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      824 2024-05-23 17:56:50.000000 neuroweave-0.0.4/neuroweave.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 17:56:50.000000 neuroweave-0.0.4/neuroweave.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      173 2024-05-23 17:56:50.000000 neuroweave-0.0.4/neuroweave.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-05-23 17:56:50.000000 neuroweave-0.0.4/neuroweave.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-23 17:56:50.159268 neuroweave-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1785 2024-05-23 17:55:58.000000 neuroweave-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-23 17:56:50.126992 neuroweave-0.0.4/weave/
--rw-rw-rw-   0        0        0      896 2024-05-23 11:36:09.000000 neuroweave-0.0.4/weave/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 17:56:50.129107 neuroweave-0.0.4/weave/_utils/
--rw-rw-rw-   0        0        0       42 2024-05-23 06:31:49.000000 neuroweave-0.0.4/weave/_utils/__init__.py
--rw-rw-rw-   0        0        0     4941 2024-05-23 06:32:37.000000 neuroweave-0.0.4/weave/_utils/core.py
-drwxrwxrwx   0        0        0        0 2024-05-23 17:56:50.131196 neuroweave-0.0.4/weave/cuda/
--rw-rw-rw-   0        0        0     1839 2024-05-23 06:31:49.000000 neuroweave-0.0.4/weave/cuda/__init__.py
--rw-rw-rw-   0        0        0     5708 2024-05-23 11:36:09.000000 neuroweave-0.0.4/weave/cuda/tools.py
-drwxrwxrwx   0        0        0        0 2024-05-23 17:56:50.133326 neuroweave-0.0.4/weave/neuro_dataset/
--rw-rw-rw-   0        0        0        0 2024-05-23 06:31:49.000000 neuroweave-0.0.4/weave/neuro_dataset/__init__.py
--rw-rw-rw-   0        0        0    23276 2024-05-23 11:36:09.000000 neuroweave-0.0.4/weave/neuro_dataset/main.py
-drwxrwxrwx   0        0        0        0 2024-05-23 17:56:50.137440 neuroweave-0.0.4/weave/neuro_functions/
--rw-rw-rw-   0        0        0        0 2024-05-23 06:31:49.000000 neuroweave-0.0.4/weave/neuro_functions/__init__.py
--rw-rw-rw-   0        0        0    28120 2024-05-23 11:30:14.000000 neuroweave-0.0.4/weave/neuro_functions/functions.py
-drwxrwxrwx   0        0        0        0 2024-05-23 17:56:50.141586 neuroweave-0.0.4/weave/neuro_storage/
--rw-rw-rw-   0        0        0        0 2024-05-23 06:31:49.000000 neuroweave-0.0.4/weave/neuro_storage/__init__.py
--rw-rw-rw-   0        0        0     2381 2024-05-23 06:32:37.000000 neuroweave-0.0.4/weave/neuro_storage/loader.py
--rw-rw-rw-   0        0        0     2795 2024-05-23 06:32:37.000000 neuroweave-0.0.4/weave/neuro_storage/saver.py
-drwxrwxrwx   0        0        0        0 2024-05-23 17:56:50.142623 neuroweave-0.0.4/weave/nn/
--rw-rw-rw-   0        0        0       46 2024-05-23 06:31:49.000000 neuroweave-0.0.4/weave/nn/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 17:56:50.148879 neuroweave-0.0.4/weave/nn/modules/
--rw-rw-rw-   0        0        0      239 2024-05-23 06:31:49.000000 neuroweave-0.0.4/weave/nn/modules/__init__.py
--rw-rw-rw-   0        0        0    10512 2024-05-23 11:30:14.000000 neuroweave-0.0.4/weave/nn/modules/activations.py
--rw-rw-rw-   0        0        0     3392 2024-05-23 11:36:09.000000 neuroweave-0.0.4/weave/nn/modules/layer.py
--rw-rw-rw-   0        0        0     5209 2024-05-23 11:30:14.000000 neuroweave-0.0.4/weave/nn/modules/losses.py
--rw-rw-rw-   0        0        0     4637 2024-05-23 11:30:14.000000 neuroweave-0.0.4/weave/nn/modules/model.py
-drwxrwxrwx   0        0        0        0 2024-05-23 17:56:50.150948 neuroweave-0.0.4/weave/nn/optim/
--rw-rw-rw-   0        0        0       55 2024-05-23 06:31:49.000000 neuroweave-0.0.4/weave/nn/optim/__init__.py
--rw-rw-rw-   0        0        0     5637 2024-05-23 11:30:14.000000 neuroweave-0.0.4/weave/nn/optim/optimizers.py
--rw-rw-rw-   0        0        0    46181 2024-05-23 17:55:40.000000 neuroweave-0.0.4/weave/tensor.py
-drwxrwxrwx   0        0        0        0 2024-05-23 17:56:50.154047 neuroweave-0.0.4/weave/visualization/
--rw-rw-rw-   0        0        0       71 2024-05-23 06:31:49.000000 neuroweave-0.0.4/weave/visualization/__init__.py
--rw-rw-rw-   0        0        0     1984 2024-05-23 11:36:09.000000 neuroweave-0.0.4/weave/visualization/weave_weights.py
+drwxrwxrwx   0        0        0        0 2024-05-23 18:07:11.440976 neuroweave-0.0.5/
+-rw-rw-rw-   0        0        0     1088 2024-04-25 14:13:00.000000 neuroweave-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     5677 2024-05-23 18:07:11.439942 neuroweave-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     4339 2024-05-23 11:36:09.000000 neuroweave-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-23 18:07:11.437874 neuroweave-0.0.5/neuroweave.egg-info/
+-rw-rw-rw-   0        0        0     5677 2024-05-23 18:07:11.000000 neuroweave-0.0.5/neuroweave.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      824 2024-05-23 18:07:11.000000 neuroweave-0.0.5/neuroweave.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 18:07:11.000000 neuroweave-0.0.5/neuroweave.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      173 2024-05-23 18:07:11.000000 neuroweave-0.0.5/neuroweave.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-23 18:07:11.000000 neuroweave-0.0.5/neuroweave.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-23 18:07:11.440976 neuroweave-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1785 2024-05-23 18:07:09.000000 neuroweave-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 18:07:11.413841 neuroweave-0.0.5/weave/
+-rw-rw-rw-   0        0        0      896 2024-05-23 11:36:09.000000 neuroweave-0.0.5/weave/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 18:07:11.414870 neuroweave-0.0.5/weave/_utils/
+-rw-rw-rw-   0        0        0       42 2024-05-23 06:31:49.000000 neuroweave-0.0.5/weave/_utils/__init__.py
+-rw-rw-rw-   0        0        0     4941 2024-05-23 06:32:37.000000 neuroweave-0.0.5/weave/_utils/core.py
+drwxrwxrwx   0        0        0        0 2024-05-23 18:07:11.418009 neuroweave-0.0.5/weave/cuda/
+-rw-rw-rw-   0        0        0     1839 2024-05-23 06:31:49.000000 neuroweave-0.0.5/weave/cuda/__init__.py
+-rw-rw-rw-   0        0        0     5708 2024-05-23 11:36:09.000000 neuroweave-0.0.5/weave/cuda/tools.py
+drwxrwxrwx   0        0        0        0 2024-05-23 18:07:11.419083 neuroweave-0.0.5/weave/neuro_dataset/
+-rw-rw-rw-   0        0        0        0 2024-05-23 06:31:49.000000 neuroweave-0.0.5/weave/neuro_dataset/__init__.py
+-rw-rw-rw-   0        0        0    23302 2024-05-23 18:06:55.000000 neuroweave-0.0.5/weave/neuro_dataset/main.py
+drwxrwxrwx   0        0        0        0 2024-05-23 18:07:11.421141 neuroweave-0.0.5/weave/neuro_functions/
+-rw-rw-rw-   0        0        0        0 2024-05-23 06:31:49.000000 neuroweave-0.0.5/weave/neuro_functions/__init__.py
+-rw-rw-rw-   0        0        0    28120 2024-05-23 11:30:14.000000 neuroweave-0.0.5/weave/neuro_functions/functions.py
+drwxrwxrwx   0        0        0        0 2024-05-23 18:07:11.424414 neuroweave-0.0.5/weave/neuro_storage/
+-rw-rw-rw-   0        0        0        0 2024-05-23 06:31:49.000000 neuroweave-0.0.5/weave/neuro_storage/__init__.py
+-rw-rw-rw-   0        0        0     2381 2024-05-23 06:32:37.000000 neuroweave-0.0.5/weave/neuro_storage/loader.py
+-rw-rw-rw-   0        0        0     2795 2024-05-23 06:32:37.000000 neuroweave-0.0.5/weave/neuro_storage/saver.py
+drwxrwxrwx   0        0        0        0 2024-05-23 18:07:11.425438 neuroweave-0.0.5/weave/nn/
+-rw-rw-rw-   0        0        0       46 2024-05-23 06:31:49.000000 neuroweave-0.0.5/weave/nn/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 18:07:11.431881 neuroweave-0.0.5/weave/nn/modules/
+-rw-rw-rw-   0        0        0      239 2024-05-23 06:31:49.000000 neuroweave-0.0.5/weave/nn/modules/__init__.py
+-rw-rw-rw-   0        0        0    10512 2024-05-23 11:30:14.000000 neuroweave-0.0.5/weave/nn/modules/activations.py
+-rw-rw-rw-   0        0        0     3392 2024-05-23 11:36:09.000000 neuroweave-0.0.5/weave/nn/modules/layer.py
+-rw-rw-rw-   0        0        0     5209 2024-05-23 11:30:14.000000 neuroweave-0.0.5/weave/nn/modules/losses.py
+-rw-rw-rw-   0        0        0     4637 2024-05-23 11:30:14.000000 neuroweave-0.0.5/weave/nn/modules/model.py
+drwxrwxrwx   0        0        0        0 2024-05-23 18:07:11.434280 neuroweave-0.0.5/weave/nn/optim/
+-rw-rw-rw-   0        0        0       55 2024-05-23 06:31:49.000000 neuroweave-0.0.5/weave/nn/optim/__init__.py
+-rw-rw-rw-   0        0        0     5637 2024-05-23 11:30:14.000000 neuroweave-0.0.5/weave/nn/optim/optimizers.py
+-rw-rw-rw-   0        0        0    46181 2024-05-23 17:55:40.000000 neuroweave-0.0.5/weave/tensor.py
+drwxrwxrwx   0        0        0        0 2024-05-23 18:07:11.436312 neuroweave-0.0.5/weave/visualization/
+-rw-rw-rw-   0        0        0       71 2024-05-23 06:31:49.000000 neuroweave-0.0.5/weave/visualization/__init__.py
+-rw-rw-rw-   0        0        0     1984 2024-05-23 11:36:09.000000 neuroweave-0.0.5/weave/visualization/weave_weights.py
```

### Comparing `neuroweave-0.0.4/LICENSE` & `neuroweave-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `neuroweave-0.0.4/PKG-INFO` & `neuroweave-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuroweave
-Version: 0.0.4
+Version: 0.0.5
 Summary: A small machine learning library.
 Author: Gabriel Niculescu, Carlos Molera, Stanislav Gatin, Patricia Pérez, Hugo Urbán
 Author-email: gabriellichu@gmail.com, info.prostaprog@gmail.com, carlosmoleracanals@gmail.com,pperezferre@gmail.com, hugourmaz@gmail.com
 Keywords: Python,Machine Learning
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: GPU :: NVIDIA CUDA :: 12
 Classifier: Intended Audience :: Education
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: neuroweave Version: 0.0.4 Summary: A small machine
+Metadata-Version: 2.1 Name: neuroweave Version: 0.0.5 Summary: A small machine
 learning library. Author: Gabriel Niculescu, Carlos Molera, Stanislav Gatin,
 Patricia PÃ©rez, Hugo UrbÃ¡n Author-email: gabriellichu@gmail.com,
 info.prostaprog@gmail.com, carlosmoleracanals@gmail.com,pperezferre@gmail.com,
 hugourmaz@gmail.com Keywords: Python,Machine Learning Classifier: Development
 Status :: 4 - Beta Classifier: Environment :: GPU :: NVIDIA CUDA :: 12
 Classifier: Intended Audience :: Education Classifier: Intended Audience ::
 Developers Classifier: Operating System :: Microsoft :: Windows Classifier:
```

### Comparing `neuroweave-0.0.4/README.md` & `neuroweave-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `neuroweave-0.0.4/neuroweave.egg-info/PKG-INFO` & `neuroweave-0.0.5/neuroweave.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuroweave
-Version: 0.0.4
+Version: 0.0.5
 Summary: A small machine learning library.
 Author: Gabriel Niculescu, Carlos Molera, Stanislav Gatin, Patricia Pérez, Hugo Urbán
 Author-email: gabriellichu@gmail.com, info.prostaprog@gmail.com, carlosmoleracanals@gmail.com,pperezferre@gmail.com, hugourmaz@gmail.com
 Keywords: Python,Machine Learning
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: GPU :: NVIDIA CUDA :: 12
 Classifier: Intended Audience :: Education
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: neuroweave Version: 0.0.4 Summary: A small machine
+Metadata-Version: 2.1 Name: neuroweave Version: 0.0.5 Summary: A small machine
 learning library. Author: Gabriel Niculescu, Carlos Molera, Stanislav Gatin,
 Patricia PÃ©rez, Hugo UrbÃ¡n Author-email: gabriellichu@gmail.com,
 info.prostaprog@gmail.com, carlosmoleracanals@gmail.com,pperezferre@gmail.com,
 hugourmaz@gmail.com Keywords: Python,Machine Learning Classifier: Development
 Status :: 4 - Beta Classifier: Environment :: GPU :: NVIDIA CUDA :: 12
 Classifier: Intended Audience :: Education Classifier: Intended Audience ::
 Developers Classifier: Operating System :: Microsoft :: Windows Classifier:
```

### Comparing `neuroweave-0.0.4/neuroweave.egg-info/SOURCES.txt` & `neuroweave-0.0.5/neuroweave.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neuroweave-0.0.4/setup.py` & `neuroweave-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import codecs
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 with codecs.open(os.path.join(here, 'README.md'), encoding='utf-8') as fh:
     long_description = fh.read()
 
-VERSION = '0.0.4'
+VERSION = '0.0.5'
 DESCRIPTION = 'A small machine learning library.'
 LONG_DESCRIPTION = ('A Machine Learning library with the basic components necessary for building basic '
                     'Neural Network Models')
 
 setup(
     name='neuroweave',
     version=VERSION,
```

### Comparing `neuroweave-0.0.4/weave/__init__.py` & `neuroweave-0.0.5/weave/__init__.py`

 * *Files identical despite different names*

### Comparing `neuroweave-0.0.4/weave/_utils/core.py` & `neuroweave-0.0.5/weave/_utils/core.py`

 * *Files identical despite different names*

### Comparing `neuroweave-0.0.4/weave/cuda/__init__.py` & `neuroweave-0.0.5/weave/cuda/__init__.py`

 * *Files identical despite different names*

### Comparing `neuroweave-0.0.4/weave/cuda/tools.py` & `neuroweave-0.0.5/weave/cuda/tools.py`

 * *Files identical despite different names*

### Comparing `neuroweave-0.0.4/weave/neuro_dataset/main.py` & `neuroweave-0.0.5/weave/neuro_dataset/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,16 @@
     # the mean and scaling to unit variance
     "StandardScaler",
     # Function for one-hot encoding categorical variables
     "one_hot_encode",
     # Class for applying different transformations to different columns
     "ColumnTransformer",
     # Function for label encoding categorical variables
-    "label_encode"
+    "label_encode",
+    "train_test_split",
 ]
 
 
 class Dataset:
     """
         This class is used to load and manage a dataset from a file. It supports
         loading data from a CSV file and provides methods for accessing and
```

### Comparing `neuroweave-0.0.4/weave/neuro_functions/functions.py` & `neuroweave-0.0.5/weave/neuro_functions/functions.py`

 * *Files identical despite different names*

### Comparing `neuroweave-0.0.4/weave/neuro_storage/loader.py` & `neuroweave-0.0.5/weave/neuro_storage/loader.py`

 * *Files identical despite different names*

### Comparing `neuroweave-0.0.4/weave/neuro_storage/saver.py` & `neuroweave-0.0.5/weave/neuro_storage/saver.py`

 * *Files identical despite different names*

### Comparing `neuroweave-0.0.4/weave/nn/modules/activations.py` & `neuroweave-0.0.5/weave/nn/modules/activations.py`

 * *Files identical despite different names*

### Comparing `neuroweave-0.0.4/weave/nn/modules/layer.py` & `neuroweave-0.0.5/weave/nn/modules/layer.py`

 * *Files identical despite different names*

### Comparing `neuroweave-0.0.4/weave/nn/modules/losses.py` & `neuroweave-0.0.5/weave/nn/modules/losses.py`

 * *Files identical despite different names*

### Comparing `neuroweave-0.0.4/weave/nn/modules/model.py` & `neuroweave-0.0.5/weave/nn/modules/model.py`

 * *Files identical despite different names*

### Comparing `neuroweave-0.0.4/weave/nn/optim/optimizers.py` & `neuroweave-0.0.5/weave/nn/optim/optimizers.py`

 * *Files identical despite different names*

### Comparing `neuroweave-0.0.4/weave/tensor.py` & `neuroweave-0.0.5/weave/tensor.py`

 * *Files identical despite different names*

### Comparing `neuroweave-0.0.4/weave/visualization/weave_weights.py` & `neuroweave-0.0.5/weave/visualization/weave_weights.py`

 * *Files identical despite different names*

