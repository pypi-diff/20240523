# Comparing `tmp/nadl-1.4.1.tar.gz` & `tmp/nadl-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nadl-1.4.1.tar", last modified: Wed May 22 03:11:58 2024, max compression
+gzip compressed data, was "nadl-1.4.2.tar", last modified: Wed May 22 20:30:42 2024, max compression
```

## Comparing `nadl-1.4.1.tar` & `nadl-1.4.2.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0     2275 2024-05-22 03:11:58.171534 nadl-1.4.1/pyproject.toml
--rw-r--r--   0        0        0      596 2024-04-18 21:07:32.861885 nadl-1.4.1/readme.org
--rw-r--r--   0        0        0     1806 2024-05-22 03:11:17.681084 nadl-1.4.1/src/nadl/__init__.py
--rw-r--r--   0        0        0     8364 2024-04-22 04:28:48.528762 nadl-1.4.1/src/nadl/blocks.py
--rw-r--r--   0        0        0     5149 2024-05-21 19:59:54.581010 nadl-1.4.1/src/nadl/data.py
--rw-r--r--   0        0        0     2180 2024-04-26 22:33:55.875764 nadl-1.4.1/src/nadl/images.py
--rw-r--r--   0        0        0     3483 2024-05-21 19:45:50.651928 nadl-1.4.1/src/nadl/keys.py
--rw-r--r--   0        0        0     5135 2024-05-21 15:18:23.436274 nadl-1.4.1/src/nadl/loops.py
--rw-r--r--   0        0        0     1828 2024-04-19 19:57:58.670986 nadl-1.4.1/src/nadl/metrics.py
--rw-r--r--   0        0        0     3629 2024-04-22 04:28:48.528396 nadl-1.4.1/src/nadl/nets.py
--rw-r--r--   0        0        0     3401 2024-04-19 20:04:00.936571 nadl-1.4.1/src/nadl/preprocessing.py
--rw-r--r--   0        0        0        0 2023-12-07 01:36:32.295961 nadl-1.4.1/src/nadl/py.typed
--rw-r--r--   0        0        0     3884 2024-05-15 03:21:02.151713 nadl-1.4.1/src/nadl/states.py
--rw-r--r--   0        0        0     1108 2024-04-22 04:28:48.527949 nadl-1.4.1/src/nadl/transformers.py
--rw-r--r--   0        0        0     2363 2024-05-14 05:16:59.307787 nadl-1.4.1/src/nadl/utils.py
--rw-r--r--   0        0        0     1368 1970-01-01 00:00:00.000000 nadl-1.4.1/PKG-INFO
+-rw-r--r--   0        0        0     2275 2024-05-22 20:30:42.078871 nadl-1.4.2/pyproject.toml
+-rw-r--r--   0        0        0      596 2024-04-18 21:07:32.861885 nadl-1.4.2/readme.org
+-rw-r--r--   0        0        0     6148 2024-05-22 06:49:46.036737 nadl-1.4.2/src/nadl/.DS_Store
+-rw-r--r--   0        0        0     1806 2024-05-22 20:29:53.835862 nadl-1.4.2/src/nadl/__init__.py
+-rw-r--r--   0        0        0     8364 2024-04-22 04:28:48.528762 nadl-1.4.2/src/nadl/blocks.py
+-rw-r--r--   0        0        0     5884 2024-05-22 20:29:33.026250 nadl-1.4.2/src/nadl/data.py
+-rw-r--r--   0        0        0     2180 2024-04-26 22:33:55.875764 nadl-1.4.2/src/nadl/images.py
+-rw-r--r--   0        0        0     3564 2024-05-22 05:17:23.233277 nadl-1.4.2/src/nadl/keys.py
+-rw-r--r--   0        0        0     5135 2024-05-21 15:18:23.436274 nadl-1.4.2/src/nadl/loops.py
+-rw-r--r--   0        0        0     1828 2024-04-19 19:57:58.670986 nadl-1.4.2/src/nadl/metrics.py
+-rw-r--r--   0        0        0     3629 2024-04-22 04:28:48.528396 nadl-1.4.2/src/nadl/nets.py
+-rw-r--r--   0        0        0     3401 2024-04-19 20:04:00.936571 nadl-1.4.2/src/nadl/preprocessing.py
+-rw-r--r--   0        0        0        0 2023-12-07 01:36:32.295961 nadl-1.4.2/src/nadl/py.typed
+-rw-r--r--   0        0        0     3884 2024-05-15 03:21:02.151713 nadl-1.4.2/src/nadl/states.py
+-rw-r--r--   0        0        0     1108 2024-04-22 04:28:48.527949 nadl-1.4.2/src/nadl/transformers.py
+-rw-r--r--   0        0        0     2363 2024-05-14 05:16:59.307787 nadl-1.4.2/src/nadl/utils.py
+-rw-r--r--   0        0        0     1368 1970-01-01 00:00:00.000000 nadl-1.4.2/PKG-INFO
```

### Comparing `nadl-1.4.1/pyproject.toml` & `nadl-1.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     "optax>=0.2.2",
     "equinox>=0.11.4",
     "beartype>=0.18.5",
     "scikit-image>=0.23.2",
     "orbax-checkpoint>=0.5.11",
 ]
 requires-python = ">=3.12"
