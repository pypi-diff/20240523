# Comparing `tmp/neuroweave-0.0.2.tar.gz` & `tmp/neuroweave-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuroweave-0.0.2.tar", last modified: Thu May 23 11:45:01 2024, max compression
+gzip compressed data, was "neuroweave-0.0.3.tar", last modified: Thu May 23 11:51:41 2024, max compression
```

## Comparing `neuroweave-0.0.2.tar` & `neuroweave-0.0.3.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 11:45:01.586955 neuroweave-0.0.2/
--rw-rw-rw-   0        0        0     1088 2024-04-25 14:13:00.000000 neuroweave-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     5678 2024-05-23 11:45:01.584954 neuroweave-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     4339 2024-05-23 11:36:09.000000 neuroweave-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-23 11:45:01.583951 neuroweave-0.0.2/neuroweave.egg-info/
--rw-rw-rw-   0        0        0     5678 2024-05-23 11:45:01.000000 neuroweave-0.0.2/neuroweave.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      824 2024-05-23 11:45:01.000000 neuroweave-0.0.2/neuroweave.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 11:45:01.000000 neuroweave-0.0.2/neuroweave.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      174 2024-05-23 11:45:01.000000 neuroweave-0.0.2/neuroweave.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-05-23 11:45:01.000000 neuroweave-0.0.2/neuroweave.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-23 11:45:01.586955 neuroweave-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1786 2024-05-23 11:44:35.000000 neuroweave-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-23 11:45:01.549167 neuroweave-0.0.2/weave/
--rw-rw-rw-   0        0        0      896 2024-05-23 11:36:09.000000 neuroweave-0.0.2/weave/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 11:45:01.551230 neuroweave-0.0.2/weave/_utils/
--rw-rw-rw-   0        0        0       42 2024-05-23 06:31:49.000000 neuroweave-0.0.2/weave/_utils/__init__.py
--rw-rw-rw-   0        0        0     4941 2024-05-23 06:32:37.000000 neuroweave-0.0.2/weave/_utils/core.py
-drwxrwxrwx   0        0        0        0 2024-05-23 11:45:01.553445 neuroweave-0.0.2/weave/cuda/
--rw-rw-rw-   0        0        0     1839 2024-05-23 06:31:49.000000 neuroweave-0.0.2/weave/cuda/__init__.py
--rw-rw-rw-   0        0        0     5708 2024-05-23 11:36:09.000000 neuroweave-0.0.2/weave/cuda/tools.py
-drwxrwxrwx   0        0        0        0 2024-05-23 11:45:01.555507 neuroweave-0.0.2/weave/neuro_dataset/
--rw-rw-rw-   0        0        0        0 2024-05-23 06:31:49.000000 neuroweave-0.0.2/weave/neuro_dataset/__init__.py
--rw-rw-rw-   0        0        0    23276 2024-05-23 11:36:09.000000 neuroweave-0.0.2/weave/neuro_dataset/main.py
-drwxrwxrwx   0        0        0        0 2024-05-23 11:45:01.557659 neuroweave-0.0.2/weave/neuro_functions/
--rw-rw-rw-   0        0        0        0 2024-05-23 06:31:49.000000 neuroweave-0.0.2/weave/neuro_functions/__init__.py
--rw-rw-rw-   0        0        0    28120 2024-05-23 11:30:14.000000 neuroweave-0.0.2/weave/neuro_functions/functions.py
-drwxrwxrwx   0        0        0        0 2024-05-23 11:45:01.571610 neuroweave-0.0.2/weave/neuro_storage/
--rw-rw-rw-   0        0        0        0 2024-05-23 06:31:49.000000 neuroweave-0.0.2/weave/neuro_storage/__init__.py
--rw-rw-rw-   0        0        0     2381 2024-05-23 06:32:37.000000 neuroweave-0.0.2/weave/neuro_storage/loader.py
--rw-rw-rw-   0        0        0     2795 2024-05-23 06:32:37.000000 neuroweave-0.0.2/weave/neuro_storage/saver.py
-drwxrwxrwx   0        0        0        0 2024-05-23 11:45:01.572444 neuroweave-0.0.2/weave/nn/
--rw-rw-rw-   0        0        0       46 2024-05-23 06:31:49.000000 neuroweave-0.0.2/weave/nn/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 11:45:01.577843 neuroweave-0.0.2/weave/nn/modules/
--rw-rw-rw-   0        0        0      239 2024-05-23 06:31:49.000000 neuroweave-0.0.2/weave/nn/modules/__init__.py
--rw-rw-rw-   0        0        0    10512 2024-05-23 11:30:14.000000 neuroweave-0.0.2/weave/nn/modules/activations.py
--rw-rw-rw-   0        0        0     3392 2024-05-23 11:36:09.000000 neuroweave-0.0.2/weave/nn/modules/layer.py
--rw-rw-rw-   0        0        0     5209 2024-05-23 11:30:14.000000 neuroweave-0.0.2/weave/nn/modules/losses.py
--rw-rw-rw-   0        0        0     4637 2024-05-23 11:30:14.000000 neuroweave-0.0.2/weave/nn/modules/model.py
-drwxrwxrwx   0        0        0        0 2024-05-23 11:45:01.580752 neuroweave-0.0.2/weave/nn/optim/
--rw-rw-rw-   0        0        0       55 2024-05-23 06:31:49.000000 neuroweave-0.0.2/weave/nn/optim/__init__.py
--rw-rw-rw-   0        0        0     5637 2024-05-23 11:30:14.000000 neuroweave-0.0.2/weave/nn/optim/optimizers.py
--rw-rw-rw-   0        0        0    46216 2024-05-23 11:30:14.000000 neuroweave-0.0.2/weave/tensor.py
-drwxrwxrwx   0        0        0        0 2024-05-23 11:45:01.582844 neuroweave-0.0.2/weave/visualization/
--rw-rw-rw-   0        0        0       71 2024-05-23 06:31:49.000000 neuroweave-0.0.2/weave/visualization/__init__.py
--rw-rw-rw-   0        0        0     1984 2024-05-23 11:36:09.000000 neuroweave-0.0.2/weave/visualization/weave_weights.py
+drwxrwxrwx   0        0        0        0 2024-05-23 11:51:41.915036 neuroweave-0.0.3/
+-rw-rw-rw-   0        0        0     1088 2024-04-25 14:13:00.000000 neuroweave-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     5677 2024-05-23 11:51:41.915036 neuroweave-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     4339 2024-05-23 11:36:09.000000 neuroweave-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-23 11:51:41.913951 neuroweave-0.0.3/neuroweave.egg-info/
+-rw-rw-rw-   0        0        0     5677 2024-05-23 11:51:41.000000 neuroweave-0.0.3/neuroweave.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      824 2024-05-23 11:51:41.000000 neuroweave-0.0.3/neuroweave.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 11:51:41.000000 neuroweave-0.0.3/neuroweave.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      173 2024-05-23 11:51:41.000000 neuroweave-0.0.3/neuroweave.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-23 11:51:41.000000 neuroweave-0.0.3/neuroweave.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-23 11:51:41.916063 neuroweave-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1785 2024-05-23 11:51:39.000000 neuroweave-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 11:51:41.891738 neuroweave-0.0.3/weave/
+-rw-rw-rw-   0        0        0      896 2024-05-23 11:36:09.000000 neuroweave-0.0.3/weave/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 11:51:41.895518 neuroweave-0.0.3/weave/_utils/
+-rw-rw-rw-   0        0        0       42 2024-05-23 06:31:49.000000 neuroweave-0.0.3/weave/_utils/__init__.py
+-rw-rw-rw-   0        0        0     4941 2024-05-23 06:32:37.000000 neuroweave-0.0.3/weave/_utils/core.py
+drwxrwxrwx   0        0        0        0 2024-05-23 11:51:41.898149 neuroweave-0.0.3/weave/cuda/
+-rw-rw-rw-   0        0        0     1839 2024-05-23 06:31:49.000000 neuroweave-0.0.3/weave/cuda/__init__.py
+-rw-rw-rw-   0        0        0     5708 2024-05-23 11:36:09.000000 neuroweave-0.0.3/weave/cuda/tools.py
+drwxrwxrwx   0        0        0        0 2024-05-23 11:51:41.899773 neuroweave-0.0.3/weave/neuro_dataset/
+-rw-rw-rw-   0        0        0        0 2024-05-23 06:31:49.000000 neuroweave-0.0.3/weave/neuro_dataset/__init__.py
+-rw-rw-rw-   0        0        0    23276 2024-05-23 11:36:09.000000 neuroweave-0.0.3/weave/neuro_dataset/main.py
+drwxrwxrwx   0        0        0        0 2024-05-23 11:51:41.901854 neuroweave-0.0.3/weave/neuro_functions/
+-rw-rw-rw-   0        0        0        0 2024-05-23 06:31:49.000000 neuroweave-0.0.3/weave/neuro_functions/__init__.py
+-rw-rw-rw-   0        0        0    28120 2024-05-23 11:30:14.000000 neuroweave-0.0.3/weave/neuro_functions/functions.py
+drwxrwxrwx   0        0        0        0 2024-05-23 11:51:41.903930 neuroweave-0.0.3/weave/neuro_storage/
+-rw-rw-rw-   0        0        0        0 2024-05-23 06:31:49.000000 neuroweave-0.0.3/weave/neuro_storage/__init__.py
+-rw-rw-rw-   0        0        0     2381 2024-05-23 06:32:37.000000 neuroweave-0.0.3/weave/neuro_storage/loader.py
+-rw-rw-rw-   0        0        0     2795 2024-05-23 06:32:37.000000 neuroweave-0.0.3/weave/neuro_storage/saver.py
+drwxrwxrwx   0        0        0        0 2024-05-23 11:51:41.904962 neuroweave-0.0.3/weave/nn/
+-rw-rw-rw-   0        0        0       46 2024-05-23 06:31:49.000000 neuroweave-0.0.3/weave/nn/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 11:51:41.909010 neuroweave-0.0.3/weave/nn/modules/
+-rw-rw-rw-   0        0        0      239 2024-05-23 06:31:49.000000 neuroweave-0.0.3/weave/nn/modules/__init__.py
+-rw-rw-rw-   0        0        0    10512 2024-05-23 11:30:14.000000 neuroweave-0.0.3/weave/nn/modules/activations.py
+-rw-rw-rw-   0        0        0     3392 2024-05-23 11:36:09.000000 neuroweave-0.0.3/weave/nn/modules/layer.py
+-rw-rw-rw-   0        0        0     5209 2024-05-23 11:30:14.000000 neuroweave-0.0.3/weave/nn/modules/losses.py
+-rw-rw-rw-   0        0        0     4637 2024-05-23 11:30:14.000000 neuroweave-0.0.3/weave/nn/modules/model.py
+drwxrwxrwx   0        0        0        0 2024-05-23 11:51:41.910823 neuroweave-0.0.3/weave/nn/optim/
+-rw-rw-rw-   0        0        0       55 2024-05-23 06:31:49.000000 neuroweave-0.0.3/weave/nn/optim/__init__.py
+-rw-rw-rw-   0        0        0     5637 2024-05-23 11:30:14.000000 neuroweave-0.0.3/weave/nn/optim/optimizers.py
+-rw-rw-rw-   0        0        0    46216 2024-05-23 11:30:14.000000 neuroweave-0.0.3/weave/tensor.py
+drwxrwxrwx   0        0        0        0 2024-05-23 11:51:41.912917 neuroweave-0.0.3/weave/visualization/
+-rw-rw-rw-   0        0        0       71 2024-05-23 06:31:49.000000 neuroweave-0.0.3/weave/visualization/__init__.py
+-rw-rw-rw-   0        0        0     1984 2024-05-23 11:36:09.000000 neuroweave-0.0.3/weave/visualization/weave_weights.py
```

### Comparing `neuroweave-0.0.2/LICENSE` & `neuroweave-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `neuroweave-0.0.2/PKG-INFO` & `neuroweave-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuroweave
-Version: 0.0.2
+Version: 0.0.3
 Summary: A small machine learning library.
 Author: Gabriel Niculescu, Carlos Molera, Stanislav Gatin, Patricia Pérez, Hugo Urbán
 Author-email: gabriellichu@gmail.com, info.prostaprog@gmail.com, carlosmoleracanals@gmail.com,pperezferre@gmail.com, hugourmaz@gmail.com
 Keywords: Python,Machine Learning
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: GPU :: NVIDIA CUDA :: 12
 Classifier: Intended Audience :: Education
@@ -23,15 +23,15 @@
 Requires-Dist: fastrlock>=0.8.2
 Requires-Dist: python-dateutil>=2.9.0.post0
 Requires-Dist: pytz>=2024.1
 Requires-Dist: six>=1.16.0
 Requires-Dist: tzdata>=2024.1
 Requires-Dist: matplotlib>=3.9.0
 Provides-Extra: gpu
-Requires-Dist: cupy-cuda12.x==13.1.0; extra == "gpu"
+Requires-Dist: cupy-cuda12x==13.1.0; extra == "gpu"
 
 # NeuroWeave
 <p align="center">
 <a href="https://git.io/typing-svg"><img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=30&duration=2000&pause=500&center=true&vCenter=true&multiline=true&repeat=false&random=false&width=800&height=100&lines=Interweaving+Intelligence;Where+Neurons+and+Networks+Connect" alt="Typing SVG" /></a>
 </p>
 
 ![Static Badge](https://img.shields.io/badge/Version-v1.0.0-green)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: neuroweave Version: 0.0.2 Summary: A small machine
+Metadata-Version: 2.1 Name: neuroweave Version: 0.0.3 Summary: A small machine
 learning library. Author: Gabriel Niculescu, Carlos Molera, Stanislav Gatin,
 Patricia PÃ©rez, Hugo UrbÃ¡n Author-email: gabriellichu@gmail.com,
 info.prostaprog@gmail.com, carlosmoleracanals@gmail.com,pperezferre@gmail.com,
 hugourmaz@gmail.com Keywords: Python,Machine Learning Classifier: Development
 Status :: 4 - Beta Classifier: Environment :: GPU :: NVIDIA CUDA :: 12
 Classifier: Intended Audience :: Education Classifier: Intended Audience ::
 Developers Classifier: Operating System :: Microsoft :: Windows Classifier:
@@ -10,15 +10,15 @@
 Python :: 3.12 Classifier: Topic :: Scientific/Engineering :: Artificial
 Intelligence Classifier: Topic :: Scientific/Engineering Requires-Python:
 >=3.12.0 Description-Content-Type: text/markdown License-File: LICENSE
 Requires-Dist: h5py>=3.11.0 Requires-Dist: numpy>=1.26.4 Requires-Dist:
 pandas>=2.2.2 Requires-Dist: fastrlock>=0.8.2 Requires-Dist: python-
 dateutil>=2.9.0.post0 Requires-Dist: pytz>=2024.1 Requires-Dist: six>=1.16.0
 Requires-Dist: tzdata>=2024.1 Requires-Dist: matplotlib>=3.9.0 Provides-Extra:
-gpu Requires-Dist: cupy-cuda12.x==13.1.0; extra == "gpu" # NeuroWeave
+gpu Requires-Dist: cupy-cuda12x==13.1.0; extra == "gpu" # NeuroWeave
                                  _[_T_y_p_i_n_g_ _S_V_G_]
 ![Static Badge](https://img.shields.io/badge/Version-v1.0.0-green) ![Static
 Badge](https://img.shields.io/badge/Colaboradores-5-blue) [Star Badge]![GitHub
 Repo stars](https://img.shields.io/github/stars/stas-gatin/NeuroWeave)
 NeuroWeave is a powerful and intuitive library for creating and training neural
 networks. With NeuroWeave, you can quickly build complex models, experiment
 with architectures, and adjust hyperparameters while maintaining control over
```

