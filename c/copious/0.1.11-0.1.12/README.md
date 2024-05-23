# Comparing `tmp/copious-0.1.11.tar.gz` & `tmp/copious-0.1.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "copious-0.1.11.tar", last modified: Tue May  7 10:01:36 2024, max compression
+gzip compressed data, was "copious-0.1.12.tar", last modified: Thu May 23 11:04:29 2024, max compression
```

## Comparing `copious-0.1.11.tar` & `copious-0.1.12.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-05-07 10:01:36.533587 copious-0.1.11/
--rw-r--r--   0 rlan       (501) staff       (20)      386 2024-05-07 10:01:36.533453 copious-0.1.11/PKG-INFO
--rw-r--r--   0 rlan       (501) staff       (20)      124 2024-05-07 10:00:56.000000 copious-0.1.11/README.md
-drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-05-07 10:01:36.530353 copious-0.1.11/copious/
--rw-r--r--   0 rlan       (501) staff       (20)        0 2024-05-07 09:54:59.000000 copious-0.1.11/copious/__init__.py
-drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-05-07 10:01:36.531362 copious-0.1.11/copious/cv/
--rw-r--r--   0 rlan       (501) staff       (20)        0 2024-05-07 09:54:59.000000 copious-0.1.11/copious/cv/__init__.py
--rw-r--r--   0 rlan       (501) staff       (20)     3433 2024-05-07 09:54:59.000000 copious-0.1.11/copious/cv/geometry.py
--rw-r--r--   0 rlan       (501) staff       (20)     2900 2024-05-07 09:54:59.000000 copious-0.1.11/copious/cv/graphics.py
-drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-05-07 10:01:36.531636 copious-0.1.11/copious/data_structure/
--rw-r--r--   0 rlan       (501) staff       (20)        0 2024-05-07 09:54:59.000000 copious-0.1.11/copious/data_structure/__init__.py
--rw-r--r--   0 rlan       (501) staff       (20)      646 2024-05-07 09:54:59.000000 copious-0.1.11/copious/data_structure/set.py
-drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-05-07 10:01:36.532699 copious-0.1.11/copious/io/
--rw-r--r--   0 rlan       (501) staff       (20)        0 2024-05-07 09:54:59.000000 copious-0.1.11/copious/io/__init__.py
--rw-r--r--   0 rlan       (501) staff       (20)      671 2024-05-07 09:54:59.000000 copious-0.1.11/copious/io/args.py
--rw-r--r--   0 rlan       (501) staff       (20)     1763 2024-05-07 09:54:59.000000 copious-0.1.11/copious/io/fs.py
--rw-r--r--   0 rlan       (501) staff       (20)     2686 2024-05-07 09:54:59.000000 copious-0.1.11/copious/io/indices.py
--rw-r--r--   0 rlan       (501) staff       (20)      682 2024-05-07 09:54:59.000000 copious-0.1.11/copious/io/network.py
--rw-r--r--   0 rlan       (501) staff       (20)     1441 2024-05-07 09:54:59.000000 copious-0.1.11/copious/io/parallelism.py
-drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-05-07 10:01:36.533195 copious-0.1.11/copious/plot/
--rw-r--r--   0 rlan       (501) staff       (20)      118 2024-05-07 09:54:59.000000 copious-0.1.11/copious/plot/__init__.py
--rw-r--r--   0 rlan       (501) staff       (20)     1256 2024-05-07 09:54:59.000000 copious-0.1.11/copious/plot/color.py
-drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-05-07 10:01:36.530899 copious-0.1.11/copious.egg-info/
--rw-r--r--   0 rlan       (501) staff       (20)      386 2024-05-07 10:01:36.000000 copious-0.1.11/copious.egg-info/PKG-INFO
--rw-r--r--   0 rlan       (501) staff       (20)      502 2024-05-07 10:01:36.000000 copious-0.1.11/copious.egg-info/SOURCES.txt
--rw-r--r--   0 rlan       (501) staff       (20)        1 2024-05-07 10:01:36.000000 copious-0.1.11/copious.egg-info/dependency_links.txt
--rw-r--r--   0 rlan       (501) staff       (20)       42 2024-05-07 10:01:36.000000 copious-0.1.11/copious.egg-info/requires.txt
--rw-r--r--   0 rlan       (501) staff       (20)        8 2024-05-07 10:01:36.000000 copious-0.1.11/copious.egg-info/top_level.txt
--rw-r--r--   0 rlan       (501) staff       (20)       38 2024-05-07 10:01:36.533642 copious-0.1.11/setup.cfg
--rw-r--r--   0 rlan       (501) staff       (20)      553 2024-05-07 09:57:25.000000 copious-0.1.11/setup.py
+drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-05-23 11:04:29.340757 copious-0.1.12/
+-rw-r--r--   0 rlan       (501) staff       (20)      386 2024-05-23 11:04:29.340612 copious-0.1.12/PKG-INFO
+-rw-r--r--   0 rlan       (501) staff       (20)      124 2024-05-07 10:00:56.000000 copious-0.1.12/README.md
+drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-05-23 11:04:29.337159 copious-0.1.12/copious/
+-rw-r--r--   0 rlan       (501) staff       (20)        0 2024-05-07 09:54:59.000000 copious-0.1.12/copious/__init__.py
+drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-05-23 11:04:29.338414 copious-0.1.12/copious/cv/
+-rw-r--r--   0 rlan       (501) staff       (20)        0 2024-05-07 09:54:59.000000 copious-0.1.12/copious/cv/__init__.py
+-rw-r--r--   0 rlan       (501) staff       (20)     4271 2024-05-23 11:02:14.000000 copious-0.1.12/copious/cv/geometry.py
+-rw-r--r--   0 rlan       (501) staff       (20)     2900 2024-05-07 09:54:59.000000 copious-0.1.12/copious/cv/graphics.py
+drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-05-23 11:04:29.338851 copious-0.1.12/copious/data_structure/
+-rw-r--r--   0 rlan       (501) staff       (20)        0 2024-05-07 09:54:59.000000 copious-0.1.12/copious/data_structure/__init__.py
+-rw-r--r--   0 rlan       (501) staff       (20)      646 2024-05-07 09:54:59.000000 copious-0.1.12/copious/data_structure/set.py
+drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-05-23 11:04:29.340049 copious-0.1.12/copious/io/
+-rw-r--r--   0 rlan       (501) staff       (20)        0 2024-05-07 09:54:59.000000 copious-0.1.12/copious/io/__init__.py
+-rw-r--r--   0 rlan       (501) staff       (20)      671 2024-05-07 09:54:59.000000 copious-0.1.12/copious/io/args.py
+-rw-r--r--   0 rlan       (501) staff       (20)     1763 2024-05-07 09:54:59.000000 copious-0.1.12/copious/io/fs.py
+-rw-r--r--   0 rlan       (501) staff       (20)     2686 2024-05-07 09:54:59.000000 copious-0.1.12/copious/io/indices.py
+-rw-r--r--   0 rlan       (501) staff       (20)      682 2024-05-07 09:54:59.000000 copious-0.1.12/copious/io/network.py
+-rw-r--r--   0 rlan       (501) staff       (20)     1441 2024-05-07 09:54:59.000000 copious-0.1.12/copious/io/parallelism.py
+drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-05-23 11:04:29.340390 copious-0.1.12/copious/plot/
+-rw-r--r--   0 rlan       (501) staff       (20)      118 2024-05-07 09:54:59.000000 copious-0.1.12/copious/plot/__init__.py
+-rw-r--r--   0 rlan       (501) staff       (20)     1256 2024-05-07 09:54:59.000000 copious-0.1.12/copious/plot/color.py
+drwxr-xr-x   0 rlan       (501) staff       (20)        0 2024-05-23 11:04:29.337898 copious-0.1.12/copious.egg-info/
+-rw-r--r--   0 rlan       (501) staff       (20)      386 2024-05-23 11:04:29.000000 copious-0.1.12/copious.egg-info/PKG-INFO
+-rw-r--r--   0 rlan       (501) staff       (20)      502 2024-05-23 11:04:29.000000 copious-0.1.12/copious.egg-info/SOURCES.txt
+-rw-r--r--   0 rlan       (501) staff       (20)        1 2024-05-23 11:04:29.000000 copious-0.1.12/copious.egg-info/dependency_links.txt
+-rw-r--r--   0 rlan       (501) staff       (20)       42 2024-05-23 11:04:29.000000 copious-0.1.12/copious.egg-info/requires.txt
+-rw-r--r--   0 rlan       (501) staff       (20)        8 2024-05-23 11:04:29.000000 copious-0.1.12/copious.egg-info/top_level.txt
+-rw-r--r--   0 rlan       (501) staff       (20)       38 2024-05-23 11:04:29.340826 copious-0.1.12/setup.cfg
+-rw-r--r--   0 rlan       (501) staff       (20)      553 2024-05-23 11:04:00.000000 copious-0.1.12/setup.py
```

### Comparing `copious-0.1.11/copious/cv/geometry.py` & `copious-0.1.12/copious/cv/geometry.py`

 * *Files 15% similar despite different names*

```diff
@@ -38,14 +38,40 @@
     T[:3, 3] = [x, y, z]
     T[:3, :3] = rot
     if as_homo:
         return T
     return T[:3, :]
 
 
