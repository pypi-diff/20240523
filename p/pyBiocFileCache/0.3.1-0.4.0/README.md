# Comparing `tmp/pybiocfilecache-0.3.1.tar.gz` & `tmp/pybiocfilecache-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybiocfilecache-0.3.1.tar", last modified: Thu May 16 19:28:05 2024, max compression
+gzip compressed data, was "pybiocfilecache-0.4.0.tar", last modified: Thu May 23 00:59:45 2024, max compression
```

## Comparing `pybiocfilecache-0.3.1.tar` & `pybiocfilecache-0.4.0.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:28:05.611285 pybiocfilecache-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-16 19:27:19.000000 pybiocfilecache-0.3.1/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:28:05.603284 pybiocfilecache-0.3.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:28:05.607284 pybiocfilecache-0.3.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-05-16 19:27:19.000000 pybiocfilecache-0.3.1/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-05-16 19:27:19.000000 pybiocfilecache-0.3.1/.github/workflows/pypi-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-16 19:27:19.000000 pybiocfilecache-0.3.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-16 19:27:19.000000 pybiocfilecache-0.3.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-16 19:27:19.000000 pybiocfilecache-0.3.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-16 19:27:19.000000 pybiocfilecache-0.3.1/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-16 19:27:19.000000 pybiocfilecache-0.3.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    13950 2024-05-16 19:27:19.000000 pybiocfilecache-0.3.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-16 19:27:19.000000 pybiocfilecache-0.3.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-05-16 19:28:05.611285 pybiocfilecache-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-05-16 19:27:19.000000 pybiocfilecache-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:28:05.607284 pybiocfilecache-0.3.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-16 19:27:19.000000 pybiocfilecache-0.3.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:28:05.607284 pybiocfilecache-0.3.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-16 19:27:19.000000 pybiocfilecache-0.3.1/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-16 19:27:19.000000 pybiocfilecache-0.3.1/docs/authors.md
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-16 19:27:19.000000 pybiocfilecache-0.3.1/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)    10327 2024-05-16 19:27:19.000000 pybiocfilecache-0.3.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-16 19:27:19.000000 pybiocfilecache-0.3.1/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-05-16 19:27:19.000000 pybiocfilecache-0.3.1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-16 19:27:19.000000 pybiocfilecache-0.3.1/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-05-16 19:27:19.000000 pybiocfilecache-0.3.1/docs/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-16 19:27:19.000000 pybiocfilecache-0.3.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-16 19:27:19.000000 pybiocfilecache-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-05-16 19:28:05.611285 pybiocfilecache-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-16 19:27:19.000000 pybiocfilecache-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:28:05.603284 pybiocfilecache-0.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:28:05.611285 pybiocfilecache-0.3.1/src/pyBiocFileCache.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-05-16 19:28:05.000000 pybiocfilecache-0.3.1/src/pyBiocFileCache.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-05-16 19:28:05.000000 pybiocfilecache-0.3.1/src/pyBiocFileCache.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 19:28:05.000000 pybiocfilecache-0.3.1/src/pyBiocFileCache.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 19:27:27.000000 pybiocfilecache-0.3.1/src/pyBiocFileCache.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-16 19:28:05.000000 pybiocfilecache-0.3.1/src/pyBiocFileCache.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-16 19:28:05.000000 pybiocfilecache-0.3.1/src/pyBiocFileCache.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:28:05.607284 pybiocfilecache-0.3.1/src/pybiocfilecache/
--rw-r--r--   0 runner    (1001) docker     (127)     8589 2024-05-16 19:27:19.000000 pybiocfilecache-0.3.1/src/pybiocfilecache/BiocFileCache.py
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-16 19:27:19.000000 pybiocfilecache-0.3.1/src/pybiocfilecache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-16 19:27:19.000000 pybiocfilecache-0.3.1/src/pybiocfilecache/_exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:28:05.611285 pybiocfilecache-0.3.1/src/pybiocfilecache/db/
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-05-16 19:27:19.000000 pybiocfilecache-0.3.1/src/pybiocfilecache/db/Base.py
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-16 19:27:19.000000 pybiocfilecache-0.3.1/src/pybiocfilecache/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-16 19:27:19.000000 pybiocfilecache-0.3.1/src/pybiocfilecache/db/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-05-16 19:27:19.000000 pybiocfilecache-0.3.1/src/pybiocfilecache/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:28:05.611285 pybiocfilecache-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-16 19:27:19.000000 pybiocfilecache-0.3.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:28:05.611285 pybiocfilecache-0.3.1/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-16 19:27:19.000000 pybiocfilecache-0.3.1/tests/data/test1.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-16 19:27:19.000000 pybiocfilecache-0.3.1/tests/data/test2.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-16 19:27:19.000000 pybiocfilecache-0.3.1/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-05-16 19:27:19.000000 pybiocfilecache-0.3.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 00:59:45.183634 pybiocfilecache-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-23 00:59:02.000000 pybiocfilecache-0.4.0/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 00:59:45.171634 pybiocfilecache-0.4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 00:59:45.175634 pybiocfilecache-0.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-05-23 00:59:02.000000 pybiocfilecache-0.4.0/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-05-23 00:59:02.000000 pybiocfilecache-0.4.0/.github/workflows/pypi-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-23 00:59:02.000000 pybiocfilecache-0.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-23 00:59:02.000000 pybiocfilecache-0.4.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-23 00:59:02.000000 pybiocfilecache-0.4.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-23 00:59:02.000000 pybiocfilecache-0.4.0/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-23 00:59:02.000000 pybiocfilecache-0.4.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    13950 2024-05-23 00:59:02.000000 pybiocfilecache-0.4.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-23 00:59:02.000000 pybiocfilecache-0.4.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-05-23 00:59:45.183634 pybiocfilecache-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-05-23 00:59:02.000000 pybiocfilecache-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 00:59:45.179634 pybiocfilecache-0.4.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-23 00:59:02.000000 pybiocfilecache-0.4.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 00:59:45.179634 pybiocfilecache-0.4.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-23 00:59:02.000000 pybiocfilecache-0.4.0/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-23 00:59:02.000000 pybiocfilecache-0.4.0/docs/authors.md
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-23 00:59:02.000000 pybiocfilecache-0.4.0/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10312 2024-05-23 00:59:02.000000 pybiocfilecache-0.4.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-23 00:59:02.000000 pybiocfilecache-0.4.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-05-23 00:59:02.000000 pybiocfilecache-0.4.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-23 00:59:02.000000 pybiocfilecache-0.4.0/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-05-23 00:59:02.000000 pybiocfilecache-0.4.0/docs/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-23 00:59:02.000000 pybiocfilecache-0.4.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-23 00:59:02.000000 pybiocfilecache-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-05-23 00:59:45.183634 pybiocfilecache-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-23 00:59:02.000000 pybiocfilecache-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 00:59:45.175634 pybiocfilecache-0.4.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 00:59:45.183634 pybiocfilecache-0.4.0/src/pyBiocFileCache.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-05-23 00:59:45.000000 pybiocfilecache-0.4.0/src/pyBiocFileCache.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-05-23 00:59:45.000000 pybiocfilecache-0.4.0/src/pyBiocFileCache.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 00:59:45.000000 pybiocfilecache-0.4.0/src/pyBiocFileCache.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 00:59:09.000000 pybiocfilecache-0.4.0/src/pyBiocFileCache.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-23 00:59:45.000000 pybiocfilecache-0.4.0/src/pyBiocFileCache.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-23 00:59:45.000000 pybiocfilecache-0.4.0/src/pyBiocFileCache.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 00:59:45.183634 pybiocfilecache-0.4.0/src/pybiocfilecache/
+-rw-r--r--   0 runner    (1001) docker     (127)     8577 2024-05-23 00:59:02.000000 pybiocfilecache-0.4.0/src/pybiocfilecache/BiocFileCache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-05-23 00:59:02.000000 pybiocfilecache-0.4.0/src/pybiocfilecache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-23 00:59:02.000000 pybiocfilecache-0.4.0/src/pybiocfilecache/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-23 00:59:02.000000 pybiocfilecache-0.4.0/src/pybiocfilecache/const.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 00:59:45.183634 pybiocfilecache-0.4.0/src/pybiocfilecache/db/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-23 00:59:02.000000 pybiocfilecache-0.4.0/src/pybiocfilecache/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-05-23 00:59:02.000000 pybiocfilecache-0.4.0/src/pybiocfilecache/db/db_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2054 2024-05-23 00:59:02.000000 pybiocfilecache-0.4.0/src/pybiocfilecache/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 00:59:45.183634 pybiocfilecache-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-23 00:59:02.000000 pybiocfilecache-0.4.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 00:59:45.183634 pybiocfilecache-0.4.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-23 00:59:02.000000 pybiocfilecache-0.4.0/tests/data/test1.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-23 00:59:02.000000 pybiocfilecache-0.4.0/tests/data/test2.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-23 00:59:02.000000 pybiocfilecache-0.4.0/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-05-23 00:59:02.000000 pybiocfilecache-0.4.0/tox.ini
```

### Comparing `pybiocfilecache-0.3.1/.coveragerc` & `pybiocfilecache-0.4.0/.coveragerc`

 * *Files identical despite different names*

### Comparing `pybiocfilecache-0.3.1/.github/workflows/pypi-publish.yml` & `pybiocfilecache-0.4.0/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `pybiocfilecache-0.3.1/.github/workflows/pypi-test.yml` & `pybiocfilecache-0.4.0/.github/workflows/pypi-test.yml`

 * *Files identical despite different names*

