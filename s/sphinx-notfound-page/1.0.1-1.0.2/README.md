# Comparing `tmp/sphinx_notfound_page-1.0.1.tar.gz` & `tmp/sphinx_notfound_page-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx_notfound_page-1.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "sphinx_notfound_page-1.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `sphinx_notfound_page-1.0.1.tar` & `sphinx_notfound_page-1.0.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-lrwxr-xr-x   0        0        0        0 2021-11-14 10:15:13.244299 sphinx_notfound_page-1.0.1/.eslintrc -> common/eslintrc
-lrwxr-xr-x   0        0        0        0 2021-11-14 10:15:13.254299 sphinx_notfound_page-1.0.1/.flake8 -> common/flake8
--rw-r--r--   0        0        0       81 2019-07-30 11:28:47.437314 sphinx_notfound_page-1.0.1/.gitmodules
-lrwxr-xr-x   0        0        0        0 2021-11-14 10:15:13.244299 sphinx_notfound_page-1.0.1/.isort.cfg -> common/isort.cfg
-lrwxr-xr-x   0        0        0        0 2021-11-14 10:15:13.244299 sphinx_notfound_page-1.0.1/.pep8 -> common/pep8
-lrwxr-xr-x   0        0        0        0 2021-11-14 10:15:13.244299 sphinx_notfound_page-1.0.1/.pre-commit-config.yaml -> common/pre-commit-config.yaml
--rw-r--r--   0        0        0    11233 2024-05-21 13:03:45.826350 sphinx_notfound_page-1.0.1/CHANGELOG.rst
--rw-r--r--   0        0        0     1072 2019-01-19 11:32:01.424634 sphinx_notfound_page-1.0.1/LICENSE
--rw-r--r--   0        0        0     1362 2021-04-25 19:00:36.924124 sphinx_notfound_page-1.0.1/README.rst
--rw-r--r--   0        0        0    34339 2022-08-29 15:03:35.625028 sphinx_notfound_page-1.0.1/docs/404-using-this-extension.png
--rw-r--r--   0        0        0    38048 2022-08-29 15:00:24.433754 sphinx_notfound_page-1.0.1/docs/404-without-this-extension.png
--rw-r--r--   0        0        0      216 2021-04-25 19:00:36.924124 sphinx_notfound_page-1.0.1/docs/404.rst
--rw-r--r--   0        0        0      580 2019-05-25 10:54:48.008540 sphinx_notfound_page-1.0.1/docs/Makefile
--rw-r--r--   0        0        0    68168 2022-07-18 16:56:36.852748 sphinx_notfound_page-1.0.1/docs/_static/who-is-using-it/docs.carpentries.org.png
--rw-r--r--   0        0        0    64437 2022-07-18 17:13:57.944284 sphinx_notfound_page-1.0.1/docs/_static/who-is-using-it/docs.jina.ai.png
--rw-r--r--   0        0        0    24679 2022-07-18 16:53:01.545428 sphinx_notfound_page-1.0.1/docs/_static/who-is-using-it/docs.pyvista.org.png
--rw-r--r--   0        0        0    87647 2022-07-18 16:50:44.183555 sphinx_notfound_page-1.0.1/docs/_static/who-is-using-it/docs.readthedocs.io.png
--rw-r--r--   0        0        0    55341 2022-07-18 16:58:38.521142 sphinx_notfound_page-1.0.1/docs/_static/who-is-using-it/www.attrs.org.png
--rw-r--r--   0        0        0    59498 2022-07-18 17:20:20.270689 sphinx_notfound_page-1.0.1/docs/_static/who-is-using-it/www.nengo.ai.png
--rw-r--r--   0        0        0    74477 2022-07-18 16:55:10.520497 sphinx_notfound_page-1.0.1/docs/_static/who-is-using-it/www.writethedocs.org.png
--rw-r--r--   0        0        0     5483 2023-08-24 13:36:06.694482 sphinx_notfound_page-1.0.1/docs/conf.py
--rw-r--r--   0        0        0     1969 2024-05-21 13:02:19.303142 sphinx_notfound_page-1.0.1/docs/configuration.rst
--rw-r--r--   0        0        0     2135 2022-06-29 10:10:02.805104 sphinx_notfound_page-1.0.1/docs/faq.rst
--rw-r--r--   0        0        0      495 2019-07-30 11:28:47.437314 sphinx_notfound_page-1.0.1/docs/get-involved.rst
--rw-r--r--   0        0        0     2010 2023-08-24 13:36:06.697816 sphinx_notfound_page-1.0.1/docs/how-it-works.rst
--rw-r--r--   0        0        0     2663 2023-08-23 13:37:32.431949 sphinx_notfound_page-1.0.1/docs/index.rst
--rw-r--r--   0        0        0     1450 2023-08-24 13:36:06.697816 sphinx_notfound_page-1.0.1/docs/installation.rst
--rw-r--r--   0        0        0    13265 2019-06-11 09:36:10.430735 sphinx_notfound_page-1.0.1/docs/loudly-crying-face.png
--rw-r--r--   0        0        0     1964 2023-08-24 13:36:06.697816 sphinx_notfound_page-1.0.1/docs/requirements.txt
--rw-r--r--   0        0        0     2715 2022-07-18 17:25:35.491222 sphinx_notfound_page-1.0.1/docs/who-is-using-it.rst
--rw-r--r--   0        0        0       22 2024-05-21 13:04:10.812963 sphinx_notfound_page-1.0.1/notfound/__init__.py
--rw-r--r--   0        0        0    12147 2024-05-21 13:02:19.303142 sphinx_notfound_page-1.0.1/notfound/extension.py
--rw-r--r--   0        0        0     3028 2023-08-24 13:36:06.697816 sphinx_notfound_page-1.0.1/notfound/utils.py
-lrwxr-xr-x   0        0        0        0 2021-11-14 10:15:13.244299 sphinx_notfound_page-1.0.1/prospector.yml -> common/prospector.yml
--rw-r--r--   0        0        0     2011 2024-05-21 13:04:10.802963 sphinx_notfound_page-1.0.1/pyproject.toml
-lrwxr-xr-x   0        0        0        0 2023-08-24 09:58:45.126657 sphinx_notfound_page-1.0.1/tasks.py -> common/tasks.py
--rw-r--r--   0        0        0     2858 1970-01-01 00:00:00.000000 sphinx_notfound_page-1.0.1/PKG-INFO
+lrwxr-xr-x   0        0        0        0 2021-11-14 10:15:13.244299 sphinx_notfound_page-1.0.2/.eslintrc -> common/eslintrc
+lrwxr-xr-x   0        0        0        0 2021-11-14 10:15:13.254299 sphinx_notfound_page-1.0.2/.flake8 -> common/flake8
+-rw-r--r--   0        0        0       81 2019-07-30 11:28:47.437314 sphinx_notfound_page-1.0.2/.gitmodules
+lrwxr-xr-x   0        0        0        0 2021-11-14 10:15:13.244299 sphinx_notfound_page-1.0.2/.isort.cfg -> common/isort.cfg
+lrwxr-xr-x   0        0        0        0 2021-11-14 10:15:13.244299 sphinx_notfound_page-1.0.2/.pep8 -> common/pep8
+lrwxr-xr-x   0        0        0        0 2021-11-14 10:15:13.244299 sphinx_notfound_page-1.0.2/.pre-commit-config.yaml -> common/pre-commit-config.yaml
+-rw-r--r--   0        0        0    11462 2024-05-23 14:54:26.690885 sphinx_notfound_page-1.0.2/CHANGELOG.rst
+-rw-r--r--   0        0        0     1072 2019-01-19 11:32:01.424634 sphinx_notfound_page-1.0.2/LICENSE
+-rw-r--r--   0        0        0     1362 2021-04-25 19:00:36.924124 sphinx_notfound_page-1.0.2/README.rst
+-rw-r--r--   0        0        0    34339 2022-08-29 15:03:35.625028 sphinx_notfound_page-1.0.2/docs/404-using-this-extension.png
+-rw-r--r--   0        0        0    38048 2022-08-29 15:00:24.433754 sphinx_notfound_page-1.0.2/docs/404-without-this-extension.png
+-rw-r--r--   0        0        0      216 2021-04-25 19:00:36.924124 sphinx_notfound_page-1.0.2/docs/404.rst
+-rw-r--r--   0        0        0      580 2019-05-25 10:54:48.008540 sphinx_notfound_page-1.0.2/docs/Makefile
+-rw-r--r--   0        0        0    68168 2022-07-18 16:56:36.852748 sphinx_notfound_page-1.0.2/docs/_static/who-is-using-it/docs.carpentries.org.png
+-rw-r--r--   0        0        0    64437 2022-07-18 17:13:57.944284 sphinx_notfound_page-1.0.2/docs/_static/who-is-using-it/docs.jina.ai.png
+-rw-r--r--   0        0        0    24679 2022-07-18 16:53:01.545428 sphinx_notfound_page-1.0.2/docs/_static/who-is-using-it/docs.pyvista.org.png
+-rw-r--r--   0        0        0    87647 2022-07-18 16:50:44.183555 sphinx_notfound_page-1.0.2/docs/_static/who-is-using-it/docs.readthedocs.io.png
+-rw-r--r--   0        0        0    55341 2022-07-18 16:58:38.521142 sphinx_notfound_page-1.0.2/docs/_static/who-is-using-it/www.attrs.org.png
+-rw-r--r--   0        0        0    59498 2022-07-18 17:20:20.270689 sphinx_notfound_page-1.0.2/docs/_static/who-is-using-it/www.nengo.ai.png
+-rw-r--r--   0        0        0    74477 2022-07-18 16:55:10.520497 sphinx_notfound_page-1.0.2/docs/_static/who-is-using-it/www.writethedocs.org.png
+-rw-r--r--   0        0        0     5459 2024-05-23 08:32:23.643101 sphinx_notfound_page-1.0.2/docs/conf.py
+-rw-r--r--   0        0        0     1969 2024-05-21 13:02:19.303142 sphinx_notfound_page-1.0.2/docs/configuration.rst
+-rw-r--r--   0        0        0     2135 2022-06-29 10:10:02.805104 sphinx_notfound_page-1.0.2/docs/faq.rst
+-rw-r--r--   0        0        0      495 2019-07-30 11:28:47.437314 sphinx_notfound_page-1.0.2/docs/get-involved.rst
+-rw-r--r--   0        0        0     2010 2023-08-24 13:36:06.697816 sphinx_notfound_page-1.0.2/docs/how-it-works.rst
+-rw-r--r--   0        0        0     2663 2023-08-23 13:37:32.431949 sphinx_notfound_page-1.0.2/docs/index.rst
+-rw-r--r--   0        0        0     1450 2023-08-24 13:36:06.697816 sphinx_notfound_page-1.0.2/docs/installation.rst
+-rw-r--r--   0        0        0    13265 2019-06-11 09:36:10.430735 sphinx_notfound_page-1.0.2/docs/loudly-crying-face.png
+-rw-r--r--   0        0        0     1964 2023-08-24 13:36:06.697816 sphinx_notfound_page-1.0.2/docs/requirements.txt
+-rw-r--r--   0        0        0     2715 2022-07-18 17:25:35.491222 sphinx_notfound_page-1.0.2/docs/who-is-using-it.rst
+-rw-r--r--   0        0        0       22 2024-05-23 14:55:03.767493 sphinx_notfound_page-1.0.2/notfound/__init__.py
+-rw-r--r--   0        0        0    12180 2024-05-23 14:52:12.541775 sphinx_notfound_page-1.0.2/notfound/extension.py
+-rw-r--r--   0        0        0     3028 2023-08-24 13:36:06.697816 sphinx_notfound_page-1.0.2/notfound/utils.py
+lrwxr-xr-x   0        0        0        0 2021-11-14 10:15:13.244299 sphinx_notfound_page-1.0.2/prospector.yml -> common/prospector.yml
+-rw-r--r--   0        0        0     2011 2024-05-23 14:55:03.767493 sphinx_notfound_page-1.0.2/pyproject.toml
+lrwxr-xr-x   0        0        0        0 2023-08-24 09:58:45.126657 sphinx_notfound_page-1.0.2/tasks.py -> common/tasks.py
+-rw-r--r--   0        0        0     2858 1970-01-01 00:00:00.000000 sphinx_notfound_page-1.0.2/PKG-INFO
```

### Comparing `sphinx_notfound_page-1.0.1/CHANGELOG.rst` & `sphinx_notfound_page-1.0.2/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,21 @@
 Changelog
 =========
 
 
