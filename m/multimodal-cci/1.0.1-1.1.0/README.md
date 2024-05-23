# Comparing `tmp/multimodal_cci-1.0.1.tar.gz` & `tmp/multimodal_cci-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multimodal_cci-1.0.1.tar", last modified: Mon Feb 26 01:22:41 2024, max compression
+gzip compressed data, was "multimodal_cci-1.1.0.tar", last modified: Thu May 23 02:10:31 2024, max compression
```

## Comparing `multimodal_cci-1.0.1.tar` & `multimodal_cci-1.1.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 uqlhocke (1100037689) qris-uq  (60001)        0 2024-02-26 01:22:41.302882 multimodal_cci-1.0.1/
--rw-r--r--   0 uqlhocke (1100037689) qris-uq  (60001)     1525 2024-01-04 06:59:14.000000 multimodal_cci-1.0.1/LICENSE.txt
--rw-r--r--   0 uqlhocke (1100037689) qris-uq  (60001)        0 2024-01-18 02:27:43.000000 multimodal_cci-1.0.1/MANIFEST.in
--rw-r--r--   0 uqlhocke (1100037689) qris-uq  (60001)     5647 2024-02-26 01:22:41.302667 multimodal_cci-1.0.1/PKG-INFO
--rw-r--r--   0 uqlhocke (1100037689) qris-uq  (60001)     3141 2024-02-22 04:16:02.000000 multimodal_cci-1.0.1/README.md
--rw-r--r--   0 uqlhocke (1100037689) qris-uq  (60001)       85 2024-01-05 02:47:52.000000 multimodal_cci-1.0.1/pyproject.toml
--rw-r--r--   0 uqlhocke (1100037689) qris-uq  (60001)      982 2024-02-26 01:22:41.303536 multimodal_cci-1.0.1/setup.cfg
-drwxr-xr-x   0 uqlhocke (1100037689) qris-uq  (60001)        0 2024-02-26 01:22:41.290197 multimodal_cci-1.0.1/src/
-drwxr-xr-x   0 uqlhocke (1100037689) qris-uq  (60001)        0 2024-02-26 01:22:41.296214 multimodal_cci-1.0.1/src/multimodal_cci/
--rw-r--r--   0 uqlhocke (1100037689) qris-uq  (60001)      167 2024-02-26 01:22:23.000000 multimodal_cci-1.0.1/src/multimodal_cci/__init__.py
--rw-r--r--   0 uqlhocke (1100037689) qris-uq  (60001)    21331 2024-02-26 01:20:54.000000 multimodal_cci-1.0.1/src/multimodal_cci/analysis.py
--rw-r--r--   0 uqlhocke (1100037689) qris-uq  (60001)     6902 2024-02-23 02:12:31.000000 multimodal_cci-1.0.1/src/multimodal_cci/integration.py
--rw-r--r--   0 uqlhocke (1100037689) qris-uq  (60001)     7068 2024-02-09 05:06:57.000000 multimodal_cci-1.0.1/src/multimodal_cci/plot_helper.py
--rw-r--r--   0 uqlhocke (1100037689) qris-uq  (60001)    12006 2024-02-20 04:48:22.000000 multimodal_cci-1.0.1/src/multimodal_cci/plotting.py
--rw-r--r--   0 uqlhocke (1100037689) qris-uq  (60001)     3496 2024-02-20 04:54:41.000000 multimodal_cci-1.0.1/src/multimodal_cci/scoring.py
--rw-r--r--   0 uqlhocke (1100037689) qris-uq  (60001)     6199 2024-02-21 03:43:21.000000 multimodal_cci-1.0.1/src/multimodal_cci/tools.py
-drwxr-xr-x   0 uqlhocke (1100037689) qris-uq  (60001)        0 2024-02-26 01:22:41.298896 multimodal_cci-1.0.1/src/multimodal_cci.egg-info/
-drwxr-xr-x   0 uqlhocke (1100037689) qris-uq  (60001)        0 2024-02-26 01:22:41.301990 multimodal_cci-1.0.1/src/multimodal_cci.egg-info/.ipynb_checkpoints/
--rw-r--r--   0 uqlhocke (1100037689) qris-uq  (60001)     2281 2024-01-05 02:48:52.000000 multimodal_cci-1.0.1/src/multimodal_cci.egg-info/.ipynb_checkpoints/PKG-INFO-checkpoint
--rw-r--r--   0 uqlhocke (1100037689) qris-uq  (60001)      393 2024-01-05 02:48:52.000000 multimodal_cci-1.0.1/src/multimodal_cci.egg-info/.ipynb_checkpoints/SOURCES-checkpoint.txt
--rw-r--r--   0 uqlhocke (1100037689) qris-uq  (60001)        1 2024-01-05 02:48:52.000000 multimodal_cci-1.0.1/src/multimodal_cci.egg-info/.ipynb_checkpoints/dependency_links-checkpoint.txt
--rw-r--r--   0 uqlhocke (1100037689) qris-uq  (60001)       32 2024-01-05 02:48:52.000000 multimodal_cci-1.0.1/src/multimodal_cci.egg-info/.ipynb_checkpoints/requires-checkpoint.txt
--rw-r--r--   0 uqlhocke (1100037689) qris-uq  (60001)       15 2024-01-05 02:48:52.000000 multimodal_cci-1.0.1/src/multimodal_cci.egg-info/.ipynb_checkpoints/top_level-checkpoint.txt
--rw-r--r--   0 uqlhocke (1100037689) qris-uq  (60001)     5647 2024-02-26 01:22:41.296997 multimodal_cci-1.0.1/src/multimodal_cci.egg-info/PKG-INFO
--rw-r--r--   0 uqlhocke (1100037689) qris-uq  (60001)      845 2024-02-26 01:22:41.297420 multimodal_cci-1.0.1/src/multimodal_cci.egg-info/SOURCES.txt
--rw-r--r--   0 uqlhocke (1100037689) qris-uq  (60001)        1 2024-02-26 01:22:41.297999 multimodal_cci-1.0.1/src/multimodal_cci.egg-info/dependency_links.txt
--rw-r--r--   0 uqlhocke (1100037689) qris-uq  (60001)      152 2024-02-26 01:22:41.298519 multimodal_cci-1.0.1/src/multimodal_cci.egg-info/requires.txt
--rw-r--r--   0 uqlhocke (1100037689) qris-uq  (60001)       15 2024-02-26 01:22:41.298969 multimodal_cci-1.0.1/src/multimodal_cci.egg-info/top_level.txt
+drwxr-xr-x   0 uqlhocke (1100037689) qris-uq  (60001)        0 2024-05-23 02:10:31.885646 multimodal_cci-1.1.0/
+-rw-r--r--   0 uqlhocke (1100037689) qris-uq  (60001)     1525 2024-03-05 02:02:14.000000 multimodal_cci-1.1.0/LICENSE.txt
+-rw-r--r--   0 uqlhocke (1100037689) qris-uq  (60001)        0 2024-03-05 02:02:14.000000 multimodal_cci-1.1.0/MANIFEST.in
+-rw-r--r--   0 uqlhocke (1100037689) qris-uq  (60001)     5593 2024-05-23 02:10:31.885450 multimodal_cci-1.1.0/PKG-INFO
+-rw-r--r--   0 uqlhocke (1100037689) qris-uq  (60001)     3087 2024-03-22 01:57:30.000000 multimodal_cci-1.1.0/README.md
+-rw-r--r--   0 uqlhocke (1100037689) qris-uq  (60001)       85 2024-03-05 02:02:14.000000 multimodal_cci-1.1.0/pyproject.toml
+-rw-r--r--   0 uqlhocke (1100037689) qris-uq  (60001)      982 2024-05-23 02:10:31.886077 multimodal_cci-1.1.0/setup.cfg
+drwxr-xr-x   0 uqlhocke (1100037689) qris-uq  (60001)        0 2024-05-23 02:10:31.870690 multimodal_cci-1.1.0/src/
+drwxr-xr-x   0 uqlhocke (1100037689) qris-uq  (60001)        0 2024-05-23 02:10:31.878288 multimodal_cci-1.1.0/src/multimodal_cci/
+-rw-r--r--   0 uqlhocke (1100037689) qris-uq  (60001)      168 2024-04-16 04:38:24.000000 multimodal_cci-1.1.0/src/multimodal_cci/__init__.py
+-rw-r--r--   0 uqlhocke (1100037689) qris-uq  (60001)    23578 2024-05-23 02:08:00.000000 multimodal_cci-1.1.0/src/multimodal_cci/analysis.py
+-rw-r--r--   0 uqlhocke (1100037689) qris-uq  (60001)    10198 2024-04-22 06:47:06.000000 multimodal_cci-1.1.0/src/multimodal_cci/integration.py
+-rw-r--r--   0 uqlhocke (1100037689) qris-uq  (60001)     7068 2024-03-05 02:02:14.000000 multimodal_cci-1.1.0/src/multimodal_cci/plot_helper.py
+-rw-r--r--   0 uqlhocke (1100037689) qris-uq  (60001)    17908 2024-05-23 01:47:03.000000 multimodal_cci-1.1.0/src/multimodal_cci/plotting.py
+-rw-r--r--   0 uqlhocke (1100037689) qris-uq  (60001)     3496 2024-03-05 02:02:14.000000 multimodal_cci-1.1.0/src/multimodal_cci/scoring.py
+-rw-r--r--   0 uqlhocke (1100037689) qris-uq  (60001)     8889 2024-04-17 06:13:41.000000 multimodal_cci-1.1.0/src/multimodal_cci/tools.py
+drwxr-xr-x   0 uqlhocke (1100037689) qris-uq  (60001)        0 2024-05-23 02:10:31.881376 multimodal_cci-1.1.0/src/multimodal_cci.egg-info/
+drwxr-xr-x   0 uqlhocke (1100037689) qris-uq  (60001)        0 2024-05-23 02:10:31.884800 multimodal_cci-1.1.0/src/multimodal_cci.egg-info/.ipynb_checkpoints/
+-rw-r--r--   0 uqlhocke (1100037689) qris-uq  (60001)     2281 2024-03-05 02:02:14.000000 multimodal_cci-1.1.0/src/multimodal_cci.egg-info/.ipynb_checkpoints/PKG-INFO-checkpoint
+-rw-r--r--   0 uqlhocke (1100037689) qris-uq  (60001)      393 2024-03-05 02:02:14.000000 multimodal_cci-1.1.0/src/multimodal_cci.egg-info/.ipynb_checkpoints/SOURCES-checkpoint.txt
+-rw-r--r--   0 uqlhocke (1100037689) qris-uq  (60001)        1 2024-03-05 02:02:14.000000 multimodal_cci-1.1.0/src/multimodal_cci.egg-info/.ipynb_checkpoints/dependency_links-checkpoint.txt
+-rw-r--r--   0 uqlhocke (1100037689) qris-uq  (60001)       32 2024-03-05 02:02:14.000000 multimodal_cci-1.1.0/src/multimodal_cci.egg-info/.ipynb_checkpoints/requires-checkpoint.txt
+-rw-r--r--   0 uqlhocke (1100037689) qris-uq  (60001)       15 2024-03-05 02:02:14.000000 multimodal_cci-1.1.0/src/multimodal_cci.egg-info/.ipynb_checkpoints/top_level-checkpoint.txt
+-rw-r--r--   0 uqlhocke (1100037689) qris-uq  (60001)     5593 2024-05-23 02:10:31.878999 multimodal_cci-1.1.0/src/multimodal_cci.egg-info/PKG-INFO
+-rw-r--r--   0 uqlhocke (1100037689) qris-uq  (60001)      845 2024-05-23 02:10:31.879437 multimodal_cci-1.1.0/src/multimodal_cci.egg-info/SOURCES.txt
+-rw-r--r--   0 uqlhocke (1100037689) qris-uq  (60001)        1 2024-05-23 02:10:31.880275 multimodal_cci-1.1.0/src/multimodal_cci.egg-info/dependency_links.txt
+-rw-r--r--   0 uqlhocke (1100037689) qris-uq  (60001)      152 2024-05-23 02:10:31.881004 multimodal_cci-1.1.0/src/multimodal_cci.egg-info/requires.txt
+-rw-r--r--   0 uqlhocke (1100037689) qris-uq  (60001)       15 2024-05-23 02:10:31.881474 multimodal_cci-1.1.0/src/multimodal_cci.egg-info/top_level.txt
```

### Comparing `multimodal_cci-1.0.1/LICENSE.txt` & `multimodal_cci-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `multimodal_cci-1.0.1/PKG-INFO` & `multimodal_cci-1.1.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multimodal_cci
-Version: 1.0.1
+Version: 1.1.0
 Summary: A Python package for processing multi-modal CCI data
 Home-page: https://github.com/BiomedicalMachineLearning/MultimodalCCI
 Author: Genomics and Machine Learning lab
 Author-email: l.hockey@uq.edu.au
 Project-URL: Bug Tracker, https://github.com/BiomedicalMachineLearning/MultimodalCCI/issues
 Project-URL: repository, https://github.com/BiomedicalMachineLearning/MultimodalCCI
 Classifier: Programming Language :: Python :: 3
@@ -20,88 +20,75 @@
 Requires-Dist: scikit-learn>=1.3.0
 Requires-Dist: scipy>=1.9.1
 Requires-Dist: tqdm>=4.66.1
 Requires-Dist: gseapy>=1.1.1
 Requires-Dist: scanpy>=1.9.0
 Requires-Dist: seaborn>=0.11.2
 
+# MMCCI: Multimodal Cell-Cell Interaction Integrative Analysis of Single Cell and Spatial Data
 
-<!-- <table align="center">
+<table align="center">
   <tr>
     <td>
       <b>Package</b>
     </td>
     <td>
-      <a href="https://pypi.python.org/pypi//">
-      <img src="https://img.shields.io/pypi/v/.svg" alt="PyPI Version">
+      <a href="https://pypi.python.org/pypi/multimodal-cci/">
+      <img src="https://img.shields.io/pypi/v/multimodal-cci.svg" alt="PyPI Version">
       </a>
-      <a href="https://pepy.tech/project/">
-      <img src="https://static.pepy.tech/personalized-badge/?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads"
+      <a href="https://pepy.tech/project/multimodal-cci">
+      <img src="https://static.pepy.tech/personalized-badge/multimodal-cci?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads"
         alt="PyPI downloads">
-      </a>
-      <a href="https://anaconda.org/conda-forge/">
-      <img src="https://anaconda.org/conda-forge//badges/downloads.svg" alt="Conda downloads">
-      </a>
-      <a href="https://anaconda.org/conda-forge/">
-      <img src="https://anaconda.org/conda-forge//badges/downloads.svg" alt="Install">
-      </a>
-    </td>
-  </tr>
-  <tr>
-    <td>
-      <b>Documentation</b>
-    </td>
-    <td>
-      <a href="https://multimodalcci.readthedocs/en/latest/">
-      <img src="https://multimodalcci.readthedocs.org/projects//badge/?version=latest" alt="Documentation Status">
-      </a>
     </td>
   </tr>
   <tr>
     <td>
      <b>Paper</b>
     </td>
     <td>
-      <a href="https://doi.org/"><img src="https://zenodo.org/badge/DOI/.svg"
+      <a href="https://doi.org/10.1101/2023.05.14.540710"><img src="https://zenodo.org/badge/DOI/10.1101/2023.05.14.540710.svg"
         alt="DOI"></a>
     </td>
   </tr>
   <tr>
     <td>
       <b>License</b>
     </td>
     <td>
       <a href="https://github.com/BiomedicalMachineLearning/MultimodalCCI/blob/main/LICENSE.txt"><img src="https://img.shields.io/badge/License-BSD-blue.svg"
         alt="LICENSE"></a>
     </td>
   </tr>
-</table> -->
-
-
-# MMCCI: Multimodal Cell-Cell Interaction Integration, Analysis, and Visualisation
-
+</table>
+        
 **MMCCI** is a fast and lightweight Python package for integrating and visualizing CCI networks within and between multiple modalities at the level of the individual LR pair. It works on **scRNA-seq** and **spatial transcriptomics** data samples that have been processed through the following CCI algorithms:
 1. stLearn
 2. CellChat
 3. CellPhoneDB
 4. NATMI
 5. Squidpy
 
 ## Getting Started
 
 ### Installation
 
-Coming soon
+MMCCI can be installed with `pip`
+
+```
+pip install multimodal-cci
+```
+
 
 ### Documentation
 
-Documentation and Tutorials are available at our **Read the Docs** page (coming soon).
+Documentation and Tutorials are available here and we are commited to maintaining the software and addressing issues raised by users.
 
-- There is a tutorial notebook [here](examples/brain_aging_example.ipynb)
-- To understand how to load CCI results from different tools, look at this notebook [here](example/loading_CCI_results.ipynb)
+- There is a brain aging tutorial notebook [here](examples/brain_aging_example.ipynb)
+- There is a melanoma tutorial notebook [here](examples/melanoma_example.ipynb)
+- To understand how to load CCI results from different tools, look at this notebook [here](examples/loading_CCI_results.ipynb)
 
 ## CCI Integration
 
 MMCCI allows users to integrate multiple CCI results together, both:
 1. Samples from a single modality (eg. Visium)
 2. Samples from multiple modalities (eg. Visium, Xenium and CosMX)
 
@@ -120,15 +107,18 @@
 
 ### Pipeline Diagram
 
 ![MMCCI Pipeline](docs/images/pipeline.png)
 
 ## Citing MMCCI
 
-If you have used MMCCI in your research, please consider citing us: (coming soon).
+If you have used MMCCI in your research, please consider citing us: 
+```
+Hockey, L., Mulay, O., Xiong, Z., Khosrotehrani, K., Nefzger, C. M., & Nguyen, Q. (2024). MMCCI: Multimodal Cell-Cell Interaction Integrative Analysis of Single Cell and Spatial Data. bioRxiv. doi:10.1101/2024.02.28.582639
+```
 
 
 
 
 BSD License
 
 Copyright (c) 2024, Genomics and Machine Learning lab
```

