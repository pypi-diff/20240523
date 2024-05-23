# Comparing `tmp/jaanca-0.1.0.tar.gz` & `tmp/jaanca-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaanca-0.1.0.tar", last modified: Wed May 22 01:30:30 2024, max compression
+gzip compressed data, was "jaanca-0.1.1.tar", last modified: Wed May 22 20:05:53 2024, max compression
```

## Comparing `jaanca-0.1.0.tar` & `jaanca-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 01:30:30.041350 jaanca-0.1.0/
--rw-rw-rw-   0        0        0     1092 2024-04-23 14:32:08.000000 jaanca-0.1.0/LICENSE.txt
--rw-rw-rw-   0        0        0     1412 2024-05-22 01:30:30.040349 jaanca-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      240 2024-05-22 01:20:56.000000 jaanca-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-22 01:30:30.024632 jaanca-0.1.0/jaanca/
--rw-rw-rw-   0        0        0       70 2024-05-22 00:33:46.000000 jaanca-0.1.0/jaanca/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 01:30:30.032642 jaanca-0.1.0/jaanca/utils/
--rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 jaanca-0.1.0/jaanca/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 01:30:30.035641 jaanca-0.1.0/jaanca/utils/helpers/
--rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 jaanca-0.1.0/jaanca/utils/helpers/__init__.py
--rw-rw-rw-   0        0        0     1537 2024-05-10 16:55:55.000000 jaanca-0.1.0/jaanca/utils/helpers/chronometer.py
-drwxrwxrwx   0        0        0        0 2024-05-22 01:30:30.038348 jaanca-0.1.0/jaanca.egg-info/
--rw-rw-rw-   0        0        0     1412 2024-05-22 01:30:29.000000 jaanca-0.1.0/jaanca.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      273 2024-05-22 01:30:30.000000 jaanca-0.1.0/jaanca.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 01:30:29.000000 jaanca-0.1.0/jaanca.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-22 01:30:29.000000 jaanca-0.1.0/jaanca.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-22 01:30:30.042350 jaanca-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1505 2024-05-22 01:29:32.000000 jaanca-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 20:05:53.898531 jaanca-0.1.1/
+-rw-rw-rw-   0        0        0     1092 2024-05-22 20:03:18.000000 jaanca-0.1.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     1412 2024-05-22 20:05:53.897529 jaanca-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      240 2024-05-22 01:20:56.000000 jaanca-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-22 20:05:53.880337 jaanca-0.1.1/jaanca/
+-rw-rw-rw-   0        0        0       70 2024-05-22 00:33:46.000000 jaanca-0.1.1/jaanca/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 20:05:53.889819 jaanca-0.1.1/jaanca/utils/
+-rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 jaanca-0.1.1/jaanca/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 20:05:53.893533 jaanca-0.1.1/jaanca/utils/helpers/
+-rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 jaanca-0.1.1/jaanca/utils/helpers/__init__.py
+-rw-rw-rw-   0        0        0     1537 2024-05-10 16:55:55.000000 jaanca-0.1.1/jaanca/utils/helpers/chronometer.py
+drwxrwxrwx   0        0        0        0 2024-05-22 20:05:53.895532 jaanca-0.1.1/jaanca.egg-info/
+-rw-rw-rw-   0        0        0     1412 2024-05-22 20:05:53.000000 jaanca-0.1.1/jaanca.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      273 2024-05-22 20:05:53.000000 jaanca-0.1.1/jaanca.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 20:05:53.000000 jaanca-0.1.1/jaanca.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-22 20:05:53.000000 jaanca-0.1.1/jaanca.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-22 20:05:53.899531 jaanca-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1505 2024-05-22 20:05:26.000000 jaanca-0.1.1/setup.py
```

### Comparing `jaanca-0.1.0/LICENSE.txt` & `jaanca-0.1.1/LICENSE.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The MIT License (MIT)
 
-Copyright (c) 2023 Logyca
+Copyright (c) 2023 jaanca
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `jaanca-0.1.0/PKG-INFO` & `jaanca-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaanca
-Version: 0.1.0
+Version: 0.1.1
 Summary: A tool library created by jaanca.
 Home-page: https://github.com/jaanca/python-libraries/tree/main/jaanca
 Author: Andres Cardona
 Author-email: jacardona@outlook.com
 License: MIT License
 Keywords: python tools,libraries
 Classifier: Development Status :: 4 - Beta
```

### Comparing `jaanca-0.1.0/jaanca/utils/helpers/chronometer.py` & `jaanca-0.1.1/jaanca/utils/helpers/chronometer.py`

 * *Files identical despite different names*

### Comparing `jaanca-0.1.0/jaanca.egg-info/PKG-INFO` & `jaanca-0.1.1/jaanca.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaanca
-Version: 0.1.0
+Version: 0.1.1
 Summary: A tool library created by jaanca.
 Home-page: https://github.com/jaanca/python-libraries/tree/main/jaanca
 Author: Andres Cardona
 Author-email: jacardona@outlook.com
 License: MIT License
 Keywords: python tools,libraries
 Classifier: Development Status :: 4 - Beta
```

### Comparing `jaanca-0.1.0/setup.py` & `jaanca-0.1.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup, find_packages
 
 COMPANY_NAME="jaanca"
 PACKAGE_NAME = "jaanca"
-VERSION = "0.1.0"
+VERSION = "0.1.1"
 
 install_requires = []
 
 setup(
     name=PACKAGE_NAME,
     version=VERSION,
     description=f'A tool library created by {COMPANY_NAME}.',
```

