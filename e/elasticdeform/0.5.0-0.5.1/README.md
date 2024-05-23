# Comparing `tmp/elasticdeform-0.5.0.tar.gz` & `tmp/elasticdeform-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elasticdeform-0.5.0.tar", last modified: Wed Sep 21 23:42:11 2022, max compression
+gzip compressed data, was "elasticdeform-0.5.1.tar", last modified: Thu May 23 20:27:57 2024, max compression
```

## Comparing `elasticdeform-0.5.0.tar` & `elasticdeform-0.5.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 23:42:11.776274 elasticdeform-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1637 2022-09-21 23:42:08.000000 elasticdeform-0.5.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)       89 2022-09-21 23:42:08.000000 elasticdeform-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    11458 2022-09-21 23:42:11.776274 elasticdeform-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     9085 2022-09-21 23:42:08.000000 elasticdeform-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 23:42:11.776274 elasticdeform-0.5.0/elasticdeform/
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-09-21 23:42:08.000000 elasticdeform-0.5.0/elasticdeform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12290 2022-09-21 23:42:08.000000 elasticdeform-0.5.0/elasticdeform/_deform_grid.c
--rw-r--r--   0 runner    (1001) docker     (121)    46715 2022-09-21 23:42:08.000000 elasticdeform-0.5.0/elasticdeform/deform.c
--rw-r--r--   0 runner    (1001) docker     (121)      546 2022-09-21 23:42:08.000000 elasticdeform-0.5.0/elasticdeform/deform.h
--rw-r--r--   0 runner    (1001) docker     (121)    17986 2022-09-21 23:42:08.000000 elasticdeform-0.5.0/elasticdeform/deform_grid.py
--rw-r--r--   0 runner    (1001) docker     (121)    30562 2022-09-21 23:42:08.000000 elasticdeform-0.5.0/elasticdeform/from_nd_image.c
--rw-r--r--   0 runner    (1001) docker     (121)    15554 2022-09-21 23:42:08.000000 elasticdeform-0.5.0/elasticdeform/from_scipy.h
--rw-r--r--   0 runner    (1001) docker     (121)     2707 2022-09-21 23:42:08.000000 elasticdeform-0.5.0/elasticdeform/tf.py
--rw-r--r--   0 runner    (1001) docker     (121)     2178 2022-09-21 23:42:08.000000 elasticdeform-0.5.0/elasticdeform/torch.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 23:42:11.776274 elasticdeform-0.5.0/elasticdeform.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    11458 2022-09-21 23:42:11.000000 elasticdeform-0.5.0/elasticdeform.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      473 2022-09-21 23:42:11.000000 elasticdeform-0.5.0/elasticdeform.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-21 23:42:11.000000 elasticdeform-0.5.0/elasticdeform.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-09-21 23:42:11.000000 elasticdeform-0.5.0/elasticdeform.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-09-21 23:42:11.000000 elasticdeform-0.5.0/elasticdeform.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-09-21 23:42:08.000000 elasticdeform-0.5.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-21 23:42:11.776274 elasticdeform-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1470 2022-09-21 23:42:08.000000 elasticdeform-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:27:57.446574 elasticdeform-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-05-23 20:27:50.000000 elasticdeform-0.5.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-23 20:27:50.000000 elasticdeform-0.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    11458 2024-05-23 20:27:57.446574 elasticdeform-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9085 2024-05-23 20:27:50.000000 elasticdeform-0.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:27:57.446574 elasticdeform-0.5.1/elasticdeform/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-23 20:27:50.000000 elasticdeform-0.5.1/elasticdeform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12290 2024-05-23 20:27:50.000000 elasticdeform-0.5.1/elasticdeform/_deform_grid.c
+-rw-r--r--   0 runner    (1001) docker     (127)    46715 2024-05-23 20:27:50.000000 elasticdeform-0.5.1/elasticdeform/deform.c
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-23 20:27:50.000000 elasticdeform-0.5.1/elasticdeform/deform.h
+-rw-r--r--   0 runner    (1001) docker     (127)    17986 2024-05-23 20:27:50.000000 elasticdeform-0.5.1/elasticdeform/deform_grid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30562 2024-05-23 20:27:50.000000 elasticdeform-0.5.1/elasticdeform/from_nd_image.c
+-rw-r--r--   0 runner    (1001) docker     (127)    15554 2024-05-23 20:27:50.000000 elasticdeform-0.5.1/elasticdeform/from_scipy.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-05-23 20:27:50.000000 elasticdeform-0.5.1/elasticdeform/tf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2178 2024-05-23 20:27:50.000000 elasticdeform-0.5.1/elasticdeform/torch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:27:57.446574 elasticdeform-0.5.1/elasticdeform.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11458 2024-05-23 20:27:56.000000 elasticdeform-0.5.1/elasticdeform.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-23 20:27:57.000000 elasticdeform-0.5.1/elasticdeform.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 20:27:56.000000 elasticdeform-0.5.1/elasticdeform.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-23 20:27:56.000000 elasticdeform-0.5.1/elasticdeform.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-23 20:27:56.000000 elasticdeform-0.5.1/elasticdeform.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-23 20:27:50.000000 elasticdeform-0.5.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 20:27:57.446574 elasticdeform-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-23 20:27:50.000000 elasticdeform-0.5.1/setup.py
```

### Comparing `elasticdeform-0.5.0/LICENSE.txt` & `elasticdeform-0.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `elasticdeform-0.5.0/PKG-INFO` & `elasticdeform-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elasticdeform
-Version: 0.5.0
+Version: 0.5.1
 Summary: Elastic deformations for N-D images.
 Home-page: https://github.com/gvtulder/elasticdeform
 Author: Gijs van Tulder
 Author-email: gvtulder@gmail.com
 License: BSD
 Description: Elastic deformations for N-dimensional images (Python, SciPy, NumPy, TensorFlow, PyTorch)
         =========================================================================================
```

