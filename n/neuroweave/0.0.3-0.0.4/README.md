# Comparing `tmp/neuroweave-0.0.3.tar.gz` & `tmp/neuroweave-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuroweave-0.0.3.tar", last modified: Thu May 23 11:51:41 2024, max compression
+gzip compressed data, was "neuroweave-0.0.4.tar", last modified: Thu May 23 17:56:50 2024, max compression
```

## Comparing `neuroweave-0.0.3.tar` & `neuroweave-0.0.4.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 11:51:41.915036 neuroweave-0.0.3/
--rw-rw-rw-   0        0        0     1088 2024-04-25 14:13:00.000000 neuroweave-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     5677 2024-05-23 11:51:41.915036 neuroweave-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     4339 2024-05-23 11:36:09.000000 neuroweave-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-23 11:51:41.913951 neuroweave-0.0.3/neuroweave.egg-info/
--rw-rw-rw-   0        0        0     5677 2024-05-23 11:51:41.000000 neuroweave-0.0.3/neuroweave.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      824 2024-05-23 11:51:41.000000 neuroweave-0.0.3/neuroweave.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 11:51:41.000000 neuroweave-0.0.3/neuroweave.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      173 2024-05-23 11:51:41.000000 neuroweave-0.0.3/neuroweave.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-05-23 11:51:41.000000 neuroweave-0.0.3/neuroweave.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-23 11:51:41.916063 neuroweave-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1785 2024-05-23 11:51:39.000000 neuroweave-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-23 11:51:41.891738 neuroweave-0.0.3/weave/
--rw-rw-rw-   0        0        0      896 2024-05-23 11:36:09.000000 neuroweave-0.0.3/weave/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 11:51:41.895518 neuroweave-0.0.3/weave/_utils/
--rw-rw-rw-   0        0        0       42 2024-05-23 06:31:49.000000 neuroweave-0.0.3/weave/_utils/__init__.py
--rw-rw-rw-   0        0        0     4941 2024-05-23 06:32:37.000000 neuroweave-0.0.3/weave/_utils/core.py
-drwxrwxrwx   0        0        0        0 2024-05-23 11:51:41.898149 neuroweave-0.0.3/weave/cuda/
--rw-rw-rw-   0        0        0     1839 2024-05-23 06:31:49.000000 neuroweave-0.0.3/weave/cuda/__init__.py
--rw-rw-rw-   0        0        0     5708 2024-05-23 11:36:09.000000 neuroweave-0.0.3/weave/cuda/tools.py
-drwxrwxrwx   0        0        0        0 2024-05-23 11:51:41.899773 neuroweave-0.0.3/weave/neuro_dataset/
--rw-rw-rw-   0        0        0        0 2024-05-23 06:31:49.000000 neuroweave-0.0.3/weave/neuro_dataset/__init__.py
--rw-rw-rw-   0        0        0    23276 2024-05-23 11:36:09.000000 neuroweave-0.0.3/weave/neuro_dataset/main.py
-drwxrwxrwx   0        0        0        0 2024-05-23 11:51:41.901854 neuroweave-0.0.3/weave/neuro_functions/
--rw-rw-rw-   0        0        0        0 2024-05-23 06:31:49.000000 neuroweave-0.0.3/weave/neuro_functions/__init__.py
--rw-rw-rw-   0        0        0    28120 2024-05-23 11:30:14.000000 neuroweave-0.0.3/weave/neuro_functions/functions.py
-drwxrwxrwx   0        0        0        0 2024-05-23 11:51:41.903930 neuroweave-0.0.3/weave/neuro_storage/
--rw-rw-rw-   0        0        0        0 2024-05-23 06:31:49.000000 neuroweave-0.0.3/weave/neuro_storage/__init__.py
--rw-rw-rw-   0        0        0     2381 2024-05-23 06:32:37.000000 neuroweave-0.0.3/weave/neuro_storage/loader.py
--rw-rw-rw-   0        0        0     2795 2024-05-23 06:32:37.000000 neuroweave-0.0.3/weave/neuro_storage/saver.py
-drwxrwxrwx   0        0        0        0 2024-05-23 11:51:41.904962 neuroweave-0.0.3/weave/nn/
--rw-rw-rw-   0        0        0       46 2024-05-23 06:31:49.000000 neuroweave-0.0.3/weave/nn/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 11:51:41.909010 neuroweave-0.0.3/weave/nn/modules/
--rw-rw-rw-   0        0        0      239 2024-05-23 06:31:49.000000 neuroweave-0.0.3/weave/nn/modules/__init__.py
--rw-rw-rw-   0        0        0    10512 2024-05-23 11:30:14.000000 neuroweave-0.0.3/weave/nn/modules/activations.py
--rw-rw-rw-   0        0        0     3392 2024-05-23 11:36:09.000000 neuroweave-0.0.3/weave/nn/modules/layer.py
--rw-rw-rw-   0        0        0     5209 2024-05-23 11:30:14.000000 neuroweave-0.0.3/weave/nn/modules/losses.py
--rw-rw-rw-   0        0        0     4637 2024-05-23 11:30:14.000000 neuroweave-0.0.3/weave/nn/modules/model.py
-drwxrwxrwx   0        0        0        0 2024-05-23 11:51:41.910823 neuroweave-0.0.3/weave/nn/optim/
--rw-rw-rw-   0        0        0       55 2024-05-23 06:31:49.000000 neuroweave-0.0.3/weave/nn/optim/__init__.py
--rw-rw-rw-   0        0        0     5637 2024-05-23 11:30:14.000000 neuroweave-0.0.3/weave/nn/optim/optimizers.py
--rw-rw-rw-   0        0        0    46216 2024-05-23 11:30:14.000000 neuroweave-0.0.3/weave/tensor.py
-drwxrwxrwx   0        0        0        0 2024-05-23 11:51:41.912917 neuroweave-0.0.3/weave/visualization/
--rw-rw-rw-   0        0        0       71 2024-05-23 06:31:49.000000 neuroweave-0.0.3/weave/visualization/__init__.py
--rw-rw-rw-   0        0        0     1984 2024-05-23 11:36:09.000000 neuroweave-0.0.3/weave/visualization/weave_weights.py
+drwxrwxrwx   0        0        0        0 2024-05-23 17:56:50.159268 neuroweave-0.0.4/
+-rw-rw-rw-   0        0        0     1088 2024-04-25 14:13:00.000000 neuroweave-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     5677 2024-05-23 17:56:50.157159 neuroweave-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4339 2024-05-23 11:36:09.000000 neuroweave-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-23 17:56:50.155090 neuroweave-0.0.4/neuroweave.egg-info/
+-rw-rw-rw-   0        0        0     5677 2024-05-23 17:56:50.000000 neuroweave-0.0.4/neuroweave.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      824 2024-05-23 17:56:50.000000 neuroweave-0.0.4/neuroweave.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 17:56:50.000000 neuroweave-0.0.4/neuroweave.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      173 2024-05-23 17:56:50.000000 neuroweave-0.0.4/neuroweave.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-23 17:56:50.000000 neuroweave-0.0.4/neuroweave.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-23 17:56:50.159268 neuroweave-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1785 2024-05-23 17:55:58.000000 neuroweave-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 17:56:50.126992 neuroweave-0.0.4/weave/
+-rw-rw-rw-   0        0        0      896 2024-05-23 11:36:09.000000 neuroweave-0.0.4/weave/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 17:56:50.129107 neuroweave-0.0.4/weave/_utils/
+-rw-rw-rw-   0        0        0       42 2024-05-23 06:31:49.000000 neuroweave-0.0.4/weave/_utils/__init__.py
+-rw-rw-rw-   0        0        0     4941 2024-05-23 06:32:37.000000 neuroweave-0.0.4/weave/_utils/core.py
+drwxrwxrwx   0        0        0        0 2024-05-23 17:56:50.131196 neuroweave-0.0.4/weave/cuda/
+-rw-rw-rw-   0        0        0     1839 2024-05-23 06:31:49.000000 neuroweave-0.0.4/weave/cuda/__init__.py
+-rw-rw-rw-   0        0        0     5708 2024-05-23 11:36:09.000000 neuroweave-0.0.4/weave/cuda/tools.py
+drwxrwxrwx   0        0        0        0 2024-05-23 17:56:50.133326 neuroweave-0.0.4/weave/neuro_dataset/
+-rw-rw-rw-   0        0        0        0 2024-05-23 06:31:49.000000 neuroweave-0.0.4/weave/neuro_dataset/__init__.py
+-rw-rw-rw-   0        0        0    23276 2024-05-23 11:36:09.000000 neuroweave-0.0.4/weave/neuro_dataset/main.py
+drwxrwxrwx   0        0        0        0 2024-05-23 17:56:50.137440 neuroweave-0.0.4/weave/neuro_functions/
+-rw-rw-rw-   0        0        0        0 2024-05-23 06:31:49.000000 neuroweave-0.0.4/weave/neuro_functions/__init__.py
+-rw-rw-rw-   0        0        0    28120 2024-05-23 11:30:14.000000 neuroweave-0.0.4/weave/neuro_functions/functions.py
+drwxrwxrwx   0        0        0        0 2024-05-23 17:56:50.141586 neuroweave-0.0.4/weave/neuro_storage/
+-rw-rw-rw-   0        0        0        0 2024-05-23 06:31:49.000000 neuroweave-0.0.4/weave/neuro_storage/__init__.py
+-rw-rw-rw-   0        0        0     2381 2024-05-23 06:32:37.000000 neuroweave-0.0.4/weave/neuro_storage/loader.py
+-rw-rw-rw-   0        0        0     2795 2024-05-23 06:32:37.000000 neuroweave-0.0.4/weave/neuro_storage/saver.py
+drwxrwxrwx   0        0        0        0 2024-05-23 17:56:50.142623 neuroweave-0.0.4/weave/nn/
+-rw-rw-rw-   0        0        0       46 2024-05-23 06:31:49.000000 neuroweave-0.0.4/weave/nn/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 17:56:50.148879 neuroweave-0.0.4/weave/nn/modules/
+-rw-rw-rw-   0        0        0      239 2024-05-23 06:31:49.000000 neuroweave-0.0.4/weave/nn/modules/__init__.py
+-rw-rw-rw-   0        0        0    10512 2024-05-23 11:30:14.000000 neuroweave-0.0.4/weave/nn/modules/activations.py
+-rw-rw-rw-   0        0        0     3392 2024-05-23 11:36:09.000000 neuroweave-0.0.4/weave/nn/modules/layer.py
+-rw-rw-rw-   0        0        0     5209 2024-05-23 11:30:14.000000 neuroweave-0.0.4/weave/nn/modules/losses.py
+-rw-rw-rw-   0        0        0     4637 2024-05-23 11:30:14.000000 neuroweave-0.0.4/weave/nn/modules/model.py
+drwxrwxrwx   0        0        0        0 2024-05-23 17:56:50.150948 neuroweave-0.0.4/weave/nn/optim/
+-rw-rw-rw-   0        0        0       55 2024-05-23 06:31:49.000000 neuroweave-0.0.4/weave/nn/optim/__init__.py
+-rw-rw-rw-   0        0        0     5637 2024-05-23 11:30:14.000000 neuroweave-0.0.4/weave/nn/optim/optimizers.py
+-rw-rw-rw-   0        0        0    46181 2024-05-23 17:55:40.000000 neuroweave-0.0.4/weave/tensor.py
+drwxrwxrwx   0        0        0        0 2024-05-23 17:56:50.154047 neuroweave-0.0.4/weave/visualization/
+-rw-rw-rw-   0        0        0       71 2024-05-23 06:31:49.000000 neuroweave-0.0.4/weave/visualization/__init__.py
+-rw-rw-rw-   0        0        0     1984 2024-05-23 11:36:09.000000 neuroweave-0.0.4/weave/visualization/weave_weights.py
```

### Comparing `neuroweave-0.0.3/LICENSE` & `neuroweave-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `neuroweave-0.0.3/PKG-INFO` & `neuroweave-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuroweave
-Version: 0.0.3
+Version: 0.0.4
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
-Metadata-Version: 2.1 Name: neuroweave Version: 0.0.3 Summary: A small machine
+Metadata-Version: 2.1 Name: neuroweave Version: 0.0.4 Summary: A small machine
 learning library. Author: Gabriel Niculescu, Carlos Molera, Stanislav Gatin,
 Patricia PÃ©rez, Hugo UrbÃ¡n Author-email: gabriellichu@gmail.com,
 info.prostaprog@gmail.com, carlosmoleracanals@gmail.com,pperezferre@gmail.com,
 hugourmaz@gmail.com Keywords: Python,Machine Learning Classifier: Development
 Status :: 4 - Beta Classifier: Environment :: GPU :: NVIDIA CUDA :: 12
 Classifier: Intended Audience :: Education Classifier: Intended Audience ::
 Developers Classifier: Operating System :: Microsoft :: Windows Classifier:
```

