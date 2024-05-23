# Comparing `tmp/LLM-Souverain-0.0.5.tar.gz` & `tmp/LLM-Souverain-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LLM-Souverain-0.0.5.tar", last modified: Mon Mar  4 20:03:51 2024, max compression
+gzip compressed data, was "LLM-Souverain-0.0.6.tar", last modified: Thu May 23 17:51:19 2024, max compression
```

## Comparing `LLM-Souverain-0.0.5.tar` & `LLM-Souverain-0.0.6.tar`

### file list

```diff
@@ -1,37 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-03-04 20:03:51.490008 LLM-Souverain-0.0.5/
-drwxrwxrwx   0        0        0        0 2024-03-04 20:03:51.475245 LLM-Souverain-0.0.5/LLM_Souverain.egg-info/
--rw-rw-rw-   0        0        0      270 2024-03-04 20:03:51.000000 LLM-Souverain-0.0.5/LLM_Souverain.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1204 2024-03-04 20:03:51.000000 LLM-Souverain-0.0.5/LLM_Souverain.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-04 20:03:51.000000 LLM-Souverain-0.0.5/LLM_Souverain.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       69 2024-03-04 20:03:51.000000 LLM-Souverain-0.0.5/LLM_Souverain.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       14 2024-03-04 20:03:51.000000 LLM-Souverain-0.0.5/LLM_Souverain.egg-info/namespace_packages.txt
--rw-rw-rw-   0        0        0       40 2024-03-04 20:03:51.000000 LLM-Souverain-0.0.5/LLM_Souverain.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-03-04 20:03:51.000000 LLM-Souverain-0.0.5/LLM_Souverain.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2024-01-18 15:57:45.000000 LLM-Souverain-0.0.5/License.txt
--rw-rw-rw-   0        0        0      270 2024-03-04 20:03:51.488748 LLM-Souverain-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-01-18 15:57:45.000000 LLM-Souverain-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2024-03-04 20:03:51.476246 LLM-Souverain-0.0.5/orangecontrib/
--rw-rw-rw-   0        0        0       55 2024-01-18 15:57:45.000000 LLM-Souverain-0.0.5/orangecontrib/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-04 20:03:51.476861 LLM-Souverain-0.0.5/orangecontrib/llm_souverain/
--rw-rw-rw-   0        0        0        0 2024-01-18 15:57:45.000000 LLM-Souverain-0.0.5/orangecontrib/llm_souverain/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-04 20:03:51.476861 LLM-Souverain-0.0.5/orangecontrib/llm_souverain/examples/
--rw-rw-rw-   0        0        0     7856 2024-02-20 12:43:50.000000 LLM-Souverain-0.0.5/orangecontrib/llm_souverain/examples/example-chatbot.ows
-drwxrwxrwx   0        0        0        0 2024-03-04 20:03:51.483744 LLM-Souverain-0.0.5/orangecontrib/llm_souverain/widgets/
--rw-rw-rw-   0        0        0    48045 2024-02-20 13:12:14.000000 LLM-Souverain-0.0.5/orangecontrib/llm_souverain/widgets/Chatbot.py
--rw-rw-rw-   0        0        0    41503 2024-02-20 12:52:05.000000 LLM-Souverain-0.0.5/orangecontrib/llm_souverain/widgets/DocumentEater.py
--rw-rw-rw-   0        0        0    37549 2024-02-20 12:52:36.000000 LLM-Souverain-0.0.5/orangecontrib/llm_souverain/widgets/EmbeddingsCreation.py
--rw-rw-rw-   0        0        0    38725 2024-02-20 12:52:51.000000 LLM-Souverain-0.0.5/orangecontrib/llm_souverain/widgets/LanguageModel.py
--rw-rw-rw-   0        0        0    40727 2024-02-20 12:53:11.000000 LLM-Souverain-0.0.5/orangecontrib/llm_souverain/widgets/TextPreprocessing.py
--rw-rw-rw-   0        0        0        0 2024-01-18 15:57:45.000000 LLM-Souverain-0.0.5/orangecontrib/llm_souverain/widgets/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-04 20:03:51.487750 LLM-Souverain-0.0.5/orangecontrib/llm_souverain/widgets/icons/
--rw-rw-rw-   0        0        0      831 2024-01-18 15:57:45.000000 LLM-Souverain-0.0.5/orangecontrib/llm_souverain/widgets/icons/Chatbotpy.svg
--rw-rw-rw-   0        0        0     1596 2024-01-18 15:57:45.000000 LLM-Souverain-0.0.5/orangecontrib/llm_souverain/widgets/icons/DocumentEater.svg
--rw-rw-rw-   0        0        0     4195 2024-01-18 15:57:45.000000 LLM-Souverain-0.0.5/orangecontrib/llm_souverain/widgets/icons/Embeddings.svg
--rw-rw-rw-   0        0        0     1357 2024-01-18 15:57:45.000000 LLM-Souverain-0.0.5/orangecontrib/llm_souverain/widgets/icons/LanguageModel.svg
--rw-rw-rw-   0        0        0      500 2024-01-18 15:57:45.000000 LLM-Souverain-0.0.5/orangecontrib/llm_souverain/widgets/icons/TextPreprocessing.svg
--rw-rw-rw-   0        0        0     1082 2024-02-19 21:08:44.000000 LLM-Souverain-0.0.5/orangecontrib/llm_souverain/widgets/icons/chatbot.svg
--rw-rw-rw-   0        0        0     8208 2024-03-04 20:01:27.000000 LLM-Souverain-0.0.5/orangecontrib/llm_souverain/widgets/owchatbot.py
-drwxrwxrwx   0        0        0        0 2024-03-04 20:03:51.488748 LLM-Souverain-0.0.5/orangecontrib/llm_souverain/widgets/widget_designer/
--rw-rw-rw-   0        0        0     2337 2024-03-04 19:45:00.000000 LLM-Souverain-0.0.5/orangecontrib/llm_souverain/widgets/widget_designer/owchatbot.ui
--rw-rw-rw-   0        0        0       42 2024-03-04 20:03:51.490008 LLM-Souverain-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1857 2024-03-04 20:02:37.000000 LLM-Souverain-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 17:51:19.314596 LLM-Souverain-0.0.6/
+drwxrwxrwx   0        0        0        0 2024-05-23 17:51:19.310588 LLM-Souverain-0.0.6/LLM_Souverain.egg-info/
+-rw-rw-rw-   0        0        0      270 2024-05-23 17:51:19.000000 LLM-Souverain-0.0.6/LLM_Souverain.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      509 2024-05-23 17:51:19.000000 LLM-Souverain-0.0.6/LLM_Souverain.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 17:51:19.000000 LLM-Souverain-0.0.6/LLM_Souverain.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       69 2024-05-23 17:51:19.000000 LLM-Souverain-0.0.6/LLM_Souverain.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       14 2024-05-23 17:51:19.000000 LLM-Souverain-0.0.6/LLM_Souverain.egg-info/namespace_packages.txt
+-rw-rw-rw-   0        0        0       40 2024-05-23 17:51:19.000000 LLM-Souverain-0.0.6/LLM_Souverain.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-23 17:51:19.000000 LLM-Souverain-0.0.6/LLM_Souverain.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2024-01-18 15:57:45.000000 LLM-Souverain-0.0.6/License.txt
+-rw-rw-rw-   0        0        0      270 2024-05-23 17:51:19.313594 LLM-Souverain-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-01-18 15:57:45.000000 LLM-Souverain-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-23 17:51:19.310588 LLM-Souverain-0.0.6/orangecontrib/
+-rw-rw-rw-   0        0        0       55 2024-01-18 15:57:45.000000 LLM-Souverain-0.0.6/orangecontrib/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 17:51:19.311595 LLM-Souverain-0.0.6/orangecontrib/llm_souverain/
+-rw-rw-rw-   0        0        0        0 2024-01-18 15:57:45.000000 LLM-Souverain-0.0.6/orangecontrib/llm_souverain/__init__.py
+-rw-rw-rw-   0        0        0      966 2024-03-06 08:40:04.000000 LLM-Souverain-0.0.6/orangecontrib/llm_souverain/execute_thread.py
+drwxrwxrwx   0        0        0        0 2024-05-23 17:51:19.313594 LLM-Souverain-0.0.6/orangecontrib/llm_souverain/widgets/
+-rw-rw-rw-   0        0        0        0 2024-01-18 15:57:45.000000 LLM-Souverain-0.0.6/orangecontrib/llm_souverain/widgets/__init__.py
+-rw-rw-rw-   0        0        0     8204 2024-03-12 21:47:18.000000 LLM-Souverain-0.0.6/orangecontrib/llm_souverain/widgets/owchatbot.py
+-rw-rw-rw-   0        0        0       42 2024-05-23 17:51:19.314596 LLM-Souverain-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1867 2024-05-23 17:51:17.000000 LLM-Souverain-0.0.6/setup.py
```

### Comparing `LLM-Souverain-0.0.5/orangecontrib/llm_souverain/widgets/owchatbot.py` & `LLM-Souverain-0.0.6/orangecontrib/llm_souverain/widgets/owchatbot.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from Orange.data import Domain, Table, StringVariable, ContinuousVariable, DiscreteVariable
 
 from PyQt5 import uic
 from PyQt5 import QtWidgets
 from PyQt5.QtCore import pyqtSignal
 from AnyQt.QtWidgets import QApplication
 
