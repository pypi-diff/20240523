# Comparing `tmp/petannotationvisualizer-1.2.0.tar.gz` & `tmp/petannotationvisualizer-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "petannotationvisualizer-1.2.0.tar", last modified: Thu May 23 09:43:08 2024, max compression
+gzip compressed data, was "petannotationvisualizer-1.2.1.tar", last modified: Thu May 23 10:08:56 2024, max compression
```

## Comparing `petannotationvisualizer-1.2.0.tar` & `petannotationvisualizer-1.2.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 patrizio   (501) staff       (20)        0 2024-05-23 09:43:08.159063 petannotationvisualizer-1.2.0/
-drwxr-xr-x   0 patrizio   (501) staff       (20)        0 2024-05-23 09:43:08.157745 petannotationvisualizer-1.2.0/PETvisualizer/
--rw-r--r--   0 patrizio   (501) staff       (20)     8180 2024-05-23 08:26:51.000000 petannotationvisualizer-1.2.0/PETvisualizer/Colors.py
--rw-r--r--   0 patrizio   (501) staff       (20)      900 2024-05-23 08:26:51.000000 petannotationvisualizer-1.2.0/PETvisualizer/CreateProcessGraph.py
--rw-r--r--   0 patrizio   (501) staff       (20)    12161 2024-05-23 08:26:51.000000 petannotationvisualizer-1.2.0/PETvisualizer/Labels.py
--rw-r--r--   0 patrizio   (501) staff       (20)    75339 2024-05-23 08:26:51.000000 petannotationvisualizer-1.2.0/PETvisualizer/PETVisualizer.py
--rw-r--r--   0 patrizio   (501) staff       (20)    27436 2024-05-23 08:26:51.000000 petannotationvisualizer-1.2.0/PETvisualizer/ShowProcessGraph.py
--rw-r--r--   0 patrizio   (501) staff       (20)        0 2024-05-23 08:26:51.000000 petannotationvisualizer-1.2.0/PETvisualizer/__init__.py
--rw-r--r--   0 patrizio   (501) staff       (20)       55 2024-05-23 08:26:51.000000 petannotationvisualizer-1.2.0/PETvisualizer/main.py
--rw-r--r--   0 patrizio   (501) staff       (20)   195459 2024-05-23 08:26:51.000000 petannotationvisualizer-1.2.0/PETvisualizer/pet-entities.json
--rw-r--r--   0 patrizio   (501) staff       (20)   502158 2024-05-23 08:26:51.000000 petannotationvisualizer-1.2.0/PETvisualizer/pet-relations.json
--rw-r--r--   0 patrizio   (501) staff       (20)     8266 2024-05-23 08:26:51.000000 petannotationvisualizer-1.2.0/PETvisualizer/utility.py
--rw-r--r--   0 patrizio   (501) staff       (20)    12864 2024-05-23 08:26:51.000000 petannotationvisualizer-1.2.0/PETvisualizer/wolfgold.png
--rw-r--r--   0 patrizio   (501) staff       (20)    11180 2024-05-23 09:43:08.158853 petannotationvisualizer-1.2.0/PKG-INFO
--rw-r--r--   0 patrizio   (501) staff       (20)     9791 2024-05-23 09:39:10.000000 petannotationvisualizer-1.2.0/README.md
-drwxr-xr-x   0 patrizio   (501) staff       (20)        0 2024-05-23 09:43:08.158640 petannotationvisualizer-1.2.0/petannotationvisualizer.egg-info/
--rw-r--r--   0 patrizio   (501) staff       (20)    11180 2024-05-23 09:43:08.000000 petannotationvisualizer-1.2.0/petannotationvisualizer.egg-info/PKG-INFO
--rw-r--r--   0 patrizio   (501) staff       (20)      566 2024-05-23 09:43:08.000000 petannotationvisualizer-1.2.0/petannotationvisualizer.egg-info/SOURCES.txt
--rw-r--r--   0 patrizio   (501) staff       (20)        1 2024-05-23 09:43:08.000000 petannotationvisualizer-1.2.0/petannotationvisualizer.egg-info/dependency_links.txt
--rw-r--r--   0 patrizio   (501) staff       (20)       64 2024-05-23 09:43:08.000000 petannotationvisualizer-1.2.0/petannotationvisualizer.egg-info/requires.txt
--rw-r--r--   0 patrizio   (501) staff       (20)       14 2024-05-23 09:43:08.000000 petannotationvisualizer-1.2.0/petannotationvisualizer.egg-info/top_level.txt
--rw-r--r--   0 patrizio   (501) staff       (20)       38 2024-05-23 09:43:08.159116 petannotationvisualizer-1.2.0/setup.cfg
--rw-r--r--   0 patrizio   (501) staff       (20)     2245 2024-05-23 09:43:02.000000 petannotationvisualizer-1.2.0/setup.py
+drwxr-xr-x   0 patrizio   (501) staff       (20)        0 2024-05-23 10:08:56.610881 petannotationvisualizer-1.2.1/
+drwxr-xr-x   0 patrizio   (501) staff       (20)        0 2024-05-23 10:08:56.609402 petannotationvisualizer-1.2.1/PETvisualizer/
+-rw-r--r--   0 patrizio   (501) staff       (20)     8180 2024-05-23 08:26:51.000000 petannotationvisualizer-1.2.1/PETvisualizer/Colors.py
+-rw-r--r--   0 patrizio   (501) staff       (20)      900 2024-05-23 08:26:51.000000 petannotationvisualizer-1.2.1/PETvisualizer/CreateProcessGraph.py
+-rw-r--r--   0 patrizio   (501) staff       (20)    12161 2024-05-23 08:26:51.000000 petannotationvisualizer-1.2.1/PETvisualizer/Labels.py
+-rw-r--r--   0 patrizio   (501) staff       (20)    75339 2024-05-23 08:26:51.000000 petannotationvisualizer-1.2.1/PETvisualizer/PETVisualizer.py
+-rw-r--r--   0 patrizio   (501) staff       (20)    27436 2024-05-23 08:26:51.000000 petannotationvisualizer-1.2.1/PETvisualizer/ShowProcessGraph.py
+-rw-r--r--   0 patrizio   (501) staff       (20)        0 2024-05-23 08:26:51.000000 petannotationvisualizer-1.2.1/PETvisualizer/__init__.py
+-rw-r--r--   0 patrizio   (501) staff       (20)       55 2024-05-23 08:26:51.000000 petannotationvisualizer-1.2.1/PETvisualizer/main.py
+-rw-r--r--   0 patrizio   (501) staff       (20)   195459 2024-05-23 08:26:51.000000 petannotationvisualizer-1.2.1/PETvisualizer/pet-entities.json
+-rw-r--r--   0 patrizio   (501) staff       (20)   502158 2024-05-23 08:26:51.000000 petannotationvisualizer-1.2.1/PETvisualizer/pet-relations.json
+-rw-r--r--   0 patrizio   (501) staff       (20)     8266 2024-05-23 08:26:51.000000 petannotationvisualizer-1.2.1/PETvisualizer/utility.py
+-rw-r--r--   0 patrizio   (501) staff       (20)    12864 2024-05-23 08:26:51.000000 petannotationvisualizer-1.2.1/PETvisualizer/wolfgold.png
+-rw-r--r--   0 patrizio   (501) staff       (20)    11168 2024-05-23 10:08:56.610674 petannotationvisualizer-1.2.1/PKG-INFO
+-rw-r--r--   0 patrizio   (501) staff       (20)     9779 2024-05-23 10:08:56.000000 petannotationvisualizer-1.2.1/README.md
+drwxr-xr-x   0 patrizio   (501) staff       (20)        0 2024-05-23 10:08:56.610436 petannotationvisualizer-1.2.1/petannotationvisualizer.egg-info/
+-rw-r--r--   0 patrizio   (501) staff       (20)    11168 2024-05-23 10:08:56.000000 petannotationvisualizer-1.2.1/petannotationvisualizer.egg-info/PKG-INFO
+-rw-r--r--   0 patrizio   (501) staff       (20)      566 2024-05-23 10:08:56.000000 petannotationvisualizer-1.2.1/petannotationvisualizer.egg-info/SOURCES.txt
+-rw-r--r--   0 patrizio   (501) staff       (20)        1 2024-05-23 10:08:56.000000 petannotationvisualizer-1.2.1/petannotationvisualizer.egg-info/dependency_links.txt
+-rw-r--r--   0 patrizio   (501) staff       (20)       64 2024-05-23 10:08:56.000000 petannotationvisualizer-1.2.1/petannotationvisualizer.egg-info/requires.txt
+-rw-r--r--   0 patrizio   (501) staff       (20)       14 2024-05-23 10:08:56.000000 petannotationvisualizer-1.2.1/petannotationvisualizer.egg-info/top_level.txt
+-rw-r--r--   0 patrizio   (501) staff       (20)       38 2024-05-23 10:08:56.610932 petannotationvisualizer-1.2.1/setup.cfg
+-rw-r--r--   0 patrizio   (501) staff       (20)     2245 2024-05-23 09:47:16.000000 petannotationvisualizer-1.2.1/setup.py
```

### Comparing `petannotationvisualizer-1.2.0/PETvisualizer/Colors.py` & `petannotationvisualizer-1.2.1/PETvisualizer/Colors.py`

 * *Files identical despite different names*

### Comparing `petannotationvisualizer-1.2.0/PETvisualizer/CreateProcessGraph.py` & `petannotationvisualizer-1.2.1/PETvisualizer/CreateProcessGraph.py`

 * *Files identical despite different names*

### Comparing `petannotationvisualizer-1.2.0/PETvisualizer/Labels.py` & `petannotationvisualizer-1.2.1/PETvisualizer/Labels.py`

 * *Files identical despite different names*

### Comparing `petannotationvisualizer-1.2.0/PETvisualizer/PETVisualizer.py` & `petannotationvisualizer-1.2.1/PETvisualizer/PETVisualizer.py`

 * *Files identical despite different names*

### Comparing `petannotationvisualizer-1.2.0/PETvisualizer/ShowProcessGraph.py` & `petannotationvisualizer-1.2.1/PETvisualizer/ShowProcessGraph.py`

 * *Files identical despite different names*

### Comparing `petannotationvisualizer-1.2.0/PETvisualizer/pet-entities.json` & `petannotationvisualizer-1.2.1/PETvisualizer/pet-entities.json`

 * *Files identical despite different names*

### Comparing `petannotationvisualizer-1.2.0/PETvisualizer/pet-relations.json` & `petannotationvisualizer-1.2.1/PETvisualizer/pet-relations.json`

 * *Files identical despite different names*

### Comparing `petannotationvisualizer-1.2.0/PETvisualizer/utility.py` & `petannotationvisualizer-1.2.1/PETvisualizer/utility.py`

 * *Files identical despite different names*

### Comparing `petannotationvisualizer-1.2.0/PETvisualizer/wolfgold.png` & `petannotationvisualizer-1.2.1/PETvisualizer/wolfgold.png`

 * *Files identical despite different names*

### Comparing `petannotationvisualizer-1.2.0/PKG-INFO` & `petannotationvisualizer-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: petannotationvisualizer
-Version: 1.2.0
+Version: 1.2.1
 Summary: A visualization tool for the PET dataset hosted on Huggingface.
 Home-page: https://pdi.fbk.eu/pet-dataset
 Author: Patrizio Bellan
 Author-email: patrizio.bellan@gmail.com
 Maintainer: Patrizio Bellan
 Maintainer-email: patrizio.bellan@gmail.com
 License: MIT
