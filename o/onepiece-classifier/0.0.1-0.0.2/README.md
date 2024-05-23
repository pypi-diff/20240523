# Comparing `tmp/onepiece_classifier-0.0.1.tar.gz` & `tmp/onepiece_classifier-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onepiece_classifier-0.0.1.tar", last modified: Thu May 23 06:29:37 2024, max compression
+gzip compressed data, was "onepiece_classifier-0.0.2.tar", last modified: Thu May 23 07:15:08 2024, max compression
```

## Comparing `onepiece_classifier-0.0.1.tar` & `onepiece_classifier-0.0.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 annur-afgoni  (1000) annur-afgoni  (1000)        0 2024-05-23 06:29:37.099525 onepiece_classifier-0.0.1/
--rw-rw-r--   0 annur-afgoni  (1000) annur-afgoni  (1000)    11357 2024-05-16 06:56:44.000000 onepiece_classifier-0.0.1/LICENSE
--rw-r--r--   0 annur-afgoni  (1000) annur-afgoni  (1000)     3025 2024-05-23 06:29:37.099525 onepiece_classifier-0.0.1/PKG-INFO
--rw-rw-r--   0 annur-afgoni  (1000) annur-afgoni  (1000)     2566 2024-05-21 13:06:55.000000 onepiece_classifier-0.0.1/README.md
--rw-rw-r--   0 annur-afgoni  (1000) annur-afgoni  (1000)      878 2024-05-23 06:29:37.100525 onepiece_classifier-0.0.1/setup.cfg
--rw-rw-r--   0 annur-afgoni  (1000) annur-afgoni  (1000)       38 2024-05-23 05:50:56.000000 onepiece_classifier-0.0.1/setup.py
-drwxrwxr-x   0 annur-afgoni  (1000) annur-afgoni  (1000)        0 2024-05-23 06:29:37.091525 onepiece_classifier-0.0.1/src/
-drwxrwxr-x   0 annur-afgoni  (1000) annur-afgoni  (1000)        0 2024-05-23 06:29:37.099525 onepiece_classifier-0.0.1/src/onepiece_classifier.egg-info/
--rw-r--r--   0 annur-afgoni  (1000) annur-afgoni  (1000)     3025 2024-05-23 06:29:36.000000 onepiece_classifier-0.0.1/src/onepiece_classifier.egg-info/PKG-INFO
--rw-rw-r--   0 annur-afgoni  (1000) annur-afgoni  (1000)      877 2024-05-23 06:29:37.000000 onepiece_classifier-0.0.1/src/onepiece_classifier.egg-info/SOURCES.txt
--rw-rw-r--   0 annur-afgoni  (1000) annur-afgoni  (1000)        1 2024-05-23 06:29:36.000000 onepiece_classifier-0.0.1/src/onepiece_classifier.egg-info/dependency_links.txt
--rw-rw-r--   0 annur-afgoni  (1000) annur-afgoni  (1000)       45 2024-05-23 06:29:36.000000 onepiece_classifier-0.0.1/src/onepiece_classifier.egg-info/requires.txt
--rw-rw-r--   0 annur-afgoni  (1000) annur-afgoni  (1000)       18 2024-05-23 06:29:36.000000 onepiece_classifier-0.0.1/src/onepiece_classifier.egg-info/top_level.txt
-drwxrwxr-x   0 annur-afgoni  (1000) annur-afgoni  (1000)        0 2024-05-23 06:29:37.095525 onepiece_classifier-0.0.1/src/onepiece_classify/
--rw-rw-r--   0 annur-afgoni  (1000) annur-afgoni  (1000)        0 2024-05-16 06:56:44.000000 onepiece_classifier-0.0.1/src/onepiece_classify/__init__.py
-drwxrwxr-x   0 annur-afgoni  (1000) annur-afgoni  (1000)        0 2024-05-23 06:29:37.095525 onepiece_classifier-0.0.1/src/onepiece_classify/data/
--rw-rw-r--   0 annur-afgoni  (1000) annur-afgoni  (1000)       26 2024-05-16 08:43:40.000000 onepiece_classifier-0.0.1/src/onepiece_classify/data/__init__.py
--rw-rw-r--   0 annur-afgoni  (1000) annur-afgoni  (1000)     2126 2024-05-16 08:43:40.000000 onepiece_classifier-0.0.1/src/onepiece_classify/data/setup_data.py
-drwxrwxr-x   0 annur-afgoni  (1000) annur-afgoni  (1000)        0 2024-05-23 06:29:37.096525 onepiece_classifier-0.0.1/src/onepiece_classify/infer/
--rw-rw-r--   0 annur-afgoni  (1000) annur-afgoni  (1000)       47 2024-05-16 08:43:40.000000 onepiece_classifier-0.0.1/src/onepiece_classify/infer/__init__.py
--rw-rw-r--   0 annur-afgoni  (1000) annur-afgoni  (1000)      592 2024-05-16 08:43:40.000000 onepiece_classifier-0.0.1/src/onepiece_classify/infer/base.py
--rw-rw-r--   0 annur-afgoni  (1000) annur-afgoni  (1000)     3563 2024-05-22 07:54:21.000000 onepiece_classifier-0.0.1/src/onepiece_classify/infer/recognition.py
-drwxrwxr-x   0 annur-afgoni  (1000) annur-afgoni  (1000)        0 2024-05-23 06:29:37.096525 onepiece_classifier-0.0.1/src/onepiece_classify/io/
--rw-rw-r--   0 annur-afgoni  (1000) annur-afgoni  (1000)        0 2024-05-16 06:56:44.000000 onepiece_classifier-0.0.1/src/onepiece_classify/io/__init__.py
-drwxrwxr-x   0 annur-afgoni  (1000) annur-afgoni  (1000)        0 2024-05-23 06:29:37.096525 onepiece_classifier-0.0.1/src/onepiece_classify/models/
--rw-rw-r--   0 annur-afgoni  (1000) annur-afgoni  (1000)       27 2024-05-16 08:43:40.000000 onepiece_classifier-0.0.1/src/onepiece_classify/models/__init__.py
--rw-rw-r--   0 annur-afgoni  (1000) annur-afgoni  (1000)      786 2024-05-16 08:43:40.000000 onepiece_classifier-0.0.1/src/onepiece_classify/models/build_model.py
-drwxrwxr-x   0 annur-afgoni  (1000) annur-afgoni  (1000)        0 2024-05-23 06:29:37.097525 onepiece_classifier-0.0.1/src/onepiece_classify/trainer/
--rw-rw-r--   0 annur-afgoni  (1000) annur-afgoni  (1000)       23 2024-05-16 08:43:40.000000 onepiece_classifier-0.0.1/src/onepiece_classify/trainer/__init__.py
--rw-rw-r--   0 annur-afgoni  (1000) annur-afgoni  (1000)     4781 2024-05-16 08:43:40.000000 onepiece_classifier-0.0.1/src/onepiece_classify/trainer/trainer.py
-drwxrwxr-x   0 annur-afgoni  (1000) annur-afgoni  (1000)        0 2024-05-23 06:29:37.098525 onepiece_classifier-0.0.1/src/onepiece_classify/transforms/
--rw-rw-r--   0 annur-afgoni  (1000) annur-afgoni  (1000)       21 2024-05-16 08:43:40.000000 onepiece_classifier-0.0.1/src/onepiece_classify/transforms/__init__.py
--rw-rw-r--   0 annur-afgoni  (1000) annur-afgoni  (1000)     1095 2024-05-16 08:43:40.000000 onepiece_classifier-0.0.1/src/onepiece_classify/transforms/trans.py
-drwxrwxr-x   0 annur-afgoni  (1000) annur-afgoni  (1000)        0 2024-05-23 06:29:37.098525 onepiece_classifier-0.0.1/src/onepiece_classify/utils/
--rw-rw-r--   0 annur-afgoni  (1000) annur-afgoni  (1000)       25 2024-05-22 04:34:21.000000 onepiece_classifier-0.0.1/src/onepiece_classify/utils/__init__.py
--rw-rw-r--   0 annur-afgoni  (1000) annur-afgoni  (1000)      380 2024-05-22 07:58:06.000000 onepiece_classifier-0.0.1/src/onepiece_classify/utils/downloader.py
+drwxrwxr-x   0 annur-afgoni  (1000) annur-afgoni  (1000)        0 2024-05-23 07:15:08.913372 onepiece_classifier-0.0.2/
+-rw-rw-r--   0 annur-afgoni  (1000) annur-afgoni  (1000)    11357 2024-05-16 06:56:44.000000 onepiece_classifier-0.0.2/LICENSE
+-rw-r--r--   0 annur-afgoni  (1000) annur-afgoni  (1000)     3025 2024-05-23 07:15:08.913372 onepiece_classifier-0.0.2/PKG-INFO
+-rw-rw-r--   0 annur-afgoni  (1000) annur-afgoni  (1000)     2566 2024-05-21 13:06:55.000000 onepiece_classifier-0.0.2/README.md
+-rw-rw-r--   0 annur-afgoni  (1000) annur-afgoni  (1000)      878 2024-05-23 07:15:08.914372 onepiece_classifier-0.0.2/setup.cfg
+-rw-rw-r--   0 annur-afgoni  (1000) annur-afgoni  (1000)       38 2024-05-23 05:50:56.000000 onepiece_classifier-0.0.2/setup.py
+drwxrwxr-x   0 annur-afgoni  (1000) annur-afgoni  (1000)        0 2024-05-23 07:15:08.904372 onepiece_classifier-0.0.2/src/
+drwxrwxr-x   0 annur-afgoni  (1000) annur-afgoni  (1000)        0 2024-05-23 07:15:08.912371 onepiece_classifier-0.0.2/src/onepiece_classifier.egg-info/
+-rw-r--r--   0 annur-afgoni  (1000) annur-afgoni  (1000)     3025 2024-05-23 07:15:08.000000 onepiece_classifier-0.0.2/src/onepiece_classifier.egg-info/PKG-INFO
+-rw-rw-r--   0 annur-afgoni  (1000) annur-afgoni  (1000)      877 2024-05-23 07:15:08.000000 onepiece_classifier-0.0.2/src/onepiece_classifier.egg-info/SOURCES.txt
+-rw-rw-r--   0 annur-afgoni  (1000) annur-afgoni  (1000)        1 2024-05-23 07:15:08.000000 onepiece_classifier-0.0.2/src/onepiece_classifier.egg-info/dependency_links.txt
+-rw-rw-r--   0 annur-afgoni  (1000) annur-afgoni  (1000)       45 2024-05-23 07:15:08.000000 onepiece_classifier-0.0.2/src/onepiece_classifier.egg-info/requires.txt
+-rw-rw-r--   0 annur-afgoni  (1000) annur-afgoni  (1000)       18 2024-05-23 07:15:08.000000 onepiece_classifier-0.0.2/src/onepiece_classifier.egg-info/top_level.txt
+drwxrwxr-x   0 annur-afgoni  (1000) annur-afgoni  (1000)        0 2024-05-23 07:15:08.908372 onepiece_classifier-0.0.2/src/onepiece_classify/
+-rw-rw-r--   0 annur-afgoni  (1000) annur-afgoni  (1000)        0 2024-05-16 06:56:44.000000 onepiece_classifier-0.0.2/src/onepiece_classify/__init__.py
+drwxrwxr-x   0 annur-afgoni  (1000) annur-afgoni  (1000)        0 2024-05-23 07:15:08.909372 onepiece_classifier-0.0.2/src/onepiece_classify/data/
+-rw-rw-r--   0 annur-afgoni  (1000) annur-afgoni  (1000)       26 2024-05-16 08:43:40.000000 onepiece_classifier-0.0.2/src/onepiece_classify/data/__init__.py
+-rw-rw-r--   0 annur-afgoni  (1000) annur-afgoni  (1000)     2126 2024-05-16 08:43:40.000000 onepiece_classifier-0.0.2/src/onepiece_classify/data/setup_data.py
+drwxrwxr-x   0 annur-afgoni  (1000) annur-afgoni  (1000)        0 2024-05-23 07:15:08.909372 onepiece_classifier-0.0.2/src/onepiece_classify/infer/
+-rw-rw-r--   0 annur-afgoni  (1000) annur-afgoni  (1000)       47 2024-05-16 08:43:40.000000 onepiece_classifier-0.0.2/src/onepiece_classify/infer/__init__.py
+-rw-rw-r--   0 annur-afgoni  (1000) annur-afgoni  (1000)      592 2024-05-16 08:43:40.000000 onepiece_classifier-0.0.2/src/onepiece_classify/infer/base.py
+-rw-rw-r--   0 annur-afgoni  (1000) annur-afgoni  (1000)     3563 2024-05-22 07:54:21.000000 onepiece_classifier-0.0.2/src/onepiece_classify/infer/recognition.py
+drwxrwxr-x   0 annur-afgoni  (1000) annur-afgoni  (1000)        0 2024-05-23 07:15:08.910372 onepiece_classifier-0.0.2/src/onepiece_classify/io/
+-rw-rw-r--   0 annur-afgoni  (1000) annur-afgoni  (1000)        0 2024-05-16 06:56:44.000000 onepiece_classifier-0.0.2/src/onepiece_classify/io/__init__.py
+drwxrwxr-x   0 annur-afgoni  (1000) annur-afgoni  (1000)        0 2024-05-23 07:15:08.911372 onepiece_classifier-0.0.2/src/onepiece_classify/models/
+-rw-rw-r--   0 annur-afgoni  (1000) annur-afgoni  (1000)       27 2024-05-16 08:43:40.000000 onepiece_classifier-0.0.2/src/onepiece_classify/models/__init__.py
+-rw-rw-r--   0 annur-afgoni  (1000) annur-afgoni  (1000)      786 2024-05-16 08:43:40.000000 onepiece_classifier-0.0.2/src/onepiece_classify/models/build_model.py
+drwxrwxr-x   0 annur-afgoni  (1000) annur-afgoni  (1000)        0 2024-05-23 07:15:08.911372 onepiece_classifier-0.0.2/src/onepiece_classify/trainer/
+-rw-rw-r--   0 annur-afgoni  (1000) annur-afgoni  (1000)       23 2024-05-16 08:43:40.000000 onepiece_classifier-0.0.2/src/onepiece_classify/trainer/__init__.py
+-rw-rw-r--   0 annur-afgoni  (1000) annur-afgoni  (1000)     4781 2024-05-16 08:43:40.000000 onepiece_classifier-0.0.2/src/onepiece_classify/trainer/trainer.py
+drwxrwxr-x   0 annur-afgoni  (1000) annur-afgoni  (1000)        0 2024-05-23 07:15:08.912371 onepiece_classifier-0.0.2/src/onepiece_classify/transforms/
+-rw-rw-r--   0 annur-afgoni  (1000) annur-afgoni  (1000)       21 2024-05-16 08:43:40.000000 onepiece_classifier-0.0.2/src/onepiece_classify/transforms/__init__.py
+-rw-rw-r--   0 annur-afgoni  (1000) annur-afgoni  (1000)     1095 2024-05-16 08:43:40.000000 onepiece_classifier-0.0.2/src/onepiece_classify/transforms/trans.py
+drwxrwxr-x   0 annur-afgoni  (1000) annur-afgoni  (1000)        0 2024-05-23 07:15:08.912371 onepiece_classifier-0.0.2/src/onepiece_classify/utils/
+-rw-rw-r--   0 annur-afgoni  (1000) annur-afgoni  (1000)       25 2024-05-22 04:34:21.000000 onepiece_classifier-0.0.2/src/onepiece_classify/utils/__init__.py
+-rw-rw-r--   0 annur-afgoni  (1000) annur-afgoni  (1000)      380 2024-05-22 07:58:06.000000 onepiece_classifier-0.0.2/src/onepiece_classify/utils/downloader.py
```

### Comparing `onepiece_classifier-0.0.1/LICENSE` & `onepiece_classifier-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `onepiece_classifier-0.0.1/PKG-INFO` & `onepiece_classifier-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onepiece_classifier
-Version: 0.0.1
+Version: 0.0.2
 Summary: package to predict onepiece image character
 Home-page: https://github.com/lombokai/onepiece-classifier.git
 Author: annur afgoni
 Author-email: afgoniannur@gmail.com
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `onepiece_classifier-0.0.1/README.md` & `onepiece_classifier-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `onepiece_classifier-0.0.1/setup.cfg` & `onepiece_classifier-0.0.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = onepiece_classifier
-version = 0.0.1
+version = 0.0.2
 author = annur afgoni
 author_email = afgoniannur@gmail.com
 description = package to predict onepiece image character
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/lombokai/onepiece-classifier.git
```

