# Comparing `tmp/error_manager-1.3.5.tar.gz` & `tmp/error_manager-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "error_manager-1.3.5.tar", last modified: Wed May  8 15:00:14 2024, max compression
+gzip compressed data, was "error_manager-1.4.3.tar", last modified: Thu May 23 10:17:25 2024, max compression
```

## Comparing `error_manager-1.3.5.tar` & `error_manager-1.4.3.tar`

### file list

```diff
@@ -1,45 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:00:14.672415 error_manager-1.3.5/
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-08 15:00:10.000000 error_manager-1.3.5/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-08 15:00:10.000000 error_manager-1.3.5/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 15:00:10.000000 error_manager-1.3.5/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-05-08 15:00:10.000000 error_manager-1.3.5/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-05-08 15:00:10.000000 error_manager-1.3.5/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)    43710 2024-05-08 15:00:10.000000 error_manager-1.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-08 15:00:10.000000 error_manager-1.3.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5657 2024-05-08 15:00:14.672415 error_manager-1.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-05-08 15:00:10.000000 error_manager-1.3.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:00:14.668414 error_manager-1.3.5/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-08 15:00:10.000000 error_manager-1.3.5/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-08 15:00:10.000000 error_manager-1.3.5/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-08 15:00:10.000000 error_manager-1.3.5/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-05-08 15:00:10.000000 error_manager-1.3.5/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-08 15:00:10.000000 error_manager-1.3.5/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-05-08 15:00:10.000000 error_manager-1.3.5/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-08 15:00:10.000000 error_manager-1.3.5/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:00:14.668414 error_manager-1.3.5/docs/reference/
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-08 15:00:10.000000 error_manager-1.3.5/docs/reference/base.rst
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-08 15:00:10.000000 error_manager-1.3.5/docs/reference/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-08 15:00:10.000000 error_manager-1.3.5/docs/reference/listerrors.rst
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-08 15:00:10.000000 error_manager-1.3.5/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4262 2024-05-08 15:00:10.000000 error_manager-1.3.5/docs/return_value.rst
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-08 15:00:10.000000 error_manager-1.3.5/docs/spelling_wordlist.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3662 2024-05-08 15:00:10.000000 error_manager-1.3.5/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-08 15:00:10.000000 error_manager-1.3.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-05-08 15:00:14.672415 error_manager-1.3.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:00:14.664415 error_manager-1.3.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:00:14.672415 error_manager-1.3.5/src/error_manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5657 2024-05-08 15:00:14.000000 error_manager-1.3.5/src/error_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-08 15:00:14.000000 error_manager-1.3.5/src/error_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 15:00:14.000000 error_manager-1.3.5/src/error_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-08 15:00:14.000000 error_manager-1.3.5/src/error_manager.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:00:14.672415 error_manager-1.3.5/src/errors/
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-08 15:00:10.000000 error_manager-1.3.5/src/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-05-08 15:00:10.000000 error_manager-1.3.5/src/errors/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-05-08 15:00:10.000000 error_manager-1.3.5/src/errors/data_classes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-05-08 15:00:10.000000 error_manager-1.3.5/src/errors/error.py
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-08 15:00:10.000000 error_manager-1.3.5/src/errors/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:00:14.672415 error_manager-1.3.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 15:00:10.000000 error_manager-1.3.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-05-08 15:00:10.000000 error_manager-1.3.5/tests/test_enumerator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2556 2024-05-08 15:00:10.000000 error_manager-1.3.5/tests/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3603 2024-05-08 15:00:10.000000 error_manager-1.3.5/tests/test_return_value.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:17:25.264256 error_manager-1.4.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-23 10:17:19.000000 error_manager-1.4.3/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-23 10:17:19.000000 error_manager-1.4.3/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 10:17:19.000000 error_manager-1.4.3/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-05-23 10:17:19.000000 error_manager-1.4.3/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-05-23 10:17:19.000000 error_manager-1.4.3/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    43710 2024-05-23 10:17:19.000000 error_manager-1.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-23 10:17:19.000000 error_manager-1.4.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5325 2024-05-23 10:17:25.264256 error_manager-1.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-05-23 10:17:19.000000 error_manager-1.4.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:17:25.260256 error_manager-1.4.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-23 10:17:19.000000 error_manager-1.4.3/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-23 10:17:19.000000 error_manager-1.4.3/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-23 10:17:19.000000 error_manager-1.4.3/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-05-23 10:17:19.000000 error_manager-1.4.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-23 10:17:19.000000 error_manager-1.4.3/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-05-23 10:17:19.000000 error_manager-1.4.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-23 10:17:19.000000 error_manager-1.4.3/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-23 10:17:19.000000 error_manager-1.4.3/docs/mixin_errorlist.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:17:25.260256 error_manager-1.4.3/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-23 10:17:19.000000 error_manager-1.4.3/docs/reference/base.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-23 10:17:19.000000 error_manager-1.4.3/docs/reference/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-23 10:17:19.000000 error_manager-1.4.3/docs/reference/listerrors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-23 10:17:19.000000 error_manager-1.4.3/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4262 2024-05-23 10:17:19.000000 error_manager-1.4.3/docs/return_value.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-23 10:17:19.000000 error_manager-1.4.3/docs/spelling_wordlist.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3662 2024-05-23 10:17:19.000000 error_manager-1.4.3/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-23 10:17:19.000000 error_manager-1.4.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-05-23 10:17:25.264256 error_manager-1.4.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:17:25.256256 error_manager-1.4.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:17:25.264256 error_manager-1.4.3/src/error_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5325 2024-05-23 10:17:25.000000 error_manager-1.4.3/src/error_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-05-23 10:17:25.000000 error_manager-1.4.3/src/error_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 10:17:25.000000 error_manager-1.4.3/src/error_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-23 10:17:25.000000 error_manager-1.4.3/src/error_manager.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:17:25.264256 error_manager-1.4.3/src/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-23 10:17:19.000000 error_manager-1.4.3/src/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-05-23 10:17:19.000000 error_manager-1.4.3/src/errors/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-05-23 10:17:19.000000 error_manager-1.4.3/src/errors/data_classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-05-23 10:17:19.000000 error_manager-1.4.3/src/errors/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-05-23 10:17:19.000000 error_manager-1.4.3/src/errors/mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-23 10:17:19.000000 error_manager-1.4.3/src/errors/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:17:25.264256 error_manager-1.4.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 10:17:19.000000 error_manager-1.4.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-05-23 10:17:19.000000 error_manager-1.4.3/tests/test_enumerator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2556 2024-05-23 10:17:19.000000 error_manager-1.4.3/tests/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3603 2024-05-23 10:17:19.000000 error_manager-1.4.3/tests/test_return_value.py
```

### Comparing `error_manager-1.3.5/CHANGELOG.rst` & `error_manager-1.4.3/CHANGELOG.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 
 Changelog
 =========
 
