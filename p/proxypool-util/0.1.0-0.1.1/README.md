# Comparing `tmp/proxypool_util-0.1.0.tar.gz` & `tmp/proxypool_util-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proxypool_util-0.1.0.tar", last modified: Thu May 23 16:31:06 2024, max compression
+gzip compressed data, was "proxypool_util-0.1.1.tar", last modified: Thu May 23 16:45:19 2024, max compression
```

## Comparing `proxypool_util-0.1.0.tar` & `proxypool_util-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 16:31:06.213233 proxypool_util-0.1.0/
--rw-rw-rw-   0        0        0     1093 2024-05-14 13:07:57.000000 proxypool_util-0.1.0/LICENCE
--rw-rw-rw-   0        0        0     2039 2024-05-23 16:31:06.212237 proxypool_util-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1487 2024-05-14 14:21:10.000000 proxypool_util-0.1.0/README.md
--rw-rw-rw-   0        0        0      626 2024-05-21 20:21:55.000000 proxypool_util-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-23 16:31:06.213233 proxypool_util-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-23 16:31:06.133736 proxypool_util-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2024-05-23 16:31:06.172556 proxypool_util-0.1.0/src/ProxyPool/
--rw-rw-rw-   0        0        0      234 2024-05-13 17:42:56.000000 proxypool_util-0.1.0/src/ProxyPool/ProxyExceptions.py
--rw-rw-rw-   0        0        0     4697 2024-05-14 13:36:03.000000 proxypool_util-0.1.0/src/ProxyPool/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 16:31:06.211237 proxypool_util-0.1.0/src/proxypool_util.egg-info/
--rw-rw-rw-   0        0        0     2039 2024-05-23 16:31:06.000000 proxypool_util-0.1.0/src/proxypool_util.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      303 2024-05-23 16:31:06.000000 proxypool_util-0.1.0/src/proxypool_util.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 16:31:06.000000 proxypool_util-0.1.0/src/proxypool_util.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-05-23 16:31:06.000000 proxypool_util-0.1.0/src/proxypool_util.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-23 16:31:06.209233 proxypool_util-0.1.0/tests/
--rw-rw-rw-   0        0        0     2658 2024-05-14 12:41:58.000000 proxypool_util-0.1.0/tests/test_Proxy.py
--rw-rw-rw-   0        0        0     2473 2024-05-14 12:41:58.000000 proxypool_util-0.1.0/tests/test_ProxyPool.py
+drwxrwxrwx   0        0        0        0 2024-05-23 16:45:19.338646 proxypool_util-0.1.1/
+-rw-rw-rw-   0        0        0     1093 2024-05-14 13:07:57.000000 proxypool_util-0.1.1/LICENCE
+-rw-rw-rw-   0        0        0     2039 2024-05-23 16:45:19.327691 proxypool_util-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1487 2024-05-14 14:21:10.000000 proxypool_util-0.1.1/README.md
+-rw-rw-rw-   0        0        0      626 2024-05-23 16:45:09.000000 proxypool_util-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-23 16:45:19.339703 proxypool_util-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-23 16:45:19.302019 proxypool_util-0.1.1/src/
+drwxrwxrwx   0        0        0        0 2024-05-23 16:45:19.308697 proxypool_util-0.1.1/src/ProxyPool/
+-rw-rw-rw-   0        0        0      234 2024-05-13 17:42:56.000000 proxypool_util-0.1.1/src/ProxyPool/ProxyExceptions.py
+-rw-rw-rw-   0        0        0     4704 2024-05-23 16:44:28.000000 proxypool_util-0.1.1/src/ProxyPool/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 16:45:19.326725 proxypool_util-0.1.1/src/proxypool_util.egg-info/
+-rw-rw-rw-   0        0        0     2039 2024-05-23 16:45:19.000000 proxypool_util-0.1.1/src/proxypool_util.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      303 2024-05-23 16:45:19.000000 proxypool_util-0.1.1/src/proxypool_util.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 16:45:19.000000 proxypool_util-0.1.1/src/proxypool_util.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-05-23 16:45:19.000000 proxypool_util-0.1.1/src/proxypool_util.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-23 16:45:19.325730 proxypool_util-0.1.1/tests/
+-rw-rw-rw-   0        0        0     2658 2024-05-14 12:41:58.000000 proxypool_util-0.1.1/tests/test_Proxy.py
+-rw-rw-rw-   0        0        0     2473 2024-05-14 12:41:58.000000 proxypool_util-0.1.1/tests/test_ProxyPool.py
```

### Comparing `proxypool_util-0.1.0/LICENCE` & `proxypool_util-0.1.1/LICENCE`

 * *Files identical despite different names*

### Comparing `proxypool_util-0.1.0/PKG-INFO` & `proxypool_util-0.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proxypool_util
-Version: 0.1.0
+Version: 0.1.1
 Summary: Proxy pool to rotate and manage proxies
 Author-email: Mykhailo Razbeiko <mykhailo.razb@gmail.com>
 Project-URL: Homepage, https://github.com/MykhailoRp/proxypool_util
 Project-URL: Issues, https://github.com/MykhailoRp/proxypool_util/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `proxypool_util-0.1.0/README.md` & `proxypool_util-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `proxypool_util-0.1.0/pyproject.toml` & `proxypool_util-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "proxypool_util"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Mykhailo Razbeiko", email="mykhailo.razb@gmail.com" },
 ]
 description = "Proxy pool to rotate and manage proxies"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `proxypool_util-0.1.0/src/ProxyPool/__init__.py` & `proxypool_util-0.1.1/src/ProxyPool/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import time
-import ProxyExceptions
+from . import ProxyExceptions
 
 class _ProxyDict(dict):
     def __getitem__(self, item):
         try:
             return dict.__getitem__(self, item)
         except KeyError:
             raise ProxyExceptions.UnknownProxy(f"Unknown proxy: {item}")
```

### Comparing `proxypool_util-0.1.0/src/proxypool_util.egg-info/PKG-INFO` & `proxypool_util-0.1.1/src/proxypool_util.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proxypool_util
-Version: 0.1.0
+Version: 0.1.1
 Summary: Proxy pool to rotate and manage proxies
 Author-email: Mykhailo Razbeiko <mykhailo.razb@gmail.com>
 Project-URL: Homepage, https://github.com/MykhailoRp/proxypool_util
 Project-URL: Issues, https://github.com/MykhailoRp/proxypool_util/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `proxypool_util-0.1.0/tests/test_Proxy.py` & `proxypool_util-0.1.1/tests/test_Proxy.py`

 * *Files identical despite different names*

### Comparing `proxypool_util-0.1.0/tests/test_ProxyPool.py` & `proxypool_util-0.1.1/tests/test_ProxyPool.py`

 * *Files identical despite different names*

