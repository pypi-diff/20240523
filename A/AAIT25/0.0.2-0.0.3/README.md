# Comparing `tmp/AAIT25-0.0.2.tar.gz` & `tmp/AAIT25-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AAIT25-0.0.2.tar", last modified: Thu May 23 17:49:04 2024, max compression
+gzip compressed data, was "AAIT25-0.0.3.tar", last modified: Thu May 23 17:56:17 2024, max compression
```

## Comparing `AAIT25-0.0.2.tar` & `AAIT25-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,33 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 17:49:04.244297 AAIT25-0.0.2/
-drwxrwxrwx   0        0        0        0 2024-05-23 17:49:04.242298 AAIT25-0.0.2/AAIT25.egg-info/
--rw-rw-rw-   0        0        0      347 2024-05-23 17:49:04.000000 AAIT25-0.0.2/AAIT25.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      277 2024-05-23 17:49:04.000000 AAIT25-0.0.2/AAIT25.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 17:49:04.000000 AAIT25-0.0.2/AAIT25.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2024-05-23 17:49:04.000000 AAIT25-0.0.2/AAIT25.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       14 2024-05-23 17:49:04.000000 AAIT25-0.0.2/AAIT25.egg-info/namespace_packages.txt
--rw-rw-rw-   0        0        0       29 2024-05-23 17:49:04.000000 AAIT25-0.0.2/AAIT25.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-23 17:49:04.000000 AAIT25-0.0.2/AAIT25.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2024-01-18 15:57:45.000000 AAIT25-0.0.2/License.txt
--rw-rw-rw-   0        0        0      347 2024-05-23 17:49:04.243298 AAIT25-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-01-18 15:57:45.000000 AAIT25-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-23 17:49:04.243298 AAIT25-0.0.2/orangecontrib/
--rw-rw-rw-   0        0        0       55 2024-01-18 15:57:45.000000 AAIT25-0.0.2/orangecontrib/__init__.py
--rw-rw-rw-   0        0        0       42 2024-05-23 17:49:04.244297 AAIT25-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1980 2024-05-23 17:48:56.000000 AAIT25-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 17:56:17.469364 AAIT25-0.0.3/
+drwxrwxrwx   0        0        0        0 2024-05-23 17:56:17.462859 AAIT25-0.0.3/AAIT25.egg-info/
+-rw-rw-rw-   0        0        0      236 2024-05-23 17:56:17.000000 AAIT25-0.0.3/AAIT25.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      818 2024-05-23 17:56:17.000000 AAIT25-0.0.3/AAIT25.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 17:56:17.000000 AAIT25-0.0.3/AAIT25.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2024-05-23 17:56:17.000000 AAIT25-0.0.3/AAIT25.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       14 2024-05-23 17:56:17.000000 AAIT25-0.0.3/AAIT25.egg-info/namespace_packages.txt
+-rw-rw-rw-   0        0        0       29 2024-05-23 17:56:17.000000 AAIT25-0.0.3/AAIT25.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-23 17:56:17.000000 AAIT25-0.0.3/AAIT25.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2024-01-18 15:57:45.000000 AAIT25-0.0.3/License.txt
+-rw-rw-rw-   0        0        0      236 2024-05-23 17:56:17.468352 AAIT25-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-01-18 15:57:45.000000 AAIT25-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-23 17:56:17.462859 AAIT25-0.0.3/orangecontrib/
+drwxrwxrwx   0        0        0        0 2024-05-23 17:56:17.463847 AAIT25-0.0.3/orangecontrib/AAIT/
+-rw-rw-rw-   0        0        0        0 2024-01-18 15:57:45.000000 AAIT25-0.0.3/orangecontrib/AAIT/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 17:56:17.463847 AAIT25-0.0.3/orangecontrib/AAIT/examples/
+-rw-rw-rw-   0        0        0     7856 2024-02-20 12:43:50.000000 AAIT25-0.0.3/orangecontrib/AAIT/examples/example-chatbot.ows
+-rw-rw-rw-   0        0        0      966 2024-03-06 08:40:04.000000 AAIT25-0.0.3/orangecontrib/AAIT/execute_thread.py
+drwxrwxrwx   0        0        0        0 2024-05-23 17:56:17.464846 AAIT25-0.0.3/orangecontrib/AAIT/widgets/
+-rw-rw-rw-   0        0        0        0 2024-01-18 15:57:45.000000 AAIT25-0.0.3/orangecontrib/AAIT/widgets/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 17:56:17.465847 AAIT25-0.0.3/orangecontrib/AAIT/widgets/designer/
+-rw-rw-rw-   0        0        0     2337 2024-03-04 19:45:00.000000 AAIT25-0.0.3/orangecontrib/AAIT/widgets/designer/owchatbot.ui
+drwxrwxrwx   0        0        0        0 2024-05-23 17:56:17.468352 AAIT25-0.0.3/orangecontrib/AAIT/widgets/icons/
+-rw-rw-rw-   0        0        0      831 2024-01-18 15:57:45.000000 AAIT25-0.0.3/orangecontrib/AAIT/widgets/icons/Chatbotpy.svg
+-rw-rw-rw-   0        0        0     1596 2024-01-18 15:57:45.000000 AAIT25-0.0.3/orangecontrib/AAIT/widgets/icons/DocumentEater.svg
+-rw-rw-rw-   0        0        0     4195 2024-01-18 15:57:45.000000 AAIT25-0.0.3/orangecontrib/AAIT/widgets/icons/Embeddings.svg
+-rw-rw-rw-   0        0        0     1357 2024-01-18 15:57:45.000000 AAIT25-0.0.3/orangecontrib/AAIT/widgets/icons/LanguageModel.svg
+-rw-rw-rw-   0        0        0      500 2024-01-18 15:57:45.000000 AAIT25-0.0.3/orangecontrib/AAIT/widgets/icons/TextPreprocessing.svg
+-rw-rw-rw-   0        0        0     1082 2024-02-19 21:08:44.000000 AAIT25-0.0.3/orangecontrib/AAIT/widgets/icons/chatbot.svg
+-rw-rw-rw-   0        0        0     8204 2024-03-12 21:47:18.000000 AAIT25-0.0.3/orangecontrib/AAIT/widgets/owchatbot.py
+-rw-rw-rw-   0        0        0       55 2024-01-18 15:57:45.000000 AAIT25-0.0.3/orangecontrib/__init__.py
+-rw-rw-rw-   0        0        0       42 2024-05-23 17:56:17.469364 AAIT25-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1793 2024-05-23 17:55:57.000000 AAIT25-0.0.3/setup.py
```

### Comparing `AAIT25-0.0.2/setup.py` & `AAIT25-0.0.3/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,59 +1,62 @@
-#pypi-AgEIcHlwaS5vcmcCJGUzNzMyY2Y2LWI3NTAtNGI4Zi1iYzg1LWM3N2ZmMjk4NWFjNwACKlszLCIzMzliODczOC0yN2EwLTRlNzUtOGIwYi01ZTY3ZGQzNTJkOGEiXQAABiCSIWaaQx6SJ-eUbj6VSMw10g8Wt55CZldeWkw2whOk2Q
-
 from setuptools import setup, find_packages
 
