# Comparing `tmp/AAIT25-0.0.5.tar.gz` & `tmp/AAIT25-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AAIT25-0.0.5.tar", last modified: Thu May 23 18:01:26 2024, max compression
+gzip compressed data, was "AAIT25-0.0.6.tar", last modified: Thu May 23 18:04:49 2024, max compression
```

## Comparing `AAIT25-0.0.5.tar` & `AAIT25-0.0.6.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 18:01:26.265630 AAIT25-0.0.5/
-drwxrwxrwx   0        0        0        0 2024-05-23 18:01:26.257617 AAIT25-0.0.5/AAIT25.egg-info/
--rw-rw-rw-   0        0        0      236 2024-05-23 18:01:26.000000 AAIT25-0.0.5/AAIT25.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      818 2024-05-23 18:01:26.000000 AAIT25-0.0.5/AAIT25.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 18:01:26.000000 AAIT25-0.0.5/AAIT25.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2024-05-23 18:01:26.000000 AAIT25-0.0.5/AAIT25.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       14 2024-05-23 18:01:26.000000 AAIT25-0.0.5/AAIT25.egg-info/namespace_packages.txt
--rw-rw-rw-   0        0        0       29 2024-05-23 18:01:26.000000 AAIT25-0.0.5/AAIT25.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-23 18:01:26.000000 AAIT25-0.0.5/AAIT25.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2024-01-18 15:57:45.000000 AAIT25-0.0.5/License.txt
--rw-rw-rw-   0        0        0      236 2024-05-23 18:01:26.264631 AAIT25-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-01-18 15:57:45.000000 AAIT25-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-23 18:01:26.257617 AAIT25-0.0.5/orangecontrib/
--rw-rw-rw-   0        0        0       55 2024-01-18 15:57:45.000000 AAIT25-0.0.5/orangecontrib/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 18:01:26.258625 AAIT25-0.0.5/orangecontrib/aait/
--rw-rw-rw-   0        0        0        0 2024-01-18 15:57:45.000000 AAIT25-0.0.5/orangecontrib/aait/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 18:01:26.259625 AAIT25-0.0.5/orangecontrib/aait/examples/
--rw-rw-rw-   0        0        0     7856 2024-02-20 12:43:50.000000 AAIT25-0.0.5/orangecontrib/aait/examples/example-chatbot.ows
--rw-rw-rw-   0        0        0      966 2024-03-06 08:40:04.000000 AAIT25-0.0.5/orangecontrib/aait/execute_thread.py
-drwxrwxrwx   0        0        0        0 2024-05-23 18:01:26.260632 AAIT25-0.0.5/orangecontrib/aait/widgets/
--rw-rw-rw-   0        0        0        0 2024-01-18 15:57:45.000000 AAIT25-0.0.5/orangecontrib/aait/widgets/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 18:01:26.260632 AAIT25-0.0.5/orangecontrib/aait/widgets/designer/
--rw-rw-rw-   0        0        0     2337 2024-03-04 19:45:00.000000 AAIT25-0.0.5/orangecontrib/aait/widgets/designer/owchatbot.ui
-drwxrwxrwx   0        0        0        0 2024-05-23 18:01:26.263631 AAIT25-0.0.5/orangecontrib/aait/widgets/icons/
--rw-rw-rw-   0        0        0      831 2024-01-18 15:57:45.000000 AAIT25-0.0.5/orangecontrib/aait/widgets/icons/Chatbotpy.svg
--rw-rw-rw-   0        0        0     1596 2024-01-18 15:57:45.000000 AAIT25-0.0.5/orangecontrib/aait/widgets/icons/DocumentEater.svg
--rw-rw-rw-   0        0        0     4195 2024-01-18 15:57:45.000000 AAIT25-0.0.5/orangecontrib/aait/widgets/icons/Embeddings.svg
--rw-rw-rw-   0        0        0     1357 2024-01-18 15:57:45.000000 AAIT25-0.0.5/orangecontrib/aait/widgets/icons/LanguageModel.svg
--rw-rw-rw-   0        0        0      500 2024-01-18 15:57:45.000000 AAIT25-0.0.5/orangecontrib/aait/widgets/icons/TextPreprocessing.svg
--rw-rw-rw-   0        0        0     1082 2024-02-19 21:08:44.000000 AAIT25-0.0.5/orangecontrib/aait/widgets/icons/chatbot.svg
--rw-rw-rw-   0        0        0     8204 2024-03-12 21:47:18.000000 AAIT25-0.0.5/orangecontrib/aait/widgets/owchatbot.py
--rw-rw-rw-   0        0        0       42 2024-05-23 18:01:26.265630 AAIT25-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1793 2024-05-23 18:01:21.000000 AAIT25-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 18:04:49.294690 AAIT25-0.0.6/
+drwxrwxrwx   0        0        0        0 2024-05-23 18:04:49.287172 AAIT25-0.0.6/AAIT25.egg-info/
+-rw-rw-rw-   0        0        0      236 2024-05-23 18:04:49.000000 AAIT25-0.0.6/AAIT25.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      818 2024-05-23 18:04:49.000000 AAIT25-0.0.6/AAIT25.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 18:04:49.000000 AAIT25-0.0.6/AAIT25.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2024-05-23 18:04:49.000000 AAIT25-0.0.6/AAIT25.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       14 2024-05-23 18:04:49.000000 AAIT25-0.0.6/AAIT25.egg-info/namespace_packages.txt
+-rw-rw-rw-   0        0        0       29 2024-05-23 18:04:49.000000 AAIT25-0.0.6/AAIT25.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-23 18:04:49.000000 AAIT25-0.0.6/AAIT25.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2024-01-18 15:57:45.000000 AAIT25-0.0.6/License.txt
+-rw-rw-rw-   0        0        0      236 2024-05-23 18:04:49.293691 AAIT25-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-01-18 15:57:45.000000 AAIT25-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-23 18:04:49.287172 AAIT25-0.0.6/orangecontrib/
+drwxrwxrwx   0        0        0        0 2024-05-23 18:04:49.288685 AAIT25-0.0.6/orangecontrib/AAIT/
+-rw-rw-rw-   0        0        0        0 2024-01-18 15:57:45.000000 AAIT25-0.0.6/orangecontrib/AAIT/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 18:04:49.288685 AAIT25-0.0.6/orangecontrib/AAIT/examples/
+-rw-rw-rw-   0        0        0     7856 2024-02-20 12:43:50.000000 AAIT25-0.0.6/orangecontrib/AAIT/examples/example-chatbot.ows
+-rw-rw-rw-   0        0        0      966 2024-03-06 08:40:04.000000 AAIT25-0.0.6/orangecontrib/AAIT/execute_thread.py
+drwxrwxrwx   0        0        0        0 2024-05-23 18:04:49.289691 AAIT25-0.0.6/orangecontrib/AAIT/widgets/
+-rw-rw-rw-   0        0        0        0 2024-01-18 15:57:45.000000 AAIT25-0.0.6/orangecontrib/AAIT/widgets/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 18:04:49.290691 AAIT25-0.0.6/orangecontrib/AAIT/widgets/designer/
+-rw-rw-rw-   0        0        0     2337 2024-03-04 19:45:00.000000 AAIT25-0.0.6/orangecontrib/AAIT/widgets/designer/owchatbot.ui
+drwxrwxrwx   0        0        0        0 2024-05-23 18:04:49.293691 AAIT25-0.0.6/orangecontrib/AAIT/widgets/icons/
+-rw-rw-rw-   0        0        0      831 2024-01-18 15:57:45.000000 AAIT25-0.0.6/orangecontrib/AAIT/widgets/icons/Chatbotpy.svg
+-rw-rw-rw-   0        0        0     1596 2024-01-18 15:57:45.000000 AAIT25-0.0.6/orangecontrib/AAIT/widgets/icons/DocumentEater.svg
+-rw-rw-rw-   0        0        0     4195 2024-01-18 15:57:45.000000 AAIT25-0.0.6/orangecontrib/AAIT/widgets/icons/Embeddings.svg
+-rw-rw-rw-   0        0        0     1357 2024-01-18 15:57:45.000000 AAIT25-0.0.6/orangecontrib/AAIT/widgets/icons/LanguageModel.svg
+-rw-rw-rw-   0        0        0      500 2024-01-18 15:57:45.000000 AAIT25-0.0.6/orangecontrib/AAIT/widgets/icons/TextPreprocessing.svg
+-rw-rw-rw-   0        0        0     1082 2024-02-19 21:08:44.000000 AAIT25-0.0.6/orangecontrib/AAIT/widgets/icons/chatbot.svg
+-rw-rw-rw-   0        0        0     8197 2024-05-23 18:03:12.000000 AAIT25-0.0.6/orangecontrib/AAIT/widgets/owchatbot.py
+-rw-rw-rw-   0        0        0       55 2024-01-18 15:57:45.000000 AAIT25-0.0.6/orangecontrib/__init__.py
+-rw-rw-rw-   0        0        0       42 2024-05-23 18:04:49.294690 AAIT25-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1793 2024-05-23 18:04:24.000000 AAIT25-0.0.6/setup.py
```

### Comparing `AAIT25-0.0.5/AAIT25.egg-info/SOURCES.txt` & `AAIT25-0.0.6/AAIT25.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 AAIT25.egg-info/SOURCES.txt
 AAIT25.egg-info/dependency_links.txt
 AAIT25.egg-info/entry_points.txt
 AAIT25.egg-info/namespace_packages.txt
 AAIT25.egg-info/requires.txt
 AAIT25.egg-info/top_level.txt
 orangecontrib/__init__.py
