# Comparing `tmp/flameai-1.0.0.tar.gz` & `tmp/flameai-1.0.1.tar.gz`

## Comparing `flameai-1.0.0.tar` & `flameai-1.0.1.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 flameai-1.0.0/src/flameai/__init__.py
--rw-r--r--   0        0        0     3588 2020-02-02 00:00:00.000000 flameai-1.0.0/src/flameai/metrics.py
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 flameai-1.0.0/src/flameai/mining.py
--rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 flameai-1.0.0/src/flameai/plot.py
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 flameai-1.0.0/src/flameai/preprocessing.py
--rw-r--r--   0        0        0     2808 2020-02-02 00:00:00.000000 flameai-1.0.0/src/flameai/train.py
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 flameai-1.0.0/src/flameai/util.py
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 flameai-1.0.0/.gitignore
--rw-r--r--   0        0        0    11341 2020-02-02 00:00:00.000000 flameai-1.0.0/LICENSE
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 flameai-1.0.0/README.md
--rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 flameai-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 flameai-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 flameai-1.0.1/src/flameai/__init__.py
+-rw-r--r--   0        0        0     3588 2020-02-02 00:00:00.000000 flameai-1.0.1/src/flameai/metrics.py
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 flameai-1.0.1/src/flameai/mining.py
+-rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 flameai-1.0.1/src/flameai/plot.py
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 flameai-1.0.1/src/flameai/preprocessing.py
+-rw-r--r--   0        0        0     2808 2020-02-02 00:00:00.000000 flameai-1.0.1/src/flameai/train.py
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 flameai-1.0.1/src/flameai/util.py
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 flameai-1.0.1/tests/example.py
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 flameai-1.0.1/.gitignore
+-rw-r--r--   0        0        0    11341 2020-02-02 00:00:00.000000 flameai-1.0.1/LICENSE
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 flameai-1.0.1/README.md
+-rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 flameai-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2134 2020-02-02 00:00:00.000000 flameai-1.0.1/PKG-INFO
```

### Comparing `flameai-1.0.0/src/flameai/metrics.py` & `flameai-1.0.1/src/flameai/metrics.py`

 * *Files identical despite different names*

### Comparing `flameai-1.0.0/src/flameai/plot.py` & `flameai-1.0.1/src/flameai/plot.py`

 * *Files identical despite different names*

### Comparing `flameai-1.0.0/src/flameai/preprocessing.py` & `flameai-1.0.1/src/flameai/preprocessing.py`

 * *Files identical despite different names*

### Comparing `flameai-1.0.0/src/flameai/train.py` & `flameai-1.0.1/src/flameai/train.py`

 * *Files identical despite different names*

### Comparing `flameai-1.0.0/src/flameai/util.py` & `flameai-1.0.1/src/flameai/util.py`

 * *Files identical despite different names*

### Comparing `flameai-1.0.0/LICENSE` & `flameai-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flameai-1.0.0/pyproject.toml` & `flameai-1.0.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "flameai"
-version = "1.0.0"
+version = "1.0.1"
 description = "Deep Learning Toolkit."
 readme = "README.md"
 keywords = [
   "deep learning",
   "flameai",
 ]
 license = { text = "Apache-2.0" }
```

