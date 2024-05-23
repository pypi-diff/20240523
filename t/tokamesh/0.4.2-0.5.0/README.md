# Comparing `tmp/tokamesh-0.4.2.tar.gz` & `tmp/tokamesh-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tokamesh-0.4.2.tar", last modified: Thu May  9 08:08:10 2024, max compression
+gzip compressed data, was "tokamesh-0.5.0.tar", last modified: Thu May 23 08:03:16 2024, max compression
```

## Comparing `tokamesh-0.4.2.tar` & `tokamesh-0.5.0.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:08:10.678048 tokamesh-0.4.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:08:10.666047 tokamesh-0.4.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:08:10.670047 tokamesh-0.4.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-09 08:07:59.000000 tokamesh-0.4.2/.github/workflows/black.yml
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-05-09 08:07:59.000000 tokamesh-0.4.2/.github/workflows/python_publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-09 08:07:59.000000 tokamesh-0.4.2/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-05-09 08:07:59.000000 tokamesh-0.4.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-09 08:07:59.000000 tokamesh-0.4.2/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-09 08:07:59.000000 tokamesh-0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-05-09 08:08:10.678048 tokamesh-0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-05-09 08:07:59.000000 tokamesh-0.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:08:10.670047 tokamesh-0.4.2/demos/
--rw-r--r--   0 runner    (1001) docker     (127)   139442 2024-05-09 08:07:59.000000 tokamesh-0.4.2/demos/geometry_matrix_demo.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)   472564 2024-05-09 08:07:59.000000 tokamesh-0.4.2/demos/mesh_construction_demo.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:08:10.670047 tokamesh-0.4.2/demos/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     3854 2024-05-09 08:07:59.000000 tokamesh-0.4.2/demos/scripts/geometry_matrix_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-05-09 08:07:59.000000 tokamesh-0.4.2/demos/scripts/geometry_matrix_demo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:08:10.670047 tokamesh-0.4.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-09 08:07:59.000000 tokamesh-0.4.2/docs/docs_requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:08:10.674048 tokamesh-0.4.2/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-09 08:07:59.000000 tokamesh-0.4.2/docs/source/TriangularMesh.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5479 2024-05-09 08:07:59.000000 tokamesh-0.4.2/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-09 08:07:59.000000 tokamesh-0.4.2/docs/source/construction.rst
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-09 08:07:59.000000 tokamesh-0.4.2/docs/source/construction_refinement.rst
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-09 08:07:59.000000 tokamesh-0.4.2/docs/source/geometry.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3835 2024-05-09 08:07:59.000000 tokamesh-0.4.2/docs/source/geometry_background.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-09 08:07:59.000000 tokamesh-0.4.2/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-09 08:07:59.000000 tokamesh-0.4.2/docs/source/operators.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-05-09 08:07:59.000000 tokamesh-0.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 08:08:10.678048 tokamesh-0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 08:07:59.000000 tokamesh-0.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:08:10.674048 tokamesh-0.4.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5016 2024-05-09 08:07:59.000000 tokamesh-0.4.2/tests/test_TriangularMesh.py
--rw-r--r--   0 runner    (1001) docker     (127)    12464 2024-05-09 08:07:59.000000 tokamesh-0.4.2/tests/test_construction.py
--rw-r--r--   0 runner    (1001) docker     (127)     6759 2024-05-09 08:07:59.000000 tokamesh-0.4.2/tests/test_geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     3171 2024-05-09 08:07:59.000000 tokamesh-0.4.2/tests/test_intersection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-05-09 08:07:59.000000 tokamesh-0.4.2/tests/test_operators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:08:10.674048 tokamesh-0.4.2/tokamesh/
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-09 08:07:59.000000 tokamesh-0.4.2/tokamesh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-09 08:08:10.000000 tokamesh-0.4.2/tokamesh/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    26881 2024-05-09 08:07:59.000000 tokamesh-0.4.2/tokamesh/construction.py
--rw-r--r--   0 runner    (1001) docker     (127)    23700 2024-05-09 08:07:59.000000 tokamesh-0.4.2/tokamesh/geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     3662 2024-05-09 08:07:59.000000 tokamesh-0.4.2/tokamesh/intersection.py
--rw-r--r--   0 runner    (1001) docker     (127)    20399 2024-05-09 08:07:59.000000 tokamesh-0.4.2/tokamesh/mesh.py
--rw-r--r--   0 runner    (1001) docker     (127)    10883 2024-05-09 08:07:59.000000 tokamesh-0.4.2/tokamesh/operators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:08:10.678048 tokamesh-0.4.2/tokamesh/tokamaks/
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-09 08:07:59.000000 tokamesh-0.4.2/tokamesh/tokamaks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-05-09 08:07:59.000000 tokamesh-0.4.2/tokamesh/tokamaks/mastu_boundary_data.npz
--rw-r--r--   0 runner    (1001) docker     (127)     5061 2024-05-09 08:07:59.000000 tokamesh-0.4.2/tokamesh/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 08:08:10.678048 tokamesh-0.4.2/tokamesh.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-05-09 08:08:10.000000 tokamesh-0.4.2/tokamesh.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-09 08:08:10.000000 tokamesh-0.4.2/tokamesh.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 08:08:10.000000 tokamesh-0.4.2/tokamesh.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-09 08:08:10.000000 tokamesh-0.4.2/tokamesh.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-09 08:08:10.000000 tokamesh-0.4.2/tokamesh.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:03:16.375682 tokamesh-0.5.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:03:16.367682 tokamesh-0.5.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:03:16.367682 tokamesh-0.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-23 08:03:06.000000 tokamesh-0.5.0/.github/workflows/black.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-05-23 08:03:06.000000 tokamesh-0.5.0/.github/workflows/python_publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-23 08:03:06.000000 tokamesh-0.5.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-05-23 08:03:06.000000 tokamesh-0.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-23 08:03:06.000000 tokamesh-0.5.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-23 08:03:06.000000 tokamesh-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-05-23 08:03:16.375682 tokamesh-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-05-23 08:03:06.000000 tokamesh-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:03:16.367682 tokamesh-0.5.0/demos/
+-rw-r--r--   0 runner    (1001) docker     (127)   118332 2024-05-23 08:03:06.000000 tokamesh-0.5.0/demos/geometry_matrix_demo.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)   472564 2024-05-23 08:03:06.000000 tokamesh-0.5.0/demos/mesh_construction_demo.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:03:16.371682 tokamesh-0.5.0/demos/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-05-23 08:03:06.000000 tokamesh-0.5.0/demos/scripts/geometry_matrix_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-05-23 08:03:06.000000 tokamesh-0.5.0/demos/scripts/geometry_matrix_demo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:03:16.371682 tokamesh-0.5.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-23 08:03:06.000000 tokamesh-0.5.0/docs/docs_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:03:16.371682 tokamesh-0.5.0/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-23 08:03:06.000000 tokamesh-0.5.0/docs/source/TriangularMesh.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5479 2024-05-23 08:03:06.000000 tokamesh-0.5.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-23 08:03:06.000000 tokamesh-0.5.0/docs/source/construction.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-23 08:03:06.000000 tokamesh-0.5.0/docs/source/construction_refinement.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-23 08:03:06.000000 tokamesh-0.5.0/docs/source/geometry.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3835 2024-05-23 08:03:06.000000 tokamesh-0.5.0/docs/source/geometry_background.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-23 08:03:06.000000 tokamesh-0.5.0/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-23 08:03:06.000000 tokamesh-0.5.0/docs/source/operators.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-05-23 08:03:06.000000 tokamesh-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 08:03:16.375682 tokamesh-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 08:03:06.000000 tokamesh-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:03:16.371682 tokamesh-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5696 2024-05-23 08:03:06.000000 tokamesh-0.5.0/tests/test_TriangularMesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12464 2024-05-23 08:03:06.000000 tokamesh-0.5.0/tests/test_construction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6566 2024-05-23 08:03:06.000000 tokamesh-0.5.0/tests/test_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3171 2024-05-23 08:03:06.000000 tokamesh-0.5.0/tests/test_intersection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-05-23 08:03:06.000000 tokamesh-0.5.0/tests/test_operators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:03:16.375682 tokamesh-0.5.0/tokamesh/
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-23 08:03:06.000000 tokamesh-0.5.0/tokamesh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-23 08:03:16.000000 tokamesh-0.5.0/tokamesh/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27188 2024-05-23 08:03:06.000000 tokamesh-0.5.0/tokamesh/construction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30294 2024-05-23 08:03:06.000000 tokamesh-0.5.0/tokamesh/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3662 2024-05-23 08:03:06.000000 tokamesh-0.5.0/tokamesh/intersection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21876 2024-05-23 08:03:06.000000 tokamesh-0.5.0/tokamesh/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10327 2024-05-23 08:03:06.000000 tokamesh-0.5.0/tokamesh/operators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:03:16.375682 tokamesh-0.5.0/tokamesh/tokamaks/
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-23 08:03:06.000000 tokamesh-0.5.0/tokamesh/tokamaks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-05-23 08:03:06.000000 tokamesh-0.5.0/tokamesh/tokamaks/mastu_boundary_data.npz
+-rw-r--r--   0 runner    (1001) docker     (127)    10072 2024-05-23 08:03:06.000000 tokamesh-0.5.0/tokamesh/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:03:16.375682 tokamesh-0.5.0/tokamesh.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4034 2024-05-23 08:03:16.000000 tokamesh-0.5.0/tokamesh.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-23 08:03:16.000000 tokamesh-0.5.0/tokamesh.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 08:03:16.000000 tokamesh-0.5.0/tokamesh.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-23 08:03:16.000000 tokamesh-0.5.0/tokamesh.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-23 08:03:16.000000 tokamesh-0.5.0/tokamesh.egg-info/top_level.txt
```

### Comparing `tokamesh-0.4.2/.github/workflows/black.yml` & `tokamesh-0.5.0/.github/workflows/black.yml`

 * *Files identical despite different names*

### Comparing `tokamesh-0.4.2/.github/workflows/python_publish.yml` & `tokamesh-0.5.0/.github/workflows/python_publish.yml`

 * *Files identical despite different names*

### Comparing `tokamesh-0.4.2/.github/workflows/tests.yml` & `tokamesh-0.5.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `tokamesh-0.4.2/.gitignore` & `tokamesh-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `tokamesh-0.4.2/.readthedocs.yaml` & `tokamesh-0.5.0/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `tokamesh-0.4.2/LICENSE` & `tokamesh-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tokamesh-0.4.2/PKG-INFO` & `tokamesh-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tokamesh
-Version: 0.4.2
+Version: 0.5.0
 Summary: Python tools for constructing meshes and geometry matrices used in tomography problems
 Author-email: Chris Bowman <chris.bowman.physics@gmail.com>
 License: MIT License
         
         Copyright (c) 2021 Chris Bowman
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `tokamesh-0.4.2/README.md` & `tokamesh-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `tokamesh-0.4.2/demos/mesh_construction_demo.ipynb` & `tokamesh-0.5.0/demos/mesh_construction_demo.ipynb`

 * *Files identical despite different names*