+Version 1.0.2
+-------------
+
+:Date: May 23, 2024
+
+* Add tests for Python 3.12
+* Remove warning about unclosed files
+* Allow ``str`` and ``None`` types on ``notfound_urls_prefix``
+* Run ``pyupgrade`` and ``ruff`` on the codebase
+
 Version 1.0.1
 -------------
 
 :Date: May 21, 2024
 
 * Do not create 404 page for embedded
 * Small documentation improvements
```

### Comparing `sphinx_notfound_page-1.0.1/LICENSE` & `sphinx_notfound_page-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx_notfound_page-1.0.1/README.rst` & `sphinx_notfound_page-1.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `sphinx_notfound_page-1.0.1/docs/404-using-this-extension.png` & `sphinx_notfound_page-1.0.2/docs/404-using-this-extension.png`

 * *Files identical despite different names*

### Comparing `sphinx_notfound_page-1.0.1/docs/404-without-this-extension.png` & `sphinx_notfound_page-1.0.2/docs/404-without-this-extension.png`

 * *Files identical despite different names*

### Comparing `sphinx_notfound_page-1.0.1/docs/Makefile` & `sphinx_notfound_page-1.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `sphinx_notfound_page-1.0.1/docs/_static/who-is-using-it/docs.carpentries.org.png` & `sphinx_notfound_page-1.0.2/docs/_static/who-is-using-it/docs.carpentries.org.png`

 * *Files identical despite different names*