-version = "1.4.1"
+version = "1.4.2"
 
 [project.readme]
 content-type = "text/plain"
 file = "readme.org"
 
 [project.license]
 text = "GPLv3"
@@ -54,15 +54,15 @@
 name = "jaxlib"
 verify_ssl = true
 type = "find_links"
 
 [tool.pdm.dev-dependencies]
 dev = [
     "scipy>=1.13.0",
-    "scikit-learn>=1.4.2",
+    "scikit-learn>=1.5.0",
     "ipdb>=0.13.13",
 ]
 
 [tool.mypy]
 exclude = [
     "__pypackages__/",
     "./typings",
```

### Comparing `nadl-1.4.1/readme.org` & `nadl-1.4.2/readme.org`

 * *Files identical despite different names*

### Comparing `nadl-1.4.1/src/nadl/__init__.py` & `nadl-1.4.2/src/nadl/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 from .states import BaseTrainState, state_fn
 from .utils import (
   classit,
   rle,
   rle_array,
 )
 
-__version__ = "1.4.1"
+__version__ = "1.4.2"
 
 __all__ = [
   "PG",
   "RESC",
   "SCALER",
   "BaseTrainState",
   "DState",
```

### Comparing `nadl-1.4.1/src/nadl/blocks.py` & `nadl-1.4.2/src/nadl/blocks.py`

 * *Files identical despite different names*

### Comparing `nadl-1.4.1/src/nadl/data.py` & `nadl-1.4.2/src/nadl/data.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 
 from collections.abc import Callable, Iterator
 
 import equinox as eqx
 import jax
 import jax.numpy as jnp
 from equinox import field, tree_at
+import numpy as np
 
 from typing import NamedTuple
 
 from .keys import Keys
 from .loops import PG, RESC, PGThread
 
 
@@ -55,14 +56,29 @@
   pad: jax.Array
   shape: tuple[int, ...]
   epoch: jax.Array = field(default_factory=lambda: jnp.array(0))
   step: jax.Array = field(default_factory=lambda: jnp.array(0))
   name: str | None = None
 
 
+def _np_sort(x: jax.Array, axis: int | None = None) -> np.ndarray:
+  """Sort the array."""
+  return np.argsort(np.asarray(x), axis=axis)
+
+
+@eqx.filter_jit
+def fallback_argsort(x: jax.Array, axis: int | None = None) -> jax.Array:
+  """Fallback to numpy argsort when CPU."""
+  if jax.devices()[0].platform == "cpu":
+    return jax.pure_callback(
+      _np_sort, jax.ShapeDtypeStruct(x.shape, jnp.int32), x, axis
+    )
+  return x.argsort(axis=axis)
+
+
 class IdxDataloader[T](eqx.Module):
   """Simple index dataloader."""
 
   length: int
   pad: int
   batch_size: int
   drop_num: int = 0
@@ -87,18 +103,23 @@
 
     self.batch_size = batch_size
     self.transform = eqx.filter_jit(transform)
 
   @eqx.filter_jit
   def __call__(self, key: jax.Array | None = None) -> DState[T]:
     """Get the indexes."""
-    if key is None:
-      idxes = jnp.arange(self.length)
-    else:
-      idxes = jax.random.permutation(key, self.length)
+    idxes = jnp.arange(self.length)
+    if key is not None:
+      idxes = jnp.take_along_axis(
+        idxes,
+        # NOTE: Fallback to numpy argsort since it has performance isssue in CPU.
+        # https://github.com/google/jax/issues/10434
+        fallback_argsort(jax.random.uniform(key, (self.length,))),
+        axis=0,
+      )
     length = self.length if not self.drop_num else self.length - self.drop_num
 
     idxes = jnp.r_[idxes, jnp.full(self.pad, -1, idxes.dtype)]
     idxes = idxes[: length + self.pad].reshape(-1, self.batch_size)
     return DState(self.transform(idxes), jnp.where(idxes == -1, 1, 0), idxes.shape)
 
 
@@ -111,64 +132,64 @@
   prefix: str = "L",
   es: str = "E",
   ss: str = "S",
 ) -> Iterator[DState[T]]:
   """Simple epoch loop."""
   es, ss = f"{prefix}-{es}", f"{prefix}-{ss}"
   assert epochs > 0, "Epochs should be greater than 0."
-  if epochs > 1:
-    if es in pg.tasks:
-      pg.pg.reset(pg.tasks[es])
-    else:
-      pg.add_task(es, total=epochs, res="")
-    pg.advance(pg.tasks[es], start_epoch - 1)
-
-  vdl = eqx.filter_jit(eqx.filter_vmap(loader, axis_size=1))
   if keys:
     keys.reserve(epochs)
+
+  vdl = eqx.filter_jit(eqx.filter_vmap(loader, axis_size=1))
+  pg.console.log("Building dataloader caches...")
   ds: DState[T] = vdl() if keys is None else vdl(keys(jnp.arange(epochs)))
   ds = tree_at(lambda d: d.name, ds, prefix, is_leaf=lambda x: x is None)
 
+  if epochs > 1:
+    if es in pg.tasks:
+      pg.pg.reset(pg.tasks[es], total=epochs)
+    else:
+      pg.add_task(es, total=epochs, res="")
+    pg.advance(pg.tasks[es], start_epoch - 1)
   if ss in pg.tasks:
-    pg.pg.reset(pg.tasks[ss])
+    pg.pg.reset(pg.tasks[ss], total=ds.shape[0] * epochs, res="")
   else:
     pg.add_task(ss, total=ds.shape[0] * epochs, res="")
   pg.advance(pg.tasks[ss], (start_step := max((start_epoch - 1), 0) * ds.shape[0]))
 
   @eqx.filter_jit
-  def _select(ds: DState[T], i: jax.Array, ii: jax.Array) -> DState[T]:
+  def _select(i: jax.Array, ii: jax.Array) -> DState[T]:
     return tree_at(
       lambda x: (x.epoch, x.step),
       jax.tree.map(lambda x: x[i, ii] if isinstance(x, jax.Array) else x, ds),
       (i, i * ds.shape[0] + ii),
     )
 
   with PGThread(pg.pg, pg.tasks[ss]) as pts, PGThread(pg.pg, pg.tasks[es]) as pte:
     for i in jnp.arange(start_epoch, epochs + 1):
-      # nds = loader(keys and keys(i) or None)
       for ii in jnp.arange(start_step, ds.shape[0]):
-        yield _select(ds, i, ii)
+        yield _select(i, ii)
         pts.completed += 1
       if epochs > 1:
         pte.completed += 1
 
 
 def __test() -> None:
   """Test."""
   pg = PG.init_progress(extra_columns=(RESC,))
   keys = Keys.from_int_or_key(42)
   with pg:
     pg.console.print("Drop Last: False, Auto Pad: True")
-    dl = IdxDataloader(10, 3, drop_last=False)
+    dl = IdxDataloader(314430, 256, drop_last=False)
 
-    for i in es_loop(dl, pg, epochs=2, prefix="DFAT"):
+    for i in es_loop(dl, pg, epochs=300, keys=keys, prefix="DFAT"):
       pg.update_res(
         "DFAT-S", {"epoch": i.epoch.item(), "step": i.step.item(), "name": i.name}
       )
-      pg.console.print(i)
+      # pg.console.print(i)
       continue
     pg.console.print(i)
     pg.console.print("Drop Last: True, Auto Pad: True")
     dl = IdxDataloader(10, 3, drop_last=True)
     for i in es_loop(dl, pg, keys, prefix="DTAT"):
       pg.console.print(i)
```

### Comparing `nadl-1.4.1/src/nadl/images.py` & `nadl-1.4.2/src/nadl/images.py`

 * *Files identical despite different names*

### Comparing `nadl-1.4.1/src/nadl/keys.py` & `nadl-1.4.2/src/nadl/keys.py`

 * *Files 3% similar despite different names*

```diff
@@ -108,14 +108,18 @@
     return self.next_key()
 
   def take(self, num: int) -> jax.Array:
     """Take num keys."""
     self.reserve(jnp.max(num - len(self.keys), 0))
     return jnp.r_[*self.keys[-num:]]
 
+  def __len__(self) -> int:
+    """Length of keys."""
+    return len(self.keys)
+
   def __call__(self, epoch: int | jax.Array | None = None) -> jax.Array:
     """Get keys for epoch."""
     match epoch:
       case int():
         if epoch + 1 > len(self.keys):
           self.reserve(epoch + 1 - len(self.keys))
         return self.keys[epoch]
```

### Comparing `nadl-1.4.1/src/nadl/loops.py` & `nadl-1.4.2/src/nadl/loops.py`

 * *Files identical despite different names*

### Comparing `nadl-1.4.1/src/nadl/metrics.py` & `nadl-1.4.2/src/nadl/metrics.py`

 * *Files identical despite different names*

### Comparing `nadl-1.4.1/src/nadl/nets.py` & `nadl-1.4.2/src/nadl/nets.py`

 * *Files identical despite different names*

### Comparing `nadl-1.4.1/src/nadl/preprocessing.py` & `nadl-1.4.2/src/nadl/preprocessing.py`

 * *Files identical despite different names*

### Comparing `nadl-1.4.1/src/nadl/states.py` & `nadl-1.4.2/src/nadl/states.py`

 * *Files identical despite different names*

### Comparing `nadl-1.4.1/src/nadl/transformers.py` & `nadl-1.4.2/src/nadl/transformers.py`

 * *Files identical despite different names*

### Comparing `nadl-1.4.1/src/nadl/utils.py` & `nadl-1.4.2/src/nadl/utils.py`

 * *Files identical despite different names*

### Comparing `nadl-1.4.1/PKG-INFO` & `nadl-1.4.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nadl
-Version: 1.4.1
+Version: 1.4.2
 Summary: Nasy's Deep Learning Toolkit
 Author-Email: Nasy <nasyxx+python@gmail.com>, Nasy <nasyxx+dl@gmail.com>, Nasy <nasyxx+git@gmail.com>
 License: GPLv3
 Requires-Python: >=3.12
 Requires-Dist: jax>=0.4.28
 Requires-Dist: numpy>=1.26.4
 Requires-Dist: rich>=13.7.1
```

