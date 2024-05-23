# Comparing `tmp/cone.tokens-0.4.tar.gz` & `tmp/cone_tokens-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cone.tokens-0.4.tar", last modified: Mon Feb 12 10:17:29 2024, max compression
+gzip compressed data, was "cone_tokens-0.5.tar", last modified: Thu May 23 13:39:38 2024, max compression
```

## Comparing `cone.tokens-0.4.tar` & `cone_tokens-0.5.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-02-12 10:17:29.055801 cone.tokens-0.4/
--rw-r--r--   0 rnix      (1000) rnix      (1000)      401 2024-02-12 10:17:28.000000 cone.tokens-0.4/CHANGES.rst
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1097 2024-02-12 10:17:28.000000 cone.tokens-0.4/LICENSE.rst
--rw-r--r--   0 rnix      (1000) rnix      (1000)       98 2024-02-12 10:17:28.000000 cone.tokens-0.4/MANIFEST.in
--rw-r--r--   0 rnix      (1000) rnix      (1000)     6102 2024-02-12 10:17:29.055801 cone.tokens-0.4/PKG-INFO
--rw-r--r--   0 rnix      (1000) rnix      (1000)     4018 2024-02-12 10:17:28.000000 cone.tokens-0.4/README.rst
--rw-r--r--   0 rnix      (1000) rnix      (1000)       74 2024-02-12 10:17:29.055801 cone.tokens-0.4/setup.cfg
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1386 2024-02-12 10:17:28.000000 cone.tokens-0.4/setup.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-02-12 10:17:29.051801 cone.tokens-0.4/src/
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-02-12 10:17:29.051801 cone.tokens-0.4/src/cone/
--rw-r--r--   0 rnix      (1000) rnix      (1000)       55 2024-02-12 10:17:28.000000 cone.tokens-0.4/src/cone/__init__.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-02-12 10:17:29.051801 cone.tokens-0.4/src/cone/tokens/
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1167 2024-02-12 10:17:28.000000 cone.tokens-0.4/src/cone/tokens/__init__.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     6103 2024-02-12 10:17:28.000000 cone.tokens-0.4/src/cone/tokens/api.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-02-12 10:17:29.055801 cone.tokens-0.4/src/cone/tokens/browser/
--rw-r--r--   0 rnix      (1000) rnix      (1000)      780 2024-02-12 10:17:28.000000 cone.tokens-0.4/src/cone/tokens/browser/__init__.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     6247 2024-02-12 10:17:28.000000 cone.tokens-0.4/src/cone/tokens/browser/api.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     6893 2024-02-12 10:17:28.000000 cone.tokens-0.4/src/cone/tokens/browser/settings.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-02-12 10:17:29.055801 cone.tokens-0.4/src/cone/tokens/browser/static/
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1776 2024-02-12 10:17:28.000000 cone.tokens-0.4/src/cone/tokens/browser/static/cone.tokens.css
--rw-r--r--   0 rnix      (1000) rnix      (1000)    14333 2024-02-12 10:17:28.000000 cone.tokens-0.4/src/cone/tokens/browser/static/cone.tokens.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1413 2024-02-12 10:17:28.000000 cone.tokens-0.4/src/cone/tokens/browser/static/cone.tokens.min.css
--rw-r--r--   0 rnix      (1000) rnix      (1000)     6255 2024-02-12 10:17:28.000000 cone.tokens-0.4/src/cone/tokens/browser/static/cone.tokens.min.js
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-02-12 10:17:29.055801 cone.tokens-0.4/src/cone/tokens/browser/templates/
--rw-r--r--   0 rnix      (1000) rnix      (1000)     4645 2024-02-12 10:17:28.000000 cone.tokens-0.4/src/cone/tokens/browser/templates/token.pt
--rw-r--r--   0 rnix      (1000) rnix      (1000)      530 2024-02-12 10:17:28.000000 cone.tokens-0.4/src/cone/tokens/browser/templates/tokens.pt
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2523 2024-02-12 10:17:28.000000 cone.tokens-0.4/src/cone/tokens/browser/templates/tokens_overview.pt
--rw-r--r--   0 rnix      (1000) rnix      (1000)     8236 2024-02-12 10:17:28.000000 cone.tokens-0.4/src/cone/tokens/browser/token.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     3102 2024-02-12 10:17:28.000000 cone.tokens-0.4/src/cone/tokens/browser/tokens.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1335 2024-02-12 10:17:28.000000 cone.tokens-0.4/src/cone/tokens/exceptions.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-02-12 10:17:29.055801 cone.tokens-0.4/src/cone/tokens/locale/
--rw-r--r--   0 rnix      (1000) rnix      (1000)     5735 2024-02-12 10:17:28.000000 cone.tokens-0.4/src/cone/tokens/locale/cone.tokens.pot
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-02-12 10:17:29.051801 cone.tokens-0.4/src/cone/tokens/locale/de/
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-02-12 10:17:29.055801 cone.tokens-0.4/src/cone/tokens/locale/de/LC_MESSAGES/
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2449 2024-02-12 10:17:28.000000 cone.tokens-0.4/src/cone/tokens/locale/de/LC_MESSAGES/cone.tokens.mo
--rw-r--r--   0 rnix      (1000) rnix      (1000)     6088 2024-02-12 10:17:28.000000 cone.tokens-0.4/src/cone/tokens/locale/de/LC_MESSAGES/cone.tokens.po
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-02-12 10:17:29.051801 cone.tokens-0.4/src/cone/tokens/locale/en/
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-02-12 10:17:29.055801 cone.tokens-0.4/src/cone/tokens/locale/en/LC_MESSAGES/
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2344 2024-02-12 10:17:28.000000 cone.tokens-0.4/src/cone/tokens/locale/en/LC_MESSAGES/cone.tokens.mo
--rw-r--r--   0 rnix      (1000) rnix      (1000)     6010 2024-02-12 10:17:28.000000 cone.tokens-0.4/src/cone/tokens/locale/en/LC_MESSAGES/cone.tokens.po
--rw-r--r--   0 rnix      (1000) rnix      (1000)     3110 2024-02-12 10:17:28.000000 cone.tokens-0.4/src/cone/tokens/model.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1823 2024-02-12 10:17:28.000000 cone.tokens-0.4/src/cone/tokens/settings.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-02-12 10:17:29.055801 cone.tokens-0.4/src/cone/tokens/tests/
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1095 2024-02-12 10:17:28.000000 cone.tokens-0.4/src/cone/tokens/tests/__init__.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)    11826 2024-02-12 10:17:28.000000 cone.tokens-0.4/src/cone/tokens/tests/test_api.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)    18033 2024-02-12 10:17:28.000000 cone.tokens-0.4/src/cone/tokens/tests/test_json_api.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     3142 2024-02-12 10:17:28.000000 cone.tokens-0.4/src/cone/tokens/tests/test_model.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     4571 2024-02-12 10:17:28.000000 cone.tokens-0.4/src/cone/tokens/tests/test_settings.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)    12330 2024-02-12 10:17:28.000000 cone.tokens-0.4/src/cone/tokens/tests/test_token.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-02-12 10:17:29.055801 cone.tokens-0.4/src/cone.tokens.egg-info/
--rw-r--r--   0 rnix      (1000) rnix      (1000)     6102 2024-02-12 10:17:29.000000 cone.tokens-0.4/src/cone.tokens.egg-info/PKG-INFO
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1473 2024-02-12 10:17:29.000000 cone.tokens-0.4/src/cone.tokens.egg-info/SOURCES.txt
--rw-r--r--   0 rnix      (1000) rnix      (1000)        1 2024-02-12 10:17:29.000000 cone.tokens-0.4/src/cone.tokens.egg-info/dependency_links.txt
--rw-r--r--   0 rnix      (1000) rnix      (1000)        5 2024-02-12 10:17:29.000000 cone.tokens-0.4/src/cone.tokens.egg-info/namespace_packages.txt
--rw-r--r--   0 rnix      (1000) rnix      (1000)        1 2024-02-12 10:17:29.000000 cone.tokens-0.4/src/cone.tokens.egg-info/not-zip-safe
--rw-r--r--   0 rnix      (1000) rnix      (1000)       72 2024-02-12 10:17:29.000000 cone.tokens-0.4/src/cone.tokens.egg-info/requires.txt
--rw-r--r--   0 rnix      (1000) rnix      (1000)        5 2024-02-12 10:17:29.000000 cone.tokens-0.4/src/cone.tokens.egg-info/top_level.txt
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-05-23 13:39:38.831210 cone_tokens-0.5/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      641 2024-05-23 13:39:38.000000 cone_tokens-0.5/CHANGES.rst
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1097 2024-05-23 13:39:38.000000 cone_tokens-0.5/LICENSE.rst
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       98 2024-05-23 13:39:38.000000 cone_tokens-0.5/MANIFEST.in
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     6342 2024-05-23 13:39:38.831210 cone_tokens-0.5/PKG-INFO
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     4018 2024-05-23 13:39:38.000000 cone_tokens-0.5/README.rst
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       74 2024-05-23 13:39:38.831210 cone_tokens-0.5/setup.cfg
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1386 2024-05-23 13:39:38.000000 cone_tokens-0.5/setup.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-05-23 13:39:38.827210 cone_tokens-0.5/src/
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-05-23 13:39:38.831210 cone_tokens-0.5/src/cone/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       55 2024-05-23 13:39:38.000000 cone_tokens-0.5/src/cone/__init__.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-05-23 13:39:38.831210 cone_tokens-0.5/src/cone/tokens/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1167 2024-05-23 13:39:38.000000 cone_tokens-0.5/src/cone/tokens/__init__.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     6103 2024-05-23 13:39:38.000000 cone_tokens-0.5/src/cone/tokens/api.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-05-23 13:39:38.831210 cone_tokens-0.5/src/cone/tokens/browser/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      780 2024-05-23 13:39:38.000000 cone_tokens-0.5/src/cone/tokens/browser/__init__.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     6247 2024-05-23 13:39:38.000000 cone_tokens-0.5/src/cone/tokens/browser/api.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     6893 2024-05-23 13:39:38.000000 cone_tokens-0.5/src/cone/tokens/browser/settings.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-05-23 13:39:38.831210 cone_tokens-0.5/src/cone/tokens/browser/static/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1776 2024-05-23 13:39:38.000000 cone_tokens-0.5/src/cone/tokens/browser/static/cone.tokens.css
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    14333 2024-05-23 13:39:38.000000 cone_tokens-0.5/src/cone/tokens/browser/static/cone.tokens.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1413 2024-05-23 13:39:38.000000 cone_tokens-0.5/src/cone/tokens/browser/static/cone.tokens.min.css
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     6255 2024-05-23 13:39:38.000000 cone_tokens-0.5/src/cone/tokens/browser/static/cone.tokens.min.js
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-05-23 13:39:38.831210 cone_tokens-0.5/src/cone/tokens/browser/templates/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     4645 2024-05-23 13:39:38.000000 cone_tokens-0.5/src/cone/tokens/browser/templates/token.pt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      530 2024-05-23 13:39:38.000000 cone_tokens-0.5/src/cone/tokens/browser/templates/tokens.pt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2523 2024-05-23 13:39:38.000000 cone_tokens-0.5/src/cone/tokens/browser/templates/tokens_overview.pt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     8236 2024-05-23 13:39:38.000000 cone_tokens-0.5/src/cone/tokens/browser/token.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     3102 2024-05-23 13:39:38.000000 cone_tokens-0.5/src/cone/tokens/browser/tokens.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1335 2024-05-23 13:39:38.000000 cone_tokens-0.5/src/cone/tokens/exceptions.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-05-23 13:39:38.831210 cone_tokens-0.5/src/cone/tokens/locale/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     5735 2024-05-23 13:39:38.000000 cone_tokens-0.5/src/cone/tokens/locale/cone.tokens.pot
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-05-23 13:39:38.827210 cone_tokens-0.5/src/cone/tokens/locale/de/
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-05-23 13:39:38.831210 cone_tokens-0.5/src/cone/tokens/locale/de/LC_MESSAGES/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2449 2024-05-23 13:39:38.000000 cone_tokens-0.5/src/cone/tokens/locale/de/LC_MESSAGES/cone.tokens.mo
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     6088 2024-05-23 13:39:38.000000 cone_tokens-0.5/src/cone/tokens/locale/de/LC_MESSAGES/cone.tokens.po
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-05-23 13:39:38.831210 cone_tokens-0.5/src/cone/tokens/locale/en/
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-05-23 13:39:38.831210 cone_tokens-0.5/src/cone/tokens/locale/en/LC_MESSAGES/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2344 2024-05-23 13:39:38.000000 cone_tokens-0.5/src/cone/tokens/locale/en/LC_MESSAGES/cone.tokens.mo
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     6010 2024-05-23 13:39:38.000000 cone_tokens-0.5/src/cone/tokens/locale/en/LC_MESSAGES/cone.tokens.po
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     3128 2024-05-23 13:39:38.000000 cone_tokens-0.5/src/cone/tokens/model.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1823 2024-05-23 13:39:38.000000 cone_tokens-0.5/src/cone/tokens/settings.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-05-23 13:39:38.831210 cone_tokens-0.5/src/cone/tokens/tests/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1095 2024-05-23 13:39:38.000000 cone_tokens-0.5/src/cone/tokens/tests/__init__.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    11826 2024-05-23 13:39:38.000000 cone_tokens-0.5/src/cone/tokens/tests/test_api.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    18033 2024-05-23 13:39:38.000000 cone_tokens-0.5/src/cone/tokens/tests/test_json_api.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     3142 2024-05-23 13:39:38.000000 cone_tokens-0.5/src/cone/tokens/tests/test_model.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     4571 2024-05-23 13:39:38.000000 cone_tokens-0.5/src/cone/tokens/tests/test_settings.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    12330 2024-05-23 13:39:38.000000 cone_tokens-0.5/src/cone/tokens/tests/test_token.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-05-23 13:39:38.831210 cone_tokens-0.5/src/cone.tokens.egg-info/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     6342 2024-05-23 13:39:38.000000 cone_tokens-0.5/src/cone.tokens.egg-info/PKG-INFO
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1473 2024-05-23 13:39:38.000000 cone_tokens-0.5/src/cone.tokens.egg-info/SOURCES.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)        1 2024-05-23 13:39:38.000000 cone_tokens-0.5/src/cone.tokens.egg-info/dependency_links.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)        5 2024-05-23 13:39:38.000000 cone_tokens-0.5/src/cone.tokens.egg-info/namespace_packages.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)        1 2024-05-23 13:39:38.000000 cone_tokens-0.5/src/cone.tokens.egg-info/not-zip-safe
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       72 2024-05-23 13:39:38.000000 cone_tokens-0.5/src/cone.tokens.egg-info/requires.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)        5 2024-05-23 13:39:38.000000 cone_tokens-0.5/src/cone.tokens.egg-info/top_level.txt
```

### Comparing `cone.tokens-0.4/LICENSE.rst` & `cone_tokens-0.5/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `cone.tokens-0.4/PKG-INFO` & `cone_tokens-0.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cone.tokens
-Version: 0.4
+Version: 0.5
 Summary: cone token api
 Home-page: http://github.com/conestack/cone.tokens
 Author: Cone Contributors
 Author-email: dev@conestack.org
 License: MIT
 Keywords: node pyramid cone web
 Classifier: Environment :: Web Environment
@@ -166,14 +166,28 @@
 - Torben Baumgartner
 - Lena Daxenbichler
 
 
 Changes
 =======
 
+0.5 (2024-05-23)
+----------------
+
+- Update Makefile.
+  [rnix]
+
+- ``properties`` and ``metadata`` of ``cone.tokens.model.Tokens`` are instance
+  properties now.
+  [rnix]
+
+- Use ``ts.http_request`` instead of ``ts.ajax.request``.
+  [rnix]
+
+
 0.4 (2024-02-12)
 ----------------
 
 - Adopt Settings UI changes from ``cone.app``.
   [rnix]
```

