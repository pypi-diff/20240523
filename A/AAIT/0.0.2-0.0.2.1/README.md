# Comparing `tmp/AAIT-0.0.2.tar.gz` & `tmp/AAIT-0.0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AAIT-0.0.2.tar", last modified: Thu May 23 19:27:12 2024, max compression
+gzip compressed data, was "AAIT-0.0.2.1.tar", last modified: Thu May 23 19:28:51 2024, max compression
```

## Comparing `AAIT-0.0.2.tar` & `AAIT-0.0.2.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 19:27:12.699977 AAIT-0.0.2/
-drwxrwxrwx   0        0        0        0 2024-05-23 19:27:12.691456 AAIT-0.0.2/AAIT.egg-info/
--rw-rw-rw-   0        0        0      261 2024-05-23 19:27:12.000000 AAIT-0.0.2/AAIT.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      811 2024-05-23 19:27:12.000000 AAIT-0.0.2/AAIT.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 19:27:12.000000 AAIT-0.0.2/AAIT.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2024-05-23 19:27:12.000000 AAIT-0.0.2/AAIT.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       14 2024-05-23 19:27:12.000000 AAIT-0.0.2/AAIT.egg-info/namespace_packages.txt
--rw-rw-rw-   0        0        0       40 2024-05-23 19:27:12.000000 AAIT-0.0.2/AAIT.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-23 19:27:12.000000 AAIT-0.0.2/AAIT.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2024-01-18 15:57:45.000000 AAIT-0.0.2/License.txt
--rw-rw-rw-   0        0        0      261 2024-05-23 19:27:12.698979 AAIT-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-01-18 15:57:45.000000 AAIT-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-23 19:27:12.691456 AAIT-0.0.2/orangecontrib/
-drwxrwxrwx   0        0        0        0 2024-05-23 19:27:12.692458 AAIT-0.0.2/orangecontrib/AAIT/
--rw-rw-rw-   0        0        0        0 2024-01-18 15:57:45.000000 AAIT-0.0.2/orangecontrib/AAIT/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 19:27:12.693462 AAIT-0.0.2/orangecontrib/AAIT/examples/
--rw-rw-rw-   0        0        0     7856 2024-02-20 12:43:50.000000 AAIT-0.0.2/orangecontrib/AAIT/examples/example-chatbot.ows
--rw-rw-rw-   0        0        0      966 2024-03-06 08:40:04.000000 AAIT-0.0.2/orangecontrib/AAIT/execute_thread.py
-drwxrwxrwx   0        0        0        0 2024-05-23 19:27:12.693967 AAIT-0.0.2/orangecontrib/AAIT/widgets/
--rw-rw-rw-   0        0        0        0 2024-01-18 15:57:45.000000 AAIT-0.0.2/orangecontrib/AAIT/widgets/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 19:27:12.697977 AAIT-0.0.2/orangecontrib/AAIT/widgets/icons/
--rw-rw-rw-   0        0        0      831 2024-01-18 15:57:45.000000 AAIT-0.0.2/orangecontrib/AAIT/widgets/icons/Chatbotpy.svg
--rw-rw-rw-   0        0        0     1596 2024-01-18 15:57:45.000000 AAIT-0.0.2/orangecontrib/AAIT/widgets/icons/DocumentEater.svg
--rw-rw-rw-   0        0        0     4195 2024-01-18 15:57:45.000000 AAIT-0.0.2/orangecontrib/AAIT/widgets/icons/Embeddings.svg
--rw-rw-rw-   0        0        0     1357 2024-01-18 15:57:45.000000 AAIT-0.0.2/orangecontrib/AAIT/widgets/icons/LanguageModel.svg
--rw-rw-rw-   0        0        0      500 2024-01-18 15:57:45.000000 AAIT-0.0.2/orangecontrib/AAIT/widgets/icons/TextPreprocessing.svg
--rw-rw-rw-   0        0        0     1082 2024-02-19 21:08:44.000000 AAIT-0.0.2/orangecontrib/AAIT/widgets/icons/chatbot.svg
--rw-rw-rw-   0        0        0     8204 2024-03-12 21:47:18.000000 AAIT-0.0.2/orangecontrib/AAIT/widgets/owchatbot.py
-drwxrwxrwx   0        0        0        0 2024-05-23 19:27:12.697977 AAIT-0.0.2/orangecontrib/AAIT/widgets/widget_designer/
--rw-rw-rw-   0        0        0     2337 2024-03-04 19:45:00.000000 AAIT-0.0.2/orangecontrib/AAIT/widgets/widget_designer/owchatbot.ui
--rw-rw-rw-   0        0        0       55 2024-01-18 15:57:45.000000 AAIT-0.0.2/orangecontrib/__init__.py
--rw-rw-rw-   0        0        0       42 2024-05-23 19:27:12.699977 AAIT-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1821 2024-05-23 19:27:04.000000 AAIT-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 19:28:51.160622 AAIT-0.0.2.1/
+drwxrwxrwx   0        0        0        0 2024-05-23 19:28:51.153607 AAIT-0.0.2.1/AAIT.egg-info/
+-rw-rw-rw-   0        0        0      263 2024-05-23 19:28:51.000000 AAIT-0.0.2.1/AAIT.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      811 2024-05-23 19:28:51.000000 AAIT-0.0.2.1/AAIT.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 19:28:51.000000 AAIT-0.0.2.1/AAIT.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2024-05-23 19:28:51.000000 AAIT-0.0.2.1/AAIT.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       14 2024-05-23 19:28:51.000000 AAIT-0.0.2.1/AAIT.egg-info/namespace_packages.txt
+-rw-rw-rw-   0        0        0       40 2024-05-23 19:28:51.000000 AAIT-0.0.2.1/AAIT.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-23 19:28:51.000000 AAIT-0.0.2.1/AAIT.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2024-01-18 15:57:45.000000 AAIT-0.0.2.1/License.txt
+-rw-rw-rw-   0        0        0      263 2024-05-23 19:28:51.160622 AAIT-0.0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-01-18 15:57:45.000000 AAIT-0.0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-23 19:28:51.153607 AAIT-0.0.2.1/orangecontrib/
+drwxrwxrwx   0        0        0        0 2024-05-23 19:28:51.154611 AAIT-0.0.2.1/orangecontrib/AAIT/
+-rw-rw-rw-   0        0        0        0 2024-01-18 15:57:45.000000 AAIT-0.0.2.1/orangecontrib/AAIT/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 19:28:51.155623 AAIT-0.0.2.1/orangecontrib/AAIT/examples/
+-rw-rw-rw-   0        0        0     7856 2024-02-20 12:43:50.000000 AAIT-0.0.2.1/orangecontrib/AAIT/examples/example-chatbot.ows
+-rw-rw-rw-   0        0        0      966 2024-03-06 08:40:04.000000 AAIT-0.0.2.1/orangecontrib/AAIT/execute_thread.py
+drwxrwxrwx   0        0        0        0 2024-05-23 19:28:51.156618 AAIT-0.0.2.1/orangecontrib/AAIT/widgets/
+-rw-rw-rw-   0        0        0        0 2024-01-18 15:57:45.000000 AAIT-0.0.2.1/orangecontrib/AAIT/widgets/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 19:28:51.159615 AAIT-0.0.2.1/orangecontrib/AAIT/widgets/icons/
+-rw-rw-rw-   0        0        0      831 2024-01-18 15:57:45.000000 AAIT-0.0.2.1/orangecontrib/AAIT/widgets/icons/Chatbotpy.svg
+-rw-rw-rw-   0        0        0     1596 2024-01-18 15:57:45.000000 AAIT-0.0.2.1/orangecontrib/AAIT/widgets/icons/DocumentEater.svg
+-rw-rw-rw-   0        0        0     4195 2024-01-18 15:57:45.000000 AAIT-0.0.2.1/orangecontrib/AAIT/widgets/icons/Embeddings.svg
+-rw-rw-rw-   0        0        0     1357 2024-01-18 15:57:45.000000 AAIT-0.0.2.1/orangecontrib/AAIT/widgets/icons/LanguageModel.svg
+-rw-rw-rw-   0        0        0      500 2024-01-18 15:57:45.000000 AAIT-0.0.2.1/orangecontrib/AAIT/widgets/icons/TextPreprocessing.svg
+-rw-rw-rw-   0        0        0     1082 2024-02-19 21:08:44.000000 AAIT-0.0.2.1/orangecontrib/AAIT/widgets/icons/chatbot.svg
+-rw-rw-rw-   0        0        0     8204 2024-03-12 21:47:18.000000 AAIT-0.0.2.1/orangecontrib/AAIT/widgets/owchatbot.py
+drwxrwxrwx   0        0        0        0 2024-05-23 19:28:51.159615 AAIT-0.0.2.1/orangecontrib/AAIT/widgets/widget_designer/
+-rw-rw-rw-   0        0        0     2337 2024-03-04 19:45:00.000000 AAIT-0.0.2.1/orangecontrib/AAIT/widgets/widget_designer/owchatbot.ui
+-rw-rw-rw-   0        0        0       55 2024-01-18 15:57:45.000000 AAIT-0.0.2.1/orangecontrib/__init__.py
+-rw-rw-rw-   0        0        0       42 2024-05-23 19:28:51.161615 AAIT-0.0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1814 2024-05-23 19:28:22.000000 AAIT-0.0.2.1/setup.py
```

### Comparing `AAIT-0.0.2/AAIT.egg-info/SOURCES.txt` & `AAIT-0.0.2.1/AAIT.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `AAIT-0.0.2/orangecontrib/AAIT/examples/example-chatbot.ows` & `AAIT-0.0.2.1/orangecontrib/AAIT/examples/example-chatbot.ows`

 * *Files identical despite different names*

