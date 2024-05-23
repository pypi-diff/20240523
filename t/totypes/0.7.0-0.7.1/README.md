# Comparing `tmp/totypes-0.7.0.tar.gz` & `tmp/totypes-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "totypes-0.7.0.tar", last modified: Tue May 21 19:13:48 2024, max compression
+gzip compressed data, was "totypes-0.7.1.tar", last modified: Thu May 23 20:49:10 2024, max compression
```

## Comparing `totypes-0.7.0.tar` & `totypes-0.7.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:13:48.047429 totypes-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-21 19:13:37.000000 totypes-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3551 2024-05-21 19:13:48.047429 totypes-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-21 19:13:37.000000 totypes-0.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-21 19:13:37.000000 totypes-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 19:13:48.047429 totypes-0.7.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:13:48.043429 totypes-0.7.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:13:48.043429 totypes-0.7.0/src/totypes/
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-21 19:13:37.000000 totypes-0.7.0/src/totypes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11335 2024-05-21 19:13:37.000000 totypes-0.7.0/src/totypes/json_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-05-21 19:13:37.000000 totypes-0.7.0/src/totypes/partition_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 19:13:37.000000 totypes-0.7.0/src/totypes/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-05-21 19:13:37.000000 totypes-0.7.0/src/totypes/symmetry.py
--rw-r--r--   0 runner    (1001) docker     (127)    15202 2024-05-21 19:13:37.000000 totypes-0.7.0/src/totypes/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:13:48.047429 totypes-0.7.0/src/totypes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3551 2024-05-21 19:13:48.000000 totypes-0.7.0/src/totypes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-21 19:13:48.000000 totypes-0.7.0/src/totypes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 19:13:48.000000 totypes-0.7.0/src/totypes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-21 19:13:48.000000 totypes-0.7.0/src/totypes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-21 19:13:48.000000 totypes-0.7.0/src/totypes.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:13:48.047429 totypes-0.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    11331 2024-05-21 19:13:37.000000 totypes-0.7.0/tests/test_json_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-05-21 19:13:37.000000 totypes-0.7.0/tests/test_json_utils_server_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     7214 2024-05-21 19:13:37.000000 totypes-0.7.0/tests/test_partition_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4888 2024-05-21 19:13:37.000000 totypes-0.7.0/tests/test_symmetry.py
--rw-r--r--   0 runner    (1001) docker     (127)    10783 2024-05-21 19:13:37.000000 totypes-0.7.0/tests/test_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:49:10.146905 totypes-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-23 20:49:00.000000 totypes-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3551 2024-05-23 20:49:10.146905 totypes-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-23 20:49:00.000000 totypes-0.7.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-23 20:49:00.000000 totypes-0.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 20:49:10.146905 totypes-0.7.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:49:10.142905 totypes-0.7.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:49:10.142905 totypes-0.7.1/src/totypes/
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-23 20:49:00.000000 totypes-0.7.1/src/totypes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11335 2024-05-23 20:49:00.000000 totypes-0.7.1/src/totypes/json_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1952 2024-05-23 20:49:00.000000 totypes-0.7.1/src/totypes/partition_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 20:49:00.000000 totypes-0.7.1/src/totypes/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-05-23 20:49:00.000000 totypes-0.7.1/src/totypes/symmetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15202 2024-05-23 20:49:00.000000 totypes-0.7.1/src/totypes/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:49:10.146905 totypes-0.7.1/src/totypes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3551 2024-05-23 20:49:10.000000 totypes-0.7.1/src/totypes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-23 20:49:10.000000 totypes-0.7.1/src/totypes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 20:49:10.000000 totypes-0.7.1/src/totypes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-23 20:49:10.000000 totypes-0.7.1/src/totypes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-23 20:49:10.000000 totypes-0.7.1/src/totypes.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 20:49:10.146905 totypes-0.7.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    11331 2024-05-23 20:49:00.000000 totypes-0.7.1/tests/test_json_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-05-23 20:49:00.000000 totypes-0.7.1/tests/test_json_utils_server_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7214 2024-05-23 20:49:00.000000 totypes-0.7.1/tests/test_partition_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4884 2024-05-23 20:49:00.000000 totypes-0.7.1/tests/test_symmetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10783 2024-05-23 20:49:00.000000 totypes-0.7.1/tests/test_types.py
```

### Comparing `totypes-0.7.0/LICENSE` & `totypes-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `totypes-0.7.0/PKG-INFO` & `totypes-0.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: totypes
-Version: 0.7.0
+Version: 0.7.1
 Summary: Custom datatypes useful in a topology optimization context
 Author-email: "Martin F. Schubert" <mfschubert@gmail.com>
 Maintainer-email: "Martin F. Schubert" <mfschubert@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 The INVRS-IO authors.
         
@@ -42,15 +42,15 @@
 Provides-Extra: dev
 Requires-Dist: bump-my-version; extra == "dev"
 Requires-Dist: darglint; extra == "dev"
 Requires-Dist: totypes[tests]; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 
 # totypes - Custom types for topology optimization
-`v0.7.0`
+`v0.7.1`
 
 ## Overview
 
 The `totypes` package defines custom jax-compatible datatypes for use in a topology optimization, inverse design, or AI-guided design context. The custom types are pytree nodes consisting of standard jax arrays along with metadata that describe the desired characteristics of the arrays.
 - `BoundedArray`, an array with optional lower and/or upper bounds, used e.g. for representing layer thicknesses.
 - `Density2DArray`, an array with lower and upper bounds and characteristics such as fixed pixels, minimum feature size, or symmetry, used for representing layer density as is common in topology optimization.
```

