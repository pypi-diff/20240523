# Comparing `tmp/Taweret-1.0.1.tar.gz` & `tmp/taweret-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Taweret-1.0.1.tar", last modified: Mon Mar  4 21:23:46 2024, max compression
+gzip compressed data, was "taweret-1.0.2.tar", last modified: Thu May 23 01:40:48 2024, max compression
```

## Comparing `Taweret-1.0.1.tar` & `taweret-1.0.2.tar`

### file list

```diff
@@ -1,36 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 21:23:46.851205 Taweret-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-03-04 21:22:51.000000 Taweret-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6585 2024-03-04 21:23:46.851205 Taweret-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4213 2024-03-04 21:22:51.000000 Taweret-1.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-03-04 21:23:44.000000 Taweret-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-04 21:23:46.851205 Taweret-1.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 21:23:46.847205 Taweret-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 21:23:46.851205 Taweret-1.0.1/src/Taweret.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6585 2024-03-04 21:23:46.000000 Taweret-1.0.1/src/Taweret.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-03-04 21:23:46.000000 Taweret-1.0.1/src/Taweret.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-04 21:23:46.000000 Taweret-1.0.1/src/Taweret.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-03-04 21:23:46.000000 Taweret-1.0.1/src/Taweret.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-03-04 21:23:46.000000 Taweret-1.0.1/src/Taweret.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-03-04 21:22:51.000000 Taweret-1.0.1/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 21:23:46.847205 Taweret-1.0.1/src/core/
--rw-r--r--   0 runner    (1001) docker     (127)     7223 2024-03-04 21:22:51.000000 Taweret-1.0.1/src/core/base_mixer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-03-04 21:22:51.000000 Taweret-1.0.1/src/core/base_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4268 2024-03-04 21:22:51.000000 Taweret-1.0.1/src/core/trees_setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-03-04 21:22:51.000000 Taweret-1.0.1/src/core/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 21:23:46.847205 Taweret-1.0.1/src/mix/
--rw-r--r--   0 runner    (1001) docker     (127)    27836 2024-03-04 21:22:51.000000 Taweret-1.0.1/src/mix/bivariate_linear.py
--rw-r--r--   0 runner    (1001) docker     (127)     6450 2024-03-04 21:22:51.000000 Taweret-1.0.1/src/mix/gaussian.py
--rw-r--r--   0 runner    (1001) docker     (127)    40427 2024-03-04 21:22:51.000000 Taweret-1.0.1/src/mix/trees.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 21:23:46.851205 Taweret-1.0.1/src/models/
--rw-r--r--   0 runner    (1001) docker     (127)     7846 2024-03-04 21:22:51.000000 Taweret-1.0.1/src/models/coleman_models.py
--rw-r--r--   0 runner    (1001) docker     (127)    11054 2024-03-04 21:22:51.000000 Taweret-1.0.1/src/models/polynomial_models.py
--rw-r--r--   0 runner    (1001) docker     (127)    14713 2024-03-04 21:22:51.000000 Taweret-1.0.1/src/models/samba_models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 21:23:46.851205 Taweret-1.0.1/src/sampler/
--rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-03-04 21:22:51.000000 Taweret-1.0.1/src/sampler/likelihood_wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 21:23:46.851205 Taweret-1.0.1/src/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-03-04 21:22:51.000000 Taweret-1.0.1/src/utils/priors.py
--rw-r--r--   0 runner    (1001) docker     (127)    10017 2024-03-04 21:22:51.000000 Taweret-1.0.1/src/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 21:23:46.851205 Taweret-1.0.1/test/
--rw-r--r--   0 runner    (1001) docker     (127)     7707 2024-03-04 21:22:51.000000 Taweret-1.0.1/test/test_bivariate_linear.py
--rw-r--r--   0 runner    (1001) docker     (127)     4963 2024-03-04 21:22:51.000000 Taweret-1.0.1/test/test_gaussian.py
--rw-r--r--   0 runner    (1001) docker     (127)     4509 2024-03-04 21:22:51.000000 Taweret-1.0.1/test/test_trees.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:40:48.010551 taweret-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-05-23 01:40:42.000000 taweret-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7849 2024-05-23 01:40:48.010551 taweret-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5452 2024-05-23 01:40:42.000000 taweret-1.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-05-23 01:40:42.000000 taweret-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 01:40:48.010551 taweret-1.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:40:48.002550 taweret-1.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:40:48.002550 taweret-1.0.2/src/Taweret/
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-23 01:40:42.000000 taweret-1.0.2/src/Taweret/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:40:48.006551 taweret-1.0.2/src/Taweret/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 01:40:42.000000 taweret-1.0.2/src/Taweret/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6952 2024-05-23 01:40:42.000000 taweret-1.0.2/src/Taweret/core/base_mixer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2207 2024-05-23 01:40:42.000000 taweret-1.0.2/src/Taweret/core/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4268 2024-05-23 01:40:42.000000 taweret-1.0.2/src/Taweret/core/trees_setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2612 2024-05-23 01:40:42.000000 taweret-1.0.2/src/Taweret/core/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:40:48.006551 taweret-1.0.2/src/Taweret/mix/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 01:40:42.000000 taweret-1.0.2/src/Taweret/mix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27836 2024-05-23 01:40:42.000000 taweret-1.0.2/src/Taweret/mix/bivariate_linear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6450 2024-05-23 01:40:42.000000 taweret-1.0.2/src/Taweret/mix/gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40427 2024-05-23 01:40:42.000000 taweret-1.0.2/src/Taweret/mix/trees.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:40:48.006551 taweret-1.0.2/src/Taweret/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 01:40:42.000000 taweret-1.0.2/src/Taweret/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7846 2024-05-23 01:40:42.000000 taweret-1.0.2/src/Taweret/models/coleman_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11054 2024-05-23 01:40:42.000000 taweret-1.0.2/src/Taweret/models/polynomial_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14713 2024-05-23 01:40:42.000000 taweret-1.0.2/src/Taweret/models/samba_models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:40:48.006551 taweret-1.0.2/src/Taweret/sampler/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 01:40:42.000000 taweret-1.0.2/src/Taweret/sampler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-05-23 01:40:42.000000 taweret-1.0.2/src/Taweret/sampler/likelihood_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-05-23 01:40:42.000000 taweret-1.0.2/src/Taweret/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:40:48.006551 taweret-1.0.2/src/Taweret/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 01:40:42.000000 taweret-1.0.2/src/Taweret/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:40:48.006551 taweret-1.0.2/src/Taweret/tests/bart_bmm_test_data/
+-rw-r--r--   0 runner    (1001) docker     (127)    22955 2024-05-23 01:40:42.000000 taweret-1.0.2/src/Taweret/tests/bart_bmm_test_data/2d_pmean.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    45235 2024-05-23 01:40:42.000000 taweret-1.0.2/src/Taweret/tests/bart_bmm_test_data/2d_wmean.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 01:40:42.000000 taweret-1.0.2/src/Taweret/tests/bart_bmm_test_data/2d_x_test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-05-23 01:40:42.000000 taweret-1.0.2/src/Taweret/tests/bart_bmm_test_data/2d_x_train.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-23 01:40:42.000000 taweret-1.0.2/src/Taweret/tests/bart_bmm_test_data/2d_y_train.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    25058 2024-05-23 01:40:42.000000 taweret-1.0.2/src/Taweret/tests/samba_results.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7707 2024-05-23 01:40:42.000000 taweret-1.0.2/src/Taweret/tests/test_bivariate_linear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5089 2024-05-23 01:40:42.000000 taweret-1.0.2/src/Taweret/tests/test_gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4496 2024-05-23 01:40:42.000000 taweret-1.0.2/src/Taweret/tests/test_trees.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:40:48.006551 taweret-1.0.2/src/Taweret/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 01:40:42.000000 taweret-1.0.2/src/Taweret/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-05-23 01:40:42.000000 taweret-1.0.2/src/Taweret/utils/priors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10017 2024-05-23 01:40:42.000000 taweret-1.0.2/src/Taweret/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:40:48.010551 taweret-1.0.2/src/Taweret.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7849 2024-05-23 01:40:47.000000 taweret-1.0.2/src/Taweret.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-23 01:40:47.000000 taweret-1.0.2/src/Taweret.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 01:40:47.000000 taweret-1.0.2/src/Taweret.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-23 01:40:47.000000 taweret-1.0.2/src/Taweret.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-23 01:40:47.000000 taweret-1.0.2/src/Taweret.egg-info/top_level.txt
```

### Comparing `Taweret-1.0.1/LICENSE` & `taweret-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Taweret-1.0.1/PKG-INFO` & `taweret-1.0.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Taweret
-Version: 1.0.1
+Version: 1.0.2
 Summary: A python package for Bayesian model mixing
 Author-email: Kevin Ingles <kingles@illinois.edu>, "Dananjaya (Dan) Liyanage" <liyanage@osu.edu>, Alexandra Semposki <as727414@ohio.edu>, John Yannotty <yannotty.1@buckeyemail.osu.edu>
 License: MIT License
         
         Copyright (c) 2022 Dananjaya Liyanage, Alexandra Semposki, John Yannotty, Kevin Ingles
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -26,15 +26,15 @@
         SOFTWARE.
         
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Science/Research
-Requires-Python: >=3.10
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.20.3
 Requires-Dist: matplotlib
 Requires-Dist: scipy>=1.7.0
 Requires-Dist: seaborn
 Requires-Dist: emcee