### Comparing `AAIT-0.0.2/orangecontrib/AAIT/execute_thread.py` & `AAIT-0.0.2.1/orangecontrib/AAIT/execute_thread.py`

 * *Files identical despite different names*

### Comparing `AAIT-0.0.2/orangecontrib/AAIT/widgets/icons/Chatbotpy.svg` & `AAIT-0.0.2.1/orangecontrib/AAIT/widgets/icons/Chatbotpy.svg`

 * *Files identical despite different names*

### Comparing `AAIT-0.0.2/orangecontrib/AAIT/widgets/icons/DocumentEater.svg` & `AAIT-0.0.2.1/orangecontrib/AAIT/widgets/icons/DocumentEater.svg`

 * *Files identical despite different names*

### Comparing `AAIT-0.0.2/orangecontrib/AAIT/widgets/icons/Embeddings.svg` & `AAIT-0.0.2.1/orangecontrib/AAIT/widgets/icons/Embeddings.svg`

 * *Files identical despite different names*

### Comparing `AAIT-0.0.2/orangecontrib/AAIT/widgets/icons/LanguageModel.svg` & `AAIT-0.0.2.1/orangecontrib/AAIT/widgets/icons/LanguageModel.svg`

 * *Files identical despite different names*

### Comparing `AAIT-0.0.2/orangecontrib/AAIT/widgets/icons/chatbot.svg` & `AAIT-0.0.2.1/orangecontrib/AAIT/widgets/icons/chatbot.svg`

 * *Files identical despite different names*