+1.4.0 (2024-05-23)
+------------------
+* Added ``ErrorListByMixin`` class to support autocompletion and type checking of your custom project errors
+
 1.3.2 (2023-10-23)
 ------------------
 * Added support for python 3.12
 
 1.3.1 (2023-10-20)
 ------------------
 * Refactored setup.cfg and pyproject.toml
```

### Comparing `error_manager-1.3.5/CONTRIBUTING.rst` & `error_manager-1.4.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `error_manager-1.3.5/LICENSE` & `error_manager-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `error_manager-1.3.5/README.rst` & `error_manager-1.4.3/docs/index.rst`

 * *Files 19% similar despite different names*

```diff
@@ -1,96 +1,81 @@
 =============
 Error Manager
 =============
 
-A lightweight implementation of a manager for error messages throughout your
-project. Allows you to easily define and register error codes and messages.
-Enable easy access to a single list of registerd error codes and messages
-throughout your project.
+
+Managing error codes throughout you project
+===========================================
+
+**Error-manager** is a simple library for Python to manage all your projects error codes.
 
 .. start-badges
 
 .. list-table::
     :widths: 8 50
     :stub-columns: 1
 
     * - docs
       - |docs|
     * - tests
-      - |travis| |requires| |codecov|
+      - |codecov|
     * - package
-      - |version| |wheel| |supported-versions| |commits-since|
+      - |version| |commits-since|
   
 .. |docs| image:: https://readthedocs.org/projects/errors/badge/?style=flat
     :target: https://errors.readthedocs.io/
     :alt: Documentation Status
 
