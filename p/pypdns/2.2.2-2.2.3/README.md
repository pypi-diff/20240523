# Comparing `tmp/pypdns-2.2.2.tar.gz` & `tmp/pypdns-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypdns-2.2.2.tar", max compression
+gzip compressed data, was "pypdns-2.2.3.tar", max compression
```

## Comparing `pypdns-2.2.2.tar` & `pypdns-2.2.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1576 2019-12-19 12:24:43.000000 pypdns-2.2.2/LICENSE
--rw-r--r--   0        0        0     1382 2023-11-03 13:33:16.392333 pypdns-2.2.2/README.md
--rw-r--r--   0        0        0     1105 2024-02-13 09:37:19.780878 pypdns-2.2.2/pypdns/__init__.py
--rw-r--r--   0        0        0    19255 2024-02-13 09:54:46.114167 pypdns-2.2.2/pypdns/api.py
--rw-r--r--   0        0        0      510 2024-02-13 09:37:41.336968 pypdns-2.2.2/pypdns/errors.py
--rw-r--r--   0        0        0        0 2020-01-30 12:16:15.384858 pypdns-2.2.2/pypdns/py.typed
--rw-r--r--   0        0        0     1478 2024-02-13 10:07:10.030089 pypdns-2.2.2/pyproject.toml
--rw-r--r--   0        0        0     2758 1970-01-01 00:00:00.000000 pypdns-2.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1576 2024-05-23 15:17:59.240904 pypdns-2.2.3/LICENSE
+-rw-r--r--   0        0        0     1382 2024-05-23 15:17:59.240904 pypdns-2.2.3/README.md
+-rw-r--r--   0        0        0     1105 2024-05-23 15:17:59.240904 pypdns-2.2.3/pypdns/__init__.py
+-rw-r--r--   0        0        0    19255 2024-05-23 15:17:59.240904 pypdns-2.2.3/pypdns/api.py
+-rw-r--r--   0        0        0      510 2024-05-23 15:17:59.240904 pypdns-2.2.3/pypdns/errors.py
+-rw-r--r--   0        0        0        0 2024-05-23 15:17:59.240904 pypdns-2.2.3/pypdns/py.typed
+-rw-r--r--   0        0        0     1479 2024-05-23 15:17:59.240904 pypdns-2.2.3/pyproject.toml
+-rw-r--r--   0        0        0     2758 1970-01-01 00:00:00.000000 pypdns-2.2.3/PKG-INFO
```

### Comparing `pypdns-2.2.2/LICENSE` & `pypdns-2.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pypdns-2.2.2/README.md` & `pypdns-2.2.3/README.md`

 * *Files identical despite different names*

### Comparing `pypdns-2.2.2/pypdns/__init__.py` & `pypdns-2.2.3/pypdns/__init__.py`

 * *Files identical despite different names*

### Comparing `pypdns-2.2.2/pypdns/api.py` & `pypdns-2.2.3/pypdns/api.py`

 * *Files identical despite different names*

### Comparing `pypdns-2.2.2/pyproject.toml` & `pypdns-2.2.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pypdns"
-version = "2.2.2"
+version = "2.2.3"
 description = "Python API for PDNS."
 authors = ["Raphaël Vinot <raphael.vinot@circl.lu>"]
 license = "GPL-3.0+"
 
 readme = "README.md"
 
 repository = "https://github.com/CIRCL/PyPDNS"
@@ -28,25 +28,25 @@
 pdns = 'pypdns:main'
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/CIRCL/PyPDNS/issues"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-requests-cache = "^1.1.1"
-dnspython = "^2.5.0"
+requests-cache = "^1.2.0"
+dnspython = "^2.6.1"
 Sphinx = [
     {version = "<7.2", python = "<3.9", optional = true},
     {version = "^7.2", python = ">=3.9", optional = true}
 ]
 
 [tool.poetry.group.dev.dependencies]
-mypy = "^1.8.0"
-types-requests = "^2.31.0.20240125"
-pytest = "^8.0.0"
+mypy = "^1.10.0"
+types-requests = "^2.32.0.20240523"
+pytest = "^8.2.1"
 ipython = [
     {version = "<8.13.0", python = "<3.9"},
     {version = "^8.18.0", python = ">=3.9"},
     {version = "^8.19.0", python = ">=3.10"}
 ]
 
 [tool.poetry.extras]
```

### Comparing `pypdns-2.2.2/PKG-INFO` & `pypdns-2.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypdns
-Version: 2.2.2
+Version: 2.2.3
 Summary: Python API for PDNS.
 Home-page: https://github.com/CIRCL/PyPDNS
 License: GPL-3.0+
 Author: Raphaël Vinot
 Author-email: raphael.vinot@circl.lu
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -19,16 +19,16 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet
 Classifier: Topic :: Security
 Provides-Extra: docs
 Requires-Dist: Sphinx (<7.2) ; (python_version < "3.9") and (extra == "docs")
 Requires-Dist: Sphinx (>=7.2,<8.0) ; (python_version >= "3.9") and (extra == "docs")
-Requires-Dist: dnspython (>=2.5.0,<3.0.0)
-Requires-Dist: requests-cache (>=1.1.1,<2.0.0)
+Requires-Dist: dnspython (>=2.6.1,<3.0.0)
+Requires-Dist: requests-cache (>=1.2.0,<2.0.0)
 Project-URL: Bug Tracker, https://github.com/CIRCL/PyPDNS/issues
 Project-URL: Documentation, https://github.com/CIRCL/PyPDNS
 Project-URL: Repository, https://github.com/CIRCL/PyPDNS
 Description-Content-Type: text/markdown
 
 [![Documentation Status](https://readthedocs.org/projects/pypdns/badge/?version=latest)](https://pypdns.readthedocs.io/en/latest/?badge=latest)
```

