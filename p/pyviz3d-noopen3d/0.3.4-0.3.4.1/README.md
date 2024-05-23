# Comparing `tmp/pyviz3d_noopen3d-0.3.4.tar.gz` & `tmp/pyviz3d_noopen3d-0.3.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyviz3d_noopen3d-0.3.4.tar", last modified: Thu May 23 12:43:14 2024, max compression
+gzip compressed data, was "pyviz3d_noopen3d-0.3.4.1.tar", last modified: Thu May 23 13:16:12 2024, max compression
```

## Comparing `pyviz3d_noopen3d-0.3.4.tar` & `pyviz3d_noopen3d-0.3.4.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 silvanosky  (1000) silvanosky  (1000)        0 2024-05-23 12:43:14.583721 pyviz3d_noopen3d-0.3.4/
--rw-r--r--   0 silvanosky  (1000) silvanosky  (1000)     1104 2024-05-23 12:32:13.000000 pyviz3d_noopen3d-0.3.4/LICENSE
--rw-r--r--   0 silvanosky  (1000) silvanosky  (1000)       65 2024-05-23 12:32:13.000000 pyviz3d_noopen3d-0.3.4/MANIFEST.in
--rw-r--r--   0 silvanosky  (1000) silvanosky  (1000)     7339 2024-05-23 12:43:14.583721 pyviz3d_noopen3d-0.3.4/PKG-INFO
--rw-r--r--   0 silvanosky  (1000) silvanosky  (1000)     5531 2024-05-23 12:32:13.000000 pyviz3d_noopen3d-0.3.4/README.md
--rw-r--r--   0 silvanosky  (1000) silvanosky  (1000)      687 2024-05-23 12:42:37.000000 pyviz3d_noopen3d-0.3.4/pyproject.toml
-drwxr-xr-x   0 silvanosky  (1000) silvanosky  (1000)        0 2024-05-23 12:43:14.580388 pyviz3d_noopen3d-0.3.4/pyviz3d/
--rw-r--r--   0 silvanosky  (1000) silvanosky  (1000)        0 2024-05-23 12:32:14.000000 pyviz3d_noopen3d-0.3.4/pyviz3d/__init__.py
--rw-r--r--   0 silvanosky  (1000) silvanosky  (1000)     1143 2024-05-23 12:32:14.000000 pyviz3d_noopen3d-0.3.4/pyviz3d/arrow.py
--rw-r--r--   0 silvanosky  (1000) silvanosky  (1000)     1236 2024-05-23 12:32:14.000000 pyviz3d_noopen3d-0.3.4/pyviz3d/camera.py
--rw-r--r--   0 silvanosky  (1000) silvanosky  (1000)     1266 2024-05-23 12:32:14.000000 pyviz3d_noopen3d-0.3.4/pyviz3d/circles_2d.py
--rw-r--r--   0 silvanosky  (1000) silvanosky  (1000)     1168 2024-05-23 12:32:14.000000 pyviz3d_noopen3d-0.3.4/pyviz3d/cuboid.py
--rw-r--r--   0 silvanosky  (1000) silvanosky  (1000)     1060 2024-05-23 12:32:14.000000 pyviz3d_noopen3d-0.3.4/pyviz3d/labels.py
--rw-r--r--   0 silvanosky  (1000) silvanosky  (1000)     1501 2024-05-23 12:32:14.000000 pyviz3d_noopen3d-0.3.4/pyviz3d/lines.py
--rw-r--r--   0 silvanosky  (1000) silvanosky  (1000)     1681 2024-05-23 12:32:14.000000 pyviz3d_noopen3d-0.3.4/pyviz3d/mesh.py
--rw-r--r--   0 silvanosky  (1000) silvanosky  (1000)     2350 2024-05-23 12:32:14.000000 pyviz3d_noopen3d-0.3.4/pyviz3d/points.py
--rw-r--r--   0 silvanosky  (1000) silvanosky  (1000)      935 2024-05-23 12:32:14.000000 pyviz3d_noopen3d-0.3.4/pyviz3d/polyline.py
-drwxr-xr-x   0 silvanosky  (1000) silvanosky  (1000)        0 2024-05-23 12:43:14.580388 pyviz3d_noopen3d-0.3.4/pyviz3d/src/
--rw-r--r--   0 silvanosky  (1000) silvanosky  (1000)    10473 2024-05-23 12:32:14.000000 pyviz3d_noopen3d-0.3.4/pyviz3d/src/blender_tools.py
-drwxr-xr-x   0 silvanosky  (1000) silvanosky  (1000)        0 2024-05-23 12:43:14.580388 pyviz3d_noopen3d-0.3.4/pyviz3d/src/css/
--rw-r--r--   0 silvanosky  (1000) silvanosky  (1000)   194856 2024-05-23 12:32:14.000000 pyviz3d_noopen3d-0.3.4/pyviz3d/src/css/bootstrap.min.css
--rw-r--r--   0 silvanosky  (1000) silvanosky  (1000)     1406 2024-05-23 12:32:14.000000 pyviz3d_noopen3d-0.3.4/pyviz3d/src/favicon.ico
--rw-r--r--   0 silvanosky  (1000) silvanosky  (1000)     4889 2024-05-23 12:32:14.000000 pyviz3d_noopen3d-0.3.4/pyviz3d/src/index.html
-drwxr-xr-x   0 silvanosky  (1000) silvanosky  (1000)        0 2024-05-23 12:43:14.580388 pyviz3d_noopen3d-0.3.4/pyviz3d/src/js/
--rw-r--r--   0 silvanosky  (1000) silvanosky  (1000)    60363 2024-05-23 12:32:14.000000 pyviz3d_noopen3d-0.3.4/pyviz3d/src/js/bootstrap.min.js
--rw-r--r--   0 silvanosky  (1000) silvanosky  (1000)    89664 2024-05-23 12:32:14.000000 pyviz3d_noopen3d-0.3.4/pyviz3d/src/js/jquery.min.js
--rw-r--r--   0 silvanosky  (1000) silvanosky  (1000)    25452 2024-05-23 12:32:14.000000 pyviz3d_noopen3d-0.3.4/pyviz3d/src/js/scene.js
--rw-r--r--   0 silvanosky  (1000) silvanosky  (1000)    16804 2024-05-23 12:33:17.000000 pyviz3d_noopen3d-0.3.4/pyviz3d/visualizer.py
-drwxr-xr-x   0 silvanosky  (1000) silvanosky  (1000)        0 2024-05-23 12:43:14.583721 pyviz3d_noopen3d-0.3.4/pyviz3d_noopen3d.egg-info/
--rw-r--r--   0 silvanosky  (1000) silvanosky  (1000)     7339 2024-05-23 12:43:14.000000 pyviz3d_noopen3d-0.3.4/pyviz3d_noopen3d.egg-info/PKG-INFO
--rw-r--r--   0 silvanosky  (1000) silvanosky  (1000)      644 2024-05-23 12:43:14.000000 pyviz3d_noopen3d-0.3.4/pyviz3d_noopen3d.egg-info/SOURCES.txt
--rw-r--r--   0 silvanosky  (1000) silvanosky  (1000)        1 2024-05-23 12:43:14.000000 pyviz3d_noopen3d-0.3.4/pyviz3d_noopen3d.egg-info/dependency_links.txt
--rw-r--r--   0 silvanosky  (1000) silvanosky  (1000)        6 2024-05-23 12:43:14.000000 pyviz3d_noopen3d-0.3.4/pyviz3d_noopen3d.egg-info/requires.txt
--rw-r--r--   0 silvanosky  (1000) silvanosky  (1000)        8 2024-05-23 12:43:14.000000 pyviz3d_noopen3d-0.3.4/pyviz3d_noopen3d.egg-info/top_level.txt
--rw-r--r--   0 silvanosky  (1000) silvanosky  (1000)       38 2024-05-23 12:43:14.583721 pyviz3d_noopen3d-0.3.4/setup.cfg
+drwxr-xr-x   0 silvanosky  (1000) silvanosky  (1000)        0 2024-05-23 13:16:12.246138 pyviz3d_noopen3d-0.3.4.1/
+-rw-r--r--   0 silvanosky  (1000) silvanosky  (1000)     1104 2024-05-23 12:32:13.000000 pyviz3d_noopen3d-0.3.4.1/LICENSE
+-rw-r--r--   0 silvanosky  (1000) silvanosky  (1000)       65 2024-05-23 12:32:13.000000 pyviz3d_noopen3d-0.3.4.1/MANIFEST.in
+-rw-r--r--   0 silvanosky  (1000) silvanosky  (1000)     7341 2024-05-23 13:16:12.246138 pyviz3d_noopen3d-0.3.4.1/PKG-INFO
+-rw-r--r--   0 silvanosky  (1000) silvanosky  (1000)     5531 2024-05-23 12:32:13.000000 pyviz3d_noopen3d-0.3.4.1/README.md
+-rw-r--r--   0 silvanosky  (1000) silvanosky  (1000)      689 2024-05-23 13:16:06.000000 pyviz3d_noopen3d-0.3.4.1/pyproject.toml
+drwxr-xr-x   0 silvanosky  (1000) silvanosky  (1000)        0 2024-05-23 13:16:12.246138 pyviz3d_noopen3d-0.3.4.1/pyviz3d/
+-rw-r--r--   0 silvanosky  (1000) silvanosky  (1000)        0 2024-05-23 12:32:14.000000 pyviz3d_noopen3d-0.3.4.1/pyviz3d/__init__.py
+-rw-r--r--   0 silvanosky  (1000) silvanosky  (1000)     1143 2024-05-23 12:32:14.000000 pyviz3d_noopen3d-0.3.4.1/pyviz3d/arrow.py
+-rw-r--r--   0 silvanosky  (1000) silvanosky  (1000)     1236 2024-05-23 12:32:14.000000 pyviz3d_noopen3d-0.3.4.1/pyviz3d/camera.py
+-rw-r--r--   0 silvanosky  (1000) silvanosky  (1000)     1266 2024-05-23 12:32:14.000000 pyviz3d_noopen3d-0.3.4.1/pyviz3d/circles_2d.py
+-rw-r--r--   0 silvanosky  (1000) silvanosky  (1000)     1168 2024-05-23 12:32:14.000000 pyviz3d_noopen3d-0.3.4.1/pyviz3d/cuboid.py
+-rw-r--r--   0 silvanosky  (1000) silvanosky  (1000)     1060 2024-05-23 12:32:14.000000 pyviz3d_noopen3d-0.3.4.1/pyviz3d/labels.py
+-rw-r--r--   0 silvanosky  (1000) silvanosky  (1000)     1501 2024-05-23 12:32:14.000000 pyviz3d_noopen3d-0.3.4.1/pyviz3d/lines.py
+-rw-r--r--   0 silvanosky  (1000) silvanosky  (1000)     1681 2024-05-23 12:32:14.000000 pyviz3d_noopen3d-0.3.4.1/pyviz3d/mesh.py
+-rw-r--r--   0 silvanosky  (1000) silvanosky  (1000)     2350 2024-05-23 12:32:14.000000 pyviz3d_noopen3d-0.3.4.1/pyviz3d/points.py
+-rw-r--r--   0 silvanosky  (1000) silvanosky  (1000)      935 2024-05-23 12:32:14.000000 pyviz3d_noopen3d-0.3.4.1/pyviz3d/polyline.py
+drwxr-xr-x   0 silvanosky  (1000) silvanosky  (1000)        0 2024-05-23 13:16:12.246138 pyviz3d_noopen3d-0.3.4.1/pyviz3d/src/
+-rw-r--r--   0 silvanosky  (1000) silvanosky  (1000)    10473 2024-05-23 12:32:14.000000 pyviz3d_noopen3d-0.3.4.1/pyviz3d/src/blender_tools.py
+drwxr-xr-x   0 silvanosky  (1000) silvanosky  (1000)        0 2024-05-23 13:16:12.246138 pyviz3d_noopen3d-0.3.4.1/pyviz3d/src/css/
+-rw-r--r--   0 silvanosky  (1000) silvanosky  (1000)   194856 2024-05-23 12:32:14.000000 pyviz3d_noopen3d-0.3.4.1/pyviz3d/src/css/bootstrap.min.css
+-rw-r--r--   0 silvanosky  (1000) silvanosky  (1000)     1406 2024-05-23 12:32:14.000000 pyviz3d_noopen3d-0.3.4.1/pyviz3d/src/favicon.ico
+-rw-r--r--   0 silvanosky  (1000) silvanosky  (1000)     4889 2024-05-23 12:32:14.000000 pyviz3d_noopen3d-0.3.4.1/pyviz3d/src/index.html
+drwxr-xr-x   0 silvanosky  (1000) silvanosky  (1000)        0 2024-05-23 13:16:12.246138 pyviz3d_noopen3d-0.3.4.1/pyviz3d/src/js/
+-rw-r--r--   0 silvanosky  (1000) silvanosky  (1000)    60363 2024-05-23 12:32:14.000000 pyviz3d_noopen3d-0.3.4.1/pyviz3d/src/js/bootstrap.min.js
+-rw-r--r--   0 silvanosky  (1000) silvanosky  (1000)    89664 2024-05-23 12:32:14.000000 pyviz3d_noopen3d-0.3.4.1/pyviz3d/src/js/jquery.min.js
+-rw-r--r--   0 silvanosky  (1000) silvanosky  (1000)    25452 2024-05-23 12:32:14.000000 pyviz3d_noopen3d-0.3.4.1/pyviz3d/src/js/scene.js
+-rw-r--r--   0 silvanosky  (1000) silvanosky  (1000)    17239 2024-05-23 13:14:43.000000 pyviz3d_noopen3d-0.3.4.1/pyviz3d/visualizer.py
+drwxr-xr-x   0 silvanosky  (1000) silvanosky  (1000)        0 2024-05-23 13:16:12.246138 pyviz3d_noopen3d-0.3.4.1/pyviz3d_noopen3d.egg-info/
+-rw-r--r--   0 silvanosky  (1000) silvanosky  (1000)     7341 2024-05-23 13:16:12.000000 pyviz3d_noopen3d-0.3.4.1/pyviz3d_noopen3d.egg-info/PKG-INFO
+-rw-r--r--   0 silvanosky  (1000) silvanosky  (1000)      644 2024-05-23 13:16:12.000000 pyviz3d_noopen3d-0.3.4.1/pyviz3d_noopen3d.egg-info/SOURCES.txt
+-rw-r--r--   0 silvanosky  (1000) silvanosky  (1000)        1 2024-05-23 13:16:12.000000 pyviz3d_noopen3d-0.3.4.1/pyviz3d_noopen3d.egg-info/dependency_links.txt
+-rw-r--r--   0 silvanosky  (1000) silvanosky  (1000)        6 2024-05-23 13:16:12.000000 pyviz3d_noopen3d-0.3.4.1/pyviz3d_noopen3d.egg-info/requires.txt
+-rw-r--r--   0 silvanosky  (1000) silvanosky  (1000)        8 2024-05-23 13:16:12.000000 pyviz3d_noopen3d-0.3.4.1/pyviz3d_noopen3d.egg-info/top_level.txt
+-rw-r--r--   0 silvanosky  (1000) silvanosky  (1000)       38 2024-05-23 13:16:12.246138 pyviz3d_noopen3d-0.3.4.1/setup.cfg
```

### Comparing `pyviz3d_noopen3d-0.3.4/LICENSE` & `pyviz3d_noopen3d-0.3.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyviz3d_noopen3d-0.3.4/PKG-INFO` & `pyviz3d_noopen3d-0.3.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyviz3d-noopen3d
-Version: 0.3.4
+Version: 0.3.4.1
 Summary: PyViz3D is a python package to visualize 3D scenes.
 Author-email: Francis Engelmann <francis.engelmann@gmail.com>
 License: MIT License
         
         Copyright (c) 2018 Francis Engelmann <francis.engelmann@gmail.com>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pyviz3d_noopen3d-0.3.4/README.md` & `pyviz3d_noopen3d-0.3.4.1/README.md`

 * *Files identical despite different names*

### Comparing `pyviz3d_noopen3d-0.3.4/pyproject.toml` & `pyviz3d_noopen3d-0.3.4.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyviz3d-noopen3d"
-version = "0.3.4"
+version = "0.3.4.1"
 description = "PyViz3D is a python package to visualize 3D scenes."
 readme = "README.md"
 authors = [{ name = "Francis Engelmann", email = "francis.engelmann@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `pyviz3d_noopen3d-0.3.4/pyviz3d/arrow.py` & `pyviz3d_noopen3d-0.3.4.1/pyviz3d/arrow.py`

 * *Files identical despite different names*

### Comparing `pyviz3d_noopen3d-0.3.4/pyviz3d/camera.py` & `pyviz3d_noopen3d-0.3.4.1/pyviz3d/camera.py`

 * *Files identical despite different names*

### Comparing `pyviz3d_noopen3d-0.3.4/pyviz3d/circles_2d.py` & `pyviz3d_noopen3d-0.3.4.1/pyviz3d/circles_2d.py`

 * *Files identical despite different names*

### Comparing `pyviz3d_noopen3d-0.3.4/pyviz3d/cuboid.py` & `pyviz3d_noopen3d-0.3.4.1/pyviz3d/cuboid.py`

 * *Files identical despite different names*

### Comparing `pyviz3d_noopen3d-0.3.4/pyviz3d/labels.py` & `pyviz3d_noopen3d-0.3.4.1/pyviz3d/labels.py`

 * *Files identical despite different names*

### Comparing `pyviz3d_noopen3d-0.3.4/pyviz3d/lines.py` & `pyviz3d_noopen3d-0.3.4.1/pyviz3d/lines.py`

 * *Files identical despite different names*

### Comparing `pyviz3d_noopen3d-0.3.4/pyviz3d/mesh.py` & `pyviz3d_noopen3d-0.3.4.1/pyviz3d/mesh.py`

 * *Files identical despite different names*

### Comparing `pyviz3d_noopen3d-0.3.4/pyviz3d/points.py` & `pyviz3d_noopen3d-0.3.4.1/pyviz3d/points.py`

 * *Files identical despite different names*

### Comparing `pyviz3d_noopen3d-0.3.4/pyviz3d/polyline.py` & `pyviz3d_noopen3d-0.3.4.1/pyviz3d/polyline.py`

 * *Files identical despite different names*

### Comparing `pyviz3d_noopen3d-0.3.4/pyviz3d/src/blender_tools.py` & `pyviz3d_noopen3d-0.3.4.1/pyviz3d/src/blender_tools.py`

 * *Files identical despite different names*

### Comparing `pyviz3d_noopen3d-0.3.4/pyviz3d/src/css/bootstrap.min.css` & `pyviz3d_noopen3d-0.3.4.1/pyviz3d/src/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `pyviz3d_noopen3d-0.3.4/pyviz3d/src/favicon.ico` & `pyviz3d_noopen3d-0.3.4.1/pyviz3d/src/favicon.ico`

 * *Files identical despite different names*

### Comparing `pyviz3d_noopen3d-0.3.4/pyviz3d/src/index.html` & `pyviz3d_noopen3d-0.3.4.1/pyviz3d/src/index.html`

 * *Files identical despite different names*

### Comparing `pyviz3d_noopen3d-0.3.4/pyviz3d/src/js/bootstrap.min.js` & `pyviz3d_noopen3d-0.3.4.1/pyviz3d/src/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `pyviz3d_noopen3d-0.3.4/pyviz3d/src/js/jquery.min.js` & `pyviz3d_noopen3d-0.3.4.1/pyviz3d/src/js/jquery.min.js`

 * *Files identical despite different names*

### Comparing `pyviz3d_noopen3d-0.3.4/pyviz3d/src/js/scene.js` & `pyviz3d_noopen3d-0.3.4.1/pyviz3d/src/js/scene.js`

 * *Files identical despite different names*

### Comparing `pyviz3d_noopen3d-0.3.4/pyviz3d/visualizer.py` & `pyviz3d_noopen3d-0.3.4.1/pyviz3d/visualizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 from .circles_2d import Circles2D
 
 import os
 import sys
 import shutil
 import json
 import numpy as np
+from IPython.display import IFrame, display
+import tempfile
 
 def euler_to_quaternion(x: float, y: float, z: float):
     cr = np.cos(x * 0.5)
     sr = np.sin(x * 0.5)
     cp = np.cos(y * 0.5)
     sp = np.sin(y * 0.5)
     cy = np.cos(z * 0.5)
@@ -109,14 +111,25 @@
         print(
             "************************************************************************"
         )
 
         if blender_args:
             self.show_in_blender(path, blender_args, verbose)
 
+    def show(self, width=800, height=600):
+        # Save the visualization to a temporary HTML file
+        temp_file = tempfile.NamedTemporaryFile(delete=False, suffix='.html')
+        self.save(temp_file.name)
+
+        # Display the HTML visualization in the notebook
+        display(IFrame(src=temp_file.name, width=width, height=height))
+
+        # Clean up the temporary file
+        os.remove(temp_file.name)
+
     def show_in_blender(self,
                         path: str,
                         blender_args: dict,
                         verbose: bool=True):
 
         directory_destination = os.path.abspath(path)
         blender_script_path = os.path.join(directory_destination, "blender_script.py")
@@ -135,15 +148,15 @@
 
         if verbose:
             print("")
             print("************************************************************************")
             print("Blender instructions")
             print(cmd)
             print("************************************************************************")
-        
+
     def add_points(
         self,
         name: str,
         positions: np.array,
         colors: np.array=None,
         normals: np.array=None,
         point_size: int=25,
@@ -187,15 +200,15 @@
     def add_labels(self,
                    name: str,
                    labels: list,
                    positions: np.array,
                    colors: np.array,
                    visible: bool=True):
         """Add labels to the visualizer.
-        
+
         :param name: The name of the labels.
         :param labels: The text value of the labels.
         :param positions: The 3D positions of the labels.
         :param colors: The text color of the individual labels.
         :param visible: Bool if label is visible.
         """
         self.elements[self.__parse_name(name)] = Labels(labels, positions, colors, visible)
@@ -204,15 +217,15 @@
                        name: str,
                        labels: list,
                        positions: np.array,
                        border_colors: np.array,
                        fill_colors: np.array,
                        visible: bool=True):
         """Add node to the visualizer.
-        
+
         :param name: The name of the node.
         :param labels: The text value of the node.
         :param positions: The 3D positions of the node.
         :param border_colors: The text color of the individual node.
         :param fill_colors: The text color of the individual node.
         :param visible: Bool if lines are visible.
         """
@@ -263,15 +276,15 @@
                  path: str,
                  translation: np.array=np.array([0.0, 0.0, 0.0]),
                  rotation: np.array=np.array([0.0, 0.0, 0.0, 1.0]),  # [x, y, z, w] - rotate w degrees rad around the axis xyz
                  scale: np.array=np.array([1, 1, 1]),
                  color: np.array=None,
                  visible: bool=True):
         """Adds a polygon mesh to the scene as specified in the path.
-         
+
           The path is currently limited to .obj files and the color is the uniform color of the objetc.
         """
         rotation /= np.linalg.norm(rotation)  # normalize the orientation
         self.elements[self.__parse_name(name)] = Mesh(path, translation=translation, rotation=rotation, scale=scale, color=color, visible=visible)
 
     def add_polyline(self,
                      name: str,
@@ -365,15 +378,15 @@
 
             x = A * g(v, 2.0 / r) * g(u, 2.0 / r)
             y = B * g(v, 2.0 / s) * f(u, 2.0 / s)
             z = C * f(v, 2.0 / t)
             vertices =  np.concatenate([np.expand_dims(x, 1),
                                         np.expand_dims(y, 1),
                                         np.expand_dims(z, 1)], axis=1)
-            vertices = vertices @ rotation # apply rotation 
+            vertices = vertices @ rotation # apply rotation
 
             triangles = []
             for i in range(N-1):
                 for j in range(N-1):
                     triangles.append([i*N+j, (i+1)*N+j+1, (i+1)*N+j])
                     triangles.append([i*N+j, i*N+(j+1), (i+1)*N+(j+1)])
             return vertices, triangles
@@ -385,15 +398,15 @@
         import open3d as o3d
         mesh_sq = o3d.geometry.TriangleMesh()
         mesh_sq.vertices = o3d.utility.Vector3dVector(vertices)
         mesh_sq.triangles = o3d.utility.Vector3iVector(triangles)
         if not os.path.exists("objs"):
             os.makedirs("objs")
         o3d.io.write_triangle_mesh(f"objs/{name}.obj", mesh_sq, write_ascii=True, compressed=False, write_vertex_normals=False, write_vertex_colors=False, write_triangle_uvs=False, print_progress=False)
-        
+
         id_rot_quat = np.array([1,0,0,0])
         scale = np.array([1.0, 1.0, 1.0])
         self.elements[self.__parse_name(name)] = Mesh(f"objs/{name}.obj", translation=translation, rotation=id_rot_quat, scale=scale, color=color, visible=visible)
 
     def add_arrow(self,
                   name:str,
                   start: np.array,
```

### Comparing `pyviz3d_noopen3d-0.3.4/pyviz3d_noopen3d.egg-info/PKG-INFO` & `pyviz3d_noopen3d-0.3.4.1/pyviz3d_noopen3d.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyviz3d-noopen3d
-Version: 0.3.4
+Version: 0.3.4.1
 Summary: PyViz3D is a python package to visualize 3D scenes.
 Author-email: Francis Engelmann <francis.engelmann@gmail.com>
 License: MIT License
         
         Copyright (c) 2018 Francis Engelmann <francis.engelmann@gmail.com>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pyviz3d_noopen3d-0.3.4/pyviz3d_noopen3d.egg-info/SOURCES.txt` & `pyviz3d_noopen3d-0.3.4.1/pyviz3d_noopen3d.egg-info/SOURCES.txt`

 * *Files identical despite different names*