### Comparing `sphinx_notfound_page-1.0.1/docs/_static/who-is-using-it/docs.jina.ai.png` & `sphinx_notfound_page-1.0.2/docs/_static/who-is-using-it/docs.jina.ai.png`

 * *Files identical despite different names*

### Comparing `sphinx_notfound_page-1.0.1/docs/_static/who-is-using-it/docs.pyvista.org.png` & `sphinx_notfound_page-1.0.2/docs/_static/who-is-using-it/docs.pyvista.org.png`

 * *Files identical despite different names*

### Comparing `sphinx_notfound_page-1.0.1/docs/_static/who-is-using-it/docs.readthedocs.io.png` & `sphinx_notfound_page-1.0.2/docs/_static/who-is-using-it/docs.readthedocs.io.png`

 * *Files identical despite different names*

### Comparing `sphinx_notfound_page-1.0.1/docs/_static/who-is-using-it/www.attrs.org.png` & `sphinx_notfound_page-1.0.2/docs/_static/who-is-using-it/www.attrs.org.png`

 * *Files identical despite different names*

### Comparing `sphinx_notfound_page-1.0.1/docs/_static/who-is-using-it/www.nengo.ai.png` & `sphinx_notfound_page-1.0.2/docs/_static/who-is-using-it/www.nengo.ai.png`

 * *Files identical despite different names*

