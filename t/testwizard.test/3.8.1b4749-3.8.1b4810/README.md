# Comparing `tmp/testwizard.test-3.8.1b4749.tar.gz` & `tmp/testwizard.test-3.8.1b4810.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testwizard.test-3.8.1b4749.tar", last modified: Tue Mar 19 15:01:38 2024, max compression
+gzip compressed data, was "testwizard.test-3.8.1b4810.tar", last modified: Wed Mar 27 12:56:24 2024, max compression
```

## Comparing `testwizard.test-3.8.1b4749.tar` & `testwizard.test-3.8.1b4810.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-03-19 15:01:38.037043 testwizard.test-3.8.1b4749/
--rw-rw-rw-   0        0        0        4 2024-03-19 15:00:53.000000 testwizard.test-3.8.1b4749/LICENSE.txt
--rw-rw-rw-   0        0        0     9250 2024-03-19 15:01:38.037043 testwizard.test-3.8.1b4749/PKG-INFO
--rw-rw-rw-   0        0        0     8733 2024-03-19 15:00:53.000000 testwizard.test-3.8.1b4749/README.md
--rw-rw-rw-   0        0        0       42 2024-03-19 15:01:38.037043 testwizard.test-3.8.1b4749/setup.cfg
--rw-rw-rw-   0        0        0      814 2024-03-19 15:01:37.000000 testwizard.test-3.8.1b4749/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-19 15:01:38.021420 testwizard.test-3.8.1b4749/testwizard/
-drwxrwxrwx   0        0        0        0 2024-03-19 15:01:38.037043 testwizard.test-3.8.1b4749/testwizard/test/
--rw-rw-rw-   0        0        0       79 2024-03-19 15:00:53.000000 testwizard.test-3.8.1b4749/testwizard/test/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-19 15:01:38.037043 testwizard.test-3.8.1b4749/testwizard.test.egg-info/
--rw-rw-rw-   0        0        0     9250 2024-03-19 15:01:37.000000 testwizard.test-3.8.1b4749/testwizard.test.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      252 2024-03-19 15:01:37.000000 testwizard.test-3.8.1b4749/testwizard.test.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-19 15:01:37.000000 testwizard.test-3.8.1b4749/testwizard.test.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2024-03-19 15:01:37.000000 testwizard.test-3.8.1b4749/testwizard.test.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-03-19 15:01:37.000000 testwizard.test-3.8.1b4749/testwizard.test.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-03-27 12:56:24.676350 testwizard.test-3.8.1b4810/
+-rw-rw-rw-   0        0        0        4 2024-03-27 12:55:37.000000 testwizard.test-3.8.1b4810/LICENSE.txt
+-rw-rw-rw-   0        0        0     9250 2024-03-27 12:56:24.676350 testwizard.test-3.8.1b4810/PKG-INFO
+-rw-rw-rw-   0        0        0     8733 2024-03-27 12:55:37.000000 testwizard.test-3.8.1b4810/README.md
+-rw-rw-rw-   0        0        0       42 2024-03-27 12:56:24.676350 testwizard.test-3.8.1b4810/setup.cfg
+-rw-rw-rw-   0        0        0      814 2024-03-27 12:56:24.000000 testwizard.test-3.8.1b4810/setup.py
+drwxrwxrwx   0        0        0        0 2024-03-27 12:56:24.660734 testwizard.test-3.8.1b4810/testwizard/
+drwxrwxrwx   0        0        0        0 2024-03-27 12:56:24.676350 testwizard.test-3.8.1b4810/testwizard/test/
+-rw-rw-rw-   0        0        0       79 2024-03-27 12:55:37.000000 testwizard.test-3.8.1b4810/testwizard/test/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-27 12:56:24.676350 testwizard.test-3.8.1b4810/testwizard.test.egg-info/
+-rw-rw-rw-   0        0        0     9250 2024-03-27 12:56:24.000000 testwizard.test-3.8.1b4810/testwizard.test.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      252 2024-03-27 12:56:24.000000 testwizard.test-3.8.1b4810/testwizard.test.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-03-27 12:56:24.000000 testwizard.test-3.8.1b4810/testwizard.test.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2024-03-27 12:56:24.000000 testwizard.test-3.8.1b4810/testwizard.test.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-03-27 12:56:24.000000 testwizard.test-3.8.1b4810/testwizard.test.egg-info/top_level.txt
```

### Comparing `testwizard.test-3.8.1b4749/PKG-INFO` & `testwizard.test-3.8.1b4810/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testwizard.test
-Version: 3.8.1b4749
+Version: 3.8.1b4810
 Summary: Testwizard test
 Home-page: https://www.resillion.com/services/software-testing/testing-tools/testwizard/
 Author: Resillion
 Author-email: testwizard-support@resillion.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.3
```

### Comparing `testwizard.test-3.8.1b4749/README.md` & `testwizard.test-3.8.1b4810/README.md`

 * *Files identical despite different names*

### Comparing `testwizard.test-3.8.1b4749/setup.py` & `testwizard.test-3.8.1b4810/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from setuptools import setup, find_namespace_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="testwizard.test",
-    version="3.8.1b4749",
+    version="3.8.1b4810",
     author="Resillion",
     author_email="testwizard-support@resillion.com",
     description="Testwizard test",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://www.resillion.com/services/software-testing/testing-tools/testwizard/",
     packages=find_namespace_packages(),
     install_requires=[
-          'testwizard.core==3.8.1b4749',
+          'testwizard.core==3.8.1b4810',
     ],
     classifiers=[
         "Programming Language :: Python :: 3.3",
         "Development Status :: 5 - Production/Stable",
         "Operating System :: OS Independent",
     ],
 )
```

### Comparing `testwizard.test-3.8.1b4749/testwizard.test.egg-info/PKG-INFO` & `testwizard.test-3.8.1b4810/testwizard.test.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testwizard.test
-Version: 3.8.1b4749
+Version: 3.8.1b4810
 Summary: Testwizard test
 Home-page: https://www.resillion.com/services/software-testing/testing-tools/testwizard/
 Author: Resillion
 Author-email: testwizard-support@resillion.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.3
```

