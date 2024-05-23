# Comparing `tmp/nadl-1.4.3.tar.gz` & `tmp/nadl-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nadl-1.4.3.tar", last modified: Thu May 23 00:09:48 2024, max compression
+gzip compressed data, was "nadl-1.4.4.tar", last modified: Thu May 23 00:16:28 2024, max compression
```

## Comparing `nadl-1.4.3.tar` & `nadl-1.4.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     2275 2024-05-23 00:09:48.828247 nadl-1.4.3/pyproject.toml
--rw-r--r--   0        0        0      596 2024-04-18 21:07:32.861885 nadl-1.4.3/readme.org
--rw-r--r--   0        0        0     6148 2024-05-22 06:49:46.036737 nadl-1.4.3/src/nadl/.DS_Store
--rw-r--r--   0        0        0     1806 2024-05-23 00:08:22.782642 nadl-1.4.3/src/nadl/__init__.py
--rw-r--r--   0        0        0     8364 2024-04-22 04:28:48.528762 nadl-1.4.3/src/nadl/blocks.py
--rw-r--r--   0        0        0     5834 2024-05-23 00:07:51.076934 nadl-1.4.3/src/nadl/data.py
--rw-r--r--   0        0        0     2180 2024-04-26 22:33:55.875764 nadl-1.4.3/src/nadl/images.py
--rw-r--r--   0        0        0     3564 2024-05-22 05:17:23.233277 nadl-1.4.3/src/nadl/keys.py
--rw-r--r--   0        0        0     5135 2024-05-21 15:18:23.436274 nadl-1.4.3/src/nadl/loops.py
--rw-r--r--   0        0        0     1828 2024-04-19 19:57:58.670986 nadl-1.4.3/src/nadl/metrics.py
--rw-r--r--   0        0        0     3629 2024-04-22 04:28:48.528396 nadl-1.4.3/src/nadl/nets.py
--rw-r--r--   0        0        0     3401 2024-04-19 20:04:00.936571 nadl-1.4.3/src/nadl/preprocessing.py
--rw-r--r--   0        0        0        0 2023-12-07 01:36:32.295961 nadl-1.4.3/src/nadl/py.typed
--rw-r--r--   0        0        0     3884 2024-05-15 03:21:02.151713 nadl-1.4.3/src/nadl/states.py
--rw-r--r--   0        0        0     1108 2024-04-22 04:28:48.527949 nadl-1.4.3/src/nadl/transformers.py
--rw-r--r--   0        0        0     2363 2024-05-14 05:16:59.307787 nadl-1.4.3/src/nadl/utils.py
--rw-r--r--   0        0        0     1368 1970-01-01 00:00:00.000000 nadl-1.4.3/PKG-INFO
+-rw-r--r--   0        0        0     2275 2024-05-23 00:16:28.112642 nadl-1.4.4/pyproject.toml
+-rw-r--r--   0        0        0      596 2024-04-18 21:07:32.861885 nadl-1.4.4/readme.org
+-rw-r--r--   0        0        0     6148 2024-05-22 06:49:46.036737 nadl-1.4.4/src/nadl/.DS_Store
+-rw-r--r--   0        0        0     1806 2024-05-23 00:15:58.230940 nadl-1.4.4/src/nadl/__init__.py
+-rw-r--r--   0        0        0     8364 2024-04-22 04:28:48.528762 nadl-1.4.4/src/nadl/blocks.py
+-rw-r--r--   0        0        0     5836 2024-05-23 00:14:47.295979 nadl-1.4.4/src/nadl/data.py
+-rw-r--r--   0        0        0     2180 2024-04-26 22:33:55.875764 nadl-1.4.4/src/nadl/images.py
+-rw-r--r--   0        0        0     3564 2024-05-22 05:17:23.233277 nadl-1.4.4/src/nadl/keys.py
+-rw-r--r--   0        0        0     5135 2024-05-21 15:18:23.436274 nadl-1.4.4/src/nadl/loops.py
+-rw-r--r--   0        0        0     1828 2024-04-19 19:57:58.670986 nadl-1.4.4/src/nadl/metrics.py
+-rw-r--r--   0        0        0     3629 2024-04-22 04:28:48.528396 nadl-1.4.4/src/nadl/nets.py
+-rw-r--r--   0        0        0     3401 2024-04-19 20:04:00.936571 nadl-1.4.4/src/nadl/preprocessing.py
+-rw-r--r--   0        0        0        0 2023-12-07 01:36:32.295961 nadl-1.4.4/src/nadl/py.typed
+-rw-r--r--   0        0        0     3884 2024-05-15 03:21:02.151713 nadl-1.4.4/src/nadl/states.py
+-rw-r--r--   0        0        0     1108 2024-04-22 04:28:48.527949 nadl-1.4.4/src/nadl/transformers.py
+-rw-r--r--   0        0        0     2363 2024-05-14 05:16:59.307787 nadl-1.4.4/src/nadl/utils.py
+-rw-r--r--   0        0        0     1368 1970-01-01 00:00:00.000000 nadl-1.4.4/PKG-INFO
```

### Comparing `nadl-1.4.3/pyproject.toml` & `nadl-1.4.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     "optax>=0.2.2",
     "equinox>=0.11.4",
     "beartype>=0.18.5",
     "scikit-image>=0.23.2",
     "orbax-checkpoint>=0.5.11",
 ]
 requires-python = ">=3.12"
