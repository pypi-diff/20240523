# Comparing `tmp/bibla-2.0.6.tar.gz` & `tmp/bibla-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bibla-2.0.6.tar", last modified: Thu May 23 08:31:52 2024, max compression
+gzip compressed data, was "bibla-2.0.7.tar", last modified: Thu May 23 09:11:42 2024, max compression
```

## Comparing `bibla-2.0.6.tar` & `bibla-2.0.7.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:31:52.173184 bibla-2.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-23 08:31:43.000000 bibla-2.0.6/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:31:52.169184 bibla-2.0.6/.idea/
--rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-23 08:31:43.000000 bibla-2.0.6/.idea/biblint.iml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:31:52.169184 bibla-2.0.6/.idea/inspectionProfiles/
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-23 08:31:43.000000 bibla-2.0.6/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-23 08:31:43.000000 bibla-2.0.6/.idea/misc.xml
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-23 08:31:43.000000 bibla-2.0.6/.idea/modules.xml
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-23 08:31:43.000000 bibla-2.0.6/.idea/vcs.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-23 08:31:43.000000 bibla-2.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-23 08:31:43.000000 bibla-2.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6329 2024-05-23 08:31:52.173184 bibla-2.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5377 2024-05-23 08:31:43.000000 bibla-2.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:31:52.169184 bibla-2.0.6/bibla/
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-23 08:31:43.000000 bibla-2.0.6/bibla/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3760 2024-05-23 08:31:43.000000 bibla-2.0.6/bibla/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3169 2024-05-23 08:31:43.000000 bibla-2.0.6/bibla/bibla.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-05-23 08:31:43.000000 bibla-2.0.6/bibla/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4485 2024-05-23 08:31:43.000000 bibla-2.0.6/bibla/lint.py
--rw-r--r--   0 runner    (1001) docker     (127)     5259 2024-05-23 08:31:43.000000 bibla-2.0.6/bibla/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:31:52.169184 bibla-2.0.6/bibla/rules/
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-23 08:31:43.000000 bibla-2.0.6/bibla/rules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-05-23 08:31:43.000000 bibla-2.0.6/bibla/rules/database_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)    13866 2024-05-23 08:31:43.000000 bibla-2.0.6/bibla/rules/entry_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     5619 2024-05-23 08:31:43.000000 bibla-2.0.6/bibla/rules/field_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-05-23 08:31:43.000000 bibla-2.0.6/bibla/rules/specification_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-05-23 08:31:43.000000 bibla-2.0.6/bibla/rules/text_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-05-23 08:31:43.000000 bibla-2.0.6/bibla/text_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:31:52.173184 bibla-2.0.6/bibla.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6329 2024-05-23 08:31:52.000000 bibla-2.0.6/bibla.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-05-23 08:31:52.000000 bibla-2.0.6/bibla.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 08:31:52.000000 bibla-2.0.6/bibla.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-23 08:31:52.000000 bibla-2.0.6/bibla.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-23 08:31:52.000000 bibla-2.0.6/bibla.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-23 08:31:52.000000 bibla-2.0.6/bibla.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 08:31:52.173184 bibla-2.0.6/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1575 2024-05-23 08:31:43.000000 bibla-2.0.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:31:52.169184 bibla-2.0.6/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 08:31:43.000000 bibla-2.0.6/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-23 08:31:43.000000 bibla-2.0.6/test/test_base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 08:31:52.173184 bibla-2.0.6/test_data/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-23 08:31:43.000000 bibla-2.0.6/test_data/.bibla.yml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 08:31:43.000000 bibla-2.0.6/test_data/authorNameFormatting.bib
--rw-r--r--   0 runner    (1001) docker     (127)    13625 2024-05-23 08:31:43.000000 bibla-2.0.6/test_data/bibLaTeX.bib
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-23 08:31:43.000000 bibla-2.0.6/test_data/dateFormat.bib
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-23 08:31:43.000000 bibla-2.0.6/test_data/emptyEntries.bib
--rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-05-23 08:31:43.000000 bibla-2.0.6/test_data/mit.bib
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-23 08:31:43.000000 bibla-2.0.6/test_data/noHomepages.bib
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-05-23 08:31:43.000000 bibla-2.0.6/test_data/nodirectives.bib
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-23 08:31:43.000000 bibla-2.0.6/test_data/nokeys.bib
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-23 08:31:43.000000 bibla-2.0.6/test_data/originalOverAlias.bib
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-23 08:31:43.000000 bibla-2.0.6/test_data/pages.bib
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-23 08:31:43.000000 bibla-2.0.6/test_data/required.bib
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-23 08:31:43.000000 bibla-2.0.6/test_data/shouldUseDateInsteadOfYearMonthDay.bib
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-23 08:31:43.000000 bibla-2.0.6/test_data/suggestedFields.bib
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-23 08:31:43.000000 bibla-2.0.6/test_data/syntax.bib
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-23 08:31:43.000000 bibla-2.0.6/test_data/unique.bib
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-23 08:31:43.000000 bibla-2.0.6/test_data/wrongDateFormat.bib
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-23 08:31:43.000000 bibla-2.0.6/test_data/wrongFormatKey.bib
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:11:42.336589 bibla-2.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-23 09:11:37.000000 bibla-2.0.7/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:11:42.328589 bibla-2.0.7/.idea/
+-rw-r--r--   0 runner    (1001) docker     (127)      572 2024-05-23 09:11:37.000000 bibla-2.0.7/.idea/biblint.iml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:11:42.328589 bibla-2.0.7/.idea/inspectionProfiles/
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-23 09:11:37.000000 bibla-2.0.7/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-23 09:11:37.000000 bibla-2.0.7/.idea/misc.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-23 09:11:37.000000 bibla-2.0.7/.idea/modules.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-23 09:11:37.000000 bibla-2.0.7/.idea/vcs.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-23 09:11:37.000000 bibla-2.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-23 09:11:37.000000 bibla-2.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6363 2024-05-23 09:11:42.336589 bibla-2.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5377 2024-05-23 09:11:37.000000 bibla-2.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:11:42.328589 bibla-2.0.7/bibla/
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-23 09:11:37.000000 bibla-2.0.7/bibla/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3760 2024-05-23 09:11:37.000000 bibla-2.0.7/bibla/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3169 2024-05-23 09:11:37.000000 bibla-2.0.7/bibla/bibla.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-05-23 09:11:37.000000 bibla-2.0.7/bibla/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4485 2024-05-23 09:11:37.000000 bibla-2.0.7/bibla/lint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5259 2024-05-23 09:11:37.000000 bibla-2.0.7/bibla/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:11:42.332589 bibla-2.0.7/bibla/rules/
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-23 09:11:37.000000 bibla-2.0.7/bibla/rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-05-23 09:11:37.000000 bibla-2.0.7/bibla/rules/database_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13866 2024-05-23 09:11:37.000000 bibla-2.0.7/bibla/rules/entry_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5716 2024-05-23 09:11:37.000000 bibla-2.0.7/bibla/rules/field_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2428 2024-05-23 09:11:37.000000 bibla-2.0.7/bibla/rules/specification_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3101 2024-05-23 09:11:37.000000 bibla-2.0.7/bibla/rules/text_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-05-23 09:11:37.000000 bibla-2.0.7/bibla/text_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:11:42.336589 bibla-2.0.7/bibla.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6363 2024-05-23 09:11:42.000000 bibla-2.0.7/bibla.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-05-23 09:11:42.000000 bibla-2.0.7/bibla.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 09:11:42.000000 bibla-2.0.7/bibla.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-23 09:11:42.000000 bibla-2.0.7/bibla.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-23 09:11:42.000000 bibla-2.0.7/bibla.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-23 09:11:42.000000 bibla-2.0.7/bibla.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 09:11:42.336589 bibla-2.0.7/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1605 2024-05-23 09:11:37.000000 bibla-2.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:11:42.332589 bibla-2.0.7/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 09:11:37.000000 bibla-2.0.7/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-23 09:11:37.000000 bibla-2.0.7/test/test_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:11:42.336589 bibla-2.0.7/test_data/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-23 09:11:37.000000 bibla-2.0.7/test_data/.bibla.yml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 09:11:37.000000 bibla-2.0.7/test_data/authorNameFormatting.bib
+-rw-r--r--   0 runner    (1001) docker     (127)    13625 2024-05-23 09:11:37.000000 bibla-2.0.7/test_data/bibLaTeX.bib
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-23 09:11:37.000000 bibla-2.0.7/test_data/dateFormat.bib
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-23 09:11:37.000000 bibla-2.0.7/test_data/emptyEntries.bib
+-rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-05-23 09:11:37.000000 bibla-2.0.7/test_data/mit.bib
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-23 09:11:37.000000 bibla-2.0.7/test_data/noHomepages.bib
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-05-23 09:11:37.000000 bibla-2.0.7/test_data/nodirectives.bib
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-23 09:11:37.000000 bibla-2.0.7/test_data/nokeys.bib
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-23 09:11:37.000000 bibla-2.0.7/test_data/originalOverAlias.bib
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-23 09:11:37.000000 bibla-2.0.7/test_data/pages.bib
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-23 09:11:37.000000 bibla-2.0.7/test_data/required.bib
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-23 09:11:37.000000 bibla-2.0.7/test_data/shouldUseDateInsteadOfYearMonthDay.bib
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-23 09:11:37.000000 bibla-2.0.7/test_data/suggestedFields.bib
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-23 09:11:37.000000 bibla-2.0.7/test_data/syntax.bib
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-23 09:11:37.000000 bibla-2.0.7/test_data/unique.bib
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-23 09:11:37.000000 bibla-2.0.7/test_data/wrongDateFormat.bib
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-23 09:11:37.000000 bibla-2.0.7/test_data/wrongFormatKey.bib
```

### Comparing `bibla-2.0.6/.idea/biblint.iml` & `bibla-2.0.7/.idea/biblint.iml`

 * *Files identical despite different names*

### Comparing `bibla-2.0.6/LICENSE` & `bibla-2.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `bibla-2.0.6/PKG-INFO` & `bibla-2.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bibla
-Version: 2.0.6
+Version: 2.0.7
 Summary: A minimalistic bibLaTeX linter by Tristan Cuvelier.
 Home-page: https://github.com/MrClassicT/bibla
 Author: Tristan Cuvelier
 Author-email: tristan.cuvelier@student.hogent.be
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -16,14 +16,15 @@
 License-File: LICENSE
 Requires-Dist: click>=7
 Requires-Dist: fuzzywuzzy>=0.10
 Requires-Dist: markdown-table
 Requires-Dist: pybtex==0.23.0
 Requires-Dist: pyyaml>=5
 Requires-Dist: unidecode<2,>=1
+Requires-Dist: setuptools>=69.0.0
 Provides-Extra: dev
 Requires-Dist: anybadge; extra == "dev"
 Requires-Dist: markdown; extra == "dev"
 Requires-Dist: check-manifest; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 
 # bibla
```