### Comparing `totypes-0.7.0/README.md` & `totypes-0.7.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # totypes - Custom types for topology optimization
-`v0.7.0`
+`v0.7.1`
 
 ## Overview
 
 The `totypes` package defines custom jax-compatible datatypes for use in a topology optimization, inverse design, or AI-guided design context. The custom types are pytree nodes consisting of standard jax arrays along with metadata that describe the desired characteristics of the arrays.
 - `BoundedArray`, an array with optional lower and/or upper bounds, used e.g. for representing layer thicknesses.
 - `Density2DArray`, an array with lower and upper bounds and characteristics such as fixed pixels, minimum feature size, or symmetry, used for representing layer density as is common in topology optimization.
```

### Comparing `totypes-0.7.0/pyproject.toml` & `totypes-0.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 
 name = "totypes"
-version = "v0.7.0"
+version = "v0.7.1"
 description = "Custom datatypes useful in a topology optimization context"
 keywords = ["topology", "optimization", "jax", "inverse design"]
 readme = "README.md"
 requires-python = ">=3.7"
 license = {file = "LICENSE"}
 
 authors = [
```

### Comparing `totypes-0.7.0/src/totypes/json_utils.py` & `totypes-0.7.1/src/totypes/json_utils.py`

 * *Files identical despite different names*

### Comparing `totypes-0.7.0/src/totypes/partition_utils.py` & `totypes-0.7.1/src/totypes/partition_utils.py`

 * *Files identical despite different names*

### Comparing `totypes-0.7.0/src/totypes/symmetry.py` & `totypes-0.7.1/src/totypes/symmetry.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,21 +53,26 @@
 def _reflection_e_w(array: jnp.ndarray) -> jnp.ndarray:
     """Transform `array` to have reflection symmetry about the e-w axis."""
     return (array + array[..., ::-1]) / 2
 
 
 def _rotation_180(array: jnp.ndarray) -> jnp.ndarray:
     """Transform `array` to have 180-degree rotational symmetry."""
-    return (array + jnp.rot90(array, 2)) / 2
+    return (array + jnp.rot90(array, 2, axes=(-2, -1))) / 2
 
 
 def _rotation_90(array: jnp.ndarray) -> jnp.ndarray:
     """Transform `array` to have 90-degree rotational symmetry."""
     assert array.shape[-2] == array.shape[-1]
-    return (array + jnp.rot90(array, 1) + jnp.rot90(array, 2) + jnp.rot90(array, 3)) / 4
+    return (
+        array
+        + jnp.rot90(array, 1, axes=(-2, -1))
+        + jnp.rot90(array, 2, axes=(-2, -1))
+        + jnp.rot90(array, 3, axes=(-2, -1))
+    ) / 4
 
 
 SYMMETRY_FNS = {
     REFLECTION_NE_SW: _reflection_ne_sw,
     REFLECTION_NW_SE: _reflection_nw_se,
     REFLECTION_N_S: _reflection_n_s,
     REFLECTION_E_W: _reflection_e_w,
```

### Comparing `totypes-0.7.0/src/totypes/types.py` & `totypes-0.7.1/src/totypes/types.py`

 * *Files identical despite different names*

### Comparing `totypes-0.7.0/src/totypes.egg-info/PKG-INFO` & `totypes-0.7.1/src/totypes.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: totypes
-Version: 0.7.0
+Version: 0.7.1
 Summary: Custom datatypes useful in a topology optimization context
 Author-email: "Martin F. Schubert" <mfschubert@gmail.com>
 Maintainer-email: "Martin F. Schubert" <mfschubert@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 The INVRS-IO authors.
         
@@ -42,15 +42,15 @@
 Provides-Extra: dev
 Requires-Dist: bump-my-version; extra == "dev"
 Requires-Dist: darglint; extra == "dev"
 Requires-Dist: totypes[tests]; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 
 # totypes - Custom types for topology optimization
-`v0.7.0`
+`v0.7.1`
 
 ## Overview
 
 The `totypes` package defines custom jax-compatible datatypes for use in a topology optimization, inverse design, or AI-guided design context. The custom types are pytree nodes consisting of standard jax arrays along with metadata that describe the desired characteristics of the arrays.
 - `BoundedArray`, an array with optional lower and/or upper bounds, used e.g. for representing layer thicknesses.
 - `Density2DArray`, an array with lower and upper bounds and characteristics such as fixed pixels, minimum feature size, or symmetry, used for representing layer density as is common in topology optimization.
```

### Comparing `totypes-0.7.0/tests/test_json_utils.py` & `totypes-0.7.1/tests/test_json_utils.py`

 * *Files identical despite different names*

### Comparing `totypes-0.7.0/tests/test_json_utils_server_client.py` & `totypes-0.7.1/tests/test_json_utils_server_client.py`

 * *Files identical despite different names*

### Comparing `totypes-0.7.0/tests/test_partition_utils.py` & `totypes-0.7.1/tests/test_partition_utils.py`

 * *Files identical despite different names*

### Comparing `totypes-0.7.0/tests/test_symmetry.py` & `totypes-0.7.1/tests/test_symmetry.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,9 +155,9 @@
             [symmetry.REFLECTION_NE_SW],
             [symmetry.REFLECTION_NW_SE],
             [symmetry.ROTATION_180],
             [symmetry.ROTATION_90],
         ]
     )
     def test_with_batch(self, sym):
-        arr = jnp.ones((1, 10, 13, 13))
+        arr = jnp.ones((8, 13, 13))
         symmetry.symmetrize(arr, (sym,))
```

### Comparing `totypes-0.7.0/tests/test_types.py` & `totypes-0.7.1/tests/test_types.py`

 * *Files identical despite different names*

