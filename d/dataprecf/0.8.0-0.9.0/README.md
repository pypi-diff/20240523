# Comparing `tmp/dataprecf-0.8.0.tar.gz` & `tmp/dataprecf-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataprecf-0.8.0.tar", last modified: Thu May 23 16:49:43 2024, max compression
+gzip compressed data, was "dataprecf-0.9.0.tar", last modified: Thu May 23 16:56:30 2024, max compression
```

## Comparing `dataprecf-0.8.0.tar` & `dataprecf-0.9.0.tar`

### file list

```diff
@@ -1,12 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 16:49:43.879874 dataprecf-0.8.0/
--rw-rw-rw-   0        0        0     4325 2024-05-23 16:49:43.877884 dataprecf-0.8.0/PKG-INFO
--rw-rw-rw-   0        0        0     3777 2024-05-23 16:40:21.000000 dataprecf-0.8.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-23 16:49:43.846233 dataprecf-0.8.0/dataprecf/
-drwxrwxrwx   0        0        0        0 2024-05-23 16:49:43.875764 dataprecf-0.8.0/dataprecf/dataprecf.egg-info/
--rw-rw-rw-   0        0        0     4325 2024-05-23 16:49:43.000000 dataprecf-0.8.0/dataprecf/dataprecf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      242 2024-05-23 16:49:43.000000 dataprecf-0.8.0/dataprecf/dataprecf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 16:49:43.000000 dataprecf-0.8.0/dataprecf/dataprecf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2024-05-23 16:49:43.000000 dataprecf-0.8.0/dataprecf/dataprecf.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 16:49:43.000000 dataprecf-0.8.0/dataprecf/dataprecf.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      756 2024-05-23 16:49:43.884057 dataprecf-0.8.0/setup.cfg
--rw-rw-rw-   0        0        0      561 2024-05-23 16:48:28.000000 dataprecf-0.8.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 16:56:30.311652 dataprecf-0.9.0/
+-rw-rw-rw-   0        0        0       53 2024-05-23 16:54:10.000000 dataprecf-0.9.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     4325 2024-05-23 16:56:30.310420 dataprecf-0.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3777 2024-05-23 16:40:21.000000 dataprecf-0.9.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-23 16:56:30.273623 dataprecf-0.9.0/dataprecf/
+-rw-rw-rw-   0        0        0      517 2024-05-23 16:16:45.000000 dataprecf-0.9.0/dataprecf/__init__.py
+-rw-rw-rw-   0        0        0      696 2024-05-21 11:42:32.000000 dataprecf-0.9.0/dataprecf/categorical_encoder.py
+-rw-rw-rw-   0        0        0      339 2024-05-21 11:42:35.000000 dataprecf-0.9.0/dataprecf/data_type_converter.py
+drwxrwxrwx   0        0        0        0 2024-05-23 16:56:30.308331 dataprecf-0.9.0/dataprecf/dataprecf.egg-info/
+-rw-rw-rw-   0        0        0     4325 2024-05-23 16:56:30.000000 dataprecf-0.9.0/dataprecf/dataprecf.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      512 2024-05-23 16:56:30.000000 dataprecf-0.9.0/dataprecf/dataprecf.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 16:56:30.000000 dataprecf-0.9.0/dataprecf/dataprecf.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2024-05-23 16:56:30.000000 dataprecf-0.9.0/dataprecf/dataprecf.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 16:56:30.000000 dataprecf-0.9.0/dataprecf/dataprecf.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      418 2024-05-21 11:42:35.000000 dataprecf-0.9.0/dataprecf/datetime_handler.py
+-rw-rw-rw-   0        0        0      368 2024-05-21 13:05:57.000000 dataprecf-0.9.0/dataprecf/feature_engineer.py
+-rw-rw-rw-   0        0        0      608 2024-05-21 11:42:34.000000 dataprecf-0.9.0/dataprecf/missing_value_handler.py
+-rw-rw-rw-   0        0        0      437 2024-05-21 11:42:34.000000 dataprecf-0.9.0/dataprecf/outlier_handler.py
+-rw-rw-rw-   0        0        0      494 2024-05-21 11:42:34.000000 dataprecf-0.9.0/dataprecf/scaler.py
+-rw-rw-rw-   0        0        0      688 2024-05-21 11:42:33.000000 dataprecf-0.9.0/dataprecf/text_cleaner.py
+-rw-rw-rw-   0        0        0      756 2024-05-23 16:56:30.314713 dataprecf-0.9.0/setup.cfg
+-rw-rw-rw-   0        0        0      561 2024-05-23 16:56:16.000000 dataprecf-0.9.0/setup.py
```

### Comparing `dataprecf-0.8.0/PKG-INFO` & `dataprecf-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataprecf
-Version: 0.8.0
+Version: 0.9.0
 Summary: A data preprocessor for machine learning projects.
 Author: fatmanur caliskan, cihan yilmaz
 Author-email: fatmanur.caliskan@stu.fsm.edu.tr, cihan.yilmaz@stu.fsm.edu.tr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `dataprecf-0.8.0/README.md` & `dataprecf-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `dataprecf-0.8.0/dataprecf/dataprecf.egg-info/PKG-INFO` & `dataprecf-0.9.0/dataprecf/dataprecf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataprecf
-Version: 0.8.0
+Version: 0.9.0
 Summary: A data preprocessor for machine learning projects.
 Author: fatmanur caliskan, cihan yilmaz
 Author-email: fatmanur.caliskan@stu.fsm.edu.tr, cihan.yilmaz@stu.fsm.edu.tr
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `dataprecf-0.8.0/setup.cfg` & `dataprecf-0.9.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2064 6174 6170 7265 6366 0d0a 7665   = dataprecf..ve
-00000020: 7273 696f 6e20 3d20 302e 382e 300d 0a61  rsion = 0.8.0..a
+00000020: 7273 696f 6e20 3d20 302e 392e 300d 0a61  rsion = 0.9.0..a
 00000030: 7574 686f 7220 3d20 6661 746d 616e 7572  uthor = fatmanur
 00000040: 2063 616c 6973 6b61 6e2c 2063 6968 616e   caliskan, cihan
 00000050: 2079 696c 6d61 7a0d 0a61 7574 686f 725f   yilmaz..author_
 00000060: 656d 6169 6c20 3d20 6661 746d 616e 7572  email = fatmanur
 00000070: 2e63 616c 6973 6b61 6e40 7374 752e 6673  .caliskan@stu.fs
 00000080: 6d2e 6564 752e 7472 2c20 6369 6861 6e2e  m.edu.tr, cihan.
 00000090: 7969 6c6d 617a 4073 7475 2e66 736d 2e65  yilmaz@stu.fsm.e
```

### Comparing `dataprecf-0.8.0/setup.py` & `dataprecf-0.9.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='dataprecf',
-    version='0.8.0',
+    version='0.9.0',
     packages=find_packages(where='dataprecf'),
     install_requires=[
         'pandas',
         'numpy',
         'scikit-learn',
         'nltk',
     ],
```

