# Comparing `tmp/AAIT25-0.0.4.tar.gz` & `tmp/AAIT25-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AAIT25-0.0.4.tar", last modified: Thu May 23 17:58:56 2024, max compression
+gzip compressed data, was "AAIT25-0.0.5.tar", last modified: Thu May 23 18:01:26 2024, max compression
```

## Comparing `AAIT25-0.0.4.tar` & `AAIT25-0.0.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 17:58:56.301000 AAIT25-0.0.4/
-drwxrwxrwx   0        0        0        0 2024-05-23 17:58:56.293461 AAIT25-0.0.4/AAIT25.egg-info/
--rw-rw-rw-   0        0        0      236 2024-05-23 17:58:56.000000 AAIT25-0.0.4/AAIT25.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      818 2024-05-23 17:58:56.000000 AAIT25-0.0.4/AAIT25.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 17:58:56.000000 AAIT25-0.0.4/AAIT25.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2024-05-23 17:58:56.000000 AAIT25-0.0.4/AAIT25.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       14 2024-05-23 17:58:56.000000 AAIT25-0.0.4/AAIT25.egg-info/namespace_packages.txt
--rw-rw-rw-   0        0        0       29 2024-05-23 17:58:56.000000 AAIT25-0.0.4/AAIT25.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-23 17:58:56.000000 AAIT25-0.0.4/AAIT25.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2024-01-18 15:57:45.000000 AAIT25-0.0.4/License.txt
--rw-rw-rw-   0        0        0      236 2024-05-23 17:58:56.299998 AAIT25-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-01-18 15:57:45.000000 AAIT25-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-23 17:58:56.294462 AAIT25-0.0.4/orangecontrib/
--rw-rw-rw-   0        0        0       55 2024-01-18 15:57:45.000000 AAIT25-0.0.4/orangecontrib/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 17:58:56.295472 AAIT25-0.0.4/orangecontrib/aait/
--rw-rw-rw-   0        0        0        0 2024-01-18 15:57:45.000000 AAIT25-0.0.4/orangecontrib/aait/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 17:58:56.295472 AAIT25-0.0.4/orangecontrib/aait/examples/
--rw-rw-rw-   0        0        0     7856 2024-02-20 12:43:50.000000 AAIT25-0.0.4/orangecontrib/aait/examples/example-chatbot.ows
--rw-rw-rw-   0        0        0      966 2024-03-06 08:40:04.000000 AAIT25-0.0.4/orangecontrib/aait/execute_thread.py
-drwxrwxrwx   0        0        0        0 2024-05-23 17:58:56.296460 AAIT25-0.0.4/orangecontrib/aait/widgets/
--rw-rw-rw-   0        0        0        0 2024-01-18 15:57:45.000000 AAIT25-0.0.4/orangecontrib/aait/widgets/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 17:58:56.297466 AAIT25-0.0.4/orangecontrib/aait/widgets/designer/
--rw-rw-rw-   0        0        0     2337 2024-03-04 19:45:00.000000 AAIT25-0.0.4/orangecontrib/aait/widgets/designer/owchatbot.ui
-drwxrwxrwx   0        0        0        0 2024-05-23 17:58:56.299998 AAIT25-0.0.4/orangecontrib/aait/widgets/icons/
--rw-rw-rw-   0        0        0      831 2024-01-18 15:57:45.000000 AAIT25-0.0.4/orangecontrib/aait/widgets/icons/Chatbotpy.svg
--rw-rw-rw-   0        0        0     1596 2024-01-18 15:57:45.000000 AAIT25-0.0.4/orangecontrib/aait/widgets/icons/DocumentEater.svg
--rw-rw-rw-   0        0        0     4195 2024-01-18 15:57:45.000000 AAIT25-0.0.4/orangecontrib/aait/widgets/icons/Embeddings.svg
--rw-rw-rw-   0        0        0     1357 2024-01-18 15:57:45.000000 AAIT25-0.0.4/orangecontrib/aait/widgets/icons/LanguageModel.svg
--rw-rw-rw-   0        0        0      500 2024-01-18 15:57:45.000000 AAIT25-0.0.4/orangecontrib/aait/widgets/icons/TextPreprocessing.svg
--rw-rw-rw-   0        0        0     1082 2024-02-19 21:08:44.000000 AAIT25-0.0.4/orangecontrib/aait/widgets/icons/chatbot.svg
--rw-rw-rw-   0        0        0     8204 2024-03-12 21:47:18.000000 AAIT25-0.0.4/orangecontrib/aait/widgets/owchatbot.py
--rw-rw-rw-   0        0        0       42 2024-05-23 17:58:56.301000 AAIT25-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1793 2024-05-23 17:58:46.000000 AAIT25-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 18:01:26.265630 AAIT25-0.0.5/
+drwxrwxrwx   0        0        0        0 2024-05-23 18:01:26.257617 AAIT25-0.0.5/AAIT25.egg-info/
+-rw-rw-rw-   0        0        0      236 2024-05-23 18:01:26.000000 AAIT25-0.0.5/AAIT25.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      818 2024-05-23 18:01:26.000000 AAIT25-0.0.5/AAIT25.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 18:01:26.000000 AAIT25-0.0.5/AAIT25.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2024-05-23 18:01:26.000000 AAIT25-0.0.5/AAIT25.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       14 2024-05-23 18:01:26.000000 AAIT25-0.0.5/AAIT25.egg-info/namespace_packages.txt
+-rw-rw-rw-   0        0        0       29 2024-05-23 18:01:26.000000 AAIT25-0.0.5/AAIT25.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-23 18:01:26.000000 AAIT25-0.0.5/AAIT25.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2024-01-18 15:57:45.000000 AAIT25-0.0.5/License.txt
+-rw-rw-rw-   0        0        0      236 2024-05-23 18:01:26.264631 AAIT25-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-01-18 15:57:45.000000 AAIT25-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-23 18:01:26.257617 AAIT25-0.0.5/orangecontrib/
+-rw-rw-rw-   0        0        0       55 2024-01-18 15:57:45.000000 AAIT25-0.0.5/orangecontrib/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 18:01:26.258625 AAIT25-0.0.5/orangecontrib/aait/
+-rw-rw-rw-   0        0        0        0 2024-01-18 15:57:45.000000 AAIT25-0.0.5/orangecontrib/aait/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 18:01:26.259625 AAIT25-0.0.5/orangecontrib/aait/examples/
+-rw-rw-rw-   0        0        0     7856 2024-02-20 12:43:50.000000 AAIT25-0.0.5/orangecontrib/aait/examples/example-chatbot.ows
+-rw-rw-rw-   0        0        0      966 2024-03-06 08:40:04.000000 AAIT25-0.0.5/orangecontrib/aait/execute_thread.py
+drwxrwxrwx   0        0        0        0 2024-05-23 18:01:26.260632 AAIT25-0.0.5/orangecontrib/aait/widgets/
+-rw-rw-rw-   0        0        0        0 2024-01-18 15:57:45.000000 AAIT25-0.0.5/orangecontrib/aait/widgets/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 18:01:26.260632 AAIT25-0.0.5/orangecontrib/aait/widgets/designer/
+-rw-rw-rw-   0        0        0     2337 2024-03-04 19:45:00.000000 AAIT25-0.0.5/orangecontrib/aait/widgets/designer/owchatbot.ui
+drwxrwxrwx   0        0        0        0 2024-05-23 18:01:26.263631 AAIT25-0.0.5/orangecontrib/aait/widgets/icons/
+-rw-rw-rw-   0        0        0      831 2024-01-18 15:57:45.000000 AAIT25-0.0.5/orangecontrib/aait/widgets/icons/Chatbotpy.svg
+-rw-rw-rw-   0        0        0     1596 2024-01-18 15:57:45.000000 AAIT25-0.0.5/orangecontrib/aait/widgets/icons/DocumentEater.svg
+-rw-rw-rw-   0        0        0     4195 2024-01-18 15:57:45.000000 AAIT25-0.0.5/orangecontrib/aait/widgets/icons/Embeddings.svg
+-rw-rw-rw-   0        0        0     1357 2024-01-18 15:57:45.000000 AAIT25-0.0.5/orangecontrib/aait/widgets/icons/LanguageModel.svg
+-rw-rw-rw-   0        0        0      500 2024-01-18 15:57:45.000000 AAIT25-0.0.5/orangecontrib/aait/widgets/icons/TextPreprocessing.svg
+-rw-rw-rw-   0        0        0     1082 2024-02-19 21:08:44.000000 AAIT25-0.0.5/orangecontrib/aait/widgets/icons/chatbot.svg
+-rw-rw-rw-   0        0        0     8204 2024-03-12 21:47:18.000000 AAIT25-0.0.5/orangecontrib/aait/widgets/owchatbot.py
+-rw-rw-rw-   0        0        0       42 2024-05-23 18:01:26.265630 AAIT25-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1793 2024-05-23 18:01:21.000000 AAIT25-0.0.5/setup.py
```

### Comparing `AAIT25-0.0.4/AAIT25.egg-info/SOURCES.txt` & `AAIT25-0.0.5/AAIT25.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `AAIT25-0.0.4/orangecontrib/aait/examples/example-chatbot.ows` & `AAIT25-0.0.5/orangecontrib/aait/examples/example-chatbot.ows`

 * *Files identical despite different names*