-from Orange.widgets.dev_workflow.HKH_execute_thread import ExecuteThread
+from orangecontrib.llm_souverain.execute_thread import ExecuteThread
 
 from gpt4all import GPT4All
 
 
 class OWChatbot(widget.OWWidget):
     name = "Chatbot"
     description = """Select a local language model (.gguf file) to process a text request !
```

### Comparing `LLM-Souverain-0.0.5/setup.py` & `LLM-Souverain-0.0.6/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 # Nom du package PyPI ('pip install NAME')
 NAME = "LLM-Souverain"
 
 # Version du package PyPI
-VERSION = "0.0.5" # la version doit être supérieure à la précédente sinon la publication sera refusée
+VERSION = "0.0.6" # la version doit être supérieure à la précédente sinon la publication sera refusée
 
 # Facultatif / Adaptable à souhait
 AUTHOR = ""
 AUTHOR_EMAIL = ""
 URL = ""
 DESCRIPTION = "LLM addons for Orange Data Mining !"
 LICENSE = ""
@@ -16,18 +16,18 @@
 # 'orange3 add-on' permet de rendre l'addon téléchargeable via l'interface addons d'Orange 
 KEYWORDS = ("orange3 add-on",)
 
 # Tous les packages python existants dans le projet
 PACKAGES = find_packages()
 
 # Fichiers additionnels aux fichiers .py (comme les icons ou des .ows)
-PACKAGE_DATA = {
-	"orangecontrib.llm_souverain.widgets": ["icons/*", "widget_designer/*"], # contenu du dossier 'icons' situé dans 'orangecontrib/hkh_bot/widgets'
-	"orangecontrib.llm_souverain": ["examples/*"],
-}
+# PACKAGE_DATA = {
+# 	"orangecontrib.llm_souverain.widgets": ["icons/*", "widget_designer/*"], # contenu du dossier 'icons' situé dans 'orangecontrib/hkh_bot/widgets'
+# 	"orangecontrib.llm_souverain": ["examples/*"],
+# }
 # /!\ les noms de fichier 'orangecontrib.hkh_bot.widgets' doivent correspondre à l'arborescence
 
 # Dépendances
 INSTALL_REQUIRES = ["gpt4all==2.2.1", "Orange3-Textable==3.1.11"]
 
 # Spécifie le dossier contenant les widgets et le nom de section qu'aura l'addon sur Orange
 ENTRY_POINTS = {
@@ -44,15 +44,15 @@
 	  author=AUTHOR,
 	  author_email=AUTHOR_EMAIL,
 	  url=URL,
 	  description=DESCRIPTION,
 	  license=LICENSE,
 	  keywords=KEYWORDS,
 	  packages=PACKAGES,
-	  package_data=PACKAGE_DATA,
+	  # package_data=PACKAGE_DATA,
 	  install_requires=INSTALL_REQUIRES,
 	  entry_points=ENTRY_POINTS,
 	  namespace_packages=NAMESPACE_PACKAGES,
 )
```