-# Nom du package PyPI
+# Nom du package PyPI ('pip install NAME')
 NAME = "AAIT25"
 
 # Version du package PyPI
-VERSION = "0.0.2"  # la version doit être supérieure à la précédente sinon la publication sera refusée
+VERSION = "0.0.3" # la version doit être supérieure à la précédente sinon la publication sera refusée
 
 # Facultatif / Adaptable à souhait
-AUTHOR = "Orange community"
+AUTHOR = ""
 AUTHOR_EMAIL = ""
 URL = ""
-DESCRIPTION = ("Advanced Artificial Intelligence Tools is a package meant to develop "
-               "and enable advanced AI functionalities in Orange Data Mining.")
+DESCRIPTION = "LLM addons for Orange Data Mining !"
 LICENSE = ""
 
 # 'orange3 add-on' permet de rendre l'addon téléchargeable via l'interface addons d'Orange 
 KEYWORDS = ("orange3 add-on",)
 
 # Tous les packages python existants dans le projet
 PACKAGES = find_packages()
 
 # Fichiers additionnels aux fichiers .py (comme les icons ou des .ows)
-# PACKAGE_DATA = {
-# 	"orangecontrib.AAIT.widgets.base": ["designer/*", "icons/*"],
-# 	"orangecontrib.AAIT.widgets.encapsulation": ["designer/*", "icons/*"],
-# 	"orangecontrib.AAIT.widgets.llm": ["designer/*", "icons/*"],
-# 	"orangecontrib.AAIT.widgets.optimiser": ["designer/*", "icons/*"],
-# }
-#
+PACKAGE_DATA = {
+	"orangecontrib.AAIT.widgets": ["icons/*", "designer/*"], # contenu du dossier 'icons' situé dans 'orangecontrib/hkh_bot/widgets'
+	"orangecontrib.AAIT": ["examples/*"],
+}
+# /!\ les noms de fichier 'orangecontrib.hkh_bot.widgets' doivent correspondre à l'arborescence
 
 # Dépendances
 INSTALL_REQUIRES = ["sentence-transformers==2.5.1"]
 
 # Spécifie le dossier contenant les widgets et le nom de section qu'aura l'addon sur Orange
 ENTRY_POINTS = {
-    "orange.widgets": (
-        "AAIT = orangecontrib.AAIT.widgets",
-    )
+	"orange.widgets": (
+		"AAIT = orangecontrib.AAIT.widgets", # 'HKH-Bot' sera le nom de la section Orange contenant les widgets
+	)
 }
+# /!\ les noms de fichier 'orangecontrib.hkh_bot.widgets' doivent correspondre à l'arborescence
 
 NAMESPACE_PACKAGES = ["orangecontrib"]
 
 setup(name=NAME,
-      version=VERSION,
-      author=AUTHOR,
-      author_email=AUTHOR_EMAIL,
-      url=URL,
-      description=DESCRIPTION,
-      license=LICENSE,
-      keywords=KEYWORDS,
-      packages=PACKAGES,
-      # package_data=PACKAGE_DATA,
-      install_requires=INSTALL_REQUIRES,
-      entry_points=ENTRY_POINTS,
-      namespace_packages=NAMESPACE_PACKAGES,
-      )
+	  version=VERSION,
+	  author=AUTHOR,
+	  author_email=AUTHOR_EMAIL,
+	  url=URL,
+	  description=DESCRIPTION,
+	  license=LICENSE,
+	  keywords=KEYWORDS,
+	  packages=PACKAGES,
+	  package_data=PACKAGE_DATA,
+	  install_requires=INSTALL_REQUIRES,
+	  entry_points=ENTRY_POINTS,
+	  namespace_packages=NAMESPACE_PACKAGES,
+)
+
+
+
+
+
+
+
```

