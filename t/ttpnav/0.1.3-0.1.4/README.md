# Comparing `tmp/ttpnav-0.1.3.tar.gz` & `tmp/ttpnav-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ttpnav-0.1.3.tar", last modified: Wed May 22 23:19:24 2024, max compression
+gzip compressed data, was "ttpnav-0.1.4.tar", last modified: Wed May 22 23:21:14 2024, max compression
```

## Comparing `ttpnav-0.1.3.tar` & `ttpnav-0.1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 23:19:24.839523 ttpnav-0.1.3/
--rw-rw-rw-   0        0        0     1089 2024-05-21 20:42:38.000000 ttpnav-0.1.3/LICENSE
--rw-rw-rw-   0        0        0    20865 2024-05-22 23:19:24.839523 ttpnav-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0    20368 2024-05-22 23:16:04.000000 ttpnav-0.1.3/README.md
--rw-rw-rw-   0        0        0       42 2024-05-22 23:19:24.840521 ttpnav-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      750 2024-05-22 21:57:34.000000 ttpnav-0.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-22 23:19:24.823521 ttpnav-0.1.3/tests/
--rw-rw-rw-   0        0        0        0 2024-05-20 19:55:46.000000 ttpnav-0.1.3/tests/__init__.py
--rw-rw-rw-   0        0        0    11081 2024-05-22 23:13:14.000000 ttpnav-0.1.3/tests/test_mitre_data.py
-drwxrwxrwx   0        0        0        0 2024-05-22 23:19:24.824520 ttpnav-0.1.3/ttpnav/
--rw-rw-rw-   0        0        0       33 2024-05-20 19:53:09.000000 ttpnav-0.1.3/ttpnav/__init__.py
--rw-rw-rw-   0        0        0    12649 2024-05-21 19:55:24.000000 ttpnav-0.1.3/ttpnav/mitre_data.py
-drwxrwxrwx   0        0        0        0 2024-05-22 23:19:24.838522 ttpnav-0.1.3/ttpnav.egg-info/
--rw-rw-rw-   0        0        0    20865 2024-05-22 23:19:24.000000 ttpnav-0.1.3/ttpnav.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2024-05-22 23:19:24.000000 ttpnav-0.1.3/ttpnav.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 23:19:24.000000 ttpnav-0.1.3/ttpnav.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2024-05-22 23:19:24.000000 ttpnav-0.1.3/ttpnav.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-22 23:19:24.000000 ttpnav-0.1.3/ttpnav.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-22 23:21:14.349285 ttpnav-0.1.4/
+-rw-rw-rw-   0        0        0     1089 2024-05-21 20:42:38.000000 ttpnav-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0    20865 2024-05-22 23:21:14.348285 ttpnav-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0    20368 2024-05-22 23:16:04.000000 ttpnav-0.1.4/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-22 23:21:14.349285 ttpnav-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      750 2024-05-22 23:21:12.000000 ttpnav-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 23:21:14.334284 ttpnav-0.1.4/tests/
+-rw-rw-rw-   0        0        0        0 2024-05-20 19:55:46.000000 ttpnav-0.1.4/tests/__init__.py
+-rw-rw-rw-   0        0        0    11081 2024-05-22 23:13:14.000000 ttpnav-0.1.4/tests/test_mitre_data.py
+drwxrwxrwx   0        0        0        0 2024-05-22 23:21:14.336284 ttpnav-0.1.4/ttpnav/
+-rw-rw-rw-   0        0        0       33 2024-05-20 19:53:09.000000 ttpnav-0.1.4/ttpnav/__init__.py
+-rw-rw-rw-   0        0        0    12649 2024-05-21 19:55:24.000000 ttpnav-0.1.4/ttpnav/mitre_data.py
+drwxrwxrwx   0        0        0        0 2024-05-22 23:21:14.348285 ttpnav-0.1.4/ttpnav.egg-info/
+-rw-rw-rw-   0        0        0    20865 2024-05-22 23:21:14.000000 ttpnav-0.1.4/ttpnav.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2024-05-22 23:21:14.000000 ttpnav-0.1.4/ttpnav.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 23:21:14.000000 ttpnav-0.1.4/ttpnav.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2024-05-22 23:21:14.000000 ttpnav-0.1.4/ttpnav.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-22 23:21:14.000000 ttpnav-0.1.4/ttpnav.egg-info/top_level.txt
```

### Comparing `ttpnav-0.1.3/LICENSE` & `ttpnav-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ttpnav-0.1.3/PKG-INFO` & `ttpnav-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ttpnav
-Version: 0.1.3
+Version: 0.1.4
 Summary: A package to navigate MITRE ATT&CK data easily.
 Home-page: https://github.com/fish-not-phish/ttpnav
 Author: Joseph Fisher
 Author-email: jfisher@cyntel.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ttpnav-0.1.3/README.md` & `ttpnav-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `ttpnav-0.1.3/setup.py` & `ttpnav-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="ttpnav",
-    version="0.1.3",
+    version="0.1.4",
     author="Joseph Fisher",
     author_email="jfisher@cyntel.com",
     description="A package to navigate MITRE ATT&CK data easily.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/fish-not-phish/ttpnav",
     packages=find_packages(),
```

### Comparing `ttpnav-0.1.3/tests/test_mitre_data.py` & `ttpnav-0.1.4/tests/test_mitre_data.py`

 * *Files identical despite different names*

### Comparing `ttpnav-0.1.3/ttpnav/mitre_data.py` & `ttpnav-0.1.4/ttpnav/mitre_data.py`

 * *Files identical despite different names*

### Comparing `ttpnav-0.1.3/ttpnav.egg-info/PKG-INFO` & `ttpnav-0.1.4/ttpnav.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ttpnav
-Version: 0.1.3
+Version: 0.1.4
 Summary: A package to navigate MITRE ATT&CK data easily.
 Home-page: https://github.com/fish-not-phish/ttpnav
 Author: Joseph Fisher
 Author-email: jfisher@cyntel.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