#### html2text {}

```diff
@@ -1,54 +1,64 @@
-Metadata-Version: 2.1 Name: multimodal_cci Version: 1.0.1 Summary: A Python
+Metadata-Version: 2.1 Name: multimodal_cci Version: 1.1.0 Summary: A Python
 package for processing multi-modal CCI data Home-page: https://github.com/
 BiomedicalMachineLearning/MultimodalCCI Author: Genomics and Machine Learning
 lab Author-email: l.hockey@uq.edu.au Project-URL: Bug Tracker, https://
 github.com/BiomedicalMachineLearning/MultimodalCCI/issues Project-URL:
 repository, https://github.com/BiomedicalMachineLearning/MultimodalCCI
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9 Description-Content-Type: text/markdown License-File:
 LICENSE.txt Requires-Dist: numpy>=1.24.0 Requires-Dist: pandas>=2.1.4 Requires-
 Dist: networkx>=3.2.1 Requires-Dist: matplotlib>=3.8.2 Requires-Dist: scikit-
 learn>=1.3.0 Requires-Dist: scipy>=1.9.1 Requires-Dist: tqdm>=4.66.1 Requires-
 Dist: gseapy>=1.1.1 Requires-Dist: scanpy>=1.9.0 Requires-Dist: seaborn>=0.11.2
-# MMCCI: Multimodal Cell-Cell Interaction Integration, Analysis, and
-Visualisation **MMCCI** is a fast and lightweight Python package for
-integrating and visualizing CCI networks within and between multiple modalities
-at the level of the individual LR pair. It works on **scRNA-seq** and **spatial
+# MMCCI: Multimodal Cell-Cell Interaction Integrative Analysis of Single Cell
+and Spatial Data
+                    PPaacckkaaggee _[_P_y_P_I_ _V_e_r_s_i_o_n_]_[_P_y_P_I_ _d_o_w_n_l_o_a_d_s_]
+                    PPaappeerr   _[_D_O_I_]
+                    LLiicceennssee _[_L_I_C_E_N_S_E_]
+**MMCCI** is a fast and lightweight Python package for integrating and
+visualizing CCI networks within and between multiple modalities at the level of
+the individual LR pair. It works on **scRNA-seq** and **spatial
 transcriptomics** data samples that have been processed through the following
 CCI algorithms: 1. stLearn 2. CellChat 3. CellPhoneDB 4. NATMI 5. Squidpy ##
-Getting Started ### Installation Coming soon ### Documentation Documentation
-and Tutorials are available at our **Read the Docs** page (coming soon). -
-There is a tutorial notebook [here](examples/brain_aging_example.ipynb) - To
-understand how to load CCI results from different tools, look at this notebook
-[here](example/loading_CCI_results.ipynb) ## CCI Integration MMCCI allows users
-to integrate multiple CCI results together, both: 1. Samples from a single
-modality (eg. Visium) 2. Samples from multiple modalities (eg. Visium, Xenium
-and CosMX) ![Integration Method](docs/images/integration_method.png) ## CCI
-Analysis MMCCI provides multiple useful analyses that can be run on the
-integrated networks or from a single sample: 1. Network comparison between
-groups with permutation testing 2. CLustering of LR pairs with similar networks
-3. Clustering of spots/cells with similar interaction scores 4. Sender-receiver
-LR querying 5. GSEA pathway analysis ![Downstream Analyses](docs/images/
-analyses.png) ### Pipeline Diagram ![MMCCI Pipeline](docs/images/pipeline.png)
-## Citing MMCCI If you have used MMCCI in your research, please consider citing
-us: (coming soon). BSD License Copyright (c) 2024, Genomics and Machine
-Learning lab All rights reserved. Redistribution and use in source and binary
-forms, with or without modification, are permitted provided that the following
-conditions are met: * Redistributions of source code must retain the above
-copyright notice, this list of conditions and the following disclaimer. *
-Redistributions in binary form must reproduce the above copyright notice, this
-list of conditions and the following disclaimer in the documentation and/or
-other materials provided with the distribution. * Neither the name of the
-copyright holder nor the names of its contributors may be used to endorse or
-promote products derived from this software without specific prior written
-permission. THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
-"AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO,
-THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
-ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
-LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
-CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE
-GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION)
-HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT
-LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT
-OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+Getting Started ### Installation MMCCI can be installed with `pip` ``` pip
+install multimodal-cci ``` ### Documentation Documentation and Tutorials are
+available here and we are commited to maintaining the software and addressing
+issues raised by users. - There is a brain aging tutorial notebook [here]
+(examples/brain_aging_example.ipynb) - There is a melanoma tutorial notebook
+[here](examples/melanoma_example.ipynb) - To understand how to load CCI results
+from different tools, look at this notebook [here](examples/
+loading_CCI_results.ipynb) ## CCI Integration MMCCI allows users to integrate
+multiple CCI results together, both: 1. Samples from a single modality (eg.
+Visium) 2. Samples from multiple modalities (eg. Visium, Xenium and CosMX) !
+[Integration Method](docs/images/integration_method.png) ## CCI Analysis MMCCI
+provides multiple useful analyses that can be run on the integrated networks or
+from a single sample: 1. Network comparison between groups with permutation
+testing 2. CLustering of LR pairs with similar networks 3. Clustering of spots/
+cells with similar interaction scores 4. Sender-receiver LR querying 5. GSEA
+pathway analysis ![Downstream Analyses](docs/images/analyses.png) ### Pipeline
+Diagram ![MMCCI Pipeline](docs/images/pipeline.png) ## Citing MMCCI If you have
+used MMCCI in your research, please consider citing us: ``` Hockey, L., Mulay,
+O., Xiong, Z., Khosrotehrani, K., Nefzger, C. M., & Nguyen, Q. (2024). MMCCI:
+Multimodal Cell-Cell Interaction Integrative Analysis of Single Cell and
+Spatial Data. bioRxiv. doi:10.1101/2024.02.28.582639 ``` BSD License Copyright
+(c) 2024, Genomics and Machine Learning lab All rights reserved. Redistribution
+and use in source and binary forms, with or without modification, are permitted
+provided that the following conditions are met: * Redistributions of source
+code must retain the above copyright notice, this list of conditions and the
+following disclaimer. * Redistributions in binary form must reproduce the above
+copyright notice, this list of conditions and the following disclaimer in the
+documentation and/or other materials provided with the distribution. * Neither
+the name of the copyright holder nor the names of its contributors may be used
+to endorse or promote products derived from this software without specific
+prior written permission. THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS
+AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT
+NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A
+PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
+CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
+EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT
+OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING
+IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY
+OF SUCH DAMAGE.
```

