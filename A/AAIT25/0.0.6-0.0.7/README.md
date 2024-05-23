# Comparing `tmp/AAIT25-0.0.6.tar.gz` & `tmp/AAIT25-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AAIT25-0.0.6.tar", last modified: Thu May 23 18:04:49 2024, max compression
+gzip compressed data, was "AAIT25-0.0.7.tar", last modified: Thu May 23 18:09:06 2024, max compression
```

## Comparing `AAIT25-0.0.6.tar` & `AAIT25-0.0.7.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 18:04:49.294690 AAIT25-0.0.6/
-drwxrwxrwx   0        0        0        0 2024-05-23 18:04:49.287172 AAIT25-0.0.6/AAIT25.egg-info/
--rw-rw-rw-   0        0        0      236 2024-05-23 18:04:49.000000 AAIT25-0.0.6/AAIT25.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      818 2024-05-23 18:04:49.000000 AAIT25-0.0.6/AAIT25.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 18:04:49.000000 AAIT25-0.0.6/AAIT25.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2024-05-23 18:04:49.000000 AAIT25-0.0.6/AAIT25.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       14 2024-05-23 18:04:49.000000 AAIT25-0.0.6/AAIT25.egg-info/namespace_packages.txt
--rw-rw-rw-   0        0        0       29 2024-05-23 18:04:49.000000 AAIT25-0.0.6/AAIT25.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-23 18:04:49.000000 AAIT25-0.0.6/AAIT25.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2024-01-18 15:57:45.000000 AAIT25-0.0.6/License.txt
--rw-rw-rw-   0        0        0      236 2024-05-23 18:04:49.293691 AAIT25-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-01-18 15:57:45.000000 AAIT25-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-23 18:04:49.287172 AAIT25-0.0.6/orangecontrib/
-drwxrwxrwx   0        0        0        0 2024-05-23 18:04:49.288685 AAIT25-0.0.6/orangecontrib/AAIT/
--rw-rw-rw-   0        0        0        0 2024-01-18 15:57:45.000000 AAIT25-0.0.6/orangecontrib/AAIT/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 18:04:49.288685 AAIT25-0.0.6/orangecontrib/AAIT/examples/
--rw-rw-rw-   0        0        0     7856 2024-02-20 12:43:50.000000 AAIT25-0.0.6/orangecontrib/AAIT/examples/example-chatbot.ows
--rw-rw-rw-   0        0        0      966 2024-03-06 08:40:04.000000 AAIT25-0.0.6/orangecontrib/AAIT/execute_thread.py
-drwxrwxrwx   0        0        0        0 2024-05-23 18:04:49.289691 AAIT25-0.0.6/orangecontrib/AAIT/widgets/
--rw-rw-rw-   0        0        0        0 2024-01-18 15:57:45.000000 AAIT25-0.0.6/orangecontrib/AAIT/widgets/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 18:04:49.290691 AAIT25-0.0.6/orangecontrib/AAIT/widgets/designer/
--rw-rw-rw-   0        0        0     2337 2024-03-04 19:45:00.000000 AAIT25-0.0.6/orangecontrib/AAIT/widgets/designer/owchatbot.ui
-drwxrwxrwx   0        0        0        0 2024-05-23 18:04:49.293691 AAIT25-0.0.6/orangecontrib/AAIT/widgets/icons/
--rw-rw-rw-   0        0        0      831 2024-01-18 15:57:45.000000 AAIT25-0.0.6/orangecontrib/AAIT/widgets/icons/Chatbotpy.svg
--rw-rw-rw-   0        0        0     1596 2024-01-18 15:57:45.000000 AAIT25-0.0.6/orangecontrib/AAIT/widgets/icons/DocumentEater.svg
--rw-rw-rw-   0        0        0     4195 2024-01-18 15:57:45.000000 AAIT25-0.0.6/orangecontrib/AAIT/widgets/icons/Embeddings.svg
--rw-rw-rw-   0        0        0     1357 2024-01-18 15:57:45.000000 AAIT25-0.0.6/orangecontrib/AAIT/widgets/icons/LanguageModel.svg
--rw-rw-rw-   0        0        0      500 2024-01-18 15:57:45.000000 AAIT25-0.0.6/orangecontrib/AAIT/widgets/icons/TextPreprocessing.svg
--rw-rw-rw-   0        0        0     1082 2024-02-19 21:08:44.000000 AAIT25-0.0.6/orangecontrib/AAIT/widgets/icons/chatbot.svg
--rw-rw-rw-   0        0        0     8197 2024-05-23 18:03:12.000000 AAIT25-0.0.6/orangecontrib/AAIT/widgets/owchatbot.py
--rw-rw-rw-   0        0        0       55 2024-01-18 15:57:45.000000 AAIT25-0.0.6/orangecontrib/__init__.py
--rw-rw-rw-   0        0        0       42 2024-05-23 18:04:49.294690 AAIT25-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1793 2024-05-23 18:04:24.000000 AAIT25-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 18:09:06.631350 AAIT25-0.0.7/
+drwxrwxrwx   0        0        0        0 2024-05-23 18:09:06.623829 AAIT25-0.0.7/AAIT25.egg-info/
+-rw-rw-rw-   0        0        0      236 2024-05-23 18:09:06.000000 AAIT25-0.0.7/AAIT25.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      818 2024-05-23 18:09:06.000000 AAIT25-0.0.7/AAIT25.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 18:09:06.000000 AAIT25-0.0.7/AAIT25.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2024-05-23 18:09:06.000000 AAIT25-0.0.7/AAIT25.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       14 2024-05-23 18:09:06.000000 AAIT25-0.0.7/AAIT25.egg-info/namespace_packages.txt
+-rw-rw-rw-   0        0        0       29 2024-05-23 18:09:06.000000 AAIT25-0.0.7/AAIT25.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-23 18:09:06.000000 AAIT25-0.0.7/AAIT25.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2024-01-18 15:57:45.000000 AAIT25-0.0.7/License.txt
+-rw-rw-rw-   0        0        0      236 2024-05-23 18:09:06.630356 AAIT25-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-01-18 15:57:45.000000 AAIT25-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-23 18:09:06.623829 AAIT25-0.0.7/orangecontrib/
+drwxrwxrwx   0        0        0        0 2024-05-23 18:09:06.624827 AAIT25-0.0.7/orangecontrib/AAIT/
+-rw-rw-rw-   0        0        0        0 2024-01-18 15:57:45.000000 AAIT25-0.0.7/orangecontrib/AAIT/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 18:09:06.624827 AAIT25-0.0.7/orangecontrib/AAIT/examples/
+-rw-rw-rw-   0        0        0     7856 2024-02-20 12:43:50.000000 AAIT25-0.0.7/orangecontrib/AAIT/examples/example-chatbot.ows
+-rw-rw-rw-   0        0        0      966 2024-03-06 08:40:04.000000 AAIT25-0.0.7/orangecontrib/AAIT/execute_thread.py
+drwxrwxrwx   0        0        0        0 2024-05-23 18:09:06.625822 AAIT25-0.0.7/orangecontrib/AAIT/widgets/
+-rw-rw-rw-   0        0        0        0 2024-01-18 15:57:45.000000 AAIT25-0.0.7/orangecontrib/AAIT/widgets/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 18:09:06.625822 AAIT25-0.0.7/orangecontrib/AAIT/widgets/designer/
+-rw-rw-rw-   0        0        0     2337 2024-03-04 19:45:00.000000 AAIT25-0.0.7/orangecontrib/AAIT/widgets/designer/owchatbot.ui
+drwxrwxrwx   0        0        0        0 2024-05-23 18:09:06.630356 AAIT25-0.0.7/orangecontrib/AAIT/widgets/icons/
+-rw-rw-rw-   0        0        0      831 2024-01-18 15:57:45.000000 AAIT25-0.0.7/orangecontrib/AAIT/widgets/icons/Chatbotpy.svg
+-rw-rw-rw-   0        0        0     1596 2024-01-18 15:57:45.000000 AAIT25-0.0.7/orangecontrib/AAIT/widgets/icons/DocumentEater.svg
+-rw-rw-rw-   0        0        0     4195 2024-01-18 15:57:45.000000 AAIT25-0.0.7/orangecontrib/AAIT/widgets/icons/Embeddings.svg
+-rw-rw-rw-   0        0        0     1357 2024-01-18 15:57:45.000000 AAIT25-0.0.7/orangecontrib/AAIT/widgets/icons/LanguageModel.svg
+-rw-rw-rw-   0        0        0      500 2024-01-18 15:57:45.000000 AAIT25-0.0.7/orangecontrib/AAIT/widgets/icons/TextPreprocessing.svg
+-rw-rw-rw-   0        0        0     1082 2024-02-19 21:08:44.000000 AAIT25-0.0.7/orangecontrib/AAIT/widgets/icons/chatbot.svg
+-rw-rw-rw-   0        0        0     8188 2024-05-23 18:08:49.000000 AAIT25-0.0.7/orangecontrib/AAIT/widgets/owchatbot.py
+-rw-rw-rw-   0        0        0       55 2024-01-18 15:57:45.000000 AAIT25-0.0.7/orangecontrib/__init__.py
+-rw-rw-rw-   0        0        0       42 2024-05-23 18:09:06.631350 AAIT25-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1793 2024-05-23 18:08:56.000000 AAIT25-0.0.7/setup.py
```

### Comparing `AAIT25-0.0.6/AAIT25.egg-info/SOURCES.txt` & `AAIT25-0.0.7/AAIT25.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `AAIT25-0.0.6/orangecontrib/AAIT/examples/example-chatbot.ows` & `AAIT25-0.0.7/orangecontrib/AAIT/examples/example-chatbot.ows`

 * *Files identical despite different names*