+def euler2mat(x: float, y: float, z: float, as_homo: bool = False, axis_order: str = "XYZ", degrees: bool = True) -> np.ndarray:
+    """A helper function that convert euler angles (3 values) representation to transformation matrix representation.
+
+    Parameters
+    ----------
+    x : float
+        x coordinate of the translation
+    y : float
+        y coordinate of the translation
+    z : float
+        z coordinate of the translation
+    as_homo: bool
+        if true, the matrix will be saved as homogeneous (4x4), otherwise, it will be saved as 3x4
+
+    Returns
+    -------
+    np.ndarray
+        of shape (3, 4) if as_homo == False, otherwise, (4, 4)
+    """
+    rot = np.eye(4)
+    rot[:3, :3] = Rotation.from_euler(axis_order, [x, y, z], degrees=degrees).as_matrix()
+    if as_homo:
+        return rot
+    return rot[:3, :3]
+
+
 def points3d_to_homo(points3d: np.ndarray) -> np.ndarray:
     return np.concatenate((points3d, np.ones(len(points3d))[:, None]), axis=1)
 
 
 def homo_to_points3d(points_homo: np.ndarray) -> np.ndarray:
     return points_homo[:, :3]
```

### Comparing `copious-0.1.11/copious/cv/graphics.py` & `copious-0.1.12/copious/cv/graphics.py`

 * *Files identical despite different names*

### Comparing `copious-0.1.11/copious/data_structure/set.py` & `copious-0.1.12/copious/data_structure/set.py`

 * *Files identical despite different names*

### Comparing `copious-0.1.11/copious/io/args.py` & `copious-0.1.12/copious/io/args.py`

 * *Files identical despite different names*

### Comparing `copious-0.1.11/copious/io/fs.py` & `copious-0.1.12/copious/io/fs.py`

 * *Files identical despite different names*

### Comparing `copious-0.1.11/copious/io/indices.py` & `copious-0.1.12/copious/io/indices.py`

 * *Files identical despite different names*

### Comparing `copious-0.1.11/copious/io/network.py` & `copious-0.1.12/copious/io/network.py`

 * *Files identical despite different names*

### Comparing `copious-0.1.11/copious/io/parallelism.py` & `copious-0.1.12/copious/io/parallelism.py`

 * *Files identical despite different names*

### Comparing `copious-0.1.11/copious/plot/color.py` & `copious-0.1.12/copious/plot/color.py`

 * *Files identical despite different names*

### Comparing `copious-0.1.11/setup.py` & `copious-0.1.12/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='copious',
-    version='0.1.11',
+    version='0.1.12',
     packages=find_packages(),
     description='A handy tool that make your day to day programming much easier. ',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='brianlan',
     author_email='brianlanbo@gmail.com',
     url='https://gitlab.com/rlan/copious',
```