-orangecontrib/aait/__init__.py
-orangecontrib/aait/execute_thread.py
-orangecontrib/aait/examples/example-chatbot.ows
-orangecontrib/aait/widgets/__init__.py
-orangecontrib/aait/widgets/owchatbot.py
-orangecontrib/aait/widgets/designer/owchatbot.ui
-orangecontrib/aait/widgets/icons/Chatbotpy.svg
-orangecontrib/aait/widgets/icons/DocumentEater.svg
-orangecontrib/aait/widgets/icons/Embeddings.svg
-orangecontrib/aait/widgets/icons/LanguageModel.svg
-orangecontrib/aait/widgets/icons/TextPreprocessing.svg
-orangecontrib/aait/widgets/icons/chatbot.svg
+orangecontrib/AAIT/__init__.py
+orangecontrib/AAIT/execute_thread.py
+orangecontrib/AAIT/examples/example-chatbot.ows
+orangecontrib/AAIT/widgets/__init__.py
+orangecontrib/AAIT/widgets/owchatbot.py
+orangecontrib/AAIT/widgets/designer/owchatbot.ui
+orangecontrib/AAIT/widgets/icons/Chatbotpy.svg
+orangecontrib/AAIT/widgets/icons/DocumentEater.svg
+orangecontrib/AAIT/widgets/icons/Embeddings.svg
+orangecontrib/AAIT/widgets/icons/LanguageModel.svg
+orangecontrib/AAIT/widgets/icons/TextPreprocessing.svg
+orangecontrib/AAIT/widgets/icons/chatbot.svg
```

### Comparing `AAIT25-0.0.5/orangecontrib/aait/examples/example-chatbot.ows` & `AAIT25-0.0.6/orangecontrib/AAIT/examples/example-chatbot.ows`

 * *Files identical despite different names*

### Comparing `AAIT25-0.0.5/orangecontrib/aait/execute_thread.py` & `AAIT25-0.0.6/orangecontrib/AAIT/execute_thread.py`

 * *Files identical despite different names*

### Comparing `AAIT25-0.0.5/orangecontrib/aait/widgets/designer/owchatbot.ui` & `AAIT25-0.0.6/orangecontrib/AAIT/widgets/designer/owchatbot.ui`

 * *Files identical despite different names*

### Comparing `AAIT25-0.0.5/orangecontrib/aait/widgets/icons/Chatbotpy.svg` & `AAIT25-0.0.6/orangecontrib/AAIT/widgets/icons/Chatbotpy.svg`

 * *Files identical despite different names*

### Comparing `AAIT25-0.0.5/orangecontrib/aait/widgets/icons/DocumentEater.svg` & `AAIT25-0.0.6/orangecontrib/AAIT/widgets/icons/DocumentEater.svg`

 * *Files identical despite different names*

### Comparing `AAIT25-0.0.5/orangecontrib/aait/widgets/icons/Embeddings.svg` & `AAIT25-0.0.6/orangecontrib/AAIT/widgets/icons/Embeddings.svg`

 * *Files identical despite different names*

### Comparing `AAIT25-0.0.5/orangecontrib/aait/widgets/icons/LanguageModel.svg` & `AAIT25-0.0.6/orangecontrib/AAIT/widgets/icons/LanguageModel.svg`

 * *Files identical despite different names*

### Comparing `AAIT25-0.0.5/orangecontrib/aait/widgets/icons/chatbot.svg` & `AAIT25-0.0.6/orangecontrib/AAIT/widgets/icons/chatbot.svg`

 * *Files identical despite different names*

### Comparing `AAIT25-0.0.5/orangecontrib/aait/widgets/owchatbot.py` & `AAIT25-0.0.6/orangecontrib/AAIT/widgets/owchatbot.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,15 +100,15 @@
                            "repeat_penalty": 1.18, "repeat_last_n": 64, "n_batch": 8}
         self.llm = None
 
         self.thread = None
         self.current_answer = ""
 
         ### QT Management ###
