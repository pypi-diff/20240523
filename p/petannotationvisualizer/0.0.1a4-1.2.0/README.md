# Comparing `tmp/PETAnnotationVisualizer-0.0.1a4.tar.gz` & `tmp/petannotationvisualizer-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PETAnnotationVisualizer-0.0.1a4.tar", last modified: Sun May 29 10:26:10 2022, max compression
+gzip compressed data, was "petannotationvisualizer-1.2.0.tar", last modified: Thu May 23 09:43:08 2024, max compression
```

## Comparing `PETAnnotationVisualizer-0.0.1a4.tar` & `petannotationvisualizer-1.2.0.tar`

### file list

```diff
@@ -1,19 +1,23 @@
-drwxr-xr-x   0 patrizio   (501) staff       (20)        0 2022-05-29 10:26:10.358692 PETAnnotationVisualizer-0.0.1a4/
--rw-r--r--   0 patrizio   (501) staff       (20)        0 2022-05-10 20:52:11.000000 PETAnnotationVisualizer-0.0.1a4/LICENSE.txt
--rw-r--r--   0 patrizio   (501) staff       (20)       41 2022-05-29 10:06:04.000000 PETAnnotationVisualizer-0.0.1a4/MANIFEST.in
-drwxr-xr-x   0 patrizio   (501) staff       (20)        0 2022-05-29 10:26:10.357619 PETAnnotationVisualizer-0.0.1a4/PETAnnotationVisualizer/
--rw-r--r--   0 patrizio   (501) staff       (20)     7144 2021-11-22 17:01:46.000000 PETAnnotationVisualizer-0.0.1a4/PETAnnotationVisualizer/Colors.py
--rw-r--r--   0 patrizio   (501) staff       (20)    46985 2022-05-29 10:25:56.000000 PETAnnotationVisualizer-0.0.1a4/PETAnnotationVisualizer/Visualizer.py
--rw-r--r--   0 patrizio   (501) staff       (20)        0 2021-10-28 12:23:14.000000 PETAnnotationVisualizer-0.0.1a4/PETAnnotationVisualizer/__init__.py
--rw-r--r--   0 patrizio   (501) staff       (20)     4988 2021-12-17 15:19:16.000000 PETAnnotationVisualizer-0.0.1a4/PETAnnotationVisualizer/logo.png
--rw-r--r--   0 patrizio   (501) staff       (20)      428 2021-11-22 17:01:21.000000 PETAnnotationVisualizer-0.0.1a4/PETAnnotationVisualizer/printColors.py
-drwxr-xr-x   0 patrizio   (501) staff       (20)        0 2022-05-29 10:26:10.358345 PETAnnotationVisualizer-0.0.1a4/PETAnnotationVisualizer.egg-info/
--rw-r--r--   0 patrizio   (501) staff       (20)     1729 2022-05-29 10:26:10.000000 PETAnnotationVisualizer-0.0.1a4/PETAnnotationVisualizer.egg-info/PKG-INFO
--rw-r--r--   0 patrizio   (501) staff       (20)      457 2022-05-29 10:26:10.000000 PETAnnotationVisualizer-0.0.1a4/PETAnnotationVisualizer.egg-info/SOURCES.txt
--rw-r--r--   0 patrizio   (501) staff       (20)        1 2022-05-29 10:26:10.000000 PETAnnotationVisualizer-0.0.1a4/PETAnnotationVisualizer.egg-info/dependency_links.txt
--rw-r--r--   0 patrizio   (501) staff       (20)       34 2022-05-29 10:26:10.000000 PETAnnotationVisualizer-0.0.1a4/PETAnnotationVisualizer.egg-info/requires.txt
--rw-r--r--   0 patrizio   (501) staff       (20)       24 2022-05-29 10:26:10.000000 PETAnnotationVisualizer-0.0.1a4/PETAnnotationVisualizer.egg-info/top_level.txt
--rw-r--r--   0 patrizio   (501) staff       (20)     1729 2022-05-29 10:26:10.358532 PETAnnotationVisualizer-0.0.1a4/PKG-INFO
--rw-r--r--   0 patrizio   (501) staff       (20)      597 2022-05-20 14:26:49.000000 PETAnnotationVisualizer-0.0.1a4/README.rst
--rw-r--r--   0 patrizio   (501) staff       (20)       38 2022-05-29 10:26:10.358744 PETAnnotationVisualizer-0.0.1a4/setup.cfg
--rw-r--r--   0 patrizio   (501) staff       (20)     1827 2022-05-29 10:26:01.000000 PETAnnotationVisualizer-0.0.1a4/setup.py
+drwxr-xr-x   0 patrizio   (501) staff       (20)        0 2024-05-23 09:43:08.159063 petannotationvisualizer-1.2.0/
+drwxr-xr-x   0 patrizio   (501) staff       (20)        0 2024-05-23 09:43:08.157745 petannotationvisualizer-1.2.0/PETvisualizer/
+-rw-r--r--   0 patrizio   (501) staff       (20)     8180 2024-05-23 08:26:51.000000 petannotationvisualizer-1.2.0/PETvisualizer/Colors.py
+-rw-r--r--   0 patrizio   (501) staff       (20)      900 2024-05-23 08:26:51.000000 petannotationvisualizer-1.2.0/PETvisualizer/CreateProcessGraph.py
+-rw-r--r--   0 patrizio   (501) staff       (20)    12161 2024-05-23 08:26:51.000000 petannotationvisualizer-1.2.0/PETvisualizer/Labels.py
+-rw-r--r--   0 patrizio   (501) staff       (20)    75339 2024-05-23 08:26:51.000000 petannotationvisualizer-1.2.0/PETvisualizer/PETVisualizer.py
+-rw-r--r--   0 patrizio   (501) staff       (20)    27436 2024-05-23 08:26:51.000000 petannotationvisualizer-1.2.0/PETvisualizer/ShowProcessGraph.py
+-rw-r--r--   0 patrizio   (501) staff       (20)        0 2024-05-23 08:26:51.000000 petannotationvisualizer-1.2.0/PETvisualizer/__init__.py
+-rw-r--r--   0 patrizio   (501) staff       (20)       55 2024-05-23 08:26:51.000000 petannotationvisualizer-1.2.0/PETvisualizer/main.py
+-rw-r--r--   0 patrizio   (501) staff       (20)   195459 2024-05-23 08:26:51.000000 petannotationvisualizer-1.2.0/PETvisualizer/pet-entities.json
+-rw-r--r--   0 patrizio   (501) staff       (20)   502158 2024-05-23 08:26:51.000000 petannotationvisualizer-1.2.0/PETvisualizer/pet-relations.json
+-rw-r--r--   0 patrizio   (501) staff       (20)     8266 2024-05-23 08:26:51.000000 petannotationvisualizer-1.2.0/PETvisualizer/utility.py
+-rw-r--r--   0 patrizio   (501) staff       (20)    12864 2024-05-23 08:26:51.000000 petannotationvisualizer-1.2.0/PETvisualizer/wolfgold.png
+-rw-r--r--   0 patrizio   (501) staff       (20)    11180 2024-05-23 09:43:08.158853 petannotationvisualizer-1.2.0/PKG-INFO
+-rw-r--r--   0 patrizio   (501) staff       (20)     9791 2024-05-23 09:39:10.000000 petannotationvisualizer-1.2.0/README.md
+drwxr-xr-x   0 patrizio   (501) staff       (20)        0 2024-05-23 09:43:08.158640 petannotationvisualizer-1.2.0/petannotationvisualizer.egg-info/
+-rw-r--r--   0 patrizio   (501) staff       (20)    11180 2024-05-23 09:43:08.000000 petannotationvisualizer-1.2.0/petannotationvisualizer.egg-info/PKG-INFO
+-rw-r--r--   0 patrizio   (501) staff       (20)      566 2024-05-23 09:43:08.000000 petannotationvisualizer-1.2.0/petannotationvisualizer.egg-info/SOURCES.txt
+-rw-r--r--   0 patrizio   (501) staff       (20)        1 2024-05-23 09:43:08.000000 petannotationvisualizer-1.2.0/petannotationvisualizer.egg-info/dependency_links.txt
+-rw-r--r--   0 patrizio   (501) staff       (20)       64 2024-05-23 09:43:08.000000 petannotationvisualizer-1.2.0/petannotationvisualizer.egg-info/requires.txt
+-rw-r--r--   0 patrizio   (501) staff       (20)       14 2024-05-23 09:43:08.000000 petannotationvisualizer-1.2.0/petannotationvisualizer.egg-info/top_level.txt
+-rw-r--r--   0 patrizio   (501) staff       (20)       38 2024-05-23 09:43:08.159116 petannotationvisualizer-1.2.0/setup.cfg
+-rw-r--r--   0 patrizio   (501) staff       (20)     2245 2024-05-23 09:43:02.000000 petannotationvisualizer-1.2.0/setup.py
```

### Comparing `PETAnnotationVisualizer-0.0.1a4/PETAnnotationVisualizer/Colors.py` & `petannotationvisualizer-1.2.0/PETvisualizer/Colors.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import numpy as np
-
+from petreader.labels import *
 # =============================================================================
 # COLORS
 # =============================================================================
 
 Null_Color = 'ghost white'
 
 # old, no more used. 
