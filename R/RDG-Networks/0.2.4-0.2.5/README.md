# Comparing `tmp/RDG-Networks-0.2.4.tar.gz` & `tmp/RDG-Networks-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RDG-Networks-0.2.4.tar", last modified: Mon May 13 19:35:11 2024, max compression
+gzip compressed data, was "RDG-Networks-0.2.5.tar", last modified: Thu May 23 12:49:39 2024, max compression
```

## Comparing `RDG-Networks-0.2.4.tar` & `RDG-Networks-0.2.5.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 5746604    (501) staff       (20)        0 2024-05-13 19:35:11.938723 RDG-Networks-0.2.4/
--rw-r--r--   0 5746604    (501) staff       (20)      598 2024-05-07 14:05:23.000000 RDG-Networks-0.2.4/LICENSE.txt
--rw-r--r--   0 5746604    (501) staff       (20)     2422 2024-05-13 19:35:11.938527 RDG-Networks-0.2.4/PKG-INFO
-drwxr-xr-x   0 5746604    (501) staff       (20)        0 2024-05-13 19:35:11.937037 RDG-Networks-0.2.4/RDG_Networks.egg-info/
--rw-r--r--   0 5746604    (501) staff       (20)     2422 2024-05-13 19:35:11.000000 RDG-Networks-0.2.4/RDG_Networks.egg-info/PKG-INFO
--rw-r--r--   0 5746604    (501) staff       (20)      527 2024-05-13 19:35:11.000000 RDG-Networks-0.2.4/RDG_Networks.egg-info/SOURCES.txt
--rw-r--r--   0 5746604    (501) staff       (20)        1 2024-05-13 19:35:11.000000 RDG-Networks-0.2.4/RDG_Networks.egg-info/dependency_links.txt
--rw-r--r--   0 5746604    (501) staff       (20)      350 2024-05-13 19:35:11.000000 RDG-Networks-0.2.4/RDG_Networks.egg-info/entry_points.txt
--rw-r--r--   0 5746604    (501) staff       (20)       36 2024-05-13 19:35:11.000000 RDG-Networks-0.2.4/RDG_Networks.egg-info/requires.txt
--rw-r--r--   0 5746604    (501) staff       (20)       13 2024-05-13 19:35:11.000000 RDG-Networks-0.2.4/RDG_Networks.egg-info/top_level.txt
-drwxr-xr-x   0 5746604    (501) staff       (20)        0 2024-05-13 19:35:11.938292 RDG-Networks-0.2.4/RDG_networks/
--rw-r--r--   0 5746604    (501) staff       (20)     7977 2024-03-04 14:31:37.000000 RDG-Networks-0.2.4/RDG_networks/Classes.py
--rw-r--r--   0 5746604    (501) staff       (20)      661 2024-05-06 18:35:06.000000 RDG-Networks-0.2.4/RDG_networks/__init__.py
--rw-r--r--   0 5746604    (501) staff       (20)      984 2024-03-04 14:31:54.000000 RDG-Networks-0.2.4/RDG_networks/draw_segments.py
--rw-r--r--   0 5746604    (501) staff       (20)     1127 2024-03-04 14:31:51.000000 RDG-Networks-0.2.4/RDG_networks/generate_line_network.py
--rw-r--r--   0 5746604    (501) staff       (20)     9004 2024-05-06 18:31:39.000000 RDG-Networks-0.2.4/RDG_networks/generate_line_segments.py
--rw-r--r--   0 5746604    (501) staff       (20)     7531 2024-05-13 19:33:11.000000 RDG-Networks-0.2.4/RDG_networks/generate_line_segments_dynamic.py
--rw-r--r--   0 5746604    (501) staff       (20)     2797 2024-03-04 14:52:33.000000 RDG-Networks-0.2.4/RDG_networks/get_intersection_segments.py
--rw-r--r--   0 5746604    (501) staff       (20)     1605 2024-03-01 14:53:20.000000 RDG-Networks-0.2.4/RDG_networks/sample_in_polygon.py
--rw-r--r--   0 5746604    (501) staff       (20)     1940 2024-05-07 14:03:34.000000 RDG-Networks-0.2.4/README.md
--rw-r--r--   0 5746604    (501) staff       (20)       38 2024-05-13 19:35:11.938772 RDG-Networks-0.2.4/setup.cfg
--rw-r--r--   0 5746604    (501) staff       (20)     1162 2024-05-13 19:35:05.000000 RDG-Networks-0.2.4/setup.py
+drwxr-xr-x   0 5746604    (501) staff       (20)        0 2024-05-23 12:49:39.609876 RDG-Networks-0.2.5/
+-rw-r--r--   0 5746604    (501) staff       (20)      598 2024-05-07 14:05:23.000000 RDG-Networks-0.2.5/LICENSE.txt
+-rw-r--r--   0 5746604    (501) staff       (20)     2422 2024-05-23 12:49:39.609634 RDG-Networks-0.2.5/PKG-INFO
+drwxr-xr-x   0 5746604    (501) staff       (20)        0 2024-05-23 12:49:39.606293 RDG-Networks-0.2.5/RDG_Networks.egg-info/
+-rw-r--r--   0 5746604    (501) staff       (20)     2422 2024-05-23 12:49:39.000000 RDG-Networks-0.2.5/RDG_Networks.egg-info/PKG-INFO
+-rw-r--r--   0 5746604    (501) staff       (20)      573 2024-05-23 12:49:39.000000 RDG-Networks-0.2.5/RDG_Networks.egg-info/SOURCES.txt
+-rw-r--r--   0 5746604    (501) staff       (20)        1 2024-05-23 12:49:39.000000 RDG-Networks-0.2.5/RDG_Networks.egg-info/dependency_links.txt
+-rw-r--r--   0 5746604    (501) staff       (20)      350 2024-05-23 12:49:39.000000 RDG-Networks-0.2.5/RDG_Networks.egg-info/entry_points.txt
+-rw-r--r--   0 5746604    (501) staff       (20)       36 2024-05-23 12:49:39.000000 RDG-Networks-0.2.5/RDG_Networks.egg-info/requires.txt
+-rw-r--r--   0 5746604    (501) staff       (20)       13 2024-05-23 12:49:39.000000 RDG-Networks-0.2.5/RDG_Networks.egg-info/top_level.txt
+drwxr-xr-x   0 5746604    (501) staff       (20)        0 2024-05-23 12:49:39.609183 RDG-Networks-0.2.5/RDG_networks/
+-rw-r--r--   0 5746604    (501) staff       (20)     7977 2024-03-04 14:31:37.000000 RDG-Networks-0.2.5/RDG_networks/Classes.py
+-rw-r--r--   0 5746604    (501) staff       (20)      661 2024-05-06 18:35:06.000000 RDG-Networks-0.2.5/RDG_networks/__init__.py
+-rw-r--r--   0 5746604    (501) staff       (20)      984 2024-03-04 14:31:54.000000 RDG-Networks-0.2.5/RDG_networks/draw_segments.py
+-rw-r--r--   0 5746604    (501) staff       (20)     1127 2024-03-04 14:31:51.000000 RDG-Networks-0.2.5/RDG_networks/generate_line_network.py
+-rw-r--r--   0 5746604    (501) staff       (20)     9004 2024-05-06 18:31:39.000000 RDG-Networks-0.2.5/RDG_networks/generate_line_segments.py
+-rw-r--r--   0 5746604    (501) staff       (20)     7531 2024-05-13 19:33:11.000000 RDG-Networks-0.2.5/RDG_networks/generate_line_segments_dynamic.py
+-rw-r--r--   0 5746604    (501) staff       (20)     9265 2024-05-23 12:47:45.000000 RDG-Networks-0.2.5/RDG_networks/generate_line_segments_static.py
+-rw-r--r--   0 5746604    (501) staff       (20)     2797 2024-03-04 14:52:33.000000 RDG-Networks-0.2.5/RDG_networks/get_intersection_segments.py
+-rw-r--r--   0 5746604    (501) staff       (20)     1605 2024-03-01 14:53:20.000000 RDG-Networks-0.2.5/RDG_networks/sample_in_polygon.py
+-rw-r--r--   0 5746604    (501) staff       (20)     1940 2024-05-07 14:03:34.000000 RDG-Networks-0.2.5/README.md
+-rw-r--r--   0 5746604    (501) staff       (20)       38 2024-05-23 12:49:39.609940 RDG-Networks-0.2.5/setup.cfg
+-rw-r--r--   0 5746604    (501) staff       (20)     1162 2024-05-23 12:48:13.000000 RDG-Networks-0.2.5/setup.py
```

### Comparing `RDG-Networks-0.2.4/LICENSE.txt` & `RDG-Networks-0.2.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `RDG-Networks-0.2.4/PKG-INFO` & `RDG-Networks-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RDG-Networks
-Version: 0.2.4
+Version: 0.2.5
 Summary: Most of the code from the RDG Networks project
 Home-page: https://github.com/NiekMooij/RDG_networks
 Author: Niek Mooij
 Author-email: mooij.niek@gmail.com
 License: All Rights Reserved
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `RDG-Networks-0.2.4/RDG_Networks.egg-info/PKG-INFO` & `RDG-Networks-0.2.5/RDG_Networks.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RDG-Networks
-Version: 0.2.4
+Version: 0.2.5
 Summary: Most of the code from the RDG Networks project
 Home-page: https://github.com/NiekMooij/RDG_networks
 Author: Niek Mooij
 Author-email: mooij.niek@gmail.com
 License: All Rights Reserved
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `RDG-Networks-0.2.4/RDG_Networks.egg-info/SOURCES.txt` & `RDG-Networks-0.2.5/RDG_Networks.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -9,9 +9,10 @@
 RDG_Networks.egg-info/top_level.txt
 RDG_networks/Classes.py
 RDG_networks/__init__.py
 RDG_networks/draw_segments.py
 RDG_networks/generate_line_network.py
 RDG_networks/generate_line_segments.py
 RDG_networks/generate_line_segments_dynamic.py
+RDG_networks/generate_line_segments_static.py
 RDG_networks/get_intersection_segments.py
 RDG_networks/sample_in_polygon.py
```