-.. |travis| image:: https://api.travis-ci.com/MaartendeRuyter/errors.svg?branch=master
-    :alt: Travis-CI Build Status
-    :target: https://travis-ci.com/github/MaartendeRuyter/errors
-
-.. |requires| image:: https://requires.io/github/MaartendeRuyter/errors/requirements.svg?branch=master
-    :alt: Requirements Status
-    :target: https://requires.io/github/MaartendeRuyter/errors/requirements/?branch=master
-
 .. |codecov| image:: https://codecov.io/gh/MaartendeRuyter/errors/branch/master/graphs/badge.svg?branch=master
     :alt: Coverage Status
     :target: https://codecov.io/github/MaartendeRuyter/errors
 
 .. |version| image:: https://img.shields.io/pypi/v/error-manager.svg
     :alt: PyPI Package latest release
     :target: https://pypi.org/project/error-manager
 
-.. |wheel| image:: https://img.shields.io/pypi/wheel/error-manager.svg
-    :alt: PyPI Wheel
-    :target: https://pypi.org/project/error-manager
-
-.. |supported-versions| image:: https://img.shields.io/pypi/pyversions/error-manager.svg
-    :alt: Supported versions
-    :target: https://pypi.org/project/error-manager
-
 .. |commits-since| image:: https://img.shields.io/github/commits-since/MaartendeRuyter/errors/v0.1.0.svg
     :alt: Commits since latest release
     :target: https://github.com/MaartendeRuyter/errors/compare/v0.1.0...master
 
 
-.. end-badges
-
-
-* Free software: GNU Lesser General Public License v3 or later (LGPLv3+)
 
-Installation
-============
-
-::
-
-    pip install error-manager
-
-You can also install the in-development version with::
+.. end-badges
 
-    pip install https://github.com/MaartendeRuyter/errors/archive/master.zip
 
-
-Main usecases
-=============
-Error manager provides you with a ``ListErrors`` class to retrieve your
-custom error codes and descriptions throughout your project::
+error-manager main use cases
+----------------------------
+Main use case for the error-manager package is to implement a ``ListErrors`` class that can be used throughout 
+your project to define and access immutable standard error codes and descriptions ::
 
     # retrieve customer defined ErrorCode object form ``ListErrors`` class