### Comparing `cone.tokens-0.4/README.rst` & `cone_tokens-0.5/README.rst`

 * *Files identical despite different names*

### Comparing `cone.tokens-0.4/setup.py` & `cone_tokens-0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 
 def read_file(name):
     with open(os.path.join(os.path.dirname(__file__), name)) as f:
         return f.read()
 
 
-version = '0.4'
+version = '0.5'
 shortdesc = 'cone token api'
 longdesc = '\n\n'.join([read_file(name) for name in [
     'README.rst',
     'CHANGES.rst',
     'LICENSE.rst'
 ]])
```

### Comparing `cone.tokens-0.4/src/cone/tokens/__init__.py` & `cone_tokens-0.5/src/cone/tokens/__init__.py`

 * *Files identical despite different names*

### Comparing `cone.tokens-0.4/src/cone/tokens/api.py` & `cone_tokens-0.5/src/cone/tokens/api.py`

 * *Files identical despite different names*

### Comparing `cone.tokens-0.4/src/cone/tokens/browser/__init__.py` & `cone_tokens-0.5/src/cone/tokens/browser/__init__.py`

 * *Files identical despite different names*

### Comparing `cone.tokens-0.4/src/cone/tokens/browser/api.py` & `cone_tokens-0.5/src/cone/tokens/browser/api.py`

 * *Files identical despite different names*

### Comparing `cone.tokens-0.4/src/cone/tokens/browser/settings.py` & `cone_tokens-0.5/src/cone/tokens/browser/settings.py`

 * *Files identical despite different names*

### Comparing `cone.tokens-0.4/src/cone/tokens/browser/static/cone.tokens.css` & `cone_tokens-0.5/src/cone/tokens/browser/static/cone.tokens.css`

 * *Files identical despite different names*

### Comparing `cone.tokens-0.4/src/cone/tokens/browser/static/cone.tokens.js` & `cone_tokens-0.5/src/cone/tokens/browser/static/cone.tokens.js`

 * *Files 7% similar despite different names*

#### js-beautify {}

```diff
@@ -22,15 +22,15 @@
                 button.on('click', function(e) {
                     that.set_usage_count(button.data('usage-count'));
                 });
             });
         }
         request_api(params) {
             const settings = this.settings;
-            ts.ajax.request({
+            ts.http_request({
                 url: `${settings.base_url}/update_token`,
                 params: params,
                 type: 'json',
                 method: 'POST',
                 success: (data, status, request) => {
                     if (data.success) {
                         ts.ajax.action({
@@ -166,15 +166,15 @@
                 params: params
             });
         }
         add_tokens(evt) {
             const base_url = this.token_settings.base_url;
 
             function add(amount, count) {
-                ts.ajax.request({
+                ts.http_request({
                     url: `${base_url}/add_token`,
                     params: {},
                     type: 'json',
                     method: 'POST',
                     success: (data, status, request) => {
                         if (data.success) {
                             count += 1;
@@ -213,15 +213,15 @@
                 message: 'Do you really want to delete selected tokens?',
                 on_confirm: () => {
                     let uids = [];
                     for (let token of this.tokens) {
                         let uid = $(token).data('token-uid');
                         uids.push(uid);
                     }
-                    ts.ajax.request({
+                    ts.http_request({
                         url: `${base_url}/delete_tokens`,
                         params: {
                             token_uids: JSON.stringify(uids)
                         },
                         type: 'json',
                         method: 'POST',
                         success: (data, status, request) => {
@@ -309,29 +309,29 @@
                 selector: '#layout',
                 mode: 'replace',
                 url: `${this.base_url}/${token_uid}`,
                 params: {}
             });
         }
         query_token(value) {
-            ts.ajax.request({
+            ts.http_request({
                 url: `${this.base_url}/query_token`,
                 params: {
                     value: value
                 },
                 type: 'json',
                 success: (data, status, request) => {
                     if (data.success) {
                         if (!data.token) {
                             this.active = false;
                             ts.show_dialog({
                                 title: 'Token not exists?',
                                 message: 'Do you want to create it?',
                                 on_confirm: () => {
-                                    ts.ajax.request({
+                                    ts.http_request({
                                         url: `${this.base_url}/add_token`,
                                         params: {
                                             value: value
                                         },
                                         type: 'json',
                                         method: 'POST',
                                         success: (data, status, request) => {
```

### Comparing `cone.tokens-0.4/src/cone/tokens/browser/static/cone.tokens.min.css` & `cone_tokens-0.5/src/cone/tokens/browser/static/cone.tokens.min.css`

 * *Files identical despite different names*

### Comparing `cone.tokens-0.4/src/cone/tokens/browser/static/cone.tokens.min.js` & `cone_tokens-0.5/src/cone/tokens/browser/static/cone.tokens.min.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -19,15 +19,15 @@
                 t.on("click", (function(e) {
                     s.set_usage_count(t.data("usage-count"))
                 }))
             }))
         }
         request_api(t) {
             const e = this.settings;
-            s.ajax.request({
+            s.http_request({
                 url: `${e.base_url}/update_token`,
                 params: t,
                 type: "json",
                 method: "POST",
                 success: (t, n, i) => {
                     t.success ? s.ajax.action({
                         name: "content",
@@ -101,15 +101,15 @@
                 params: e
             })
         }
         add_tokens(t) {
             const e = this.token_settings.base_url;
             let n = this.add_tokens_input.val();
             n && (n = parseInt(n), function t(n, i) {
-                s.ajax.request({
+                s.http_request({
                     url: `${e}/add_token`,
                     params: {},
                     type: "json",
                     method: "POST",
                     success: (o, a, r) => {
                         o.success ? n === (i += 1) ? s.ajax.action({
                             name: "tokens_overview",
@@ -132,15 +132,15 @@
                 message: "Do you really want to delete selected tokens?",
                 on_confirm: () => {
                     let t = [];
                     for (let s of this.tokens) {
                         let n = e(s).data("token-uid");
                         t.push(n)
                     }
-                    s.ajax.request({
+                    s.http_request({
                         url: `${n}/delete_tokens`,
                         params: {
                             token_uids: JSON.stringify(t)
                         },
                         type: "json",
                         method: "POST",
                         success: (t, e, i) => {
@@ -204,26 +204,26 @@
                 selector: "#layout",
                 mode: "replace",
                 url: `${this.base_url}/${t}`,
                 params: {}
             })
         }
         query_token(t) {
-            s.ajax.request({
+            s.http_request({
                 url: `${this.base_url}/query_token`,
                 params: {
                     value: t
                 },
                 type: "json",
                 success: (e, n, i) => {
                     e.success ? e.token ? this.load_token(e.token.uid) : (this.active = !1, s.show_dialog({
                         title: "Token not exists?",
                         message: "Do you want to create it?",
                         on_confirm: () => {
-                            s.ajax.request({
+                            s.http_request({
                                 url: `${this.base_url}/add_token`,
                                 params: {
                                     value: t
                                 },
                                 type: "json",
                                 method: "POST",
                                 success: (t, e, n) => {
```

### Comparing `cone.tokens-0.4/src/cone/tokens/browser/templates/token.pt` & `cone_tokens-0.5/src/cone/tokens/browser/templates/token.pt`

 * *Files identical despite different names*

### Comparing `cone.tokens-0.4/src/cone/tokens/browser/templates/tokens.pt` & `cone_tokens-0.5/src/cone/tokens/browser/templates/tokens.pt`

 * *Files identical despite different names*

### Comparing `cone.tokens-0.4/src/cone/tokens/browser/templates/tokens_overview.pt` & `cone_tokens-0.5/src/cone/tokens/browser/templates/tokens_overview.pt`

 * *Files identical despite different names*

### Comparing `cone.tokens-0.4/src/cone/tokens/browser/token.py` & `cone_tokens-0.5/src/cone/tokens/browser/token.py`

 * *Files identical despite different names*

### Comparing `cone.tokens-0.4/src/cone/tokens/browser/tokens.py` & `cone_tokens-0.5/src/cone/tokens/browser/tokens.py`

 * *Files identical despite different names*

### Comparing `cone.tokens-0.4/src/cone/tokens/exceptions.py` & `cone_tokens-0.5/src/cone/tokens/exceptions.py`

 * *Files identical despite different names*

### Comparing `cone.tokens-0.4/src/cone/tokens/locale/cone.tokens.pot` & `cone_tokens-0.5/src/cone/tokens/locale/cone.tokens.pot`

 * *Files identical despite different names*

### Comparing `cone.tokens-0.4/src/cone/tokens/locale/de/LC_MESSAGES/cone.tokens.mo` & `cone_tokens-0.5/src/cone/tokens/locale/de/LC_MESSAGES/cone.tokens.mo`

 * *Files identical despite different names*

### Comparing `cone.tokens-0.4/src/cone/tokens/locale/de/LC_MESSAGES/cone.tokens.po` & `cone_tokens-0.5/src/cone/tokens/locale/de/LC_MESSAGES/cone.tokens.po`

 * *Files identical despite different names*

### Comparing `cone.tokens-0.4/src/cone/tokens/locale/en/LC_MESSAGES/cone.tokens.mo` & `cone_tokens-0.5/src/cone/tokens/locale/en/LC_MESSAGES/cone.tokens.mo`

 * *Files identical despite different names*

### Comparing `cone.tokens-0.4/src/cone/tokens/locale/en/LC_MESSAGES/cone.tokens.po` & `cone_tokens-0.5/src/cone/tokens/locale/en/LC_MESSAGES/cone.tokens.po`

 * *Files identical despite different names*

### Comparing `cone.tokens-0.4/src/cone/tokens/model.py` & `cone_tokens-0.5/src/cone/tokens/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -76,25 +76,25 @@
 #@plumbing(SQLPrincipalACL)
 @implementer(IUUID)
 class TokenContainer(SQLTableNode):
     record_class = TokenRecord
     child_factory = TokenNode
     uuid = uuid.UUID('c40ef458-832f-42e6-9add-2dda2afb8920')
 
-    @property
+    @instance_property
     def properties(self):
         props = Properties()
         props.in_navtree = True
         props.action_up = True
         #props.action_sharing = True
         props.action_view = True
         props.action_list = True
         return props
 
-    @property
+    @instance_property
     def metadata(self):
         md = Metadata()
         info = self.nodeinfo
         md.title = info.title
         md.description = info.description
         return md
```

### Comparing `cone.tokens-0.4/src/cone/tokens/settings.py` & `cone_tokens-0.5/src/cone/tokens/settings.py`

 * *Files identical despite different names*

### Comparing `cone.tokens-0.4/src/cone/tokens/tests/__init__.py` & `cone_tokens-0.5/src/cone/tokens/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cone.tokens-0.4/src/cone/tokens/tests/test_api.py` & `cone_tokens-0.5/src/cone/tokens/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `cone.tokens-0.4/src/cone/tokens/tests/test_json_api.py` & `cone_tokens-0.5/src/cone/tokens/tests/test_json_api.py`

 * *Files identical despite different names*

### Comparing `cone.tokens-0.4/src/cone/tokens/tests/test_model.py` & `cone_tokens-0.5/src/cone/tokens/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `cone.tokens-0.4/src/cone/tokens/tests/test_settings.py` & `cone_tokens-0.5/src/cone/tokens/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `cone.tokens-0.4/src/cone/tokens/tests/test_token.py` & `cone_tokens-0.5/src/cone/tokens/tests/test_token.py`

 * *Files identical despite different names*

### Comparing `cone.tokens-0.4/src/cone.tokens.egg-info/PKG-INFO` & `cone_tokens-0.5/src/cone.tokens.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cone.tokens
-Version: 0.4
+Version: 0.5
 Summary: cone token api
 Home-page: http://github.com/conestack/cone.tokens
 Author: Cone Contributors
 Author-email: dev@conestack.org
 License: MIT
 Keywords: node pyramid cone web
 Classifier: Environment :: Web Environment
@@ -166,14 +166,28 @@
 - Torben Baumgartner
 - Lena Daxenbichler
 
 
 Changes
 =======
 
+0.5 (2024-05-23)
+----------------
+
+- Update Makefile.
+  [rnix]
+
+- ``properties`` and ``metadata`` of ``cone.tokens.model.Tokens`` are instance
+  properties now.
+  [rnix]
+
+- Use ``ts.http_request`` instead of ``ts.ajax.request``.
+  [rnix]
+
+
 0.4 (2024-02-12)
 ----------------
 
 - Adopt Settings UI changes from ``cone.app``.
   [rnix]
```

### Comparing `cone.tokens-0.4/src/cone.tokens.egg-info/SOURCES.txt` & `cone_tokens-0.5/src/cone.tokens.egg-info/SOURCES.txt`

 * *Files identical despite different names*