### Comparing `RDG-Networks-0.2.4/RDG_networks/Classes.py` & `RDG-Networks-0.2.5/RDG_networks/Classes.py`

 * *Files identical despite different names*

### Comparing `RDG-Networks-0.2.4/RDG_networks/__init__.py` & `RDG-Networks-0.2.5/RDG_networks/__init__.py`

 * *Files identical despite different names*

### Comparing `RDG-Networks-0.2.4/RDG_networks/draw_segments.py` & `RDG-Networks-0.2.5/RDG_networks/draw_segments.py`

 * *Files identical despite different names*

### Comparing `RDG-Networks-0.2.4/RDG_networks/generate_line_network.py` & `RDG-Networks-0.2.5/RDG_networks/generate_line_network.py`

 * *Files identical despite different names*

### Comparing `RDG-Networks-0.2.4/RDG_networks/generate_line_segments.py` & `RDG-Networks-0.2.5/RDG_networks/generate_line_segments.py`

 * *Files identical despite different names*

### Comparing `RDG-Networks-0.2.4/RDG_networks/generate_line_segments_dynamic.py` & `RDG-Networks-0.2.5/RDG_networks/generate_line_segments_dynamic.py`

 * *Files identical despite different names*

### Comparing `RDG-Networks-0.2.4/RDG_networks/get_intersection_segments.py` & `RDG-Networks-0.2.5/RDG_networks/get_intersection_segments.py`

 * *Files identical despite different names*

### Comparing `RDG-Networks-0.2.4/RDG_networks/sample_in_polygon.py` & `RDG-Networks-0.2.5/RDG_networks/sample_in_polygon.py`

 * *Files identical despite different names*

### Comparing `RDG-Networks-0.2.4/README.md` & `RDG-Networks-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `RDG-Networks-0.2.4/setup.py` & `RDG-Networks-0.2.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='RDG-Networks',
-    version='0.2.4',
+    version='0.2.5',
     author='Niek Mooij',
     author_email='mooij.niek@gmail.com',
     description='Most of the code from the RDG Networks project',
     long_description=open('README.md').read(),
     url='https://github.com/NiekMooij/RDG_networks',
     classifiers=[
             'Programming Language :: Python :: 3',
```