### Comparing `AAIT25-0.0.4/orangecontrib/aait/execute_thread.py` & `AAIT25-0.0.5/orangecontrib/aait/execute_thread.py`

 * *Files identical despite different names*

### Comparing `AAIT25-0.0.4/orangecontrib/aait/widgets/designer/owchatbot.ui` & `AAIT25-0.0.5/orangecontrib/aait/widgets/designer/owchatbot.ui`

 * *Files identical despite different names*

### Comparing `AAIT25-0.0.4/orangecontrib/aait/widgets/icons/Chatbotpy.svg` & `AAIT25-0.0.5/orangecontrib/aait/widgets/icons/Chatbotpy.svg`

 * *Files identical despite different names*

### Comparing `AAIT25-0.0.4/orangecontrib/aait/widgets/icons/DocumentEater.svg` & `AAIT25-0.0.5/orangecontrib/aait/widgets/icons/DocumentEater.svg`

 * *Files identical despite different names*

### Comparing `AAIT25-0.0.4/orangecontrib/aait/widgets/icons/Embeddings.svg` & `AAIT25-0.0.5/orangecontrib/aait/widgets/icons/Embeddings.svg`

 * *Files identical despite different names*

### Comparing `AAIT25-0.0.4/orangecontrib/aait/widgets/icons/LanguageModel.svg` & `AAIT25-0.0.5/orangecontrib/aait/widgets/icons/LanguageModel.svg`

 * *Files identical despite different names*

### Comparing `AAIT25-0.0.4/orangecontrib/aait/widgets/icons/chatbot.svg` & `AAIT25-0.0.5/orangecontrib/aait/widgets/icons/chatbot.svg`

 * *Files identical despite different names*

### Comparing `AAIT25-0.0.4/orangecontrib/aait/widgets/owchatbot.py` & `AAIT25-0.0.5/orangecontrib/aait/widgets/owchatbot.py`

 * *Files identical despite different names*

### Comparing `AAIT25-0.0.4/setup.py` & `AAIT25-0.0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 # Nom du package PyPI ('pip install NAME')
 NAME = "AAIT25"
 
 # Version du package PyPI
-VERSION = "0.0.4" # la version doit être supérieure à la précédente sinon la publication sera refusée
+VERSION = "0.0.5" # la version doit être supérieure à la précédente sinon la publication sera refusée
 
 # Facultatif / Adaptable à souhait
 AUTHOR = ""
 AUTHOR_EMAIL = ""
 URL = ""
 DESCRIPTION = "LLM addons for Orange Data Mining !"
 LICENSE = ""
```

