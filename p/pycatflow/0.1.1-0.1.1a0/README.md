# Comparing `tmp/pycatflow-0.1.1.tar.gz` & `tmp/pycatflow-0.1.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycatflow-0.1.1.tar", last modified: Thu May 23 19:59:03 2024, max compression
+gzip compressed data, was "pycatflow-0.1.1a0.tar", last modified: Thu May 23 20:03:33 2024, max compression
```

## Comparing `pycatflow-0.1.1.tar` & `pycatflow-0.1.1a0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 bumatic    (501) staff       (20)        0 2024-05-23 19:59:03.403694 pycatflow-0.1.1/
--rw-rw-r--   0 bumatic    (501) staff       (20)     1077 2021-10-03 11:41:14.000000 pycatflow-0.1.1/LICENSE
--rw-r--r--   0 bumatic    (501) staff       (20)     3302 2024-05-23 19:59:03.399579 pycatflow-0.1.1/PKG-INFO
--rw-rw-r--   0 bumatic    (501) staff       (20)     2844 2021-10-03 11:41:14.000000 pycatflow-0.1.1/README.md
-drwxr-xr-x   0 bumatic    (501) staff       (20)        0 2024-05-23 19:59:03.341055 pycatflow-0.1.1/pycatflow/
--rw-rw-r--   0 bumatic    (501) staff       (20)       40 2021-10-03 11:41:14.000000 pycatflow-0.1.1/pycatflow/__init__.py
--rw-rw-r--   0 bumatic    (501) staff       (20)     9068 2021-10-03 11:41:14.000000 pycatflow-0.1.1/pycatflow/input.py
--rw-rw-r--   0 bumatic    (501) staff       (20)    27937 2021-10-03 11:41:14.000000 pycatflow-0.1.1/pycatflow/viz.py
-drwxr-xr-x   0 bumatic    (501) staff       (20)        0 2024-05-23 19:59:03.395072 pycatflow-0.1.1/pycatflow.egg-info/
--rw-r--r--   0 bumatic    (501) staff       (20)     3302 2024-05-23 19:59:03.000000 pycatflow-0.1.1/pycatflow.egg-info/PKG-INFO
--rw-r--r--   0 bumatic    (501) staff       (20)      263 2024-05-23 19:59:03.000000 pycatflow-0.1.1/pycatflow.egg-info/SOURCES.txt
--rw-r--r--   0 bumatic    (501) staff       (20)        1 2024-05-23 19:59:03.000000 pycatflow-0.1.1/pycatflow.egg-info/dependency_links.txt
--rw-r--r--   0 bumatic    (501) staff       (20)       23 2024-05-23 19:59:03.000000 pycatflow-0.1.1/pycatflow.egg-info/requires.txt
--rw-r--r--   0 bumatic    (501) staff       (20)       10 2024-05-23 19:59:03.000000 pycatflow-0.1.1/pycatflow.egg-info/top_level.txt
--rw-rw-r--   0 bumatic    (501) staff       (20)      108 2021-10-03 11:41:14.000000 pycatflow-0.1.1/pyproject.toml
--rw-r--r--   0 bumatic    (501) staff       (20)       38 2024-05-23 19:59:03.404068 pycatflow-0.1.1/setup.cfg
--rw-rw-r--   0 bumatic    (501) staff       (20)      788 2024-05-23 19:58:25.000000 pycatflow-0.1.1/setup.py
+drwxr-xr-x   0 bumatic    (501) staff       (20)        0 2024-05-23 20:03:33.047376 pycatflow-0.1.1a0/
+-rw-rw-r--   0 bumatic    (501) staff       (20)     1077 2021-10-03 11:41:14.000000 pycatflow-0.1.1a0/LICENSE
+-rw-r--r--   0 bumatic    (501) staff       (20)     3308 2024-05-23 20:03:33.026826 pycatflow-0.1.1a0/PKG-INFO
+-rw-rw-r--   0 bumatic    (501) staff       (20)     2844 2021-10-03 11:41:14.000000 pycatflow-0.1.1a0/README.md
+drwxr-xr-x   0 bumatic    (501) staff       (20)        0 2024-05-23 20:03:32.968984 pycatflow-0.1.1a0/pycatflow/
+-rw-rw-r--   0 bumatic    (501) staff       (20)       40 2021-10-03 11:41:14.000000 pycatflow-0.1.1a0/pycatflow/__init__.py
+-rw-rw-r--   0 bumatic    (501) staff       (20)     9068 2021-10-03 11:41:14.000000 pycatflow-0.1.1a0/pycatflow/input.py
+-rw-rw-r--   0 bumatic    (501) staff       (20)    27937 2021-10-03 11:41:14.000000 pycatflow-0.1.1a0/pycatflow/viz.py
+drwxr-xr-x   0 bumatic    (501) staff       (20)        0 2024-05-23 20:03:33.022929 pycatflow-0.1.1a0/pycatflow.egg-info/
+-rw-r--r--   0 bumatic    (501) staff       (20)     3308 2024-05-23 20:03:32.000000 pycatflow-0.1.1a0/pycatflow.egg-info/PKG-INFO
+-rw-r--r--   0 bumatic    (501) staff       (20)      263 2024-05-23 20:03:32.000000 pycatflow-0.1.1a0/pycatflow.egg-info/SOURCES.txt
+-rw-r--r--   0 bumatic    (501) staff       (20)        1 2024-05-23 20:03:32.000000 pycatflow-0.1.1a0/pycatflow.egg-info/dependency_links.txt
+-rw-r--r--   0 bumatic    (501) staff       (20)       27 2024-05-23 20:03:32.000000 pycatflow-0.1.1a0/pycatflow.egg-info/requires.txt
+-rw-r--r--   0 bumatic    (501) staff       (20)       10 2024-05-23 20:03:32.000000 pycatflow-0.1.1a0/pycatflow.egg-info/top_level.txt
+-rw-rw-r--   0 bumatic    (501) staff       (20)      108 2021-10-03 11:41:14.000000 pycatflow-0.1.1a0/pyproject.toml
+-rw-r--r--   0 bumatic    (501) staff       (20)       38 2024-05-23 20:03:33.047651 pycatflow-0.1.1a0/setup.cfg
+-rw-rw-r--   0 bumatic    (501) staff       (20)      793 2024-05-23 20:03:03.000000 pycatflow-0.1.1a0/setup.py
```

### Comparing `pycatflow-0.1.1/LICENSE` & `pycatflow-0.1.1a0/LICENSE`

 * *Files identical despite different names*

### Comparing `pycatflow-0.1.1/PKG-INFO` & `pycatflow-0.1.1a0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: pycatflow
-Version: 0.1.1
+Version: 0.1.1a0
 Summary: A tool for visualizing categorical data over time.
 Home-page: https://github.com/bumatic/PyCatFlow
 Author: Marcus Burkhardt
 Author-email: marcus.burkhardt@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: drawSVG<2.0