### Comparing `multimodal_cci-1.0.1/README.md` & `multimodal_cci-1.1.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,81 +1,68 @@
+# MMCCI: Multimodal Cell-Cell Interaction Integrative Analysis of Single Cell and Spatial Data
 
-<!-- <table align="center">
+<table align="center">
   <tr>
     <td>
       <b>Package</b>
     </td>
     <td>
-      <a href="https://pypi.python.org/pypi//">
-      <img src="https://img.shields.io/pypi/v/.svg" alt="PyPI Version">
+      <a href="https://pypi.python.org/pypi/multimodal-cci/">
+      <img src="https://img.shields.io/pypi/v/multimodal-cci.svg" alt="PyPI Version">
       </a>
-      <a href="https://pepy.tech/project/">
-      <img src="https://static.pepy.tech/personalized-badge/?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads"
+      <a href="https://pepy.tech/project/multimodal-cci">
+      <img src="https://static.pepy.tech/personalized-badge/multimodal-cci?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads"
         alt="PyPI downloads">
-      </a>
-      <a href="https://anaconda.org/conda-forge/">
-      <img src="https://anaconda.org/conda-forge//badges/downloads.svg" alt="Conda downloads">
-      </a>
-      <a href="https://anaconda.org/conda-forge/">
-      <img src="https://anaconda.org/conda-forge//badges/downloads.svg" alt="Install">
-      </a>
-    </td>
-  </tr>
-  <tr>
-    <td>
-      <b>Documentation</b>
-    </td>
-    <td>
-      <a href="https://multimodalcci.readthedocs/en/latest/">
-      <img src="https://multimodalcci.readthedocs.org/projects//badge/?version=latest" alt="Documentation Status">
-      </a>
     </td>
   </tr>
   <tr>
     <td>
      <b>Paper</b>
     </td>
     <td>
