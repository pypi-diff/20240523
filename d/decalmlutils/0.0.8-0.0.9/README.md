# Comparing `tmp/decalmlutils-0.0.8.tar.gz` & `tmp/decalmlutils-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decalmlutils-0.0.8.tar", last modified: Thu May 23 16:52:25 2024, max compression
+gzip compressed data, was "decalmlutils-0.0.9.tar", last modified: Thu May 23 17:05:55 2024, max compression
```

## Comparing `decalmlutils-0.0.8.tar` & `decalmlutils-0.0.9.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2024-05-23 16:52:25.120402 decalmlutils-0.0.8/
--rw-rw-r--   0 richard   (1000) richard   (1000)    11358 2024-02-14 15:27:04.000000 decalmlutils-0.0.8/LICENSE
--rw-r--r--   0 richard   (1000) richard   (1000)     6350 2024-05-23 16:52:25.120402 decalmlutils-0.0.8/PKG-INFO
--rw-rw-r--   0 richard   (1000) richard   (1000)     2117 2024-05-10 21:20:37.000000 decalmlutils-0.0.8/README.md
-drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2024-05-23 16:52:25.116402 decalmlutils-0.0.8/decalmlutils/
--rw-rw-r--   0 richard   (1000) richard   (1000)      306 2024-05-23 16:52:08.000000 decalmlutils-0.0.8/decalmlutils/__init__.py
--rw-rw-r--   0 richard   (1000) richard   (1000)      659 2024-05-10 21:26:05.000000 decalmlutils-0.0.8/decalmlutils/dataframes.py
--rw-rw-r--   0 richard   (1000) richard   (1000)    22461 2024-05-10 18:40:47.000000 decalmlutils-0.0.8/decalmlutils/debug_info.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     2119 2024-02-16 14:37:48.000000 decalmlutils-0.0.8/decalmlutils/geom.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     2042 2024-05-23 14:29:50.000000 decalmlutils-0.0.8/decalmlutils/logging_utils.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     1435 2024-05-04 10:01:16.000000 decalmlutils-0.0.8/decalmlutils/np_memmap.py
--rw-rw-r--   0 richard   (1000) richard   (1000)       39 2024-02-14 22:42:19.000000 decalmlutils-0.0.8/decalmlutils/plotting.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     2582 2024-02-16 14:01:25.000000 decalmlutils-0.0.8/decalmlutils/profiling.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     3016 2024-02-16 13:58:24.000000 decalmlutils-0.0.8/decalmlutils/ray_utils.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     4080 2024-02-16 14:05:12.000000 decalmlutils-0.0.8/decalmlutils/tensors.py
--rw-rw-r--   0 richard   (1000) richard   (1000)      878 2024-02-15 15:26:01.000000 decalmlutils-0.0.8/decalmlutils/testing.py
--rw-rw-r--   0 richard   (1000) richard   (1000)       46 2024-02-14 20:27:28.000000 decalmlutils-0.0.8/decalmlutils/text.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     1561 2024-05-10 21:28:40.000000 decalmlutils-0.0.8/decalmlutils/training.py
--rw-rw-r--   0 richard   (1000) richard   (1000)       47 2024-02-14 20:27:28.000000 decalmlutils-0.0.8/decalmlutils/web.py
-drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2024-05-23 16:52:25.116402 decalmlutils-0.0.8/decalmlutils.egg-info/
--rw-r--r--   0 richard   (1000) richard   (1000)     6350 2024-05-23 16:52:25.000000 decalmlutils-0.0.8/decalmlutils.egg-info/PKG-INFO
--rw-rw-r--   0 richard   (1000) richard   (1000)      694 2024-05-23 16:52:25.000000 decalmlutils-0.0.8/decalmlutils.egg-info/SOURCES.txt
--rw-rw-r--   0 richard   (1000) richard   (1000)        1 2024-05-23 16:52:25.000000 decalmlutils-0.0.8/decalmlutils.egg-info/dependency_links.txt
--rw-rw-r--   0 richard   (1000) richard   (1000)      846 2024-05-23 16:52:25.000000 decalmlutils-0.0.8/decalmlutils.egg-info/requires.txt
--rw-rw-r--   0 richard   (1000) richard   (1000)       13 2024-05-23 16:52:25.000000 decalmlutils-0.0.8/decalmlutils.egg-info/top_level.txt
--rw-rw-r--   0 richard   (1000) richard   (1000)     1043 2024-05-23 14:38:06.000000 decalmlutils-0.0.8/pyproject.toml
--rw-rw-r--   0 richard   (1000) richard   (1000)       38 2024-05-23 16:52:25.120402 decalmlutils-0.0.8/setup.cfg
--rw-rw-r--   0 richard   (1000) richard   (1000)     3902 2024-05-23 16:52:08.000000 decalmlutils-0.0.8/setup.py
-drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2024-05-23 16:52:25.116402 decalmlutils-0.0.8/tests/
--rw-rw-r--   0 richard   (1000) richard   (1000)        0 2024-02-14 21:27:17.000000 decalmlutils-0.0.8/tests/test_plotting.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     1586 2024-05-10 21:05:07.000000 decalmlutils-0.0.8/tests/test_tensors.py
--rw-rw-r--   0 richard   (1000) richard   (1000)      233 2024-05-10 21:05:07.000000 decalmlutils-0.0.8/tests/test_testing.py
--rw-rw-r--   0 richard   (1000) richard   (1000)        0 2024-02-14 21:25:36.000000 decalmlutils-0.0.8/tests/test_text.py
--rw-rw-r--   0 richard   (1000) richard   (1000)      167 2024-05-23 14:45:15.000000 decalmlutils-0.0.8/tests/test_training.py
--rw-rw-r--   0 richard   (1000) richard   (1000)        0 2024-02-16 17:31:23.000000 decalmlutils-0.0.8/tests/test_web.py
+drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2024-05-23 17:05:55.727457 decalmlutils-0.0.9/
+-rw-rw-r--   0 richard   (1000) richard   (1000)    11358 2024-02-14 15:27:04.000000 decalmlutils-0.0.9/LICENSE
+-rw-r--r--   0 richard   (1000) richard   (1000)     6350 2024-05-23 17:05:55.727457 decalmlutils-0.0.9/PKG-INFO
+-rw-rw-r--   0 richard   (1000) richard   (1000)     2117 2024-05-10 21:20:37.000000 decalmlutils-0.0.9/README.md
+drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2024-05-23 17:05:55.719457 decalmlutils-0.0.9/decalmlutils/
+-rw-rw-r--   0 richard   (1000) richard   (1000)      303 2024-05-23 17:05:47.000000 decalmlutils-0.0.9/decalmlutils/__init__.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)      659 2024-05-10 21:26:05.000000 decalmlutils-0.0.9/decalmlutils/dataframes.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)    22461 2024-05-10 18:40:47.000000 decalmlutils-0.0.9/decalmlutils/debug_info.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     2119 2024-02-16 14:37:48.000000 decalmlutils-0.0.9/decalmlutils/geom.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     2042 2024-05-23 14:29:50.000000 decalmlutils-0.0.9/decalmlutils/logging_utils.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     7067 2024-05-21 21:12:36.000000 decalmlutils-0.0.9/decalmlutils/misc.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     1435 2024-05-04 10:01:16.000000 decalmlutils-0.0.9/decalmlutils/np_memmap.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)       39 2024-02-14 22:42:19.000000 decalmlutils-0.0.9/decalmlutils/plotting.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     2582 2024-02-16 14:01:25.000000 decalmlutils-0.0.9/decalmlutils/profiling.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     3016 2024-02-16 13:58:24.000000 decalmlutils-0.0.9/decalmlutils/ray_utils.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     4080 2024-02-16 14:05:12.000000 decalmlutils-0.0.9/decalmlutils/tensors.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)      878 2024-02-15 15:26:01.000000 decalmlutils-0.0.9/decalmlutils/testing.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)       46 2024-02-14 20:27:28.000000 decalmlutils-0.0.9/decalmlutils/text.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     1558 2024-05-23 16:59:08.000000 decalmlutils-0.0.9/decalmlutils/training.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)       47 2024-02-14 20:27:28.000000 decalmlutils-0.0.9/decalmlutils/web.py
+drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2024-05-23 17:05:55.719457 decalmlutils-0.0.9/decalmlutils.egg-info/
+-rw-r--r--   0 richard   (1000) richard   (1000)     6350 2024-05-23 17:05:55.000000 decalmlutils-0.0.9/decalmlutils.egg-info/PKG-INFO
+-rw-rw-r--   0 richard   (1000) richard   (1000)      715 2024-05-23 17:05:55.000000 decalmlutils-0.0.9/decalmlutils.egg-info/SOURCES.txt
+-rw-rw-r--   0 richard   (1000) richard   (1000)        1 2024-05-23 17:05:55.000000 decalmlutils-0.0.9/decalmlutils.egg-info/dependency_links.txt
+-rw-rw-r--   0 richard   (1000) richard   (1000)      846 2024-05-23 17:05:55.000000 decalmlutils-0.0.9/decalmlutils.egg-info/requires.txt
+-rw-rw-r--   0 richard   (1000) richard   (1000)       13 2024-05-23 17:05:55.000000 decalmlutils-0.0.9/decalmlutils.egg-info/top_level.txt
+-rw-rw-r--   0 richard   (1000) richard   (1000)     1043 2024-05-23 14:38:06.000000 decalmlutils-0.0.9/pyproject.toml
+-rw-rw-r--   0 richard   (1000) richard   (1000)       38 2024-05-23 17:05:55.727457 decalmlutils-0.0.9/setup.cfg
+-rw-rw-r--   0 richard   (1000) richard   (1000)     3902 2024-05-23 17:05:47.000000 decalmlutils-0.0.9/setup.py
+drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2024-05-23 17:05:55.719457 decalmlutils-0.0.9/tests/
+-rw-rw-r--   0 richard   (1000) richard   (1000)        0 2024-02-14 21:27:17.000000 decalmlutils-0.0.9/tests/test_plotting.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     1586 2024-05-10 21:05:07.000000 decalmlutils-0.0.9/tests/test_tensors.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)      233 2024-05-10 21:05:07.000000 decalmlutils-0.0.9/tests/test_testing.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)        0 2024-02-14 21:25:36.000000 decalmlutils-0.0.9/tests/test_text.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)      167 2024-05-23 14:45:15.000000 decalmlutils-0.0.9/tests/test_training.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)        0 2024-02-16 17:31:23.000000 decalmlutils-0.0.9/tests/test_web.py
```

### Comparing `decalmlutils-0.0.8/LICENSE` & `decalmlutils-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `decalmlutils-0.0.8/PKG-INFO` & `decalmlutils-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decalmlutils
-Version: 0.0.8
+Version: 0.0.9
 Summary: Useful functions when working with Machine Learning in Python
 Home-page: https://github.com/crypdick/decalmlutils
 Author: Richard Decal
 Author-email: public@richarddecal.com
 License: Apache
 Keywords: deep learning pytorch numpy
 Classifier: Development Status :: 5 - Production/Stable
@@ -72,49 +72,49 @@
 Requires-Dist: pytest; extra == "tests"
 Requires-Dist: pytest-cov; extra == "tests"
 Requires-Dist: pytest-env; extra == "tests"
 Requires-Dist: pytest-xdist; extra == "tests"
 Requires-Dist: pytest-mock; extra == "tests"
 Requires-Dist: hypothesis; extra == "tests"
 Provides-Extra: all
-Requires-Dist: jinja2; extra == "all"
-Requires-Dist: pytest-cov; extra == "all"
-Requires-Dist: requests; extra == "all"
-Requires-Dist: boto3; extra == "all"
-Requires-Dist: pre-commit; extra == "all"
-Requires-Dist: torch; extra == "all"
 Requires-Dist: jira; extra == "all"
-Requires-Dist: pytest-env; extra == "all"
-Requires-Dist: slack_sdk; extra == "all"
-Requires-Dist: torchvision; extra == "all"
-Requires-Dist: tenacity; extra == "all"
-Requires-Dist: graphviz; extra == "all"
-Requires-Dist: matplotlib>=3.4.0; extra == "all"
-Requires-Dist: geojson; extra == "all"
-Requires-Dist: metaflow; extra == "all"
-Requires-Dist: twine; extra == "all"
+Requires-Dist: torch; extra == "all"
+Requires-Dist: pyarrow; extra == "all"
 Requires-Dist: numpy; extra == "all"
+Requires-Dist: ipython; extra == "all"
 Requires-Dist: build; extra == "all"
-Requires-Dist: pytest-xdist; extra == "all"
+Requires-Dist: pytest-env; extra == "all"
 Requires-Dist: pytest-mock; extra == "all"
-Requires-Dist: GitPython; extra == "all"
-Requires-Dist: ray; extra == "all"
-Requires-Dist: ipython; extra == "all"
-Requires-Dist: pyarrow; extra == "all"
+Requires-Dist: pytest-cov; extra == "all"
 Requires-Dist: hypothesis; extra == "all"
-Requires-Dist: isort; extra == "all"
-Requires-Dist: pytest; extra == "all"
+Requires-Dist: jinja2; extra == "all"
+Requires-Dist: tenacity; extra == "all"
 Requires-Dist: bump2version; extra == "all"
 Requires-Dist: ruff; extra == "all"
-Requires-Dist: watchtower; extra == "all"
-Requires-Dist: click; extra == "all"
-Requires-Dist: pyinstrument; extra == "all"
+Requires-Dist: pytest-xdist; extra == "all"
+Requires-Dist: pre-commit; extra == "all"
 Requires-Dist: scikit-learn; extra == "all"
+Requires-Dist: pytest; extra == "all"
+Requires-Dist: ray; extra == "all"
+Requires-Dist: pyinstrument; extra == "all"
+Requires-Dist: metaflow; extra == "all"
+Requires-Dist: geojson; extra == "all"
+Requires-Dist: matplotlib>=3.4.0; extra == "all"
+Requires-Dist: isort; extra == "all"
 Requires-Dist: pandas; extra == "all"
+Requires-Dist: torchvision; extra == "all"
+Requires-Dist: graphviz; extra == "all"
+Requires-Dist: slack_sdk; extra == "all"
+Requires-Dist: boto3; extra == "all"
 Requires-Dist: seaborn; extra == "all"
+Requires-Dist: watchtower; extra == "all"
+Requires-Dist: twine; extra == "all"
+Requires-Dist: requests; extra == "all"
+Requires-Dist: GitPython; extra == "all"
+Requires-Dist: click; extra == "all"
 
 # decalmlutils
 
 [![Build status](https://github.com/crypdick/decalmlutils/actions/workflows/python-app.yml/badge.svg)](https://github.com/crypdick/decalmlutils/actions/workflows/python-app.yml)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
```