### Comparing `AAIT25-0.0.6/orangecontrib/AAIT/execute_thread.py` & `AAIT25-0.0.7/orangecontrib/AAIT/execute_thread.py`

 * *Files identical despite different names*

### Comparing `AAIT25-0.0.6/orangecontrib/AAIT/widgets/designer/owchatbot.ui` & `AAIT25-0.0.7/orangecontrib/AAIT/widgets/designer/owchatbot.ui`

 * *Files identical despite different names*

### Comparing `AAIT25-0.0.6/orangecontrib/AAIT/widgets/icons/Chatbotpy.svg` & `AAIT25-0.0.7/orangecontrib/AAIT/widgets/icons/Chatbotpy.svg`

 * *Files identical despite different names*

### Comparing `AAIT25-0.0.6/orangecontrib/AAIT/widgets/icons/DocumentEater.svg` & `AAIT25-0.0.7/orangecontrib/AAIT/widgets/icons/DocumentEater.svg`

 * *Files identical despite different names*

### Comparing `AAIT25-0.0.6/orangecontrib/AAIT/widgets/icons/Embeddings.svg` & `AAIT25-0.0.7/orangecontrib/AAIT/widgets/icons/Embeddings.svg`

 * *Files identical despite different names*

### Comparing `AAIT25-0.0.6/orangecontrib/AAIT/widgets/icons/LanguageModel.svg` & `AAIT25-0.0.7/orangecontrib/AAIT/widgets/icons/LanguageModel.svg`

 * *Files identical despite different names*

