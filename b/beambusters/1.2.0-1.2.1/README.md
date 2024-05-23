# Comparing `tmp/beambusters-1.2.0.tar.gz` & `tmp/beambusters-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beambusters-1.2.0.tar", max compression
+gzip compressed data, was "beambusters-1.2.1.tar", max compression
```

## Comparing `beambusters-1.2.0.tar` & `beambusters-1.2.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    35149 2024-05-22 15:54:42.031692 beambusters-1.2.0/LICENSE
--rw-r--r--   0        0        0      630 2024-05-22 15:54:42.031692 beambusters-1.2.0/README.md
--rwxr-xr-x   0        0        0        0 2024-05-22 15:54:42.031692 beambusters-1.2.0/beambusters/__init__.py
--rw-r--r--   0        0        0    11827 2024-05-22 15:54:42.031692 beambusters-1.2.0/beambusters/main.py
--rwxr-xr-x   0        0        0     3170 2024-05-22 15:54:42.031692 beambusters-1.2.0/beambusters/settings.py
--rwxr-xr-x   0        0        0      143 2024-05-22 15:54:42.031692 beambusters-1.2.0/beambusters/utils.py
--rw-r--r--   0        0        0     2026 2024-05-22 15:54:51.699699 beambusters-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     3962 1970-01-01 00:00:00.000000 beambusters-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-22 16:01:34.654952 beambusters-1.2.1/LICENSE
+-rw-r--r--   0        0        0      630 2024-05-22 16:01:34.654952 beambusters-1.2.1/README.md
+-rwxr-xr-x   0        0        0        0 2024-05-22 16:01:34.654952 beambusters-1.2.1/beambusters/__init__.py
+-rw-r--r--   0        0        0    11845 2024-05-22 16:01:34.654952 beambusters-1.2.1/beambusters/main.py
+-rwxr-xr-x   0        0        0     3170 2024-05-22 16:01:34.654952 beambusters-1.2.1/beambusters/settings.py
+-rwxr-xr-x   0        0        0      143 2024-05-22 16:01:34.654952 beambusters-1.2.1/beambusters/utils.py
+-rw-r--r--   0        0        0     2026 2024-05-22 16:01:46.571013 beambusters-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3962 1970-01-01 00:00:00.000000 beambusters-1.2.1/PKG-INFO
```

### Comparing `beambusters-1.2.0/LICENSE` & `beambusters-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `beambusters-1.2.0/README.md` & `beambusters-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `beambusters-1.2.0/beambusters/main.py` & `beambusters-1.2.1/beambusters/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from beambusters import settings
 import subprocess as sub
 import h5py
 import numpy as np
 from beambusters.utils import centering_converged
 import matplotlib.pyplot as plt
 import math
+import hdf5plugin
 import os
 import pathlib
 import sys
 from bblib.methods import CenterOfMass, FriedelPairs, MinimizePeakFWHM, CircleDetection
 from bblib.models import PF8Info, PF8
 
 app = typer.Typer()
```

### Comparing `beambusters-1.2.0/beambusters/settings.py` & `beambusters-1.2.1/beambusters/settings.py`

 * *Files identical despite different names*

### Comparing `beambusters-1.2.0/pyproject.toml` & `beambusters-1.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "beambusters"
-version = "1.2.0"
+version = "1.2.1"
 description = ""
 authors = ["Ana Rodrigues <anananacr@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 beambusters = "beambusters.main:app"
```

### Comparing `beambusters-1.2.0/PKG-INFO` & `beambusters-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beambusters
-Version: 1.2.0
+Version: 1.2.1
 Summary: 
 Author: Ana Rodrigues
 Author-email: anananacr@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