### Comparing `bibla-2.0.6/README.md` & `bibla-2.0.7/README.md`

 * *Files identical despite different names*

### Comparing `bibla-2.0.6/bibla/__main__.py` & `bibla-2.0.7/bibla/__main__.py`

 * *Files identical despite different names*

### Comparing `bibla-2.0.6/bibla/bibla.yml` & `bibla-2.0.7/bibla/bibla.yml`

 * *Files identical despite different names*

### Comparing `bibla-2.0.6/bibla/config.py` & `bibla-2.0.7/bibla/config.py`

 * *Files identical despite different names*

### Comparing `bibla-2.0.6/bibla/lint.py` & `bibla-2.0.7/bibla/lint.py`

 * *Files identical despite different names*

### Comparing `bibla-2.0.6/bibla/rule.py` & `bibla-2.0.7/bibla/rule.py`

 * *Files identical despite different names*

### Comparing `bibla-2.0.6/bibla/rules/database_rules.py` & `bibla-2.0.7/bibla/rules/database_rules.py`

 * *Files identical despite different names*

### Comparing `bibla-2.0.6/bibla/rules/entry_rules.py` & `bibla-2.0.7/bibla/rules/entry_rules.py`

 * *Files identical despite different names*

### Comparing `bibla-2.0.6/bibla/rules/field_rules.py` & `bibla-2.0.7/bibla/rules/field_rules.py`

 * *Files 3% similar despite different names*

