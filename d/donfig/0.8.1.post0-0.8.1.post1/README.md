# Comparing `tmp/donfig-0.8.1.post0.tar.gz` & `tmp/donfig-0.8.1.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "donfig-0.8.1.post0.tar", last modified: Wed Oct 25 14:15:19 2023, max compression
+gzip compressed data, was "donfig-0.8.1.post1.tar", last modified: Thu May 23 14:13:47 2024, max compression
```

## Comparing `donfig-0.8.1.post0.tar` & `donfig-0.8.1.post1.tar`

### file list

```diff
@@ -1,28 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-25 14:15:19.148716 donfig-0.8.1.post0/
--rw-r--r--   0 runner    (1001) docker     (127)      671 2023-10-25 14:15:07.000000 donfig-0.8.1.post0/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2023-10-25 14:15:07.000000 donfig-0.8.1.post0/DASK_LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2023-10-25 14:15:07.000000 donfig-0.8.1.post0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       90 2023-10-25 14:15:07.000000 donfig-0.8.1.post0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4948 2023-10-25 14:15:19.148716 donfig-0.8.1.post0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3950 2023-10-25 14:15:07.000000 donfig-0.8.1.post0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-25 14:15:19.144715 donfig-0.8.1.post0/doc/
--rw-r--r--   0 runner    (1001) docker     (127)     6025 2023-10-25 14:15:07.000000 donfig-0.8.1.post0/doc/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-25 14:15:19.148716 donfig-0.8.1.post0/donfig/
--rw-r--r--   0 runner    (1001) docker     (127)      142 2023-10-25 14:15:07.000000 donfig-0.8.1.post0/donfig/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3425 2023-10-25 14:15:07.000000 donfig-0.8.1.post0/donfig/_lock.py
--rw-r--r--   0 runner    (1001) docker     (127)    24644 2023-10-25 14:15:07.000000 donfig-0.8.1.post0/donfig/config_obj.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-25 14:15:19.144715 donfig-0.8.1.post0/donfig/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-25 14:15:07.000000 donfig-0.8.1.post0/donfig/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19003 2023-10-25 14:15:07.000000 donfig-0.8.1.post0/donfig/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2567 2023-10-25 14:15:07.000000 donfig-0.8.1.post0/donfig/tests/test_lock.py
--rw-r--r--   0 runner    (1001) docker     (127)     1732 2023-10-25 14:15:07.000000 donfig-0.8.1.post0/donfig/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      503 2023-10-25 14:15:19.148716 donfig-0.8.1.post0/donfig/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-25 14:15:19.144715 donfig-0.8.1.post0/donfig.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4948 2023-10-25 14:15:19.000000 donfig-0.8.1.post0/donfig.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      426 2023-10-25 14:15:19.000000 donfig-0.8.1.post0/donfig.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-25 14:15:19.000000 donfig-0.8.1.post0/donfig.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       84 2023-10-25 14:15:19.000000 donfig-0.8.1.post0/donfig.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2023-10-25 14:15:19.000000 donfig-0.8.1.post0/donfig.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2110 2023-10-25 14:15:07.000000 donfig-0.8.1.post0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      173 2023-10-25 14:15:19.148716 donfig-0.8.1.post0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2023-10-25 14:15:07.000000 donfig-0.8.1.post0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:13:47.940012 donfig-0.8.1.post1/
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-23 14:13:41.000000 donfig-0.8.1.post1/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-05-23 14:13:41.000000 donfig-0.8.1.post1/DASK_LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-23 14:13:41.000000 donfig-0.8.1.post1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-23 14:13:41.000000 donfig-0.8.1.post1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4948 2024-05-23 14:13:47.940012 donfig-0.8.1.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3950 2024-05-23 14:13:41.000000 donfig-0.8.1.post1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:13:47.940012 donfig-0.8.1.post1/donfig/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-23 14:13:41.000000 donfig-0.8.1.post1/donfig/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-05-23 14:13:41.000000 donfig-0.8.1.post1/donfig/_lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24644 2024-05-23 14:13:41.000000 donfig-0.8.1.post1/donfig/config_obj.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:13:47.940012 donfig-0.8.1.post1/donfig/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 14:13:41.000000 donfig-0.8.1.post1/donfig/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19003 2024-05-23 14:13:41.000000 donfig-0.8.1.post1/donfig/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-05-23 14:13:41.000000 donfig-0.8.1.post1/donfig/tests/test_lock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-05-23 14:13:41.000000 donfig-0.8.1.post1/donfig/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-23 14:13:47.940012 donfig-0.8.1.post1/donfig/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:13:47.940012 donfig-0.8.1.post1/donfig.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4948 2024-05-23 14:13:47.000000 donfig-0.8.1.post1/donfig.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-23 14:13:47.000000 donfig-0.8.1.post1/donfig.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 14:13:47.000000 donfig-0.8.1.post1/donfig.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-23 14:13:47.000000 donfig-0.8.1.post1/donfig.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-23 14:13:47.000000 donfig-0.8.1.post1/donfig.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-05-23 14:13:41.000000 donfig-0.8.1.post1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-23 14:13:47.940012 donfig-0.8.1.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-05-23 14:13:41.000000 donfig-0.8.1.post1/setup.py
```

### Comparing `donfig-0.8.1.post0/AUTHORS.md` & `donfig-0.8.1.post1/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `donfig-0.8.1.post0/DASK_LICENSE.txt` & `donfig-0.8.1.post1/DASK_LICENSE.txt`

 * *Files identical despite different names*