-      <a href="https://doi.org/"><img src="https://zenodo.org/badge/DOI/.svg"
+      <a href="https://doi.org/10.1101/2023.05.14.540710"><img src="https://zenodo.org/badge/DOI/10.1101/2023.05.14.540710.svg"
         alt="DOI"></a>
     </td>
   </tr>
   <tr>
     <td>
       <b>License</b>
     </td>
     <td>
       <a href="https://github.com/BiomedicalMachineLearning/MultimodalCCI/blob/main/LICENSE.txt"><img src="https://img.shields.io/badge/License-BSD-blue.svg"
         alt="LICENSE"></a>
     </td>
   </tr>
-</table> -->
-
-
-# MMCCI: Multimodal Cell-Cell Interaction Integration, Analysis, and Visualisation
-
+</table>
+        
 **MMCCI** is a fast and lightweight Python package for integrating and visualizing CCI networks within and between multiple modalities at the level of the individual LR pair. It works on **scRNA-seq** and **spatial transcriptomics** data samples that have been processed through the following CCI algorithms:
 1. stLearn
 2. CellChat
 3. CellPhoneDB
 4. NATMI
 5. Squidpy
 
 ## Getting Started
 
 ### Installation
 
-Coming soon
+MMCCI can be installed with `pip`
+
+```
+pip install multimodal-cci
+```
+
 
 ### Documentation
 
-Documentation and Tutorials are available at our **Read the Docs** page (coming soon).
+Documentation and Tutorials are available here and we are commited to maintaining the software and addressing issues raised by users.
 
-- There is a tutorial notebook [here](examples/brain_aging_example.ipynb)
-- To understand how to load CCI results from different tools, look at this notebook [here](example/loading_CCI_results.ipynb)
+- There is a brain aging tutorial notebook [here](examples/brain_aging_example.ipynb)
+- There is a melanoma tutorial notebook [here](examples/melanoma_example.ipynb)
+- To understand how to load CCI results from different tools, look at this notebook [here](examples/loading_CCI_results.ipynb)
 
 ## CCI Integration
 
 MMCCI allows users to integrate multiple CCI results together, both:
 1. Samples from a single modality (eg. Visium)
 2. Samples from multiple modalities (eg. Visium, Xenium and CosMX)
 
@@ -94,9 +81,12 @@
 
 ### Pipeline Diagram
 
 ![MMCCI Pipeline](docs/images/pipeline.png)
 
 ## Citing MMCCI
 
-If you have used MMCCI in your research, please consider citing us: (coming soon).
+If you have used MMCCI in your research, please consider citing us: 
+```
+Hockey, L., Mulay, O., Xiong, Z., Khosrotehrani, K., Nefzger, C. M., & Nguyen, Q. (2024). MMCCI: Multimodal Cell-Cell Interaction Integrative Analysis of Single Cell and Spatial Data. bioRxiv. doi:10.1101/2024.02.28.582639
+```
```

#### html2text {}

```diff
@@ -1,22 +1,31 @@
-# MMCCI: Multimodal Cell-Cell Interaction Integration, Analysis, and
-Visualisation **MMCCI** is a fast and lightweight Python package for
-integrating and visualizing CCI networks within and between multiple modalities
-at the level of the individual LR pair. It works on **scRNA-seq** and **spatial
+# MMCCI: Multimodal Cell-Cell Interaction Integrative Analysis of Single Cell
+and Spatial Data
+                    PPaacckkaaggee _[_P_y_P_I_ _V_e_r_s_i_o_n_]_[_P_y_P_I_ _d_o_w_n_l_o_a_d_s_]
+                    PPaappeerr   _[_D_O_I_]
+                    LLiicceennssee _[_L_I_C_E_N_S_E_]
+**MMCCI** is a fast and lightweight Python package for integrating and
+visualizing CCI networks within and between multiple modalities at the level of
+the individual LR pair. It works on **scRNA-seq** and **spatial
 transcriptomics** data samples that have been processed through the following
 CCI algorithms: 1. stLearn 2. CellChat 3. CellPhoneDB 4. NATMI 5. Squidpy ##
-Getting Started ### Installation Coming soon ### Documentation Documentation
-and Tutorials are available at our **Read the Docs** page (coming soon). -
-There is a tutorial notebook [here](examples/brain_aging_example.ipynb) - To
-understand how to load CCI results from different tools, look at this notebook
-[here](example/loading_CCI_results.ipynb) ## CCI Integration MMCCI allows users
-to integrate multiple CCI results together, both: 1. Samples from a single
-modality (eg. Visium) 2. Samples from multiple modalities (eg. Visium, Xenium
-and CosMX) ![Integration Method](docs/images/integration_method.png) ## CCI
-Analysis MMCCI provides multiple useful analyses that can be run on the
-integrated networks or from a single sample: 1. Network comparison between
-groups with permutation testing 2. CLustering of LR pairs with similar networks
-3. Clustering of spots/cells with similar interaction scores 4. Sender-receiver
-LR querying 5. GSEA pathway analysis ![Downstream Analyses](docs/images/
-analyses.png) ### Pipeline Diagram ![MMCCI Pipeline](docs/images/pipeline.png)
-## Citing MMCCI If you have used MMCCI in your research, please consider citing
-us: (coming soon).
+Getting Started ### Installation MMCCI can be installed with `pip` ``` pip
+install multimodal-cci ``` ### Documentation Documentation and Tutorials are
+available here and we are commited to maintaining the software and addressing
+issues raised by users. - There is a brain aging tutorial notebook [here]
+(examples/brain_aging_example.ipynb) - There is a melanoma tutorial notebook
+[here](examples/melanoma_example.ipynb) - To understand how to load CCI results
+from different tools, look at this notebook [here](examples/
+loading_CCI_results.ipynb) ## CCI Integration MMCCI allows users to integrate
+multiple CCI results together, both: 1. Samples from a single modality (eg.
+Visium) 2. Samples from multiple modalities (eg. Visium, Xenium and CosMX) !
+[Integration Method](docs/images/integration_method.png) ## CCI Analysis MMCCI
+provides multiple useful analyses that can be run on the integrated networks or
+from a single sample: 1. Network comparison between groups with permutation
+testing 2. CLustering of LR pairs with similar networks 3. Clustering of spots/
+cells with similar interaction scores 4. Sender-receiver LR querying 5. GSEA
+pathway analysis ![Downstream Analyses](docs/images/analyses.png) ### Pipeline
+Diagram ![MMCCI Pipeline](docs/images/pipeline.png) ## Citing MMCCI If you have
+used MMCCI in your research, please consider citing us: ``` Hockey, L., Mulay,
+O., Xiong, Z., Khosrotehrani, K., Nefzger, C. M., & Nguyen, Q. (2024). MMCCI:
+Multimodal Cell-Cell Interaction Integrative Analysis of Single Cell and
+Spatial Data. bioRxiv. doi:10.1101/2024.02.28.582639 ```
```

### Comparing `multimodal_cci-1.0.1/setup.cfg` & `multimodal_cci-1.1.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = multimodal_cci
-version = 1.0.1
+version = 1.1.0
 author = Genomics and Machine Learning lab
 author_email = l.hockey@uq.edu.au
 description = A Python package for processing multi-modal CCI data
 long_description = file: README.md, LICENSE.txt
 long_description_content_type = text/markdown
 url = https://github.com/BiomedicalMachineLearning/MultimodalCCI
 project_urls =