@@ -12,38 +12,40 @@
 #             'Han': 'black',
 #             'Chiara': 'purple',
 #             'Mauro': 'red',
 #             'Simone': 'orange'}
 # the new implementation
 # taken from http://www.science.smith.edu/dftwiki/index.php/Color_Charts_for_TKinter
 MARK_COLORS = {
-    'Activity': 'dark green',
-    'AND Gateway': 'orange',
-    'XOR Gateway': 'red',
-    'Activity Data': 'dark salmon',
-    'Actor': 'royal blue',
-    'Condition Specification': 'gold4',
-    'Further Specification': 'medium orchid',
-
-    'Sequence Flow': 'green',
-    'Uses': 'dark salmon',
-    'Roles': 'blue',
-
-    'Same Gateway': 'red',
-
-    'Activity Data coref mention': 'gold',
-    'Actor coref mention': 'azure',
+   ACTIVITY: 'dark green',
+    AND_GATEWAY: 'orange',
+    XOR_GATEWAY: 'red',
+    ACTIVITY_DATA: 'dark salmon',
+    ACTOR: 'royal blue',
+    CONDITION_SPECIFICATION: 'gold4',
+    FURTHER_SPECIFICATION: 'medium orchid',
+
+    FLOW: 'green',
+    USES: 'dark salmon',
+    ACTOR_PERFORMER: 'blue',
+    ACTOR_RECIPIENT: 'blue',
+    FURTHER_SPECIFICATION_RELATION: 'orchid',
+    SAME_GATEWAY: 'red',
 }
 
