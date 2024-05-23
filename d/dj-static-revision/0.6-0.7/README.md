# Comparing `tmp/dj_static_revision-0.6.tar.gz` & `tmp/dj_static_revision-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dj_static_revision-0.6.tar", max compression
+gzip compressed data, was "dj_static_revision-0.7.tar", max compression
```

## Comparing `dj_static_revision-0.6.tar` & `dj_static_revision-0.7.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1886 2023-07-19 10:51:15.578757 dj_static_revision-0.6/README.rst
--rw-r--r--   0        0        0      145 2020-04-01 16:23:10.000000 dj_static_revision-0.6/dj_static_revision/__init__.py
--rw-r--r--   0        0        0      240 2020-04-18 17:45:36.000000 dj_static_revision-0.6/dj_static_revision/context_processors.py
--rw-r--r--   0        0        0        0 2023-07-19 10:23:07.163312 dj_static_revision-0.6/dj_static_revision/py.typed
--rw-r--r--   0        0        0     1685 2020-04-18 17:43:17.000000 dj_static_revision-0.6/dj_static_revision/utils.py
--rw-r--r--   0        0        0     1482 2023-07-19 10:58:10.489489 dj_static_revision-0.6/pyproject.toml
--rw-r--r--   0        0        0     3030 1970-01-01 00:00:00.000000 dj_static_revision-0.6/PKG-INFO
+-rw-r--r--   0        0        0     1886 2023-07-19 10:51:15.578757 dj_static_revision-0.7/README.rst
+-rw-r--r--   0        0        0      145 2020-04-01 16:23:10.000000 dj_static_revision-0.7/dj_static_revision/__init__.py
+-rw-r--r--   0        0        0      240 2020-04-18 17:45:36.000000 dj_static_revision-0.7/dj_static_revision/context_processors.py
+-rw-r--r--   0        0        0        0 2023-07-19 10:23:07.163312 dj_static_revision-0.7/dj_static_revision/py.typed
+-rw-r--r--   0        0        0     1685 2020-04-18 17:43:17.000000 dj_static_revision-0.7/dj_static_revision/utils.py
+-rw-r--r--   0        0        0     1512 2024-05-23 11:41:46.891489 dj_static_revision-0.7/pyproject.toml
+-rw-r--r--   0        0        0     3109 1970-01-01 00:00:00.000000 dj_static_revision-0.7/PKG-INFO
```

### Comparing `dj_static_revision-0.6/README.rst` & `dj_static_revision-0.7/README.rst`

 * *Files identical despite different names*

### Comparing `dj_static_revision-0.6/dj_static_revision/utils.py` & `dj_static_revision-0.7/dj_static_revision/utils.py`

 * *Files identical despite different names*

### Comparing `dj_static_revision-0.6/pyproject.toml` & `dj_static_revision-0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,40 @@
 [tool.poetry]
 name = "dj-static-revision"