### Comparing `neuroweave-0.0.2/README.md` & `neuroweave-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `neuroweave-0.0.2/neuroweave.egg-info/PKG-INFO` & `neuroweave-0.0.3/neuroweave.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neuroweave
-Version: 0.0.2
+Version: 0.0.3
 Summary: A small machine learning library.
 Author: Gabriel Niculescu, Carlos Molera, Stanislav Gatin, Patricia Pérez, Hugo Urbán
 Author-email: gabriellichu@gmail.com, info.prostaprog@gmail.com, carlosmoleracanals@gmail.com,pperezferre@gmail.com, hugourmaz@gmail.com
 Keywords: Python,Machine Learning
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: GPU :: NVIDIA CUDA :: 12
 Classifier: Intended Audience :: Education
@@ -23,15 +23,15 @@
 Requires-Dist: fastrlock>=0.8.2
 Requires-Dist: python-dateutil>=2.9.0.post0
 Requires-Dist: pytz>=2024.1
 Requires-Dist: six>=1.16.0
 Requires-Dist: tzdata>=2024.1
 Requires-Dist: matplotlib>=3.9.0
 Provides-Extra: gpu
-Requires-Dist: cupy-cuda12.x==13.1.0; extra == "gpu"
+Requires-Dist: cupy-cuda12x==13.1.0; extra == "gpu"
 
 # NeuroWeave
 <p align="center">
 <a href="https://git.io/typing-svg"><img src="https://readme-typing-svg.demolab.com?font=Fira+Code&size=30&duration=2000&pause=500&center=true&vCenter=true&multiline=true&repeat=false&random=false&width=800&height=100&lines=Interweaving+Intelligence;Where+Neurons+and+Networks+Connect" alt="Typing SVG" /></a>
 </p>
 
 ![Static Badge](https://img.shields.io/badge/Version-v1.0.0-green)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: neuroweave Version: 0.0.2 Summary: A small machine
+Metadata-Version: 2.1 Name: neuroweave Version: 0.0.3 Summary: A small machine
 learning library. Author: Gabriel Niculescu, Carlos Molera, Stanislav Gatin,
 Patricia PÃ©rez, Hugo UrbÃ¡n Author-email: gabriellichu@gmail.com,
 info.prostaprog@gmail.com, carlosmoleracanals@gmail.com,pperezferre@gmail.com,
 hugourmaz@gmail.com Keywords: Python,Machine Learning Classifier: Development
 Status :: 4 - Beta Classifier: Environment :: GPU :: NVIDIA CUDA :: 12
 Classifier: Intended Audience :: Education Classifier: Intended Audience ::
 Developers Classifier: Operating System :: Microsoft :: Windows Classifier:
@@ -10,15 +10,15 @@
 Python :: 3.12 Classifier: Topic :: Scientific/Engineering :: Artificial
 Intelligence Classifier: Topic :: Scientific/Engineering Requires-Python:
 >=3.12.0 Description-Content-Type: text/markdown License-File: LICENSE
 Requires-Dist: h5py>=3.11.0 Requires-Dist: numpy>=1.26.4 Requires-Dist:
 pandas>=2.2.2 Requires-Dist: fastrlock>=0.8.2 Requires-Dist: python-
 dateutil>=2.9.0.post0 Requires-Dist: pytz>=2024.1 Requires-Dist: six>=1.16.0
 Requires-Dist: tzdata>=2024.1 Requires-Dist: matplotlib>=3.9.0 Provides-Extra:
-gpu Requires-Dist: cupy-cuda12.x==13.1.0; extra == "gpu" # NeuroWeave
+gpu Requires-Dist: cupy-cuda12x==13.1.0; extra == "gpu" # NeuroWeave
                                  _[_T_y_p_i_n_g_ _S_V_G_]
 ![Static Badge](https://img.shields.io/badge/Version-v1.0.0-green) ![Static
 Badge](https://img.shields.io/badge/Colaboradores-5-blue) [Star Badge]![GitHub
 Repo stars](https://img.shields.io/github/stars/stas-gatin/NeuroWeave)
 NeuroWeave is a powerful and intuitive library for creating and training neural
 networks. With NeuroWeave, you can quickly build complex models, experiment
 with architectures, and adjust hyperparameters while maintaining control over
```

### Comparing `neuroweave-0.0.2/neuroweave.egg-info/SOURCES.txt` & `neuroweave-0.0.3/neuroweave.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neuroweave-0.0.2/setup.py` & `neuroweave-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import codecs
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 with codecs.open(os.path.join(here, 'README.md'), encoding='utf-8') as fh:
     long_description = fh.read()
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = 'A small machine learning library.'
 LONG_DESCRIPTION = ('A Machine Learning library with the basic components necessary for building basic '
                     'Neural Network Models')
 
 setup(
     name='neuroweave',
     version=VERSION,
@@ -20,15 +20,15 @@
     description=DESCRIPTION,
     long_description_content_type='text/markdown',
     long_description=long_description,
     packages=find_packages(),
     install_requires=['h5py>=3.11.0', 'numpy>=1.26.4', 'pandas>=2.2.2', 'fastrlock>=0.8.2',
                       'python-dateutil>=2.9.0.post0', 'pytz>=2024.1', 'six>=1.16.0', 'tzdata>=2024.1',
                       'matplotlib>=3.9.0'],
-    extras_require={'GPU': ['cupy-cuda12.x==13.1.0']},
+    extras_require={'GPU': ['cupy-cuda12x==13.1.0']},
     python_requires='>=3.12.0',
     keywords=['Python', 'Machine Learning'],
     classifiers=[
         'Development Status :: 4 - Beta',
         'Environment :: GPU :: NVIDIA CUDA :: 12',
         'Intended Audience :: Education',
         'Intended Audience :: Developers',
```

### Comparing `neuroweave-0.0.2/weave/__init__.py` & `neuroweave-0.0.3/weave/__init__.py`

 * *Files identical despite different names*

### Comparing `neuroweave-0.0.2/weave/_utils/core.py` & `neuroweave-0.0.3/weave/_utils/core.py`

 * *Files identical despite different names*

### Comparing `neuroweave-0.0.2/weave/cuda/__init__.py` & `neuroweave-0.0.3/weave/cuda/__init__.py`

 * *Files identical despite different names*

### Comparing `neuroweave-0.0.2/weave/cuda/tools.py` & `neuroweave-0.0.3/weave/cuda/tools.py`

 * *Files identical despite different names*

### Comparing `neuroweave-0.0.2/weave/neuro_dataset/main.py` & `neuroweave-0.0.3/weave/neuro_dataset/main.py`

 * *Files identical despite different names*

### Comparing `neuroweave-0.0.2/weave/neuro_functions/functions.py` & `neuroweave-0.0.3/weave/neuro_functions/functions.py`

 * *Files identical despite different names*

### Comparing `neuroweave-0.0.2/weave/neuro_storage/loader.py` & `neuroweave-0.0.3/weave/neuro_storage/loader.py`

 * *Files identical despite different names*

### Comparing `neuroweave-0.0.2/weave/neuro_storage/saver.py` & `neuroweave-0.0.3/weave/neuro_storage/saver.py`

 * *Files identical despite different names*

### Comparing `neuroweave-0.0.2/weave/nn/modules/activations.py` & `neuroweave-0.0.3/weave/nn/modules/activations.py`

 * *Files identical despite different names*

### Comparing `neuroweave-0.0.2/weave/nn/modules/layer.py` & `neuroweave-0.0.3/weave/nn/modules/layer.py`

 * *Files identical despite different names*

### Comparing `neuroweave-0.0.2/weave/nn/modules/losses.py` & `neuroweave-0.0.3/weave/nn/modules/losses.py`

 * *Files identical despite different names*

### Comparing `neuroweave-0.0.2/weave/nn/modules/model.py` & `neuroweave-0.0.3/weave/nn/modules/model.py`

 * *Files identical despite different names*

### Comparing `neuroweave-0.0.2/weave/nn/optim/optimizers.py` & `neuroweave-0.0.3/weave/nn/optim/optimizers.py`

 * *Files identical despite different names*

### Comparing `neuroweave-0.0.2/weave/tensor.py` & `neuroweave-0.0.3/weave/tensor.py`

 * *Files identical despite different names*

### Comparing `neuroweave-0.0.2/weave/visualization/weave_weights.py` & `neuroweave-0.0.3/weave/visualization/weave_weights.py`

 * *Files identical despite different names*

