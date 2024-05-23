# Comparing `tmp/clore_pynvml-11.5.2.tar.gz` & `tmp/clore_pynvml-11.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clore_pynvml-11.5.2.tar", last modified: Thu May 23 13:20:19 2024, max compression
+gzip compressed data, was "clore_pynvml-11.5.3.tar", last modified: Thu May 23 13:23:16 2024, max compression
```

## Comparing `clore_pynvml-11.5.2.tar` & `clore_pynvml-11.5.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:20:19.904576 clore_pynvml-11.5.2/
--rw-r--r--   0 root         (0) root         (0)     1496 2023-02-15 03:22:12.000000 clore_pynvml-11.5.2/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)       27 2024-04-30 13:48:18.000000 clore_pynvml-11.5.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     7999 2024-05-23 13:20:19.904576 clore_pynvml-11.5.2/PKG-INFO
--rwxr-xr-x   0 root         (0) root         (0)     7169 2024-05-23 13:20:07.000000 clore_pynvml-11.5.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:20:19.904576 clore_pynvml-11.5.2/clore_pynvml.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7999 2024-05-23 13:20:19.000000 clore_pynvml-11.5.2/clore_pynvml.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      279 2024-05-23 13:20:19.000000 clore_pynvml-11.5.2/clore_pynvml.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-23 13:20:19.000000 clore_pynvml-11.5.2/clore_pynvml.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        7 2024-05-23 13:20:19.000000 clore_pynvml-11.5.2/clore_pynvml.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:20:19.904576 clore_pynvml-11.5.2/pynvml/
--rw-r--r--   0 root         (0) root         (0)      113 2023-02-15 03:22:12.000000 clore_pynvml-11.5.2/pynvml/__init__.py
--rw-r--r--   0 root         (0) root         (0)      498 2023-02-15 03:36:38.000000 clore_pynvml-11.5.2/pynvml/_version.py
--rw-r--r--   0 root         (0) root         (0)   170467 2024-05-23 12:43:17.000000 clore_pynvml-11.5.2/pynvml/nvml.py
--rw-r--r--   0 root         (0) root         (0)     1582 2024-05-23 13:20:07.000000 clore_pynvml-11.5.2/pynvml/setup.py
--rwxr-xr-x   0 root         (0) root         (0)   137578 2024-05-23 13:17:52.000000 clore_pynvml-11.5.2/pynvml/smi.py
--rw-r--r--   0 root         (0) root         (0)       77 2024-05-23 13:20:19.904576 clore_pynvml-11.5.2/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     1582 2024-05-23 13:20:07.000000 clore_pynvml-11.5.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:23:16.154182 clore_pynvml-11.5.3/
+-rw-r--r--   0 root         (0) root         (0)     1496 2023-02-15 03:22:12.000000 clore_pynvml-11.5.3/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)       33 2024-05-23 13:22:03.000000 clore_pynvml-11.5.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     7999 2024-05-23 13:23:16.154182 clore_pynvml-11.5.3/PKG-INFO
+-rwxr-xr-x   0 root         (0) root         (0)     7169 2024-05-23 13:23:11.000000 clore_pynvml-11.5.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:23:16.154182 clore_pynvml-11.5.3/clore_pynvml/
+-rw-r--r--   0 root         (0) root         (0)      113 2023-02-15 03:22:12.000000 clore_pynvml-11.5.3/clore_pynvml/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      498 2023-02-15 03:36:38.000000 clore_pynvml-11.5.3/clore_pynvml/_version.py
+-rw-r--r--   0 root         (0) root         (0)   170467 2024-05-23 12:43:17.000000 clore_pynvml-11.5.3/clore_pynvml/nvml.py
+-rw-r--r--   0 root         (0) root         (0)     1582 2024-05-23 13:23:11.000000 clore_pynvml-11.5.3/clore_pynvml/setup.py
+-rwxr-xr-x   0 root         (0) root         (0)   137578 2024-05-23 13:17:52.000000 clore_pynvml-11.5.3/clore_pynvml/smi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 13:23:16.154182 clore_pynvml-11.5.3/clore_pynvml.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7999 2024-05-23 13:23:16.000000 clore_pynvml-11.5.3/clore_pynvml.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      309 2024-05-23 13:23:16.000000 clore_pynvml-11.5.3/clore_pynvml.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-23 13:23:16.000000 clore_pynvml-11.5.3/clore_pynvml.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-05-23 13:23:16.000000 clore_pynvml-11.5.3/clore_pynvml.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       77 2024-05-23 13:23:16.154182 clore_pynvml-11.5.3/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     1582 2024-05-23 13:23:11.000000 clore_pynvml-11.5.3/setup.py
```

### Comparing `clore_pynvml-11.5.2/LICENSE.txt` & `clore_pynvml-11.5.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `clore_pynvml-11.5.2/PKG-INFO` & `clore_pynvml-11.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clore_pynvml
-Version: 11.5.2
+Version: 11.5.3
 Summary: Python Bindings for the NVIDIA Management Library
 Home-page: http://www.nvidia.com/
 Author: NVIDIA Corporation
 Author-email: rzamora@nvidia.com
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -227,10 +227,10 @@
     - Updated smi.py NVML_BRAND_NAMES
     - Aligned nvml.py with latest nvidia-ml-py deployment (11.495.46)
 -   Version 11.4.1
     - Fix comma bugs in nvml.py
 -   Version 11.5.0
     - Updated nvml.py to support CUDA 11.5 and CUDA 12
     - Aligned with latest nvidia-ml-py deployment (11.525.84)
--   Version 11.5.2 CLORE
+-   Version 11.5.3 CLORE
     - removed versioneer
     - fixed nvmlDeviceGetGpcClkMinMaxVfOffset, nvmlDeviceGetMemClkMinMaxVfOffset
```