-version = "0.6"
+version = "0.7"
 description = "Revision info for Django static file"
 authors = ["Nguyễn Hồng Quân <ng.hong.quan@gmail.com>"]
 license = "Apache-2.0"
 repository = "https://github.com/AgriConnect/dj-static-revision.git"
 homepage = "https://github.com/AgriConnect/dj-static-revision"
 readme = "README.rst"
 keywords = ["django", "static", "version", "cache"]
 classifiers = [
     "Framework :: Django",
     "Framework :: Django :: 3.2",
     "Framework :: Django :: 4.0",
     "Framework :: Django :: 4.1",
     "Framework :: Django :: 4.2",
+    "Framework :: Django :: 5.0",
     "Environment :: Web Environment",
     "Topic :: Software Development :: Libraries :: Python Modules"
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-dulwich = "^0.21.5"
-single-version = "^1.5.1"
+dulwich = "<0.25"
+single-version = "^1.6.0"
 
 [tool.poetry.group.dev.dependencies]
-pytest = "^7.4.0"
-pytest-env = "^0.8.2"
+pytest = "^8.2.1"
+pytest-env = "^1.1.3"
 
 
 [tool.poetry.group.lint.dependencies]
-ruff = "^0.0.278"
+ruff = "^0.4.5"
 
 [tool.ruff]
 line-length = 120
 
 target-version = "py310"
 
 exclude = [
```

### Comparing `dj_static_revision-0.6/PKG-INFO` & `dj_static_revision-0.7/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 Metadata-Version: 2.1
 Name: dj-static-revision
-Version: 0.6
+Version: 0.7
 Summary: Revision info for Django static file
 Home-page: https://github.com/AgriConnect/dj-static-revision
 License: Apache-2.0
 Keywords: django,static,version,cache
 Author: Nguyễn Hồng Quân
 Author-email: ng.hong.quan@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: Django :: 4.2
+Classifier: Framework :: Django :: 5.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: dulwich (>=0.21.5,<0.22.0)
-Requires-Dist: single-version (>=1.5.1,<2.0.0)
+Requires-Dist: dulwich (<0.25)
+Requires-Dist: single-version (>=1.6.0,<2.0.0)
 Project-URL: Repository, https://github.com/AgriConnect/dj-static-revision.git
 Description-Content-Type: text/x-rst
 
 ======================
 Django Static Revision
 ======================
```

#### html2text {}

```diff
@@ -1,24 +1,25 @@
-Metadata-Version: 2.1 Name: dj-static-revision Version: 0.6 Summary: Revision
+Metadata-Version: 2.1 Name: dj-static-revision Version: 0.7 Summary: Revision
 info for Django static file Home-page: https://github.com/AgriConnect/dj-
 static-revision License: Apache-2.0 Keywords: django,static,version,cache
 Author: Nguyá»n Há»ng QuÃ¢n Author-email: ng.hong.quan@gmail.com Requires-
 Python: >=3.8,<4.0 Classifier: Environment :: Web Environment Classifier:
 Framework :: Django Classifier: Framework :: Django :: 3.2 Classifier:
 Framework :: Django :: 4.0 Classifier: Framework :: Django :: 4.1 Classifier:
-Framework :: Django :: 4.2 Classifier: License :: OSI Approved :: Apache
-Software License Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Classifier: Topic :: Software
-Development :: Libraries :: Python Modules Requires-Dist: dulwich
-(>=0.21.5,<0.22.0) Requires-Dist: single-version (>=1.5.1,<2.0.0) Project-URL:
-Repository, https://github.com/AgriConnect/dj-static-revision.git Description-
-Content-Type: text/x-rst ====================== Django Static Revision
-====================== .. image:: https://madewithlove.now.sh/
+Framework :: Django :: 4.2 Classifier: Framework :: Django :: 5.0 Classifier:
+License :: OSI Approved :: Apache Software License Classifier: Programming
+Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12 Classifier: Topic ::
+Software Development :: Libraries :: Python Modules Requires-Dist: dulwich
+(<0.25) Requires-Dist: single-version (>=1.6.0,<2.0.0) Project-URL: Repository,
+https://github.com/AgriConnect/dj-static-revision.git Description-Content-Type:
+text/x-rst ====================== Django Static Revision ======================
+.. image:: https://madewithlove.now.sh/
 vn?heart=true&colorA=%23ffcd00&colorB=%23da251d .. image:: https://badgen.net/
 pypi/v/dj-static-revision :target: https://pypi.org/project/dj-static-revision
 Django plugin to provide a context variable for retrieving the version of
 running application. This variable is meant to change the URL of a static file,
 to invalidate browser cache. Install ------- .. code-block:: shell pip3 install
 dj-static-revision `Django Static Revision` only supports Python 3.8+. Usage --
 --- Add ``dj_static_revision.context_processors.static_revision`` to your
```