### Comparing `AAIT-0.0.2/orangecontrib/AAIT/widgets/owchatbot.py` & `AAIT-0.0.2.1/orangecontrib/AAIT/widgets/owchatbot.py`

 * *Files identical despite different names*

### Comparing `AAIT-0.0.2/orangecontrib/AAIT/widgets/widget_designer/owchatbot.ui` & `AAIT-0.0.2.1/orangecontrib/AAIT/widgets/widget_designer/owchatbot.ui`

 * *Files identical despite different names*

### Comparing `AAIT-0.0.2/setup.py` & `AAIT-0.0.2.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 # Nom du package PyPI ('pip install NAME')
 NAME = "AAIT"
 
 # Version du package PyPI
-VERSION = "0.0.2" # la version doit être supérieure à la précédente sinon la publication sera refusée
+VERSION = "0.0.2.1" # la version doit être supérieure à la précédente sinon la publication sera refusée
 
 # Facultatif / Adaptable à souhait
 AUTHOR = ""
 AUTHOR_EMAIL = ""
 URL = ""
 DESCRIPTION = "LLM addons for Orange Data Mining !"
 LICENSE = ""
@@ -28,15 +28,15 @@
 
 # Dépendances
 INSTALL_REQUIRES = ["gpt4all==2.2.1", "Orange3-Textable==3.1.11"]
 
 # Spécifie le dossier contenant les widgets et le nom de section qu'aura l'addon sur Orange
 ENTRY_POINTS = {
 	"orange.widgets": (
-		"LLM-Souverain = orangecontrib.AAIT.widgets", # 'HKH-Bot' sera le nom de la section Orange contenant les widgets
+		"AAIT = orangecontrib.AAIT.widgets", # 'HKH-Bot' sera le nom de la section Orange contenant les widgets
 	)
 }
 # /!\ les noms de fichier 'orangecontrib.hkh_bot.widgets' doivent correspondre à l'arborescence
 
 NAMESPACE_PACKAGES = ["orangecontrib"]
 
 setup(name=NAME,
```

