# Comparing `tmp/cvtkit-0.0.3.tar.gz` & `tmp/cvtkit-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvtkit-0.0.3.tar", last modified: Mon Nov 27 21:26:30 2023, max compression
+gzip compressed data, was "cvtkit-0.0.4.tar", last modified: Wed May 22 22:05:21 2024, max compression
```

## Comparing `cvtkit-0.0.3.tar` & `cvtkit-0.0.4.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxrwxr-x   0 nate      (1000) nate      (1000)        0 2023-11-27 21:26:30.783327 cvtkit-0.0.3/
--rw-rw-r--   0 nate      (1000) nate      (1000)    35150 2022-12-21 20:38:41.000000 cvtkit-0.0.3/LICENSE.txt
--rw-rw-r--   0 nate      (1000) nate      (1000)     1566 2023-11-27 21:26:30.783327 cvtkit-0.0.3/PKG-INFO
--rw-rw-r--   0 nate      (1000) nate      (1000)      249 2023-02-10 23:26:25.000000 cvtkit-0.0.3/README.md
--rw-rw-r--   0 nate      (1000) nate      (1000)       38 2023-11-27 21:26:30.783327 cvtkit-0.0.3/setup.cfg
--rw-rw-r--   0 nate      (1000) nate      (1000)     1717 2023-11-27 21:25:58.000000 cvtkit-0.0.3/setup.py
-drwxrwxr-x   0 nate      (1000) nate      (1000)        0 2023-11-27 21:26:30.783327 cvtkit-0.0.3/src/
-drwxrwxr-x   0 nate      (1000) nate      (1000)        0 2023-11-27 21:26:30.783327 cvtkit-0.0.3/src/cvt/
--rw-rw-r--   0 nate      (1000) nate      (1000)      178 2023-03-16 19:22:49.000000 cvtkit-0.0.3/src/cvt/__init__.py
--rw-rw-r--   0 nate      (1000) nate      (1000)     5171 2023-03-21 16:59:29.000000 cvtkit-0.0.3/src/cvt/camera.py
-drwxrwxr-x   0 nate      (1000) nate      (1000)        0 2023-11-27 21:26:30.783327 cvtkit-0.0.3/src/cvt/datasets/
--rw-rw-r--   0 nate      (1000) nate      (1000)      547 2023-02-07 17:20:24.000000 cvtkit-0.0.3/src/cvt/datasets/__init__.py
--rw-rw-r--   0 nate      (1000) nate      (1000)        0 2023-01-09 18:27:55.000000 cvtkit-0.0.3/src/cvt/datasets/blended.py
--rw-rw-r--   0 nate      (1000) nate      (1000)     3366 2023-02-07 17:28:58.000000 cvtkit-0.0.3/src/cvt/datasets/dtu.py
--rw-rw-r--   0 nate      (1000) nate      (1000)        0 2023-01-09 18:27:55.000000 cvtkit-0.0.3/src/cvt/datasets/tanks.py
--rw-rw-r--   0 nate      (1000) nate      (1000)     4562 2023-03-16 22:31:21.000000 cvtkit-0.0.3/src/cvt/filtering.py
--rw-rw-r--   0 nate      (1000) nate      (1000)    25636 2023-11-27 20:41:13.000000 cvtkit-0.0.3/src/cvt/geometry.py
--rw-rw-r--   0 nate      (1000) nate      (1000)    13601 2023-11-17 00:08:45.000000 cvtkit-0.0.3/src/cvt/io.py
--rw-rw-r--   0 nate      (1000) nate      (1000)    11457 2023-03-16 18:31:36.000000 cvtkit-0.0.3/src/cvt/metrics.py
--rw-rw-r--   0 nate      (1000) nate      (1000)     6671 2023-09-13 17:12:00.000000 cvtkit-0.0.3/src/cvt/util.py
-drwxrwxr-x   0 nate      (1000) nate      (1000)        0 2023-11-27 21:26:30.783327 cvtkit-0.0.3/src/cvt/visualization/
--rw-rw-r--   0 nate      (1000) nate      (1000)      669 2023-02-07 17:20:25.000000 cvtkit-0.0.3/src/cvt/visualization/__init__.py
--rw-rw-r--   0 nate      (1000) nate      (1000)     1544 2023-01-10 23:29:11.000000 cvtkit-0.0.3/src/cvt/visualization/latex.py
--rw-rw-r--   0 nate      (1000) nate      (1000)     8490 2023-11-17 00:03:24.000000 cvtkit-0.0.3/src/cvt/visualization/util.py
--rw-rw-r--   0 nate      (1000) nate      (1000)     2512 2023-01-10 23:47:01.000000 cvtkit-0.0.3/src/cvt/visualization/video.py
-drwxrwxr-x   0 nate      (1000) nate      (1000)        0 2023-11-27 21:26:30.783327 cvtkit-0.0.3/src/cvtkit.egg-info/
--rw-rw-r--   0 nate      (1000) nate      (1000)     1566 2023-11-27 21:26:30.000000 cvtkit-0.0.3/src/cvtkit.egg-info/PKG-INFO
--rw-rw-r--   0 nate      (1000) nate      (1000)      560 2023-11-27 21:26:30.000000 cvtkit-0.0.3/src/cvtkit.egg-info/SOURCES.txt
--rw-rw-r--   0 nate      (1000) nate      (1000)        1 2023-11-27 21:26:30.000000 cvtkit-0.0.3/src/cvtkit.egg-info/dependency_links.txt
--rw-rw-r--   0 nate      (1000) nate      (1000)       19 2023-11-27 21:26:30.000000 cvtkit-0.0.3/src/cvtkit.egg-info/requires.txt
--rw-rw-r--   0 nate      (1000) nate      (1000)        4 2023-11-27 21:26:30.000000 cvtkit-0.0.3/src/cvtkit.egg-info/top_level.txt
+drwxrwxr-x   0 nate      (1000) nate      (1000)        0 2024-05-22 22:05:21.334689 cvtkit-0.0.4/
+-rw-rw-r--   0 nate      (1000) nate      (1000)    35150 2023-11-27 21:29:27.000000 cvtkit-0.0.4/LICENSE.txt
+-rw-r--r--   0 nate      (1000) nate      (1000)     1855 2024-05-22 22:05:21.334689 cvtkit-0.0.4/PKG-INFO
+-rw-rw-r--   0 nate      (1000) nate      (1000)      242 2024-04-09 21:27:05.000000 cvtkit-0.0.4/README.md
+-rw-rw-r--   0 nate      (1000) nate      (1000)     1466 2024-05-22 22:04:12.000000 cvtkit-0.0.4/pyproject.toml
+-rw-rw-r--   0 nate      (1000) nate      (1000)       38 2024-05-22 22:05:21.334689 cvtkit-0.0.4/setup.cfg
+-rw-rw-r--   0 nate      (1000) nate      (1000)     1649 2024-05-22 22:04:16.000000 cvtkit-0.0.4/setup.py
+drwxrwxr-x   0 nate      (1000) nate      (1000)        0 2024-05-22 22:05:21.330689 cvtkit-0.0.4/src/
+drwxrwxr-x   0 nate      (1000) nate      (1000)        0 2024-05-22 22:05:21.330689 cvtkit-0.0.4/src/cvt/
+-rw-rw-r--   0 nate      (1000) nate      (1000)      178 2023-11-27 21:29:27.000000 cvtkit-0.0.4/src/cvt/__init__.py
+-rw-rw-r--   0 nate      (1000) nate      (1000)     5171 2023-11-27 21:29:27.000000 cvtkit-0.0.4/src/cvt/camera.py
+drwxrwxr-x   0 nate      (1000) nate      (1000)        0 2024-05-22 22:05:21.330689 cvtkit-0.0.4/src/cvt/datasets/
+-rw-rw-r--   0 nate      (1000) nate      (1000)      547 2023-11-27 21:29:27.000000 cvtkit-0.0.4/src/cvt/datasets/__init__.py
+-rw-rw-r--   0 nate      (1000) nate      (1000)        0 2023-11-27 21:29:27.000000 cvtkit-0.0.4/src/cvt/datasets/blended.py
+-rw-rw-r--   0 nate      (1000) nate      (1000)     3366 2023-11-27 21:29:27.000000 cvtkit-0.0.4/src/cvt/datasets/dtu.py
+-rw-rw-r--   0 nate      (1000) nate      (1000)        0 2023-11-27 21:29:27.000000 cvtkit-0.0.4/src/cvt/datasets/tanks.py
+-rw-rw-r--   0 nate      (1000) nate      (1000)     4562 2023-11-27 21:29:27.000000 cvtkit-0.0.4/src/cvt/filtering.py
+-rw-rw-r--   0 nate      (1000) nate      (1000)    25636 2024-05-22 20:47:23.000000 cvtkit-0.0.4/src/cvt/geometry.py
+-rw-rw-r--   0 nate      (1000) nate      (1000)    13601 2024-05-22 20:47:30.000000 cvtkit-0.0.4/src/cvt/io.py
+-rw-rw-r--   0 nate      (1000) nate      (1000)    11457 2023-11-27 21:29:27.000000 cvtkit-0.0.4/src/cvt/metrics.py
+-rw-rw-r--   0 nate      (1000) nate      (1000)     6671 2023-11-27 21:29:27.000000 cvtkit-0.0.4/src/cvt/util.py
+drwxrwxr-x   0 nate      (1000) nate      (1000)        0 2024-05-22 22:05:21.330689 cvtkit-0.0.4/src/cvt/visualization/
+-rw-rw-r--   0 nate      (1000) nate      (1000)      669 2023-11-27 21:29:27.000000 cvtkit-0.0.4/src/cvt/visualization/__init__.py
+-rw-rw-r--   0 nate      (1000) nate      (1000)     1544 2023-11-27 21:29:27.000000 cvtkit-0.0.4/src/cvt/visualization/latex.py
+-rw-rw-r--   0 nate      (1000) nate      (1000)     8490 2024-05-22 20:47:49.000000 cvtkit-0.0.4/src/cvt/visualization/util.py
+-rw-rw-r--   0 nate      (1000) nate      (1000)     2512 2023-11-27 21:29:27.000000 cvtkit-0.0.4/src/cvt/visualization/video.py
+drwxrwxr-x   0 nate      (1000) nate      (1000)        0 2024-05-22 22:05:21.330689 cvtkit-0.0.4/src/cvtkit.egg-info/
+-rw-r--r--   0 nate      (1000) nate      (1000)     1855 2024-05-22 22:05:21.000000 cvtkit-0.0.4/src/cvtkit.egg-info/PKG-INFO
+-rw-rw-r--   0 nate      (1000) nate      (1000)      575 2024-05-22 22:05:21.000000 cvtkit-0.0.4/src/cvtkit.egg-info/SOURCES.txt
+-rw-rw-r--   0 nate      (1000) nate      (1000)        1 2024-05-22 22:05:21.000000 cvtkit-0.0.4/src/cvtkit.egg-info/dependency_links.txt
+-rw-rw-r--   0 nate      (1000) nate      (1000)       31 2024-05-22 22:05:21.000000 cvtkit-0.0.4/src/cvtkit.egg-info/requires.txt
+-rw-rw-r--   0 nate      (1000) nate      (1000)        4 2024-05-22 22:05:21.000000 cvtkit-0.0.4/src/cvtkit.egg-info/top_level.txt
```

### Comparing `cvtkit-0.0.3/LICENSE.txt` & `cvtkit-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cvtkit-0.0.3/setup.py` & `cvtkit-0.0.4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as doc:
     long_desc = doc.read()
 
 setup(
         name="cvtkit",
-        version="0.0.3",
         description="A Python library including general functions and operations on various computer vision related structures.",
         long_description=long_desc,
         long_description_content_type="text/markdown",
         url="https://github.com/nburgdorfer/vision_toolkit",
         author="Nathaniel Burgdorfer",
         author_email="nburgdorfer@gmail.com",
         packages=find_packages(where="src"),
@@ -20,15 +19,14 @@
             "Intended Audience :: Education",
             "Intended Audience :: Science/Research",
             "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
             "Natural Language :: English",
             "Operating System :: OS Independent",
             "Programming Language :: Python :: 3",
             "Programming Language :: Python :: 3.9",
-            "Programming Language :: C++",
             "Topic :: Multimedia",
             "Topic :: Multimedia :: Graphics",
             "Topic :: Multimedia :: Graphics :: 3D Modeling",
             "Topic :: Multimedia :: Graphics :: 3D Rendering",
             "Topic :: Scientific/Engineering",
             "Topic :: Scientific/Engineering :: Image Processing",
             "Topic :: Scientific/Engineering :: Visualization",
```

### Comparing `cvtkit-0.0.3/src/cvt/camera.py` & `cvtkit-0.0.4/src/cvt/camera.py`

 * *Files identical despite different names*

### Comparing `cvtkit-0.0.3/src/cvt/datasets/__init__.py` & `cvtkit-0.0.4/src/cvt/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `cvtkit-0.0.3/src/cvt/datasets/dtu.py` & `cvtkit-0.0.4/src/cvt/datasets/dtu.py`

 * *Files identical despite different names*

### Comparing `cvtkit-0.0.3/src/cvt/filtering.py` & `cvtkit-0.0.4/src/cvt/filtering.py`

 * *Files identical despite different names*

### Comparing `cvtkit-0.0.3/src/cvt/geometry.py` & `cvtkit-0.0.4/src/cvt/geometry.py`

 * *Files identical despite different names*

### Comparing `cvtkit-0.0.3/src/cvt/io.py` & `cvtkit-0.0.4/src/cvt/io.py`

 * *Files identical despite different names*

### Comparing `cvtkit-0.0.3/src/cvt/metrics.py` & `cvtkit-0.0.4/src/cvt/metrics.py`

 * *Files identical despite different names*

### Comparing `cvtkit-0.0.3/src/cvt/util.py` & `cvtkit-0.0.4/src/cvt/util.py`

 * *Files identical despite different names*

### Comparing `cvtkit-0.0.3/src/cvt/visualization/__init__.py` & `cvtkit-0.0.4/src/cvt/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `cvtkit-0.0.3/src/cvt/visualization/latex.py` & `cvtkit-0.0.4/src/cvt/visualization/latex.py`

 * *Files identical despite different names*

### Comparing `cvtkit-0.0.3/src/cvt/visualization/util.py` & `cvtkit-0.0.4/src/cvt/visualization/util.py`

 * *Files identical despite different names*

### Comparing `cvtkit-0.0.3/src/cvt/visualization/video.py` & `cvtkit-0.0.4/src/cvt/visualization/video.py`

 * *Files identical despite different names*

### Comparing `cvtkit-0.0.3/src/cvtkit.egg-info/SOURCES.txt` & `cvtkit-0.0.4/src/cvtkit.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 LICENSE.txt
 README.md
+pyproject.toml
 setup.py
 src/cvt/__init__.py
 src/cvt/camera.py
 src/cvt/filtering.py
 src/cvt/geometry.py
 src/cvt/io.py
 src/cvt/metrics.py
```