+
 PRECISION = 'orange'
 RECALL = 'green'
 F1SCORE = 'blue'
 
 Annotator_Colors = {
-    k:color for k, color in enumerate([ 'dark slate gray', 'dim gray', 'slate gray',
+    k:color for k, color in enumerate(['gainsboro',
+    'linen', 'antique white', 'papaya whip', 'blanched almond', 'bisque', 'peach puff',
+    'navajo white', 'lemon chiffon',
+    'lavender blush', 'misty rose', 'dark slate gray', 'dim gray', 'slate gray',
     'light slate gray', 'gray',  'midnight blue', 'navy', 'cornflower blue', 'dark slate blue',
     'slate blue', 'medium slate blue', 'light slate blue', 'medium blue', 'royal blue',  'blue',
     'dodger blue', 'deep sky blue', 'sky blue', 'light sky blue', 
     'dark turquoise', 'medium turquoise', 'turquoise',
     'cyan', 'cadet blue', 'medium aquamarine',  'dark green', 'dark olive green',
     'dark sea green', 'sea green', 'medium sea green', 'light sea green',
     'medium spring green', 'lime green', 'yellow green',
@@ -56,44 +58,51 @@
     'medium orchid', 'dark orchid', 'dark violet', 'blue violet', 'purple', 'medium purple',
     'snow4',
     'SlateBlue1', 'SlateBlue2', 'SlateBlue3',
     'SlateBlue4', 'RoyalBlue1', 'RoyalBlue2', 'RoyalBlue3', 'RoyalBlue4', 'blue2', 'blue4',
     'DodgerBlue2', 'DodgerBlue3', 'DodgerBlue4', 'SteelBlue1', 'SteelBlue2',
     'SteelBlue3', 'SteelBlue4', 'DeepSkyBlue2', 'DeepSkyBlue3', 'DeepSkyBlue4',
     'SkyBlue3', 'SkyBlue4',
-    'turquoise4', 'cyan2', 'cyan3',
-    'cyan4', 'DarkSlateGray4',
-    'aquamarine2', 'aquamarine4',
+    # 'LightSkyBlue1', 'LightSkyBlue2',
+    # 'LightSkyBlue3', 'LightSkyBlue4', 'SlateGray1', 'SlateGray2', 'SlateGray3',
+    # 'SlateGray4', 'LightSteelBlue1', 'LightSteelBlue2', 'LightSteelBlue3',
+    # 'LightSteelBlue4', 'LightBlue1', 'LightBlue2', 'LightBlue3', 'LightBlue4',
+    # 'LightCyan2', 'LightCyan3', 'LightCyan4', 'PaleTurquoise1', 'PaleTurquoise2',
+    # 'PaleTurquoise3', 'PaleTurquoise4', 'CadetBlue1', 'CadetBlue2', 'CadetBlue3',
+    # 'CadetBlue4',
+    'turquoise1', 'turquoise2', 'turquoise3', 'turquoise4', 'cyan2', 'cyan3',
+    'cyan4', 'DarkSlateGray1', 'DarkSlateGray2', 'DarkSlateGray3', 'DarkSlateGray4',
+    'aquamarine2', 'aquamarine4', 'DarkSeaGreen1', 'DarkSeaGreen2', 'DarkSeaGreen3',
     'DarkSeaGreen4', 'SeaGreen1', 'SeaGreen2', 'SeaGreen3', 'PaleGreen1', 'PaleGreen2',
     'PaleGreen3', 'PaleGreen4', 'SpringGreen2', 'SpringGreen3', 'SpringGreen4',
     'green2', 'green3', 'green4', 'chartreuse2', 'chartreuse3', 'chartreuse4',
     'OliveDrab1', 'OliveDrab2', 'OliveDrab4', 'DarkOliveGreen1', 'DarkOliveGreen2',
     'DarkOliveGreen3', 'DarkOliveGreen4', 'khaki1', 'khaki2', 'khaki3', 'khaki4',
     'LightGoldenrod1', 'LightGoldenrod2', 'LightGoldenrod3', 'LightGoldenrod4',
-     'LightYellow4', 'yellow2', 'yellow3', 'yellow4',
+    'LightYellow2', 'LightYellow3', 'LightYellow4', 'yellow2', 'yellow3', 'yellow4',
     'gold2', 'gold3', 'gold4', 'goldenrod1', 'goldenrod2', 'goldenrod3', 'goldenrod4',
     'DarkGoldenrod1', 'DarkGoldenrod2', 'DarkGoldenrod3', 'DarkGoldenrod4',
-     'RosyBrown3', 'RosyBrown4', 'IndianRed1', 'IndianRed2',
-    'IndianRed3', 'IndianRed4', 'sienna1', 'sienna2', 'sienna3', 'sienna4',
-                                        'burlywood4', 'wheat4', 'tan1',
+    'RosyBrown1', 'RosyBrown2', 'RosyBrown3', 'RosyBrown4', 'IndianRed1', 'IndianRed2',
+    'IndianRed3', 'IndianRed4', 'sienna1', 'sienna2', 'sienna3', 'sienna4', 'burlywood1',
+    'burlywood2', 'burlywood3', 'burlywood4', 'wheat1', 'wheat2', 'wheat3', 'wheat4', 'tan1',
     'tan2', 'tan4', 'chocolate1', 'chocolate2', 'chocolate3', 'firebrick1', 'firebrick2',
     'firebrick3', 'firebrick4', 'brown1', 'brown2', 'brown3', 'brown4', 'salmon1', 'salmon2',
     'salmon3', 'salmon4', 'LightSalmon2', 'LightSalmon3', 'LightSalmon4', 'orange2',
     'orange3', 'orange4', 'DarkOrange1', 'DarkOrange2', 'DarkOrange3', 'DarkOrange4',
     'coral1', 'coral2', 'coral3', 'coral4', 'tomato2', 'tomato3', 'tomato4', 'OrangeRed2',
     'OrangeRed3', 'OrangeRed4', 'red2', 'red3', 'red4', 'DeepPink2', 'DeepPink3', 'DeepPink4',
-    'HotPink1', 'HotPink2', 'HotPink3', 'HotPink4', 'pink4',
-
+    'HotPink1', 'HotPink2', 'HotPink3', 'HotPink4', 'pink1', 'pink2', 'pink3', 'pink4',
+    'LightPink1', 'LightPink2', 'LightPink3', 'LightPink4', 'PaleVioletRed1',
     'PaleVioletRed2', 'PaleVioletRed3', 'PaleVioletRed4', 'maroon1', 'maroon2',
     'maroon3', 'maroon4', 'VioletRed1', 'VioletRed2', 'VioletRed3', 'VioletRed4',
-    'magenta2', 'magenta3', 'magenta4', 'orchid1', 'orchid2', 'orchid3', 'orchid4',
-                                        'MediumOrchid1', 'MediumOrchid2', 'MediumOrchid3',
+    'magenta2', 'magenta3', 'magenta4', 'orchid1', 'orchid2', 'orchid3', 'orchid4', 'plum1',
+    'plum2', 'plum3', 'plum4', 'MediumOrchid1', 'MediumOrchid2', 'MediumOrchid3',
     'MediumOrchid4', 'DarkOrchid1', 'DarkOrchid2', 'DarkOrchid3', 'DarkOrchid4',
     'purple1', 'purple2', 'purple3', 'purple4', 'MediumPurple1', 'MediumPurple2',
-    'MediumPurple3', 'MediumPurple4',])
+    'MediumPurple3', 'MediumPurple4', 'thistle1', 'thistle2', 'thistle3', 'thistle4'])
                                        }        
 
 Sentence_Type_Colors = {
     # gold standard colors
     'Uninformative': 'red',
     'Process Relevant':'blue',
     'Process Model Relevant': 'green',
```

### Comparing `PETAnnotationVisualizer-0.0.1a4/setup.py` & `petannotationvisualizer-1.2.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,53 +5,60 @@
     """
     Utility function to read the README file. Used for the long_description.
     :param fname:
     :return:
     """
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
-_REQUIRED = ['PETAnnotationDataset', 'Pillow', 'numpy']
+_REQUIRED = ['networkx','tqdm','petdatasetreader','matplotlib','mplcursors','pygraphviz']
 _EXTRAS = []
 
 setup(
-    name='PETAnnotationVisualizer',
-    version='0.0.1a4',
-    packages=find_packages(exclude=("tests","otherfiles")),
+    name='petannotationvisualizer',
+    version='1.2.0',
+    packages=find_packages(exclude=("tests", "docs", "dist", "build")),
     install_requires=_REQUIRED,
     # extras_require=_EXTRAS,
+    package_data={'': ['*.json', '*.png', ]},
     include_package_data=True,
     platforms="Any",
 
-    # python_requires='!=2.7, >=3.9.*',
+    # python_requires='!=2.7, >=3.5.*',
     classifiers=[
-            "Development Status :: 3 - Alpha",
+
             "License :: OSI Approved :: MIT License",
             "Natural Language :: English",
 
             "Intended Audience :: Science/Research",
             "Intended Audience :: Developers",
             "Intended Audience :: Education",
             "Intended Audience :: End Users/Desktop",
             "Intended Audience :: Information Technology",
 
             "Programming Language :: Python :: 3",
+            "Programming Language :: Python :: 3.5",
+            "Programming Language :: Python :: 3.6",
+            "Programming Language :: Python :: 3.7",
+            "Programming Language :: Python :: 3.8",
             "Programming Language :: Python :: 3.9",
             "Programming Language :: Python :: 3.10",
             "Programming Language :: Python :: 3.11",
             "Programming Language :: Python :: 3.12",
 
             "Topic :: Scientific/Engineering",
             "Topic :: Utilities",
         ],
+
     author='Patrizio Bellan',
     author_email='patrizio.bellan@gmail.com',
     maintainer="Patrizio Bellan",
     maintainer_email="patrizio.bellan@gmail.com",
 
-    url='http://www.example.com/it',
+    url='https://pdi.fbk.eu/pet-dataset',
 
     license='MIT',
-    keywords=["visualizer", "PET", "dataset"],
-    description="PET Annotators' Annotation PETAnnotationVisualizer",
-    long_description=read("README.rst"),
-    long_description_content_type='text/x-rst',
+    keywords=["PET visualizer", "huggingface", "PET", "dataset", "process extraction from text",
+              "natural language processing", "nlp", "business process management", "bpm"],
+    description='A visualization tool for the PET dataset hosted on Huggingface.',
+    long_description=read("README.md"),
+    long_description_content_type='text/markdown',
 )
```

