# Comparing `tmp/pyhashlookup-1.2.3.tar.gz` & `tmp/pyhashlookup-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhashlookup-1.2.3.tar", max compression
+gzip compressed data, was "pyhashlookup-1.2.4.tar", max compression
```

## Comparing `pyhashlookup-1.2.3.tar` & `pyhashlookup-1.2.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35149 2024-04-02 13:42:43.669783 pyhashlookup-1.2.3/LICENSE
--rw-r--r--   0        0        0      616 2024-04-02 13:42:43.669783 pyhashlookup-1.2.3/README.md
--rw-r--r--   0        0        0     1018 2024-04-02 13:42:43.669783 pyhashlookup-1.2.3/pyhashlookup/__init__.py
--rw-r--r--   0        0        0     5106 2024-04-02 13:42:43.673783 pyhashlookup-1.2.3/pyhashlookup/api.py
--rw-r--r--   0        0        0        0 2024-04-02 13:42:43.673783 pyhashlookup-1.2.3/pyhashlookup/py.typed
--rw-r--r--   0        0        0     1501 2024-04-02 13:42:43.673783 pyhashlookup-1.2.3/pyproject.toml
--rw-r--r--   0        0        0     2059 1970-01-01 00:00:00.000000 pyhashlookup-1.2.3/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-23 15:26:50.725756 pyhashlookup-1.2.4/LICENSE
+-rw-r--r--   0        0        0      616 2024-05-23 15:26:50.725756 pyhashlookup-1.2.4/README.md
+-rw-r--r--   0        0        0     1018 2024-05-23 15:26:50.725756 pyhashlookup-1.2.4/pyhashlookup/__init__.py
+-rw-r--r--   0        0        0     5106 2024-05-23 15:26:50.725756 pyhashlookup-1.2.4/pyhashlookup/api.py
+-rw-r--r--   0        0        0        0 2024-05-23 15:26:50.725756 pyhashlookup-1.2.4/pyhashlookup/py.typed
+-rw-r--r--   0        0        0     1502 2024-05-23 15:26:50.725756 pyhashlookup-1.2.4/pyproject.toml
+-rw-r--r--   0        0        0     2059 1970-01-01 00:00:00.000000 pyhashlookup-1.2.4/PKG-INFO
```

### Comparing `pyhashlookup-1.2.3/LICENSE` & `pyhashlookup-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyhashlookup-1.2.3/README.md` & `pyhashlookup-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `pyhashlookup-1.2.3/pyhashlookup/__init__.py` & `pyhashlookup-1.2.4/pyhashlookup/__init__.py`

 * *Files identical despite different names*

### Comparing `pyhashlookup-1.2.3/pyhashlookup/api.py` & `pyhashlookup-1.2.4/pyhashlookup/api.py`

 * *Files identical despite different names*

### Comparing `pyhashlookup-1.2.3/pyproject.toml` & `pyhashlookup-1.2.4/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyhashlookup"
-version = "1.2.3"
+version = "1.2.4"
 description = "Python CLI and module for CIRCL hash lookup"
 authors = ["Raphaël Vinot <raphael.vinot@circl.lu>"]
 license = "BSD-3-Clause"
 repository = "https://github.com/hashlookup/PyHashlookup"
 documentation = "https://pyhashlookup.readthedocs.io/en/latest/"
 
 readme = "README.md"
@@ -29,23 +29,23 @@
 
 [tool.poetry.scripts]
 hashlookup = 'pyhashlookup:main'
 
 [tool.poetry.dependencies]
 python = "^3.8"
 dnspython = "^2.6.1"
-requests = "^2.31.0"
+requests = "^2.32.2"
 Sphinx = [
     {version = "<7.2", python = "<3.9", optional = true},
     {version = "^7.2", python = ">=3.9", optional = true}
 ]
 
 [tool.poetry.dev-dependencies]
-mypy = "^1.9.0"
-types-requests = "^2.31.0.20240402"
+mypy = "^1.10.0"
+types-requests = "^2.32.0.20240523"
 pytest-cov = "^5.0.0"
 
 [tool.poetry.extras]
 docs = ["Sphinx"]
 
 [build-system]
 requires = ["poetry_core"]
```

### Comparing `pyhashlookup-1.2.3/PKG-INFO` & `pyhashlookup-1.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhashlookup
-Version: 1.2.3
+Version: 1.2.4
 Summary: Python CLI and module for CIRCL hash lookup
 Home-page: https://github.com/hashlookup/PyHashlookup
 License: BSD-3-Clause
 Author: Raphaël Vinot
 Author-email: raphael.vinot@circl.lu
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -22,15 +22,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet
 Classifier: Topic :: Security
 Provides-Extra: docs
 Requires-Dist: Sphinx (<7.2) ; (python_version < "3.9") and (extra == "docs")
 Requires-Dist: Sphinx (>=7.2,<8.0) ; (python_version >= "3.9") and (extra == "docs")
 Requires-Dist: dnspython (>=2.6.1,<3.0.0)
-Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: requests (>=2.32.2,<3.0.0)
 Project-URL: Documentation, https://pyhashlookup.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/hashlookup/PyHashlookup
 Description-Content-Type: text/markdown
 
 [![Documentation Status](https://readthedocs.org/projects/pyhashlookup/badge/?version=latest)](https://pyhashlookup.readthedocs.io/en/latest/?badge=latest)
 
 # PyHashlookup
```