### Comparing `sphinx_notfound_page-1.0.1/docs/_static/who-is-using-it/www.writethedocs.org.png` & `sphinx_notfound_page-1.0.2/docs/_static/who-is-using-it/www.writethedocs.org.png`

 * *Files identical despite different names*

### Comparing `sphinx_notfound_page-1.0.1/docs/conf.py` & `sphinx_notfound_page-1.0.2/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 #
 # Configuration file for the Sphinx documentation builder.
 #
 # This file does only contain a selection of the most common options. For a
 # full list see the documentation:
 # http://www.sphinx-doc.org/en/master/config
```

### Comparing `sphinx_notfound_page-1.0.1/docs/configuration.rst` & `sphinx_notfound_page-1.0.2/docs/configuration.rst`

 * *Files identical despite different names*

### Comparing `sphinx_notfound_page-1.0.1/docs/faq.rst` & `sphinx_notfound_page-1.0.2/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `sphinx_notfound_page-1.0.1/docs/how-it-works.rst` & `sphinx_notfound_page-1.0.2/docs/how-it-works.rst`

 * *Files identical despite different names*

### Comparing `sphinx_notfound_page-1.0.1/docs/index.rst` & `sphinx_notfound_page-1.0.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `sphinx_notfound_page-1.0.1/docs/installation.rst` & `sphinx_notfound_page-1.0.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `sphinx_notfound_page-1.0.1/docs/loudly-crying-face.png` & `sphinx_notfound_page-1.0.2/docs/loudly-crying-face.png`

 * *Files identical despite different names*