### Comparing `elasticdeform-0.5.0/README.md` & `elasticdeform-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `elasticdeform-0.5.0/elasticdeform/_deform_grid.c` & `elasticdeform-0.5.1/elasticdeform/_deform_grid.c`

 * *Files identical despite different names*

### Comparing `elasticdeform-0.5.0/elasticdeform/deform.c` & `elasticdeform-0.5.1/elasticdeform/deform.c`

 * *Files identical despite different names*

### Comparing `elasticdeform-0.5.0/elasticdeform/deform.h` & `elasticdeform-0.5.1/elasticdeform/deform.h`

 * *Files identical despite different names*

### Comparing `elasticdeform-0.5.0/elasticdeform/deform_grid.py` & `elasticdeform-0.5.1/elasticdeform/deform_grid.py`

 * *Files identical despite different names*

### Comparing `elasticdeform-0.5.0/elasticdeform/from_nd_image.c` & `elasticdeform-0.5.1/elasticdeform/from_nd_image.c`

 * *Files identical despite different names*

### Comparing `elasticdeform-0.5.0/elasticdeform/from_scipy.h` & `elasticdeform-0.5.1/elasticdeform/from_scipy.h`

 * *Files identical despite different names*

### Comparing `elasticdeform-0.5.0/elasticdeform/tf.py` & `elasticdeform-0.5.1/elasticdeform/tf.py`

 * *Files identical despite different names*

### Comparing `elasticdeform-0.5.0/elasticdeform/torch.py` & `elasticdeform-0.5.1/elasticdeform/torch.py`

 * *Files identical despite different names*

### Comparing `elasticdeform-0.5.0/elasticdeform.egg-info/PKG-INFO` & `elasticdeform-0.5.1/elasticdeform.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elasticdeform
-Version: 0.5.0
+Version: 0.5.1
 Summary: Elastic deformations for N-D images.
 Home-page: https://github.com/gvtulder/elasticdeform
 Author: Gijs van Tulder
 Author-email: gvtulder@gmail.com
 License: BSD
 Description: Elastic deformations for N-dimensional images (Python, SciPy, NumPy, TensorFlow, PyTorch)
         =========================================================================================
```

### Comparing `elasticdeform-0.5.0/setup.py` & `elasticdeform-0.5.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,23 +2,26 @@
 from setuptools import setup, Extension
 from setuptools.command.build_ext import build_ext as _build_ext
 
 class build_ext(_build_ext):
     def finalize_options(self):
         _build_ext.finalize_options(self)
         # Prevent numpy from thinking it is still in its setup process:
-        __builtins__.__NUMPY_SETUP__ = False
+        if isinstance(__builtins__, dict):
+            __builtins__["__NUMPY_SETUP__"] = False
+        else:
+            __builtins__.__NUMPY_SETUP__ = False
         import numpy
         self.include_dirs.append(numpy.get_include())
 
 with io.open('README.md', encoding='utf-8') as f:
     readme_txt = f.read()
 
 setup(name='elasticdeform',
-      version='0.5.0',
+      version='0.5.1',
       description='Elastic deformations for N-D images.',
       long_description_content_type='text/markdown',
       long_description=readme_txt,
       author='Gijs van Tulder',
       author_email='gvtulder@gmail.com',
       url='https://github.com/gvtulder/elasticdeform',
       license='BSD',
```

