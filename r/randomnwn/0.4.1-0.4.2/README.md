# Comparing `tmp/randomnwn-0.4.1.tar.gz` & `tmp/randomnwn-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "randomnwn-0.4.1.tar", last modified: Thu May  2 19:55:21 2024, max compression
+gzip compressed data, was "randomnwn-0.4.2.tar", last modified: Thu May 23 18:32:35 2024, max compression
```

## Comparing `randomnwn-0.4.1.tar` & `randomnwn-0.4.2.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:55:21.032698 randomnwn-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-02 19:55:14.000000 randomnwn-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-05-02 19:55:21.032698 randomnwn-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2190 2024-05-02 19:55:14.000000 randomnwn-0.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:55:21.032698 randomnwn-0.4.1/randomnwn/
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-02 19:55:14.000000 randomnwn-0.4.1/randomnwn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5077 2024-05-02 19:55:14.000000 randomnwn-0.4.1/randomnwn/_models.py
--rw-r--r--   0 runner    (1001) docker     (127)    13216 2024-05-02 19:55:14.000000 randomnwn-0.4.1/randomnwn/calculations.py
--rw-r--r--   0 runner    (1001) docker     (127)    11299 2024-05-02 19:55:14.000000 randomnwn-0.4.1/randomnwn/dynamics.py
--rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-05-02 19:55:14.000000 randomnwn-0.4.1/randomnwn/fromtext.py
--rw-r--r--   0 runner    (1001) docker     (127)     4165 2024-05-02 19:55:14.000000 randomnwn-0.4.1/randomnwn/line_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    15555 2024-05-02 19:55:14.000000 randomnwn-0.4.1/randomnwn/nanowires.py
--rw-r--r--   0 runner    (1001) docker     (127)     6168 2024-05-02 19:55:14.000000 randomnwn-0.4.1/randomnwn/plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-05-02 19:55:14.000000 randomnwn-0.4.1/randomnwn/units.py
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-02 19:55:14.000000 randomnwn-0.4.1/randomnwn/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:55:21.032698 randomnwn-0.4.1/randomnwn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-05-02 19:55:21.000000 randomnwn-0.4.1/randomnwn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-02 19:55:21.000000 randomnwn-0.4.1/randomnwn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 19:55:21.000000 randomnwn-0.4.1/randomnwn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-02 19:55:21.000000 randomnwn-0.4.1/randomnwn.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 19:55:21.032698 randomnwn-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-02 19:55:14.000000 randomnwn-0.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:55:21.032698 randomnwn-0.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-05-02 19:55:14.000000 randomnwn-0.4.1/tests/test_nanowires.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:32:35.427605 randomnwn-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-23 18:32:24.000000 randomnwn-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2816 2024-05-23 18:32:35.427605 randomnwn-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-05-23 18:32:24.000000 randomnwn-0.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:32:35.427605 randomnwn-0.4.2/randomnwn/
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-23 18:32:24.000000 randomnwn-0.4.2/randomnwn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5077 2024-05-23 18:32:24.000000 randomnwn-0.4.2/randomnwn/_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13216 2024-05-23 18:32:24.000000 randomnwn-0.4.2/randomnwn/calculations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11299 2024-05-23 18:32:24.000000 randomnwn-0.4.2/randomnwn/dynamics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3569 2024-05-23 18:32:24.000000 randomnwn-0.4.2/randomnwn/fromtext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4165 2024-05-23 18:32:24.000000 randomnwn-0.4.2/randomnwn/line_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15555 2024-05-23 18:32:24.000000 randomnwn-0.4.2/randomnwn/nanowires.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6168 2024-05-23 18:32:24.000000 randomnwn-0.4.2/randomnwn/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-05-23 18:32:24.000000 randomnwn-0.4.2/randomnwn/units.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-23 18:32:24.000000 randomnwn-0.4.2/randomnwn/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:32:35.427605 randomnwn-0.4.2/randomnwn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2816 2024-05-23 18:32:35.000000 randomnwn-0.4.2/randomnwn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-23 18:32:35.000000 randomnwn-0.4.2/randomnwn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 18:32:35.000000 randomnwn-0.4.2/randomnwn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-23 18:32:35.000000 randomnwn-0.4.2/randomnwn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-23 18:32:35.000000 randomnwn-0.4.2/randomnwn.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 18:32:35.427605 randomnwn-0.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-23 18:32:24.000000 randomnwn-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:32:35.427605 randomnwn-0.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-05-23 18:32:24.000000 randomnwn-0.4.2/tests/test_nanowires.py
```

### Comparing `randomnwn-0.4.1/PKG-INFO` & `randomnwn-0.4.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: randomnwn
-Version: 0.4.1
-Summary: Modelling and analyzing random nanowire networks in Python.
-Home-page: https://github.com/marcus-k/Random-NWNs
-Author: Marcus Kasdorf
-Author-email: marcus.kasdorf@ucalgary.ca
-License: MIT License
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Random NWNs [![Tests](https://github.com/marcus-k/Random-NWNs/actions/workflows/python-package.yml/badge.svg)](https://github.com/marcus-k/Random-NWNs/actions/workflows/python-package.yml)
 
 Python package for modelling and analyzing random nanowire networks. This package was a summer research project lasting from May 2021 to August 2021 under the supervision of Dr. Claudia Gomes da Rocha. 
 
 **Update:** This project will now be continuing as of May 2024. If you are using this project, please note there will be **active development** on it and the functionality may change.
 
 For future additions, feel free to fork the repository. Please cite Marcus Kasdorf if you wish to extend the project.
@@ -23,36 +11,38 @@
 * [Usage](#usage)
 * [Uninstallation](#uninstallation)
 
 # Installation
 
 Random NWNs can be installed from PyPI for quick use or installed manually for development.
 
-## Latest
+## Production
 
-The latest version can be installed from PyPI:
+The latest version of randomnwn can be installed from PyPI:
 
 `pip install randomnwn`
 
-## Development
-
-For convenience, one can use the `environment.yml` file with Anaconda to create a new
-virtual environment with all the required dependencies.
+An Anaconda environment file is also provided to create a new virtual 
+environment with the minimum required dependencies required to run the package.
 
-`conda env create -f environment.yml`
+`conda env create -n randomnwn -f environment.yml`
 
-This will create a new environment named `randomnwn`. To activate the environment, use:
+Be sure you activate the environment before using the package!
 
 `conda activate randomnwn`
 
-Then, to install the package, use pip. One can install the package in the usual way
-above, or install it in editable mode to allow for local development. Navigate to the 
-base folder and run:
+## Development
+
+One can use the `dev-environment.yml` file with Anaconda to create a new 
+virtual environment with all the required dependencies for development.
+
+`conda env create -n randomnwn -f dev-environment.yml`
 
-`pip install -e .`
+This will also install the randomnwn package in editable mode (i.e. as if 
+running `pip install -e .` in the base folder).
 
 # Usage
 
 Nanowire network objects are simply [NetworkX](https://github.com/networkx/networkx) graphs with various attributes stored in the graph, edges, and nodes.
 
 ```python
 >>> import randomnwn as rnwn
```

### Comparing `randomnwn-0.4.1/README.md` & `randomnwn-0.4.2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: randomnwn
+Version: 0.4.2
+Summary: Modelling and analyzing random nanowire networks in Python.
+Home-page: https://github.com/marcus-k/Random-NWNs
+Author: Marcus Kasdorf
+Author-email: marcus.kasdorf@ucalgary.ca
+License: MIT License
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: matplotlib>=3.8.4
+Requires-Dist: networkx>=3.1
+Requires-Dist: numpy>=1.26.4
+Requires-Dist: scipy>=1.13.0
+Requires-Dist: Shapely<3,>=2.0.4
+
 # Random NWNs [![Tests](https://github.com/marcus-k/Random-NWNs/actions/workflows/python-package.yml/badge.svg)](https://github.com/marcus-k/Random-NWNs/actions/workflows/python-package.yml)
 
 Python package for modelling and analyzing random nanowire networks. This package was a summer research project lasting from May 2021 to August 2021 under the supervision of Dr. Claudia Gomes da Rocha. 
 
 **Update:** This project will now be continuing as of May 2024. If you are using this project, please note there will be **active development** on it and the functionality may change.
 
 For future additions, feel free to fork the repository. Please cite Marcus Kasdorf if you wish to extend the project.
@@ -11,36 +28,38 @@
 * [Usage](#usage)
 * [Uninstallation](#uninstallation)
 
 # Installation
 
 Random NWNs can be installed from PyPI for quick use or installed manually for development.
 
-## Latest
+## Production
 
-The latest version can be installed from PyPI:
+The latest version of randomnwn can be installed from PyPI:
 
 `pip install randomnwn`
 
-## Development
-
-For convenience, one can use the `environment.yml` file with Anaconda to create a new
-virtual environment with all the required dependencies.
+An Anaconda environment file is also provided to create a new virtual 
+environment with the minimum required dependencies required to run the package.
 
-`conda env create -f environment.yml`
+`conda env create -n randomnwn -f environment.yml`
 
-This will create a new environment named `randomnwn`. To activate the environment, use:
+Be sure you activate the environment before using the package!
 
 `conda activate randomnwn`
 
-Then, to install the package, use pip. One can install the package in the usual way
-above, or install it in editable mode to allow for local development. Navigate to the 
-base folder and run:
+## Development
+
+One can use the `dev-environment.yml` file with Anaconda to create a new 
+virtual environment with all the required dependencies for development.
+
+`conda env create -n randomnwn -f dev-environment.yml`
 
-`pip install -e .`
+This will also install the randomnwn package in editable mode (i.e. as if 
+running `pip install -e .` in the base folder).
 
 # Usage
 
 Nanowire network objects are simply [NetworkX](https://github.com/networkx/networkx) graphs with various attributes stored in the graph, edges, and nodes.
 
 ```python
 >>> import randomnwn as rnwn
```

### Comparing `randomnwn-0.4.1/randomnwn/__init__.py` & `randomnwn-0.4.2/randomnwn/__init__.py`

 * *Files identical despite different names*

### Comparing `randomnwn-0.4.1/randomnwn/_models.py` & `randomnwn-0.4.2/randomnwn/_models.py`

 * *Files identical despite different names*

### Comparing `randomnwn-0.4.1/randomnwn/calculations.py` & `randomnwn-0.4.2/randomnwn/calculations.py`

 * *Files identical despite different names*

### Comparing `randomnwn-0.4.1/randomnwn/dynamics.py` & `randomnwn-0.4.2/randomnwn/dynamics.py`

 * *Files identical despite different names*

### Comparing `randomnwn-0.4.1/randomnwn/fromtext.py` & `randomnwn-0.4.2/randomnwn/fromtext.py`

 * *Files identical despite different names*

### Comparing `randomnwn-0.4.1/randomnwn/line_functions.py` & `randomnwn-0.4.2/randomnwn/line_functions.py`

 * *Files identical despite different names*

### Comparing `randomnwn-0.4.1/randomnwn/nanowires.py` & `randomnwn-0.4.2/randomnwn/nanowires.py`

 * *Files identical despite different names*

### Comparing `randomnwn-0.4.1/randomnwn/plotting.py` & `randomnwn-0.4.2/randomnwn/plotting.py`

 * *Files identical despite different names*

### Comparing `randomnwn-0.4.1/randomnwn/units.py` & `randomnwn-0.4.2/randomnwn/units.py`

 * *Files identical despite different names*

### Comparing `randomnwn-0.4.1/randomnwn.egg-info/PKG-INFO` & `randomnwn-0.4.2/randomnwn.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 Metadata-Version: 2.1
 Name: randomnwn
-Version: 0.4.1
+Version: 0.4.2
 Summary: Modelling and analyzing random nanowire networks in Python.
 Home-page: https://github.com/marcus-k/Random-NWNs
 Author: Marcus Kasdorf
 Author-email: marcus.kasdorf@ucalgary.ca
 License: MIT License
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: matplotlib>=3.8.4
+Requires-Dist: networkx>=3.1
+Requires-Dist: numpy>=1.26.4
+Requires-Dist: scipy>=1.13.0
+Requires-Dist: Shapely<3,>=2.0.4
 
 # Random NWNs [![Tests](https://github.com/marcus-k/Random-NWNs/actions/workflows/python-package.yml/badge.svg)](https://github.com/marcus-k/Random-NWNs/actions/workflows/python-package.yml)
 
 Python package for modelling and analyzing random nanowire networks. This package was a summer research project lasting from May 2021 to August 2021 under the supervision of Dr. Claudia Gomes da Rocha. 
 
 **Update:** This project will now be continuing as of May 2024. If you are using this project, please note there will be **active development** on it and the functionality may change.
 
@@ -23,36 +28,38 @@
 * [Usage](#usage)
 * [Uninstallation](#uninstallation)
 
 # Installation
 
 Random NWNs can be installed from PyPI for quick use or installed manually for development.
 
-## Latest
+## Production
 
-The latest version can be installed from PyPI:
+The latest version of randomnwn can be installed from PyPI:
 
 `pip install randomnwn`
 
-## Development
-
-For convenience, one can use the `environment.yml` file with Anaconda to create a new
-virtual environment with all the required dependencies.
+An Anaconda environment file is also provided to create a new virtual 
+environment with the minimum required dependencies required to run the package.
 
-`conda env create -f environment.yml`
+`conda env create -n randomnwn -f environment.yml`
 
-This will create a new environment named `randomnwn`. To activate the environment, use:
+Be sure you activate the environment before using the package!
 
 `conda activate randomnwn`
 
-Then, to install the package, use pip. One can install the package in the usual way
-above, or install it in editable mode to allow for local development. Navigate to the 
-base folder and run:
+## Development
+
+One can use the `dev-environment.yml` file with Anaconda to create a new 
+virtual environment with all the required dependencies for development.
+
+`conda env create -n randomnwn -f dev-environment.yml`
 
-`pip install -e .`
+This will also install the randomnwn package in editable mode (i.e. as if 
+running `pip install -e .` in the base folder).
 
 # Usage
 
 Nanowire network objects are simply [NetworkX](https://github.com/networkx/networkx) graphs with various attributes stored in the graph, edges, and nodes.
 
 ```python
 >>> import randomnwn as rnwn
```

### Comparing `randomnwn-0.4.1/setup.py` & `randomnwn-0.4.2/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -4,19 +4,26 @@
 with open("randomnwn/version.py", "r") as f:
     exec(f.read(), namespace)
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
-    name='randomnwn',
+    name="randomnwn",
     version=namespace["__version__"],    
-    description='Modelling and analyzing random nanowire networks in Python.',
+    description="Modelling and analyzing random nanowire networks in Python.",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url='https://github.com/marcus-k/Random-NWNs',
-    author='Marcus Kasdorf',
-    author_email='marcus.kasdorf@ucalgary.ca',
-    license='MIT License',
-    packages=['randomnwn'],
-    python_requires='>=3.10'
+    url="https://github.com/marcus-k/Random-NWNs",
+    author="Marcus Kasdorf",
+    author_email="marcus.kasdorf@ucalgary.ca",
+    license="MIT License",
+    packages=["randomnwn"],
+    python_requires=">=3.10",
+    install_requires=[
+        "matplotlib>=3.8.4",
+        "networkx>=3.1",
+        "numpy>=1.26.4",
+        "scipy>=1.13.0",
+        "Shapely>=2.0.4,<3",
+    ],
 )
```

### Comparing `randomnwn-0.4.1/tests/test_nanowires.py` & `randomnwn-0.4.2/tests/test_nanowires.py`

 * *Files identical despite different names*