-        uic.loadUi(os.path.dirname(os.path.abspath(__file__)) + '/widget_designer/owchatbot.ui', self)
+        uic.loadUi(os.path.dirname(os.path.abspath(__file__)) + '/designer/owchatbot.ui', self)
         self.setFixedWidth(571)
         self.setFixedHeight(468)
         self.setAutoFillBackground(True)
 
         self.pushbtn_selectModel = self.findChild(QtWidgets.QPushButton, "selectModel")
         self.label_selectedModel = self.findChild(QtWidgets.QLabel, "selectedModel")
         self.label_answer = self.findChild(QtWidgets.QPlainTextEdit, "answer")
```

### Comparing `AAIT25-0.0.5/setup.py` & `AAIT25-0.0.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 # Nom du package PyPI ('pip install NAME')
 NAME = "AAIT25"
 
 # Version du package PyPI
-VERSION = "0.0.5" # la version doit être supérieure à la précédente sinon la publication sera refusée
+VERSION = "0.0.6" # la version doit être supérieure à la précédente sinon la publication sera refusée
 
 # Facultatif / Adaptable à souhait
 AUTHOR = ""
 AUTHOR_EMAIL = ""
 URL = ""
 DESCRIPTION = "LLM addons for Orange Data Mining !"
 LICENSE = ""
