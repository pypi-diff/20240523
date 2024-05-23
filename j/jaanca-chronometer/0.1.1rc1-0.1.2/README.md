# Comparing `tmp/jaanca_chronometer-0.1.1rc1.tar.gz` & `tmp/jaanca_chronometer-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaanca_chronometer-0.1.1rc1.tar", last modified: Wed May 22 02:12:59 2024, max compression
+gzip compressed data, was "jaanca_chronometer-0.1.2.tar", last modified: Wed May 22 20:06:30 2024, max compression
```

## Comparing `jaanca_chronometer-0.1.1rc1.tar` & `jaanca_chronometer-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 02:12:59.041681 jaanca_chronometer-0.1.1rc1/
--rw-rw-rw-   0        0        0     1092 2024-04-23 14:32:08.000000 jaanca_chronometer-0.1.1rc1/LICENSE.txt
--rw-rw-rw-   0        0        0     4498 2024-05-22 02:12:59.040682 jaanca_chronometer-0.1.1rc1/PKG-INFO
--rw-rw-rw-   0        0        0     3205 2024-05-22 01:18:07.000000 jaanca_chronometer-0.1.1rc1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-22 02:12:59.022640 jaanca_chronometer-0.1.1rc1/jaanca_chronometer/
--rw-rw-rw-   0        0        0       70 2024-05-22 00:33:46.000000 jaanca_chronometer-0.1.1rc1/jaanca_chronometer/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 02:12:59.033789 jaanca_chronometer-0.1.1rc1/jaanca_chronometer/utils/
--rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 jaanca_chronometer-0.1.1rc1/jaanca_chronometer/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 02:12:59.036786 jaanca_chronometer-0.1.1rc1/jaanca_chronometer/utils/helpers/
--rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 jaanca_chronometer-0.1.1rc1/jaanca_chronometer/utils/helpers/__init__.py
--rw-rw-rw-   0        0        0     1651 2024-05-22 02:12:10.000000 jaanca_chronometer-0.1.1rc1/jaanca_chronometer/utils/helpers/chronometer.py
-drwxrwxrwx   0        0        0        0 2024-05-22 02:12:59.038681 jaanca_chronometer-0.1.1rc1/jaanca_chronometer.egg-info/
--rw-rw-rw-   0        0        0     4498 2024-05-22 02:12:58.000000 jaanca_chronometer-0.1.1rc1/jaanca_chronometer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      369 2024-05-22 02:12:59.000000 jaanca_chronometer-0.1.1rc1/jaanca_chronometer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 02:12:58.000000 jaanca_chronometer-0.1.1rc1/jaanca_chronometer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2024-05-22 02:12:58.000000 jaanca_chronometer-0.1.1rc1/jaanca_chronometer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-22 02:12:59.042682 jaanca_chronometer-0.1.1rc1/setup.cfg
--rw-rw-rw-   0        0        0     1627 2024-05-22 02:12:48.000000 jaanca_chronometer-0.1.1rc1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 20:06:30.126216 jaanca_chronometer-0.1.2/
+-rw-rw-rw-   0        0        0     1092 2024-05-22 20:03:29.000000 jaanca_chronometer-0.1.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     4589 2024-05-22 20:06:30.125218 jaanca_chronometer-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3299 2024-05-22 20:04:49.000000 jaanca_chronometer-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-22 20:06:30.109316 jaanca_chronometer-0.1.2/jaanca_chronometer/
+-rw-rw-rw-   0        0        0       70 2024-05-22 00:33:46.000000 jaanca_chronometer-0.1.2/jaanca_chronometer/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 20:06:30.118219 jaanca_chronometer-0.1.2/jaanca_chronometer/utils/
+-rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 jaanca_chronometer-0.1.2/jaanca_chronometer/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 20:06:30.121213 jaanca_chronometer-0.1.2/jaanca_chronometer/utils/helpers/
+-rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 jaanca_chronometer-0.1.2/jaanca_chronometer/utils/helpers/__init__.py
+-rw-rw-rw-   0        0        0     1651 2024-05-22 02:12:10.000000 jaanca_chronometer-0.1.2/jaanca_chronometer/utils/helpers/chronometer.py
+drwxrwxrwx   0        0        0        0 2024-05-22 20:06:30.123215 jaanca_chronometer-0.1.2/jaanca_chronometer.egg-info/
+-rw-rw-rw-   0        0        0     4589 2024-05-22 20:06:30.000000 jaanca_chronometer-0.1.2/jaanca_chronometer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      369 2024-05-22 20:06:30.000000 jaanca_chronometer-0.1.2/jaanca_chronometer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 20:06:30.000000 jaanca_chronometer-0.1.2/jaanca_chronometer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2024-05-22 20:06:30.000000 jaanca_chronometer-0.1.2/jaanca_chronometer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-22 20:06:30.127214 jaanca_chronometer-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1624 2024-05-22 20:05:36.000000 jaanca_chronometer-0.1.2/setup.py
```

### Comparing `jaanca_chronometer-0.1.1rc1/LICENSE.txt` & `jaanca_chronometer-0.1.2/LICENSE.txt`

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

### Comparing `jaanca_chronometer-0.1.1rc1/PKG-INFO` & `jaanca_chronometer-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaanca-chronometer
-Version: 0.1.1rc1
+Version: 0.1.2
 Summary: A tool library created by jaanca that allows measuring the time between two moments in the source code.
 Home-page: https://github.com/jaanca/python-libraries/tree/main/jaanca-chronometer
 Author: Andres Cardona
 Author-email: jacardona@outlook.com
 License: MIT License
 Keywords: timer stopwatch in interval format for databases
 Classifier: Development Status :: 4 - Beta
