# Comparing `tmp/jaanca-0.1.2rc1.tar.gz` & `tmp/jaanca-0.1.2rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaanca-0.1.2rc1.tar", last modified: Thu May 23 14:04:24 2024, max compression
+gzip compressed data, was "jaanca-0.1.2rc2.tar", last modified: Thu May 23 14:19:11 2024, max compression
```

## Comparing `jaanca-0.1.2rc1.tar` & `jaanca-0.1.2rc2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 14:04:24.488100 jaanca-0.1.2rc1/
--rw-rw-rw-   0        0        0     1092 2024-05-22 20:03:18.000000 jaanca-0.1.2rc1/LICENSE.txt
--rw-rw-rw-   0        0        0     1865 2024-05-23 14:04:24.487223 jaanca-0.1.2rc1/PKG-INFO
--rw-rw-rw-   0        0        0      675 2024-05-23 14:01:38.000000 jaanca-0.1.2rc1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-23 14:04:24.470203 jaanca-0.1.2rc1/jaanca/
--rw-rw-rw-   0        0        0       70 2024-05-22 00:33:46.000000 jaanca-0.1.2rc1/jaanca/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 14:04:24.479213 jaanca-0.1.2rc1/jaanca/utils/
--rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 jaanca-0.1.2rc1/jaanca/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 14:04:24.483215 jaanca-0.1.2rc1/jaanca/utils/helpers/
--rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 jaanca-0.1.2rc1/jaanca/utils/helpers/__init__.py
--rw-rw-rw-   0        0        0     1537 2024-05-10 16:55:55.000000 jaanca-0.1.2rc1/jaanca/utils/helpers/chronometer.py
-drwxrwxrwx   0        0        0        0 2024-05-23 14:04:24.485217 jaanca-0.1.2rc1/jaanca.egg-info/
--rw-rw-rw-   0        0        0     1865 2024-05-23 14:04:24.000000 jaanca-0.1.2rc1/jaanca.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      273 2024-05-23 14:04:24.000000 jaanca-0.1.2rc1/jaanca.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 14:04:24.000000 jaanca-0.1.2rc1/jaanca.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-23 14:04:24.000000 jaanca-0.1.2rc1/jaanca.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-23 14:04:24.489222 jaanca-0.1.2rc1/setup.cfg
--rw-rw-rw-   0        0        0     1523 2024-05-23 13:59:12.000000 jaanca-0.1.2rc1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 14:19:11.073271 jaanca-0.1.2rc2/
+-rw-rw-rw-   0        0        0     1092 2024-05-22 20:03:18.000000 jaanca-0.1.2rc2/LICENSE.txt
+-rw-rw-rw-   0        0        0     1957 2024-05-23 14:19:11.072273 jaanca-0.1.2rc2/PKG-INFO
+-rw-rw-rw-   0        0        0      767 2024-05-23 14:17:17.000000 jaanca-0.1.2rc2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-23 14:19:11.057272 jaanca-0.1.2rc2/jaanca/
+-rw-rw-rw-   0        0        0       70 2024-05-22 00:33:46.000000 jaanca-0.1.2rc2/jaanca/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 14:19:11.066272 jaanca-0.1.2rc2/jaanca/utils/
+-rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 jaanca-0.1.2rc2/jaanca/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 14:19:11.068271 jaanca-0.1.2rc2/jaanca/utils/helpers/
+-rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 jaanca-0.1.2rc2/jaanca/utils/helpers/__init__.py
+-rw-rw-rw-   0        0        0     1537 2024-05-10 16:55:55.000000 jaanca-0.1.2rc2/jaanca/utils/helpers/chronometer.py
+drwxrwxrwx   0        0        0        0 2024-05-23 14:19:11.071272 jaanca-0.1.2rc2/jaanca.egg-info/
+-rw-rw-rw-   0        0        0     1957 2024-05-23 14:19:11.000000 jaanca-0.1.2rc2/jaanca.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      273 2024-05-23 14:19:11.000000 jaanca-0.1.2rc2/jaanca.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 14:19:11.000000 jaanca-0.1.2rc2/jaanca.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-23 14:19:11.000000 jaanca-0.1.2rc2/jaanca.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-23 14:19:11.074274 jaanca-0.1.2rc2/setup.cfg
+-rw-rw-rw-   0        0        0     1523 2024-05-23 14:18:55.000000 jaanca-0.1.2rc2/setup.py
```

### Comparing `jaanca-0.1.2rc1/LICENSE.txt` & `jaanca-0.1.2rc2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jaanca-0.1.2rc1/PKG-INFO` & `jaanca-0.1.2rc2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaanca
-Version: 0.1.2rc1
+Version: 0.1.2rc2
 Summary: A tool library created by jaanca.
 Home-page: https://github.com/jaanca/python-libraries/tree/main/jaanca
 Author: Jaime Andres Cardona Carrillo
 Author-email: jacardona@outlook.com
 License: MIT License
 Keywords: python tools,libraries
 Classifier: Development Status :: 4 - Beta