### Comparing `donfig-0.8.1.post0/LICENSE.txt` & `donfig-0.8.1.post1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `donfig-0.8.1.post0/PKG-INFO` & `donfig-0.8.1.post1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: donfig
-Version: 0.8.1.post0
+Version: 0.8.1.post1
 Summary: Python package for configuring a python package
 Maintainer-email: David Hoese <david.hoese@ssec.wisc.edu>
 License: MIT
 Project-URL: Homepage, https://github.com/pytroll/donfig
 Keywords: task-scheduling parallel numpy pandas pydata
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `donfig-0.8.1.post0/README.rst` & `donfig-0.8.1.post1/README.rst`

 * *Files identical despite different names*

### Comparing `donfig-0.8.1.post0/donfig/_lock.py` & `donfig-0.8.1.post1/donfig/_lock.py`

 * *Files identical despite different names*

### Comparing `donfig-0.8.1.post0/donfig/config_obj.py` & `donfig-0.8.1.post1/donfig/config_obj.py`

 * *Files identical despite different names*

### Comparing `donfig-0.8.1.post0/donfig/tests/test_config.py` & `donfig-0.8.1.post1/donfig/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `donfig-0.8.1.post0/donfig/tests/test_lock.py` & `donfig-0.8.1.post1/donfig/tests/test_lock.py`

 * *Files identical despite different names*

### Comparing `donfig-0.8.1.post0/donfig/utils.py` & `donfig-0.8.1.post1/donfig/utils.py`

 * *Files identical despite different names*

### Comparing `donfig-0.8.1.post0/donfig.egg-info/PKG-INFO` & `donfig-0.8.1.post1/donfig.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: donfig
-Version: 0.8.1.post0
+Version: 0.8.1.post1
 Summary: Python package for configuring a python package
 Maintainer-email: David Hoese <david.hoese@ssec.wisc.edu>
 License: MIT
 Project-URL: Homepage, https://github.com/pytroll/donfig
 Keywords: task-scheduling parallel numpy pandas pydata
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `donfig-0.8.1.post0/pyproject.toml` & `donfig-0.8.1.post1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     "cloudpickle",
 ]
 
 [tool.setuptools]
 include-package-data = true
 
 [tool.setuptools.packages]
-find = {}
+find = { namespaces = false }
 
 [tool.mypy]
 # Silence errors about Python 3.9-style delayed type annotations on Python 3.8
 python_version = "3.9"
 # See https://github.com/python/mypy/issues/12286 for automatic multi-platform support
 platform = "linux"
 # platform = win32
```

### Comparing `donfig-0.8.1.post0/setup.py` & `donfig-0.8.1.post1/setup.py`

 * *Files identical despite different names*