### Comparing `neuroweave-0.0.3/README.md` & `neuroweave-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `neuroweave-0.0.3/neuroweave.egg-info/PKG-INFO` & `neuroweave-0.0.4/neuroweave.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuroweave
-Version: 0.0.3
+Version: 0.0.4
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
-Metadata-Version: 2.1 Name: neuroweave Version: 0.0.3 Summary: A small machine
+Metadata-Version: 2.1 Name: neuroweave Version: 0.0.4 Summary: A small machine
 learning library. Author: Gabriel Niculescu, Carlos Molera, Stanislav Gatin,
 Patricia PÃ©rez, Hugo UrbÃ¡n Author-email: gabriellichu@gmail.com,
 info.prostaprog@gmail.com, carlosmoleracanals@gmail.com,pperezferre@gmail.com,
 hugourmaz@gmail.com Keywords: Python,Machine Learning Classifier: Development
 Status :: 4 - Beta Classifier: Environment :: GPU :: NVIDIA CUDA :: 12
 Classifier: Intended Audience :: Education Classifier: Intended Audience ::
 Developers Classifier: Operating System :: Microsoft :: Windows Classifier:
```

### Comparing `neuroweave-0.0.3/neuroweave.egg-info/SOURCES.txt` & `neuroweave-0.0.4/neuroweave.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neuroweave-0.0.3/setup.py` & `neuroweave-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import codecs
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 with codecs.open(os.path.join(here, 'README.md'), encoding='utf-8') as fh:
     long_description = fh.read()
 