@@ -39,16 +39,17 @@
     <img src="https://img.shields.io/badge/Python-%5B%3E%3D3.8%2C%3C%3D3.11%5D-blue" alt="Python">
 </a>
 </p>
 
 
 ---
 
-# What libraries
+#  A tool library created by jaanca
 
-* **Python library**: A tool library created by jaanca.
+[Source code](https://github.com/jaanca/python-libraries/tree/main/jaanca)
+| [Package (PyPI)](https://pypi.org/project/jaanca/)
 
 ---
 
 # Here is a non-exhaustive list of related packages:
 
 - [jaanca-chronometer](https://pypi.org/project/jaanca-chronometer/) : jaanca's helper chronometer
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: jaanca Version: 0.1.2rc1 Summary: A tool library
+Metadata-Version: 2.1 Name: jaanca Version: 0.1.2rc2 Summary: A tool library
 created by jaanca. Home-page: https://github.com/jaanca/python-libraries/tree/
 main/jaanca Author: Jaime Andres Cardona Carrillo Author-email:
 jacardona@outlook.com License: MIT License Keywords: python tools,libraries
 Classifier: Development Status :: 4 - Beta Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Information Technology Classifier:
 Intended Audience :: System Administrators Classifier: License :: OSI Approved
 :: MIT License Classifier: Operating System :: OS Independent Classifier:
@@ -12,10 +12,12 @@
 Python :: 3 Classifier: Programming Language :: Python Classifier: Topic ::
 Software Development :: Libraries :: Python Modules Classifier: Topic :: System
 :: Monitoring Classifier: Topic :: Software Development Classifier: Typing ::
 Typed Requires-Python: >=3.8 Description-Content-Type: text/markdown License-
 File: LICENSE.txt
                             jjaaaannccaa ppuubblliicc lliibbrraarriieess
                            _[_P_a_c_k_a_g_e_ _v_e_r_s_i_o_n_]_[_P_y_t_h_o_n_]
---- # What libraries * **Python library**: A tool library created by jaanca. --
-- # Here is a non-exhaustive list of related packages: - [jaanca-chronometer]
-(https://pypi.org/project/jaanca-chronometer/) : jaanca's helper chronometer
+--- # A tool library created by jaanca [Source code](https://github.com/jaanca/
+python-libraries/tree/main/jaanca) | [Package (PyPI)](https://pypi.org/project/
+jaanca/) --- # Here is a non-exhaustive list of related packages: - [jaanca-
+chronometer](https://pypi.org/project/jaanca-chronometer/) : jaanca's helper
+chronometer
```

### Comparing `jaanca-0.1.2rc1/README.md` & `jaanca-0.1.2rc2/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -10,16 +10,17 @@
     <img src="https://img.shields.io/badge/Python-%5B%3E%3D3.8%2C%3C%3D3.11%5D-blue" alt="Python">
 </a>
 </p>
 
 
 ---
 
-# What libraries
+#  A tool library created by jaanca
 
-* **Python library**: A tool library created by jaanca.
+[Source code](https://github.com/jaanca/python-libraries/tree/main/jaanca)
+| [Package (PyPI)](https://pypi.org/project/jaanca/)
 
 ---
 
 # Here is a non-exhaustive list of related packages:
 
 - [jaanca-chronometer](https://pypi.org/project/jaanca-chronometer/) : jaanca's helper chronometer
```

#### html2text {}

```diff
@@ -1,5 +1,7 @@
                             jjaaaannccaa ppuubblliicc lliibbrraarriieess
                            _[_P_a_c_k_a_g_e_ _v_e_r_s_i_o_n_]_[_P_y_t_h_o_n_]
---- # What libraries * **Python library**: A tool library created by jaanca. --
-- # Here is a non-exhaustive list of related packages: - [jaanca-chronometer]
-(https://pypi.org/project/jaanca-chronometer/) : jaanca's helper chronometer
+--- # A tool library created by jaanca [Source code](https://github.com/jaanca/
+python-libraries/tree/main/jaanca) | [Package (PyPI)](https://pypi.org/project/
+jaanca/) --- # Here is a non-exhaustive list of related packages: - [jaanca-
+chronometer](https://pypi.org/project/jaanca-chronometer/) : jaanca's helper
+chronometer
```

### Comparing `jaanca-0.1.2rc1/jaanca/utils/helpers/chronometer.py` & `jaanca-0.1.2rc2/jaanca/utils/helpers/chronometer.py`

 * *Files identical despite different names*

### Comparing `jaanca-0.1.2rc1/jaanca.egg-info/PKG-INFO` & `jaanca-0.1.2rc2/jaanca.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaanca
-Version: 0.1.2rc1
+Version: 0.1.2rc2
 Summary: A tool library created by jaanca.
 Home-page: https://github.com/jaanca/python-libraries/tree/main/jaanca
 Author: Jaime Andres Cardona Carrillo
 Author-email: jacardona@outlook.com
 License: MIT License
 Keywords: python tools,libraries
 Classifier: Development Status :: 4 - Beta
@@ -39,16 +39,17 @@
     <img src="https://img.shields.io/badge/Python-%5B%3E%3D3.8%2C%3C%3D3.11%5D-blue" alt="Python">
 </a>
 </p>
 
 
 ---
 
-# What libraries
+#  A tool library created by jaanca
 
-* **Python library**: A tool library created by jaanca.
+[Source code](https://github.com/jaanca/python-libraries/tree/main/jaanca)
+| [Package (PyPI)](https://pypi.org/project/jaanca/)
 
 ---
 
 # Here is a non-exhaustive list of related packages:
 
 - [jaanca-chronometer](https://pypi.org/project/jaanca-chronometer/) : jaanca's helper chronometer
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: jaanca Version: 0.1.2rc1 Summary: A tool library
+Metadata-Version: 2.1 Name: jaanca Version: 0.1.2rc2 Summary: A tool library
 created by jaanca. Home-page: https://github.com/jaanca/python-libraries/tree/
 main/jaanca Author: Jaime Andres Cardona Carrillo Author-email:
 jacardona@outlook.com License: MIT License Keywords: python tools,libraries
 Classifier: Development Status :: 4 - Beta Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Information Technology Classifier:
 Intended Audience :: System Administrators Classifier: License :: OSI Approved
 :: MIT License Classifier: Operating System :: OS Independent Classifier:
@@ -12,10 +12,12 @@
 Python :: 3 Classifier: Programming Language :: Python Classifier: Topic ::
 Software Development :: Libraries :: Python Modules Classifier: Topic :: System
 :: Monitoring Classifier: Topic :: Software Development Classifier: Typing ::
 Typed Requires-Python: >=3.8 Description-Content-Type: text/markdown License-
 File: LICENSE.txt
                             jjaaaannccaa ppuubblliicc lliibbrraarriieess
                            _[_P_a_c_k_a_g_e_ _v_e_r_s_i_o_n_]_[_P_y_t_h_o_n_]
---- # What libraries * **Python library**: A tool library created by jaanca. --
-- # Here is a non-exhaustive list of related packages: - [jaanca-chronometer]
-(https://pypi.org/project/jaanca-chronometer/) : jaanca's helper chronometer
+--- # A tool library created by jaanca [Source code](https://github.com/jaanca/
+python-libraries/tree/main/jaanca) | [Package (PyPI)](https://pypi.org/project/
+jaanca/) --- # Here is a non-exhaustive list of related packages: - [jaanca-
+chronometer](https://pypi.org/project/jaanca-chronometer/) : jaanca's helper
+chronometer
```

### Comparing `jaanca-0.1.2rc1/setup.py` & `jaanca-0.1.2rc2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup, find_packages
 
 COMPANY_NAME="jaanca"
 PACKAGE_NAME = "jaanca"
-VERSION = "0.1.2rc1"
+VERSION = "0.1.2rc2"
 
 install_requires = []
 
 setup(
     name=PACKAGE_NAME,
     version=VERSION,
     description=f'A tool library created by {COMPANY_NAME}.',
```