-version = "1.4.3"
+version = "1.4.4"
 
 [project.readme]
 content-type = "text/plain"
 file = "readme.org"
 
 [project.license]
 text = "GPLv3"
```

### Comparing `nadl-1.4.3/readme.org` & `nadl-1.4.4/readme.org`

 * *Files identical despite different names*

### Comparing `nadl-1.4.3/src/nadl/.DS_Store` & `nadl-1.4.4/src/nadl/.DS_Store`

 * *Files identical despite different names*

### Comparing `nadl-1.4.3/src/nadl/__init__.py` & `nadl-1.4.4/src/nadl/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 from .states import BaseTrainState, state_fn
 from .utils import (
   classit,
   rle,
   rle_array,
 )
 
-__version__ = "1.4.3"
+__version__ = "1.4.4"
 
 __all__ = [
   "PG",
   "RESC",
   "SCALER",
   "BaseTrainState",
   "DState",
```

### Comparing `nadl-1.4.3/src/nadl/blocks.py` & `nadl-1.4.4/src/nadl/blocks.py`

 * *Files identical despite different names*

### Comparing `nadl-1.4.3/src/nadl/data.py` & `nadl-1.4.4/src/nadl/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,15 +149,15 @@
     else:
       pg.add_task(es, total=epochs, res="")
     pg.advance(pg.tasks[es], start_epoch - 1)
   if ss in pg.tasks:
     pg.pg.reset(pg.tasks[ss], total=ds.shape[0] * epochs, res="")
   else:
     pg.add_task(ss, total=ds.shape[0] * epochs, res="")
-  pg.advance(pg.tasks[ss], (start_step := max((start_epoch - 1), 0) * ds.shape[0]))
+  pg.advance(pg.tasks[ss], (start_step := max((start_epoch - 1), 0)))
 
   @eqx.filter_jit
   def _select(i: jax.Array, ii: jax.Array) -> DState[T]:
     return tree_at(
       lambda x: (x.epoch, x.step),
       jax.tree.map(lambda x: x[i, ii] if isinstance(x, jax.Array) else x, ds),
       (i, i * ds.shape[0] + ii),
@@ -176,15 +176,15 @@
   """Test."""
   pg = PG.init_progress(extra_columns=(RESC,))
   keys = Keys.from_int_or_key(42)
   with pg:
     pg.console.print("Drop Last: False, Auto Pad: True")
     dl = IdxDataloader(314430, 256, drop_last=False)
 
-    for i in es_loop(dl, pg, epochs=300, keys=keys, prefix="DFAT"):
+    for i in es_loop(dl, pg, epochs=300, keys=keys, prefix="DFAT", start_epoch=10):
       pg.update_res(
         "DFAT-S", {"epoch": i.epoch.item(), "step": i.step.item(), "name": i.name}
       )
       # pg.console.print(i)
       continue
     pg.console.print(i)
     pg.console.print("Drop Last: True, Auto Pad: True")
```

### Comparing `nadl-1.4.3/src/nadl/images.py` & `nadl-1.4.4/src/nadl/images.py`

 * *Files identical despite different names*

### Comparing `nadl-1.4.3/src/nadl/keys.py` & `nadl-1.4.4/src/nadl/keys.py`

 * *Files identical despite different names*

### Comparing `nadl-1.4.3/src/nadl/loops.py` & `nadl-1.4.4/src/nadl/loops.py`

 * *Files identical despite different names*

### Comparing `nadl-1.4.3/src/nadl/metrics.py` & `nadl-1.4.4/src/nadl/metrics.py`

 * *Files identical despite different names*

### Comparing `nadl-1.4.3/src/nadl/nets.py` & `nadl-1.4.4/src/nadl/nets.py`

 * *Files identical despite different names*

### Comparing `nadl-1.4.3/src/nadl/preprocessing.py` & `nadl-1.4.4/src/nadl/preprocessing.py`

 * *Files identical despite different names*

### Comparing `nadl-1.4.3/src/nadl/states.py` & `nadl-1.4.4/src/nadl/states.py`

 * *Files identical despite different names*

### Comparing `nadl-1.4.3/src/nadl/transformers.py` & `nadl-1.4.4/src/nadl/transformers.py`

 * *Files identical despite different names*

### Comparing `nadl-1.4.3/src/nadl/utils.py` & `nadl-1.4.4/src/nadl/utils.py`

 * *Files identical despite different names*

### Comparing `nadl-1.4.3/PKG-INFO` & `nadl-1.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nadl
-Version: 1.4.3
+Version: 1.4.4
 Summary: Nasy's Deep Learning Toolkit
 Author-Email: Nasy <nasyxx+python@gmail.com>, Nasy <nasyxx+dl@gmail.com>, Nasy <nasyxx+git@gmail.com>
 License: GPLv3
 Requires-Python: >=3.12
 Requires-Dist: jax>=0.4.28
 Requires-Dist: numpy>=1.26.4
 Requires-Dist: rich>=13.7.1
```

