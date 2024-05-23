# Comparing `tmp/local_text_summarizer-0.1.tar.gz` & `tmp/local_text_summarizer-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "local_text_summarizer-0.1.tar", last modified: Wed May 22 16:45:51 2024, max compression
+gzip compressed data, was "local_text_summarizer-0.2.tar", last modified: Thu May 23 18:53:02 2024, max compression
```

## Comparing `local_text_summarizer-0.1.tar` & `local_text_summarizer-0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 16:45:51.842359 local_text_summarizer-0.1/
--rw-rw-rw-   0        0        0       48 2024-05-22 16:17:10.000000 local_text_summarizer-0.1/LICENSE
--rw-rw-rw-   0        0        0      691 2024-05-22 16:45:51.839071 local_text_summarizer-0.1/PKG-INFO
--rw-rw-rw-   0        0        0      189 2024-05-22 16:34:26.000000 local_text_summarizer-0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-22 16:45:51.835888 local_text_summarizer-0.1/local_text_summarizer.egg-info/
--rw-rw-rw-   0        0        0      691 2024-05-22 16:45:51.000000 local_text_summarizer-0.1/local_text_summarizer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      367 2024-05-22 16:45:51.000000 local_text_summarizer-0.1/local_text_summarizer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 16:45:51.000000 local_text_summarizer-0.1/local_text_summarizer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2024-05-22 16:45:51.000000 local_text_summarizer-0.1/local_text_summarizer.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        5 2024-05-22 16:45:51.000000 local_text_summarizer-0.1/local_text_summarizer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2024-05-22 16:45:51.000000 local_text_summarizer-0.1/local_text_summarizer.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-22 16:45:51.831205 local_text_summarizer-0.1/locat_text_summarizer/
--rw-rw-rw-   0        0        0       38 2024-05-22 16:17:10.000000 local_text_summarizer-0.1/locat_text_summarizer/__init__.py
--rw-rw-rw-   0        0        0     2069 2024-05-22 16:18:07.000000 local_text_summarizer-0.1/locat_text_summarizer/summarize.py
--rw-rw-rw-   0        0        0       42 2024-05-22 16:45:51.842419 local_text_summarizer-0.1/setup.cfg
--rw-rw-rw-   0        0        0      780 2024-05-22 16:33:11.000000 local_text_summarizer-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 18:53:02.749340 local_text_summarizer-0.2/
+-rw-rw-rw-   0        0        0       48 2024-05-22 16:17:10.000000 local_text_summarizer-0.2/LICENSE
+-rw-rw-rw-   0        0        0     3152 2024-05-23 18:53:02.745342 local_text_summarizer-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2665 2024-05-23 18:52:47.000000 local_text_summarizer-0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-23 18:53:02.716356 local_text_summarizer-0.2/local_text_summarizer/
+-rw-rw-rw-   0        0        0       38 2024-05-22 16:17:10.000000 local_text_summarizer-0.2/local_text_summarizer/__init__.py
+-rw-rw-rw-   0        0        0     2069 2024-05-23 18:49:17.000000 local_text_summarizer-0.2/local_text_summarizer/summarize.py
+drwxrwxrwx   0        0        0        0 2024-05-23 18:53:02.743343 local_text_summarizer-0.2/local_text_summarizer.egg-info/
+-rw-rw-rw-   0        0        0     3152 2024-05-23 18:53:02.000000 local_text_summarizer-0.2/local_text_summarizer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      367 2024-05-23 18:53:02.000000 local_text_summarizer-0.2/local_text_summarizer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 18:53:02.000000 local_text_summarizer-0.2/local_text_summarizer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2024-05-23 18:53:02.000000 local_text_summarizer-0.2/local_text_summarizer.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        5 2024-05-23 18:53:02.000000 local_text_summarizer-0.2/local_text_summarizer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2024-05-23 18:53:02.000000 local_text_summarizer-0.2/local_text_summarizer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-23 18:53:02.749340 local_text_summarizer-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      780 2024-05-23 18:48:41.000000 local_text_summarizer-0.2/setup.py
```

### Comparing `local_text_summarizer-0.1/locat_text_summarizer/summarize.py` & `local_text_summarizer-0.2/local_text_summarizer/summarize.py`

 * *Files identical despite different names*

### Comparing `local_text_summarizer-0.1/setup.py` & `local_text_summarizer-0.2/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='local_text_summarizer',
-    version='0.1',
+    version='0.2',
     packages=find_packages(),
     install_requires=[
         'nltk',
     ],
     entry_points={
         'console_scripts': [
             'summarize=local_text_summarizer.summarize:main',
```