### Comparing `AAIT25-0.0.6/orangecontrib/AAIT/widgets/icons/chatbot.svg` & `AAIT25-0.0.7/orangecontrib/AAIT/widgets/icons/chatbot.svg`

 * *Files identical despite different names*

### Comparing `AAIT25-0.0.6/orangecontrib/AAIT/widgets/owchatbot.py` & `AAIT25-0.0.7/orangecontrib/AAIT/widgets/owchatbot.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from Orange.data import Domain, Table, StringVariable, ContinuousVariable, DiscreteVariable
 
 from PyQt5 import uic
 from PyQt5 import QtWidgets
 from PyQt5.QtCore import pyqtSignal
 from AnyQt.QtWidgets import QApplication
 
-from orangecontrib.llm_souverain.execute_thread import ExecuteThread
+from orangecontrib.AAIT.execute_thread import ExecuteThread
 
 from gpt4all import GPT4All
 
 
 class OWChatbot(widget.OWWidget):
     name = "Chatbot"
     description = """Select a local language model (.gguf file) to process a text request !
```

### Comparing `AAIT25-0.0.6/setup.py` & `AAIT25-0.0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 # Nom du package PyPI ('pip install NAME')
 NAME = "AAIT25"
 
 # Version du package PyPI
-VERSION = "0.0.6" # la version doit être supérieure à la précédente sinon la publication sera refusée
+VERSION = "0.0.7" # la version doit être supérieure à la précédente sinon la publication sera refusée
 
 # Facultatif / Adaptable à souhait
 AUTHOR = ""
 AUTHOR_EMAIL = ""
 URL = ""
 DESCRIPTION = "LLM addons for Orange Data Mining !"
 LICENSE = ""
```

