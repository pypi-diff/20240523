# Comparing `tmp/jaanca-0.1.1.tar.gz` & `tmp/jaanca-0.1.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaanca-0.1.1.tar", last modified: Wed May 22 20:05:53 2024, max compression
+gzip compressed data, was "jaanca-0.1.2rc1.tar", last modified: Thu May 23 14:04:24 2024, max compression
```

## Comparing `jaanca-0.1.1.tar` & `jaanca-0.1.2rc1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 20:05:53.898531 jaanca-0.1.1/
--rw-rw-rw-   0        0        0     1092 2024-05-22 20:03:18.000000 jaanca-0.1.1/LICENSE.txt
--rw-rw-rw-   0        0        0     1412 2024-05-22 20:05:53.897529 jaanca-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      240 2024-05-22 01:20:56.000000 jaanca-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-22 20:05:53.880337 jaanca-0.1.1/jaanca/
--rw-rw-rw-   0        0        0       70 2024-05-22 00:33:46.000000 jaanca-0.1.1/jaanca/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 20:05:53.889819 jaanca-0.1.1/jaanca/utils/
--rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 jaanca-0.1.1/jaanca/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 20:05:53.893533 jaanca-0.1.1/jaanca/utils/helpers/
--rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 jaanca-0.1.1/jaanca/utils/helpers/__init__.py
--rw-rw-rw-   0        0        0     1537 2024-05-10 16:55:55.000000 jaanca-0.1.1/jaanca/utils/helpers/chronometer.py
-drwxrwxrwx   0        0        0        0 2024-05-22 20:05:53.895532 jaanca-0.1.1/jaanca.egg-info/
--rw-rw-rw-   0        0        0     1412 2024-05-22 20:05:53.000000 jaanca-0.1.1/jaanca.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      273 2024-05-22 20:05:53.000000 jaanca-0.1.1/jaanca.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 20:05:53.000000 jaanca-0.1.1/jaanca.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-22 20:05:53.000000 jaanca-0.1.1/jaanca.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-22 20:05:53.899531 jaanca-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1505 2024-05-22 20:05:26.000000 jaanca-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 14:04:24.488100 jaanca-0.1.2rc1/
+-rw-rw-rw-   0        0        0     1092 2024-05-22 20:03:18.000000 jaanca-0.1.2rc1/LICENSE.txt
+-rw-rw-rw-   0        0        0     1865 2024-05-23 14:04:24.487223 jaanca-0.1.2rc1/PKG-INFO
+-rw-rw-rw-   0        0        0      675 2024-05-23 14:01:38.000000 jaanca-0.1.2rc1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-23 14:04:24.470203 jaanca-0.1.2rc1/jaanca/
+-rw-rw-rw-   0        0        0       70 2024-05-22 00:33:46.000000 jaanca-0.1.2rc1/jaanca/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 14:04:24.479213 jaanca-0.1.2rc1/jaanca/utils/
+-rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 jaanca-0.1.2rc1/jaanca/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 14:04:24.483215 jaanca-0.1.2rc1/jaanca/utils/helpers/
+-rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 jaanca-0.1.2rc1/jaanca/utils/helpers/__init__.py
+-rw-rw-rw-   0        0        0     1537 2024-05-10 16:55:55.000000 jaanca-0.1.2rc1/jaanca/utils/helpers/chronometer.py
+drwxrwxrwx   0        0        0        0 2024-05-23 14:04:24.485217 jaanca-0.1.2rc1/jaanca.egg-info/
+-rw-rw-rw-   0        0        0     1865 2024-05-23 14:04:24.000000 jaanca-0.1.2rc1/jaanca.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      273 2024-05-23 14:04:24.000000 jaanca-0.1.2rc1/jaanca.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 14:04:24.000000 jaanca-0.1.2rc1/jaanca.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-23 14:04:24.000000 jaanca-0.1.2rc1/jaanca.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-23 14:04:24.489222 jaanca-0.1.2rc1/setup.cfg
+-rw-rw-rw-   0        0        0     1523 2024-05-23 13:59:12.000000 jaanca-0.1.2rc1/setup.py
```

### Comparing `jaanca-0.1.1/LICENSE.txt` & `jaanca-0.1.2rc1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jaanca-0.1.1/jaanca/utils/helpers/chronometer.py` & `jaanca-0.1.2rc1/jaanca/utils/helpers/chronometer.py`

 * *Files identical despite different names*

### Comparing `jaanca-0.1.1/setup.py` & `jaanca-0.1.2rc1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 #!/usr/bin/env python
 from setuptools import setup, find_packages
 
 COMPANY_NAME="jaanca"
 PACKAGE_NAME = "jaanca"
-VERSION = "0.1.1"
+VERSION = "0.1.2rc1"
 
 install_requires = []
 
 setup(
     name=PACKAGE_NAME,
     version=VERSION,
     description=f'A tool library created by {COMPANY_NAME}.',
     long_description=open('README.md', 'r').read(),
     long_description_content_type='text/markdown',
     license='MIT License',
-    author='Andres Cardona',
+    author='Jaime Andres Cardona Carrillo',
     author_email='jacardona@outlook.com',
     url='https://github.com/jaanca/python-libraries/tree/main/jaanca',
     keywords="python tools, libraries",
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "Intended Audience :: Information Technology",
```