### Comparing `tokamesh-0.4.2/demos/scripts/geometry_matrix_benchmark.py` & `tokamesh-0.5.0/demos/scripts/geometry_matrix_benchmark.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from numpy import linspace, array, zeros, sqrt, sinc
-from scipy.sparse import csc_matrix
 from numpy.random import multivariate_normal
 from scipy.integrate import simps
 import matplotlib.pyplot as plt
 
 from tokamesh.construction import equilateral_mesh
 from tokamesh import TriangularMesh
-from tokamesh.geometry import BarycentricGeometryMatrix
+from tokamesh.geometry import calculate_geometry_matrix
 from tokamesh.utilities import Camera
 
+
 """
 This script demonstrates that line-integrals over rays through a field
 defined by barycentric interpolation on a mesh are calculated correctly
 by geometry matrices produced by the BarycentricGeometryMatrix class.
 """
 
 # build a basic mesh out of equilateral triangles
@@ -22,53 +22,49 @@
 # generate a random test field using a gaussian process
 distance = sqrt((R[:, None] - R[None, :]) ** 2 + (z[:, None] - z[None, :]) ** 2)
 scale = 0.04
 covariance = sinc(distance / scale) ** 2
 field = multivariate_normal(zeros(R.size), covariance)
 field -= field.min()
 
-# Generate an image of the field on the mesh
-R_axis, z_axis, field_image = mesh.get_field_image(field, shape=(200, 150))
 
 # plot the test field
 from matplotlib import colormaps
 
 cmap = colormaps["viridis"]
 
 fig = plt.figure(figsize=(7, 7))
-ax1 = fig.add_subplot(111)
-ax1.contourf(R_axis, z_axis, field_image.T, 30)
+ax1 = fig.add_subplot(1, 1, 1)
+mesh.plot_field(ax1, field, mesh_color="white", colormap=cmap)
 ax1.set_facecolor(cmap(0.0))
-mesh.draw(ax1, lw=0.25, color="white")
 ax1.axis("equal")
 ax1.set_title("Gaussian random field on the mesh")
 plt.tight_layout()
 plt.show()
 
 
 # generate a synthetic camera to image the field
 cam_position = array([0.17, 0.19, 0.18])
 cam_direction = array([-0.1, -0.1, -0.06])
 cam = Camera(
     position=cam_position, direction=cam_direction, max_distance=1.0, num_x=5, num_y=15
 )
 
 # calculate the geometry matrix data
-BGM = BarycentricGeometryMatrix(
-    R=R, z=z, triangles=triangles, ray_origins=cam.ray_starts, ray_ends=cam.ray_ends
+geomat = calculate_geometry_matrix(
+    R=R,
+    z=z,
+    triangles=triangles,
+    ray_origins=cam.ray_starts,
+    ray_ends=cam.ray_ends,
+    n_processes=2,
 )
 
-matrix_data = BGM.calculate()
-
-# extract the data and build a sparse matrix
-entry_values = matrix_data["entry_values"]
-row_values = matrix_data["row_indices"]
-col_values = matrix_data["col_indices"]
-shape = matrix_data["shape"]
-G = csc_matrix((entry_values, (row_values, col_values)), shape=shape)
+# create a sparse array instance of the geometry matrix
+G = geomat.build_sparse_array()
 
 # get the geometry matrix prediction of the line-integrals
 matrix_integrals = G @ field
 
 # manually calculate the line integrals for comparison
 L = linspace(0, 0.5, 3000)  # build a distance axis for the integrals
 # get the position of each ray at each distance
@@ -80,15 +76,15 @@
         R_projection[:, i], z_projection[:, i], vertex_values=field
     )
     direct_integrals[i] = simps(samples, x=L)
 
 
 # plot the results
 fig = plt.figure(figsize=(12, 6))