@@ -45,18 +45,22 @@
 Requires-Dist: bilby
 Requires-Dist: ptemcee
 Requires-Dist: sphinx_rtd_theme
 Requires-Dist: sphinxcontrib-bibtex
 Requires-Dist: nbsphinx
 Requires-Dist: pandoc
 Requires-Dist: pytest
+Requires-Dist: pytest-cov
 Requires-Dist: Pyarrow
 Requires-Dist: openbtmixing
 
+
+
 # Taweret
+[![codecov](https://codecov.io/gh/bandframework/Taweret/graph/badge.svg?token=BQ7ZAD5ONP)](https://codecov.io/gh/bandframework/Taweret)
 
 <img align="right" width="200" src="logos/taweret_logo.PNG">
 
 Welcome to the GitHub repo for Taweret, the state of the art Python package for applying Bayesian Model Mixing! 
 
 ## About
 Taweret is a new generalized package to help with applying Bayesian model mixing methods, developed by members of the [BAND](https://bandframework.github.io/) collaboration, to a wide variety of problems in physics. 
@@ -112,14 +116,23 @@
 Taweret also depends on the OpenBT Mixing package in order to execute the trees modulde. This package is built with OpenMPI thus Windows users can work with the trees module using Windows Subsystem for Linux. Installation instructions are shown below.
 
 OpenBT will run within the Windows 10 Windows Subsystem for Linux (WSL) environment. For instructions on installing WSL,
 please see (https://ubuntu.com/wsl). We recommend installing the Ubuntu 20.04 WSL build. There are also instructions
 [here](https://wiki.ubuntu.com/WSL?action=subscribe&_ga=2.237944261.411635877.1601405226-783048612.1601405226#Installing_Packages_on_Ubuntu) 
 on keeping your Ubuntu WSL up to date, or installing additional features like X support. Once you have installed the WSL Ubuntu layer, start the WSL Ubuntu shell from the start menu and then you can begin working with Taweret.
 
+## Running on Codespaces
+GitHub's Codespaces is a great place to test using Taweret. Right now, you can try out Taweret's Bivariate Linear BMM and Multivariate BMM methods there, by following the instructions below. 
+
+1. Click the dropdown arrow on the green 'code' button found at the top of this page.
+2. Click on the tab there that says 'codespaces'.
+3. Click the button for 'create Codespace on main'.
+4. Wait for the terminal to be finish spinning up a virtual environment and loading all needed variables (this can take a few minutes).
+5. Once that is done, navigate on the file tree to a notebook you wish to run. To run a file, you need to set a kernel for the Jupyter notebook, so click on 'choose a kernel' in the upper right hand corner of the notebook. If you haven't gotten this message already, a message will pop up that says 'install preferred Python extension?', and you should click 'yes'.
+6. When you click 'choose a kernel' it will offer a preferred Python version or a base version (usually a newer Python version). Choose whichever you prefer, and then you can run the notebook!
 
 ## Citing Taweret
 If you have benefited from Taweret, please cite our software using the following format:
 
 ```
 @inproceedings{Taweret,
     author = "Liyanage, Dan and Semposki, Alexandra and Yannotty, John and Ingles, Kevin",
```

### Comparing `Taweret-1.0.1/README.md` & `taweret-1.0.2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,11 @@
+
+
 # Taweret
+[![codecov](https://codecov.io/gh/bandframework/Taweret/graph/badge.svg?token=BQ7ZAD5ONP)](https://codecov.io/gh/bandframework/Taweret)
 
 <img align="right" width="200" src="logos/taweret_logo.PNG">
 
 Welcome to the GitHub repo for Taweret, the state of the art Python package for applying Bayesian Model Mixing! 
 
 ## About
 Taweret is a new generalized package to help with applying Bayesian model mixing methods, developed by members of the [BAND](https://bandframework.github.io/) collaboration, to a wide variety of problems in physics. 
@@ -58,14 +61,23 @@
 Taweret also depends on the OpenBT Mixing package in order to execute the trees modulde. This package is built with OpenMPI thus Windows users can work with the trees module using Windows Subsystem for Linux. Installation instructions are shown below.
 
 OpenBT will run within the Windows 10 Windows Subsystem for Linux (WSL) environment. For instructions on installing WSL,
 please see (https://ubuntu.com/wsl). We recommend installing the Ubuntu 20.04 WSL build. There are also instructions
 [here](https://wiki.ubuntu.com/WSL?action=subscribe&_ga=2.237944261.411635877.1601405226-783048612.1601405226#Installing_Packages_on_Ubuntu) 
 on keeping your Ubuntu WSL up to date, or installing additional features like X support. Once you have installed the WSL Ubuntu layer, start the WSL Ubuntu shell from the start menu and then you can begin working with Taweret.
 
+## Running on Codespaces
+GitHub's Codespaces is a great place to test using Taweret. Right now, you can try out Taweret's Bivariate Linear BMM and Multivariate BMM methods there, by following the instructions below. 
+
+1. Click the dropdown arrow on the green 'code' button found at the top of this page.
+2. Click on the tab there that says 'codespaces'.
+3. Click the button for 'create Codespace on main'.
+4. Wait for the terminal to be finish spinning up a virtual environment and loading all needed variables (this can take a few minutes).
+5. Once that is done, navigate on the file tree to a notebook you wish to run. To run a file, you need to set a kernel for the Jupyter notebook, so click on 'choose a kernel' in the upper right hand corner of the notebook. If you haven't gotten this message already, a message will pop up that says 'install preferred Python extension?', and you should click 'yes'.
+6. When you click 'choose a kernel' it will offer a preferred Python version or a base version (usually a newer Python version). Choose whichever you prefer, and then you can run the notebook!
 
 ## Citing Taweret
 If you have benefited from Taweret, please cite our software using the following format:
 
 ```
 @inproceedings{Taweret,
     author = "Liyanage, Dan and Semposki, Alexandra and Yannotty, John and Ingles, Kevin",
```

### Comparing `Taweret-1.0.1/pyproject.toml` & `taweret-1.0.2/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
+[tool.setuptools.package-data]
+Taweret = ["tests/samba_results.txt", "tests/bart_bmm_test_data/2d_*.txt"]
 
 [project]
 name = "Taweret"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
     { name="Kevin Ingles", email="kingles@illinois.edu"},
     { name="Dananjaya (Dan) Liyanage", email="liyanage@osu.edu"},
     { name="Alexandra Semposki", email="as727414@ohio.edu"},
     { name="John Yannotty", email="yannotty.1@buckeyemail.osu.edu"},
 ]
 description = "A python package for Bayesian model mixing"
 readme = "README.md"
 license = {file = "LICENSE"}
-requires-python = ">=3.10"
+requires-python = ">=3.9"
 dependencies = [
     "numpy>=1.20.3",
     "matplotlib",
     "scipy>=1.7.0",
     "seaborn",
     "emcee",
     "corner",
@@ -29,14 +31,15 @@
     "bilby",
     "ptemcee",
     "sphinx_rtd_theme",
     "sphinxcontrib-bibtex",
     "nbsphinx",
     "pandoc",
     "pytest",
+    "pytest-cov",
     "Pyarrow",
     "openbtmixing",
 ]
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
```

### Comparing `Taweret-1.0.1/src/Taweret.egg-info/PKG-INFO` & `taweret-1.0.2/src/Taweret.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Taweret
-Version: 1.0.1
+Version: 1.0.2
 Summary: A python package for Bayesian model mixing
 Author-email: Kevin Ingles <kingles@illinois.edu>, "Dananjaya (Dan) Liyanage" <liyanage@osu.edu>, Alexandra Semposki <as727414@ohio.edu>, John Yannotty <yannotty.1@buckeyemail.osu.edu>
 License: MIT License
         
         Copyright (c) 2022 Dananjaya Liyanage, Alexandra Semposki, John Yannotty, Kevin Ingles
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -26,15 +26,15 @@
         SOFTWARE.
         
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Science/Research
-Requires-Python: >=3.10
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.20.3
 Requires-Dist: matplotlib
 Requires-Dist: scipy>=1.7.0
 Requires-Dist: seaborn
 Requires-Dist: emcee
@@ -45,18 +45,22 @@
 Requires-Dist: bilby
 Requires-Dist: ptemcee
 Requires-Dist: sphinx_rtd_theme
 Requires-Dist: sphinxcontrib-bibtex
 Requires-Dist: nbsphinx
 Requires-Dist: pandoc
 Requires-Dist: pytest
+Requires-Dist: pytest-cov
 Requires-Dist: Pyarrow
 Requires-Dist: openbtmixing
 
+
+
 # Taweret
+[![codecov](https://codecov.io/gh/bandframework/Taweret/graph/badge.svg?token=BQ7ZAD5ONP)](https://codecov.io/gh/bandframework/Taweret)
 
 <img align="right" width="200" src="logos/taweret_logo.PNG">
 
 Welcome to the GitHub repo for Taweret, the state of the art Python package for applying Bayesian Model Mixing! 
 
 ## About
 Taweret is a new generalized package to help with applying Bayesian model mixing methods, developed by members of the [BAND](https://bandframework.github.io/) collaboration, to a wide variety of problems in physics. 
@@ -112,14 +116,23 @@
 Taweret also depends on the OpenBT Mixing package in order to execute the trees modulde. This package is built with OpenMPI thus Windows users can work with the trees module using Windows Subsystem for Linux. Installation instructions are shown below.
 
 OpenBT will run within the Windows 10 Windows Subsystem for Linux (WSL) environment. For instructions on installing WSL,
 please see (https://ubuntu.com/wsl). We recommend installing the Ubuntu 20.04 WSL build. There are also instructions
 [here](https://wiki.ubuntu.com/WSL?action=subscribe&_ga=2.237944261.411635877.1601405226-783048612.1601405226#Installing_Packages_on_Ubuntu) 
 on keeping your Ubuntu WSL up to date, or installing additional features like X support. Once you have installed the WSL Ubuntu layer, start the WSL Ubuntu shell from the start menu and then you can begin working with Taweret.
 
+## Running on Codespaces
+GitHub's Codespaces is a great place to test using Taweret. Right now, you can try out Taweret's Bivariate Linear BMM and Multivariate BMM methods there, by following the instructions below. 
+
+1. Click the dropdown arrow on the green 'code' button found at the top of this page.
+2. Click on the tab there that says 'codespaces'.
+3. Click the button for 'create Codespace on main'.
+4. Wait for the terminal to be finish spinning up a virtual environment and loading all needed variables (this can take a few minutes).
+5. Once that is done, navigate on the file tree to a notebook you wish to run. To run a file, you need to set a kernel for the Jupyter notebook, so click on 'choose a kernel' in the upper right hand corner of the notebook. If you haven't gotten this message already, a message will pop up that says 'install preferred Python extension?', and you should click 'yes'.
+6. When you click 'choose a kernel' it will offer a preferred Python version or a base version (usually a newer Python version). Choose whichever you prefer, and then you can run the notebook!
 
 ## Citing Taweret
 If you have benefited from Taweret, please cite our software using the following format:
 
 ```
 @inproceedings{Taweret,
     author = "Liyanage, Dan and Semposki, Alexandra and Yannotty, John and Ingles, Kevin",
```

### Comparing `Taweret-1.0.1/src/core/base_mixer.py` & `taweret-1.0.2/src/Taweret/core/base_mixer.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,15 +34,14 @@
                         for i in range(len(self._model_list)):
                             value += self._model_list[i](
                                 x, model_parameters[i]
                             ) * weight[i]
                         return value
 
         """
-        return NotImplemented
 
     @abstractmethod
     def evaluate_weights(self):
         '''
         Calculate or sample a point estimate for model weights
 
         Returns:
@@ -60,26 +59,23 @@
                 class MyMixer(BaseMixer):
                     # . . .
                     def evaluate_weights(self, dirichlet_params):
                         return scipy.stats.dirichlet.rvs(dirichlet_params)
                     # . . .
 
         '''
-        return NotImplemented
 
     @property
     @abstractmethod
     def map(self):
         '''
         Stores the MAP values for the posterior distributions and is set
         during the self.train step
         '''
 
-        return NotImplemented
-
     @abstractmethod
     def predict(self):
         '''
         Evaluate posterior to make prediction at test points.
 
         Returns:
         --------
@@ -104,15 +100,14 @@
                     # . . .
                     def predict(self, x_test):
                         # work to calculate everything
                         # . . .
                         return posterior, means, credible_intervals, std_dev
 
         '''
-        return NotImplemented
 
     @abstractmethod
     def predict_weights(self):
         '''
         Calculate posterior predictive distribution for model weights
 
         Returns:
@@ -170,28 +165,26 @@
                 class MyMixer(BaseMixer):
                     # . . .
                     def prior_predict(self, x_test):
                         # work to calculate everything
                         # . . .
                         return prior, means, credible_intervals, std_dev
         '''
-        return NotImplemented
 
     @property
     @abstractmethod
     def posterior(self):
         '''
         Stores the most recent posteriors from running self.train function
 
         Returns:
         --------
         _posterior : np.ndarray
             posterior from learning the weights
         '''
-        return NotImplemented
 
     @property
     @abstractmethod
     def prior(self):
         '''
         Dictionary of prior distributions. Format should be compatible with
         sampler.
@@ -201,15 +194,14 @@
         _prior : Dict[str, Any]
             Underlying prior object(s)
 
         Example:
         --------
         Please consult ``BaseMixer.set_prior`` for an example
         '''
-        return NotImplemented
 
     @abstractmethod
     def set_prior(self):
         '''
         User must provide function that sets a member varibale called
         ``_prior``.
         Dictionary of prior distributions. Format should be compatible with
@@ -228,15 +220,14 @@
                 # creating a bilby prior dict
                 priors = dict()
                 priors['a'] = bilby.core.prior.MultivariateGaussian(mvg, 'a')
                 priors['b'] = bilby.core.prior.MultivariateGaussian(mvg, 'b')
                 m = MyMixer()
                 m.set_prior(prior_dict=priors)
       '''
-        return NotImplemented
 
     @abstractmethod
     def train(self):
         '''
         Run sampler to learn parameters. Method should also create class
         members that store the posterior and other diagnostic quantities
         import for plotting
@@ -244,8 +235,7 @@
         class
 
         Return:
         -------
         _posterior : np.ndarray
             the mcmc chain return from sampler
         '''
-        return NotImplemented
```

### Comparing `Taweret-1.0.1/src/core/base_model.py` & `taweret-1.0.2/src/Taweret/core/base_model.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,15 +26,14 @@
                     def model(self, the_model):
                         self._model = the_model
 
                     def evaluate(self, model_parameters):
                         return self._model(model_parameters)
                     # . . .
         '''
-        return NotImplemented
 
     @abstractmethod
     def log_likelihood_elementwise(self):
         r'''
         Calculate log_likelihood for array of points given, and return with
         array with same shape[0]
 
@@ -54,15 +53,14 @@
                     ):
                         # Assuming a normal distribution for error
                         y = self.evaluate(model_params)
                         # If y_exp, y_err, y are numpy arrays of same length
                         return np.exp(-(y - y_exp) **2 / (2 * y_err ** 2)) \
                             / np.sqrt(2 * np.pi * y_err ** 2))
         '''
-        return NotImplemented
 
     @abstractmethod
     def set_prior(self):
         '''
         User must provide function that sets a member varibale called _prior.
         Dictionary of prior distributions. Format should be compatible with
         sampler.
@@ -74,8 +72,7 @@
 
                 class MyModel(BaseMixer):
                     # . . .
                     def set_prior(self, prior_dict):
                         self._prior = prior_dict
                     # . . .
         '''
-        return NotImplemented
```

### Comparing `Taweret-1.0.1/src/core/trees_setup.py` & `taweret-1.0.2/src/Taweret/core/trees_setup.py`

 * *Files identical despite different names*

### Comparing `Taweret-1.0.1/src/core/wrappers.py` & `taweret-1.0.2/src/Taweret/core/wrappers.py`

 * *Files identical despite different names*

### Comparing `Taweret-1.0.1/src/mix/bivariate_linear.py` & `taweret-1.0.2/src/Taweret/mix/bivariate_linear.py`

 * *Files identical despite different names*

### Comparing `Taweret-1.0.1/src/mix/gaussian.py` & `taweret-1.0.2/src/Taweret/mix/gaussian.py`

 * *Files identical despite different names*

### Comparing `Taweret-1.0.1/src/mix/trees.py` & `taweret-1.0.2/src/Taweret/mix/trees.py`

 * *Files identical despite different names*

### Comparing `Taweret-1.0.1/src/models/coleman_models.py` & `taweret-1.0.2/src/Taweret/models/coleman_models.py`

 * *Files identical despite different names*

### Comparing `Taweret-1.0.1/src/models/polynomial_models.py` & `taweret-1.0.2/src/Taweret/models/polynomial_models.py`

 * *Files identical despite different names*

### Comparing `Taweret-1.0.1/src/models/samba_models.py` & `taweret-1.0.2/src/Taweret/models/samba_models.py`

 * *Files identical despite different names*

### Comparing `Taweret-1.0.1/src/sampler/likelihood_wrappers.py` & `taweret-1.0.2/src/Taweret/sampler/likelihood_wrappers.py`

 * *Files identical despite different names*

### Comparing `Taweret-1.0.1/src/utils/priors.py` & `taweret-1.0.2/src/Taweret/utils/priors.py`

 * *Files identical despite different names*

### Comparing `Taweret-1.0.1/src/utils/utils.py` & `taweret-1.0.2/src/Taweret/utils/utils.py`

 * *Files identical despite different names*

### Comparing `Taweret-1.0.1/test/test_bivariate_linear.py` & `taweret-1.0.2/src/Taweret/tests/test_bivariate_linear.py`

 * *Files identical despite different names*

### Comparing `Taweret-1.0.1/test/test_gaussian.py` & `taweret-1.0.2/src/Taweret/tests/test_gaussian.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,20 +2,21 @@
 # Testing file for gaussian.py (SAMBA multivariate BMM)
 # we can test both the samba_models and gaussian.py code
 # in this pytest script here
 # Author: Alexandra Semposki
 # Date: 03 April 2023
 ###########################################################
 
-import os
 import sys
+from pathlib import Path
 
 # Set Taweret Path
-dirname = os.popen("find $PWD -type f -name test_gaussian.py").read()
-taweret_wd = dirname.split("test")[0]
+dirname = Path(__file__).absolute()
+cwd = dirname.parent
+taweret_wd = str(dirname).split("test")[0]
 sys.path.append(taweret_wd)
 
 from Taweret.core.base_model import *
 from Taweret.core.base_mixer import *
 from Taweret.mix.gaussian import *
 from Taweret.models.samba_models import *
 import pytest
@@ -75,15 +76,16 @@
     assert np.array_equal(np.asarray(models["2"]), model_2), \
         "incorrect models['2'] values"
 
 
 def test_evaluate():
 
     # pull result from SAMBA to check against
-    samba_arrays = np.loadtxt('samba_results.txt', delimiter=',')
+    results_file = cwd / 'samba_results.txt'
+    samba_arrays = np.loadtxt(str(results_file), delimiter=',')
 
     # split up into arrays for each test
     samba_loworder = samba_arrays[0]
     samba_highorder = samba_arrays[1]
     samba_lowstd = samba_arrays[2]
     samba_highstd = samba_arrays[3]
 
@@ -112,15 +114,16 @@
     assert mixed.n_models == n_models, "class variable self.n_models not set"
     assert np.array_equal(mixed.x, g), "class variable self.x not set"
 
 
 def test_mixing():
 
     # call samba_results.txt file
-    samba_arrays = np.loadtxt('samba_results.txt', delimiter=',')
+    results_file = cwd / 'samba_results.txt'
+    samba_arrays = np.loadtxt(results_file, delimiter=',')
 
     # split up for these tests
     samba_mean = samba_arrays[4]
     samba_intervallow = samba_arrays[5]
     samba_intervalhigh = samba_arrays[6]
     samba_std = samba_arrays[7]
 
@@ -141,15 +144,16 @@
         "higher interval not matching"
     assert np.allclose(samba_std, std_dev), "standard deviation not matching"
 
 
 def test_evaluate_weights():
 
     # call samba_results.txt file
-    samba_arrays = np.loadtxt('samba_results.txt', delimiter=',')
+    results_file = cwd / 'samba_results.txt'
+    samba_arrays = np.loadtxt(results_file, delimiter=',')
 
     # separate out weights
     weights_low = samba_arrays[8]
     weights_high = samba_arrays[9]
 
     # test weights
     assert np.allclose(weights_low, mixed.var_weights[0, :]), \
```

### Comparing `Taweret-1.0.1/test/test_trees.py` & `taweret-1.0.2/src/Taweret/tests/test_trees.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 """
 # Imports
 import os
 import sys
 import numpy as np
 
+from pathlib import Path
 
 # Check for OpenMPI installation
 from subprocess import run as cmd
 from subprocess import CalledProcessError
 try:
     cmd(['mpirun', '--version', '>', '/dev/null'])
 except (CalledProcessError):
@@ -29,33 +30,34 @@
 sys.path.append(taweret_wd)
 
 
 from Taweret.models.polynomial_models import sin_cos_exp
 from Taweret.mix.trees import Trees
 
 
+_TEST_DATA = Path(__file__).parent.joinpath("bart_bmm_test_data").resolve()
+
+
 # ---------------------------------------------
 # Define the test functions
 # ---------------------------------------------
 # Test the constructor with the model set
 def test_init():
     # check passing of variables into Multivariate class
     assert mix.model_dict == model_dict, "class object self.model_dict not set."
     assert mix.nummodels == len(
         model_dict), "class object self.nummodels not set."
 
 
 # Test the mixing fun
 def test_mixing():
-    x_train = np.loadtxt(
-        taweret_wd + 'test/bart_bmm_test_data/2d_x_train.txt').reshape(80, 2)
+    x_train = np.loadtxt(_TEST_DATA.joinpath('2d_x_train.txt')).reshape(80, 2)
     x_train = x_train.reshape(2, 80).transpose()
 
-    y_train = np.loadtxt(
-        taweret_wd + 'test/bart_bmm_test_data/2d_y_train.txt').reshape(80, 1)
+    y_train = np.loadtxt(_TEST_DATA.joinpath('2d_y_train.txt')).reshape(80, 1)
 
     # Set prior information
     mix.set_prior(
         k=2.5,
         ntree=30,
         overallnu=5,
         overallsd=0.01,
@@ -94,17 +96,15 @@
     x1_test = np.outer(np.linspace(-3, 3, n_test), np.ones(n_test))
     x2_test = x1_test.copy().transpose()
     f0_test = (np.sin(x1_test) + np.cos(x2_test))
     x_test = np.array([x1_test.reshape(x1_test.size,),
                       x2_test.reshape(x1_test.size,)]).transpose()
 
     # Read in test results
-    pmean_test = np.loadtxt(
-        taweret_wd +
-        'test/bart_bmm_test_data/2d_pmean.txt')
+    pmean_test = np.loadtxt(_TEST_DATA.joinpath('2d_pmean.txt'))
     eps = 0.10
 
     # Get predictions
     ppost, pmean, pci, pstd = mix.predict(X=x_test, ci=0.95)
 
     # Test the values
     perr = np.mean(np.abs(pmean - pmean_test))
@@ -120,17 +120,15 @@
     x_test = np.array([x1_test.reshape(x1_test.size,),
                       x2_test.reshape(x1_test.size,)]).transpose()
 
     wpost, wmean, wci, wstd = mix.predict_weights(X=x_test, ci=0.95)
 
     # Read in test results
     wteps = 0.05
-    wmean_test = np.loadtxt(
-        taweret_wd +
-        'test/bart_bmm_test_data/2d_wmean.txt')
+    wmean_test = np.loadtxt(_TEST_DATA.joinpath('2d_wmean.txt'))
 
     # Test the values
     werr = np.mean(np.abs(wmean - wmean_test))
     assert werr < wteps, "Inaccurate weights."
 
 
 # Test sigma
```