### Comparing `decalmlutils-0.0.8/README.md` & `decalmlutils-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `decalmlutils-0.0.8/decalmlutils/dataframes.py` & `decalmlutils-0.0.9/decalmlutils/dataframes.py`

 * *Files identical despite different names*

### Comparing `decalmlutils-0.0.8/decalmlutils/debug_info.py` & `decalmlutils-0.0.9/decalmlutils/debug_info.py`

 * *Files identical despite different names*

### Comparing `decalmlutils-0.0.8/decalmlutils/geom.py` & `decalmlutils-0.0.9/decalmlutils/geom.py`

 * *Files identical despite different names*

### Comparing `decalmlutils-0.0.8/decalmlutils/logging_utils.py` & `decalmlutils-0.0.9/decalmlutils/logging_utils.py`

 * *Files identical despite different names*

### Comparing `decalmlutils-0.0.8/decalmlutils/np_memmap.py` & `decalmlutils-0.0.9/decalmlutils/np_memmap.py`

 * *Files identical despite different names*

### Comparing `decalmlutils-0.0.8/decalmlutils/profiling.py` & `decalmlutils-0.0.9/decalmlutils/profiling.py`

 * *Files identical despite different names*

### Comparing `decalmlutils-0.0.8/decalmlutils/ray_utils.py` & `decalmlutils-0.0.9/decalmlutils/ray_utils.py`

 * *Files identical despite different names*