### Comparing `pybiocfilecache-0.3.1/.gitignore` & `pybiocfilecache-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pybiocfilecache-0.3.1/.pre-commit-config.yaml` & `pybiocfilecache-0.4.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pybiocfilecache-0.3.1/CONTRIBUTING.rst` & `pybiocfilecache-0.4.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pybiocfilecache-0.3.1/LICENSE.txt` & `pybiocfilecache-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pybiocfilecache-0.3.1/PKG-INFO` & `pybiocfilecache-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyBiocFileCache
-Version: 0.3.1
+Version: 0.4.0
 Summary: File based cache for resources and metadata
 Home-page: https://github.com/epiviz/pyBiocFileCache
 Author: jkanche
 Author-email: jayaram.kancherla@gmail.com
 License: MIT
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
```

### Comparing `pybiocfilecache-0.3.1/README.md` & `pybiocfilecache-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `pybiocfilecache-0.3.1/docs/Makefile` & `pybiocfilecache-0.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pybiocfilecache-0.3.1/docs/conf.py` & `pybiocfilecache-0.4.0/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -175,18 +175,15 @@
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 html_theme = "furo"
 
 # Theme options are theme-specific and customize the look and feel of a theme
 # further.  For a list of options available for each theme, see the
 # documentation.
-html_theme_options = {
-    "sidebar_width": "300px",
-    "page_width": "1200px"
-}
+html_theme_options = {"sidebar_width": "300px", "page_width": "1200px"}
 
 # Add any paths that contain custom themes here, relative to this directory.
 # html_theme_path = []
 
 # The name for this set of Sphinx documents.  If None, it defaults to
 # "<project> v<release> documentation".
 # html_title = None
@@ -262,17 +259,15 @@
     # "pointsize": "10pt",
     # Additional stuff for the LaTeX preamble.
     # "preamble": "",
 }
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title, author, documentclass [howto/manual]).
-latex_documents = [
-    ("index", "user_guide.tex", "pyBiocFileCache Documentation", "jkanche", "manual")
-]
+latex_documents = [("index", "user_guide.tex", "pyBiocFileCache Documentation", "jkanche", "manual")]
 
 # The name of an image file (relative to this directory) to place at the top of
 # the title page.
 # latex_logo = ""
 
 # For "manual" documents, if this is true, then toplevel headings are parts,
 # not chapters.
@@ -300,8 +295,8 @@
     "sklearn": ("https://scikit-learn.org/stable", None),
     "pandas": ("https://pandas.pydata.org/pandas-docs/stable", None),
     "scipy": ("https://docs.scipy.org/doc/scipy/reference", None),
     "setuptools": ("https://setuptools.readthedocs.io/en/stable/", None),
     "pyscaffold": ("https://pyscaffold.org/en/stable", None),
 }
 
-print(f"loading configurations for {project} {version} ...", file=sys.stderr)
+print(f"loading configurations for {project} {version} ...", file=sys.stderr)
```