@@ -17,26 +17,26 @@
 KEYWORDS = ("orange3 add-on",)
 
 # Tous les packages python existants dans le projet
 PACKAGES = find_packages()
 
 # Fichiers additionnels aux fichiers .py (comme les icons ou des .ows)
 PACKAGE_DATA = {
-	"orangecontrib.aait.widgets": ["icons/*", "designer/*"], # contenu du dossier 'icons' situé dans 'orangecontrib/hkh_bot/widgets'
-	"orangecontrib.aait": ["examples/*"],
+	"orangecontrib.AAIT.widgets": ["icons/*", "designer/*"], # contenu du dossier 'icons' situé dans 'orangecontrib/hkh_bot/widgets'
+	"orangecontrib.AAIT": ["examples/*"],
 }
 # /!\ les noms de fichier 'orangecontrib.hkh_bot.widgets' doivent correspondre à l'arborescence
 
 # Dépendances
 INSTALL_REQUIRES = ["sentence-transformers==2.5.1"]
 
 # Spécifie le dossier contenant les widgets et le nom de section qu'aura l'addon sur Orange
 ENTRY_POINTS = {
 	"orange.widgets": (
-		"AAIT = orangecontrib.aait.widgets", # 'HKH-Bot' sera le nom de la section Orange contenant les widgets
+		"AAIT = orangecontrib.AAIT.widgets", # 'HKH-Bot' sera le nom de la section Orange contenant les widgets
 	)
 }
 # /!\ les noms de fichier 'orangecontrib.hkh_bot.widgets' doivent correspondre à l'arborescence
 
 NAMESPACE_PACKAGES = ["orangecontrib"]
 
 setup(name=NAME,
```

