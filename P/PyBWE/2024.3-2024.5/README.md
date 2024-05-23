# Comparing `tmp/PyBWE-2024.3.tar.gz` & `tmp/pybwe-2024.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyBWE-2024.3.tar", last modified: Thu Mar  7 13:02:39 2024, max compression
+gzip compressed data, was "pybwe-2024.5.tar", last modified: Thu May 23 00:20:34 2024, max compression
```

## Comparing `PyBWE-2024.3.tar` & `pybwe-2024.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 13:02:39.867996 PyBWE-2024.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-03-07 13:02:27.000000 PyBWE-2024.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10341 2024-03-07 13:02:39.867996 PyBWE-2024.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9570 2024-03-07 13:02:27.000000 PyBWE-2024.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-07 13:02:39.867996 PyBWE-2024.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      912 2024-03-07 13:02:27.000000 PyBWE-2024.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 13:02:39.863997 PyBWE-2024.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 13:02:39.867996 PyBWE-2024.3/src/PyBWE/
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-03-07 13:02:27.000000 PyBWE-2024.3/src/PyBWE/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-03-07 13:02:27.000000 PyBWE-2024.3/src/PyBWE/function_BWE.py
--rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-03-07 13:02:27.000000 PyBWE-2024.3/src/PyBWE/function_ar_extrapolation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-03-07 13:02:27.000000 PyBWE-2024.3/src/PyBWE/function_burg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 13:02:39.867996 PyBWE-2024.3/src/PyBWE.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10341 2024-03-07 13:02:39.000000 PyBWE-2024.3/src/PyBWE.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-03-07 13:02:39.000000 PyBWE-2024.3/src/PyBWE.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-07 13:02:39.000000 PyBWE-2024.3/src/PyBWE.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-07 13:02:39.000000 PyBWE-2024.3/src/PyBWE.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-07 13:02:39.000000 PyBWE-2024.3/src/PyBWE.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-07 13:02:39.000000 PyBWE-2024.3/src/PyBWE.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 13:02:39.867996 PyBWE-2024.3/src/PyPBWE/
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-03-07 13:02:27.000000 PyBWE-2024.3/src/PyPBWE/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-03-07 13:02:27.000000 PyBWE-2024.3/src/PyPBWE/function_PBWE.py
--rw-r--r--   0 runner    (1001) docker     (127)     4149 2024-03-07 13:02:27.000000 PyBWE-2024.3/src/PyPBWE/function_polar_burg.py
--rw-r--r--   0 runner    (1001) docker     (127)     5099 2024-03-07 13:02:27.000000 PyBWE-2024.3/src/PyPBWE/function_polar_extrapolation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-07 13:02:39.867996 PyBWE-2024.3/src/PySSBWE/
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-03-07 13:02:27.000000 PyBWE-2024.3/src/PySSBWE/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-03-07 13:02:27.000000 PyBWE-2024.3/src/PySSBWE/function_AIC.py
--rw-r--r--   0 runner    (1001) docker     (127)     4915 2024-03-07 13:02:27.000000 PyBWE-2024.3/src/PySSBWE/function_SSBWE.py
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-03-07 13:02:27.000000 PyBWE-2024.3/src/PySSBWE/function_statespace_extrapolation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-03-07 13:02:27.000000 PyBWE-2024.3/src/PySSBWE/function_statespace_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-03-07 13:02:27.000000 PyBWE-2024.3/src/PySSBWE/function_statespace_properties.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 00:20:34.738926 pybwe-2024.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-23 00:20:20.000000 pybwe-2024.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10439 2024-05-23 00:20:34.738926 pybwe-2024.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9668 2024-05-23 00:20:20.000000 pybwe-2024.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 00:20:34.738926 pybwe-2024.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-05-23 00:20:20.000000 pybwe-2024.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 00:20:34.734926 pybwe-2024.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 00:20:34.734926 pybwe-2024.5/src/PyBWE/
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-23 00:20:20.000000 pybwe-2024.5/src/PyBWE/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-05-23 00:20:20.000000 pybwe-2024.5/src/PyBWE/function_BWE.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-05-23 00:20:20.000000 pybwe-2024.5/src/PyBWE/function_ar_extrapolation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-05-23 00:20:20.000000 pybwe-2024.5/src/PyBWE/function_burg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 00:20:34.738926 pybwe-2024.5/src/PyBWE.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10439 2024-05-23 00:20:34.000000 pybwe-2024.5/src/PyBWE.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-23 00:20:34.000000 pybwe-2024.5/src/PyBWE.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 00:20:34.000000 pybwe-2024.5/src/PyBWE.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 00:20:34.000000 pybwe-2024.5/src/PyBWE.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-23 00:20:34.000000 pybwe-2024.5/src/PyBWE.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-23 00:20:34.000000 pybwe-2024.5/src/PyBWE.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 00:20:34.738926 pybwe-2024.5/src/PyPBWE/
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-23 00:20:20.000000 pybwe-2024.5/src/PyPBWE/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-05-23 00:20:20.000000 pybwe-2024.5/src/PyPBWE/function_PBWE.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4149 2024-05-23 00:20:20.000000 pybwe-2024.5/src/PyPBWE/function_polar_burg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5099 2024-05-23 00:20:20.000000 pybwe-2024.5/src/PyPBWE/function_polar_extrapolation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 00:20:34.738926 pybwe-2024.5/src/PySSBWE/
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-23 00:20:20.000000 pybwe-2024.5/src/PySSBWE/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-05-23 00:20:20.000000 pybwe-2024.5/src/PySSBWE/function_AIC.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4915 2024-05-23 00:20:20.000000 pybwe-2024.5/src/PySSBWE/function_SSBWE.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-05-23 00:20:20.000000 pybwe-2024.5/src/PySSBWE/function_statespace_extrapolation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4260 2024-05-23 00:20:20.000000 pybwe-2024.5/src/PySSBWE/function_statespace_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2347 2024-05-23 00:20:20.000000 pybwe-2024.5/src/PySSBWE/function_statespace_properties.py
```

### Comparing `PyBWE-2024.3/LICENSE` & `pybwe-2024.5/LICENSE`

 * *Files identical despite different names*

### Comparing `PyBWE-2024.3/PKG-INFO` & `pybwe-2024.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyBWE
-Version: 2024.3
+Version: 2024.5
 Summary: Python tools for Bandwidth Extrapolation (BWE) of radar data
 Home-page: https://github.com/NicOudart/PyBWE
 Author: Nicolas OUDART
 Author-email: nicolas.oudart@latmos.ipsl.fr
 Keywords: bwe,radar,resolution,bandwidth,extrapolation,sounder,planetary,science,astronomy,astrophysics,signal processing,spectral
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -23,14 +23,15 @@
 [![status](https://joss.theoj.org/papers/16898c7ed1ff84843966a673e06dd513/status.svg)](https://joss.theoj.org/papers/16898c7ed1ff84843966a673e06dd513)
 
 [<img src="https://github.com/NicOudart/PyBWE/raw/main/Logo_PyBWE.png" width="500"/>](Logo_PyBWE.png)
 
 # PyBWE: Python tools for Bandwidth Extrapolation of planetary radar signals
 
 Resolution enhancement of radar signals with the super-resolution technique named "Bandwidth Extrapolation" (BWE).
+Website for documentation: [https://nicoudart.github.io/PyBWE](https://nicoudart.github.io/PyBWE)
 
 ## Introduction to PyBWE
 
 ### The Bandwidth Extrapolation technique
 
 Range resolution enhancement is one of the main challenges in radar signal processing. It is limited by the frequency 
 bandwidth of the instrument: the larger is the bandwidth, the better is the resolution.
```

### Comparing `PyBWE-2024.3/README.md` & `pybwe-2024.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 [![status](https://joss.theoj.org/papers/16898c7ed1ff84843966a673e06dd513/status.svg)](https://joss.theoj.org/papers/16898c7ed1ff84843966a673e06dd513)
 
 [<img src="https://github.com/NicOudart/PyBWE/raw/main/Logo_PyBWE.png" width="500"/>](Logo_PyBWE.png)
 
 # PyBWE: Python tools for Bandwidth Extrapolation of planetary radar signals
 
 Resolution enhancement of radar signals with the super-resolution technique named "Bandwidth Extrapolation" (BWE).
+Website for documentation: [https://nicoudart.github.io/PyBWE](https://nicoudart.github.io/PyBWE)
 
 ## Introduction to PyBWE
 
 ### The Bandwidth Extrapolation technique
 
 Range resolution enhancement is one of the main challenges in radar signal processing. It is limited by the frequency 
 bandwidth of the instrument: the larger is the bandwidth, the better is the resolution.
```

### Comparing `PyBWE-2024.3/setup.py` & `pybwe-2024.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup,find_packages
 
 setup(name='PyBWE',
-version='2024.03',
+version='2024.05',
 description='Python tools for Bandwidth Extrapolation (BWE) of radar data',
 long_description=open("README.md").read(),
 long_description_content_type='text/markdown',
 url='https://github.com/NicOudart/PyBWE',
 author='Nicolas OUDART',
 author_email='nicolas.oudart@latmos.ipsl.fr',
 packages=find_packages('src'),
```

### Comparing `PyBWE-2024.3/src/PyBWE/function_BWE.py` & `pybwe-2024.5/src/PyBWE/function_BWE.py`

 * *Files identical despite different names*

### Comparing `PyBWE-2024.3/src/PyBWE/function_ar_extrapolation.py` & `pybwe-2024.5/src/PyBWE/function_ar_extrapolation.py`

 * *Files identical despite different names*

### Comparing `PyBWE-2024.3/src/PyBWE/function_burg.py` & `pybwe-2024.5/src/PyBWE/function_burg.py`

 * *Files identical despite different names*

### Comparing `PyBWE-2024.3/src/PyBWE.egg-info/PKG-INFO` & `pybwe-2024.5/src/PyBWE.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyBWE
-Version: 2024.3
+Version: 2024.5
 Summary: Python tools for Bandwidth Extrapolation (BWE) of radar data
 Home-page: https://github.com/NicOudart/PyBWE
 Author: Nicolas OUDART
 Author-email: nicolas.oudart@latmos.ipsl.fr
 Keywords: bwe,radar,resolution,bandwidth,extrapolation,sounder,planetary,science,astronomy,astrophysics,signal processing,spectral
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -23,14 +23,15 @@
 [![status](https://joss.theoj.org/papers/16898c7ed1ff84843966a673e06dd513/status.svg)](https://joss.theoj.org/papers/16898c7ed1ff84843966a673e06dd513)
 
 [<img src="https://github.com/NicOudart/PyBWE/raw/main/Logo_PyBWE.png" width="500"/>](Logo_PyBWE.png)
 
 # PyBWE: Python tools for Bandwidth Extrapolation of planetary radar signals
 
 Resolution enhancement of radar signals with the super-resolution technique named "Bandwidth Extrapolation" (BWE).
+Website for documentation: [https://nicoudart.github.io/PyBWE](https://nicoudart.github.io/PyBWE)
 
 ## Introduction to PyBWE
 
 ### The Bandwidth Extrapolation technique
 
 Range resolution enhancement is one of the main challenges in radar signal processing. It is limited by the frequency 
 bandwidth of the instrument: the larger is the bandwidth, the better is the resolution.
```

### Comparing `PyBWE-2024.3/src/PyBWE.egg-info/SOURCES.txt` & `pybwe-2024.5/src/PyBWE.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyBWE-2024.3/src/PyPBWE/function_PBWE.py` & `pybwe-2024.5/src/PyPBWE/function_PBWE.py`

 * *Files identical despite different names*

### Comparing `PyBWE-2024.3/src/PyPBWE/function_polar_burg.py` & `pybwe-2024.5/src/PyPBWE/function_polar_burg.py`

 * *Files identical despite different names*

### Comparing `PyBWE-2024.3/src/PyPBWE/function_polar_extrapolation.py` & `pybwe-2024.5/src/PyPBWE/function_polar_extrapolation.py`

 * *Files identical despite different names*

### Comparing `PyBWE-2024.3/src/PySSBWE/function_AIC.py` & `pybwe-2024.5/src/PySSBWE/function_AIC.py`

 * *Files identical despite different names*

### Comparing `PyBWE-2024.3/src/PySSBWE/function_SSBWE.py` & `pybwe-2024.5/src/PySSBWE/function_SSBWE.py`

 * *Files identical despite different names*

### Comparing `PyBWE-2024.3/src/PySSBWE/function_statespace_extrapolation.py` & `pybwe-2024.5/src/PySSBWE/function_statespace_extrapolation.py`

 * *Files identical despite different names*

### Comparing `PyBWE-2024.3/src/PySSBWE/function_statespace_model.py` & `pybwe-2024.5/src/PySSBWE/function_statespace_model.py`

 * *Files identical despite different names*

### Comparing `PyBWE-2024.3/src/PySSBWE/function_statespace_properties.py` & `pybwe-2024.5/src/PySSBWE/function_statespace_properties.py`

 * *Files identical despite different names*

