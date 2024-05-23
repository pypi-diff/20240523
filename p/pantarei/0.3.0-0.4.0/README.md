# Comparing `tmp/pantarei-0.3.0.tar.gz` & `tmp/pantarei-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pantarei-0.3.0.tar", last modified: Thu Apr 25 12:09:37 2024, max compression
+gzip compressed data, was "pantarei-0.4.0.tar", last modified: Thu May 23 11:23:01 2024, max compression
```

## Comparing `pantarei-0.3.0.tar` & `pantarei-0.4.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 coslo     (1000) coslo     (1000)        0 2024-04-25 12:09:37.201454 pantarei-0.3.0/
--rw-rw-r--   0 coslo     (1000) coslo     (1000)    35147 2023-03-25 17:07:32.000000 pantarei-0.3.0/LICENSE
--rw-r--r--   0 coslo     (1000) coslo     (1000)     3751 2024-04-25 12:09:37.201454 pantarei-0.3.0/PKG-INFO
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     3040 2024-04-23 18:58:43.000000 pantarei-0.3.0/README.md
-drwxrwxr-x   0 coslo     (1000) coslo     (1000)        0 2024-04-25 12:09:37.201454 pantarei-0.3.0/pantarei/
--rw-rw-r--   0 coslo     (1000) coslo     (1000)      262 2024-04-23 18:51:12.000000 pantarei-0.3.0/pantarei/__init__.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     5417 2024-04-10 21:22:43.000000 pantarei-0.3.0/pantarei/_attempt.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     2218 2024-04-25 06:03:54.000000 pantarei-0.3.0/pantarei/backends.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     2480 2024-04-24 19:24:11.000000 pantarei-0.3.0/pantarei/cache.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     8508 2024-04-23 18:51:59.000000 pantarei-0.3.0/pantarei/core.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)    20484 2024-04-25 11:54:56.000000 pantarei-0.3.0/pantarei/database.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     9085 2024-04-25 05:57:44.000000 pantarei-0.3.0/pantarei/helpers.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     1111 2024-04-23 18:50:56.000000 pantarei-0.3.0/pantarei/hooks.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)    10936 2024-04-23 19:11:45.000000 pantarei-0.3.0/pantarei/job.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     6587 2024-04-23 18:50:56.000000 pantarei-0.3.0/pantarei/parsers.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     5551 2024-04-25 05:52:37.000000 pantarei-0.3.0/pantarei/scheduler.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)    11135 2024-04-25 07:31:07.000000 pantarei-0.3.0/pantarei/syncer.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     5974 2024-04-23 19:13:14.000000 pantarei-0.3.0/pantarei/task.py
-drwxrwxr-x   0 coslo     (1000) coslo     (1000)        0 2024-04-25 12:09:37.201454 pantarei-0.3.0/pantarei.egg-info/
--rw-r--r--   0 coslo     (1000) coslo     (1000)     3751 2024-04-25 12:09:37.000000 pantarei-0.3.0/pantarei.egg-info/PKG-INFO
--rw-rw-r--   0 coslo     (1000) coslo     (1000)      483 2024-04-25 12:09:37.000000 pantarei-0.3.0/pantarei.egg-info/SOURCES.txt
--rw-rw-r--   0 coslo     (1000) coslo     (1000)        1 2024-04-25 12:09:37.000000 pantarei-0.3.0/pantarei.egg-info/dependency_links.txt
--rw-rw-r--   0 coslo     (1000) coslo     (1000)       25 2024-04-25 12:09:37.000000 pantarei-0.3.0/pantarei.egg-info/requires.txt
--rw-rw-r--   0 coslo     (1000) coslo     (1000)        9 2024-04-25 12:09:37.000000 pantarei-0.3.0/pantarei.egg-info/top_level.txt
--rw-rw-r--   0 coslo     (1000) coslo     (1000)      781 2024-04-25 12:09:29.000000 pantarei-0.3.0/pyproject.toml
--rw-rw-r--   0 coslo     (1000) coslo     (1000)      178 2024-04-25 12:09:37.201454 pantarei-0.3.0/setup.cfg
-drwxrwxr-x   0 coslo     (1000) coslo     (1000)        0 2024-04-25 12:09:37.201454 pantarei-0.3.0/tests/
--rw-rw-r--   0 coslo     (1000) coslo     (1000)     7227 2024-04-25 08:24:45.000000 pantarei-0.3.0/tests/test.py
--rw-rw-r--   0 coslo     (1000) coslo     (1000)    12286 2024-04-25 11:56:48.000000 pantarei-0.3.0/tests/test_db.py
+drwxrwxr-x   0 coslo     (1000) coslo     (1000)        0 2024-05-23 11:23:01.152099 pantarei-0.4.0/
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)    35147 2023-03-25 17:07:32.000000 pantarei-0.4.0/LICENSE
+-rw-r--r--   0 coslo     (1000) coslo     (1000)     3751 2024-05-23 11:23:01.152099 pantarei-0.4.0/PKG-INFO
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     3040 2024-04-25 14:47:06.000000 pantarei-0.4.0/README.md
+drwxrwxr-x   0 coslo     (1000) coslo     (1000)        0 2024-05-23 11:23:01.148099 pantarei-0.4.0/pantarei/
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)      380 2024-04-25 15:08:31.000000 pantarei-0.4.0/pantarei/__init__.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     5417 2024-04-10 21:22:43.000000 pantarei-0.4.0/pantarei/_attempt.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     2218 2024-04-25 14:47:06.000000 pantarei-0.4.0/pantarei/backends.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     2780 2024-05-05 14:49:20.000000 pantarei-0.4.0/pantarei/cache.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     8543 2024-04-30 14:20:39.000000 pantarei-0.4.0/pantarei/core.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)    22629 2024-05-14 11:38:36.000000 pantarei-0.4.0/pantarei/database.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     9085 2024-04-25 14:47:06.000000 pantarei-0.4.0/pantarei/helpers.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     1111 2024-04-23 18:50:56.000000 pantarei-0.4.0/pantarei/hooks.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)    11612 2024-05-02 19:00:23.000000 pantarei-0.4.0/pantarei/job.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     6587 2024-04-23 18:50:56.000000 pantarei-0.4.0/pantarei/parsers.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     5415 2024-05-09 17:24:26.000000 pantarei-0.4.0/pantarei/scheduler.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)    11135 2024-04-25 07:31:07.000000 pantarei-0.4.0/pantarei/syncer.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     7864 2024-05-02 17:00:11.000000 pantarei-0.4.0/pantarei/task.py
+drwxrwxr-x   0 coslo     (1000) coslo     (1000)        0 2024-05-23 11:23:01.152099 pantarei-0.4.0/pantarei.egg-info/
+-rw-r--r--   0 coslo     (1000) coslo     (1000)     3751 2024-05-23 11:23:01.000000 pantarei-0.4.0/pantarei.egg-info/PKG-INFO
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)      483 2024-05-23 11:23:01.000000 pantarei-0.4.0/pantarei.egg-info/SOURCES.txt
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)        1 2024-05-23 11:23:01.000000 pantarei-0.4.0/pantarei.egg-info/dependency_links.txt
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)       25 2024-05-23 11:23:01.000000 pantarei-0.4.0/pantarei.egg-info/requires.txt
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)        9 2024-05-23 11:23:01.000000 pantarei-0.4.0/pantarei.egg-info/top_level.txt
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)      781 2024-05-23 11:22:54.000000 pantarei-0.4.0/pyproject.toml
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)      178 2024-05-23 11:23:01.152099 pantarei-0.4.0/setup.cfg
+drwxrwxr-x   0 coslo     (1000) coslo     (1000)        0 2024-05-23 11:23:01.152099 pantarei-0.4.0/tests/
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)     9271 2024-05-05 14:49:49.000000 pantarei-0.4.0/tests/test.py
+-rw-rw-r--   0 coslo     (1000) coslo     (1000)    13618 2024-05-14 11:40:14.000000 pantarei-0.4.0/tests/test_db.py
```

### Comparing `pantarei-0.3.0/LICENSE` & `pantarei-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pantarei-0.3.0/PKG-INFO` & `pantarei-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pantarei
-Version: 0.3.0
+Version: 0.4.0
 Summary: A general-purpose workflow manager
 Author-email: Daniele Coslovich <daniele.coslovich@umontpellier.fr>
 License: GPLv3
 Project-URL: repository, https://framagit.org/coslo/pantarei
 Project-URL: homepage, https://framagit.org/coslo/pantarei
 Project-URL: documentation, https://coslo.frama.io/pantarei
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `pantarei-0.3.0/README.md` & `pantarei-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `pantarei-0.3.0/pantarei/_attempt.py` & `pantarei-0.4.0/pantarei/_attempt.py`

 * *Files identical despite different names*

### Comparing `pantarei-0.3.0/pantarei/backends.py` & `pantarei-0.4.0/pantarei/backends.py`

 * *Files identical despite different names*

### Comparing `pantarei-0.3.0/pantarei/cache.py` & `pantarei-0.4.0/pantarei/cache.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,22 +11,28 @@
 
 def _itemize(data):
     """Itemize numpy arrays in data"""
     if isinstance(data, dict):
         # Turn all ndarrays into lists
         new_data = {}
         for key in data:
