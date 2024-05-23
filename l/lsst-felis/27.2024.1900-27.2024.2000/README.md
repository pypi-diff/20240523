# Comparing `tmp/lsst_felis-27.2024.1900.tar.gz` & `tmp/lsst_felis-27.2024.2000.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lsst_felis-27.2024.1900.tar", last modified: Thu May  9 09:47:03 2024, max compression
+gzip compressed data, was "lsst_felis-27.2024.2000.tar", last modified: Thu May 16 09:34:14 2024, max compression
```

## Comparing `lsst_felis-27.2024.1900.tar` & `lsst_felis-27.2024.2000.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:47:03.492851 lsst_felis-27.2024.1900/
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-09 09:46:57.000000 lsst_felis-27.2024.1900/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-05-09 09:46:57.000000 lsst_felis-27.2024.1900/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-05-09 09:47:03.492851 lsst_felis-27.2024.1900/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3743 2024-05-09 09:46:57.000000 lsst_felis-27.2024.1900/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-05-09 09:46:57.000000 lsst_felis-27.2024.1900/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:47:03.484851 lsst_felis-27.2024.1900/python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:47:03.488851 lsst_felis-27.2024.1900/python/felis/
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-09 09:46:57.000000 lsst_felis-27.2024.1900/python/felis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10279 2024-05-09 09:46:57.000000 lsst_felis-27.2024.1900/python/felis/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    21351 2024-05-09 09:46:57.000000 lsst_felis-27.2024.1900/python/felis/datamodel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:47:03.488851 lsst_felis-27.2024.1900/python/felis/db/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 09:46:57.000000 lsst_felis-27.2024.1900/python/felis/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-05-09 09:46:57.000000 lsst_felis-27.2024.1900/python/felis/db/_variants.py
--rw-r--r--   0 runner    (1001) docker     (127)     5735 2024-05-09 09:46:57.000000 lsst_felis-27.2024.1900/python/felis/db/sqltypes.py
--rw-r--r--   0 runner    (1001) docker     (127)    18907 2024-05-09 09:46:57.000000 lsst_felis-27.2024.1900/python/felis/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 09:46:57.000000 lsst_felis-27.2024.1900/python/felis/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    16795 2024-05-09 09:46:57.000000 lsst_felis-27.2024.1900/python/felis/tap.py
--rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-05-09 09:46:57.000000 lsst_felis-27.2024.1900/python/felis/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     3465 2024-05-09 09:46:57.000000 lsst_felis-27.2024.1900/python/felis/validation.py
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-09 09:47:03.000000 lsst_felis-27.2024.1900/python/felis/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:47:03.488851 lsst_felis-27.2024.1900/python/lsst_felis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-05-09 09:47:03.000000 lsst_felis-27.2024.1900/python/lsst_felis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-09 09:47:03.000000 lsst_felis-27.2024.1900/python/lsst_felis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 09:47:03.000000 lsst_felis-27.2024.1900/python/lsst_felis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-09 09:47:03.000000 lsst_felis-27.2024.1900/python/lsst_felis.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-09 09:47:03.000000 lsst_felis-27.2024.1900/python/lsst_felis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-09 09:47:03.000000 lsst_felis-27.2024.1900/python/lsst_felis.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 09:47:03.000000 lsst_felis-27.2024.1900/python/lsst_felis.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-09 09:47:03.492851 lsst_felis-27.2024.1900/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 09:47:03.488851 lsst_felis-27.2024.1900/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4637 2024-05-09 09:46:57.000000 lsst_felis-27.2024.1900/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    22986 2024-05-09 09:46:57.000000 lsst_felis-27.2024.1900/tests/test_datamodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3879 2024-05-09 09:46:57.000000 lsst_felis-27.2024.1900/tests/test_datatypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     9328 2024-05-09 09:46:57.000000 lsst_felis-27.2024.1900/tests/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-05-09 09:46:57.000000 lsst_felis-27.2024.1900/tests/test_tap.py
--rw-r--r--   0 runner    (1001) docker     (127)     9453 2024-05-09 09:46:57.000000 lsst_felis-27.2024.1900/tests/test_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:34:14.911290 lsst_felis-27.2024.2000/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-16 09:34:06.000000 lsst_felis-27.2024.2000/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-05-16 09:34:06.000000 lsst_felis-27.2024.2000/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-05-16 09:34:14.911290 lsst_felis-27.2024.2000/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3743 2024-05-16 09:34:06.000000 lsst_felis-27.2024.2000/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3365 2024-05-16 09:34:06.000000 lsst_felis-27.2024.2000/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:34:14.907290 lsst_felis-27.2024.2000/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:34:14.907290 lsst_felis-27.2024.2000/python/felis/
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-16 09:34:06.000000 lsst_felis-27.2024.2000/python/felis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10279 2024-05-16 09:34:06.000000 lsst_felis-27.2024.2000/python/felis/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21351 2024-05-16 09:34:06.000000 lsst_felis-27.2024.2000/python/felis/datamodel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:34:14.907290 lsst_felis-27.2024.2000/python/felis/db/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 09:34:06.000000 lsst_felis-27.2024.2000/python/felis/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3368 2024-05-16 09:34:06.000000 lsst_felis-27.2024.2000/python/felis/db/_variants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5735 2024-05-16 09:34:06.000000 lsst_felis-27.2024.2000/python/felis/db/sqltypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18910 2024-05-16 09:34:06.000000 lsst_felis-27.2024.2000/python/felis/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 09:34:06.000000 lsst_felis-27.2024.2000/python/felis/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    16795 2024-05-16 09:34:06.000000 lsst_felis-27.2024.2000/python/felis/tap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-05-16 09:34:06.000000 lsst_felis-27.2024.2000/python/felis/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3465 2024-05-16 09:34:06.000000 lsst_felis-27.2024.2000/python/felis/validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-16 09:34:14.000000 lsst_felis-27.2024.2000/python/felis/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:34:14.911290 lsst_felis-27.2024.2000/python/lsst_felis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-05-16 09:34:14.000000 lsst_felis-27.2024.2000/python/lsst_felis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-16 09:34:14.000000 lsst_felis-27.2024.2000/python/lsst_felis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 09:34:14.000000 lsst_felis-27.2024.2000/python/lsst_felis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-16 09:34:14.000000 lsst_felis-27.2024.2000/python/lsst_felis.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-16 09:34:14.000000 lsst_felis-27.2024.2000/python/lsst_felis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-16 09:34:14.000000 lsst_felis-27.2024.2000/python/lsst_felis.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 09:34:14.000000 lsst_felis-27.2024.2000/python/lsst_felis.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-16 09:34:14.911290 lsst_felis-27.2024.2000/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:34:14.911290 lsst_felis-27.2024.2000/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4637 2024-05-16 09:34:06.000000 lsst_felis-27.2024.2000/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22986 2024-05-16 09:34:06.000000 lsst_felis-27.2024.2000/tests/test_datamodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3879 2024-05-16 09:34:06.000000 lsst_felis-27.2024.2000/tests/test_datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9328 2024-05-16 09:34:06.000000 lsst_felis-27.2024.2000/tests/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-05-16 09:34:06.000000 lsst_felis-27.2024.2000/tests/test_tap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9453 2024-05-16 09:34:06.000000 lsst_felis-27.2024.2000/tests/test_validation.py
```

### Comparing `lsst_felis-27.2024.1900/LICENSE` & `lsst_felis-27.2024.2000/LICENSE`

 * *Files identical despite different names*

### Comparing `lsst_felis-27.2024.1900/PKG-INFO` & `lsst_felis-27.2024.2000/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsst-felis
-Version: 27.2024.1900
+Version: 27.2024.2000
 Summary: A vocabulary for describing catalogs and acting on those descriptions
 Author-email: Rubin Observatory Data Management <dm-admin@lists.lsst.org>
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: Homepage, https://felis.lsst.io
 Project-URL: Source, https://github.com/lsst/felis
 Keywords: lsst
 Classifier: Intended Audience :: Science/Research