-VERSION = '0.0.3'
+VERSION = '0.0.4'
 DESCRIPTION = 'A small machine learning library.'
 LONG_DESCRIPTION = ('A Machine Learning library with the basic components necessary for building basic '
                     'Neural Network Models')
 
 setup(
     name='neuroweave',
     version=VERSION,
```

### Comparing `neuroweave-0.0.3/weave/__init__.py` & `neuroweave-0.0.4/weave/__init__.py`

 * *Files identical despite different names*

### Comparing `neuroweave-0.0.3/weave/_utils/core.py` & `neuroweave-0.0.4/weave/_utils/core.py`

 * *Files identical despite different names*

### Comparing `neuroweave-0.0.3/weave/cuda/__init__.py` & `neuroweave-0.0.4/weave/cuda/__init__.py`

 * *Files identical despite different names*

### Comparing `neuroweave-0.0.3/weave/cuda/tools.py` & `neuroweave-0.0.4/weave/cuda/tools.py`

 * *Files identical despite different names*

### Comparing `neuroweave-0.0.3/weave/neuro_dataset/main.py` & `neuroweave-0.0.4/weave/neuro_dataset/main.py`

 * *Files identical despite different names*

### Comparing `neuroweave-0.0.3/weave/neuro_functions/functions.py` & `neuroweave-0.0.4/weave/neuro_functions/functions.py`

 * *Files identical despite different names*

### Comparing `neuroweave-0.0.3/weave/neuro_storage/loader.py` & `neuroweave-0.0.4/weave/neuro_storage/loader.py`

 * *Files identical despite different names*

### Comparing `neuroweave-0.0.3/weave/neuro_storage/saver.py` & `neuroweave-0.0.4/weave/neuro_storage/saver.py`

 * *Files identical despite different names*

### Comparing `neuroweave-0.0.3/weave/nn/modules/activations.py` & `neuroweave-0.0.4/weave/nn/modules/activations.py`

 * *Files identical despite different names*

### Comparing `neuroweave-0.0.3/weave/nn/modules/layer.py` & `neuroweave-0.0.4/weave/nn/modules/layer.py`

 * *Files identical despite different names*

### Comparing `neuroweave-0.0.3/weave/nn/modules/losses.py` & `neuroweave-0.0.4/weave/nn/modules/losses.py`

 * *Files identical despite different names*

### Comparing `neuroweave-0.0.3/weave/nn/modules/model.py` & `neuroweave-0.0.4/weave/nn/modules/model.py`

 * *Files identical despite different names*

### Comparing `neuroweave-0.0.3/weave/nn/optim/optimizers.py` & `neuroweave-0.0.4/weave/nn/optim/optimizers.py`

 * *Files identical despite different names*

### Comparing `neuroweave-0.0.3/weave/tensor.py` & `neuroweave-0.0.4/weave/tensor.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,17 +65,17 @@
                 dtype = array.dtype
         elif shape is None and data is None:
             raise AttributeError('Either shape or data must be given when creating the array.')
         return super().__new__(cls, shape, dtype, buffer, offset, strides, order)
 
     def __init__(self, shape=None, dtype=None, *, data=None, _children=(), _op=None, use_grad: bool = False,
                  device: Union['weave.cuda.Device', str] = 'cpu'):
-        if use_grad is True and self.dtype not in [*neuroweave._float_types, float]:
+        if use_grad is True and self.dtype not in [*weave._float_types, float]:
             raise ValueError('Only Tensors with floating types support gradients.')
-        self.device = neuroweave.cuda.Device(device) if isinstance(device, str) else device  # assign the correct device
+        self.device = weave.cuda.Device(device) if isinstance(device, str) else device  # assign the correct device
         self._data: Any
         self.data = data
         if data is not None:
             self._populate(data)  # If data was provided, we populate the tensor making use of NumPy's API
         self.grad = 0
         # We only store the data for the backward functions if use_grad is enabled
         if use_grad:
@@ -86,21 +86,21 @@
 
     def __array_finalize__(self, obj):
         # We just make use of NumPy's API, but we have to adapt it in order to get a Tensor object
         pass
 
     def _populate(self, data):
         if self.device == 'cpu':
-            cpu_accepted_types = Union[np.ndarray, int, float, Tensor, list, *neuroweave._types]
+            cpu_accepted_types = Union[np.ndarray, int, float, Tensor, list, *weave._types]
             if not isinstance(data, cpu_accepted_types):
                 raise TypeError(f'Invalid data type for Tensor: {data.__class__.__name__}')
             # By using ellipsis indexing, we can refer to all the dimensions of the Tensor
             self[...] = data
         else:
-            cuda_accepted_types = Union[np.ndarray, int, float, cp.ndarray, Tensor, list, *neuroweave._types]
+            cuda_accepted_types = Union[np.ndarray, int, float, cp.ndarray, Tensor, list, *weave._types]
             if not isinstance(data, cuda_accepted_types):
                 raise TypeError(f'Invalid data type for Tensor: {data.__class__.__name__}')
             # By using ellipsis indexing, we can refer to all the dimensions of the Tensor
             self[...] = data.get() if isinstance(data, cp.ndarray) else data
 
     def __add__(self, other: Any) -> "Tensor":
         if type(other) in [np.ndarray, list]:  # transform organized data structures into Tensors
@@ -495,15 +495,15 @@
 
     @data.setter
     def data(self, value):
         if self.device == 'cpu':
             if value is None:
                 self._data = np.asarray(self)
             else:
-                types = Union[np.ndarray, list, *neuroweave._types, int, float, Tensor]
+                types = Union[np.ndarray, list, *weave._types, int, float, Tensor]
                 self._data = value.get() if not isinstance(value, types) else np.asarray(value, dtype=self.dtype)
         else:
             if value is None:
                 # cupy tends to make arrays of nan in some cases, so we have to fix for it
                 self._data = cp.nan_to_num(cp.asarray(self, dtype=self.dtype))
             else:
                 self._data = value if isinstance(value, cp.ndarray) else cp.asarray(value, dtype=self.dtype)
@@ -559,23 +559,23 @@
             node._backward()  # Run the backwards function of all tensors in reverse
 
     def cpu(self):
         """
         Transfers the tensor and all its attributes to the CPU memory if not already in it.
         """
         if not (self.device == 'cpu'):
-            self.device = neuroweave.cuda.Device('cpu')
+            self.device = weave.cuda.Device('cpu')
             self.data = self.data.get()
 
     def cuda(self):
         """
         Transfers the tensor and all its attributes to the GPU memory if not already in it.
         """
         if self.device == 'cpu':
-            self.device = neuroweave.cuda.Device('cuda')
+            self.device = weave.cuda.Device('cuda')
             self.data = cp.asarray(self.data)
 
     # From this point onward, we implement many of the methods that a subclass from numpy.ndarray is expected to have.
     # Due to the sheer amount of methods, however, only some of them have been implemented, and these have been selected
     # according to how common we believe them to be in a Machine Learning environment.
     # Another thing to note is that some of the arguments or keyword arguments for the methods are left unused even when
     # they are still defined. This is to maintain compatibility with CuPy's array model as well as sticking to NumPy's
```

### Comparing `neuroweave-0.0.3/weave/visualization/weave_weights.py` & `neuroweave-0.0.4/weave/visualization/weave_weights.py`

 * *Files identical despite different names*