### Comparing `clore_pynvml-11.5.2/README.md` & `clore_pynvml-11.5.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -205,10 +205,10 @@
     - Updated smi.py NVML_BRAND_NAMES
     - Aligned nvml.py with latest nvidia-ml-py deployment (11.495.46)
 -   Version 11.4.1
     - Fix comma bugs in nvml.py
 -   Version 11.5.0
     - Updated nvml.py to support CUDA 11.5 and CUDA 12
     - Aligned with latest nvidia-ml-py deployment (11.525.84)
--   Version 11.5.2 CLORE
+-   Version 11.5.3 CLORE
     - removed versioneer
     - fixed nvmlDeviceGetGpcClkMinMaxVfOffset, nvmlDeviceGetMemClkMinMaxVfOffset
```

### Comparing `clore_pynvml-11.5.2/clore_pynvml.egg-info/PKG-INFO` & `clore_pynvml-11.5.3/clore_pynvml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clore_pynvml
-Version: 11.5.2
+Version: 11.5.3
 Summary: Python Bindings for the NVIDIA Management Library
 Home-page: http://www.nvidia.com/
 Author: NVIDIA Corporation
 Author-email: rzamora@nvidia.com
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -227,10 +227,10 @@
     - Updated smi.py NVML_BRAND_NAMES
     - Aligned nvml.py with latest nvidia-ml-py deployment (11.495.46)
 -   Version 11.4.1
     - Fix comma bugs in nvml.py
 -   Version 11.5.0
     - Updated nvml.py to support CUDA 11.5 and CUDA 12
     - Aligned with latest nvidia-ml-py deployment (11.525.84)
--   Version 11.5.2 CLORE
+-   Version 11.5.3 CLORE
     - removed versioneer
     - fixed nvmlDeviceGetGpcClkMinMaxVfOffset, nvmlDeviceGetMemClkMinMaxVfOffset
```

### Comparing `clore_pynvml-11.5.2/pynvml/nvml.py` & `clore_pynvml-11.5.3/clore_pynvml/nvml.py`

 * *Files identical despite different names*

### Comparing `clore_pynvml-11.5.2/pynvml/setup.py` & `clore_pynvml-11.5.3/clore_pynvml/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # earlier versions don't support all classifiers
 #if version < '2.2.3':
 #    from distutils.dist import DistributionMetadata
 #    DistributionMetadata.classifiers = None
 #    DistributionMetadata.download_url = None
 
 setup(name='clore_pynvml',
-      version="11.5.2",
+      version="11.5.3",
       python_requires='>=3.6',
       description='Python Bindings for the NVIDIA Management Library',
       long_description=long_description,
       long_description_content_type='text/markdown',
       packages=find_packages(exclude=['notebooks', 'docs', 'tests']),
       package_data={'clore_pynvml': ['README.md','help_query_gpu.txt']},
       license="BSD",
```

### Comparing `clore_pynvml-11.5.2/pynvml/smi.py` & `clore_pynvml-11.5.3/clore_pynvml/smi.py`

 * *Files identical despite different names*

### Comparing `clore_pynvml-11.5.2/setup.py` & `clore_pynvml-11.5.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # earlier versions don't support all classifiers
 #if version < '2.2.3':
 #    from distutils.dist import DistributionMetadata
 #    DistributionMetadata.classifiers = None
 #    DistributionMetadata.download_url = None
 
 setup(name='clore_pynvml',
-      version="11.5.2",
+      version="11.5.3",
       python_requires='>=3.6',
       description='Python Bindings for the NVIDIA Management Library',
       long_description=long_description,
       long_description_content_type='text/markdown',
       packages=find_packages(exclude=['notebooks', 'docs', 'tests']),
       package_data={'clore_pynvml': ['README.md','help_query_gpu.txt']},
       license="BSD",
```