### Comparing `onepiece_classifier-0.0.1/src/onepiece_classifier.egg-info/PKG-INFO` & `onepiece_classifier-0.0.2/src/onepiece_classifier.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onepiece_classifier
-Version: 0.0.1
+Version: 0.0.2
 Summary: package to predict onepiece image character
 Home-page: https://github.com/lombokai/onepiece-classifier.git
 Author: annur afgoni
 Author-email: afgoniannur@gmail.com
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `onepiece_classifier-0.0.1/src/onepiece_classifier.egg-info/SOURCES.txt` & `onepiece_classifier-0.0.2/src/onepiece_classifier.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `onepiece_classifier-0.0.1/src/onepiece_classify/data/setup_data.py` & `onepiece_classifier-0.0.2/src/onepiece_classify/data/setup_data.py`

 * *Files identical despite different names*

### Comparing `onepiece_classifier-0.0.1/src/onepiece_classify/infer/base.py` & `onepiece_classifier-0.0.2/src/onepiece_classify/infer/base.py`

 * *Files identical despite different names*

### Comparing `onepiece_classifier-0.0.1/src/onepiece_classify/infer/recognition.py` & `onepiece_classifier-0.0.2/src/onepiece_classify/infer/recognition.py`

 * *Files identical despite different names*

### Comparing `onepiece_classifier-0.0.1/src/onepiece_classify/models/build_model.py` & `onepiece_classifier-0.0.2/src/onepiece_classify/models/build_model.py`

 * *Files identical despite different names*

### Comparing `onepiece_classifier-0.0.1/src/onepiece_classify/trainer/trainer.py` & `onepiece_classifier-0.0.2/src/onepiece_classify/trainer/trainer.py`

 * *Files identical despite different names*

### Comparing `onepiece_classifier-0.0.1/src/onepiece_classify/transforms/trans.py` & `onepiece_classifier-0.0.2/src/onepiece_classify/transforms/trans.py`

 * *Files identical despite different names*

