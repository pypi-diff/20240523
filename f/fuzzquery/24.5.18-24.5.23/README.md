# Comparing `tmp/fuzzquery-24.5.18.tar.gz` & `tmp/fuzzquery-24.5.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fuzzquery-24.5.18.tar", last modified: Fri May 17 22:11:39 2024, max compression
+gzip compressed data, was "fuzzquery-24.5.23.tar", last modified: Thu May 23 10:12:19 2024, max compression
```

## Comparing `fuzzquery-24.5.18.tar` & `fuzzquery-24.5.23.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-17 22:11:39.524670 fuzzquery-24.5.18/
--rw-rw-rw-   0        0        0     1090 2024-05-16 01:40:27.000000 fuzzquery-24.5.18/LICENSE
--rw-rw-rw-   0        0        0     5817 2024-05-17 22:11:39.524670 fuzzquery-24.5.18/PKG-INFO
--rw-rw-rw-   0        0        0     5003 2024-05-17 22:10:28.000000 fuzzquery-24.5.18/README.md
--rw-rw-rw-   0        0        0      911 2024-05-17 22:10:40.000000 fuzzquery-24.5.18/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-17 22:11:39.524670 fuzzquery-24.5.18/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-17 22:11:39.415294 fuzzquery-24.5.18/src/
-drwxrwxrwx   0        0        0        0 2024-05-17 22:11:39.446541 fuzzquery-24.5.18/src/fuzzquery/
--rw-rw-rw-   0        0        0       22 2024-05-17 02:21:23.000000 fuzzquery-24.5.18/src/fuzzquery/__init__.py
--rw-rw-rw-   0        0        0     4355 2024-05-17 22:07:32.000000 fuzzquery-24.5.18/src/fuzzquery/fuzzy.py
-drwxrwxrwx   0        0        0        0 2024-05-17 22:11:39.509045 fuzzquery-24.5.18/src/fuzzquery.egg-info/
--rw-rw-rw-   0        0        0     5817 2024-05-17 22:11:39.000000 fuzzquery-24.5.18/src/fuzzquery.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      265 2024-05-17 22:11:39.000000 fuzzquery-24.5.18/src/fuzzquery.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 22:11:39.000000 fuzzquery-24.5.18/src/fuzzquery.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-05-17 22:11:39.000000 fuzzquery-24.5.18/src/fuzzquery.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-17 22:11:39.000000 fuzzquery-24.5.18/src/fuzzquery.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-23 10:12:19.037449 fuzzquery-24.5.23/
+-rw-rw-rw-   0        0        0     1090 2024-05-16 01:40:27.000000 fuzzquery-24.5.23/LICENSE
+-rw-rw-rw-   0        0        0     5832 2024-05-23 10:12:19.033447 fuzzquery-24.5.23/PKG-INFO
+-rw-rw-rw-   0        0        0     5003 2024-05-17 22:10:28.000000 fuzzquery-24.5.23/README.md
+-rw-rw-rw-   0        0        0      926 2024-05-23 10:11:49.000000 fuzzquery-24.5.23/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-23 10:12:19.038452 fuzzquery-24.5.23/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-23 10:12:18.959034 fuzzquery-24.5.23/src/
+drwxrwxrwx   0        0        0        0 2024-05-23 10:12:18.989714 fuzzquery-24.5.23/src/fuzzquery/
+-rw-rw-rw-   0        0        0     5266 2024-05-23 08:45:12.000000 fuzzquery-24.5.23/src/fuzzquery/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 10:12:19.026434 fuzzquery-24.5.23/src/fuzzquery.egg-info/
+-rw-rw-rw-   0        0        0     5832 2024-05-23 10:12:18.000000 fuzzquery-24.5.23/src/fuzzquery.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      242 2024-05-23 10:12:18.000000 fuzzquery-24.5.23/src/fuzzquery.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 10:12:18.000000 fuzzquery-24.5.23/src/fuzzquery.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-23 10:12:18.000000 fuzzquery-24.5.23/src/fuzzquery.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-23 10:12:18.000000 fuzzquery-24.5.23/src/fuzzquery.egg-info/top_level.txt
```

### Comparing `fuzzquery-24.5.18/LICENSE` & `fuzzquery-24.5.23/LICENSE`

 * *Files identical despite different names*

### Comparing `fuzzquery-24.5.18/PKG-INFO` & `fuzzquery-24.5.23/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: fuzzquery
-Version: 24.5.18
-Summary: A lightweight package for performing fuzzy string matching with a very simple token system
+Version: 24.5.23
+Summary: A lightweight package for fuzzy word/phrase searches in a body of text, using a very simple token system.
 Author-email: Oyster Shucker <onemadgypsy@gmail.com>
 Maintainer-email: Oyster Shucker <onemadgypsy@gmail.com>
 Project-URL: Homepage, https://github.com/OneMadGypsy/fuzzquery
 Project-URL: Issues, https://github.com/OneMadGypsy/fuzzquery/issues
 Keywords: fuzzy,string,matching,token,regex
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 4 - Beta
```

### Comparing `fuzzquery-24.5.18/README.md` & `fuzzquery-24.5.23/README.md`

 * *Files identical despite different names*

### Comparing `fuzzquery-24.5.18/pyproject.toml` & `fuzzquery-24.5.23/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fuzzquery"
-version = "24.5.18"
-description = "A lightweight package for performing fuzzy string matching with a very simple token system"
+version = "24.5.23"
+description = "A lightweight package for fuzzy word/phrase searches in a body of text, using a very simple token system."
 dependencies = ["regex>=2024.5.15",]
 keywords = ["fuzzy", "string", "matching", "token", "regex"]
 authors = [{ name="Oyster Shucker", email="onemadgypsy@gmail.com" },]
 maintainers = [{ name="Oyster Shucker", email="onemadgypsy@gmail.com" },]
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `fuzzquery-24.5.18/src/fuzzquery.egg-info/PKG-INFO` & `fuzzquery-24.5.23/src/fuzzquery.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: fuzzquery
-Version: 24.5.18
-Summary: A lightweight package for performing fuzzy string matching with a very simple token system
+Version: 24.5.23
+Summary: A lightweight package for fuzzy word/phrase searches in a body of text, using a very simple token system.
 Author-email: Oyster Shucker <onemadgypsy@gmail.com>
 Maintainer-email: Oyster Shucker <onemadgypsy@gmail.com>
 Project-URL: Homepage, https://github.com/OneMadGypsy/fuzzquery
 Project-URL: Issues, https://github.com/OneMadGypsy/fuzzquery/issues
 Keywords: fuzzy,string,matching,token,regex
 Classifier: Intended Audience :: Developers
 Classifier: Development Status :: 4 - Beta
```