### Comparing `decalmlutils-0.0.8/decalmlutils/tensors.py` & `decalmlutils-0.0.9/decalmlutils/tensors.py`

 * *Files identical despite different names*

### Comparing `decalmlutils-0.0.8/decalmlutils/testing.py` & `decalmlutils-0.0.9/decalmlutils/testing.py`

 * *Files identical despite different names*

### Comparing `decalmlutils-0.0.8/decalmlutils/training.py` & `decalmlutils-0.0.9/decalmlutils/training.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import random
 
 import numpy as np
 import torch
 from beartype import beartype
 from beartype.typing import Optional
 
-from decalmlutils.io.misc import millify
+from decalmlutils.misc import millify
 
 
 @beartype
 def seed_everything(seed: Optional[int] = None):
     """
     Seeds all random number generators. Record the seed you used for reproducibility.
```

### Comparing `decalmlutils-0.0.8/decalmlutils.egg-info/PKG-INFO` & `decalmlutils-0.0.9/decalmlutils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decalmlutils
-Version: 0.0.8
+Version: 0.0.9
 Summary: Useful functions when working with Machine Learning in Python
 Home-page: https://github.com/crypdick/decalmlutils
 Author: Richard Decal
 Author-email: public@richarddecal.com
 License: Apache
 Keywords: deep learning pytorch numpy
 Classifier: Development Status :: 5 - Production/Stable
@@ -72,49 +72,49 @@
 Requires-Dist: pytest; extra == "tests"
 Requires-Dist: pytest-cov; extra == "tests"
 Requires-Dist: pytest-env; extra == "tests"
 Requires-Dist: pytest-xdist; extra == "tests"
 Requires-Dist: pytest-mock; extra == "tests"
 Requires-Dist: hypothesis; extra == "tests"
 Provides-Extra: all
-Requires-Dist: jinja2; extra == "all"
-Requires-Dist: pytest-cov; extra == "all"
-Requires-Dist: requests; extra == "all"
-Requires-Dist: boto3; extra == "all"
-Requires-Dist: pre-commit; extra == "all"
-Requires-Dist: torch; extra == "all"
 Requires-Dist: jira; extra == "all"
-Requires-Dist: pytest-env; extra == "all"
-Requires-Dist: slack_sdk; extra == "all"
-Requires-Dist: torchvision; extra == "all"
-Requires-Dist: tenacity; extra == "all"
-Requires-Dist: graphviz; extra == "all"
-Requires-Dist: matplotlib>=3.4.0; extra == "all"
-Requires-Dist: geojson; extra == "all"
-Requires-Dist: metaflow; extra == "all"
-Requires-Dist: twine; extra == "all"
+Requires-Dist: torch; extra == "all"
+Requires-Dist: pyarrow; extra == "all"
 Requires-Dist: numpy; extra == "all"
+Requires-Dist: ipython; extra == "all"
 Requires-Dist: build; extra == "all"
-Requires-Dist: pytest-xdist; extra == "all"
+Requires-Dist: pytest-env; extra == "all"
 Requires-Dist: pytest-mock; extra == "all"
-Requires-Dist: GitPython; extra == "all"
-Requires-Dist: ray; extra == "all"
-Requires-Dist: ipython; extra == "all"
-Requires-Dist: pyarrow; extra == "all"
+Requires-Dist: pytest-cov; extra == "all"
 Requires-Dist: hypothesis; extra == "all"
-Requires-Dist: isort; extra == "all"
-Requires-Dist: pytest; extra == "all"
+Requires-Dist: jinja2; extra == "all"
+Requires-Dist: tenacity; extra == "all"
 Requires-Dist: bump2version; extra == "all"
 Requires-Dist: ruff; extra == "all"
-Requires-Dist: watchtower; extra == "all"
-Requires-Dist: click; extra == "all"
-Requires-Dist: pyinstrument; extra == "all"
+Requires-Dist: pytest-xdist; extra == "all"
+Requires-Dist: pre-commit; extra == "all"
 Requires-Dist: scikit-learn; extra == "all"
+Requires-Dist: pytest; extra == "all"
+Requires-Dist: ray; extra == "all"
+Requires-Dist: pyinstrument; extra == "all"
+Requires-Dist: metaflow; extra == "all"
+Requires-Dist: geojson; extra == "all"
+Requires-Dist: matplotlib>=3.4.0; extra == "all"
+Requires-Dist: isort; extra == "all"
 Requires-Dist: pandas; extra == "all"
+Requires-Dist: torchvision; extra == "all"
+Requires-Dist: graphviz; extra == "all"
+Requires-Dist: slack_sdk; extra == "all"
+Requires-Dist: boto3; extra == "all"
 Requires-Dist: seaborn; extra == "all"
+Requires-Dist: watchtower; extra == "all"
+Requires-Dist: twine; extra == "all"
+Requires-Dist: requests; extra == "all"
+Requires-Dist: GitPython; extra == "all"
+Requires-Dist: click; extra == "all"
 
 # decalmlutils
 
 [![Build status](https://github.com/crypdick/decalmlutils/actions/workflows/python-app.yml/badge.svg)](https://github.com/crypdick/decalmlutils/actions/workflows/python-app.yml)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
```

### Comparing `decalmlutils-0.0.8/decalmlutils.egg-info/SOURCES.txt` & `decalmlutils-0.0.9/decalmlutils.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 pyproject.toml
 setup.py
 decalmlutils/__init__.py
 decalmlutils/dataframes.py
 decalmlutils/debug_info.py
 decalmlutils/geom.py
 decalmlutils/logging_utils.py
+decalmlutils/misc.py
 decalmlutils/np_memmap.py
 decalmlutils/plotting.py
 decalmlutils/profiling.py
 decalmlutils/ray_utils.py
 decalmlutils/tensors.py
 decalmlutils/testing.py
 decalmlutils/text.py
```

### Comparing `decalmlutils-0.0.8/decalmlutils.egg-info/requires.txt` & `decalmlutils-0.0.9/decalmlutils.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -2,49 +2,49 @@
 ftfy>=5.8
 beartype
 pydantic
 pydantic-settings
 natsort
 
 [all]
-jinja2
-pytest-cov
-requests
-boto3
-pre-commit
-torch
 jira
-pytest-env
-slack_sdk
-torchvision
-tenacity
-graphviz
-matplotlib>=3.4.0
-geojson
-metaflow
-twine
+torch
+pyarrow
 numpy
+ipython
 build
-pytest-xdist
+pytest-env
 pytest-mock
-GitPython
-ray
-ipython
-pyarrow
+pytest-cov
 hypothesis
-isort
-pytest
+jinja2
+tenacity
 bump2version
 ruff
-watchtower
-click
-pyinstrument
+pytest-xdist
+pre-commit
 scikit-learn
+pytest
+ray
+pyinstrument
+metaflow
+geojson
+matplotlib>=3.4.0
+isort
 pandas
+torchvision
+graphviz
+slack_sdk
+boto3
 seaborn
+watchtower
+twine
+requests
+GitPython
+click
 
 [aws]
 boto3
 watchtower
 tenacity
 
 [dev]
```

### Comparing `decalmlutils-0.0.8/pyproject.toml` & `decalmlutils-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `decalmlutils-0.0.8/setup.py` & `decalmlutils-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 extras = {
     **_extras,
     "all": list({dep for deps in _extras.values() for dep in deps}),
 }
 
 setup(
     name="decalmlutils",
-    version="0.0.8",
+    version="0.0.9",
     author="Richard Decal",
     author_email="public@richarddecal.com",
     description="Useful functions when working with Machine Learning in Python",
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     keywords="deep learning pytorch numpy",
     license="Apache",
```

### Comparing `decalmlutils-0.0.8/tests/test_tensors.py` & `decalmlutils-0.0.9/tests/test_tensors.py`

 * *Files identical despite different names*