```

### Comparing `multimodal_cci-1.0.1/src/multimodal_cci/analysis.py` & `multimodal_cci-1.1.0/src/multimodal_cci/analysis.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import gseapy as gp
 import seaborn as sns
 import statistics
 import subprocess
 import umap
 import matplotlib.pyplot as plt
 import importlib.resources
+import anndata as ad
 
 from matplotlib import pyplot as plt
 from matplotlib.colors import LinearSegmentedColormap
 
 from gseapy import barplot, dotplot
 from tqdm import tqdm
 from scipy.spatial.distance import pdist, squareform
@@ -385,14 +386,24 @@
         LR.obs["leiden"] = LR.obs["leiden"].astype("int64")
         sc.pl.spatial(
             LR,
             img_key="hires",
             color="leiden",
             size=1.5,
             cmap=cmap)
+        sc.pp.pca(LR)
+        sc.pp.highly_variable_genes(LR, flavor="seurat", n_top_genes=2000)
+        sc.pp.neighbors(LR, use_rep="X_pca", n_neighbors=15)
+        sc.tl.umap(LR)
+        sc.pl.umap(
+            LR,
+            color="leiden",
+            cmap=cmap,
+            legend_loc=None  # Remove the legend
+        )
 
         sample.obs["LR_Cluster"] = LR.obs["leiden"]
         barplot_data = (
             sample
             .obs.groupby(["cell_type", "LR_Cluster"])
             .size()
             .reset_index(name="Count")
@@ -616,7 +627,69 @@
         )
 
         # ax = dotplot(enr.res2d, cmap="viridis_r", size=10, figsize=(3, 5))
 
         # ax = barplot(enr.res2d, figsize=(4, 5), color="darkred")
 
     return enr.results
+
+
+def pathway_subset(sample, gsea_results, terms, strict=False):
+    """Subsets a sample to only include interactions between genes in a set of
+    pathways.
+
+    Args:
+        sample (dict): The sample to subset.
+        gsea_results (pd.DataFrame): The GSEA results to use to subset the sample.
+        terms (list): The terms to subset the sample with.
+        strict (bool): Whether to only include interactions between genes in the
+        same pathway.
+
+    Returns:
+        dict: The subsetted sample.
+    """
+
+    genes = []
+    grouped = {}
+
+    for term in terms:
+        filtered_df = gsea_results[gsea_results['Term'] == term]
+        gene_list = filtered_df['Genes'].tolist()
+
+        for gene in gene_list:
+            genes.extend(gene.lower().split(";"))
+
+    for key in sample.keys():
+        lig, rec = key.lower().split("_")
+        if strict:
+            if lig in genes and rec in genes:
+                grouped[key] = sample[key]
+        else:
+            if lig in genes or rec in genes:
+                grouped[key] = sample[key]
+
+    return grouped
+
+
+def add_lr_module_score(sample, lr_list, key_name="score"):
+    """Adds a module score to an AnnData object run through stLearn based on the
+    interactions in a list of ligand-receptor pairs.
+
+    Args:
+        sample (AnnData): The AnnData object to add the score to. Must be processed
+        through stLearn.
+        lr_list (list): The list of ligand-receptor pairs to use.
+        key_name (str): The key to use for the score.
+
+    Returns:
+        AnnData: The AnnData object with the module score added.
+    """
+
+    lr_counts = pd.DataFrame(sample.obsm['lr_sig_scores'])
+    lr_counts.index = sample.obs.index
+    lr_counts.columns = sample.uns['lr_summary'].index
+
+    adata = ad.AnnData(lr_counts)
+    sc.tl.score_genes(adata, gene_list=lr_list)
+    sample.obs[key_name] = adata.obs['score']
+
+    return sample
```

### Comparing `multimodal_cci-1.0.1/src/multimodal_cci/integration.py` & `multimodal_cci-1.1.0/src/multimodal_cci/integration.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 import numpy as np
 import pandas as pd
 import matplotlib.pyplot as plt
 
+from scipy import stats
+
 from . import scoring as sc
+from . import tools as tl
 
 
 def normalise_within_tech(samples, sample_sizes, target=None):
     """Normalizes LR matrices within a list of samples to a target sample based on
     number of spots to account for differences in sample size.
 
     Args:
@@ -28,21 +31,21 @@
     for i, sample in enumerate(samples):
         for lr, matrix in sample.items():
             samples[i][lr] = matrix * (target / sample_sizes[i])
 
     return samples
 
 
-def get_majority_lr_pairs(samples, equal_to=False):
-    """Identifies the LR pairs present in a majority of samples.
+def get_lr_pairs(samples, method=">=50%"):
+    """Identifies the LR pairs present in a list of samples according to the given method.
 
     Args:
         samples (list): A list of dictionaries of LR matrices
-        equal_to (bool) (optional): If True, includes LR pairs present in exactly half
-        of the samples. Defaults to False.
+        method (str) (optional): The method to use for identifying LR pairs. Options are
+        "all", ">=50%", ">50%", and "any". Defaults to ">=50%".
 
     Returns:
         list: A list of LR pairs that are present in a majority of samples
     """
 
     if not isinstance(samples, list):
         raise ValueError("Samples must be a list of dicts of LR matrices.")
@@ -52,20 +55,27 @@
 
     for sample in samples:
         for lr_pair, matrix in sample.items():
             if sum(sum(matrix.values)) != 0:
                 lr_pairs_counts[lr_pair] = lr_pairs_counts.setdefault(lr_pair, 0) + 1
 
     for lr_pair, count in lr_pairs_counts.items():
-        if equal_to:
+        if method == "all":
+            if count == len(samples):
+                lr_pairs.append(lr_pair)
+        elif method == ">=50%":
             if count >= len(samples) / 2:
                 lr_pairs.append(lr_pair)
-        else:
+        elif method == ">50%":
             if count > len(samples) / 2:
                 lr_pairs.append(lr_pair)
+        elif method == "any":
+            lr_pairs.append(lr_pair)
+        else:
+            raise ValueError("Method must be 'all', '>=50%', '>50%', or 'any'.")
 
     return lr_pairs
 
 
 def subset_samples(samples, lr_pairs):
     """Subsets each sample in samples to only contain the LR pairs in lr_pairs.
 
@@ -126,42 +136,35 @@
         for lr, df in samples[tech].items():
             factor = max(tech_counts) / tech_counts[tech]
             samples[tech][lr] = df * factor
 
     return samples
 
 
-def integrate_samples(samples, all_lr_pairs=False):
+def integrate_samples(samples, method=">=50%"):
     """Integrates matrices from different technologies.
 
     Args:
         samples (list): A list of samples with different technologies.