-            if isinstance(data, numpy.ndarray):
+            if isinstance(data[key], numpy.ndarray):
                 new_data[key] = numpy.ndarray.tolist(data[key])
+            elif type(data[key]).__module__ == 'numpy':
+                # Could not find a better way to check any dytpe
+                new_data[key] = data[key].item()
             else:
                 new_data[key] = data[key]
         return new_data
     # If data is an ndarray, turn it to a list
     if isinstance(data, numpy.ndarray):
         return numpy.ndarray.tolist(data)
+    if type(data).__module__ == 'numpy':
+        # Could not find a better way to check any dytpe
+        return data.item()
     # Just return data if all else fails
     return data
 
 class Cache:
     """
     Cache results of function evaluation on the basis of its name and
     keyword arguments
```

### Comparing `pantarei-0.3.0/pantarei/core.py` & `pantarei-0.4.0/pantarei/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -260,10 +260,10 @@
 def __report():    
     report(only=('running', 'failed'))
 
 
 # We should not do this during unit tests
 # The jobs will be there but the cache may be gone
 # This will give a spurious final line
-# TODO: register these hooks somewhere else
+# TODO: register these hooks somewhere else, this must not be done globally!
 atexit.register(__report)
-atexit.register(orphans)
+# atexit.register(orphans)
```

### Comparing `pantarei-0.3.0/pantarei/database.py` & `pantarei-0.4.0/pantarei/database.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,77 +3,101 @@
 """
 import os
 import tempfile
 import hashlib
 from itertools import compress
 
 import numpy