@@ -45,14 +45,16 @@
 ```python
 from jaanca_chronometer import Chronometer
 import time
 
 if __name__=="__main__":
     chronometer=Chronometer()
 
+    print(f"date_time format or interval format: {chronometer.get_format_time()}")
+
     chronometer.start()
     time.sleep(1)
     chronometer.stop()
     elapsed_time=str(chronometer.get_elapsed_time())
     print(elapsed_time)
 ```
 
@@ -77,15 +79,15 @@
 
 ```
 
 ---
 
 # Semantic Versioning
 
-logyca < MAJOR >.< MINOR >.< PATCH >
+jaanca-library < MAJOR >.< MINOR >.< PATCH >
 
 * **MAJOR**: version when you make incompatible API changes
 * **MINOR**: version when you add functionality in a backwards compatible manner
 * **PATCH**: version when you make backwards compatible bug fixes
 
 ## Definitions for releasing versions
 * https://peps.python.org/pep-0440/
@@ -114,10 +116,10 @@
 
 ## [0.0.1rcX] - 2024-05-21
 ### Added
 - First tests using pypi.org in develop environment.
 - Examples of use are added to the documentation of the functions in docstring
 - In the samples folder of this library, there are complete working examples of using the code.
 
-## [0.1.0] - 2024-05-21
+## [0.1.X] - 2024-05-21
 ### Added
 - Completion of testing and launch into production.
```

### Comparing `jaanca_chronometer-0.1.1rc1/README.md` & `jaanca_chronometer-0.1.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 ```python
 from jaanca_chronometer import Chronometer
 import time
 
 if __name__=="__main__":
     chronometer=Chronometer()
 
+    print(f"date_time format or interval format: {chronometer.get_format_time()}")
+
     chronometer.start()
     time.sleep(1)
     chronometer.stop()
     elapsed_time=str(chronometer.get_elapsed_time())
     print(elapsed_time)
 ```
 
@@ -48,15 +50,15 @@
 
 ```
 
 ---
 
 # Semantic Versioning
 
-logyca < MAJOR >.< MINOR >.< PATCH >
+jaanca-library < MAJOR >.< MINOR >.< PATCH >
 
 * **MAJOR**: version when you make incompatible API changes
 * **MINOR**: version when you add functionality in a backwards compatible manner
 * **PATCH**: version when you make backwards compatible bug fixes
 
 ## Definitions for releasing versions
 * https://peps.python.org/pep-0440/
@@ -85,10 +87,10 @@
 
 ## [0.0.1rcX] - 2024-05-21
 ### Added
 - First tests using pypi.org in develop environment.
 - Examples of use are added to the documentation of the functions in docstring
 - In the samples folder of this library, there are complete working examples of using the code.
 
-## [0.1.0] - 2024-05-21
+## [0.1.X] - 2024-05-21
 ### Added
 - Completion of testing and launch into production.
```

### Comparing `jaanca_chronometer-0.1.1rc1/jaanca_chronometer/utils/helpers/chronometer.py` & `jaanca_chronometer-0.1.2/jaanca_chronometer/utils/helpers/chronometer.py`

 * *Files identical despite different names*

### Comparing `jaanca_chronometer-0.1.1rc1/jaanca_chronometer.egg-info/PKG-INFO` & `jaanca_chronometer-0.1.2/jaanca_chronometer.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaanca-chronometer
-Version: 0.1.1rc1
+Version: 0.1.2
 Summary: A tool library created by jaanca that allows measuring the time between two moments in the source code.
 Home-page: https://github.com/jaanca/python-libraries/tree/main/jaanca-chronometer
 Author: Andres Cardona
 Author-email: jacardona@outlook.com
 License: MIT License
 Keywords: timer stopwatch in interval format for databases
 Classifier: Development Status :: 4 - Beta
@@ -45,14 +45,16 @@
 ```python
 from jaanca_chronometer import Chronometer
 import time
 
 if __name__=="__main__":
     chronometer=Chronometer()
 
+    print(f"date_time format or interval format: {chronometer.get_format_time()}")
+
     chronometer.start()
     time.sleep(1)
     chronometer.stop()
     elapsed_time=str(chronometer.get_elapsed_time())
     print(elapsed_time)
 ```
 
@@ -77,15 +79,15 @@
 
 ```
 
 ---
 
 # Semantic Versioning
 
-logyca < MAJOR >.< MINOR >.< PATCH >
+jaanca-library < MAJOR >.< MINOR >.< PATCH >
 
 * **MAJOR**: version when you make incompatible API changes
 * **MINOR**: version when you add functionality in a backwards compatible manner
 * **PATCH**: version when you make backwards compatible bug fixes
 
 ## Definitions for releasing versions
 * https://peps.python.org/pep-0440/
@@ -114,10 +116,10 @@
 
 ## [0.0.1rcX] - 2024-05-21
 ### Added
 - First tests using pypi.org in develop environment.
 - Examples of use are added to the documentation of the functions in docstring
 - In the samples folder of this library, there are complete working examples of using the code.
 
-## [0.1.0] - 2024-05-21
+## [0.1.X] - 2024-05-21
 ### Added
 - Completion of testing and launch into production.
```

### Comparing `jaanca_chronometer-0.1.1rc1/setup.py` & `jaanca_chronometer-0.1.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup, find_packages
 
 COMPANY_NAME="jaanca"
 PACKAGE_NAME = "jaanca-chronometer"
-VERSION = "0.1.1rc1"
+VERSION = "0.1.2"
 
 install_requires = []
 
 setup(
     name=PACKAGE_NAME,
     version=VERSION,
     description=f'A tool library created by {COMPANY_NAME} that allows measuring the time between two moments in the source code.',
```

