# Comparing `tmp/petannotationvisualizer-1.2.1.tar.gz` & `tmp/petannotationvisualizer-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "petannotationvisualizer-1.2.1.tar", last modified: Thu May 23 10:08:56 2024, max compression
+gzip compressed data, was "petannotationvisualizer-1.2.2.tar", last modified: Thu May 23 10:13:03 2024, max compression
```

## Comparing `petannotationvisualizer-1.2.1.tar` & `petannotationvisualizer-1.2.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 patrizio   (501) staff       (20)        0 2024-05-23 10:08:56.610881 petannotationvisualizer-1.2.1/
-drwxr-xr-x   0 patrizio   (501) staff       (20)        0 2024-05-23 10:08:56.609402 petannotationvisualizer-1.2.1/PETvisualizer/
--rw-r--r--   0 patrizio   (501) staff       (20)     8180 2024-05-23 08:26:51.000000 petannotationvisualizer-1.2.1/PETvisualizer/Colors.py
--rw-r--r--   0 patrizio   (501) staff       (20)      900 2024-05-23 08:26:51.000000 petannotationvisualizer-1.2.1/PETvisualizer/CreateProcessGraph.py
--rw-r--r--   0 patrizio   (501) staff       (20)    12161 2024-05-23 08:26:51.000000 petannotationvisualizer-1.2.1/PETvisualizer/Labels.py
--rw-r--r--   0 patrizio   (501) staff       (20)    75339 2024-05-23 08:26:51.000000 petannotationvisualizer-1.2.1/PETvisualizer/PETVisualizer.py
--rw-r--r--   0 patrizio   (501) staff       (20)    27436 2024-05-23 08:26:51.000000 petannotationvisualizer-1.2.1/PETvisualizer/ShowProcessGraph.py
--rw-r--r--   0 patrizio   (501) staff       (20)        0 2024-05-23 08:26:51.000000 petannotationvisualizer-1.2.1/PETvisualizer/__init__.py
--rw-r--r--   0 patrizio   (501) staff       (20)       55 2024-05-23 08:26:51.000000 petannotationvisualizer-1.2.1/PETvisualizer/main.py
--rw-r--r--   0 patrizio   (501) staff       (20)   195459 2024-05-23 08:26:51.000000 petannotationvisualizer-1.2.1/PETvisualizer/pet-entities.json
--rw-r--r--   0 patrizio   (501) staff       (20)   502158 2024-05-23 08:26:51.000000 petannotationvisualizer-1.2.1/PETvisualizer/pet-relations.json
--rw-r--r--   0 patrizio   (501) staff       (20)     8266 2024-05-23 08:26:51.000000 petannotationvisualizer-1.2.1/PETvisualizer/utility.py
--rw-r--r--   0 patrizio   (501) staff       (20)    12864 2024-05-23 08:26:51.000000 petannotationvisualizer-1.2.1/PETvisualizer/wolfgold.png
--rw-r--r--   0 patrizio   (501) staff       (20)    11168 2024-05-23 10:08:56.610674 petannotationvisualizer-1.2.1/PKG-INFO
--rw-r--r--   0 patrizio   (501) staff       (20)     9779 2024-05-23 10:08:56.000000 petannotationvisualizer-1.2.1/README.md
-drwxr-xr-x   0 patrizio   (501) staff       (20)        0 2024-05-23 10:08:56.610436 petannotationvisualizer-1.2.1/petannotationvisualizer.egg-info/
--rw-r--r--   0 patrizio   (501) staff       (20)    11168 2024-05-23 10:08:56.000000 petannotationvisualizer-1.2.1/petannotationvisualizer.egg-info/PKG-INFO
--rw-r--r--   0 patrizio   (501) staff       (20)      566 2024-05-23 10:08:56.000000 petannotationvisualizer-1.2.1/petannotationvisualizer.egg-info/SOURCES.txt
--rw-r--r--   0 patrizio   (501) staff       (20)        1 2024-05-23 10:08:56.000000 petannotationvisualizer-1.2.1/petannotationvisualizer.egg-info/dependency_links.txt
--rw-r--r--   0 patrizio   (501) staff       (20)       64 2024-05-23 10:08:56.000000 petannotationvisualizer-1.2.1/petannotationvisualizer.egg-info/requires.txt
--rw-r--r--   0 patrizio   (501) staff       (20)       14 2024-05-23 10:08:56.000000 petannotationvisualizer-1.2.1/petannotationvisualizer.egg-info/top_level.txt
--rw-r--r--   0 patrizio   (501) staff       (20)       38 2024-05-23 10:08:56.610932 petannotationvisualizer-1.2.1/setup.cfg
--rw-r--r--   0 patrizio   (501) staff       (20)     2245 2024-05-23 09:47:16.000000 petannotationvisualizer-1.2.1/setup.py
+drwxr-xr-x   0 patrizio   (501) staff       (20)        0 2024-05-23 10:13:03.460204 petannotationvisualizer-1.2.2/
+drwxr-xr-x   0 patrizio   (501) staff       (20)        0 2024-05-23 10:13:03.445869 petannotationvisualizer-1.2.2/PETvisualizer/
+-rw-r--r--   0 patrizio   (501) staff       (20)     8180 2024-05-23 08:26:51.000000 petannotationvisualizer-1.2.2/PETvisualizer/Colors.py
+-rw-r--r--   0 patrizio   (501) staff       (20)      900 2024-05-23 08:26:51.000000 petannotationvisualizer-1.2.2/PETvisualizer/CreateProcessGraph.py
+-rw-r--r--   0 patrizio   (501) staff       (20)    12161 2024-05-23 08:26:51.000000 petannotationvisualizer-1.2.2/PETvisualizer/Labels.py
+-rw-r--r--   0 patrizio   (501) staff       (20)    75339 2024-05-23 08:26:51.000000 petannotationvisualizer-1.2.2/PETvisualizer/PETVisualizer.py
+-rw-r--r--   0 patrizio   (501) staff       (20)    27436 2024-05-23 08:26:51.000000 petannotationvisualizer-1.2.2/PETvisualizer/ShowProcessGraph.py
+-rw-r--r--   0 patrizio   (501) staff       (20)        0 2024-05-23 08:26:51.000000 petannotationvisualizer-1.2.2/PETvisualizer/__init__.py
+-rw-r--r--   0 patrizio   (501) staff       (20)       55 2024-05-23 08:26:51.000000 petannotationvisualizer-1.2.2/PETvisualizer/main.py
+-rw-r--r--   0 patrizio   (501) staff       (20)   195459 2024-05-23 08:26:51.000000 petannotationvisualizer-1.2.2/PETvisualizer/pet-entities.json
+-rw-r--r--   0 patrizio   (501) staff       (20)   502158 2024-05-23 08:26:51.000000 petannotationvisualizer-1.2.2/PETvisualizer/pet-relations.json
+-rw-r--r--   0 patrizio   (501) staff       (20)     8266 2024-05-23 08:26:51.000000 petannotationvisualizer-1.2.2/PETvisualizer/utility.py
+-rw-r--r--   0 patrizio   (501) staff       (20)    12864 2024-05-23 08:26:51.000000 petannotationvisualizer-1.2.2/PETvisualizer/wolfgold.png
+-rw-r--r--   0 patrizio   (501) staff       (20)    11172 2024-05-23 10:13:03.455976 petannotationvisualizer-1.2.2/PKG-INFO
+-rw-r--r--   0 patrizio   (501) staff       (20)     9783 2024-05-23 10:12:20.000000 petannotationvisualizer-1.2.2/README.md
+drwxr-xr-x   0 patrizio   (501) staff       (20)        0 2024-05-23 10:13:03.455648 petannotationvisualizer-1.2.2/petannotationvisualizer.egg-info/
+-rw-r--r--   0 patrizio   (501) staff       (20)    11172 2024-05-23 10:13:03.000000 petannotationvisualizer-1.2.2/petannotationvisualizer.egg-info/PKG-INFO
+-rw-r--r--   0 patrizio   (501) staff       (20)      566 2024-05-23 10:13:03.000000 petannotationvisualizer-1.2.2/petannotationvisualizer.egg-info/SOURCES.txt
+-rw-r--r--   0 patrizio   (501) staff       (20)        1 2024-05-23 10:13:03.000000 petannotationvisualizer-1.2.2/petannotationvisualizer.egg-info/dependency_links.txt
+-rw-r--r--   0 patrizio   (501) staff       (20)       64 2024-05-23 10:13:03.000000 petannotationvisualizer-1.2.2/petannotationvisualizer.egg-info/requires.txt
+-rw-r--r--   0 patrizio   (501) staff       (20)       14 2024-05-23 10:13:03.000000 petannotationvisualizer-1.2.2/petannotationvisualizer.egg-info/top_level.txt
+-rw-r--r--   0 patrizio   (501) staff       (20)       38 2024-05-23 10:13:03.460291 petannotationvisualizer-1.2.2/setup.cfg
+-rw-r--r--   0 patrizio   (501) staff       (20)     2245 2024-05-23 10:13:03.000000 petannotationvisualizer-1.2.2/setup.py
```

### Comparing `petannotationvisualizer-1.2.1/PETvisualizer/Colors.py` & `petannotationvisualizer-1.2.2/PETvisualizer/Colors.py`

 * *Files identical despite different names*

### Comparing `petannotationvisualizer-1.2.1/PETvisualizer/CreateProcessGraph.py` & `petannotationvisualizer-1.2.2/PETvisualizer/CreateProcessGraph.py`

 * *Files identical despite different names*

### Comparing `petannotationvisualizer-1.2.1/PETvisualizer/Labels.py` & `petannotationvisualizer-1.2.2/PETvisualizer/Labels.py`

 * *Files identical despite different names*

### Comparing `petannotationvisualizer-1.2.1/PETvisualizer/PETVisualizer.py` & `petannotationvisualizer-1.2.2/PETvisualizer/PETVisualizer.py`

 * *Files identical despite different names*

### Comparing `petannotationvisualizer-1.2.1/PETvisualizer/ShowProcessGraph.py` & `petannotationvisualizer-1.2.2/PETvisualizer/ShowProcessGraph.py`

 * *Files identical despite different names*

### Comparing `petannotationvisualizer-1.2.1/PETvisualizer/pet-entities.json` & `petannotationvisualizer-1.2.2/PETvisualizer/pet-entities.json`

 * *Files identical despite different names*

### Comparing `petannotationvisualizer-1.2.1/PETvisualizer/pet-relations.json` & `petannotationvisualizer-1.2.2/PETvisualizer/pet-relations.json`

 * *Files identical despite different names*

### Comparing `petannotationvisualizer-1.2.1/PETvisualizer/utility.py` & `petannotationvisualizer-1.2.2/PETvisualizer/utility.py`

 * *Files identical despite different names*

### Comparing `petannotationvisualizer-1.2.1/PETvisualizer/wolfgold.png` & `petannotationvisualizer-1.2.2/PETvisualizer/wolfgold.png`

 * *Files identical despite different names*

### Comparing `petannotationvisualizer-1.2.1/PKG-INFO` & `petannotationvisualizer-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: petannotationvisualizer
-Version: 1.2.1
+Version: 1.2.2
 Summary: A visualization tool for the PET dataset hosted on Huggingface.
 Home-page: https://pdi.fbk.eu/pet-dataset
 Author: Patrizio Bellan
 Author-email: patrizio.bellan@gmail.com
 Maintainer: Patrizio Bellan
 Maintainer-email: patrizio.bellan@gmail.com
 License: MIT
