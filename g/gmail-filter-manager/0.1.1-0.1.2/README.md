# Comparing `tmp/gmail_filter_manager-0.1.1.tar.gz` & `tmp/gmail_filter_manager-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gmail_filter_manager-0.1.1.tar", max compression
+gzip compressed data, was "gmail_filter_manager-0.1.2.tar", max compression
```

## Comparing `gmail_filter_manager-0.1.1.tar` & `gmail_filter_manager-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0     1063 2023-07-03 15:22:21.185577 gmail_filter_manager-0.1.1/LICENSE
--rw-r--r--   0        0        0    10498 2023-07-03 15:25:41.899568 gmail_filter_manager-0.1.1/README.md
--rw-r--r--   0        0        0     2618 2023-07-03 15:26:33.882862 gmail_filter_manager-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      107 2023-07-03 15:23:24.839486 gmail_filter_manager-0.1.1/src/gmail_filter_manager/__init__.py
--rwxr-xr-x   0        0        0     1495 2023-07-03 15:25:21.739699 gmail_filter_manager-0.1.1/src/gmail_filter_manager/gfm_extract.py
--rwxr-xr-x   0        0        0     2002 2023-07-03 15:25:35.576272 gmail_filter_manager-0.1.1/src/gmail_filter_manager/gfm_make.py
--rw-r--r--   0        0        0    11352 1970-01-01 00:00:00.000000 gmail_filter_manager-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-07-03 15:22:21.185577 gmail_filter_manager-0.1.2/LICENSE
+-rw-r--r--   0        0        0    10498 2023-07-03 15:25:41.899568 gmail_filter_manager-0.1.2/README.md
+-rw-r--r--   0        0        0     2610 2024-05-23 00:30:12.380597 gmail_filter_manager-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      107 2023-07-03 15:23:24.839486 gmail_filter_manager-0.1.2/src/gmail_filter_manager/__init__.py
+-rwxr-xr-x   0        0        0     1495 2023-07-03 15:25:21.739699 gmail_filter_manager-0.1.2/src/gmail_filter_manager/gfm_extract.py
+-rwxr-xr-x   0        0        0     2002 2023-07-03 15:25:35.576272 gmail_filter_manager-0.1.2/src/gmail_filter_manager/gfm_make.py
+-rw-r--r--   0        0        0        0 2024-05-23 00:27:14.626266 gmail_filter_manager-0.1.2/src/gmail_filter_manager/py.typed
+-rw-r--r--   0        0        0    11404 1970-01-01 00:00:00.000000 gmail_filter_manager-0.1.2/PKG-INFO
```

### Comparing `gmail_filter_manager-0.1.1/LICENSE` & `gmail_filter_manager-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gmail_filter_manager-0.1.1/README.md` & `gmail_filter_manager-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `gmail_filter_manager-0.1.1/pyproject.toml` & `gmail_filter_manager-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gmail-filter-manager"
-version = "0.1.1"
+version = "0.1.2"
 description = "Gmail filer manager using YAML format."
 authors = ["rcmdnk <rcmdnk@gmail.com>"]
 repository = "https://github.com/rcmdnk/gmail_filter_manager"
 homepage = "https://github.com/rcmdnk/gmail_filter_manager"
 readme = "README.md"
 license = "MIT"
 keywords = ["gmail", "yaml", "cli"]
@@ -12,19 +12,19 @@
     "Development Status :: 3 - Alpha",
     "Environment :: Console",
     "Operating System :: OS Independent",
     "Topic :: Utilities",
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.8.1,<3.12"
+python = "^3.8.1"
 ruamel-yaml = "^0.17.32"
 
 [tool.poetry.group.dev.dependencies]
-pyproject-pre-commit = "0.0.15"
+pyproject-pre-commit = "0.1.9"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 gfm_extract = "gmail_filter_manager:gfm_extract"
```

### Comparing `gmail_filter_manager-0.1.1/src/gmail_filter_manager/gfm_extract.py` & `gmail_filter_manager-0.1.2/src/gmail_filter_manager/gfm_extract.py`

 * *Files identical despite different names*

### Comparing `gmail_filter_manager-0.1.1/src/gmail_filter_manager/gfm_make.py` & `gmail_filter_manager-0.1.2/src/gmail_filter_manager/gfm_make.py`

 * *Files identical despite different names*

### Comparing `gmail_filter_manager-0.1.1/PKG-INFO` & `gmail_filter_manager-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: gmail-filter-manager
-Version: 0.1.1
+Version: 0.1.2
 Summary: Gmail filer manager using YAML format.
 Home-page: https://github.com/rcmdnk/gmail_filter_manager
 License: MIT
 Keywords: gmail,yaml,cli
 Author: rcmdnk
 Author-email: rcmdnk@gmail.com
-Requires-Python: >=3.8.1,<3.12
+Requires-Python: >=3.8.1,<4.0.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Utilities
 Requires-Dist: ruamel-yaml (>=0.17.32,<0.18.0)
 Project-URL: Repository, https://github.com/rcmdnk/gmail_filter_manager
 Description-Content-Type: text/markdown
 
 # gmail_filter_manager
```