-    >>> from errors import ListErrors
-    >>> error = ListErrors.COULD_NOT_FIND_ERROR_CODE
-    >>> error
-    ErrorCode(code='ER_GETERROR_00001', description='Could not find requested 
-    error code', error_data=<class 'dict'>)
+    >>> from errors.error import ListErrors
+    >>> ListErrors.API_GET_RETURNED_404
+    ErrorCode(
+        code='ER_API404_00001',
+        description='API get request returned 404',
+        error_data={})
     
-    # add custom error data to error message when you want to persist or log
-    # the error
-    >>> from errors import add_error_data   
-    >>> error_with_data = add_error_data(error, {'key': 'Example error data'})
+    # add custom error data to error message when you want to persist or log the error
+    # As the errorcode are immutable the add_error_data returns a new error (immutable) error code. 
+    >>> from errors.base import add_error_data
+    >>> error_without_data = ListErrors.API_GET_RETURNED_404
+    >>> error_with_data = add_error_data(error_without_data, {'url': 'www.bad_url.com'})
     >>> error_with_data 
-    ErrorCode(code='ER_GETERROR_00001', description='Could not find requested error code', error_data={'key': 'Example error data'})
+    ErrorCode(
+        code='ER_API404_00001',
+        description='API get request returned 404',
+        error_data={'url': 'www.bad_url.com'})
+    
+This ErrorCode could be returned by the method performing the request so that
+the logic calling this method is aware of the failing request.
+
+In order to use a single type as return value the error-manager package introduces a `ReturnValue` class
+that can hold the actual response, any possible downstream errors and the status of the return value. See 
+ReturnValue documentation.
+
 
 
 Documentation
 =============
 
 https://errors.readthedocs.io/
```

### Comparing `error_manager-1.3.5/docs/Makefile` & `error_manager-1.4.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `error_manager-1.3.5/docs/conf.py` & `error_manager-1.4.3/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 ]
 source_suffix = '.rst'
 master_doc = 'index'
 
 project = 'error manager'
 copyright = '2024, Maarten de Ruyter'
 author = 'Maarten de Ruyter'
-release = '1.3.5'
+release = '1.4.3'
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
 
 extensions = []
 
 templates_path = ['_templates']
```

### Comparing `error_manager-1.3.5/docs/index.rst` & `error_manager-1.4.3/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -13,26 +13,22 @@
 .. list-table::
     :widths: 8 50
     :stub-columns: 1
 
     * - docs
       - |docs|
     * - tests
-      - |travis| |codecov|
+      - |codecov|
     * - package
       - |version| |commits-since|
   
 .. |docs| image:: https://readthedocs.org/projects/errors/badge/?style=flat
     :target: https://errors.readthedocs.io/
     :alt: Documentation Status
 
-.. |travis| image:: https://api.travis-ci.com/MaartendeRuyter/errors.svg?branch=master
-    :alt: Travis-CI Build Status
-    :target: https://travis-ci.com/github/MaartendeRuyter/errors
-
 .. |codecov| image:: https://codecov.io/gh/MaartendeRuyter/errors/branch/master/graphs/badge.svg?branch=master
     :alt: Coverage Status
     :target: https://codecov.io/github/MaartendeRuyter/errors
 
 .. |version| image:: https://img.shields.io/pypi/v/error-manager.svg
     :alt: PyPI Package latest release
     :target: https://pypi.org/project/error-manager
@@ -72,28 +68,13 @@
     
 This ErrorCode could be returned by the method performing the request so that
 the logic calling this method is aware of the failing request.
 
 In order to use a single type as return value the error-manager package introduces a `ReturnValue` class
 that can hold the actual response, any possible downstream errors and the status of the return value. See 
 ReturnValue documentation.
-    
-see :doc:`usage section <usage>` on how to create and
-register custom error codes for your project
 
-.. toctree::
-   :maxdepth: 2
-   :caption: Contents:
-
-   usage
-   return_value
-   reference/index
-   contributing
-   authors
-   changelog
-
-
-Indices and tables
-==================
-* :ref:`genindex`
-* :ref:`modindex`
-* :ref:`search`
+
+Documentation
+=============
+
+https://errors.readthedocs.io/
```

### Comparing `error_manager-1.3.5/docs/make.bat` & `error_manager-1.4.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `error_manager-1.3.5/docs/return_value.rst` & `error_manager-1.4.3/docs/return_value.rst`

 * *Files identical despite different names*

### Comparing `error_manager-1.3.5/docs/usage.rst` & `error_manager-1.4.3/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `error_manager-1.3.5/setup.cfg` & `error_manager-1.4.3/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = error-manager
-version = 1.3.5
+version = 1.4.3
 description = Manage error codes, descriptions and data in a unified way throughout a project
 long_description = file: README.rst, CHANGELOG.rst
 long_description_content_type = text/x-rst
 url = https://github.com/MaartendeRuyter/errors
 author = Maarten de Ruyter
 author_email = "Maarten de Ruyter" <maarten@geodatagarden.com>
 license = GNU
```

### Comparing `error_manager-1.3.5/src/error_manager.egg-info/SOURCES.txt` & `error_manager-1.4.3/src/error_manager.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 docs/Makefile
 docs/authors.rst
 docs/changelog.rst
 docs/conf.py
 docs/contributing.rst
 docs/index.rst
 docs/make.bat
+docs/mixin_errorlist.rst
 docs/requirements.txt
 docs/return_value.rst
 docs/spelling_wordlist.txt
 docs/usage.rst
 docs/reference/base.rst
 docs/reference/index.rst
 docs/reference/listerrors.rst
@@ -26,12 +27,13 @@
 src/error_manager.egg-info/SOURCES.txt
 src/error_manager.egg-info/dependency_links.txt
 src/error_manager.egg-info/top_level.txt
 src/errors/__init__.py
 src/errors/base.py
 src/errors/data_classes.py
 src/errors/error.py
+src/errors/mixin.py
 src/errors/settings.py
 tests/__init__.py
 tests/test_enumerator.py
 tests/test_errors.py
 tests/test_return_value.py
```

### Comparing `error_manager-1.3.5/src/errors/base.py` & `error_manager-1.4.3/src/errors/base.py`

 * *Files identical despite different names*

### Comparing `error_manager-1.3.5/src/errors/data_classes.py` & `error_manager-1.4.3/src/errors/data_classes.py`

 * *Files identical despite different names*

### Comparing `error_manager-1.3.5/src/errors/error.py` & `error_manager-1.4.3/src/errors/error.py`

 * *Files identical despite different names*

### Comparing `error_manager-1.3.5/tests/test_enumerator.py` & `error_manager-1.4.3/tests/test_enumerator.py`

 * *Files identical despite different names*

### Comparing `error_manager-1.3.5/tests/test_errors.py` & `error_manager-1.4.3/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `error_manager-1.3.5/tests/test_return_value.py` & `error_manager-1.4.3/tests/test_return_value.py`

 * *Files identical despite different names*

