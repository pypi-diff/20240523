# Comparing `tmp/pdfdol-0.1.4.tar.gz` & `tmp/pdfdol-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdfdol-0.1.4.tar", last modified: Thu May 23 12:25:58 2024, max compression
+gzip compressed data, was "pdfdol-0.1.5.tar", last modified: Thu May 23 12:27:36 2024, max compression
```

## Comparing `pdfdol-0.1.4.tar` & `pdfdol-0.1.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:25:58.200355 pdfdol-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-23 12:25:27.000000 pdfdol-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-05-23 12:25:58.200355 pdfdol-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-23 12:25:27.000000 pdfdol-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:25:58.200355 pdfdol-0.1.4/pdfdol/
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-23 12:25:27.000000 pdfdol-0.1.4/pdfdol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-23 12:25:27.000000 pdfdol-0.1.4/pdfdol/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:25:58.200355 pdfdol-0.1.4/pdfdol/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-23 12:25:27.000000 pdfdol-0.1.4/pdfdol/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-23 12:25:27.000000 pdfdol-0.1.4/pdfdol/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-23 12:25:27.000000 pdfdol-0.1.4/pdfdol/tests/utils_for_testing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4151 2024-05-23 12:25:35.000000 pdfdol-0.1.4/pdfdol/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:25:58.200355 pdfdol-0.1.4/pdfdol.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-05-23 12:25:58.000000 pdfdol-0.1.4/pdfdol.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-23 12:25:58.000000 pdfdol-0.1.4/pdfdol.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 12:25:58.000000 pdfdol-0.1.4/pdfdol.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 12:25:58.000000 pdfdol-0.1.4/pdfdol.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-23 12:25:58.000000 pdfdol-0.1.4/pdfdol.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-23 12:25:58.000000 pdfdol-0.1.4/pdfdol.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-23 12:25:58.204355 pdfdol-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-23 12:25:27.000000 pdfdol-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:27:36.323398 pdfdol-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-23 12:27:12.000000 pdfdol-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-23 12:27:36.323398 pdfdol-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-23 12:27:12.000000 pdfdol-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:27:36.319398 pdfdol-0.1.5/pdfdol/
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-23 12:27:12.000000 pdfdol-0.1.5/pdfdol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-23 12:27:12.000000 pdfdol-0.1.5/pdfdol/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:27:36.323398 pdfdol-0.1.5/pdfdol/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-23 12:27:12.000000 pdfdol-0.1.5/pdfdol/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      444 2024-05-23 12:27:12.000000 pdfdol-0.1.5/pdfdol/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-23 12:27:12.000000 pdfdol-0.1.5/pdfdol/tests/utils_for_testing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4151 2024-05-23 12:27:16.000000 pdfdol-0.1.5/pdfdol/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:27:36.323398 pdfdol-0.1.5/pdfdol.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-23 12:27:36.000000 pdfdol-0.1.5/pdfdol.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-23 12:27:36.000000 pdfdol-0.1.5/pdfdol.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 12:27:36.000000 pdfdol-0.1.5/pdfdol.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 12:27:36.000000 pdfdol-0.1.5/pdfdol.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-23 12:27:36.000000 pdfdol-0.1.5/pdfdol.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-23 12:27:36.000000 pdfdol-0.1.5/pdfdol.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-23 12:27:36.323398 pdfdol-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-23 12:27:12.000000 pdfdol-0.1.5/setup.py
```

### Comparing `pdfdol-0.1.4/LICENSE` & `pdfdol-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pdfdol-0.1.4/PKG-INFO` & `pdfdol-0.1.5/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,7 @@
-Metadata-Version: 2.1
-Name: pdfdol
-Version: 0.1.4
-Summary: Data Object Layer for PDF data
-Author: OtoSense
-License: mit
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 
 # pdfdol
 Data Object Layer for PDF data
 
 
 To install:	```pip install pdfdol```
 
@@ -44,7 +35,18 @@
 from dol import add_decoder
 page_separator = '---------------------'
 FilesReader = add_decoder(PdfFilesReader, decoder=page_separator.join)
 # and then
 pdfs = FilesReader(folder_path)
 # ...
 ```
+
+If you need to concatinate a bunch of pdfs together, you can do so in many
+ways. Here's one:
+
+```python
+from dol import Files
+from pdfdol import concat_pdfs
+
+s = Files('~/Downloads/cosmograph_documentation_pdfs/')
+concat_pdfs(s, key_order=sorted)
+```
```

### Comparing `pdfdol-0.1.4/pdfdol/base.py` & `pdfdol-0.1.5/pdfdol/base.py`

 * *Files identical despite different names*

### Comparing `pdfdol-0.1.4/pdfdol/util.py` & `pdfdol-0.1.5/pdfdol/util.py`

 * *Files identical despite different names*

### Comparing `pdfdol-0.1.4/pdfdol.egg-info/PKG-INFO` & `pdfdol-0.1.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdfdol
-Version: 0.1.4
+Version: 0.1.5
 Summary: Data Object Layer for PDF data
 Author: OtoSense
 License: mit
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
@@ -44,7 +44,18 @@
 from dol import add_decoder
 page_separator = '---------------------'
 FilesReader = add_decoder(PdfFilesReader, decoder=page_separator.join)
 # and then
 pdfs = FilesReader(folder_path)
 # ...
 ```
+
+If you need to concatinate a bunch of pdfs together, you can do so in many
+ways. Here's one:
+
+```python
+from dol import Files
+from pdfdol import concat_pdfs
+
+s = Files('~/Downloads/cosmograph_documentation_pdfs/')
+concat_pdfs(s, key_order=sorted)
+```
```