```diff
@@ -105,13 +105,15 @@
     :param key: The key of the current bibliography entry
     :param entry: The current bibliography entry
     :param database: All bibliography entries
     :return: True if no field contains special characters, False otherwise.
     """
     special_chars = ['%', '&', '$', '#', '_', '\\', '~', '^', '|']
 
-    for field in entry.fields.values():
-        if any(char in field for char in special_chars):
+    for field_name, field_value in entry.fields.items():
+        if field_name == 'url':
+            return True
+        if any(char in field_value for char in special_chars):
             for char in special_chars:
-                if char in field and field[field.index(char) - 1] != '\\':
+                if char in field_value and field_value[field_value.index(char) - 1] != '\\':
                     return False
     return True
```

### Comparing `bibla-2.0.6/bibla/rules/specification_rules.py` & `bibla-2.0.7/bibla/rules/specification_rules.py`

 * *Files identical despite different names*

### Comparing `bibla-2.0.6/bibla/rules/text_rules.py` & `bibla-2.0.7/bibla/rules/text_rules.py`

 * *Files identical despite different names*

### Comparing `bibla-2.0.6/bibla/text_utils.py` & `bibla-2.0.7/bibla/text_utils.py`

 * *Files identical despite different names*

### Comparing `bibla-2.0.6/bibla.egg-info/PKG-INFO` & `bibla-2.0.7/bibla.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bibla
-Version: 2.0.6
+Version: 2.0.7
 Summary: A minimalistic bibLaTeX linter by Tristan Cuvelier.
 Home-page: https://github.com/MrClassicT/bibla
 Author: Tristan Cuvelier
 Author-email: tristan.cuvelier@student.hogent.be
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -16,14 +16,15 @@
 License-File: LICENSE
 Requires-Dist: click>=7
 Requires-Dist: fuzzywuzzy>=0.10
 Requires-Dist: markdown-table
 Requires-Dist: pybtex==0.23.0
 Requires-Dist: pyyaml>=5
 Requires-Dist: unidecode<2,>=1