-        all_lr_pairs (bool) (optional): If True and two samples are used, use all the LR
-        pairs from either sample. Defaults to False.
+        method (str) (optional): The method to use for identifying LR pairs. Options are
+        "all", ">=50%", ">50%", and "any". Defaults to ">=50%".
 
     Returns:
         dict: A dictionary where keys are LR pairs and values are the integrated
         matrices.
     """
 
     if not isinstance(samples, list):
         raise ValueError("Samples must be a list of dicts of LR matrices.")
 
     integrated = {}
     lr_matrices = {}
 
-    if len(samples) == 2:
-        if all_lr_pairs:
-            lr_pairs = get_majority_lr_pairs(samples, equal_to=True)
-        else:
-            lr_pairs = get_majority_lr_pairs(samples, equal_to=False)
-
-    elif len(samples) > 2:
-        lr_pairs = sorted(get_majority_lr_pairs(samples, equal_to=True))
-
+    if len(samples) >= 2:
+        lr_pairs = sorted(get_lr_pairs(samples, method=method))
     else:
         raise ValueError("Integration needs at least two samples")
 
     for i in range(len(lr_pairs)):
         lr = lr_pairs[i]
 
         for tech in range(len(samples)):
@@ -214,7 +217,104 @@
     if total is None:
         return None
 
     total = total / total.sum().sum()
     total = total.fillna(0)
 
     return total
+
+
+def correct_pvals_matrix(dataframes, method="stouffer"):
+    """Corrects p-values across a list of pandas DataFrames.
+
+    Args:
+        dataframes (list): A list of pandas DataFrames with p vals to combine.
+        method (str) (optional): The method to use for combining p-values. Options are
+        "stouffer" and "fisher". Defaults to "stouffer".
+
+    Returns:
+        pd.DataFrame: A DataFrame with corrected p-values.
+    """
+
+    result_df = dataframes[0]
+
+    for i in range(len(dataframes)):
+        dataframes[i], result_df = tl.align_dataframes(
+            dataframes[i], result_df, fill_value=np.NaN)
+
+    for i in range(len(dataframes)):
+        dataframes[i], result_df = tl.align_dataframes(
+            dataframes[i], result_df, fill_value=np.NaN)
+
+    result_df = result_df.astype(np.float64)
+    for i, row in result_df.iterrows():
+        for j in row.index:
+            values = [df.loc[i, j] for df in dataframes]
+            values = [
+                0.00000000001 if x == 0 else (
+                    0.9999999999 if x == 1 else x) for x in values]
+            values = [x for x in values if not np.isnan(x)]
+            result_df.loc[i, j] = stats.combine_pvalues(values, method=method, )[1]
+
+    return result_df
+
+
+def integrate_p_vals(samples, method="stouffer"):
+    """Integrates p-values from different samples.
+
+    Args:
+        samples (list): A list of dictionaries of LR matrices.
+        method (str) (optional): The method to use for combining p-values. Options
+        are "stouffer" and "fisher". Defaults to "stouffer".
+
+    Returns:
+        dict: A dictionary where keys are LR pairs and values are the integrated
+        p-values.
+    """
+
+    if not isinstance(samples, list):
+        raise ValueError("Samples must be a list of dicts of LR matrices.")
+
+    integrated = {}
+    lr_matrices = {}
+
+    lr_pairs = set()
+    for sample in samples:
+        lr_pairs.update(sample.keys())
+    lr_pairs = list(lr_pairs)
+
+    for i in range(len(lr_pairs)):
+        lr = lr_pairs[i]
+
+        for tech in range(len(samples)):
+            if lr in samples[tech]:
+                if lr in lr_matrices:
+                    lr_matrices[lr].append(samples[tech][lr])
+                else:
+                    lr_matrices[lr] = [samples[tech][lr]]
+
+    for lr, matrices in lr_matrices.items():
+        integrated[lr] = correct_pvals_matrix(matrices, method=method)
+
+    return integrated
+
+
+def remove_insignificant(sample, p_vals, cutoff=0.05):
+    """Removes insignificant interactions from a sample based on p-values.
+
+    Args:
+        sample (dict): A sample containing matrices for different LR pairs.
+        p_vals (dict): A dictionary of p-values for the LR pairs in the sample.
+
+    Returns:
+        dict: A dictionary of matrices with insignificant interactions set to 0.
+    """
+
+    corrected_sample = {}
+    for lr, matrix in sample.items():
+        for i, row in matrix.iterrows():
+            for j in row.index:
+                if p_vals[lr].loc[i, j] > cutoff:
+                    matrix.loc[i, j] = 0
+        corrected_sample[lr] = matrix
+
+    return corrected_sample
```

### Comparing `multimodal_cci-1.0.1/src/multimodal_cci/plot_helper.py` & `multimodal_cci-1.1.0/src/multimodal_cci/plot_helper.py`

 * *Files identical despite different names*

### Comparing `multimodal_cci-1.0.1/src/multimodal_cci/scoring.py` & `multimodal_cci-1.1.0/src/multimodal_cci/scoring.py`

 * *Files identical despite different names*

### Comparing `multimodal_cci-1.0.1/src/multimodal_cci/tools.py` & `multimodal_cci-1.1.0/src/multimodal_cci/tools.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 import pandas as pd
 import numpy as np
 import scanpy as sc
 
 
-def align_dataframes(m1, m2):
+def align_dataframes(m1, m2, fill_value=0):
     """Aligns two DataFrames by matching their indices and columns, filling missing
     values with 0.
 
     Args:
         m1, m2 (pd.DataFrame): The DataFrames to align.
 
     Returns:
         tuple: A tuple of the aligned DataFrames.
     """
 
-    m1, m2 = m1.align(m2, fill_value=0)
+    m1, m2 = m1.align(m2, fill_value=fill_value)
 
     columns = sorted(set(m1.columns) | set(m2.columns))
-    m1 = m1.reindex(columns, fill_value=0)
-    m2 = m2.reindex(columns, fill_value=0)
+    m1 = m1.reindex(columns, fill_value=fill_value)
+    m2 = m2.reindex(columns, fill_value=fill_value)
 
     rows = sorted(set(m1.index) | set(m2.index))
-    m1 = m1.reindex(rows, fill_value=0)
-    m2 = m2.reindex(rows, fill_value=0)
+    m1 = m1.reindex(rows, fill_value=fill_value)
+    m2 = m2.reindex(rows, fill_value=fill_value)
 
     return m1, m2
 
 
 def rename_celltypes(sample, replacements):
     """Renames cell types in a sample.
 
@@ -48,116 +48,172 @@
             index=replacements,
             columns=replacements,
             inplace=True)
 
     return renamed
 
 
-def read_stLearn(path):
+def read_stLearn(path, key="cell_type", return_adata=False):
     """Reads a stLearn ligand-receptor analysis output and converts it to a dictionary
     of LR matrices that can be used with the multimodal cci functions.
 
     Args:
         path (str): The path to the stLearn ligand-receptor analysis output.
+        key (str) (optional): The key in adata.obs that was used for CCI. Defaults to
+            "cell_type".
+        return_adata (bool) (optional): Whether to return the AnnData object as well.
+            Defaults to False.
 
     Returns:
-        dict: A dictionary of LR matrices.
-        int: The number of cells or spots in the dataset.
+        dict: The n_spots, lr_scores, lr_pvals, and AnnData (optional).
     """
 
     adata = sc.read_h5ad(path)
 
-    return adata.uns['per_lr_cci_cell_type'], adata.shape[0]
+    if return_adata:
+        out = {
+            "n_spots": adata.shape[0],
+            "lr_scores": adata.uns[f"per_lr_cci_raw_{key}"],
+            "lr_pvals": adata.uns[f"per_lr_cci_pvals_{key}"],
+            "adata": adata
+        }
+    else:
+        out = {
+            "n_spots": adata.shape[0],
+            "lr_scores": adata.uns[f"per_lr_cci_raw_{key}"],
+            "lr_pvals": adata.uns[f"per_lr_cci_pvals_{key}"]
+        }
 
+    return out
 
-def read_CellPhoneDB(path):
+
+def read_CellPhoneDB(means_path, pvals_path):
     """Reads a CellPhoneDB interaction scores txt file and converts it to a dictionary
     of LR matrices that can be used with the multimodal cci functions.
 
     Args:
-        path (str): the path to the interaction scores txt file.
+        means_path (str): Path to the means txt file.
+        pvals_path (str): Path to the pvals txt file.
 
     Returns:
-        dict: A dictionary of LR matrices.
+        dict: The LR scores and p_vals
     """
 
-    cp_obj = pd.read_csv(path, delimiter="\t")
+    cp_obj = pd.read_csv(means_path, delimiter="\t")
+    lr_dict = {}
+    for ind in cp_obj.index:
+
+        key = cp_obj["interacting_pair"][ind]
 
-    sample = {}
+        val = cp_obj.iloc[ind, cp_obj.columns.get_loc("classification") + 1:]
+        val = pd.DataFrame({"Index": val.index, "Value": val.values})
+        val[["Row", "Col"]] = val["Index"].str.split("|", expand=True)
+        val = val.drop("Index", axis=1)
+        val = val.pivot(index="Row", columns="Col", values="Value")
+        val = val.rename_axis(None, axis=1).rename_axis(None)
+        lr_dict[key] = val
 
+    cp_obj = pd.read_csv(pvals_path, delimiter="\t")
+    p_vals_dict = {}
     for ind in cp_obj.index:
 
         key = cp_obj["interacting_pair"][ind]
 
         val = cp_obj.iloc[ind, cp_obj.columns.get_loc("classification") + 1:]
         val = pd.DataFrame({"Index": val.index, "Value": val.values})
         val[["Row", "Col"]] = val["Index"].str.split("|", expand=True)
         val = val.drop("Index", axis=1)
         val = val.pivot(index="Row", columns="Col", values="Value")
         val = val.rename_axis(None, axis=1).rename_axis(None)
+        val = val.fillna(1)
+        p_vals_dict[key] = val
 
-        sample[key] = val
+    out = {
+        "lr_scores": lr_dict,
+        "lr_pvals": p_vals_dict
+    }
 
-    return sample
+    return out
 
 
 def read_Squidpy(result):
     """Reads a Squidpy ligand-receptor analysis output and converts it to a dictionary
     of LR matrices that can be used with the multimodal cci functions.
 
     Args:
         result (dict): The output from squidpy.gr.ligrec.
 
     Returns:
-        dict: A dictionary of LR matrices.
+        dict: The LR scores and p_vals.
     """
 
     lr_dict = {}
     pvals = pd.DataFrame(result["pvalues"])
 
     cci_names = np.array([col[0] + "--" + col[1] for col in pvals.columns])
     cell_type_set = np.unique([col[0] for col in pvals.columns])
 
     for i, row in enumerate(pvals.index):
 
         int_matrix = np.zeros((len(cell_type_set), len(cell_type_set)))
         lr_ = "_".join(list(row))
