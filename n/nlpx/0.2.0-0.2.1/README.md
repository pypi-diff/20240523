# Comparing `tmp/nlpx-0.2.0.tar.gz` & `tmp/nlpx-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlpx-0.2.0.tar", last modified: Wed May 22 02:11:06 2024, max compression
+gzip compressed data, was "nlpx-0.2.1.tar", last modified: Thu May 23 00:31:58 2024, max compression
```

## Comparing `nlpx-0.2.0.tar` & `nlpx-0.2.1.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-22 02:11:06.590511 nlpx-0.2.0/
--rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-22 02:11:06.589764 nlpx-0.2.0/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)      448 2024-04-07 01:09:43.000000 nlpx-0.2.0/README.rst
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-22 02:11:06.582520 nlpx-0.2.0/nlpx/
--rw-r--r--   0 summy      (501) staff       (20)        0 2024-05-21 11:15:55.000000 nlpx-0.2.0/nlpx/__init__.py
--rw-r--r--   0 summy      (501) staff       (20)    41701 2024-04-07 00:53:15.000000 nlpx-0.2.0/nlpx/text_token.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-22 02:11:06.587431 nlpx-0.2.0/nlpx.egg-info/
--rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-22 02:11:06.000000 nlpx-0.2.0/nlpx.egg-info/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)      194 2024-05-22 02:11:06.000000 nlpx-0.2.0/nlpx.egg-info/SOURCES.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-22 02:11:06.000000 nlpx-0.2.0/nlpx.egg-info/dependency_links.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-22 02:11:06.000000 nlpx-0.2.0/nlpx.egg-info/not-zip-safe
--rw-r--r--   0 summy      (501) staff       (20)        5 2024-05-22 02:11:06.000000 nlpx-0.2.0/nlpx.egg-info/top_level.txt
--rw-r--r--   0 summy      (501) staff       (20)       38 2024-05-22 02:11:06.590764 nlpx-0.2.0/setup.cfg
--rw-r--r--   0 summy      (501) staff       (20)      998 2024-05-22 02:11:00.000000 nlpx-0.2.0/setup.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-23 00:31:58.669281 nlpx-0.2.1/
+-rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-23 00:31:58.668810 nlpx-0.2.1/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)      448 2024-04-07 01:09:43.000000 nlpx-0.2.1/README.rst
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-23 00:31:58.662931 nlpx-0.2.1/nlpx/
+-rw-r--r--   0 summy      (501) staff       (20)        0 2024-05-21 11:15:55.000000 nlpx-0.2.1/nlpx/__init__.py
+-rw-r--r--   0 summy      (501) staff       (20)     2091 2024-05-21 12:03:46.000000 nlpx-0.2.1/nlpx/_text_cnn.py
+-rw-r--r--   0 summy      (501) staff       (20)       30 2024-05-23 00:31:50.000000 nlpx-0.2.1/nlpx/models.py
+-rw-r--r--   0 summy      (501) staff       (20)    41701 2024-04-07 00:53:15.000000 nlpx-0.2.1/nlpx/text_token.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-23 00:31:58.668084 nlpx-0.2.1/nlpx.egg-info/
+-rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-23 00:31:58.000000 nlpx-0.2.1/nlpx.egg-info/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)      227 2024-05-23 00:31:58.000000 nlpx-0.2.1/nlpx.egg-info/SOURCES.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-23 00:31:58.000000 nlpx-0.2.1/nlpx.egg-info/dependency_links.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-23 00:31:58.000000 nlpx-0.2.1/nlpx.egg-info/not-zip-safe
+-rw-r--r--   0 summy      (501) staff       (20)        5 2024-05-23 00:31:58.000000 nlpx-0.2.1/nlpx.egg-info/top_level.txt
+-rw-r--r--   0 summy      (501) staff       (20)       38 2024-05-23 00:31:58.669492 nlpx-0.2.1/setup.cfg
+-rw-r--r--   0 summy      (501) staff       (20)      998 2024-05-23 00:31:50.000000 nlpx-0.2.1/setup.py
```

### Comparing `nlpx-0.2.0/PKG-INFO` & `nlpx-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: nlpx
-Version: 0.2.0
+Version: 0.2.1
 Summary: A tool set for NLP.
 Home-page: https://gitee.com/summry/nlpx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: NLP
 Platform: UNKNOWN
-Requires-Python: >=3.5
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 Usage Sample
 ''''''''''''
 
 .. code:: python
```

### Comparing `nlpx-0.2.0/nlpx/text_token.py` & `nlpx-0.2.1/nlpx/text_token.py`

 * *Files identical despite different names*

### Comparing `nlpx-0.2.0/nlpx.egg-info/PKG-INFO` & `nlpx-0.2.1/nlpx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: nlpx
-Version: 0.2.0
+Version: 0.2.1
 Summary: A tool set for NLP.
 Home-page: https://gitee.com/summry/nlpx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: NLP
 Platform: UNKNOWN
-Requires-Python: >=3.5
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 Usage Sample
 ''''''''''''
 
 .. code:: python
```

