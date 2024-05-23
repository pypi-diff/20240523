# Comparing `tmp/flameai-1.0.1.tar.gz` & `tmp/flameai-1.0.2.tar.gz`

## Comparing `flameai-1.0.1.tar` & `flameai-1.0.2.tar`

### file list

```diff
@@ -1,13 +1,16 @@
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 flameai-1.0.1/src/flameai/__init__.py
--rw-r--r--   0        0        0     3588 2020-02-02 00:00:00.000000 flameai-1.0.1/src/flameai/metrics.py
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 flameai-1.0.1/src/flameai/mining.py
--rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 flameai-1.0.1/src/flameai/plot.py
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 flameai-1.0.1/src/flameai/preprocessing.py
--rw-r--r--   0        0        0     2808 2020-02-02 00:00:00.000000 flameai-1.0.1/src/flameai/train.py
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 flameai-1.0.1/src/flameai/util.py
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 flameai-1.0.1/tests/example.py
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 flameai-1.0.1/.gitignore
--rw-r--r--   0        0        0    11341 2020-02-02 00:00:00.000000 flameai-1.0.1/LICENSE
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 flameai-1.0.1/README.md
--rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 flameai-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 flameai-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 flameai-1.0.2/src/flameai/__init__.py
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 flameai-1.0.2/src/flameai/__main__.py
+-rw-r--r--   0        0        0     1324 2020-02-02 00:00:00.000000 flameai-1.0.2/src/flameai/_env.py
+-rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 flameai-1.0.2/src/flameai/cmd.py
+-rw-r--r--   0        0        0     3545 2020-02-02 00:00:00.000000 flameai-1.0.2/src/flameai/metrics.py
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 flameai-1.0.2/src/flameai/mining.py
+-rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 flameai-1.0.2/src/flameai/plot.py
+-rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 flameai-1.0.2/src/flameai/preprocessing.py
+-rw-r--r--   0        0        0     2808 2020-02-02 00:00:00.000000 flameai-1.0.2/src/flameai/train.py
+-rw-r--r--   0        0        0     1769 2020-02-02 00:00:00.000000 flameai-1.0.2/src/flameai/util.py
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 flameai-1.0.2/tests/test_metrics.py
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 flameai-1.0.2/.gitignore
+-rw-r--r--   0        0        0    11341 2020-02-02 00:00:00.000000 flameai-1.0.2/LICENSE
+-rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 flameai-1.0.2/README.md
+-rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 flameai-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2764 2020-02-02 00:00:00.000000 flameai-1.0.2/PKG-INFO
```

### Comparing `flameai-1.0.1/src/flameai/metrics.py` & `flameai-1.0.2/src/flameai/metrics.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import numpy as np
 import pandas as pd
 import sklearn.metrics
-import lightgbm as lgb
 
 from typing import Tuple, Optional, Any
-from flameai.train import gen_threshold
+from .train import gen_threshold
 
 
-def lgb_feature_importance(gbm: lgb.Booster) -> None:
+def lgb_feature_importance(gbm) -> None:
     """
     Calculate the importance of features in a LightGBM model.
 
     :param gbm: The trained LightGBM model.
     """
     items = [(k, v) for k, v in zip(gbm.feature_name(), gbm.feature_importance())]
     sorted_items = sorted(items, key = lambda e: e[1], reverse = True)
```

### Comparing `flameai-1.0.1/src/flameai/plot.py` & `flameai-1.0.2/src/flameai/plot.py`

 * *Files identical despite different names*

### Comparing `flameai-1.0.1/src/flameai/train.py` & `flameai-1.0.2/src/flameai/train.py`

 * *Files identical despite different names*

### Comparing `flameai-1.0.1/LICENSE` & `flameai-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `flameai-1.0.1/pyproject.toml` & `flameai-1.0.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,49 +1,53 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "flameai"
-version = "1.0.1"
+version = "1.0.2"
 description = "Deep Learning Toolkit."
 readme = "README.md"
 keywords = [
   "deep learning",
   "flameai",
 ]
 license = { text = "Apache-2.0" }
 authors = [
   { name = "luochang" },
   { email = "luochang212@gmail.com" },
 ]
-requires-python = ">=3.8"
+requires-python = ">=3.10"
 dependencies = [
   "numpy>=1.26.4",
   "pandas>=2.2.0",
   "scipy>=1.13.0",
   "scikit-learn>=1.5.0",
   "matplotlib>=3.8.4",
   "seaborn>=0.13.2",
   "optuna>=3.6.1",
+  "click>=8.1.7",
+  "torch>=2.2.2",
 ]
 classifiers = [
   "License :: OSI Approved :: Apache Software License",
   "Operating System :: MacOS",
   "Operating System :: Microsoft :: Windows",
   "Operating System :: POSIX",
   "Operating System :: Unix",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3 :: Only",
-  "Programming Language :: Python :: 3.8",
-  "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
   "Topic :: Scientific/Engineering :: Artificial Intelligence",
 ]
 
+[project.scripts]
+hey = "flameai.cmd:hey"
+hve = "flameai.cmd:hive_cli"
+cev = "flameai.__main__:check_env"
 
 [project.urls]
 repository = "https://github.com/luochang212/flameai"
 bug-tracker = "https://github.com/luochang212/flameai/issues"
 documentation = "https://luochang212.github.io/posts/flameai"
```

