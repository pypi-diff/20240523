# Comparing `tmp/twogroups_heatmap-0.1.tar.gz` & `tmp/twogroups_heatmap-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twogroups_heatmap-0.1.tar", last modified: Wed May 15 09:51:56 2024, max compression
+gzip compressed data, was "twogroups_heatmap-0.1.1.tar", last modified: Thu May 23 06:31:35 2024, max compression
```

## Comparing `twogroups_heatmap-0.1.tar` & `twogroups_heatmap-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwsr-x   0 edoardo.giacopuzzi  (3721) gassu-w   (7972)        0 2024-05-15 09:51:56.117469 twogroups_heatmap-0.1/
--rwxrwxr-x   0 edoardo.giacopuzzi  (3721) gassu-w   (7972)     1074 2024-05-15 08:41:37.000000 twogroups_heatmap-0.1/LICENSE
--rw-r--r--   0 edoardo.giacopuzzi  (3721) gassu-w   (7972)     2638 2024-05-15 09:51:56.100737 twogroups_heatmap-0.1/PKG-INFO
--rw-rw-r--   0 edoardo.giacopuzzi  (3721) gassu-w   (7972)      562 2024-05-15 09:09:04.000000 twogroups_heatmap-0.1/README.md
--rwxrwxr-x   0 edoardo.giacopuzzi  (3721) gassu-w   (7972)      860 2024-05-15 09:51:48.000000 twogroups_heatmap-0.1/pyproject.toml
--rw-rw-r--   0 edoardo.giacopuzzi  (3721) gassu-w   (7972)       38 2024-05-15 09:51:56.122740 twogroups_heatmap-0.1/setup.cfg
--rwxrwxr-x   0 edoardo.giacopuzzi  (3721) gassu-w   (7972)      857 2024-05-15 09:01:21.000000 twogroups_heatmap-0.1/setup.py
-drwxrwsr-x   0 edoardo.giacopuzzi  (3721) gassu-w   (7972)        0 2024-05-15 09:51:56.075959 twogroups_heatmap-0.1/twogroups_heatmap.egg-info/
--rw-r--r--   0 edoardo.giacopuzzi  (3721) gassu-w   (7972)     2638 2024-05-15 09:51:55.000000 twogroups_heatmap-0.1/twogroups_heatmap.egg-info/PKG-INFO
--rw-rw-r--   0 edoardo.giacopuzzi  (3721) gassu-w   (7972)      245 2024-05-15 09:51:55.000000 twogroups_heatmap-0.1/twogroups_heatmap.egg-info/SOURCES.txt
--rw-rw-r--   0 edoardo.giacopuzzi  (3721) gassu-w   (7972)        1 2024-05-15 09:51:55.000000 twogroups_heatmap-0.1/twogroups_heatmap.egg-info/dependency_links.txt
--rw-rw-r--   0 edoardo.giacopuzzi  (3721) gassu-w   (7972)       32 2024-05-15 09:51:55.000000 twogroups_heatmap-0.1/twogroups_heatmap.egg-info/requires.txt
--rw-rw-r--   0 edoardo.giacopuzzi  (3721) gassu-w   (7972)        1 2024-05-15 09:51:55.000000 twogroups_heatmap-0.1/twogroups_heatmap.egg-info/top_level.txt
+drwxrwsr-x   0 edoardo.giacopuzzi  (3721) gassu-w   (7972)        0 2024-05-23 06:31:35.102248 twogroups_heatmap-0.1.1/
+-rwxrwxr-x   0 edoardo.giacopuzzi  (3721) gassu-w   (7972)     1074 2024-05-15 08:41:37.000000 twogroups_heatmap-0.1.1/LICENSE
+-rw-r--r--   0 edoardo.giacopuzzi  (3721) gassu-w   (7972)     2661 2024-05-23 06:31:35.048458 twogroups_heatmap-0.1.1/PKG-INFO
+-rw-rw-r--   0 edoardo.giacopuzzi  (3721) gassu-w   (7972)      562 2024-05-15 09:09:04.000000 twogroups_heatmap-0.1.1/README.md
+-rwxrwxr-x   0 edoardo.giacopuzzi  (3721) gassu-w   (7972)      883 2024-05-23 06:29:10.000000 twogroups_heatmap-0.1.1/pyproject.toml
+-rw-rw-r--   0 edoardo.giacopuzzi  (3721) gassu-w   (7972)       38 2024-05-23 06:31:35.112283 twogroups_heatmap-0.1.1/setup.cfg
+-rwxrwxr-x   0 edoardo.giacopuzzi  (3721) gassu-w   (7972)      859 2024-05-23 06:29:35.000000 twogroups_heatmap-0.1.1/setup.py
+drwxrwsr-x   0 edoardo.giacopuzzi  (3721) gassu-w   (7972)        0 2024-05-23 06:31:34.959496 twogroups_heatmap-0.1.1/twogroups_heatmap.egg-info/
+-rw-r--r--   0 edoardo.giacopuzzi  (3721) gassu-w   (7972)     2661 2024-05-23 06:31:32.000000 twogroups_heatmap-0.1.1/twogroups_heatmap.egg-info/PKG-INFO
+-rw-rw-r--   0 edoardo.giacopuzzi  (3721) gassu-w   (7972)      245 2024-05-23 06:31:33.000000 twogroups_heatmap-0.1.1/twogroups_heatmap.egg-info/SOURCES.txt
+-rw-rw-r--   0 edoardo.giacopuzzi  (3721) gassu-w   (7972)        1 2024-05-23 06:31:32.000000 twogroups_heatmap-0.1.1/twogroups_heatmap.egg-info/dependency_links.txt
+-rw-rw-r--   0 edoardo.giacopuzzi  (3721) gassu-w   (7972)       54 2024-05-23 06:31:32.000000 twogroups_heatmap-0.1.1/twogroups_heatmap.egg-info/requires.txt
+-rw-rw-r--   0 edoardo.giacopuzzi  (3721) gassu-w   (7972)        1 2024-05-23 06:31:32.000000 twogroups_heatmap-0.1.1/twogroups_heatmap.egg-info/top_level.txt
```

### Comparing `twogroups_heatmap-0.1/LICENSE` & `twogroups_heatmap-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `twogroups_heatmap-0.1/PKG-INFO` & `twogroups_heatmap-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twogroups_heatmap
-Version: 0.1
+Version: 0.1.1
 Summary: Create a heatmap of representing intersection between two groups
 Home-page: https://github.com/HTGenomeAnalysisUnit/sc_2g_heatmap.git
 Author: Giuditta Clerici
 Author-email: Giuditta Clerici <giuditta.clerici@external.fht.org>, Edoardo Giacopuzzi <edoardo.giacopuzzi@external.fht.org>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -26,21 +26,21 @@
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/HTGenomeAnalysisUnit/sc_2g_heatmap.git
 Project-URL: Issues, https://github.com/HTGenomeAnalysisUnit/sc_2g_heatmap/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: seaborn
-Requires-Dist: pandas
-Requires-Dist: numpy
-Requires-Dist: matplotlib
+Requires-Dist: seaborn>=0.12
+Requires-Dist: pandas>=1.5
+Requires-Dist: numpy>=1.23
+Requires-Dist: matplotlib>=3.6
 
 # Two groups heatmap
 
 Generate an heatmap comparing overlaps between 2 set of labels in a pandas dataframe. This is useful in single-cell to compare the overlap between two clustering methods or 2 sets of cell type labels.
 
 ## Installation
```