-Requires-Dist: matplotlib
+Requires-Dist: matplotlib<3.9
 
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5531785.svg)](https://doi.org/10.5281/zenodo.5531785)
 
 # PyCatFlow
 
 This package is a visualization tool which allows the representation of temporal developments, based on categorical data. I wrote a short [article on Medium](https://medium.com/@bumatic/pycatflow-visualizing-categorical-data-over-time-b344102bcce2) in which I outline the basic idea of PyCatFlow and provide a Tutorial for non-programmers based on a [Jupyter Notebook with interactive widgets that can be run online](https://mybinder.org/v2/gist/bumatic/83c3423595cde010da7ad059c6b8b2f5/HEAD).
```

### Comparing `pycatflow-0.1.1/README.md` & `pycatflow-0.1.1a0/README.md`

 * *Files identical despite different names*

### Comparing `pycatflow-0.1.1/pycatflow/input.py` & `pycatflow-0.1.1a0/pycatflow/input.py`

 * *Files identical despite different names*

### Comparing `pycatflow-0.1.1/pycatflow/viz.py` & `pycatflow-0.1.1a0/pycatflow/viz.py`

 * *Files identical despite different names*

### Comparing `pycatflow-0.1.1/pycatflow.egg-info/PKG-INFO` & `pycatflow-0.1.1a0/pycatflow.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: pycatflow
-Version: 0.1.1
+Version: 0.1.1a0
 Summary: A tool for visualizing categorical data over time.
 Home-page: https://github.com/bumatic/PyCatFlow
 Author: Marcus Burkhardt
 Author-email: marcus.burkhardt@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: drawSVG<2.0
-Requires-Dist: matplotlib
+Requires-Dist: matplotlib<3.9
 
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5531785.svg)](https://doi.org/10.5281/zenodo.5531785)
 
 # PyCatFlow
 
 This package is a visualization tool which allows the representation of temporal developments, based on categorical data. I wrote a short [article on Medium](https://medium.com/@bumatic/pycatflow-visualizing-categorical-data-over-time-b344102bcce2) in which I outline the basic idea of PyCatFlow and provide a Tutorial for non-programmers based on a [Jupyter Notebook with interactive widgets that can be run online](https://mybinder.org/v2/gist/bumatic/83c3423595cde010da7ad059c6b8b2f5/HEAD).
```

### Comparing `pycatflow-0.1.1/setup.py` & `pycatflow-0.1.1a0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pycatflow", 
-    version="0.1.1",
+    version="0.1.1a",
     author="Marcus Burkhardt",
     author_email="marcus.burkhardt@gmail.com",
     description="A tool for visualizing categorical data over time.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/bumatic/PyCatFlow",
     license="MIT",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     packages=setuptools.find_packages(),
     python_requires=">=3.6",
-    install_requires=['drawSVG<2.0', 'matplotlib']
+    install_requires=['drawSVG<2.0', 'matplotlib<3.9']
 )
```