```

### Comparing `lsst_felis-27.2024.1900/README.rst` & `lsst_felis-27.2024.2000/README.rst`

 * *Files identical despite different names*

### Comparing `lsst_felis-27.2024.1900/pyproject.toml` & `lsst_felis-27.2024.2000/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lsst_felis-27.2024.1900/python/felis/__init__.py` & `lsst_felis-27.2024.2000/python/felis/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst_felis-27.2024.1900/python/felis/cli.py` & `lsst_felis-27.2024.2000/python/felis/cli.py`

 * *Files identical despite different names*

### Comparing `lsst_felis-27.2024.1900/python/felis/datamodel.py` & `lsst_felis-27.2024.2000/python/felis/datamodel.py`

 * *Files identical despite different names*

### Comparing `lsst_felis-27.2024.1900/python/felis/db/_variants.py` & `lsst_felis-27.2024.2000/python/felis/db/_variants.py`

 * *Files identical despite different names*

### Comparing `lsst_felis-27.2024.1900/python/felis/db/sqltypes.py` & `lsst_felis-27.2024.2000/python/felis/db/sqltypes.py`

 * *Files identical despite different names*

### Comparing `lsst_felis-27.2024.1900/python/felis/metadata.py` & `lsst_felis-27.2024.2000/python/felis/metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -338,15 +338,15 @@
         ValueError
             If the constraint type is not recognized.
         TypeError
             If the constraint object is not the expected type.
         """
         args: dict[str, Any] = {
             "name": constraint_obj.name or None,
-            "info": constraint_obj.description or None,
+            "comment": constraint_obj.description or None,
             "deferrable": constraint_obj.deferrable or None,
             "initially": constraint_obj.initially or None,
         }
         constraint: Constraint
         constraint_type = constraint_obj.type
 
         if isinstance(constraint_obj, datamodel.ForeignKeyConstraint):
```

### Comparing `lsst_felis-27.2024.1900/python/felis/tap.py` & `lsst_felis-27.2024.2000/python/felis/tap.py`

 * *Files identical despite different names*

### Comparing `lsst_felis-27.2024.1900/python/felis/types.py` & `lsst_felis-27.2024.2000/python/felis/types.py`

 * *Files identical despite different names*

### Comparing `lsst_felis-27.2024.1900/python/felis/validation.py` & `lsst_felis-27.2024.2000/python/felis/validation.py`

 * *Files identical despite different names*

### Comparing `lsst_felis-27.2024.1900/python/lsst_felis.egg-info/PKG-INFO` & `lsst_felis-27.2024.2000/python/lsst_felis.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsst-felis
-Version: 27.2024.1900
+Version: 27.2024.2000
 Summary: A vocabulary for describing catalogs and acting on those descriptions
 Author-email: Rubin Observatory Data Management <dm-admin@lists.lsst.org>
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: Homepage, https://felis.lsst.io
 Project-URL: Source, https://github.com/lsst/felis
 Keywords: lsst
 Classifier: Intended Audience :: Science/Research
```

### Comparing `lsst_felis-27.2024.1900/python/lsst_felis.egg-info/SOURCES.txt` & `lsst_felis-27.2024.2000/python/lsst_felis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lsst_felis-27.2024.1900/tests/test_cli.py` & `lsst_felis-27.2024.2000/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `lsst_felis-27.2024.1900/tests/test_datamodel.py` & `lsst_felis-27.2024.2000/tests/test_datamodel.py`

 * *Files identical despite different names*

### Comparing `lsst_felis-27.2024.1900/tests/test_datatypes.py` & `lsst_felis-27.2024.2000/tests/test_datatypes.py`

 * *Files identical despite different names*

### Comparing `lsst_felis-27.2024.1900/tests/test_metadata.py` & `lsst_felis-27.2024.2000/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `lsst_felis-27.2024.1900/tests/test_tap.py` & `lsst_felis-27.2024.2000/tests/test_tap.py`

 * *Files identical despite different names*

### Comparing `lsst_felis-27.2024.1900/tests/test_validation.py` & `lsst_felis-27.2024.2000/tests/test_validation.py`

 * *Files identical despite different names*