-from tinydb import Query
+from tinydb import Query as _Query
 from tinydb.storages import Storage, MemoryStorage
 from tinydb.table import Table
 
 from .helpers import _wget, pprint
 
+# Obnubilate pickle because Query objects cannot be pickled
+# They are throwaway objects for us anyway
+class Query(_Query):
+
+    def __getstate__(self):
+        return {}
+
+    def __setstate__(self, value):
+        pass
 
 # Default query
-# query = Query()
+query = Query()
+
 def where(key):
     return Query()[key]
 
 
 class maskablelist(list):
     """
     Data structure for heterogeneous arrays
     """
 
+    def __init__(self, iterable, crop=False):
+        super().__init__(iterable)
+        self.crop = crop
+
+    # Obnubilate pickle
+    def __setstate__(self, value):
+        pass
+
+    # Obnubilate pickle
+    def __getstate__(self):
+        return {}
+    
     def __getitem__(self, index):
         try:
             return super().__getitem__(index)
         except TypeError:
             return maskablelist(compress(self, index))
 
     def __getattr__(self, name):
         """
         Forward all unknown attribute calls to numpy array
         """
-        x = [numpy.array(entry).shape for entry in self]
-        all_equal = x.count(x[0]) == len(x)
         # TODO: have axis=0 always mean the first one even if not homo
         # TODO: handle case when all shapes are eventually equal because of mask
         # TODO: in callable check value of axis, if axis=0 raise error when not homo and not cropping
         if callable(getattr(numpy.ndarray(1), name)):
             # Return a callable that applies the method on each entry of the masked list
             # along the first dimension and return the results as a list
             def _attr(*args, **kwargs):
                 res = []
                 for i in range(len(self)):
                     res.append(getattr(numpy.array(list(self[i])), name)(*args, **kwargs))
                 return res
-            return _attr
 
-            # Version cropping each dimension to make it a numpy array
-            # def _attr(*args, **kwargs):
-            #     res = []
-            #     min_shape = None
-            #     for entry in self:
-            #         x = numpy.array(list(entry))
-            #         if min_shape is None:
-            #             min_shape = x.shape
-            #         else:
-            #             min_shape = numpy.min([x.shape, min_shape], axis=0)
-            #     #minsize = numpy.min([numpy.array(list(self[i]))[-1] for i in range(len(self))])
-            #     ranges = [range(shape) for shape in min_shape]
-            #     idx = numpy.ix_(*ranges)
-            #     for entry in self:
-            #         # res.append(getattr(numpy.array(list(entry)), name)(*args, **kwargs))
-            #         res.append(numpy.array(list(entry))[idx])
-            #     # return res
-            #     #print(numpy.array(res).shape)
-            #     return getattr(numpy.array(res), name)(*args, **kwargs)
-            # return _attr
+            # Crop each dimension to make it a numpy array
+            def _attr_crop(*args, **kwargs):
+                res = []
+                min_shape = None
+                for entry in self:
+                    #print('*', entry)
+                    x = numpy.array(list(entry))
+                    if min_shape is None:
+                        min_shape = x.shape
+                    else:
+                        min_shape = numpy.min([x.shape, min_shape], axis=0)
+                #minsize = numpy.min([numpy.array(list(self[i]))[-1] for i in range(len(self))])
+                ranges = [range(shape) for shape in min_shape]
+                idx = numpy.ix_(*ranges)
+                for entry in self:
+                    # res.append(getattr(numpy.array(list(entry)), name)(*args, **kwargs))
+                    res.append(numpy.array(list(entry))[idx])
+                # return res
+                #print('--', numpy.array(res).shape)
+                return getattr(numpy.array(res), name)(*args, **kwargs)
+
+            if self.crop:
+                return _attr_crop
+            else:
+                return _attr
 
         else:
             return [getattr(numpy.array(entry), name) for entry in self]
 
     def unique(self, *args, **kwargs):
         # TODO: fix this
         return numpy.unique(self, *args, **kwargs)
@@ -111,56 +135,98 @@
 class Data:
 
     """
     A container for data with a pandas-like interface
     """
 
     # TODO: should we call them key and values and perhaps alias key as columns() (accessor like pandas)
