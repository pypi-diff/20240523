# Comparing `tmp/computegraph-0.4.4.tar.gz` & `tmp/computegraph-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "computegraph-0.4.4.tar", max compression
+gzip compressed data, was "computegraph-0.4.5.tar", max compression
```

## Comparing `computegraph-0.4.4.tar` & `computegraph-0.4.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      120 2023-02-10 03:25:56.177925 computegraph-0.4.4/computegraph/__init__.py
--rw-r--r--   0        0        0       37 2022-07-27 01:31:10.208964 computegraph-0.4.4/computegraph/draw/__init__.py
--rw-r--r--   0        0        0     6357 2022-07-27 01:31:10.209474 computegraph-0.4.4/computegraph/draw/add_edge.py
--rw-r--r--   0        0        0     4492 2023-04-26 00:33:51.036337 computegraph-0.4.4/computegraph/draw/draw.py
--rw-r--r--   0        0        0     1199 2022-07-27 01:31:10.209964 computegraph-0.4.4/computegraph/draw/ngraph.py
--rw-r--r--   0        0        0     1283 2022-07-27 01:31:10.208464 computegraph-0.4.4/computegraph/draw/README.md
--rw-r--r--   0        0        0     3108 2023-02-10 03:25:56.179927 computegraph-0.4.4/computegraph/dynamic.py
--rw-r--r--   0        0        0     6335 2023-04-26 01:01:04.663285 computegraph-0.4.4/computegraph/graph.py
--rw-r--r--   0        0        0     1989 2023-08-22 06:06:26.588913 computegraph-0.4.4/computegraph/jaxify.py
--rw-r--r--   0        0        0      490 2022-07-27 01:31:10.210965 computegraph-0.4.4/computegraph/options.py
--rw-r--r--   0        0        0     7850 2023-09-27 23:36:37.023825 computegraph-0.4.4/computegraph/types.py
--rw-r--r--   0        0        0    13318 2023-09-05 03:02:19.790758 computegraph-0.4.4/computegraph/utils.py
--rw-r--r--   0        0        0     1296 2022-07-27 01:31:10.207464 computegraph-0.4.4/LICENSE
--rw-r--r--   0        0        0     1272 2023-09-27 23:36:55.342831 computegraph-0.4.4/pyproject.toml
--rw-r--r--   0        0        0       88 2022-07-27 01:31:10.207965 computegraph-0.4.4/README.md
--rw-r--r--   0        0        0     1351 1970-01-01 00:00:00.000000 computegraph-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0      120 2023-02-10 03:25:56.177925 computegraph-0.4.5/computegraph/__init__.py
+-rw-r--r--   0        0        0       37 2022-07-27 01:31:10.208964 computegraph-0.4.5/computegraph/draw/__init__.py
+-rw-r--r--   0        0        0     6357 2022-07-27 01:31:10.209474 computegraph-0.4.5/computegraph/draw/add_edge.py
+-rw-r--r--   0        0        0     4492 2023-04-26 00:33:51.036337 computegraph-0.4.5/computegraph/draw/draw.py
+-rw-r--r--   0        0        0     1199 2022-07-27 01:31:10.209964 computegraph-0.4.5/computegraph/draw/ngraph.py
+-rw-r--r--   0        0        0     1283 2022-07-27 01:31:10.208464 computegraph-0.4.5/computegraph/draw/README.md
+-rw-r--r--   0        0        0     3108 2023-02-10 03:25:56.179927 computegraph-0.4.5/computegraph/dynamic.py
+-rw-r--r--   0        0        0     6335 2023-04-26 01:01:04.663285 computegraph-0.4.5/computegraph/graph.py
+-rw-r--r--   0        0        0     1954 2024-05-23 21:20:10.103273 computegraph-0.4.5/computegraph/jaxify.py
+-rw-r--r--   0        0        0      490 2022-07-27 01:31:10.210965 computegraph-0.4.5/computegraph/options.py
+-rw-r--r--   0        0        0     7850 2023-09-27 23:37:57.250335 computegraph-0.4.5/computegraph/types.py
+-rw-r--r--   0        0        0    13318 2023-09-27 23:37:57.251343 computegraph-0.4.5/computegraph/utils.py
+-rw-r--r--   0        0        0     1296 2022-07-27 01:31:10.207464 computegraph-0.4.5/LICENSE
+-rw-r--r--   0        0        0     1193 2024-05-23 21:24:45.204746 computegraph-0.4.5/pyproject.toml
+-rw-r--r--   0        0        0       88 2022-07-27 01:31:10.207965 computegraph-0.4.5/README.md
+-rw-r--r--   0        0        0     1196 1970-01-01 00:00:00.000000 computegraph-0.4.5/PKG-INFO
```

### Comparing `computegraph-0.4.4/computegraph/draw/add_edge.py` & `computegraph-0.4.5/computegraph/draw/add_edge.py`

 * *Files identical despite different names*

### Comparing `computegraph-0.4.4/computegraph/draw/draw.py` & `computegraph-0.4.5/computegraph/draw/draw.py`

 * *Files identical despite different names*

### Comparing `computegraph-0.4.4/computegraph/draw/ngraph.py` & `computegraph-0.4.5/computegraph/draw/ngraph.py`

 * *Files identical despite different names*

### Comparing `computegraph-0.4.4/computegraph/draw/README.md` & `computegraph-0.4.5/computegraph/draw/README.md`

 * *Files identical despite different names*

### Comparing `computegraph-0.4.4/computegraph/dynamic.py` & `computegraph-0.4.5/computegraph/dynamic.py`

 * *Files identical despite different names*

### Comparing `computegraph-0.4.4/computegraph/graph.py` & `computegraph-0.4.5/computegraph/graph.py`

 * *Files identical despite different names*

### Comparing `computegraph-0.4.4/computegraph/jaxify.py` & `computegraph-0.4.5/computegraph/jaxify.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,38 +2,37 @@
 The main entry point into using Jax in summer
 This should imported before any model code that uses jax, or builds jax functions
 
 The current jax status is stored in the environment variable SUMMER_USE_JAX
 Other modules should interact with this solely via set_using_jax and get_using_jax
 """
 
-
 import warnings
 import os
 
 from typing import Union
 
 import numpy as np
 import scipy
 
 try:
     from jax import numpy as jnp
     from jax import scipy as jsp
-    from jax.config import config as _jax_config
+    import jax
 
     # Jax configuration
     # FIXME: We need to find a more appropriate place to ensure this happens globally
-    _jax_config.update("jax_platform_name", "cpu")
-    _jax_config.update("jax_enable_x64", True)
+    jax.config.update("jax_platform_name", "cpu")
+    jax.config.update("jax_enable_x64", True)
 
     N_CORES = os.cpu_count()
 
-    os.environ[
-        "XLA_FLAGS"
-    ] = f"--xla_force_host_platform_device_count={N_CORES} --xla_cpu_multi_thread_eigen=false intra_op_parallelism_threads=1"
+    os.environ["XLA_FLAGS"] = (
+        f"--xla_force_host_platform_device_count={N_CORES} --xla_cpu_multi_thread_eigen=false intra_op_parallelism_threads=1"
+    )
 
     Array = Union[jnp.ndarray, np.ndarray]
 
 except ImportError:
     warnings.warn("Could not import jax, model performance will be limited")
 
     Array = np.ndarray
```

### Comparing `computegraph-0.4.4/computegraph/types.py` & `computegraph-0.4.5/computegraph/types.py`

 * *Files identical despite different names*

### Comparing `computegraph-0.4.4/computegraph/utils.py` & `computegraph-0.4.5/computegraph/utils.py`

 * *Files identical despite different names*

### Comparing `computegraph-0.4.4/LICENSE` & `computegraph-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `computegraph-0.4.4/pyproject.toml` & `computegraph-0.4.5/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "computegraph"
-version = "0.4.4"
+version = "0.4.5"
 readme = "README.md"
 license = "BSD-2-Clause"
 homepage = "https://github.com/monash-emu/computegraph"
 repository = "https://github.com/monash-emu/computegraph"
 documentation = "https://github.com/monash-emu/computegraph"
 keywords = [
     "graph",
@@ -16,25 +16,24 @@
 description = "computegraph is a tool for managing computational graphs using networkx"
 authors = ["David Shipman <dshipman@gmail.com>"]
 packages = [
     {include = "computegraph"}
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.8.0"
-numpy = ">=1.20.3"
-networkx = ">=2.6.2"
-scipy = ">=1.7.3"
+python = ">=3.10.0"
+#numpy = ">=1.20.3"
+#networkx = ">=2.6.2"
+#scipy = ">=1.7.3"
 pygraphviz = {version = ">=1.8", platform = "linux", optional = true}
 matplotlib = {version = ">=3.5.1", optional = true}
 plotly = {version = ">=5.6.0", optional = true}
-jax =  [
-    {extras = ["cpu"], version = ">=0.4", platform = "linux"},
-    {extras = ["cpu"], version = ">=0.4", platform = "darwin"}
-]
+jax = ">=0.4.28"
+networkx = "^3.3"
+jaxlib = "^0.4.28"
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2.5"
 black = "^20.8b0"
 pytest-parallel = "^0.1.0"
 pre-commit = "^2.19.0"
```

### Comparing `computegraph-0.4.4/PKG-INFO` & `computegraph-0.4.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,29 @@
 Metadata-Version: 2.1
 Name: computegraph
-Version: 0.4.4
+Version: 0.4.5
 Summary: computegraph is a tool for managing computational graphs using networkx
 Home-page: https://github.com/monash-emu/computegraph
 License: BSD-2-Clause
 Keywords: graph,networkx,plotting,jax,summerepi2
 Author: David Shipman
 Author-email: dshipman@gmail.com
-Requires-Python: >=3.8.0
+Requires-Python: >=3.10.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: plotting
-Requires-Dist: jax[cpu] (>=0.4) ; sys_platform == "darwin"
-Requires-Dist: jax[cpu] (>=0.4) ; sys_platform == "linux"
+Requires-Dist: jax (>=0.4.28)
+Requires-Dist: jaxlib (>=0.4.28,<0.5.0)
 Requires-Dist: matplotlib (>=3.5.1) ; extra == "plotting"
-Requires-Dist: networkx (>=2.6.2)
-Requires-Dist: numpy (>=1.20.3)
+Requires-Dist: networkx (>=3.3,<4.0)
 Requires-Dist: plotly (>=5.6.0) ; extra == "plotting"
 Requires-Dist: pygraphviz (>=1.8) ; (sys_platform == "linux") and (extra == "plotting")
-Requires-Dist: scipy (>=1.7.3)
 Project-URL: Documentation, https://github.com/monash-emu/computegraph
 Project-URL: Repository, https://github.com/monash-emu/computegraph
 Description-Content-Type: text/markdown
 
 # computegraph
 Tools for managing computation graphs based on dictionaries and networkx
```