@@ -52,15 +52,15 @@
 ========
 The extraction of process models from natural language text is an essential task for process discovery. Several approaches have been developed in recent years to address this task. Still, one of the main limitations is the impossibility of visualizing the extracted process model and comparing it with gold standard data to assess similarity. 
 In this paper, we present PET Visualizer, a visualization tool developed to graphically represent the process models of the document annotated in the PET dataset, the unique gold-standard dataset developed for process information extraction tasks.
 The main goal of PET Visualizer is to provide a way to visualize the dataset, making it easier to analyze and understand the process models. 
 The tool supports several visualization options and can be easily integrated into existing workflows or extend the function implemented. During the system presentation, we demonstrate the effectiveness of the tool and its potential impact in improving process extraction from text tas
 
 ---
-![PET Visualizers GUI](PETvisualizer/figures/PETVisualizerscreenshot1.jpg)
+![PET Visualizers GUI](figures/PETVisualizerscreenshot1.jpg)
 *Fig.1 A screenshot of the PET Visualizer GUI.*
 
 We present PET Visualizer, a tool developed to graphically visualize process model document annotations and the representation of the process model in the form of labeled graphs. For this first version of the tool, we concentrate on providing a graphical representation of the annotations of the [PET dataset](https://huggingface.co/datasets/patriziobellan/PET), the unique gold-standard dataset freely available specifically for process information extraction tasks.  The PET dataset is a corpus of human-annotated process model descriptions. It consists of a collection of 45 descriptions annotated with process model elements and relations at the textual level. 
 
 The GUI, shown in *Fig.1*, is composed of three main parts: ***Command Bar***, ***Annotation Menu***, and ***Text Area***.
 
 On the top left side of the GUI, there is the *Command Bar*.
@@ -70,26 +70,26 @@
 - Export Data* Exports the dataset in a JSON format after manipulation.
 - Export for HuggingFace* Exports the manipulated dataset in the same format and following the original schema of the PET dataset on HuggingFace. This important feature allows the extension of the PET dataset with new data while keeping compatibility with other PET-related tools (e.g., [PET Dataset Reader](https://pypi.org/project/petdatasetreader/)).
 - Show Process Graph* Shows the process model graph of the annotations of a document. When you choose to visualize the process graph of a document, a new window displays the graph representation where the nodes represent the entities and the edges represent the relations.
 		At the top of this window, we implemented the two accessibility controls to increase the size of nodes and edges and the font size of the text.
 		At the bottom side, there are the common *matplotlib* commands to navigate and export the graph image.
 		An example of graph visualization is shown in *Fig.2*.
 - *Load Json Data* Loads a local dataset. The local dataset is split into two JSON files: an *entities* annotation file and a *relations* annotation file. This command is straightforward but makes the dataset loading operation faster than loading from the HuggingFace repository every time.
-![PET Visualizers GUI - process graph](PETvisualizer/figures/PETVisualizerscreenshootgraph.jpg)
+![PET Visualizers GUI - process graph](figures/PETVisualizerscreenshootgraph.jpg)
 *Fig.2 A screenshot of the PET Visualizer - Process Graph visualization.*
 
 Finally, in the last part of the command bar, we implemented two scroll controls that allow users to set the size of the annotation lines and the font size of the text. These two controls would increase *accessibility* of our tool.
 
 On the right-hand side of the GUI, the *Annotation Menu* allows users to create, delete, or edit annotations. The menu is divided into two cards, one for process model elements (as shown in Figure \ref{fig:menuentities*) and the other for process model element relations (as shown in Figure \ref{fig:menurelations*). Each schedule consists of a list box that displays all the annotations (either elements or relations) of the document. When an item is selected in the list box, the corresponding annotation is highlighted in the *Text Area*.
 
 
  
 *Entities Menu*
 ---
-![PET Visualizers GUI - Entities Menu](PETvisualizer/figures/PETVisualizermenuentities.jpg)
+![PET Visualizers GUI - Entities Menu](figures/PETVisualizermenuentities.jpg)
 *Fig.3 Entities menu.*
 
 The Entities Menu card, shown in *Fig.3*, lists all the process model element annotations of the selected document.
 This menu consists of a list box containing all the process model annotations for a document. Each item represents a single annotation. The list box reports the annotation ID, the type of process model element annotated (such as *PET activity*), and the words annotated (e.g., *a company*) for each annotation.
 Below the list box, a process element type combo box reports the type of process model element, while the *n sent* text field shows the index of the sentence of the words annotated. The *Begin* and *End* text fields represent the index of the first and last words of the span of words that the annotation covers\footnote{It is essential to note that all the indexes (sentence, begin, end) start from 0.*.
 When an entity is selected, its information fills these text fields.
 When creating a new annotation, these fields must be filled with the annotation data.
@@ -98,15 +98,15 @@
 - *Show temp Annotation* This command displays the annotation being edited.
 - *Add Annotation* This command adds a newly created annotation to the document.
 - *Delete Annotation*This command deletes the selected annotation.
 
 
 *Relations Menu*
 ---
-![PET Visualizers GUI - Relations Menu](PETvisualizer/figures/PETVisualizermenurelations.jpg)
+![PET Visualizers GUI - Relations Menu](figures/PETVisualizermenurelations.jpg)
 *Fig.4 Relations menu.*
  
 
 The Relations Menu card, shown in *Fig.4*, contains all the process model relation annotations of a document. This menu comprises a list box where each item represents a single annotation and includes the annotation ID, the type of relation annotated (e.g., *PET uses relation*), and the source and target elements of the relation.
 
 Below the list of relations, three combo boxes report the source, the relation type, and the target element.
 When a relation is selected, the relation data fills the combo boxes.
@@ -120,15 +120,15 @@
 At the bottom part of the card, there are three annotation commands:
 - *Create New Annotation* This command starts the creation of a new annotation.	
 - *Add Annotation* This command adds a newly created annotation to the document.
 - *Delete Annotation* This command deletes the selected annotation.
 
 ***Text Area*** part lies in the central part of the GUI. It shows the text of a document and its annotations. PET elements are highlighted in boxes, while PET relations connect PET elements using labeled arrows. Boxes and relation arrows follow the color schema reported in *Fig.5*.
 
-![Color Schema](PETvisualizer/figures/colorschema.jpg)
+![Color Schema](https://github.com/patriziobellan86/PETvisualizer/blob/master/img/colorschema.jpg)
 *Fig.5 Relations menu.*
 
 
 Dependencies installation notes
 ===============================
 If the installation of requirements fails, you need to downgrade the setuptool and wheel packages.
 run the following command in a terminal:
```

### Comparing `petannotationvisualizer-1.2.0/README.md` & `petannotationvisualizer-1.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 ========
 The extraction of process models from natural language text is an essential task for process discovery. Several approaches have been developed in recent years to address this task. Still, one of the main limitations is the impossibility of visualizing the extracted process model and comparing it with gold standard data to assess similarity. 
 In this paper, we present PET Visualizer, a visualization tool developed to graphically represent the process models of the document annotated in the PET dataset, the unique gold-standard dataset developed for process information extraction tasks.
 The main goal of PET Visualizer is to provide a way to visualize the dataset, making it easier to analyze and understand the process models. 
 The tool supports several visualization options and can be easily integrated into existing workflows or extend the function implemented. During the system presentation, we demonstrate the effectiveness of the tool and its potential impact in improving process extraction from text tas
 
 ---
-![PET Visualizers GUI](PETvisualizer/figures/PETVisualizerscreenshot1.jpg)
+![PET Visualizers GUI](figures/PETVisualizerscreenshot1.jpg)
 *Fig.1 A screenshot of the PET Visualizer GUI.*
 
 We present PET Visualizer, a tool developed to graphically visualize process model document annotations and the representation of the process model in the form of labeled graphs. For this first version of the tool, we concentrate on providing a graphical representation of the annotations of the [PET dataset](https://huggingface.co/datasets/patriziobellan/PET), the unique gold-standard dataset freely available specifically for process information extraction tasks.  The PET dataset is a corpus of human-annotated process model descriptions. It consists of a collection of 45 descriptions annotated with process model elements and relations at the textual level. 
 
 The GUI, shown in *Fig.1*, is composed of three main parts: ***Command Bar***, ***Annotation Menu***, and ***Text Area***.
 
 On the top left side of the GUI, there is the *Command Bar*.
@@ -38,26 +38,26 @@
 - Export Data* Exports the dataset in a JSON format after manipulation.
 - Export for HuggingFace* Exports the manipulated dataset in the same format and following the original schema of the PET dataset on HuggingFace. This important feature allows the extension of the PET dataset with new data while keeping compatibility with other PET-related tools (e.g., [PET Dataset Reader](https://pypi.org/project/petdatasetreader/)).
 - Show Process Graph* Shows the process model graph of the annotations of a document. When you choose to visualize the process graph of a document, a new window displays the graph representation where the nodes represent the entities and the edges represent the relations.
 		At the top of this window, we implemented the two accessibility controls to increase the size of nodes and edges and the font size of the text.
 		At the bottom side, there are the common *matplotlib* commands to navigate and export the graph image.
 		An example of graph visualization is shown in *Fig.2*.
 - *Load Json Data* Loads a local dataset. The local dataset is split into two JSON files: an *entities* annotation file and a *relations* annotation file. This command is straightforward but makes the dataset loading operation faster than loading from the HuggingFace repository every time.
-![PET Visualizers GUI - process graph](PETvisualizer/figures/PETVisualizerscreenshootgraph.jpg)
+![PET Visualizers GUI - process graph](figures/PETVisualizerscreenshootgraph.jpg)
 *Fig.2 A screenshot of the PET Visualizer - Process Graph visualization.*
 
 Finally, in the last part of the command bar, we implemented two scroll controls that allow users to set the size of the annotation lines and the font size of the text. These two controls would increase *accessibility* of our tool.
 
 On the right-hand side of the GUI, the *Annotation Menu* allows users to create, delete, or edit annotations. The menu is divided into two cards, one for process model elements (as shown in Figure \ref{fig:menuentities*) and the other for process model element relations (as shown in Figure \ref{fig:menurelations*). Each schedule consists of a list box that displays all the annotations (either elements or relations) of the document. When an item is selected in the list box, the corresponding annotation is highlighted in the *Text Area*.
 
 
  
 *Entities Menu*
 ---
-![PET Visualizers GUI - Entities Menu](PETvisualizer/figures/PETVisualizermenuentities.jpg)
+![PET Visualizers GUI - Entities Menu](figures/PETVisualizermenuentities.jpg)
 *Fig.3 Entities menu.*
 
 The Entities Menu card, shown in *Fig.3*, lists all the process model element annotations of the selected document.
 This menu consists of a list box containing all the process model annotations for a document. Each item represents a single annotation. The list box reports the annotation ID, the type of process model element annotated (such as *PET activity*), and the words annotated (e.g., *a company*) for each annotation.
 Below the list box, a process element type combo box reports the type of process model element, while the *n sent* text field shows the index of the sentence of the words annotated. The *Begin* and *End* text fields represent the index of the first and last words of the span of words that the annotation covers\footnote{It is essential to note that all the indexes (sentence, begin, end) start from 0.*.
 When an entity is selected, its information fills these text fields.
 When creating a new annotation, these fields must be filled with the annotation data.
@@ -66,15 +66,15 @@
 - *Show temp Annotation* This command displays the annotation being edited.
 - *Add Annotation* This command adds a newly created annotation to the document.
 - *Delete Annotation*This command deletes the selected annotation.
 
 
 *Relations Menu*
 ---
-![PET Visualizers GUI - Relations Menu](PETvisualizer/figures/PETVisualizermenurelations.jpg)
+![PET Visualizers GUI - Relations Menu](figures/PETVisualizermenurelations.jpg)
 *Fig.4 Relations menu.*
  
 
 The Relations Menu card, shown in *Fig.4*, contains all the process model relation annotations of a document. This menu comprises a list box where each item represents a single annotation and includes the annotation ID, the type of relation annotated (e.g., *PET uses relation*), and the source and target elements of the relation.
 
 Below the list of relations, three combo boxes report the source, the relation type, and the target element.
 When a relation is selected, the relation data fills the combo boxes.
@@ -88,15 +88,15 @@
 At the bottom part of the card, there are three annotation commands:
 - *Create New Annotation* This command starts the creation of a new annotation.	
 - *Add Annotation* This command adds a newly created annotation to the document.
 - *Delete Annotation* This command deletes the selected annotation.
 
 ***Text Area*** part lies in the central part of the GUI. It shows the text of a document and its annotations. PET elements are highlighted in boxes, while PET relations connect PET elements using labeled arrows. Boxes and relation arrows follow the color schema reported in *Fig.5*.
 
-![Color Schema](PETvisualizer/figures/colorschema.jpg)
+![Color Schema](https://github.com/patriziobellan86/PETvisualizer/blob/master/img/colorschema.jpg)
 *Fig.5 Relations menu.*
 
 
 Dependencies installation notes
 ===============================
 If the installation of requirements fails, you need to downgrade the setuptool and wheel packages.
 run the following command in a terminal:
```

### Comparing `petannotationvisualizer-1.2.0/petannotationvisualizer.egg-info/PKG-INFO` & `petannotationvisualizer-1.2.1/petannotationvisualizer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: petannotationvisualizer
-Version: 1.2.0
+Version: 1.2.1
 Summary: A visualization tool for the PET dataset hosted on Huggingface.
 Home-page: https://pdi.fbk.eu/pet-dataset
 Author: Patrizio Bellan
 Author-email: patrizio.bellan@gmail.com
 Maintainer: Patrizio Bellan
 Maintainer-email: patrizio.bellan@gmail.com
 License: MIT
@@ -52,15 +52,15 @@
 ========
 The extraction of process models from natural language text is an essential task for process discovery. Several approaches have been developed in recent years to address this task. Still, one of the main limitations is the impossibility of visualizing the extracted process model and comparing it with gold standard data to assess similarity. 
 In this paper, we present PET Visualizer, a visualization tool developed to graphically represent the process models of the document annotated in the PET dataset, the unique gold-standard dataset developed for process information extraction tasks.
 The main goal of PET Visualizer is to provide a way to visualize the dataset, making it easier to analyze and understand the process models. 
 The tool supports several visualization options and can be easily integrated into existing workflows or extend the function implemented. During the system presentation, we demonstrate the effectiveness of the tool and its potential impact in improving process extraction from text tas
 
 ---
-![PET Visualizers GUI](PETvisualizer/figures/PETVisualizerscreenshot1.jpg)
+![PET Visualizers GUI](figures/PETVisualizerscreenshot1.jpg)
 *Fig.1 A screenshot of the PET Visualizer GUI.*
 
 We present PET Visualizer, a tool developed to graphically visualize process model document annotations and the representation of the process model in the form of labeled graphs. For this first version of the tool, we concentrate on providing a graphical representation of the annotations of the [PET dataset](https://huggingface.co/datasets/patriziobellan/PET), the unique gold-standard dataset freely available specifically for process information extraction tasks.  The PET dataset is a corpus of human-annotated process model descriptions. It consists of a collection of 45 descriptions annotated with process model elements and relations at the textual level. 
 
 The GUI, shown in *Fig.1*, is composed of three main parts: ***Command Bar***, ***Annotation Menu***, and ***Text Area***.
 
 On the top left side of the GUI, there is the *Command Bar*.
@@ -70,26 +70,26 @@
 - Export Data* Exports the dataset in a JSON format after manipulation.
 - Export for HuggingFace* Exports the manipulated dataset in the same format and following the original schema of the PET dataset on HuggingFace. This important feature allows the extension of the PET dataset with new data while keeping compatibility with other PET-related tools (e.g., [PET Dataset Reader](https://pypi.org/project/petdatasetreader/)).
 - Show Process Graph* Shows the process model graph of the annotations of a document. When you choose to visualize the process graph of a document, a new window displays the graph representation where the nodes represent the entities and the edges represent the relations.
 		At the top of this window, we implemented the two accessibility controls to increase the size of nodes and edges and the font size of the text.
 		At the bottom side, there are the common *matplotlib* commands to navigate and export the graph image.
 		An example of graph visualization is shown in *Fig.2*.
 - *Load Json Data* Loads a local dataset. The local dataset is split into two JSON files: an *entities* annotation file and a *relations* annotation file. This command is straightforward but makes the dataset loading operation faster than loading from the HuggingFace repository every time.
-![PET Visualizers GUI - process graph](PETvisualizer/figures/PETVisualizerscreenshootgraph.jpg)
+![PET Visualizers GUI - process graph](figures/PETVisualizerscreenshootgraph.jpg)
 *Fig.2 A screenshot of the PET Visualizer - Process Graph visualization.*
 
 Finally, in the last part of the command bar, we implemented two scroll controls that allow users to set the size of the annotation lines and the font size of the text. These two controls would increase *accessibility* of our tool.
 
 On the right-hand side of the GUI, the *Annotation Menu* allows users to create, delete, or edit annotations. The menu is divided into two cards, one for process model elements (as shown in Figure \ref{fig:menuentities*) and the other for process model element relations (as shown in Figure \ref{fig:menurelations*). Each schedule consists of a list box that displays all the annotations (either elements or relations) of the document. When an item is selected in the list box, the corresponding annotation is highlighted in the *Text Area*.
 
 
  
 *Entities Menu*
 ---
-![PET Visualizers GUI - Entities Menu](PETvisualizer/figures/PETVisualizermenuentities.jpg)
+![PET Visualizers GUI - Entities Menu](figures/PETVisualizermenuentities.jpg)
 *Fig.3 Entities menu.*
 
 The Entities Menu card, shown in *Fig.3*, lists all the process model element annotations of the selected document.
 This menu consists of a list box containing all the process model annotations for a document. Each item represents a single annotation. The list box reports the annotation ID, the type of process model element annotated (such as *PET activity*), and the words annotated (e.g., *a company*) for each annotation.
 Below the list box, a process element type combo box reports the type of process model element, while the *n sent* text field shows the index of the sentence of the words annotated. The *Begin* and *End* text fields represent the index of the first and last words of the span of words that the annotation covers\footnote{It is essential to note that all the indexes (sentence, begin, end) start from 0.*.
 When an entity is selected, its information fills these text fields.
 When creating a new annotation, these fields must be filled with the annotation data.
@@ -98,15 +98,15 @@
 - *Show temp Annotation* This command displays the annotation being edited.
 - *Add Annotation* This command adds a newly created annotation to the document.
 - *Delete Annotation*This command deletes the selected annotation.
 
 
 *Relations Menu*
 ---
-![PET Visualizers GUI - Relations Menu](PETvisualizer/figures/PETVisualizermenurelations.jpg)
+![PET Visualizers GUI - Relations Menu](figures/PETVisualizermenurelations.jpg)
 *Fig.4 Relations menu.*
  
 
 The Relations Menu card, shown in *Fig.4*, contains all the process model relation annotations of a document. This menu comprises a list box where each item represents a single annotation and includes the annotation ID, the type of relation annotated (e.g., *PET uses relation*), and the source and target elements of the relation.
 
 Below the list of relations, three combo boxes report the source, the relation type, and the target element.
 When a relation is selected, the relation data fills the combo boxes.
@@ -120,15 +120,15 @@
 At the bottom part of the card, there are three annotation commands:
 - *Create New Annotation* This command starts the creation of a new annotation.	
 - *Add Annotation* This command adds a newly created annotation to the document.
 - *Delete Annotation* This command deletes the selected annotation.
 
 ***Text Area*** part lies in the central part of the GUI. It shows the text of a document and its annotations. PET elements are highlighted in boxes, while PET relations connect PET elements using labeled arrows. Boxes and relation arrows follow the color schema reported in *Fig.5*.
 
-![Color Schema](PETvisualizer/figures/colorschema.jpg)
+![Color Schema](https://github.com/patriziobellan86/PETvisualizer/blob/master/img/colorschema.jpg)
 *Fig.5 Relations menu.*
 
 
 Dependencies installation notes
 ===============================
 If the installation of requirements fails, you need to downgrade the setuptool and wheel packages.
 run the following command in a terminal:
```

### Comparing `petannotationvisualizer-1.2.0/petannotationvisualizer.egg-info/SOURCES.txt` & `petannotationvisualizer-1.2.1/petannotationvisualizer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `petannotationvisualizer-1.2.0/setup.py` & `petannotationvisualizer-1.2.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 _REQUIRED = ['networkx','tqdm','petdatasetreader','matplotlib','mplcursors','pygraphviz']
 _EXTRAS = []
 
 setup(
     name='petannotationvisualizer',
-    version='1.2.0',
+    version='1.2.1',
     packages=find_packages(exclude=("tests", "docs", "dist", "build")),
     install_requires=_REQUIRED,
     # extras_require=_EXTRAS,
     package_data={'': ['*.json', '*.png', ]},
     include_package_data=True,
     platforms="Any",
```