### Comparing `pybiocfilecache-0.3.1/docs/index.md` & `pybiocfilecache-0.4.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `pybiocfilecache-0.3.1/docs/readme.md` & `pybiocfilecache-0.4.0/docs/readme.md`

 * *Files identical despite different names*

### Comparing `pybiocfilecache-0.3.1/pyproject.toml` & `pybiocfilecache-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pybiocfilecache-0.3.1/setup.cfg` & `pybiocfilecache-0.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `pybiocfilecache-0.3.1/setup.py` & `pybiocfilecache-0.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `pybiocfilecache-0.3.1/src/pyBiocFileCache.egg-info/PKG-INFO` & `pybiocfilecache-0.4.0/src/pyBiocFileCache.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyBiocFileCache
-Version: 0.3.1
+Version: 0.4.0
 Summary: File based cache for resources and metadata
 Home-page: https://github.com/epiviz/pyBiocFileCache
 Author: jkanche
 Author-email: jayaram.kancherla@gmail.com
 License: MIT
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
```

### Comparing `pybiocfilecache-0.3.1/src/pyBiocFileCache.egg-info/SOURCES.txt` & `pybiocfilecache-0.4.0/src/pyBiocFileCache.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 src/pyBiocFileCache.egg-info/dependency_links.txt
 src/pyBiocFileCache.egg-info/not-zip-safe
 src/pyBiocFileCache.egg-info/requires.txt
 src/pyBiocFileCache.egg-info/top_level.txt
 src/pybiocfilecache/BiocFileCache.py
 src/pybiocfilecache/__init__.py
 src/pybiocfilecache/_exceptions.py
