# Comparing `tmp/conf_finder-0.1.2.tar.gz` & `tmp/conf_finder-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conf_finder-0.1.2.tar", max compression
+gzip compressed data, was "conf_finder-0.1.3.tar", max compression
```

## Comparing `conf_finder-0.1.2.tar` & `conf_finder-0.1.3.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0    11337 2023-09-23 01:28:35.105891 conf_finder-0.1.2/LICENSE
--rw-r--r--   0        0        0     3307 2023-09-25 00:58:15.522693 conf_finder-0.1.2/README.md
--rw-r--r--   0        0        0     2039 2023-10-04 05:37:13.968841 conf_finder-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      114 2023-09-25 00:58:15.524309 conf_finder-0.1.2/src/conf_finder/__init__.py
--rw-r--r--   0        0        0       81 2023-09-23 01:29:28.332967 conf_finder-0.1.2/src/conf_finder/__version__.py
--rw-r--r--   0        0        0     7236 2023-09-25 00:58:15.524959 conf_finder-0.1.2/src/conf_finder/conf_finder.py
--rw-r--r--   0        0        0     3993 1970-01-01 00:00:00.000000 conf_finder-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    11337 2023-09-23 01:28:35.105891 conf_finder-0.1.3/LICENSE
+-rw-r--r--   0        0        0     3307 2023-09-25 00:58:15.522693 conf_finder-0.1.3/README.md
+-rw-r--r--   0        0        0     2039 2024-05-23 00:26:19.986327 conf_finder-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      114 2023-09-25 00:58:15.524309 conf_finder-0.1.3/src/conf_finder/__init__.py
+-rw-r--r--   0        0        0       81 2023-09-23 01:29:28.332967 conf_finder-0.1.3/src/conf_finder/__version__.py
+-rw-r--r--   0        0        0     7236 2023-09-25 00:58:15.524959 conf_finder-0.1.3/src/conf_finder/conf_finder.py
+-rw-r--r--   0        0        0        0 2024-05-23 00:25:30.362395 conf_finder-0.1.3/src/conf_finder/py.typed
+-rw-r--r--   0        0        0     3995 1970-01-01 00:00:00.000000 conf_finder-0.1.3/PKG-INFO
```

### Comparing `conf_finder-0.1.2/LICENSE` & `conf_finder-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `conf_finder-0.1.2/README.md` & `conf_finder-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `conf_finder-0.1.2/pyproject.toml` & `conf_finder-0.1.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 [tool.poetry]
 name = "conf-finder"
-version = "0.1.2"
+version = "0.1.3"
 description = "Configuration file finder."
 authors = ["rcmdnk <rcmdnk@gmail.com>"]
 repository = "https://github.com/rcmdnk/conf-finder"
 homepage = "https://github.com/rcmdnk/conf-finder"
 readme = "README.md"
 license = "apache-2.0"
 keywords = ["XGB", "XGB_CONFIG_HOME", "Git", "CONFIG"]
 classifiers = []
 
 [tool.poetry.dependencies]
-python = "^3.9"
-gitpython = "^3.1.37"
+python = "^3.10"
+gitpython = "^3.1.41"
 
 [tool.poetry.group.dev.dependencies]
 tomli = { version = "^2.0.1", python = "<3.11"}
 pytest = "^7.4.2"
 pytest-cov = "^4.1.0"
 pytest-xdist = "^3.3.1"
 pytest-benchmark = "^4.0.0"
-pyproject-pre-commit = "^0.0.28"
+pyproject-pre-commit = "^0.1.8"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 addopts = "-n auto"
```

### Comparing `conf_finder-0.1.2/src/conf_finder/conf_finder.py` & `conf_finder-0.1.3/src/conf_finder/conf_finder.py`

 * *Files identical despite different names*

### Comparing `conf_finder-0.1.2/PKG-INFO` & `conf_finder-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: conf-finder
-Version: 0.1.2
+Version: 0.1.3
 Summary: Configuration file finder.
 Home-page: https://github.com/rcmdnk/conf-finder
 License: Apache-2.0
 Keywords: XGB,XGB_CONFIG_HOME,Git,CONFIG
 Author: rcmdnk
 Author-email: rcmdnk@gmail.com
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: gitpython (>=3.1.37,<4.0.0)
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: gitpython (>=3.1.41,<4.0.0)
 Project-URL: Repository, https://github.com/rcmdnk/conf-finder
 Description-Content-Type: text/markdown
 
 # conf-finder
 
 [![test](https://github.com/rcmdnk/conf-finder/actions/workflows/test.yml/badge.svg)](https://github.com/rcmdnk/conf-finder/actions/workflows/test.yml)
 [![test coverage](https://img.shields.io/badge/coverage-check%20here-blue.svg)](https://github.com/rcmdnk/conf-finder/tree/coverage)
```