-
-        # Getting sig CCIs for this lr #
-        lr_pvals = np.array(pvals.values[i, :])
-        sig_bool = lr_pvals < 0.05
-        lr_ccis = cci_names[sig_bool]
+        lr_ccis = cci_names
         lig = list(row)[0]
         rec = list(row)[1]
         for j, cci in enumerate(lr_ccis):
             c1, c2 = cci.split("--")
             row = np.where(cell_type_set == c1)[0][0]
             col = np.where(cell_type_set == c2)[0][0]
             int_matrix[row, col] = result["means"][c1][c2][lig][rec]
 
         lr_dict[lr_] = pd.DataFrame(
             int_matrix, index=cell_type_set, columns=cell_type_set
         )
 
-    return lr_dict
+    pvals_dict = {}
+
+    for i, row in enumerate(pvals.index):
+
+        int_matrix = np.zeros((len(cell_type_set), len(cell_type_set)))
+        lr_ = '_'.join(list(row))
+        lr_ccis = cci_names
+        lig = list(row)[0]
+        rec = list(row)[1]
+        for j, cci in enumerate(lr_ccis):
+            c1, c2 = cci.split('--')
+            row = np.where(cell_type_set == c1)[0][0]
+            col = np.where(cell_type_set == c2)[0][0]
+            int_matrix[row, col] = result['pvalues'][c1][c2][lig][rec]
+
+        df = pd.DataFrame(int_matrix, index=cell_type_set, columns=cell_type_set)
+        df = df.fillna(1)
+        pvals_dict[lr_] = df
+
+    out = {
+        "lr_scores": lr_dict,
+        "lr_pvals": pvals_dict
+    }
+
+    return out
 
 
 def read_CellChat(path):
     """Reads a CellChat ligand-receptor analysis output (cellchat@dr) and converts it to
     a dictionary of LR matrices that can be used with the multimodal cci functions.
 
     Args:
         path (str): The output from cellchat@dr.
 
     Returns:
-        dict: A dictionary of LR matrices.
+        dict: The LR scores and p_vals
     """
 
     result = pd.read_csv(path)
     lr_dict = {}
+    pvals_dict = {}
 
     cell_type_set = np.unique(np.concatenate([result["source"], result["target"]]))
 
     for i in result.index:
         lr_ = result['interaction_name'][i]
         if lr_ not in lr_dict.keys():
             int_matrix = np.zeros((len(cell_type_set), len(cell_type_set)))
@@ -167,15 +223,36 @@
         col = np.where(cell_type_set == result["target"][i])[0][0]
         int_matrix[row, col] = result["prob"][i]
 
         lr_dict[lr_] = pd.DataFrame(
             int_matrix, index=cell_type_set, columns=cell_type_set
         )
 