-ax1 = fig.add_subplot(211)
+ax1 = fig.add_subplot(2, 1, 1)
 ax1.plot(direct_integrals, "-", label="brute-force result", c="red")
 ax1.plot(
     matrix_integrals,
     label="geometry matrix result",
     marker="o",
     markerfacecolor="none",
     ls="none",
@@ -99,24 +95,24 @@
 ax1.set_ylabel("line-integral prediction")
 ax1.set_xlim([-2, 77])
 ax1.grid()
 ax1.legend()
 
 abs_frac_diff = abs(matrix_integrals / direct_integrals - 1)
 mean_afd = abs_frac_diff.mean()
-ax2 = fig.add_subplot(212)
+ax2 = fig.add_subplot(2, 1, 2)
 ax2.plot(abs_frac_diff, c="green", alpha=0.5)
 ax2.plot(abs_frac_diff, ".", c="green", markersize=4)
 ax2.plot(
     [-10, 85],
     [mean_afd, mean_afd],
     ls="dashed",
     c="red",
     lw=2,
-    label="{:.3%} mean absolute fractional difference".format(mean_afd),
+    label=f"{mean_afd:.3%} mean absolute fractional difference",
 )
 ax2.set_ylim([1e-5, 1e-2])
 ax2.set_yscale("log")
 ax2.set_xlim([-1, 75])
 ax2.set_xlabel("Pixel-ray number")
 ax2.set_ylabel("absolute fractional difference")
 ax2.grid()
```

### Comparing `tokamesh-0.4.2/demos/scripts/geometry_matrix_demo.py` & `tokamesh-0.5.0/demos/scripts/geometry_matrix_demo.py`

 * *Files identical despite different names*

### Comparing `tokamesh-0.4.2/docs/source/conf.py` & `tokamesh-0.5.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `tokamesh-0.4.2/docs/source/geometry_background.rst` & `tokamesh-0.5.0/docs/source/geometry_background.rst`

 * *Files identical despite different names*

### Comparing `tokamesh-0.4.2/docs/source/index.rst` & `tokamesh-0.5.0/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `tokamesh-0.4.2/pyproject.toml` & `tokamesh-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [build-system]
 requires = [
-    "setuptools >= 42",
+    "setuptools >= 61",
     "setuptools_scm[toml] >= 6.2",
     "setuptools_scm_git_archive",
     "wheel >= 0.29.0",
 ]
 build-backend = "setuptools.build_meta"
```

### Comparing `tokamesh-0.4.2/tests/test_TriangularMesh.py` & `tokamesh-0.5.0/tests/test_TriangularMesh.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import pytest
-from numpy import arange, array, sin, cos, pi, isclose, ones
-from numpy.random import uniform, seed
+from numpy import arange, array, sin, cos, pi, isclose, ones, sqrt, sinc, zeros
+from numpy.random import uniform, seed, multivariate_normal
 from tokamesh import TriangularMesh
 from tokamesh.utilities import BinaryTree
 from tokamesh.construction import equilateral_mesh
+import matplotlib.pyplot as plt
 from hypothesis import given, strategies as st
 
 
 @given(st.floats(-4, 8))
 def test_binary_tree(value):
     limit_left, limit_right = -4, 8
 
@@ -138,7 +139,30 @@
     # ideally we should find a way to generate lots of random
     # points just outside the boundary of the mesh to check.
 
 
 def test_find_triangle_inconsistent_shapes(mesh):
     with pytest.raises(ValueError):
         mesh.find_triangle(ones([2, 1]), ones([2, 3]))
+
+
+def test_plot_field(mesh):
+    # generate a random test field using a gaussian process
+    distance = sqrt(
+        (mesh.R[:, None] - mesh.R[None, :]) ** 2
+        + (mesh.z[:, None] - mesh.z[None, :]) ** 2
+    )
+    scale = 0.04
+    covariance = sinc(distance / scale) ** 2
+    field = multivariate_normal(zeros(mesh.R.size), covariance)
+    field -= field.min()
+
+    fig = plt.figure(figsize=(7, 7))
+    ax = fig.add_subplot(1, 1, 1)
+    mesh.plot_field(
+        ax=ax,
+        vertex_values=field,
+        colormap="Blues",
+        mesh_color="black",
+        mesh_thickness=0.4,
+    )
+    plt.close()
```

### Comparing `tokamesh-0.4.2/tests/test_construction.py` & `tokamesh-0.5.0/tests/test_construction.py`

 * *Files identical despite different names*

### Comparing `tokamesh-0.4.2/tests/test_geometry.py` & `tokamesh-0.5.0/tests/test_geometry.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,75 +1,72 @@
 from numpy import sqrt, sinc, sin, cos, pi, exp
 from numpy import array, linspace, zeros, array_equal, piecewise
-from scipy.sparse import csc_matrix
-from numpy.random import multivariate_normal
-from scipy.integrate import quad, simps
+from numpy.random import default_rng
+from scipy.integrate import quad, simpson
 
 from tokamesh.construction import equilateral_mesh
 from tokamesh import TriangularMesh
-from tokamesh.geometry import BarycentricGeometryMatrix, linear_geometry_matrix
-from tokamesh.geometry import radius_hyperbolic_integral
+from tokamesh.geometry import calculate_geometry_matrix
+from tokamesh.geometry import radius_hyperbolic_integral, linear_geometry_matrix
 from tokamesh.utilities import build_edge_map, Camera
 
 
-def test_BarycentricGeometryMatrix():
+def test_geometry_matrix_calculation():
     # build a basic mesh out of equilateral triangles
     R, z, triangles = equilateral_mesh(
         resolution=0.01, R_range=[0, 0.2], z_range=[-0.2, 0.2]
     )
     mesh = TriangularMesh(R, z, triangles)
 
     # generate a random test field using a gaussian process
     distance = sqrt((R[:, None] - R[None, :]) ** 2 + (z[:, None] - z[None, :]) ** 2)
     scale = 0.04
     covariance = sinc(distance / scale) ** 2
-    field = multivariate_normal(zeros(R.size), covariance)
+
+    rng = default_rng(123)
+    field = rng.multivariate_normal(zeros(R.size), covariance)
     field -= field.min()
 
     # generate a synthetic camera to image the field
     cam_position = array([0.17, 0.19, 0.18])
     cam_direction = array([-0.1, -0.1, -0.06])
     cam = Camera(
         position=cam_position,
         direction=cam_direction,
         max_distance=1.0,
         num_x=5,
         num_y=15,
     )
 
-    # calculate the geometry matrix data
-    BGM = BarycentricGeometryMatrix(
-        R=R, z=z, triangles=triangles, ray_origins=cam.ray_starts, ray_ends=cam.ray_ends
-    )
-
-    matrix_data = BGM.calculate()
-
-    # extract the data and build a sparse matrix
-    entry_values = matrix_data["entry_values"]
-    row_values = matrix_data["row_indices"]
-    col_values = matrix_data["col_indices"]
-    shape = matrix_data["shape"]
-    G = csc_matrix((entry_values, (row_values, col_values)), shape=shape)
-
-    # get the geometry matrix prediction of the line-integrals
-    matrix_integrals = G @ field
-
     # manually calculate the line integrals for comparison
     L = linspace(0, 1.0, 3000)  # build a distance axis for the integrals
     # get the position of each ray at each distance
     R_projection, z_projection = cam.project_rays(L)
     # directly integrate along each ray
     direct_integrals = zeros(R_projection.shape[1])
     for i in range(R_projection.shape[1]):
         samples = mesh.interpolate(
             R_projection[:, i], z_projection[:, i], vertex_values=field
         )
-        direct_integrals[i] = simps(samples, x=L)
+        direct_integrals[i] = simpson(samples, x=L)
+
+    for n_procs in [1, 2, 3]:
+        geomat = calculate_geometry_matrix(
+            R=R,
+            z=z,
+            triangles=triangles,
+            ray_origins=cam.ray_starts,
+            ray_ends=cam.ray_ends,
+            n_processes=n_procs,
+        )
 
-    assert (abs(direct_integrals - matrix_integrals) < 1e-3).all()
+        G = geomat.build_sparse_array()
+        # get the geometry matrix prediction of the line-integrals
+        matrix_integrals = G @ field
+        assert (abs(direct_integrals / matrix_integrals - 1) < 1e-3).all()
 
 
 def test_radius_hyperbolic_integral():
     # testing analytic integral solution of following function:
     def R(l, l_tan, R_tan_sq, sqrt_q2):
         return sqrt((sqrt_q2 * (l - l_tan)) ** 2 + R_tan_sq)
 
@@ -158,24 +155,24 @@
     R = linspace(0.25, 1.6, n_points)
     z1 = (R - 1.4) / 0.05
     z2 = (R - 0.35) / 0.02
     emission = exp(-0.5 * z1**2) + 0.5 * exp(-0.5 * z2**2) + 0.005
 
     # Use geometry matrix to calculate the analytic integral result
     G = linear_geometry_matrix(R=R, ray_origins=origins, ray_ends=ends)
-    analytic_integral = G.dot(emission)
+    analytic_integral = G @ emission
 
     # Directly integrate over the basis functions to get the numerical integral
     basis = [LinearBF(R[0] - 1e-5, R[0], R[1])]
     basis.extend([LinearBF(R[i - 1], R[i], R[i + 1]) for i in range(1, n_points - 1)])
     basis.append(LinearBF(R[-2], R[-1], R[-1] + 1e-5))
     numerical_integral = zeros(n_rays)
     for i in range(n_rays):
         L = linspace(0, lengths[i], 5000)
         x_ray = rays[i, 0] * L + origins[i, 0]
         y_ray = rays[i, 1] * L + origins[i, 1]
         R = sqrt(x_ray**2 + y_ray**2)
         F = sum(w * lbf(R) for lbf, w in zip(basis, emission))
-        numerical_integral[i] = simps(F, x=L)
+        numerical_integral[i] = simpson(F, x=L)
 
     # check that analytic integral agrees with numerical one
     assert abs(analytic_integral - numerical_integral).max() < 1e-5
```

### Comparing `tokamesh-0.4.2/tests/test_intersection.py` & `tokamesh-0.5.0/tests/test_intersection.py`

 * *Files identical despite different names*

### Comparing `tokamesh-0.4.2/tests/test_operators.py` & `tokamesh-0.5.0/tests/test_operators.py`

 * *Files identical despite different names*

### Comparing `tokamesh-0.4.2/tokamesh/construction.py` & `tokamesh-0.5.0/tokamesh/construction.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from numpy import sqrt, ceil, sin, cos, arctan2, diff, minimum, maximum, cumsum
 from numpy import array, ones, zeros, full, linspace, arange, concatenate, vstack
 from numpy import in1d, unique, isclose, nan, atleast_1d, intersect1d
 from numpy import int64, ndarray
 from warnings import warn
 
-from tokamesh.utilities import build_edge_map
-
+from tokamesh.utilities import build_edge_map, map_edge_connections
 
 MeshData = tuple[ndarray, ndarray, ndarray]
 floatpair = tuple[float, float]
 
 
 def equilateral_mesh(
     R_range: floatpair,
@@ -256,23 +255,28 @@
     # Construct a mapping from triangles to edges, and edges to vertices
     triangle_edges, edge_vertices, _ = build_edge_map(triangles)
     # identify edges on the boundary by finding edges which are only part of one triangle
     unique_vals, counts = unique(triangle_edges, return_counts=True)
     boundary_edges_indices = (counts == 1).nonzero()[0]
     boundary_edges = edge_vertices[boundary_edges_indices, :]
 
-    # now create a map between an edge, and the other edges to which it's connected
-    boundary_connections = {}
-    for i in range(boundary_edges.shape[0]):
-        edges = (
-            (boundary_edges[i, 0] == boundary_edges)
-            | (boundary_edges[i, 1] == boundary_edges)
-        ).nonzero()[0]
-        boundary_connections[i] = [e for e in edges if e != i]
+    _, edges_per_vertex = unique(boundary_edges, return_counts=True)
+    if edges_per_vertex.max() > 2:
+        warn(
+            """\n
+            \r[ find_boundaries warning ]
+            \r>> The given mesh contains at least two sub-meshes which
+            \r>> are connected by only one vertex. Currently, it is not
+            \r>> guaranteed that find_boundaries will draw separate
+            \r>> boundaries for each sub-mesh.
+            """
+        )
 
+    # now create a map between an edge, and the other edges to which it's connected
+    boundary_connections = map_edge_connections(boundary_edges)
     # we use a set to keep track of which edges have already been used as part of a boundary
     unused_edges = {i for i in range(boundary_edges.shape[0])}
 
     # now follow the connections map to build the boundaries
     boundaries = []
     while len(unused_edges) > 0:
         current_boundary = [unused_edges.pop()]  # start at an arbitrary unused edge
@@ -283,26 +287,14 @@
                     current_boundary.append(edge)
                     unused_edges.remove(edge)
                     break
             else:
                 break
         boundaries.append(boundary_edges_indices[current_boundary])
 
-    _, edges_per_vertex = unique(boundary_edges, return_counts=True)
-    if edges_per_vertex.max() > 2:
-        warn(
-            """\n
-            [ find_boundaries warning ]
-            >> The given mesh contains at least two sub-meshes which
-            >> are connected by only one vertex. Currently, it is not
-            >> guaranteed that find_boundaries will draw separate
-            >> boundaries for each sub-mesh.
-            """
-        )
-
     # Now we need to convert the boundaries from edge indices to vertex indices
     vertex_boundaries = []
     for boundary in boundaries:
         # the order of the first two vertex indices needs to match the direction
         # in which the boundary is being traced.
         v1, v2 = edge_vertices[boundary[0], :]
         if v1 in edge_vertices[boundary[1], :]:
@@ -549,14 +541,15 @@
     R_boundary: ndarray,
     z_boundary: ndarray,
     resolution: float,
     edge_resolution: float = None,
     edge_padding: float = 0.75,
     edge_max_area: float = 1.1,
     rotation: float = None,
+    central_mesh: MeshData = None,
 ) -> MeshData:
     """
     Generate a triangular mesh which fills the space inside a given boundary using a 2-stage
     process. First, a mesh of equilateral triangles is created which fills the space up to a
     chosen minimum distance from the boundary. An irregular mesh is then generated which fills
     the space between the central equilateral mesh and the boundary. The two meshes are then
     merged, and the resulting mesh is returned.
@@ -588,29 +581,38 @@
         irregular edge mesh, such that no triangle will have an area larger than
         ``edge_max_area`` times the target area set by the ``edge_resolution`` argument.
 
     :param rotation: \
         Angle (in radians) by which the orientations of triangles in the central
         equilateral mesh are rotated, relative to their default orientation.
 
+    :param central_mesh: \
+        Allows the central mesh to be specified directly rather than being generated
+        automatically. The central mesh data is specified as a tuple of numpy arrays
+        specifying the major radius of the vertices, the z-height of the vertices and
+        the indices of the triangles respectively.
+
     :return: \
         A tuple containing ``R_vert``, ``z_vert`` and ``triangles``.
         ``R_vert`` is the major-radius of the vertices as a 1D array. ``z_vert`` the is
         z-height of the vertices as a 1D array. ``triangles`` is a 2D array of integers
         of shape ``(N,3)`` specifying the indices of the vertices which form each triangle
         in the mesh, where ``N`` is the total number of triangles.
     """
     # build the central mesh
-    central_R, central_z, central_triangles = build_central_mesh(
-        R_boundary=R_boundary,
-        z_boundary=z_boundary,
-        resolution=resolution,
-        padding_factor=edge_padding,
-        rotation=rotation,
-    )
+    if central_mesh is None:
+        central_R, central_z, central_triangles = build_central_mesh(
+            R_boundary=R_boundary,
+            z_boundary=z_boundary,
+            resolution=resolution,
+            padding_factor=edge_padding,
+            rotation=rotation,
+        )
+    else:
+        central_R, central_z, central_triangles = central_mesh
 
     # find all boundaries on the central mesh
     boundaries = find_boundaries(central_triangles)
     # if there is more than one boundary, then there are multiple sub-meshes
     # pick the largest boundary, and discard any vertices which are outside of it
     boundaries = sorted(boundaries, key=lambda x: len(x))
     central_boundary = boundaries[-1]
```

### Comparing `tokamesh-0.4.2/tokamesh/geometry.py` & `tokamesh-0.5.0/tokamesh/geometry.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,219 @@
 from numpy import sqrt, log
 from numpy import absolute, nan, isfinite, minimum, maximum, isnan
-from numpy import array, full, zeros, stack, savez, concatenate
+from numpy import array, full, zeros, stack, savez, concatenate, load
 from numpy import ndarray, finfo
+from scipy.sparse import csc_array
 from collections import defaultdict
+from dataclasses import dataclass
+from multiprocessing import Process, Pipe
+from multiprocessing.connection import Connection
 from time import perf_counter
 import sys
 
-from tokamesh.utilities import build_edge_map
+from tokamesh.utilities import build_edge_map, partition_triangles
 
 
-class BarycentricGeometryMatrix:
+@dataclass
+class GeometryMatrix:
+    """
+    A class for packaging and manipulating geometry matrix data.
+
+    :ivar entry_values: \
+        The values of the non-zero matrix elements as a numpy ``ndarray``.
+
+    :ivar row_indices: \
+        The row indices of the non-zero matrix elements as a numpy ``ndarray``.
+
+    :ivar col_indices: \
+        The column indices of the non-zero matrix elements as a numpy ``ndarray``.
+
+    :ivar matrix_shape: \
+        The shape of the geometry matrix as a numpy ``ndarray``.
+
+    :ivar R_vertices: \
+        The major-radius of the triangular mesh vertices as a numpy ``ndarray``.
+
+    :ivar z_vertices: \
+        The z-height of the triangular mesh vertices as a numpy ``ndarray``.
+
+    :ivar triangle_vertices: \
+        A 2D numpy ``ndarray`` of integers specifying the indices of the vertices which
+        form each of the triangles in the mesh. The array has shape ``(N,3)`` where
+        ``N`` is the total number of triangles.
+    """
+
+    entry_values: ndarray
+    row_indices: ndarray
+    col_indices: ndarray
+    matrix_shape: ndarray
+    R_vertices: ndarray
+    z_vertices: ndarray
+    triangle_vertices: ndarray
+
+    def build_sparse_array(self, sparse_array_type=csc_array):
+        """
+        :param sparse_array_type: \
+            A sparse array type from ``scipy.sparse``.
+
+        :return: \
+            The geometry matrix as an instance of the given sparse array type.
+        """
+        return sparse_array_type(
+            (self.entry_values, (self.row_indices, self.col_indices)),
+            shape=self.matrix_shape,
+        )
+
+    def save(self, filename: str):
+        """
+        Save the geometry matrix data in the numpy ``.npz`` format.
+        
+        :param filename: \
+            The filename to which the geometry matrix data is saved.
+        """
+        savez(
+            filename,
+            entry_values=self.entry_values,
+            row_indices=self.row_indices,
+            col_indices=self.col_indices,
+            matrix_shape=self.matrix_shape,
+            R_vertices=self.R_vertices,
+            z_vertices=self.z_vertices,
+            triangle_vertices=self.triangle_vertices,
+        )
+
+    @classmethod
+    def load(cls, filename: str):
+        """
+        Load and return a saved ``GeometryMatrix`` instance from file.
+
+        :param filename: \
+            The filename of the saved geometry matrix data.
+
+        :return: \
+            The loaded data as a ``GeometryMatrix`` instance.
+        """
+        data = load(filename)
+        return cls(
+            entry_values=data["entry_values"],
+            row_indices=data["row_indices"],
+            col_indices=data["col_indices"],
+            matrix_shape=data["matrix_shape"],
+            R_vertices=data["R_vertices"],
+            z_vertices=data["z_vertices"],
+            triangle_vertices=data["triangle_vertices"],
+        )
+
+
+def calculate_geometry_matrix(
+    R: ndarray,
+    z: ndarray,
+    triangles: ndarray,
+    ray_origins: ndarray,
+    ray_ends: ndarray,
+    n_processes: int,
+) -> GeometryMatrix:
+    """
+    Calculate a geometry matrix over a given triangular mesh using
+    barycentric linear interpolation.
+
+    :param R: \
+        The major radius of each mesh vertex as a 1D numpy array.
+
+    :param z: \
+        The z-height of each mesh vertex as a 1D numpy array.
+
+    :param triangles: \
+        A 2D numpy array of integers specifying the indices of the vertices which form
+        each of the triangles in the mesh. The array must have shape ``(N,3)`` where
+        ``N`` is the total number of triangles.
+
+    :param ray_origins: \
+        The ``(x,y,z)`` position vectors of the origin of each ray (i.e. line-of-sight)
+        as a 2D numpy array. The array must have shape ``(M,3)`` where ``M`` is the
+        total number of rays.
+
+    :param ray_ends: \
+        The ``(x,y,z)`` position vectors of the end-points of each ray (i.e. line-of-sight)
+        as a 2D numpy array. The array must have shape ``(M,3)`` where ``M`` is the
+        total number of rays.
+
+    :param n_processes: \
+        Number of processes over which the computation is distributed.
+
+    :return: \
+        A ``GeometryMatrix`` object containing the geometry matrix data - see the
+        documentation for ``GeometryMatrix`` for details.
+    """
+    t_start = perf_counter()
+    dt = perf_counter() - t_start
+    sys.stdout.write(
+        f"\r >> Calculating geometry matrix...                                         "
+    )
+    sys.stdout.flush()
+
+    GC = GeometryCalculator(
+        R=R,
+        z=z,
+        triangles=triangles,
+        ray_origins=ray_origins,
+        ray_ends=ray_ends,
+    )
+
+    index_groups = partition_triangles(
+        R=R, z=z, triangles=triangles, partitions=n_processes
+    )
+
+    # calculate the contribution to the matrix for each triangle
+    # Spawn a separate process for each chain object
+    processes = []
+    connections = []
+    for indices in index_groups:
+        parent_ctn, child_ctn = Pipe()
+        connections.append(parent_ctn)
+        p = Process(
+            target=triangle_process,
+            args=(GC, indices, child_ctn),
+        )
+        processes.append(p)
+
+    [p.start() for p in processes]
+    vertex_maps = [pipe.recv() for pipe in connections]
+    [p.join() for p in processes]
+
+    GF = GeometryFactors()
+    for v in vertex_maps:
+        for inds, value in v.items():
+            GF.vertex_map[inds] += value
+
+    t_elapsed = perf_counter() - t_start
+    mins, secs = divmod(t_elapsed, 60)
+    hrs, mins = divmod(mins, 60)
+    time_taken = f"{int(hrs)}:{int(mins):02d}:{int(secs):02d}"
+    sys.stdout.write(
+        f"\r >> Calculating geometry matrix:  [ completed in {time_taken} ]            "
+    )
+    sys.stdout.flush()
+    sys.stdout.write("\n")
+
+    # convert the calculated matrix elements to a form appropriate for sparse arrays
+    data_vals, vertex_inds, ray_inds = GF.get_sparse_matrix_data()
+
+    return GeometryMatrix(
+        entry_values=data_vals,
+        row_indices=ray_inds,
+        col_indices=vertex_inds,
+        matrix_shape=array([GC.n_rays, GC.n_vertices]),
+        R_vertices=R,
+        z_vertices=z,
+        triangle_vertices=triangles,
+    )
+
+
+class GeometryCalculator:
     """
     Class for calculating geometry matrices over triangular meshes using
     barycentric linear interpolation.
 
     :param R: \
         The major radius of each mesh vertex as a 1D numpy array.
 
@@ -135,15 +335,15 @@
             the dictionary is as follows: ``entry_values`` is a 1D numpy array containing
             the values of all non-zero matrix entries. ``row_indices`` is a 1D numpy
             array containing the row-index of each of the non-zero entries. ``col_indices``
             is a 1D numpy array containing the column-index of each of the non-zero entries.
             ``shape`` is a 1D numpy array containing the dimensions of the matrix. The
             arrays defining the mesh are also stored as ``R``, ``z`` and ``triangles``.
         """
-        # clear the geometry factors in case they contains data from a previous calculation
+        # clear the geometry factors in case they contain data from a previous calculation
         self.GeomFacs.vertex_map.clear()
         # process the first triangle so we can estimate the run-time
         t_start = perf_counter()
         self.process_triangle(0)
         dt = perf_counter() - t_start
 
         # use the estimate to break the evaluation into groups
@@ -299,15 +499,15 @@
         valid_intersections = isfinite(intersections)
         intersection_count = valid_intersections.sum(axis=1)
         # At this point, each ray should have an even number of intersections, if any
         # have an odd number then something has gone wrong, so raise an error.
         if (intersection_count % 2 == 1).any():
             raise ValueError(
                 f"""\n\n
-                \r[ BarycentricGeometryMatrix error ]
+                \r[ GeometryCalculator error ]
                 \r>> One or more rays has an odd number of intersections with
                 \r>> triangle {tri_index}. This is typically caused by insufficient
                 \r>> floating-point precision in the intersection calculations.
                 """
             )
 
         max_intersections = intersection_count.max()
@@ -368,46 +568,46 @@
         Check that all the data have the correct shapes / types
         """
         if not all(
             type(arg) is ndarray for arg in [R, z, triangle_inds, ray_starts, ray_ends]
         ):
             raise TypeError(
                 """\n\n
-                \r[ BarycentricGeometryMatrix error ]
+                \r[ GeometryCalculator error ]
                 \r>> All arguments must be of type numpy.ndarray.
                 """
             )
 
         if R.ndim != 1 or z.ndim != 1 or R.size != z.size:
             raise ValueError(
                 """\n\n
-                \r[ BarycentricGeometryMatrix error ]
+                \r[ GeometryCalculator error ]
                 \r>> 'R' and 'z' arguments must be 1-dimensional arrays of equal length.
                 """
             )
 
         if triangle_inds.ndim != 2 or triangle_inds.shape[1] != 3:
             raise ValueError(
                 """\n\n
-                \r[ BarycentricGeometryMatrix error ]
+                \r[ GeometryCalculator error ]
                 \r>> 'triangle_inds' argument must be a 2-dimensional array of shape (N,3)
                 \r>> where 'N' is the total number of triangles.
                 """
             )
 
         if (
             ray_starts.ndim != 2
             or ray_ends.ndim != 2
             or ray_starts.shape[1] != 3
             or ray_ends.shape[1] != 3
             or ray_ends.shape[0] != ray_starts.shape[0]
         ):
             raise ValueError(
                 """\n\n
-                \r[ BarycentricGeometryMatrix error ]
+                \r[ GeometryCalculator error ]
                 \r>> 'ray_starts' and 'ray_ends' arguments must be 2-dimensional arrays
                 \r>> of shape (M,3), where 'M' is the total number of rays.
                 """
             )
 
         for tag, arr in [
             ("R", R),
@@ -415,15 +615,15 @@
             ("ray_starts", ray_starts),
             ("ray_ends", ray_ends),
         ]:
             float_precision = finfo(arr.dtype).precision
             if float_precision < 15:
                 raise ValueError(
                     f"""\n\n
-                    \r[ BarycentricGeometryMatrix error ]
+                    \r[ GeometryCalculator error ]
                     \r>> The '{tag}' argument array has a data-type of {arr.dtype}
                     \r>> with a decimal precision of {float_precision}.
                     \r>> Arrays should use at least 64-bit floats, such that the
                     \r>> decimal precision is 15 or above.
                     """
                 )
 
@@ -436,27 +636,36 @@
 
     ratio = (u2 + R2) / (u1 + R1)
     return 0.5 * (u2 * R2 - u1 * R1 + log(ratio) * R_tan_sqr) / sqrt_q2
 
 
 class GeometryFactors:
     def __init__(self):
-        self.vertex_map = defaultdict(lambda: 0.0)
+        self.vertex_map = defaultdict(float)
 
     def update_vertex(self, vertex_ind, ray_indices, integral_vals):
         for ray_idx, value in zip(ray_indices, integral_vals):
             self.vertex_map[(vertex_ind, ray_idx)] += value
 
     def get_sparse_matrix_data(self):
-        vertex_inds = array([key[0] for key in self.vertex_map.keys()])
-        ray_inds = array([key[1] for key in self.vertex_map.keys()])
+        vertex_inds = array([key[0] for key in self.vertex_map.keys()], dtype=int)
+        ray_inds = array([key[1] for key in self.vertex_map.keys()], dtype=int)
         data_vals = array([v for v in self.vertex_map.values()])
         return data_vals, vertex_inds, ray_inds
 
 
+def triangle_process(
+    calculator: GeometryCalculator,
+    triangle_indices: ndarray,
+    connection: Connection,
+):
+    [calculator.process_triangle(i) for i in triangle_indices]
+    connection.send(calculator.GeomFacs.vertex_map)
+
+
 def linear_geometry_matrix(
     R: ndarray, ray_origins: ndarray, ray_ends: ndarray
 ) -> ndarray:
     """
     Calculates a geometry matrix using 1D linear-interpolation basis functions
     assuming that the emission varies only as a function of major-radius.
```

### Comparing `tokamesh-0.4.2/tokamesh/intersection.py` & `tokamesh-0.5.0/tokamesh/intersection.py`

 * *Files identical despite different names*

### Comparing `tokamesh-0.4.2/tokamesh/mesh.py` & `tokamesh-0.5.0/tokamesh/mesh.py`

 * *Files 3% similar despite different names*

```diff
@@ -319,15 +319,62 @@
         if ("color" not in kwargs) and ("c" not in kwargs):
             kwargs["color"] = "black"
         ax.plot(self.R_edges[0, :].T, self.z_edges[0, :].T, **kwargs)
         if "label" in kwargs:
             kwargs["label"] = None
         ax.plot(self.R_edges[1:, :].T, self.z_edges[1:, :].T, **kwargs)
 
-    def get_field_image(self, vertex_values, shape=(150, 150), pad_fraction=0.01):
+    def plot_field(
+        self,
+        ax,
+        vertex_values: ndarray,
+        color_levels=64,
+        colormap="viridis",
+        mesh_color=None,
+        mesh_thickness=0.5,
+    ):
+        """
+        Generates a filled color contour plot of a given field specified by its value
+        at each mesh vertex.
+
+        :param ax: \
+            A ``matplotlib.pyplot`` axis object on which the field will be plotted by
+            calling the ``tricontourf`` method of the object.
+
+        :param vertex_values: \
+            The value of the field being plotted at each vertex of the mesh as a 1D numpy array.
+
+        :param color_levels: \
+            The number of color levels used to plot the field contours.
+
+        :param colormap: \
+            The name (or an instance) of a ``matplotlib`` colormap which will be used
+            to color the field contours.
+
+        :param mesh_color: \
+            The name of a ``matplotlib.pyplot`` color which will be used to draw
+            the mesh over the field. If unspecified, the mesh will not be drawn.
+
+        :param mesh_thickness: \
+            The line-width used to draw the mesh.
+        """
+        ax.tricontourf(
+            self.R,
+            self.z,
+            self.triangle_vertices,
+            vertex_values,
+            color_levels,
+            cmap=colormap,
+        )
+        if mesh_color is not None:
+            self.draw(ax, color=mesh_color, lw=mesh_thickness)
+
+    def get_field_image(
+        self, vertex_values: ndarray, shape=(150, 150), pad_fraction=0.01
+    ):
         """
         Given the value of a field at each mesh vertex, use interpolation to generate
         an image of the field across the whole mesh.
 
         :param vertex_values: \
             The value of the field being plotted at each vertex of the mesh as a 1D numpy array.
```

### Comparing `tokamesh-0.4.2/tokamesh/operators.py` & `tokamesh-0.5.0/tokamesh/operators.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 from numpy import arange, array, concatenate, full, ones, tile, ndarray, zeros
 from numpy import sqrt, diff
-from scipy.sparse import csc_matrix, csr_matrix
+from scipy.sparse import csr_array
 from scipy.special import factorial
 from scipy.linalg import solve
 from itertools import product
 from tokamesh.utilities import build_edge_map
 
 
 def edge_difference_matrix(
-    R: ndarray, z: ndarray, triangles: ndarray, normalised=False, sparse_format="csr"
+    R: ndarray,
+    z: ndarray,
+    triangles: ndarray,
+    normalised=False,
+    sparse_array_type=csr_array,
 ):
     """
     Generates a sparse matrix which, when operating on a vector of field
     values at each vertex, produces a vector of the differences in those
     field values along each edge in the mesh.
 
     :param R: \
@@ -26,18 +30,20 @@
         each of the triangles in the mesh. The array must have shape ``(N,3)`` where ``N``
         is the total number of triangles.
 
     :param bool normalised: \
         If set as ``True``, the difference in the value across each edge is normalised by
         the length of the edge, yielding an estimate of the gradient along that edge.
 
-    :param str sparse_format: \
-        Specifies the sparse-matrix format to be used for the output. Pass ``'csr'`` for
-        the ``scipy.sparse.csr_matrix`` format, and ``'csc'`` for the ``scipy.sparse.csc_matrix``
-        format.
+    :param sparse_array_type: \
+        A sparse array type from ``scipy.sparse`` which will be used as the returned
+        type of the matrix operator.
+
+    :return: \
+        The edge-difference matrix operator as a sparse array.
     """
     triangle_edges, edge_vertices, edge_map = build_edge_map(triangles)
     n_edges = edge_vertices.shape[0]
     shape = (n_edges, R.size)
     entry_vals = ones(2 * n_edges)
 
     if normalised:
@@ -47,34 +53,31 @@
         entry_vals[0::2] = inv_distances
         entry_vals[1::2] = -inv_distances
     else:
         entry_vals[1::2] = -1.0
 
     row_inds = tile(arange(n_edges), (1, 2)).T.flatten()
     col_inds = edge_vertices.T.flatten()
-    sparse_format = sparse_format if sparse_format in ["csr", "csc"] else "csr"
-    if sparse_format == "csr":
-        return csr_matrix((entry_vals, (row_inds, col_inds)), shape=shape)
-    elif sparse_format == "csc":
-        return csc_matrix((entry_vals, (row_inds, col_inds)), shape=shape)
+
+    return sparse_array_type((entry_vals, (row_inds, col_inds)), shape=shape)
 
 
 def umbrella_matrix(
     R: ndarray,
     z: ndarray,
     triangles: ndarray,
     ignore_boundary=True,
     inverse_distance_weighting=True,
     normalised=False,
-    sparse_format="csr",
+    sparse_array_type=csr_array,
 ):
     """
-    returns a sparse 'umbrella' matrix operator, which finds the difference between
-    the value of every internal vertex value and the average value of the other
-    vertices with which it is connected.
+    Returns a sparse 'umbrella' matrix operator, which finds the difference between
+    the value of every internal vertex and the average value of the other
+    vertices to which it is connected.
 
     :param R: \
         The major radius of each mesh vertex as a 1D numpy array.
 
     :param z: \
         The z-height of each mesh vertex as a 1D numpy array.
 
@@ -93,18 +96,20 @@
         irregular meshes with significant variation of edge-lengths.
 
     :param bool normalised: \
         If set as ``True`` the value produced by the operator for each vertex is normalised
         by the square of the mean distance between the neighbouring vertices and the central
         vertex.
 
-    :param str sparse_format: \
-        Specifies the sparse-matrix format to be used for the output. Pass ``'csr'`` for
-        the ``scipy.sparse.csr_matrix`` format, and ``'csc'`` for the ``scipy.sparse.csc_matrix``
-        format.
+    :param sparse_array_type: \
+        A sparse array type from ``scipy.sparse`` which will be used as the returned
+        type of the matrix operator.
+
+    :return: \
+        The umbrella matrix operator as a sparse array.
     """
     triangle_edges, edge_vertices, edge_map = build_edge_map(triangles)
 
     if ignore_boundary:
         boundary_edges = [i for i in range(len(edge_map)) if len(edge_map[i]) == 1]
         boundary_vertex_set = {edge_vertices[i, 0] for i in boundary_edges} | {
             edge_vertices[i, 1] for i in boundary_edges
@@ -139,22 +144,23 @@
         entry_vals_list.append(weights)
 
     row_indices = concatenate(row_inds_list)
     col_indices = concatenate(col_inds_list)
     entry_values = concatenate(entry_vals_list)
 
     shape = (R.size, R.size)
-    if sparse_format == "csr":
-        return csr_matrix((entry_values, (row_indices, col_indices)), shape=shape)
-    elif sparse_format == "csc":
-        return csc_matrix((entry_values, (row_indices, col_indices)), shape=shape)
+    return sparse_array_type((entry_values, (row_indices, col_indices)), shape=shape)
 
 
 def parallel_derivative(
-    R: ndarray, z: ndarray, index_grid: ndarray, order=2, sparse_format="csr"
+    R: ndarray,
+    z: ndarray,
+    index_grid: ndarray,
+    order=2,
+    sparse_array_type=csr_array,
 ):
     """
     Constructs a sparse matrix operator which estimates the derivative (with respect
     to poloidal distance) of a given set of field values at each vertex in direction
     parallel to the magnetic field.
 
     :param R: \
@@ -166,18 +172,20 @@
     :param index_grid: \
         A 2D numpy array specifying the indices of triangular mesh vertices
         corresponding to each cell of the rectangular field-aligned grid.
 
     :param order: \
         The order of the derivative to be estimated. Must be either 1 or 2.
 
-    :param str sparse_format: \
-        Specifies the sparse-matrix format to be used for the output. Pass ``'csr'`` for
-        the ``scipy.sparse.csr_matrix`` format, and ``'csc'`` for the ``scipy.sparse.csc_matrix``
-        format.
+    :param sparse_array_type: \
+        A sparse array type from ``scipy.sparse`` which will be used as the returned
+        type of the matrix operator.
+
+    :return: \
+        The parallel derivative matrix operator as a sparse array.
     """
     shape = (3, index_grid.shape[0] * index_grid.shape[1])
     values = zeros(shape)
     i_indices = zeros(shape)
     j_indices = zeros(shape)
 
     prod = product(range(index_grid.shape[0]), range(index_grid.shape[1]))
@@ -199,22 +207,24 @@
 
         values[:, k] = coeffs
         i_indices[:, k] = index_grid[i, j]
         j_indices[:, k] = inds
 
     shape = (R.size, R.size)
     indices = (i_indices.flatten(), j_indices.flatten())
-    if sparse_format == "csr":
-        return csr_matrix((values.flatten(), indices), shape=shape)
-    elif sparse_format == "csc":
-        return csc_matrix((values.flatten(), indices), shape=shape)
+
+    return sparse_array_type((values.flatten(), indices), shape=shape)
 
 
 def perpendicular_derivative(
-    R: ndarray, z: ndarray, index_grid: ndarray, order=2, sparse_format="csr"
+    R: ndarray,
+    z: ndarray,
+    index_grid: ndarray,
+    order=2,
+    sparse_array_type=csr_array,
 ):
     """
     Constructs a sparse matrix operator which estimates the derivative (with respect
     to poloidal distance) of a given set of field values at each vertex in direction
     perpendicular to the magnetic field.
 
     :param R: \
@@ -226,18 +236,20 @@
     :param index_grid: \
         A 2D numpy array specifying the indices of triangular mesh vertices
         corresponding to each cell of the rectangular field-aligned grid.
 
     :param order: \
         The order of the derivative to be estimated. Must be either 1 or 2.
 
-    :param str sparse_format: \
-        Specifies the sparse-matrix format to be used for the output. Pass ``'csr'`` for
-        the ``scipy.sparse.csr_matrix`` format, and ``'csc'`` for the ``scipy.sparse.csc_matrix``
-        format.
+    :param sparse_array_type: \
+        A sparse array type from ``scipy.sparse`` which will be used as the returned
+        type of the matrix operator.
+
+    :return: \
+        The perpendicular derivative matrix operator as a sparse array.
     """
     shape = (3, index_grid.shape[0] * index_grid.shape[1])
     values = zeros(shape)
     i_indices = zeros(shape)
     j_indices = zeros(shape)
 
     prod = product(range(index_grid.shape[0]), range(index_grid.shape[1]))
@@ -259,18 +271,15 @@
 
         values[:, k] = coeffs
         i_indices[:, k] = index_grid[i, j]
         j_indices[:, k] = inds
 
     shape = (R.size, R.size)
     indices = (i_indices.flatten(), j_indices.flatten())
-    if sparse_format == "csr":
-        return csr_matrix((values.flatten(), indices), shape=shape)
-    elif sparse_format == "csc":
-        return csc_matrix((values.flatten(), indices), shape=shape)
+    return sparse_array_type((values.flatten(), indices), shape=shape)
 
 
 def get_fd_coeffs(points, order=1):
     # check validity of inputs
     if type(points) is not ndarray:
         points = array(points)
     n = len(points)
```

### Comparing `tokamesh-0.4.2/tokamesh/tokamaks/__init__.py` & `tokamesh-0.5.0/tokamesh/tokamaks/__init__.py`

 * *Files identical despite different names*

### Comparing `tokamesh-0.4.2/tokamesh/tokamaks/mastu_boundary_data.npz` & `tokamesh-0.5.0/tokamesh/tokamaks/mastu_boundary_data.npz`

 * *Files identical despite different names*

### Comparing `tokamesh-0.4.2/tokamesh.egg-info/PKG-INFO` & `tokamesh-0.5.0/tokamesh.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tokamesh
-Version: 0.4.2
+Version: 0.5.0
 Summary: Python tools for constructing meshes and geometry matrices used in tomography problems
 Author-email: Chris Bowman <chris.bowman.physics@gmail.com>
 License: MIT License
         
         Copyright (c) 2021 Chris Bowman
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `tokamesh-0.4.2/tokamesh.egg-info/SOURCES.txt` & `tokamesh-0.5.0/tokamesh.egg-info/SOURCES.txt`

 * *Files identical despite different names*