-    def __init__(self, rows, columns):
+    # TODO: hey, if the input is a list of dicts, columns is not needed, can it be dropped from args?
+    # TODO: shall we support a seq of seq + separate keys?
+    # TODO: store data as _data, accessor data() or view() accepts keys as arguments and return a view on those fields
+    def __init__(self, rows, columns, crop=False):
         """
-        :param rows: dataset as a sequence of sequences
-        :param columns: names of each entry of the dataset
+        :param rows: input data as a sequence of dicts
+        :param columns:
         """
         self.rows = rows
         self.columns = columns
+        self.crop = crop
         self._maskable = False
 
+    def view(self, *args):
+        """Return a Data instance with a view on the given keys/fields/columns"""
+        return Data([{arg: row[arg] for arg in args} for row in self.rows], args)
+
+    def sort(self, *args, reverse=False):
+        """Return a Data instance sorted according to the given keys/fields/columns"""
+        entries = sorted(self.rows, key=lambda x: [x[key] for key in args], reverse=reverse)
+        return Data(entries, self.columns)
+    
+    def __deepcopy__(self, memo):
+        """Needed because we have cleared __getstate__"""
+        from copy import deepcopy
+        cls = self.__class__
+        result = cls.__new__(cls)
+        memo[id(self)] = result
+        for k, v in self.__dict__.items():
+            setattr(result, k, deepcopy(v, memo))
+        return result        
+    
+    def copy(self):
+        """Return a deep copy of `self`"""
+        from copy import deepcopy
+        return deepcopy(self)
+    
     def __repr__(self):
         from .helpers import pprint
         from io import StringIO
         with StringIO() as io:
             pprint(self.rows, columns=self.columns, file=io)
             txt = io.getvalue()
         return txt
 
     def __len__(self):
         return len(self.rows)
 
+    # Obnubilate pickle
+    def __setstate__(self, value):
+        pass
+
+    # Obnubilate pickle
+    def __getstate__(self):
+        return {}
+
+    # def __getattr__(self, name):
+    #     """
+    #     Forward all unknown attribute calls to numpy array
+    #     """
+    #     pass
+
     def __getitem__(self, key):
         if type(self.rows) == list:
             if isinstance(key, str):                
                 # We access a single row by key
                 if self._maskable:
-                    return maskablelist([row[key] for row in self.rows])
+                    return maskablelist([row[key] for row in self.rows], crop=self.crop)
                 try:
                     # Homogenous
                     return ndarray(numpy.array([row[key] for row in self.rows]))
                 except ValueError:
                     # Non-homogeneous
-                    return maskablelist([row[key] for row in self.rows])
+                    return maskablelist([row[key] for row in self.rows], crop=self.crop)
             elif isinstance(key, int):
                 # Access list index
                 return self.rows[key]
             elif isinstance(key, slice):
                 # Slice
                 return Data(self.rows[key], self.columns)
             else:
                 # This is a mask
                 assert len(key) == len(self.rows), f'{key}'
-                return maskablelist([row[key] for row in self.rows])
+                return maskablelist([row[key] for row in self.rows], crop=self.crop)
         else:
             return self.rows.__getitem__(key)
 
 
 # Temporarily for compat
 NanoDF = Data
 
@@ -343,14 +409,22 @@
         """Alias of `find`"""
         return self.find(*args, **kwargs)
 
     def row(self, *args, **kwargs):
         """Alias of `find_one`"""
         return self.find_one(*args, **kwargs)
 