### Comparing `twogroups_heatmap-0.1/README.md` & `twogroups_heatmap-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `twogroups_heatmap-0.1/pyproject.toml` & `twogroups_heatmap-0.1.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [project]
 name = "twogroups_heatmap"
-version = "0.1"
+version = "0.1.1"
 authors = [
   { name="Giuditta Clerici", email="giuditta.clerici@external.fht.org" },
   { name="Edoardo Giacopuzzi", email="edoardo.giacopuzzi@external.fht.org" }
 ]
 description = "Create a heatmap of representing intersection between two groups"
 readme = "README.md"
 license = {file = "LICENSE"}
-requires-python = ">=3.10"
+requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-    "seaborn",
-    "pandas",
-    "numpy",
-    "matplotlib",
+    "seaborn>=0.12",
+    "pandas>=1.5",
+    "numpy>=1.23",
+    "matplotlib>=3.6",
 ]
 
 [project.urls]
 Homepage = "https://github.com/HTGenomeAnalysisUnit/sc_2g_heatmap.git"
 Issues = "https://github.com/HTGenomeAnalysisUnit/sc_2g_heatmap/issues"
 
 [build-system]
```

### Comparing `twogroups_heatmap-0.1/setup.py` & `twogroups_heatmap-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 here = pathlib.Path(__file__).parent.resolve()
 
 # Get the long description from the README file
 long_description = (here / 'README.md').read_text(encoding='utf-8')
 
 setup(
     name='twogroups_heatmap',
-    version='0.1',
+    version='0.1.1',
     description='Create a heatmap of representing intersection between two groups',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/HTGenomeAnalysisUnit/sc_2g_heatmap.git',
     author='Giuditta Clerici',
     author_email='giuditta.clerici@external.ght.org',
     classifiers=[
```

### Comparing `twogroups_heatmap-0.1/twogroups_heatmap.egg-info/PKG-INFO` & `twogroups_heatmap-0.1.1/twogroups_heatmap.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twogroups_heatmap
-Version: 0.1
+Version: 0.1.1
 Summary: Create a heatmap of representing intersection between two groups
 Home-page: https://github.com/HTGenomeAnalysisUnit/sc_2g_heatmap.git
 Author: Giuditta Clerici
 Author-email: Giuditta Clerici <giuditta.clerici@external.fht.org>, Edoardo Giacopuzzi <edoardo.giacopuzzi@external.fht.org>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -26,21 +26,21 @@
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/HTGenomeAnalysisUnit/sc_2g_heatmap.git
 Project-URL: Issues, https://github.com/HTGenomeAnalysisUnit/sc_2g_heatmap/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: seaborn
-Requires-Dist: pandas
-Requires-Dist: numpy
-Requires-Dist: matplotlib
+Requires-Dist: seaborn>=0.12
+Requires-Dist: pandas>=1.5
+Requires-Dist: numpy>=1.23
+Requires-Dist: matplotlib>=3.6
 
 # Two groups heatmap
 
 Generate an heatmap comparing overlaps between 2 set of labels in a pandas dataframe. This is useful in single-cell to compare the overlap between two clustering methods or 2 sets of cell type labels.
 
 ## Installation
```

