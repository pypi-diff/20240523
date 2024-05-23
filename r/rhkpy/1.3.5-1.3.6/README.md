# Comparing `tmp/rhkpy-1.3.5.tar.gz` & `tmp/rhkpy-1.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rhkpy-1.3.5.tar", last modified: Wed Jan 17 09:26:37 2024, max compression
+gzip compressed data, was "rhkpy-1.3.6.tar", last modified: Thu May 23 08:29:58 2024, max compression
```

## Comparing `rhkpy-1.3.5.tar` & `rhkpy-1.3.6.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 09:26:37.442009 rhkpy-1.3.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-01-17 09:26:27.000000 rhkpy-1.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-01-17 09:26:37.442009 rhkpy-1.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-01-17 09:26:27.000000 rhkpy-1.3.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 09:26:37.438009 rhkpy-1.3.5/rhkpy/
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-01-17 09:26:28.000000 rhkpy-1.3.5/rhkpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    65633 2024-01-17 09:26:28.000000 rhkpy-1.3.5/rhkpy/rhkpy_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)    35856 2024-01-17 09:26:28.000000 rhkpy-1.3.5/rhkpy/rhkpy_process.py
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-01-17 09:26:28.000000 rhkpy-1.3.5/rhkpy/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 09:26:37.438009 rhkpy-1.3.5/rhkpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-01-17 09:26:37.000000 rhkpy-1.3.5/rhkpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-01-17 09:26:37.000000 rhkpy-1.3.5/rhkpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-17 09:26:37.000000 rhkpy-1.3.5/rhkpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-01-17 09:26:37.000000 rhkpy-1.3.5/rhkpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-01-17 09:26:37.000000 rhkpy-1.3.5/rhkpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-17 09:26:37.442009 rhkpy-1.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-01-17 09:26:28.000000 rhkpy-1.3.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 09:26:37.438009 rhkpy-1.3.5/spym/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-01-17 09:26:28.000000 rhkpy-1.3.5/spym/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 09:26:37.438009 rhkpy-1.3.5/spym/_accessors/
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-01-17 09:26:28.000000 rhkpy-1.3.5/spym/_accessors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-01-17 09:26:28.000000 rhkpy-1.3.5/spym/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 09:26:37.438009 rhkpy-1.3.5/spym/io/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-01-17 09:26:28.000000 rhkpy-1.3.5/spym/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-01-17 09:26:28.000000 rhkpy-1.3.5/spym/io/load.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 09:26:37.438009 rhkpy-1.3.5/spym/io/omicronscala/
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-01-17 09:26:28.000000 rhkpy-1.3.5/spym/io/omicronscala/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4007 2024-01-17 09:26:28.000000 rhkpy-1.3.5/spym/io/omicronscala/_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     8611 2024-01-17 09:26:28.000000 rhkpy-1.3.5/spym/io/omicronscala/_scala.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 09:26:37.442009 rhkpy-1.3.5/spym/io/rhksm4/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-01-17 09:26:28.000000 rhkpy-1.3.5/spym/io/rhksm4/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5240 2024-01-17 09:26:28.000000 rhkpy-1.3.5/spym/io/rhksm4/_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)    49984 2024-01-17 09:26:28.000000 rhkpy-1.3.5/spym/io/rhksm4/_sm4.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 09:26:37.442009 rhkpy-1.3.5/spym/plotting/
--rw-r--r--   0 runner    (1001) docker     (127)     4803 2024-01-17 09:26:28.000000 rhkpy-1.3.5/spym/plotting/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 09:26:37.442009 rhkpy-1.3.5/spym/process/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-01-17 09:26:28.000000 rhkpy-1.3.5/spym/process/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6186 2024-01-17 09:26:28.000000 rhkpy-1.3.5/spym/process/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     3299 2024-01-17 09:26:28.000000 rhkpy-1.3.5/spym/process/level.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:29:58.659744 rhkpy-1.3.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-23 08:29:48.000000 rhkpy-1.3.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-05-23 08:29:58.659744 rhkpy-1.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-05-23 08:29:48.000000 rhkpy-1.3.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:29:58.655743 rhkpy-1.3.6/rhkpy/
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-23 08:29:48.000000 rhkpy-1.3.6/rhkpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65633 2024-05-23 08:29:48.000000 rhkpy-1.3.6/rhkpy/rhkpy_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35856 2024-05-23 08:29:48.000000 rhkpy-1.3.6/rhkpy/rhkpy_process.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-23 08:29:48.000000 rhkpy-1.3.6/rhkpy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:29:58.659744 rhkpy-1.3.6/rhkpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-05-23 08:29:58.000000 rhkpy-1.3.6/rhkpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-23 08:29:58.000000 rhkpy-1.3.6/rhkpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 08:29:58.000000 rhkpy-1.3.6/rhkpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-23 08:29:58.000000 rhkpy-1.3.6/rhkpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-23 08:29:58.000000 rhkpy-1.3.6/rhkpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 08:29:58.659744 rhkpy-1.3.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-23 08:29:48.000000 rhkpy-1.3.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:29:58.659744 rhkpy-1.3.6/spym/
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-23 08:29:48.000000 rhkpy-1.3.6/spym/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:29:58.659744 rhkpy-1.3.6/spym/_accessors/
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-23 08:29:48.000000 rhkpy-1.3.6/spym/_accessors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-23 08:29:48.000000 rhkpy-1.3.6/spym/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:29:58.659744 rhkpy-1.3.6/spym/io/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-23 08:29:48.000000 rhkpy-1.3.6/spym/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-05-23 08:29:48.000000 rhkpy-1.3.6/spym/io/load.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:29:58.659744 rhkpy-1.3.6/spym/io/omicronscala/
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-23 08:29:48.000000 rhkpy-1.3.6/spym/io/omicronscala/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4007 2024-05-23 08:29:48.000000 rhkpy-1.3.6/spym/io/omicronscala/_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8611 2024-05-23 08:29:48.000000 rhkpy-1.3.6/spym/io/omicronscala/_scala.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:29:58.659744 rhkpy-1.3.6/spym/io/rhksm4/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-23 08:29:48.000000 rhkpy-1.3.6/spym/io/rhksm4/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5240 2024-05-23 08:29:48.000000 rhkpy-1.3.6/spym/io/rhksm4/_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49989 2024-05-23 08:29:48.000000 rhkpy-1.3.6/spym/io/rhksm4/_sm4.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:29:58.659744 rhkpy-1.3.6/spym/plotting/
+-rw-r--r--   0 runner    (1001) docker     (127)     4803 2024-05-23 08:29:48.000000 rhkpy-1.3.6/spym/plotting/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:29:58.659744 rhkpy-1.3.6/spym/process/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-23 08:29:48.000000 rhkpy-1.3.6/spym/process/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6186 2024-05-23 08:29:48.000000 rhkpy-1.3.6/spym/process/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3299 2024-05-23 08:29:48.000000 rhkpy-1.3.6/spym/process/level.py
```

### Comparing `rhkpy-1.3.5/LICENSE` & `rhkpy-1.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `rhkpy-1.3.5/PKG-INFO` & `rhkpy-1.3.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: rhkpy
-Version: 1.3.5
+Version: 1.3.6
 Summary: A python package for processing Scanning Tunneling Microscopy (STM) data from RHK, based on the spym project.
 Home-page: https://github.com/zrbyte/rhkpy
 Author: Peter Nemes-Incze
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # RHK STM data analysis tool
 
-Based on the [spym project](https://github.com/rescipy-project/spym) (version 0.9), for use in our research group.
+Based on the [spym project](https://github.com/rescipy-project/spym) (version 0.9.1).
 
 Documentation can be found here: https://zrbyte.github.io/rhkpy/
 
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/zrbyte/rhkpy/HEAD)
 
 If you use this package in your publication, consider citing it:
 Peter Nemes-I., & Mirco Panighel. (2023). zrbyte/rhkpy: v1.3.3 (v1.3.3). Zenodo. https://zenodo.org/doi/10.5281/zenodo.10143224
```