+    # Obnubilate pickle
+    def __setstate__(self, value):
+        pass
+
+    # Obnubilate pickle
+    def __getstate__(self):
+        return {}
+    
     def __getitem__(self, key):
         return self.rows()[key]
 
     def groupby(self, key, condition=None, reverse=False):
         """
         Return a `Data` instance with entries with common `key` grouped
         along an extra first dimension
```

### Comparing `pantarei-0.3.0/pantarei/helpers.py` & `pantarei-0.4.0/pantarei/helpers.py`

 * *Files identical despite different names*

### Comparing `pantarei-0.3.0/pantarei/hooks.py` & `pantarei-0.4.0/pantarei/hooks.py`

 * *Files identical despite different names*

### Comparing `pantarei-0.3.0/pantarei/job.py` & `pantarei-0.4.0/pantarei/job.py`

 * *Files 4% similar despite different names*

```diff
@@ -154,15 +154,14 @@
             self.kwargs = kwargs
 
         # Add this to global list, make a snapshot for transient jobs
         from copy import deepcopy
         core._jobs.append(deepcopy(self))
         core.jobs.append(self.qualified_name())
 
-        # TODO: if job is running (ex. on a remote cluster) we should skip right away
         assert self.mode in ['safe', 'brave', 'timid', 'clean', 'veryclean', 'scratch']
         if self.mode == 'timid':
             pass
         elif self.mode == 'scratch':
             self.clear(**self.kwargs)
             self._submit()
         elif self.state == 'failed' and self.mode == 'safe':
@@ -172,49 +171,73 @@
             print(f'WARNING: skipping failed job {self.qualified_name()}')
         elif self.state == 'failed' and self.mode == 'clean':
             self.clear(**self.kwargs)
         elif self.mode == 'veryclean':
             self.clear(**self.kwargs)
         elif self.task.done(**self.kwargs):
             return self.task(**self.kwargs)
+        elif self.state in ['running', 'queued']:
+            # Job is running (ex. on a remote cluster), we skip right away
+            pass
+        elif self.scheduler.queued(self.qualified_name()):
+            # Do nothing if job is in queue
+            pass
         else:
             self._submit()
 
         # We reset the arguments if they were passed to __call__
         if len(kwargs) > 0:
             self.kwargs = {}
 
-    def _submit(self):
-        # Do nothing if job is in queue
-        if self.scheduler is not None:
-            if self.scheduler.queued(self.qualified_name()):
-                # print('JOB IS IN QUEUE', self.qualified_name())
-                return
-
+    def _submit(self):        
         # dirname = os.path.join(self.task.cache.path, self.qualified_name())
         mkdir(self.path)
         session_pkl = os.path.join(self.path, '.session.pkl')
         context_pkl = os.path.join(self.path, '.context.pkl')
         job_state = os.path.join(self.path, 'job.yaml')
         job_output = os.path.join(self.path, 'job.out')
         kwargs = serialize_kwargs(self.kwargs)
 
         n = _stack_index
         n = -2  # for
+        # s = stacks[n]
         stacks = inspect.stack()
         s = stacks[n]
         for n in range(len(stacks)-1, -1, -1):
             if 'job' in stacks[n].frame.f_locals:
                 s = stacks[n]
-                from .helpers import debug_stacks
-                # debug_stacks(stacks)
+                # print('FOUND', n)
+                # from .helpers import debug_stacks
+                # debug_stacks([s])
                 break            
 
-        # s = stacks[n]
+        # fix issues with emacs python shell execution
+        # TODO: this should not be needed anymore
+        var = s.frame.f_locals
+        if '__pyfile' in var:
+            # s = stacks[-2]
+            s = stacks[n - 1]
+            garbage = var.pop('__pyfile')
+            del garbage
 
+        # Attempt to clear the imported module session for pickling
+        # var = s.frame.f_locals
+        # if '__builtins__' in var:
+        #     for clear in ['__builtins__', '__cached__']:
+        #         garbage = var.pop(clear)
+        #         del garbage
+        #         var['__cached__'] = None
+        #         var['__name__'] = '__main__'
+        #         var['__package__'] = None
+        #         var['__spec__'] = None
+                
+        #import pprint
+        #pprint.pprint(s.frame.f_locals)
+        #pprint.pprint(s.frame.f_globals)
+            
         from types import ModuleType
         context = ModuleType('context')
         # context.__dict__.update(s.frame.f_globals)
         # args = s.frame.f_locals
         # import pprint
         # pprint.pprint(s.frame.f_locals)
         # pprint.pprint(s.frame.f_globals)
@@ -230,31 +253,24 @@
         # print('query' in s.frame.f_globals)
         # print('query' in s.frame.f_locals)
         # Nothing of this works
         # query = s.frame.f_globals.pop('query')
         # del query
         # s.frame.f_locals.pop('query')
         dill.dump_module(context_pkl, module=context, refimported=True)
-
+        # print(context_pkl)
+        # print(session_pkl)
         # from .helpers import debug_stacks
         # debug_stacks(stacks)
 
         # print('---------------')
         # print(s.frame)
         # print(s.frame.f_locals)
         # print('---------------')
 
-        # fix issues with emacs python shell execution
-        var = s.frame.f_locals
-        if '__pyfile' in var:
-            # s = stacks[-2]
-            s = stacks[n - 1]
-            garbage = var.pop('__pyfile')
-            del garbage
-
         # TODO: at the line of the called there should be a Job instance
         # else it
         # for s in stacks[:0:-1]:
         #     print(s.frame, s.frame.f_lineno, s.frame.f_code.co_name)
         #     #print(s.frame.f_code)
         #     j = s.frame.f_lineno - s.frame.f_code.co_firstlineno
         #     src, _ = inspect.getsourcelines(s.frame.f_code)
@@ -288,15 +304,15 @@
 
 fh = open('{job_state}', 'a')
 print('job_node:', hostname, file=fh, flush=True)
 print('job_start:', time.time(), file=fh, flush=True)
 try:
     dill.load_module('{session_pkl}')
     context = dill.load_module('{context_pkl}')
-    import pprint
+    #import pprint
     #pprint.pprint(locals())
     #pprint.pprint(globals())
     #print()
     #pprint.pprint(context.__dict__)
     context.job.task({kwargs})
     #job.task({kwargs})
 except:
```

### Comparing `pantarei-0.3.0/pantarei/parsers.py` & `pantarei-0.4.0/pantarei/parsers.py`

 * *Files identical despite different names*

### Comparing `pantarei-0.3.0/pantarei/scheduler.py` & `pantarei-0.4.0/pantarei/scheduler.py`

 * *Files 8% similar despite different names*

```diff
@@ -65,15 +65,21 @@
                 # print('must', len(self.queue()), len(self.queue()) > max_jobs)
                 must_wait = len(self.queue()) > max_jobs
 
             if must_wait:
                 if self.verbose and not muted:
                     print('waiting...')
                     muted = True
-                time.sleep(seconds)
+                from . import core
+                if core.mode == 'timid':
+                    import sys
+                    print('...cannot proceed further in timid mode\n')
+                    sys.exit()
+                else:
+                    time.sleep(seconds)
             else:
                 break
 
     def queue(self):
         """Return a list of jobs in the scheduler queue"""
         output = subprocess.check_output(self.backend['queue'], shell=True)
         queued_jobs = output.decode().split('\n')[:-1]
@@ -127,38 +133,32 @@
                 continue
             value = params[name]
             if value is not None:
                 args.append(f'{directive} {flag} {value}')
 
         # TODO: strip spaces when preceeded by = (like '-l nodes= 1' should be '-l nodes=1')
 
+        # Define prologue and epilogue
+        prologue = ''
+        epilogue = ''
+        
         # The backend uses batch jobs
         header = '\n'.join(args)
         # Interpolate script with job header
-        body = script
-        shebang = '#!/usr/bin/env python'
         if script.startswith('#!'):
             lines = script.split('\n')
             shebang = lines.pop(0)
             body = '\n'.join(lines)
+        else:
+            body = script
+            shebang = '#!/usr/bin/env python'
+            
         # Submit the job
         output = subprocess.check_output(f"""{self.backend['submit']} <<'EOF'
 {shebang}
 {header}
