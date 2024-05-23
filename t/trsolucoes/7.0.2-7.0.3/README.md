# Comparing `tmp/trsolucoes-7.0.2.tar.gz` & `tmp/trsolucoes-7.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trsolucoes-7.0.2.tar", last modified: Mon May 20 22:14:32 2024, max compression
+gzip compressed data, was "trsolucoes-7.0.3.tar", last modified: Thu May 23 12:56:30 2024, max compression
```

## Comparing `trsolucoes-7.0.2.tar` & `trsolucoes-7.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-20 22:14:32.460768 trsolucoes-7.0.2/
--rw-rw-rw-   0        0        0     1088 2024-05-19 21:10:17.000000 trsolucoes-7.0.2/LICENCE
--rw-rw-rw-   0        0        0     2508 2024-05-20 22:14:32.458715 trsolucoes-7.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2182 2024-05-19 21:25:05.000000 trsolucoes-7.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-20 22:14:32.452743 trsolucoes-7.0.2/selenium_helper/
--rw-rw-rw-   0        0        0       43 2024-05-19 21:10:17.000000 trsolucoes-7.0.2/selenium_helper/__init__.py
--rw-rw-rw-   0        0        0    13509 2024-05-20 22:11:44.000000 trsolucoes-7.0.2/selenium_helper/selenium_helper.py
--rw-rw-rw-   0        0        0       42 2024-05-20 22:14:32.460768 trsolucoes-7.0.2/setup.cfg
--rw-rw-rw-   0        0        0      543 2024-05-20 22:14:17.000000 trsolucoes-7.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-20 22:14:32.457384 trsolucoes-7.0.2/trsolucoes.egg-info/
--rw-rw-rw-   0        0        0     2508 2024-05-20 22:14:32.000000 trsolucoes-7.0.2/trsolucoes.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      225 2024-05-20 22:14:32.000000 trsolucoes-7.0.2/trsolucoes.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-20 22:14:32.000000 trsolucoes-7.0.2/trsolucoes.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-05-20 22:14:32.000000 trsolucoes-7.0.2/trsolucoes.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-23 12:56:30.051502 trsolucoes-7.0.3/
+-rw-rw-rw-   0        0        0     1088 2024-05-19 21:10:17.000000 trsolucoes-7.0.3/LICENCE
+-rw-rw-rw-   0        0        0     2508 2024-05-23 12:56:30.051502 trsolucoes-7.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2182 2024-05-19 21:25:05.000000 trsolucoes-7.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-23 12:56:30.046518 trsolucoes-7.0.3/selenium_helper/
+-rw-rw-rw-   0        0        0       58 2024-05-23 12:55:47.000000 trsolucoes-7.0.3/selenium_helper/__init__.py
+-rw-rw-rw-   0        0        0    13509 2024-05-20 22:11:44.000000 trsolucoes-7.0.3/selenium_helper/selenium_helper.py
+-rw-rw-rw-   0        0        0       42 2024-05-23 12:56:30.051502 trsolucoes-7.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      543 2024-05-23 12:56:22.000000 trsolucoes-7.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 12:56:30.049508 trsolucoes-7.0.3/trsolucoes.egg-info/
+-rw-rw-rw-   0        0        0     2508 2024-05-23 12:56:30.000000 trsolucoes-7.0.3/trsolucoes.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      225 2024-05-23 12:56:30.000000 trsolucoes-7.0.3/trsolucoes.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 12:56:30.000000 trsolucoes-7.0.3/trsolucoes.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-05-23 12:56:30.000000 trsolucoes-7.0.3/trsolucoes.egg-info/top_level.txt
```

### Comparing `trsolucoes-7.0.2/LICENCE` & `trsolucoes-7.0.3/LICENCE`

 * *Files identical despite different names*

### Comparing `trsolucoes-7.0.2/PKG-INFO` & `trsolucoes-7.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trsolucoes
-Version: 7.0.2
+Version: 7.0.3
 Summary: Um repositório não oficial de funções de auxilio para Selenium
 Author: Tainan Ramos
 Author-email: tainan@trsolucoes.com.br
 License: MIT License
 Keywords: trsolucoes
 Requires: selenium
 Description-Content-Type: text/markdown
```

### Comparing `trsolucoes-7.0.2/README.md` & `trsolucoes-7.0.3/README.md`

 * *Files identical despite different names*

### Comparing `trsolucoes-7.0.2/selenium_helper/selenium_helper.py` & `trsolucoes-7.0.3/selenium_helper/selenium_helper.py`

 * *Files identical despite different names*

### Comparing `trsolucoes-7.0.2/setup.py` & `trsolucoes-7.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="UTF-8") as arq:
     readme = arq.read()
 
 setup(name="trsolucoes",
-      version="7.0.2",
+      version="7.0.3",
       license="MIT License",
       author="Tainan Ramos",
       long_description=readme,
       long_description_content_type="text/markdown",
       author_email="tainan@trsolucoes.com.br",
       keywords="trsolucoes",
       description="Um repositório não oficial de funções de auxilio para Selenium",
```

### Comparing `trsolucoes-7.0.2/trsolucoes.egg-info/PKG-INFO` & `trsolucoes-7.0.3/trsolucoes.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trsolucoes
-Version: 7.0.2
+Version: 7.0.3
 Summary: Um repositório não oficial de funções de auxilio para Selenium
 Author: Tainan Ramos
 Author-email: tainan@trsolucoes.com.br
 License: MIT License
 Keywords: trsolucoes
 Requires: selenium
 Description-Content-Type: text/markdown
```