+src/pybiocfilecache/const.py
 src/pybiocfilecache/utils.py
-src/pybiocfilecache/db/Base.py
 src/pybiocfilecache/db/__init__.py
-src/pybiocfilecache/db/schema.py
+src/pybiocfilecache/db/db_config.py
 tests/conftest.py
 tests/test_cache.py
 tests/data/test1.txt
 tests/data/test2.txt
```

### Comparing `pybiocfilecache-0.3.1/src/pybiocfilecache/BiocFileCache.py` & `pybiocfilecache-0.4.0/src/pybiocfilecache/BiocFileCache.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,15 @@
 from time import sleep, time
 from typing import List, Literal, Optional, Union
 
 from sqlalchemy import func
 from sqlalchemy.orm import Session
 
 from ._exceptions import NoFpathError, RnameExistsError, RpathTimeoutError
-from .db import create_schema
-from .db.schema import Resource
+from .db.db_config import create_schema, Resource
 from .utils import copy_or_move, create_tmp_dir, generate_id
 
 __author__ = "Jayaram Kancherla"
 __copyright__ = "jkanche"
 __license__ = "MIT"
```

### Comparing `pybiocfilecache-0.3.1/src/pybiocfilecache/__init__.py` & `pybiocfilecache-0.4.0/src/pybiocfilecache/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,13 +13,13 @@
 except PackageNotFoundError:  # pragma: no cover
     __version__ = "unknown"
 finally:
     del version, PackageNotFoundError
 
 from .BiocFileCache import BiocFileCache as BiocFileCache
 
-from .db.schema import Metadata as Metadata
-from .db.schema import Resource as Resource
+from .db.db_config import Metadata as Metadata
+from .db.db_config import Resource as Resource
 
 from ._exceptions import NoFpathError as NoFpathError
 from ._exceptions import RnameExistsError as RnameExistsError
 from ._exceptions import RpathTimeoutError as RpathTimeoutError
```

### Comparing `pybiocfilecache-0.3.1/src/pybiocfilecache/utils.py` & `pybiocfilecache-0.4.0/src/pybiocfilecache/utils.py`

 * *Files identical despite different names*

### Comparing `pybiocfilecache-0.3.1/tests/test_cache.py` & `pybiocfilecache-0.4.0/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `pybiocfilecache-0.3.1/tox.ini` & `pybiocfilecache-0.4.0/tox.ini`

 * *Files identical despite different names*

