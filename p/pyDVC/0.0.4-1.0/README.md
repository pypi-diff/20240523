# Comparing `tmp/pydvc-0.0.4.tar.gz` & `tmp/pyDVC-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydvc-0.0.4.tar", last modified: Thu May 23 08:58:34 2024, max compression
+gzip compressed data, was "pyDVC-1.0.tar", last modified: Thu May 23 08:16:54 2024, max compression
```

## Comparing `pydvc-0.0.4.tar` & `pyDVC-1.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:58:34.061864 pydvc-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-05-23 08:58:30.000000 pydvc-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2977 2024-05-23 08:58:34.061864 pydvc-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-23 08:58:30.000000 pydvc-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:58:34.061864 pydvc-0.0.4/pyDVC.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2977 2024-05-23 08:58:34.000000 pydvc-0.0.4/pyDVC.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-23 08:58:34.000000 pydvc-0.0.4/pyDVC.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 08:58:34.000000 pydvc-0.0.4/pyDVC.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-23 08:58:34.000000 pydvc-0.0.4/pyDVC.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-23 08:58:34.000000 pydvc-0.0.4/pyDVC.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     7152 2024-05-23 08:58:30.000000 pydvc-0.0.4/pyDVC.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 08:58:34.061864 pydvc-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-23 08:58:30.000000 pydvc-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:16:54.088908 pyDVC-1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-05-23 08:16:51.000000 pyDVC-1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-05-23 08:16:54.088908 pyDVC-1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-23 08:16:51.000000 pyDVC-1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:16:54.088908 pyDVC-1.0/pyDVC.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-05-23 08:16:54.000000 pyDVC-1.0/pyDVC.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-23 08:16:54.000000 pyDVC-1.0/pyDVC.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 08:16:54.000000 pyDVC-1.0/pyDVC.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-23 08:16:54.000000 pyDVC-1.0/pyDVC.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-23 08:16:54.000000 pyDVC-1.0/pyDVC.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7152 2024-05-23 08:16:51.000000 pyDVC-1.0/pyDVC.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 08:16:54.088908 pyDVC-1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-23 08:16:51.000000 pyDVC-1.0/setup.py
```

### Comparing `pydvc-0.0.4/LICENSE` & `pyDVC-1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydvc-0.0.4/pyDVC.py` & `pyDVC-1.0/pyDVC.py`

 * *Files identical despite different names*

### Comparing `pydvc-0.0.4/setup.py` & `pyDVC-1.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 import setuptools
 
-# read README for long description
-from pathlib import Path
-this_directory = Path(__file__).parent
-long_description = (this_directory / "README.md").read_text()
-
 setuptools.setup(
     name='pyDVC',
-    version='0.0.4',
+    version='1.0',
     packages=setuptools.find_packages(),
     url='https://github.com/jadball/pyDVC',
     license='BSD 3-Clause',
     author='James Ball',
     author_email='jadball@gmail.com',
     description='Python implementation of Discrete Voronoi Chain algorithm by Mirko Velić, Dave May & Louis Moresi (2009).',
-    long_description=long_description,
-    long_description_content_type='text/markdown',
+    long_description=
+    """Python implementation of Discrete Voronoi Chain algorithm.
+    First described by Velić, Mirko & May, Dave & Moresi, Louis. (2009). A Fast Robust Algorithm for Computing Discrete Voronoi Diagrams. J Math Model Algor. 8. 343-355. 10.1007/s10852-008-9097-6.
+    http://dx.doi.org/10.1007/s10852-008-9097-6""",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: BSD License",
         "Operating System :: OS Independent",
     ],
     py_modules=["pyDVC"],
     python_requires='>=3.6',
```