### Comparing `rhkpy-1.3.5/README.md` & `rhkpy-1.3.6/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # RHK STM data analysis tool
 
-Based on the [spym project](https://github.com/rescipy-project/spym) (version 0.9), for use in our research group.
+Based on the [spym project](https://github.com/rescipy-project/spym) (version 0.9.1).
 
 Documentation can be found here: https://zrbyte.github.io/rhkpy/
 
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/zrbyte/rhkpy/HEAD)
 
 If you use this package in your publication, consider citing it:
 Peter Nemes-I., & Mirco Panighel. (2023). zrbyte/rhkpy: v1.3.3 (v1.3.3). Zenodo. https://zenodo.org/doi/10.5281/zenodo.10143224
```

### Comparing `rhkpy-1.3.5/rhkpy/__init__.py` & `rhkpy-1.3.6/rhkpy/__init__.py`

 * *Files identical despite different names*

### Comparing `rhkpy-1.3.5/rhkpy/rhkpy_loader.py` & `rhkpy-1.3.6/rhkpy/rhkpy_loader.py`

 * *Files identical despite different names*

### Comparing `rhkpy-1.3.5/rhkpy/rhkpy_process.py` & `rhkpy-1.3.6/rhkpy/rhkpy_process.py`

 * *Files identical despite different names*

### Comparing `rhkpy-1.3.5/rhkpy.egg-info/PKG-INFO` & `rhkpy-1.3.6/rhkpy.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: rhkpy
-Version: 1.3.5
+Version: 1.3.6
 Summary: A python package for processing Scanning Tunneling Microscopy (STM) data from RHK, based on the spym project.
 Home-page: https://github.com/zrbyte/rhkpy
 Author: Peter Nemes-Incze
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # RHK STM data analysis tool
 
-Based on the [spym project](https://github.com/rescipy-project/spym) (version 0.9), for use in our research group.
+Based on the [spym project](https://github.com/rescipy-project/spym) (version 0.9.1).
 
 Documentation can be found here: https://zrbyte.github.io/rhkpy/
 
 [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/zrbyte/rhkpy/HEAD)
 
 If you use this package in your publication, consider citing it:
 Peter Nemes-I., & Mirco Panighel. (2023). zrbyte/rhkpy: v1.3.3 (v1.3.3). Zenodo. https://zenodo.org/doi/10.5281/zenodo.10143224
```

### Comparing `rhkpy-1.3.5/rhkpy.egg-info/SOURCES.txt` & `rhkpy-1.3.6/rhkpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rhkpy-1.3.5/setup.py` & `rhkpy-1.3.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name = "rhkpy",
-    version = "1.3.5",
+    version = "1.3.6",
     packages = find_packages(),
     # python_requires = '>=3.10',
     install_requires = [
         "matplotlib",
         "numpy",
         "pandas",
         "scipy",
```

### Comparing `rhkpy-1.3.5/spym/_accessors/__init__.py` & `rhkpy-1.3.6/spym/_accessors/__init__.py`

 * *Files identical despite different names*

### Comparing `rhkpy-1.3.5/spym/io/load.py` & `rhkpy-1.3.6/spym/io/load.py`

 * *Files identical despite different names*

### Comparing `rhkpy-1.3.5/spym/io/omicronscala/_methods.py` & `rhkpy-1.3.6/spym/io/omicronscala/_methods.py`

 * *Files identical despite different names*

### Comparing `rhkpy-1.3.5/spym/io/omicronscala/_scala.py` & `rhkpy-1.3.6/spym/io/omicronscala/_scala.py`

 * *Files identical despite different names*

### Comparing `rhkpy-1.3.5/spym/io/rhksm4/_methods.py` & `rhkpy-1.3.6/spym/io/rhksm4/_methods.py`

 * *Files identical despite different names*

### Comparing `rhkpy-1.3.5/spym/io/rhksm4/_sm4.py` & `rhkpy-1.3.6/spym/io/rhksm4/_sm4.py`

 * *Files 0% similar despite different names*

```diff
@@ -610,15 +610,15 @@
 
         self._sm4._seek(offset, 0)
 
         if self._PRM_CompressionFlag == 0:
             PRMdata = np.fromfile(self._sm4._file, dtype=np.uint32, count=self._PRM_DataSize)
         elif self._PRM_CompressionFlag == 1:
             comprPRMdata = np.fromfile(self._sm4._file, dtype=np.uint32, count=self._PRM_CompressionSize)
-            PRMdata = zlib.decompress(comprPRMdata, wbits=0, bufsize=self._PRM_DataSize)
+            PRMdata = zlib.decompressobj(wbits=0).decompress(comprPRMdata,self._PRM_DataSize)
 
         self.attrs['RHK_PRMdata'] = PRMdata.decode('CP437')
 
     def _read_PRMHeader(self, offset):
         ''' Read PRM Header for the current page.
         
         Valid only for RHK XPMPro generated files.
```

### Comparing `rhkpy-1.3.5/spym/plotting/__init__.py` & `rhkpy-1.3.6/spym/plotting/__init__.py`

 * *Files identical despite different names*

### Comparing `rhkpy-1.3.5/spym/process/filters.py` & `rhkpy-1.3.6/spym/process/filters.py`

 * *Files identical despite different names*

### Comparing `rhkpy-1.3.5/spym/process/level.py` & `rhkpy-1.3.6/spym/process/level.py`

 * *Files identical despite different names*