-    return lr_dict
+    for i in result.index:
+        lr_ = result['interaction_name'][i]
+        if lr_ not in lr_dict.keys():
+            int_matrix = np.zeros((len(cell_type_set), len(cell_type_set)))
+        else:
+            int_matrix = lr_dict[lr_].values
+        row = np.where(cell_type_set == result["source"][i])[0][0]
+        col = np.where(cell_type_set == result["target"][i])[0][0]
+        int_matrix[row, col] = result["pval"][i]
+
+        df = pd.DataFrame(
+            int_matrix, index=cell_type_set, columns=cell_type_set
+        )
+        df = df.fillna(1)
+        pvals_dict[lr_] = df
+
+    out = {
+        "lr_scores": lr_dict,
+        "lr_pvals": pvals_dict
+    }
+
+    return out
 
 
 def read_NATMI(path):
     """Reads a NATMI ligand-receptor analysis output (Edges_lrc2p.csv) and converts it
     to a dictionary of LR matrices that can be used with the multimodal cci functions.
 
     Args:
```

### Comparing `multimodal_cci-1.0.1/src/multimodal_cci.egg-info/.ipynb_checkpoints/PKG-INFO-checkpoint` & `multimodal_cci-1.1.0/src/multimodal_cci.egg-info/.ipynb_checkpoints/PKG-INFO-checkpoint`

 * *Files identical despite different names*

### Comparing `multimodal_cci-1.0.1/src/multimodal_cci.egg-info/PKG-INFO` & `multimodal_cci-1.1.0/src/multimodal_cci.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multimodal_cci
-Version: 1.0.1
+Version: 1.1.0
 Summary: A Python package for processing multi-modal CCI data
 Home-page: https://github.com/BiomedicalMachineLearning/MultimodalCCI
 Author: Genomics and Machine Learning lab
 Author-email: l.hockey@uq.edu.au
 Project-URL: Bug Tracker, https://github.com/BiomedicalMachineLearning/MultimodalCCI/issues
 Project-URL: repository, https://github.com/BiomedicalMachineLearning/MultimodalCCI
 Classifier: Programming Language :: Python :: 3
@@ -20,88 +20,75 @@
 Requires-Dist: scikit-learn>=1.3.0
 Requires-Dist: scipy>=1.9.1
 Requires-Dist: tqdm>=4.66.1
 Requires-Dist: gseapy>=1.1.1
 Requires-Dist: scanpy>=1.9.0
 Requires-Dist: seaborn>=0.11.2
 
+# MMCCI: Multimodal Cell-Cell Interaction Integrative Analysis of Single Cell and Spatial Data
 
-<!-- <table align="center">
+<table align="center">
   <tr>
     <td>
       <b>Package</b>
     </td>
     <td>
-      <a href="https://pypi.python.org/pypi//">
-      <img src="https://img.shields.io/pypi/v/.svg" alt="PyPI Version">
+      <a href="https://pypi.python.org/pypi/multimodal-cci/">
+      <img src="https://img.shields.io/pypi/v/multimodal-cci.svg" alt="PyPI Version">
       </a>
-      <a href="https://pepy.tech/project/">
-      <img src="https://static.pepy.tech/personalized-badge/?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads"
+      <a href="https://pepy.tech/project/multimodal-cci">
+      <img src="https://static.pepy.tech/personalized-badge/multimodal-cci?period=total&units=international_system&left_color=grey&right_color=orange&left_text=Downloads"
         alt="PyPI downloads">
-      </a>
-      <a href="https://anaconda.org/conda-forge/">
-      <img src="https://anaconda.org/conda-forge//badges/downloads.svg" alt="Conda downloads">
-      </a>
-      <a href="https://anaconda.org/conda-forge/">
-      <img src="https://anaconda.org/conda-forge//badges/downloads.svg" alt="Install">
-      </a>
-    </td>
-  </tr>
-  <tr>
-    <td>
-      <b>Documentation</b>
-    </td>
-    <td>
-      <a href="https://multimodalcci.readthedocs/en/latest/">
-      <img src="https://multimodalcci.readthedocs.org/projects//badge/?version=latest" alt="Documentation Status">
-      </a>
     </td>
   </tr>
   <tr>
     <td>
      <b>Paper</b>
     </td>
     <td>
-      <a href="https://doi.org/"><img src="https://zenodo.org/badge/DOI/.svg"
+      <a href="https://doi.org/10.1101/2023.05.14.540710"><img src="https://zenodo.org/badge/DOI/10.1101/2023.05.14.540710.svg"
         alt="DOI"></a>
     </td>
   </tr>
   <tr>
     <td>
       <b>License</b>
     </td>
     <td>
       <a href="https://github.com/BiomedicalMachineLearning/MultimodalCCI/blob/main/LICENSE.txt"><img src="https://img.shields.io/badge/License-BSD-blue.svg"
         alt="LICENSE"></a>
     </td>
   </tr>
-</table> -->
-
-
-# MMCCI: Multimodal Cell-Cell Interaction Integration, Analysis, and Visualisation
-
+</table>
+        
 **MMCCI** is a fast and lightweight Python package for integrating and visualizing CCI networks within and between multiple modalities at the level of the individual LR pair. It works on **scRNA-seq** and **spatial transcriptomics** data samples that have been processed through the following CCI algorithms:
 1. stLearn
 2. CellChat
 3. CellPhoneDB
 4. NATMI
 5. Squidpy
 
 ## Getting Started
 
 ### Installation
 
-Coming soon
+MMCCI can be installed with `pip`
+
+```
+pip install multimodal-cci
+```
+
 
 ### Documentation
 
-Documentation and Tutorials are available at our **Read the Docs** page (coming soon).
+Documentation and Tutorials are available here and we are commited to maintaining the software and addressing issues raised by users.
 
-- There is a tutorial notebook [here](examples/brain_aging_example.ipynb)
-- To understand how to load CCI results from different tools, look at this notebook [here](example/loading_CCI_results.ipynb)
+- There is a brain aging tutorial notebook [here](examples/brain_aging_example.ipynb)
+- There is a melanoma tutorial notebook [here](examples/melanoma_example.ipynb)
+- To understand how to load CCI results from different tools, look at this notebook [here](examples/loading_CCI_results.ipynb)
 
 ## CCI Integration
 
 MMCCI allows users to integrate multiple CCI results together, both:
 1. Samples from a single modality (eg. Visium)
 2. Samples from multiple modalities (eg. Visium, Xenium and CosMX)
 
@@ -120,15 +107,18 @@
 
 ### Pipeline Diagram
 
 ![MMCCI Pipeline](docs/images/pipeline.png)
 
 ## Citing MMCCI
 
-If you have used MMCCI in your research, please consider citing us: (coming soon).
+If you have used MMCCI in your research, please consider citing us: 
+```
+Hockey, L., Mulay, O., Xiong, Z., Khosrotehrani, K., Nefzger, C. M., & Nguyen, Q. (2024). MMCCI: Multimodal Cell-Cell Interaction Integrative Analysis of Single Cell and Spatial Data. bioRxiv. doi:10.1101/2024.02.28.582639
+```
 
 
 
 
 BSD License
 
 Copyright (c) 2024, Genomics and Machine Learning lab
```

#### html2text {}

```diff
@@ -1,54 +1,64 @@
-Metadata-Version: 2.1 Name: multimodal_cci Version: 1.0.1 Summary: A Python
+Metadata-Version: 2.1 Name: multimodal_cci Version: 1.1.0 Summary: A Python
 package for processing multi-modal CCI data Home-page: https://github.com/
 BiomedicalMachineLearning/MultimodalCCI Author: Genomics and Machine Learning
 lab Author-email: l.hockey@uq.edu.au Project-URL: Bug Tracker, https://
 github.com/BiomedicalMachineLearning/MultimodalCCI/issues Project-URL:
 repository, https://github.com/BiomedicalMachineLearning/MultimodalCCI
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9 Description-Content-Type: text/markdown License-File:
 LICENSE.txt Requires-Dist: numpy>=1.24.0 Requires-Dist: pandas>=2.1.4 Requires-
 Dist: networkx>=3.2.1 Requires-Dist: matplotlib>=3.8.2 Requires-Dist: scikit-
 learn>=1.3.0 Requires-Dist: scipy>=1.9.1 Requires-Dist: tqdm>=4.66.1 Requires-
 Dist: gseapy>=1.1.1 Requires-Dist: scanpy>=1.9.0 Requires-Dist: seaborn>=0.11.2
-# MMCCI: Multimodal Cell-Cell Interaction Integration, Analysis, and
-Visualisation **MMCCI** is a fast and lightweight Python package for
-integrating and visualizing CCI networks within and between multiple modalities
-at the level of the individual LR pair. It works on **scRNA-seq** and **spatial
+# MMCCI: Multimodal Cell-Cell Interaction Integrative Analysis of Single Cell
+and Spatial Data
+                    PPaacckkaaggee _[_P_y_P_I_ _V_e_r_s_i_o_n_]_[_P_y_P_I_ _d_o_w_n_l_o_a_d_s_]
+                    PPaappeerr   _[_D_O_I_]
+                    LLiicceennssee _[_L_I_C_E_N_S_E_]
+**MMCCI** is a fast and lightweight Python package for integrating and
+visualizing CCI networks within and between multiple modalities at the level of
+the individual LR pair. It works on **scRNA-seq** and **spatial
 transcriptomics** data samples that have been processed through the following
 CCI algorithms: 1. stLearn 2. CellChat 3. CellPhoneDB 4. NATMI 5. Squidpy ##
-Getting Started ### Installation Coming soon ### Documentation Documentation
-and Tutorials are available at our **Read the Docs** page (coming soon). -
-There is a tutorial notebook [here](examples/brain_aging_example.ipynb) - To
-understand how to load CCI results from different tools, look at this notebook
-[here](example/loading_CCI_results.ipynb) ## CCI Integration MMCCI allows users
-to integrate multiple CCI results together, both: 1. Samples from a single
-modality (eg. Visium) 2. Samples from multiple modalities (eg. Visium, Xenium
-and CosMX) ![Integration Method](docs/images/integration_method.png) ## CCI
-Analysis MMCCI provides multiple useful analyses that can be run on the
-integrated networks or from a single sample: 1. Network comparison between
-groups with permutation testing 2. CLustering of LR pairs with similar networks
-3. Clustering of spots/cells with similar interaction scores 4. Sender-receiver
-LR querying 5. GSEA pathway analysis ![Downstream Analyses](docs/images/
-analyses.png) ### Pipeline Diagram ![MMCCI Pipeline](docs/images/pipeline.png)
-## Citing MMCCI If you have used MMCCI in your research, please consider citing
-us: (coming soon). BSD License Copyright (c) 2024, Genomics and Machine
-Learning lab All rights reserved. Redistribution and use in source and binary
-forms, with or without modification, are permitted provided that the following
-conditions are met: * Redistributions of source code must retain the above
-copyright notice, this list of conditions and the following disclaimer. *
-Redistributions in binary form must reproduce the above copyright notice, this
-list of conditions and the following disclaimer in the documentation and/or
-other materials provided with the distribution. * Neither the name of the
-copyright holder nor the names of its contributors may be used to endorse or
-promote products derived from this software without specific prior written
-permission. THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS
-"AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO,
-THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
-ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE
-LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
-CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE
-GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION)
-HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT
-LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT
-OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+Getting Started ### Installation MMCCI can be installed with `pip` ``` pip
+install multimodal-cci ``` ### Documentation Documentation and Tutorials are
+available here and we are commited to maintaining the software and addressing
+issues raised by users. - There is a brain aging tutorial notebook [here]
+(examples/brain_aging_example.ipynb) - There is a melanoma tutorial notebook
+[here](examples/melanoma_example.ipynb) - To understand how to load CCI results
+from different tools, look at this notebook [here](examples/
+loading_CCI_results.ipynb) ## CCI Integration MMCCI allows users to integrate
+multiple CCI results together, both: 1. Samples from a single modality (eg.
+Visium) 2. Samples from multiple modalities (eg. Visium, Xenium and CosMX) !
+[Integration Method](docs/images/integration_method.png) ## CCI Analysis MMCCI
+provides multiple useful analyses that can be run on the integrated networks or
+from a single sample: 1. Network comparison between groups with permutation
+testing 2. CLustering of LR pairs with similar networks 3. Clustering of spots/
+cells with similar interaction scores 4. Sender-receiver LR querying 5. GSEA
+pathway analysis ![Downstream Analyses](docs/images/analyses.png) ### Pipeline
+Diagram ![MMCCI Pipeline](docs/images/pipeline.png) ## Citing MMCCI If you have
+used MMCCI in your research, please consider citing us: ``` Hockey, L., Mulay,
+O., Xiong, Z., Khosrotehrani, K., Nefzger, C. M., & Nguyen, Q. (2024). MMCCI:
+Multimodal Cell-Cell Interaction Integrative Analysis of Single Cell and
+Spatial Data. bioRxiv. doi:10.1101/2024.02.28.582639 ``` BSD License Copyright
+(c) 2024, Genomics and Machine Learning lab All rights reserved. Redistribution
+and use in source and binary forms, with or without modification, are permitted
+provided that the following conditions are met: * Redistributions of source
+code must retain the above copyright notice, this list of conditions and the
+following disclaimer. * Redistributions in binary form must reproduce the above
+copyright notice, this list of conditions and the following disclaimer in the
+documentation and/or other materials provided with the distribution. * Neither
+the name of the copyright holder nor the names of its contributors may be used
+to endorse or promote products derived from this software without specific
+prior written permission. THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS
+AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT
+NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A
+PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR
+CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
+EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT
+OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
+CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING
+IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY
+OF SUCH DAMAGE.
```

### Comparing `multimodal_cci-1.0.1/src/multimodal_cci.egg-info/SOURCES.txt` & `multimodal_cci-1.1.0/src/multimodal_cci.egg-info/SOURCES.txt`

 * *Files identical despite different names*