@@ -120,15 +120,15 @@
 At the bottom part of the card, there are three annotation commands:
 - *Create New Annotation* This command starts the creation of a new annotation.	
 - *Add Annotation* This command adds a newly created annotation to the document.
 - *Delete Annotation* This command deletes the selected annotation.
 
 ***Text Area*** part lies in the central part of the GUI. It shows the text of a document and its annotations. PET elements are highlighted in boxes, while PET relations connect PET elements using labeled arrows. Boxes and relation arrows follow the color schema reported in *Fig.5*.
 
-![Color Schema](https://github.com/patriziobellan86/PETvisualizer/blob/master/img/colorschema.jpg)
+![Color Schema](https://github.com/patriziobellan86/PETvisualizer/blob/master/figures/colorschema.jpg)
 *Fig.5 Relations menu.*
 
 
 Dependencies installation notes
 ===============================
 If the installation of requirements fails, you need to downgrade the setuptool and wheel packages.
 run the following command in a terminal:
```

### Comparing `petannotationvisualizer-1.2.1/README.md` & `petannotationvisualizer-1.2.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -88,15 +88,15 @@
 At the bottom part of the card, there are three annotation commands:
 - *Create New Annotation* This command starts the creation of a new annotation.	
 - *Add Annotation* This command adds a newly created annotation to the document.
 - *Delete Annotation* This command deletes the selected annotation.
 
 ***Text Area*** part lies in the central part of the GUI. It shows the text of a document and its annotations. PET elements are highlighted in boxes, while PET relations connect PET elements using labeled arrows. Boxes and relation arrows follow the color schema reported in *Fig.5*.
 
-![Color Schema](https://github.com/patriziobellan86/PETvisualizer/blob/master/img/colorschema.jpg)
+![Color Schema](https://github.com/patriziobellan86/PETvisualizer/blob/master/figures/colorschema.jpg)
 *Fig.5 Relations menu.*
 
 
 Dependencies installation notes
 ===============================
 If the installation of requirements fails, you need to downgrade the setuptool and wheel packages.
 run the following command in a terminal:
```

### Comparing `petannotationvisualizer-1.2.1/petannotationvisualizer.egg-info/PKG-INFO` & `petannotationvisualizer-1.2.2/petannotationvisualizer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: petannotationvisualizer
-Version: 1.2.1
+Version: 1.2.2
 Summary: A visualization tool for the PET dataset hosted on Huggingface.
 Home-page: https://pdi.fbk.eu/pet-dataset
 Author: Patrizio Bellan
 Author-email: patrizio.bellan@gmail.com
 Maintainer: Patrizio Bellan
 Maintainer-email: patrizio.bellan@gmail.com
 License: MIT
@@ -120,15 +120,15 @@
 At the bottom part of the card, there are three annotation commands:
 - *Create New Annotation* This command starts the creation of a new annotation.	
 - *Add Annotation* This command adds a newly created annotation to the document.
 - *Delete Annotation* This command deletes the selected annotation.
 
 ***Text Area*** part lies in the central part of the GUI. It shows the text of a document and its annotations. PET elements are highlighted in boxes, while PET relations connect PET elements using labeled arrows. Boxes and relation arrows follow the color schema reported in *Fig.5*.
 
-![Color Schema](https://github.com/patriziobellan86/PETvisualizer/blob/master/img/colorschema.jpg)
+![Color Schema](https://github.com/patriziobellan86/PETvisualizer/blob/master/figures/colorschema.jpg)
 *Fig.5 Relations menu.*
 
 
 Dependencies installation notes
 ===============================
 If the installation of requirements fails, you need to downgrade the setuptool and wheel packages.
 run the following command in a terminal:
```

### Comparing `petannotationvisualizer-1.2.1/petannotationvisualizer.egg-info/SOURCES.txt` & `petannotationvisualizer-1.2.2/petannotationvisualizer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `petannotationvisualizer-1.2.1/setup.py` & `petannotationvisualizer-1.2.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 _REQUIRED = ['networkx','tqdm','petdatasetreader','matplotlib','mplcursors','pygraphviz']
 _EXTRAS = []
 
 setup(
     name='petannotationvisualizer',
-    version='1.2.1',
+    version='1.2.2',
     packages=find_packages(exclude=("tests", "docs", "dist", "build")),
     install_requires=_REQUIRED,
     # extras_require=_EXTRAS,
     package_data={'': ['*.json', '*.png', ]},
     include_package_data=True,
     platforms="Any",
```