### Comparing `sphinx_notfound_page-1.0.1/docs/requirements.txt` & `sphinx_notfound_page-1.0.2/docs/requirements.txt`

 * *Files identical despite different names*

### Comparing `sphinx_notfound_page-1.0.1/docs/who-is-using-it.rst` & `sphinx_notfound_page-1.0.2/docs/who-is-using-it.rst`

 * *Files identical despite different names*

### Comparing `sphinx_notfound_page-1.0.1/notfound/extension.py` & `sphinx_notfound_page-1.0.2/notfound/extension.py`

 * *Files 0% similar despite different names*

```diff
@@ -295,14 +295,15 @@
     app.add_config_value(
         'notfound_urls_prefix',
         '/{default_language}/{default_version}/'.format(
             default_language=default_language,
             default_version=default_version,
         ),
         'html',
+        types=[str, type(None)],
     )
 
     app.connect('config-inited', validate_configs)
 
     app.connect('html-collect-pages', html_collect_pages)
 
     # Use ``priority=400`` argument here because we want to execute our function
```

### Comparing `sphinx_notfound_page-1.0.1/notfound/utils.py` & `sphinx_notfound_page-1.0.2/notfound/utils.py`

 * *Files identical despite different names*

### Comparing `sphinx_notfound_page-1.0.1/pyproject.toml` & `sphinx_notfound_page-1.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     "page",
     "sphinx",
     "documentation",
 ]
 dependencies = [
     "sphinx>=5",
 ]
-version = "1.0.1"
+version = "1.0.2"
 readme = "README.rst"
 requires-python = ">=3.8"
 license = {file = "LICENSE"}
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Framework :: Sphinx",
     "Framework :: Sphinx :: Extension",
@@ -69,15 +69,15 @@
   ".readthedocs.yml",
   "pytest.ini",
   "conftest.py",
   "tox.ini",
 ]
 
 [tool.bumpver]
-current_version = "1.0.1"
+current_version = "1.0.2"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "Release {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `sphinx_notfound_page-1.0.1/PKG-INFO` & `sphinx_notfound_page-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-notfound-page
-Version: 1.0.1
+Version: 1.0.2
 Summary: Sphinx extension to build a 404 page with absolute URLs
 Keywords: notfound,404,page,sphinx,documentation
 Author-email: Manuel Kaufmann <humitos@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Sphinx
```