+Requires-Dist: setuptools>=69.0.0
 Provides-Extra: dev
 Requires-Dist: anybadge; extra == "dev"
 Requires-Dist: markdown; extra == "dev"
 Requires-Dist: check-manifest; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 
 # bibla
```

### Comparing `bibla-2.0.6/bibla.egg-info/SOURCES.txt` & `bibla-2.0.7/bibla.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bibla-2.0.6/setup.py` & `bibla-2.0.7/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,14 +32,15 @@
     install_requires=[
         'click>=7',
         'fuzzywuzzy>=0.10',
         'markdown-table',
         'pybtex==0.23.0',
         'pyyaml>=5',
         'unidecode>=1,<2',
+        'setuptools>= 69.0.0'
     ],
     extras_require={
         'dev': [
             'anybadge',
             'markdown',
             'check-manifest',
             'twine',
```

### Comparing `bibla-2.0.6/test_data/bibLaTeX.bib` & `bibla-2.0.7/test_data/bibLaTeX.bib`

 * *Files identical despite different names*

### Comparing `bibla-2.0.6/test_data/mit.bib` & `bibla-2.0.7/test_data/mit.bib`

 * *Files identical despite different names*

### Comparing `bibla-2.0.6/test_data/nodirectives.bib` & `bibla-2.0.7/test_data/nodirectives.bib`

 * *Files identical despite different names*

### Comparing `bibla-2.0.6/test_data/originalOverAlias.bib` & `bibla-2.0.7/test_data/originalOverAlias.bib`

 * *Files identical despite different names*

### Comparing `bibla-2.0.6/test_data/wrongDateFormat.bib` & `bibla-2.0.7/test_data/wrongDateFormat.bib`

 * *Files identical despite different names*