+{prologue}
 {body}
+{epilogue}
 EOF""", shell=True)
         if self.verbose:
             print(output)
-
-    # def _queue(self):
-    #     output = subprocess.check_output('squeue -h -u $USER -o %j', shell=True)
-    #     queued_jobs = output.decode().split('\n')[:-1]
-    #     return queued_jobs
-
-    # def _header(self, job_name, job_output=None, job_error=None, ncores=1):
-    #     header = ""
-    #     header += f"#SBATCH -J {job_name}\n"
-    #     if job_output:
-    #         header += f"#SBATCH -o {job_output}\n"
-    #     if job_error:
-    #         header += f"#SBATCH -e {job_error}\n"
-    #     return header
```

### Comparing `pantarei-0.3.0/pantarei/syncer.py` & `pantarei-0.4.0/pantarei/syncer.py`

 * *Files identical despite different names*

### Comparing `pantarei-0.3.0/pantarei/task.py` & `pantarei-0.4.0/pantarei/task.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,60 @@
 """
 Task
 """
 import os
 import time
+import numpy
 from .helpers import actual_kwargs, all_actual_kwargs, rmd, rmf, tag_function
 from .cache import default_cache
 
 
+def _iterable(x):
+    return hasattr(x, '__iter__') and not isinstance(x, str)
+
+def _serialize_scientific(**kwargs):
+    """
+    Unique name of task based on predictable rounding, courtesy of
+    `numpy.format_float_scientific()`.
+    """
+    from hashlib import md5
+
+    # Old version
+    # Sort dict keys else the fqn is not permutation invariant
+    # selected_kwargs = {key: selected_kwargs[key] for key in sorted(selected_kwargs)}
+    # hash_args = md5(str(selected_kwargs).encode()).hexdigest()    
+    params = dict(unique=True, precision=12)
+    numpy.set_printoptions(formatter={'float_kind': lambda x: numpy.format_float_scientific(x, **params)})
+    # serialized_args = []
+    selected_kwargs = {}
+    # Sort dict keys to nesure permutation invariance (not need since 3. something, but still to be sure)
+    for key in sorted(kwargs):
+        var = kwargs[key]
+        if not _iterable(var):
+            if isinstance(var, float):
+                var = numpy.format_float_scientific(var, **params)
+            else:
+                var = repr(var)
+        else:
+            if hasattr(var, 'shape') and len(var.shape) == 0:
+                var = numpy.format_float_scientific(var, **params)
+            else:
+                # Delegate all the rest to numpy.
+                # It is more time-consuming, but will work systematically
+                var = repr(numpy.array(var))
+        selected_kwargs[key] = var
+        # serialized_args.append(key + ': ' + var)
+    numpy.set_printoptions()
+    # serialized_args = ', '.join(serialized_args)
+    serialized_args = str(selected_kwargs)
+    # with numpy.printoptions(formatter={'float_kind': lambda x: numpy.format_float_scientific(x, **params)}):
+    #     serialized_args = str(selected_kwargs)
+    hash_args = md5(serialized_args.encode()).hexdigest()
+    return hash_args, serialized_args
+
 class Task:
 
     """Cached execution of function"""
 
     def __init__(self, func, cache=None, done=None, clear=None, ignore=None,
                  artifacts=None, tag="", clear_first=False):
         """
@@ -72,29 +116,33 @@
         try:
             self.artifacts = results['artifacts']
         except:
             pass
         return results
 
     def qualified_name(self, **kwargs):
-        """Unique name of task"""
+        """
+        Unique name of task based on keyword arguments `kwargs`
+
+        Serialization takes place with a custom procedure so that
+        floating point arguments are rounded consistently to 12
+        significant digits (could be parametrized). Also, 0-sized
+        arrays and floats are indistinguishable as input arguments.
+        """
         from hashlib import md5
         if self.ignore is None:
             selected_kwargs = kwargs
         else:
             selected_kwargs = {}
             for key in kwargs:
                 if key not in self.ignore:
                     selected_kwargs[key] = kwargs[key]
 
-        # Sort dict keys else the fqn is not permutation invariant
-        # TODO: how to deal with rounding of floats? One option is to use
-        # numpy.format_float_scientific() but it only works with scalars
-        selected_kwargs = {key: selected_kwargs[key] for key in sorted(selected_kwargs)}
-        hash_args = md5(str(selected_kwargs).encode()).hexdigest()
+        hash_args, _ = _serialize_scientific(**selected_kwargs)
+        
         func_name = self.func.__name__
         if len(self.tag) > 0:
             return f'{func_name}-{self.tag}/{hash_args}'
         else:
             return f'{func_name}/{hash_args}'
 
     def name(self):
```

### Comparing `pantarei-0.3.0/pantarei.egg-info/PKG-INFO` & `pantarei-0.4.0/pantarei.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pantarei
-Version: 0.3.0
+Version: 0.4.0
 Summary: A general-purpose workflow manager
 Author-email: Daniele Coslovich <daniele.coslovich@umontpellier.fr>
 License: GPLv3
 Project-URL: repository, https://framagit.org/coslo/pantarei
 Project-URL: homepage, https://framagit.org/coslo/pantarei
 Project-URL: documentation, https://coslo.frama.io/pantarei
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `pantarei-0.3.0/pyproject.toml` & `pantarei-0.4.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 name = "pantarei"
 description = "A general-purpose workflow manager"
 readme = "README.md"
-version = "0.3.0"
+version = "0.4.0"
 authors = [
     {name = "Daniele Coslovich", email = "daniele.coslovich@umontpellier.fr"}
 ]
 requires-python = ">=3.8"
 license = {text = "GPLv3"}
 dependencies = [
     "numpy",
```

### Comparing `pantarei-0.3.0/tests/test.py` & `pantarei-0.4.0/tests/test.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,14 +4,35 @@
 from pantarei import *
 
 class Test(unittest.TestCase):
 
     def setUp(self):
         pass
 
+    def test_itemize(self):
+        import numpy
+        from pantarei.cache import _itemize
+        a = numpy.array([numpy.array(1.0)])
+        #print(type(a[0]), type(_itemize(a)[0]))
+        self.assertTrue(isinstance(_itemize(a), list))
+        self.assertTrue(isinstance(_itemize(a)[0], float))        
+        b = {'a': a}
+        self.assertTrue(isinstance(_itemize(b)['a'], list))
+        self.assertTrue(isinstance(_itemize(b)['a'][0], float))
+        a = numpy.array([numpy.array(1)])
+        self.assertTrue(isinstance(_itemize(a)[0], int))
+        b = {'a': a}
+        self.assertTrue(isinstance(_itemize(b)['a'][0], int))
+        import yaml
+
+        a = numpy.array([1.0])[0]
+        self.assertTrue(isinstance(_itemize(a), float))        
+        #print(type(a))
+        #print(yaml.dump(_itemize({'a': a})))
+        
     def test_task_cache(self):
         import time
         def f(x):
             time.sleep(1)
             return x
         cache = Cache('/tmp/data')
         task = Task(f, cache=cache)
@@ -41,14 +62,49 @@
             return x
         cache = Cache('/tmp/data')
         task = Task(f, cache=cache, ignore=['debug'])
         task(x=1, debug=False)
         self.assertTrue(task.done(x=1, debug=True))
         self.assertTrue(task.done(x=1, debug=False))
 
+    def test_task_default_args(self):
+        import time
+        def f(x):
+            return x
+        cache = Cache('/tmp/data')
+        task = Task(f, cache=cache)
+        qn1 = task.qualified_name(x=1)
+        # Now add an optional argument
+        def f(x, y=0):
+            return x
+        # The qualified name must be the same
+        qn2 = task.qualified_name(x=1)
+        self.assertEqual(qn1, qn2)
+
+    def test_precision(self):
+        """
+        If relative difference between input floats is less than 1e-12
+        then two tasks have the same qualified name (same hash). Also
+        check that 0-sized arrays and floats are indistinguishable.
+        """
+        import time
+        import numpy
+        def f(x):
+            return x
+        cache = Cache('/tmp/data')
+        task = Task(f, cache=cache)
+        qn1 = task.qualified_name(x=numpy.pi)
+        qn2 = task.qualified_name(x=numpy.pi + 1e-14)
+        self.assertEqual(qn1, qn2)
+        qn3 = task.qualified_name(x=numpy.pi + 1e-10)
+        self.assertNotEqual(qn1, qn3)
+        qn1 = task.qualified_name(x=numpy.array(numpy.pi))
+        qn2 = task.qualified_name(x=numpy.pi)
+        self.assertEqual(qn1, qn2)
+        
     def test_task_clear_first(self):
         import time
         def f(x):
             return x
         cache = Cache('/tmp/data')
         task = Task(f, cache=cache, clear_first=True)
         task(x=2)
@@ -108,27 +164,28 @@
         self.assertFalse(os.path.exists('/tmp/artifacts'))
         self.assertFalse(os.path.exists(cache._storage(task.qualified_name(x=1))))
 
     #@unittest.skip('Job not working from unittest')
     def test_job(self):
         import pantarei.job
         from pantarei import Task, Job, Scheduler, Cache
-        pantarei.job._stack_index = 2 #-1
+        #pantarei.job._stack_index = 2 #-1
         def f(x):
             import time
             time.sleep(1)
             return x
         task = Task(f, cache=Cache('/tmp/data'))
         job = Job(task, scheduler=Scheduler(backend='nohupx', verbose=False))
         job(x=1)
         job.scheduler.wait(seconds=1.5)
         from pantarei.core import orphans, report
         missing = orphans()
         #self.assertTrue(len(missing) == 0)
         report()
+        
 
     def test_job_cmd(self):
         script = """
 from pantarei import Task, Job, Scheduler, Cache
 
 def f(x):
     import time
```

### Comparing `pantarei-0.3.0/tests/test_db.py` & `pantarei-0.4.0/tests/test_db.py`

 * *Files 12% similar despite different names*

```diff
@@ -180,23 +180,26 @@
         for row in df:
             pass
         self.assertEqual(df.columns, ['tag', 'x'])
         # pandas has it as function, we adhere to this design
         self.assertEqual(list(df['tag'].unique()), ['a', 'b'])
         self.assertEqual(list(df['tag']), ['a', 'a', 'b'])
 
-        # TODO: fix this test!
-        # self.assertEqual(list(df['x'].mean(axis=0)), [1, 2])
+        data = df['x']
+        data.crop = True
+        #print(type(df['x']), data.shape, data.mean(axis=0))
+        self.assertEqual(list(data.mean(axis=0)), [1, 2])
 
         mask = df['tag'] == 'a'
 
         self.assertTrue(numpy.all(df['x'][mask][0] == [1, 2]))
         self.assertTrue(numpy.all(df['x'][mask][1] == [1, 2]))
 
-        # TODO: this fals atm because
+        # TODO: this fals atm, because along the first dimension we get a list
+        # print(data[mask].mean(axis=0))
         #self.assertTrue(numpy.all(df['x'][mask].mean(axis=0) == [1, 2]))
         self.assertTrue(numpy.all(df['x'][df['tag'] == 'b'][0] == [1, 2, 3]))
         self.assertEqual(list(df['tag']), ['a', 'a', 'b'])
 
     def db_variable_string(self):
         db = VeryTinyDB()
         db.insert({'tag': 'a'})
@@ -292,12 +295,41 @@
         # TODO: fix this in maskablelist.unique()
         db = VeryTinyDB()
         db.insert({'z': [1, 2]})
         db.insert({'z': [1, 2, 3]})
         # Broken
         self.assertEqual(db['z'].unique(), [[1, 2], [1, 2, 3]])
 
+    def test_maskable_inhomogeneous(self):
+        # This works
+        db = VeryTinyDB()
+        db.insert({'x': [1, 2]   , 'y': 1})
+        db.insert({'x': [1, 2, 3], 'y': 1})
+        data = db.find()
+        data.crop = True
+        print(data['x'].mean(axis=0))
+
+    def test_maskable_grouby_inhomogeneous(self):
+        # This does not work: any access to attributes or mathods of something
+        # return by groupby() fails, because we try to turn it into an ndarray
+        db = VeryTinyDB()
+        db.insert({'x': [1, 2]   , 'y': 1})
+        db.insert({'x': [1, 2, 3], 'y': 1})
+        data = db.groupby('y')
+        data.crop = True
+        # Groupby returns a list???
+        # print(type(data))
+        # print(data['x'][0])
+        # This fails
+        # print(data['x'].mean(axis=0))
+        from pantarei.database import Data, maskablelist
+        #print(maskablelist(data['x'][0], crop=True).mean(axis=0))
+        #print(Data({'x': data['x'][0]}, ['x'], crop=True)['x'])
+        print([maskablelist(group['x'], crop=True).mean(axis=0) for group in data])
+        for entry in data:
+            print(maskablelist(entry['x'], crop=True).mean(axis=0))
+        
     def tearDown(self):
         rmd('/tmp/dataset')
 
 if __name__ == '__main__':
     unittest.main()
```

