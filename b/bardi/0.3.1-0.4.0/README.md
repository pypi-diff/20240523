# Comparing `tmp/bardi-0.3.1.tar.gz` & `tmp/bardi-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bardi-0.3.1.tar", last modified: Mon Feb  5 17:48:37 2024, max compression
+gzip compressed data, was "bardi-0.4.0.tar", last modified: Thu May 23 13:09:51 2024, max compression
```

## Comparing `bardi-0.3.1.tar` & `bardi-0.4.0.tar`

### file list

```diff
@@ -1,38 +1,43 @@
-drwxr-xr-x   0 5ov      (789149836) ORNL\Domain Users (1551083765)        0 2024-02-05 17:48:37.234801 bardi-0.3.1/
--rw-r--r--   0 5ov      (789149836) ORNL\Domain Users (1551083765)     1072 2023-12-05 22:19:41.000000 bardi-0.3.1/LICENSE
--rw-r--r--   0 5ov      (789149836) ORNL\Domain Users (1551083765)    24124 2024-02-05 17:48:37.234579 bardi-0.3.1/PKG-INFO
--rwxr-xr-x   0 5ov      (789149836) ORNL\Domain Users (1551083765)    23455 2024-02-05 16:58:18.000000 bardi-0.3.1/README.md
-drwxr-xr-x   0 5ov      (789149836) ORNL\Domain Users (1551083765)        0 2024-02-05 17:48:37.230654 bardi-0.3.1/bardi/
--rwxr-xr-x   0 5ov      (789149836) ORNL\Domain Users (1551083765)        1 2023-12-13 18:49:40.000000 bardi-0.3.1/bardi/__init__.py
-drwxr-xr-x   0 5ov      (789149836) ORNL\Domain Users (1551083765)        0 2024-02-05 17:48:37.231669 bardi-0.3.1/bardi/data/
--rwxr-xr-x   0 5ov      (789149836) ORNL\Domain Users (1551083765)       63 2023-12-13 18:49:40.000000 bardi-0.3.1/bardi/data/__init__.py
--rwxr-xr-x   0 5ov      (789149836) ORNL\Domain Users (1551083765)    13989 2024-02-05 16:58:18.000000 bardi-0.3.1/bardi/data/data_handlers.py
-drwxr-xr-x   0 5ov      (789149836) ORNL\Domain Users (1551083765)        0 2024-02-05 17:48:37.231939 bardi-0.3.1/bardi/data/utils/
--rwxr-xr-x   0 5ov      (789149836) ORNL\Domain Users (1551083765)        0 2023-12-13 18:49:40.000000 bardi-0.3.1/bardi/data/utils/__init__.py
--rwxr-xr-x   0 5ov      (789149836) ORNL\Domain Users (1551083765)      825 2023-12-13 18:49:40.000000 bardi-0.3.1/bardi/data/utils/pyarrow_utils.py
-drwxr-xr-x   0 5ov      (789149836) ORNL\Domain Users (1551083765)        0 2024-02-05 17:48:37.233281 bardi-0.3.1/bardi/nlp_engineering/
--rwxr-xr-x   0 5ov      (789149836) ORNL\Domain Users (1551083765)      552 2023-12-13 18:49:40.000000 bardi-0.3.1/bardi/nlp_engineering/__init__.py
--rwxr-xr-x   0 5ov      (789149836) ORNL\Domain Users (1551083765)    12835 2024-02-05 16:58:18.000000 bardi-0.3.1/bardi/nlp_engineering/embedding_generator.py
--rwxr-xr-x   0 5ov      (789149836) ORNL\Domain Users (1551083765)     7718 2024-02-05 16:58:18.000000 bardi-0.3.1/bardi/nlp_engineering/label_processor.py
--rwxr-xr-x   0 5ov      (789149836) ORNL\Domain Users (1551083765)     5368 2024-02-05 16:58:18.000000 bardi-0.3.1/bardi/nlp_engineering/normalizer.py
--rwxr-xr-x   0 5ov      (789149836) ORNL\Domain Users (1551083765)     9846 2024-02-05 16:58:18.000000 bardi-0.3.1/bardi/nlp_engineering/post_processor.py
--rwxr-xr-x   0 5ov      (789149836) ORNL\Domain Users (1551083765)     3566 2024-02-05 16:58:18.000000 bardi-0.3.1/bardi/nlp_engineering/pre_tokenizer.py
-drwxr-xr-x   0 5ov      (789149836) ORNL\Domain Users (1551083765)        0 2024-02-05 17:48:37.233904 bardi-0.3.1/bardi/nlp_engineering/regex_library/
--rwxr-xr-x   0 5ov      (789149836) ORNL\Domain Users (1551083765)       67 2023-12-13 18:49:40.000000 bardi-0.3.1/bardi/nlp_engineering/regex_library/__init__.py
--rwxr-xr-x   0 5ov      (789149836) ORNL\Domain Users (1551083765)    13542 2024-02-05 16:58:18.000000 bardi-0.3.1/bardi/nlp_engineering/regex_library/pathology_report.py
--rwxr-xr-x   0 5ov      (789149836) ORNL\Domain Users (1551083765)    18349 2024-02-05 16:58:18.000000 bardi-0.3.1/bardi/nlp_engineering/regex_library/regex_lib.py
--rwxr-xr-x   0 5ov      (789149836) ORNL\Domain Users (1551083765)     1115 2024-02-05 16:58:18.000000 bardi-0.3.1/bardi/nlp_engineering/regex_library/regex_set.py
--rwxr-xr-x   0 5ov      (789149836) ORNL\Domain Users (1551083765)    14878 2024-02-05 16:58:18.000000 bardi-0.3.1/bardi/nlp_engineering/splitter.py
-drwxr-xr-x   0 5ov      (789149836) ORNL\Domain Users (1551083765)        0 2024-02-05 17:48:37.234151 bardi-0.3.1/bardi/nlp_engineering/utils/
--rwxr-xr-x   0 5ov      (789149836) ORNL\Domain Users (1551083765)        0 2023-12-13 18:49:40.000000 bardi-0.3.1/bardi/nlp_engineering/utils/__init__.py
--rwxr-xr-x   0 5ov      (789149836) ORNL\Domain Users (1551083765)     4048 2023-12-13 18:49:40.000000 bardi-0.3.1/bardi/nlp_engineering/utils/validations.py
--rwxr-xr-x   0 5ov      (789149836) ORNL\Domain Users (1551083765)    13534 2024-02-05 16:58:18.000000 bardi-0.3.1/bardi/pipeline.py
-drwxr-xr-x   0 5ov      (789149836) ORNL\Domain Users (1551083765)        0 2024-02-05 17:48:37.234330 bardi-0.3.1/bardi.egg-info/
--rw-r--r--   0 5ov      (789149836) ORNL\Domain Users (1551083765)    24124 2024-02-05 17:48:37.000000 bardi-0.3.1/bardi.egg-info/PKG-INFO
--rw-r--r--   0 5ov      (789149836) ORNL\Domain Users (1551083765)      889 2024-02-05 17:48:37.000000 bardi-0.3.1/bardi.egg-info/SOURCES.txt
--rw-r--r--   0 5ov      (789149836) ORNL\Domain Users (1551083765)        1 2024-02-05 17:48:37.000000 bardi-0.3.1/bardi.egg-info/dependency_links.txt
--rw-r--r--   0 5ov      (789149836) ORNL\Domain Users (1551083765)       87 2024-02-05 17:48:37.000000 bardi-0.3.1/bardi.egg-info/requires.txt
--rw-r--r--   0 5ov      (789149836) ORNL\Domain Users (1551083765)        6 2024-02-05 17:48:37.000000 bardi-0.3.1/bardi.egg-info/top_level.txt
--rwxr-xr-x   0 5ov      (789149836) ORNL\Domain Users (1551083765)      778 2024-02-05 17:46:50.000000 bardi-0.3.1/pyproject.toml
--rw-r--r--   0 5ov      (789149836) ORNL\Domain Users (1551083765)       38 2024-02-05 17:48:37.234844 bardi-0.3.1/setup.cfg
--rwxr-xr-x   0 5ov      (789149836) ORNL\Domain Users (1551083765)      379 2024-02-05 17:46:50.000000 bardi-0.3.1/setup.py
+drwxr-xr-x   0 5ov      (789149836) ORNL\Domain Users (1551083765)        0 2024-05-23 13:09:51.322547 bardi-0.4.0/
+-rwxr-xr-x   0 5ov      (789149836) ORNL\Domain Users (1551083765)     1072 2024-05-23 12:52:36.000000 bardi-0.4.0/LICENSE
+-rw-r--r--   0 5ov      (789149836) ORNL\Domain Users (1551083765)    24238 2024-05-23 13:09:51.322304 bardi-0.4.0/PKG-INFO
+-rwxr-xr-x   0 5ov      (789149836) ORNL\Domain Users (1551083765)    23467 2024-05-23 12:52:36.000000 bardi-0.4.0/README.md
+drwxr-xr-x   0 5ov      (789149836) ORNL\Domain Users (1551083765)        0 2024-05-23 13:09:51.316341 bardi-0.4.0/bardi/
+-rwxr-xr-x   0 5ov      (789149836) ORNL\Domain Users (1551083765)       90 2024-05-23 12:52:36.000000 bardi-0.4.0/bardi/__init__.py
+drwxr-xr-x   0 5ov      (789149836) ORNL\Domain Users (1551083765)        0 2024-05-23 13:09:51.317469 bardi-0.4.0/bardi/data/
+-rwxr-xr-x   0 5ov      (789149836) ORNL\Domain Users (1551083765)      276 2024-05-23 12:52:36.000000 bardi-0.4.0/bardi/data/__init__.py
+-rwxr-xr-x   0 5ov      (789149836) ORNL\Domain Users (1551083765)    13926 2024-05-23 12:52:36.000000 bardi-0.4.0/bardi/data/data_handlers.py
+drwxr-xr-x   0 5ov      (789149836) ORNL\Domain Users (1551083765)        0 2024-05-23 13:09:51.317802 bardi-0.4.0/bardi/data/utils/
+-rwxr-xr-x   0 5ov      (789149836) ORNL\Domain Users (1551083765)        0 2023-12-13 18:49:40.000000 bardi-0.4.0/bardi/data/utils/__init__.py
+-rwxr-xr-x   0 5ov      (789149836) ORNL\Domain Users (1551083765)      825 2023-12-13 18:49:40.000000 bardi-0.4.0/bardi/data/utils/pyarrow_utils.py
+drwxr-xr-x   0 5ov      (789149836) ORNL\Domain Users (1551083765)        0 2024-05-23 13:09:51.319944 bardi-0.4.0/bardi/nlp_engineering/
+-rwxr-xr-x   0 5ov      (789149836) ORNL\Domain Users (1551083765)     1029 2024-05-23 12:52:36.000000 bardi-0.4.0/bardi/nlp_engineering/__init__.py
+-rwxr-xr-x   0 5ov      (789149836) ORNL\Domain Users (1551083765)    12835 2024-02-05 16:58:18.000000 bardi-0.4.0/bardi/nlp_engineering/embedding_generator.py
+-rwxr-xr-x   0 5ov      (789149836) ORNL\Domain Users (1551083765)     8497 2024-05-23 12:52:36.000000 bardi-0.4.0/bardi/nlp_engineering/label_processor.py
+-rwxr-xr-x   0 5ov      (789149836) ORNL\Domain Users (1551083765)     5930 2024-05-23 12:52:36.000000 bardi-0.4.0/bardi/nlp_engineering/normalizer.py
+-rwxr-xr-x   0 5ov      (789149836) ORNL\Domain Users (1551083765)     4277 2024-05-23 12:52:36.000000 bardi-0.4.0/bardi/nlp_engineering/pre_tokenizer.py
+drwxr-xr-x   0 5ov      (789149836) ORNL\Domain Users (1551083765)        0 2024-05-23 13:09:51.320968 bardi-0.4.0/bardi/nlp_engineering/regex_library/
+-rwxr-xr-x   0 5ov      (789149836) ORNL\Domain Users (1551083765)      230 2024-05-23 12:52:36.000000 bardi-0.4.0/bardi/nlp_engineering/regex_library/__init__.py
+-rwxr-xr-x   0 5ov      (789149836) ORNL\Domain Users (1551083765)    13542 2024-02-05 16:58:18.000000 bardi-0.4.0/bardi/nlp_engineering/regex_library/pathology_report.py
+-rwxr-xr-x   0 5ov      (789149836) ORNL\Domain Users (1551083765)    18349 2024-02-05 16:58:18.000000 bardi-0.4.0/bardi/nlp_engineering/regex_library/regex_lib.py
+-rwxr-xr-x   0 5ov      (789149836) ORNL\Domain Users (1551083765)     1919 2024-05-23 12:52:36.000000 bardi-0.4.0/bardi/nlp_engineering/regex_library/regex_set.py
+-rwxr-xr-x   0 5ov      (789149836) ORNL\Domain Users (1551083765)    15110 2024-05-23 12:52:36.000000 bardi-0.4.0/bardi/nlp_engineering/splitter.py
+-rwxr-xr-x   0 5ov      (789149836) ORNL\Domain Users (1551083765)    11774 2024-05-23 12:52:36.000000 bardi-0.4.0/bardi/nlp_engineering/tokenizer_encoder.py
+-rwxr-xr-x   0 5ov      (789149836) ORNL\Domain Users (1551083765)     9659 2024-05-23 12:52:36.000000 bardi-0.4.0/bardi/nlp_engineering/tokenizer_trainer.py
+drwxr-xr-x   0 5ov      (789149836) ORNL\Domain Users (1551083765)        0 2024-05-23 13:09:51.321668 bardi-0.4.0/bardi/nlp_engineering/utils/
+-rwxr-xr-x   0 5ov      (789149836) ORNL\Domain Users (1551083765)        0 2023-12-13 18:49:40.000000 bardi-0.4.0/bardi/nlp_engineering/utils/__init__.py
+-rwxr-xr-x   0 5ov      (789149836) ORNL\Domain Users (1551083765)     1818 2024-05-23 12:52:36.000000 bardi-0.4.0/bardi/nlp_engineering/utils/helper_utils.py
+-rwxr-xr-x   0 5ov      (789149836) ORNL\Domain Users (1551083765)      953 2024-05-23 12:52:36.000000 bardi-0.4.0/bardi/nlp_engineering/utils/polars_utils.py
+-rwxr-xr-x   0 5ov      (789149836) ORNL\Domain Users (1551083765)     6621 2024-05-23 12:52:36.000000 bardi-0.4.0/bardi/nlp_engineering/utils/tokenizers_lib.py
+-rwxr-xr-x   0 5ov      (789149836) ORNL\Domain Users (1551083765)     4048 2023-12-13 18:49:40.000000 bardi-0.4.0/bardi/nlp_engineering/utils/validations.py
+-rwxr-xr-x   0 5ov      (789149836) ORNL\Domain Users (1551083765)    10697 2024-05-23 12:52:36.000000 bardi-0.4.0/bardi/nlp_engineering/vocab_encoder.py
+-rwxr-xr-x   0 5ov      (789149836) ORNL\Domain Users (1551083765)    13223 2024-05-23 12:52:36.000000 bardi-0.4.0/bardi/pipeline.py
+drwxr-xr-x   0 5ov      (789149836) ORNL\Domain Users (1551083765)        0 2024-05-23 13:09:51.322013 bardi-0.4.0/bardi.egg-info/
+-rw-r--r--   0 5ov      (789149836) ORNL\Domain Users (1551083765)    24238 2024-05-23 13:09:51.000000 bardi-0.4.0/bardi.egg-info/PKG-INFO
+-rw-r--r--   0 5ov      (789149836) ORNL\Domain Users (1551083765)     1108 2024-05-23 13:09:51.000000 bardi-0.4.0/bardi.egg-info/SOURCES.txt
+-rw-r--r--   0 5ov      (789149836) ORNL\Domain Users (1551083765)        1 2024-05-23 13:09:51.000000 bardi-0.4.0/bardi.egg-info/dependency_links.txt
+-rw-r--r--   0 5ov      (789149836) ORNL\Domain Users (1551083765)      144 2024-05-23 13:09:51.000000 bardi-0.4.0/bardi.egg-info/requires.txt
+-rw-r--r--   0 5ov      (789149836) ORNL\Domain Users (1551083765)        6 2024-05-23 13:09:51.000000 bardi-0.4.0/bardi.egg-info/top_level.txt
+-rwxr-xr-x   0 5ov      (789149836) ORNL\Domain Users (1551083765)      891 2024-05-23 12:53:01.000000 bardi-0.4.0/pyproject.toml
+-rw-r--r--   0 5ov      (789149836) ORNL\Domain Users (1551083765)       38 2024-05-23 13:09:51.322597 bardi-0.4.0/setup.cfg
+-rwxr-xr-x   0 5ov      (789149836) ORNL\Domain Users (1551083765)      379 2024-05-23 12:52:36.000000 bardi-0.4.0/setup.py
```

### Comparing `bardi-0.3.1/LICENSE` & `bardi-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bardi-0.3.1/PKG-INFO` & `bardi-0.4.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,35 +1,25 @@
-Metadata-Version: 2.1
-Name: bardi
-Version: 0.3.1
-Summary: A flexible machine learning data pre-processing pipeline framework.
-Author: Oak Ridge National Laboratory
-Project-URL: Homepage, https://github.com/DOE-NCI-MOSSAIC/bardi
-Project-URL: Documentation, https://doe-nci-mossaic.github.io/bardi/
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.8.0
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: duckdb>=0.8.0
-Requires-Dist: gensim>=4.1.2
-Requires-Dist: numpy>=1.21.5
-Requires-Dist: pandas>=1.4.4
-Requires-Dist: polars>=0.19.8
-Requires-Dist: pyarrow>=14.0.1
-
 
 # BARDI (Batch-processing Abstraction for Raw Data Integration)
 BARDI is a specialized framework engineered to facilitate the development of reproducible data pre-processing pipelines within machine learning workflows. 
 
 It emphasizes the following key aspects:
-    - Abstraction: By transforming common data pre-processing operations into modular components, Bardi simplifies both the development and upkeep of complex data pipelines.
-    - Efficiency: Utilizing Apache Arrow's columnar memory model for data storage and Polars for computations, Bardi enhances processing speed through multithreading, optimizing the use of available CPU resources.
-    - Modularity: Bardi's design is based on a component-driven architecture, offering users the flexibility to incorporate specific modules tailored to their unique requirements. These modules are crafted to operate seamlessly both as standalone units and within the context of a comprehensive pipeline.
-    - Extensibility: Designed with future growth in mind, Bardi allows for the straightforward addition of new custom steps, thereby broadening its functionality to encompass unaddressed demands and evolving data processing needs.
+
+ * Abstraction: By transforming common data pre-processing operations into modular components, Bardi simplifies both the
+    development and upkeep of complex data pipelines.
+
+ * Efficiency: Utilizing Apache Arrow's columnar memory model for data storage and Polars for computations, Bardi enhances
+    processing speed through multithreading, optimizing the use of available CPU resources.
+
+ * Modularity: Bardi's design is based on a component-driven architecture, offering users the flexibility to incorporate
+    specific modules tailored to their unique requirements. These modules are crafted to operate seamlessly both as standalone
+    units and within the context of a comprehensive pipeline.
+
+ * Extensibility: Designed with future growth in mind, Bardi allows for the straightforward addition of new custom steps,
+    thereby broadening its functionality to encompass unaddressed demands and evolving data processing needs.
 
 Installation
 ============
 
 ``pip install bardi``
 
 _currently not supported on Windows_
```

### Comparing `bardi-0.3.1/README.md` & `bardi-0.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,47 @@
+Metadata-Version: 2.1
+Name: bardi
+Version: 0.4.0
+Summary: A flexible machine learning data pre-processing pipeline framework.
+Author: Oak Ridge National Laboratory
+Project-URL: Homepage, https://github.com/DOE-NCI-MOSSAIC/bardi
+Project-URL: Documentation, https://doe-nci-mossaic.github.io/bardi/
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: License :: OSI Approved :: MIT License
+Requires-Python: >=3.8.0
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: duckdb==0.8.0
+Requires-Dist: gensim>=4.1.2
+Requires-Dist: numpy>=1.21.5
+Requires-Dist: pandas>=1.4.4
+Requires-Dist: polars>=0.19.8
+Requires-Dist: pyarrow>=14.0.1
+Requires-Dist: tokenizers>=0.13.3
+Requires-Dist: transformers>=4.29.2
+Requires-Dist: datasets>=2.12.0
+
 
 # BARDI (Batch-processing Abstraction for Raw Data Integration)
 BARDI is a specialized framework engineered to facilitate the development of reproducible data pre-processing pipelines within machine learning workflows. 
 
 It emphasizes the following key aspects:
-    - Abstraction: By transforming common data pre-processing operations into modular components, Bardi simplifies both the development and upkeep of complex data pipelines.
-    - Efficiency: Utilizing Apache Arrow's columnar memory model for data storage and Polars for computations, Bardi enhances processing speed through multithreading, optimizing the use of available CPU resources.
-    - Modularity: Bardi's design is based on a component-driven architecture, offering users the flexibility to incorporate specific modules tailored to their unique requirements. These modules are crafted to operate seamlessly both as standalone units and within the context of a comprehensive pipeline.
-    - Extensibility: Designed with future growth in mind, Bardi allows for the straightforward addition of new custom steps, thereby broadening its functionality to encompass unaddressed demands and evolving data processing needs.
+
+ * Abstraction: By transforming common data pre-processing operations into modular components, Bardi simplifies both the
+    development and upkeep of complex data pipelines.
+
+ * Efficiency: Utilizing Apache Arrow's columnar memory model for data storage and Polars for computations, Bardi enhances
+    processing speed through multithreading, optimizing the use of available CPU resources.
+
+ * Modularity: Bardi's design is based on a component-driven architecture, offering users the flexibility to incorporate
+    specific modules tailored to their unique requirements. These modules are crafted to operate seamlessly both as standalone
+    units and within the context of a comprehensive pipeline.
+
+ * Extensibility: Designed with future growth in mind, Bardi allows for the straightforward addition of new custom steps,
+    thereby broadening its functionality to encompass unaddressed demands and evolving data processing needs.
 
 Installation
 ============
 
 ``pip install bardi``
 
 _currently not supported on Windows_
```

### Comparing `bardi-0.3.1/bardi/data/data_handlers.py` & `bardi-0.4.0/bardi/data/data_handlers.py`

 * *Files 0% similar despite different names*

```diff
@@ -122,17 +122,15 @@
         dataset_obj.origin_row_count = row_count
         dataset_obj.origin_file_path = source
         dataset_obj.origin_format = format
 
         if min_batches:
             # If a min_batches is specified, data from the file(s) are split
             # into a list of smaller PyArrow Tables
-            tables = chunk_pyarrow_table(
-                data=table, row_count=row_count, min_batches=min_batches
-            )
+            tables = chunk_pyarrow_table(data=table, row_count=row_count, min_batches=min_batches)
 
             # Setting the bardi Dataset object's data references to the list
             # of PyArrow Tables
             dataset_obj.data = tables
 
         else:
             # If min_batches is not specified, all of the data is returned in
@@ -179,17 +177,15 @@
     dataset_obj.origin_query = query
     dataset_obj.origin_format = "duckdb"
     dataset_obj.origin_row_count = row_count
 
     if min_batches:
         # If a min_batches is specified, data from the file(s) are split into a
         # list of smaller PyArrow Tables
-        tables = chunk_pyarrow_table(
-            data=table, row_count=row_count, min_batches=min_batches
-        )
+        tables = chunk_pyarrow_table(data=table, row_count=row_count, min_batches=min_batches)
 
         # Setting the bardi Dataset object's data references to the list of
         # PyArrow Tables
         dataset_obj.data = tables
 
     else:
         # If min_batches is not specified, all of the data is returned in a
@@ -235,17 +231,15 @@
     dataset_obj = Dataset()
     dataset_obj.origin_format = "pandas"
     dataset_obj.origin_row_count = row_count
 
     if min_batches:
         # If a min_batches is specified, data from the file(s) are split into
         # a list of smaller PyArrow Tables
-        tables = chunk_pyarrow_table(
-            data=table, row_count=row_count, min_batches=min_batches
-        )
+        tables = chunk_pyarrow_table(data=table, row_count=row_count, min_batches=min_batches)
 
         # Setting the bardi Dataset object's data references to the list of
         # PyArrow Tables
         dataset_obj.data = tables
 
     else:
         # If min_batches is not specified, all of the data is returned in a
@@ -284,17 +278,15 @@
     dataset_obj = Dataset()
     dataset_obj.origin_format = "pyarrow"
     dataset_obj.origin_row_count = row_count
 
     if min_batches:
         # If a min_batches is specified, data from the file(s) are split into a
         # list of smaller PyArrow Tables
-        tables = chunk_pyarrow_table(
-            data=table, row_count=row_count, min_batches=min_batches
-        )
+        tables = chunk_pyarrow_table(data=table, row_count=row_count, min_batches=min_batches)
 
         # Setting the bardi Dataset object's data references to the list of
         # PyArrow Tables
         dataset_obj.data = tables
 
     else:
         # If min_batches is not specified, all of the data is returned in a
@@ -350,40 +342,40 @@
 
 
 # ======= Writers ========
 
 
 def to_pandas(table: pa.Table) -> pd.DataFrame:
     """Return data as a pandas DataFrame
-    
+
     Parameters
     ----------
 
     table : PyArrow.Table
         Table of data you want to convert to a Pandas DataFrame
-    
+
     Returns
     -------
 
     pandas.DataFrame
         The same data as the input table, converted into a DataFrame
     """
     df = table.to_pandas()
     return df
 
 
 def to_polars(table: pa.Table) -> pl.DataFrame:
     """Return data as a polars DataFrame
-    
+
     Parameters
     ----------
 
     table : PyArrow.Table
         Table of data you want to convert to a Pandas DataFrame
-    
+
     Returns
     -------
 
     polars.DataFrame
         The same data as the input table, converted into a DataFrame
     """
     df = pl.from_arrow(table)
@@ -426,19 +418,19 @@
             feather.write_feather(data, path, *args, **kwargs)
         elif format == "csv":
             # Convert list columns to strings
             csv_df = pl.from_arrow(data)
             schema = csv_df.schema
             csv_df = csv_df.with_columns(
                 [
-                    pl.format(
-                        "[{}]", pl.col(field).cast(pl.List(pl.Utf8)).list.join(", ")
-                    ).alias(field)
+                    pl.format("[{}]", pl.col(field).cast(pl.List(pl.Utf8)).list.join(", ")).alias(
+                        field
+                    )
                     for field in schema.keys()
-                    if schema[field] == pl.List()
+                    if (schema[field] == pl.List(pl.Int64)) or (schema[field] == pl.List(pl.Utf8))
                 ]
             )
             data = csv_df.to_arrow()
             csv.write_csv(data, path, *args, **kwargs)
         elif format == "json":
             json_object = json.dumps(data, indent=4)
             with open(path, "w") as f:
```

### Comparing `bardi-0.3.1/bardi/data/utils/pyarrow_utils.py` & `bardi-0.4.0/bardi/data/utils/pyarrow_utils.py`

 * *Files identical despite different names*

### Comparing `bardi-0.3.1/bardi/nlp_engineering/embedding_generator.py` & `bardi-0.4.0/bardi/nlp_engineering/embedding_generator.py`

 * *Files identical despite different names*

### Comparing `bardi-0.3.1/bardi/nlp_engineering/label_processor.py` & `bardi-0.4.0/bardi/nlp_engineering/label_processor.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from abc import abstractmethod
 from typing import List, Tuple, TypedDict, Union, Optional
 
 import polars as pl
 import pyarrow as pa
 
 from bardi.data import data_handlers
+from bardi.nlp_engineering.utils.polars_utils import retain_inputs
 from bardi.nlp_engineering.utils.validations import validate_pyarrow_table
 from bardi.pipeline import DataWriteConfig, Step
 
 
 class LabelProcessorArtifactsWriteConfig(TypedDict):
     """Indicates the keys and data types expected in an
     artifacts write config dict for the label processor
@@ -37,24 +38,32 @@
     fields : Union[str, List[str]]
         The name of a label column of which the values
         are used to generate a standardized mapping and
         then that mapping is applied to the column.
     method : str
         Currently only a default 'unique' method is
         supported which maps each unique value in the column to an id.
+    retain_input_fields : Optional[bool]
+        If True, will retain the original contents of the fields specified in
+        `fields` under the new names of: `labelprocessor__<field>`
     """
 
-    def __init__(self, fields: Union[str, List[str]], method: str = "unique"):
-        """Constructor method
-        """
+    def __init__(
+        self,
+        fields: Union[str, List[str]],
+        method: str = "unique",
+        retain_input_fields: bool = False,
+    ):
+        """Constructor method"""
         self.fields = fields
         if isinstance(fields, str):
             self.fields = [fields]
         else:
             self.fields = fields
+        self.retain_input_fields = retain_input_fields
         self.method = method
         self.mapping = {}
         self.id_to_label = {}
         self._data_write_config: DataWriteConfig = {
             "data_format": "parquet",
             "data_format_args": {"compression": "snappy", "use_dictionary": False},
         }
@@ -72,16 +81,15 @@
         if data_config:
             self._data_write_config = data_config
         if artifacts_config:
             self._artifacts_write_config = artifacts_config
 
     @abstractmethod
     def run(self):
-        """Abstract method
-        """
+        """Abstract method"""
         pass
 
 
 class CPULabelProcessor(LabelProcessor):
     """The label processor creates and maps a label vocab.
 
     Note
@@ -89,28 +97,32 @@
 
     This implementation of the LabelProcessor is specific for CPU computation.
 
     Attributes
     ----------
 
     fields : Union[str, List[str]]
-        The name(s) of label column(s) of which the values 
-        are used to generate a standardized mapping and then that mapping is applied to the column(s).
-    method : str 
-        Currently only a default 'unique' method is supported which maps each unique value in the column to an id.
+        The name(s) of label column(s) of which the values
+        are used to generate a standardized mapping and then that mapping is applied to
+        the column(s).
+    method : str
+        Currently only a default 'unique' method is supported which maps each unique value
+        in the column to an id.
     mapping : dict
         Mapping dict of the form {label: id} used to convert labels in the column to ids.
     id_to_label : dict
-        The reverse of mapping. Of the form {id: label} used downstream to map 
+        The reverse of mapping. Of the form {id: label} used downstream to map
         the ids back to the original label values.
+    retain_input_fields : Optional[bool]
+        If True, will retain the original contents of the fields specified in
+        `fields` under the new names of: `labelprocessor__<field>`
     """
 
     def __init__(self, *args, **kwargs):
-        """Constructor method
-        """
+        """Constructor method"""
         super().__init__(*args, **kwargs)
 
     def run(self, data: pa.Table, artifacts: Optional[dict] = None) -> Tuple[pa.Table, dict]:
         """Run a label processor using CPU computation
 
         Parameters
         ----------
@@ -144,28 +156,33 @@
 
         # Confirm that the method is passed a PyArrow Table
         produced_artifacts = {}
         for field in self.fields:
             if self.method == "unique":
                 try:
                     # Get the unique labels
-                    vals = (
-                        pl.from_arrow(data).get_column(field).unique().sort()
-                    ).to_list()
+                    vals = (pl.from_arrow(data).get_column(field).unique().sort()).to_list()
 
                     # Create a mapping for the labels
                     field_mapping = {label: id for id, label in enumerate(vals)}
                     # id_to_label is flipped vs what is needed for mapping
                     field_id_to_label = {
                         str(id): str(label) for label, id in field_mapping.items()
                     }
                     self.id_to_label[field] = field_id_to_label
 
-                    df = pl.from_arrow(data).with_columns(
-                        pl.col(field).map_dict(field_mapping, default=None)
+                    df = (
+                        pl.from_arrow(data)
+                        .pipe(
+                            retain_inputs,
+                            self.retain_input_fields,
+                            [field],
+                            self.__class__.__name__,
+                        )
+                        .with_columns(pl.col(field).map_dict(field_mapping, default=None))
                     )
 
                 except Exception as e:
                     print(
                         f"An error occured: {e} "
                         "Processing without creating the label "
                         f"mapping for {field}"
```

### Comparing `bardi-0.3.1/bardi/nlp_engineering/normalizer.py` & `bardi-0.4.0/bardi/nlp_engineering/normalizer.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,91 +3,100 @@
 from abc import abstractmethod
 from typing import List, Tuple, Union, Optional
 
 import polars as pl
 import pyarrow as pa
 
 from bardi.nlp_engineering.regex_library.regex_lib import RegexSubPair
+from bardi.nlp_engineering.utils.polars_utils import retain_inputs
 from bardi.nlp_engineering.utils.validations import (
     validate_pyarrow_table,
     validate_str_cols,
 )
 from bardi.pipeline import DataWriteConfig, Step
 
 
 class Normalizer(Step):
     """Normalizer cleans and standardizes text input using regular expression
     substitutions. Lowercasing is also applied if desired.
 
     Note
     ----
-    
-    Avoid the direct instantiation of the Normalizer class and instead instantiate 
+
+    Avoid the direct instantiation of the Normalizer class and instead instantiate
     one of the child classes depending on hardware configuration.
 
     Attributes
     ----------
 
     fields : Union[str, List[str]]
         The field or fields to be normalized.
     regex_set : List[RegexSubPair]
         List of regex substitutions to be applied.
     lowercase : Optional[bool]
         If True, lowercasing will be applied during normalization,
         defaults to True.
+    retain_input_fields : Optional[bool]
+        If True, will retain the original contents of the fields specified in
+        `fields` under the new names of: `normalizer__<field>`
     """
 
     def __init__(
         self,
         fields: Union[str, List[str]],
         regex_set: List[RegexSubPair],
         lowercase: bool = True,
+        retain_input_fields: bool = False,
     ):
-        """Constructor method
-        """
+        """Constructor method"""
         # Normalizer Configuration
         self.fields = fields
+        if isinstance(fields, str):
+            self.fields = [fields]
+        self.retain_input_fields = retain_input_fields
         self._data_write_config: DataWriteConfig = {
             "data_format": "parquet",
             "data_format_args": {"compression": "snappy", "use_dictionary": False},
         }  # Default write config
         self.lowercase = lowercase
         # List of regex substitutions to be applied
         self.regex_set: List[RegexSubPair] = regex_set
 
     @abstractmethod
     def run(self):
-        """Abstract method
-        """
+        """Abstract method"""
         pass
 
 
 class CPUNormalizer(Normalizer):
-    """Normalizer class for cleaning and standardizing text input using regular expression substitutions.
+    """Normalizer class for cleaning and standardizing text input using regular
+    expression substitutions.
 
     Note
     ----
     This implementation of the Normalizer is specific for CPU computation.
 
     Attributes
     ----------
-    
+
     fields : Union[str, List[str]]
         The name of the column(s) containing text to be normalized.
     regex_set : List[RegexSubPair]
         A list of dictionaries with keys, 'regex_str' and 'sub_str', used to
         perform regular expression substitutions of the text.
-    lowercase : Optional[bool] 
+    lowercase : Optional[bool]
         If True, lowercasing will be applied during normalization.
         Default is True.
+    retain_input_fields : Optional[bool]
+        If True, will retain the original contents of the fields specified in
+        `fields` under the new names of: `normalizer__<field>`
     """
 
     def __init__(self, *args, **kwargs):
-        """Constructor method
-        """
+        """Constructor method"""
         super().__init__(*args, **kwargs)
         # Rust uses a different syntax for regex match groups
         # than standard (uses '$' instead of backslash)
         for regex_sub_pair in self.regex_set:
             regex_sub_pair["sub_str"] = regex_sub_pair["sub_str"].replace("\\", "$")
 
     def run(self, data: pa.Table, artifacts: Optional[dict] = None) -> Tuple[pa.Table, dict]:
@@ -114,22 +123,22 @@
         # Perform validations
         validate_pyarrow_table(data=data)
         validate_str_cols(fields=self.fields, data=data)
 
         def implement_regex_substitutions(df: pl.DataFrame) -> pl.DataFrame:
             """Reusable function to apply each regex substitution
             normalization to each string field
-            
+
             Parameters
             ----------
 
             df : pl.DataFrame
                 a DataFrame containing the columns specified in the Normalizer's
                 `fields` attribute
-            
+
             Returns
             -------
             pl.DataFrame
                 a DataFrame with the specified fields having its text transformed using
                 the regular expression substitution pairs in the Normalizer object's 'regex_set'
                 attribute
             """
@@ -146,20 +155,17 @@
                 )
             return df
 
         # Use the Polars library to apply the normalization methods
         # to each field of the Table that is specified in self.fields
         df = (
             pl.from_arrow(data)
+            .pipe(retain_inputs, self.retain_input_fields, self.fields, self.__class__.__name__)
             .with_columns(
-                [
-                    pl.col(field).str.to_lowercase()
-                    for field in self.fields
-                    if self.lowercase
-                ]
+                [pl.col(field).str.to_lowercase() for field in self.fields if self.lowercase]
             )
             .pipe(implement_regex_substitutions)
         )
 
         data = df.to_arrow()
 
         return (data, None)
```

### Comparing `bardi-0.3.1/bardi/nlp_engineering/post_processor.py` & `bardi-0.4.0/bardi/nlp_engineering/vocab_encoder.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,28 +7,29 @@
 from typing import List, Union
 
 import numpy as np
 import polars as pl
 import pyarrow as pa
 
 from bardi.data.utils.pyarrow_utils import chunk_pyarrow_table
+from bardi.nlp_engineering.utils.polars_utils import retain_inputs
 from bardi.nlp_engineering.utils.validations import (
     validate_list_str_cols,
     validate_pyarrow_table,
 )
 from bardi.pipeline import DataWriteConfig, Step
 
 
-class PostProcessor(Step):
-    """The post processor maps a vocab to a list of tokens
+class VocabEncoder(Step):
+    """The vocab encoder maps a vocab to a list of tokens
 
     Note
     ----
 
-    Avoid the direct instantiation of the PostProcessor class
+    Avoid the direct instantiation of the VocabEncoder class
     and instead instantiate one of the child classes depending
     on hardware configuration
 
     Attributes
     ----------
 
     fields : Union[str, List[str]]
@@ -43,29 +44,35 @@
         is optional for the construction of the object, and
         can alternatively be provided in the run method.
         This flexibility handles the use of a pre-existing
         vocab versus creating a vocab during a pipeline run.
     concat_fields : bool
         indicate if you would like for fields to be concatenated
         into a single column or left as separate columns
+    retain_input_fields : Optional[bool]
+        If True, will retain the original contents of the fields specified in
+        `fields` under the new names of: `vocabencoder__<field>`
     """
 
     def __init__(
         self,
         fields: Union[str, List[str]],
         field_rename: str = None,
         id_to_token: dict = None,
         concat_fields: bool = False,
+        retain_input_fields: bool = False,
     ):
         """Constructor method
         """
         self.fields = fields
         if isinstance(fields, str):
             self.fields = [fields]
 
+        self.retain_input_fields = retain_input_fields
+
         self.field_rename = "X"
         if field_rename:
             self.field_rename = field_rename
 
         self.mapping = None
         if id_to_token:
             # the actual application of the mapping requires
@@ -81,21 +88,21 @@
     @abstractmethod
     def run(self):
         """Abstract method
         """
         pass
 
 
-class CPUPostProcessor(PostProcessor):
-    """The post processor maps a vocab to a list of tokens
+class CPUVocabEncoder(VocabEncoder):
+    """The vocab encoder maps a vocab to a list of tokens
 
     Note
     ----
 
-    This implementation of the PostProcessor is specific for CPU computation.
+    This implementation of the VocabEncoder is specific for CPU computation.
 
     Attributes
     ----------
 
     fields : Union[str, List[str]]
         the name of the column containing a list of tokens
         that will be mapped to integers using a vocab
@@ -108,37 +115,40 @@
         is optional for the construction of the object, and
         can alternatively be provided in the run method.
         This flexibility handles the use of a pre-existing
         vocab versus creating a vocab during a pipeline run.
     concat_fields : bool
         indicate if you would like for fields to be concatenated
         into a single column or left as separate columns
+    retain_input_fields : Optional[bool]
+        If True, will retain the original contents of the fields specified in
+        `fields` under the new names of: `vocabencoder__<field>`
     """
 
     def __init__(self, *args, **kwargs):
         """Constructor method
         """
         super().__init__(*args, **kwargs)
 
     def run(
         self,
         data: pa.Table,
         artifacts: dict = None,
         id_to_token: dict = None,
     ) -> pa.Table:
-        """Run a post processor using CPU computation
+        """Run a vocab encoder using CPU computation
 
-        The post processor relies on receiving a vocab to map. The
+        The vocab encoder relies on receiving a vocab to map. The
         vocab can be supplied in multiple ways:
           - id_to_token at object creation
           - contained in the pipeline artifacts dictionary passed
             to the run method referenced by the key, 'id_to_token'
           - id_to_token in the run method
 
-        Attributes
+        Parameters
         ----------
 
         data : PyArrow Table
             The data to be processed. The data must contain the
             column specified by field at object creation
         artifacts : dict
             A dictionary of pipeline artifacts which contains
@@ -150,15 +160,15 @@
 
         Returns
         -------
 
         Tuple(PyArrow Table, dict)
             A tuple with:
                 - the first element holding a PyArrow Table of data
-                processed with the post processor
+                processed with the vocab encoder
                 - the second element of the tuple intended for
                 artifacts is None
 
         Raises
         ------
 
         AttributeError
@@ -168,30 +178,39 @@
             The run method was not supplied a PyArrow Table
         """
 
         # Perform validations
         validate_pyarrow_table(data=data)
         validate_list_str_cols(fields=self.fields, data=data)
 
+        # Retain original columns if needed - doing it here before any PyArrow Table
+        # chunking takes place
+        df = (
+            pl.from_arrow(data)
+            .pipe(retain_inputs, self.retain_input_fields, self.fields, self.__class__.__name__)
+        )
+        data = df.to_arrow()
+
         # Check if vocab was passed through the artifacts dict
-        if "id_to_token" in artifacts.keys():
-            id_to_token = artifacts["id_to_token"]
+        if artifacts:
+            if "id_to_token" in artifacts.keys():
+                id_to_token = artifacts["id_to_token"]
 
         # Check if a vocab was passed directly to the method -
         # the route used if a vocab was created during script execution
         if id_to_token:
             self.mapping = {token: id for id, token in id_to_token.items()}
         # Check if a vocab was referenced in the initial object creation -
         # the route used if there was a pre-existing vocab
         elif not self.mapping:
             # If a vocab wasn't referenced in either place, then there
             # isn't a vocab to use in this run method
             raise AttributeError(
                 "id_to_token must be provided to either "
-                "the PostProcessor object instantiation "
+                "the VocabEncoder object instantiation "
                 "or to the run method"
             )
 
         # Grab the <unk> id from the supplied vocab
         try:
             self.unk_id = self.mapping["<unk>"]
         except KeyError:
@@ -268,19 +287,19 @@
             df = df.rename({self.fields[0]: self.field_rename})
 
         data = df.to_arrow()
 
         return (data, None)
 
     def get_parameters(self):
-        """Retrive the post-processor object configuration
+        """Retrive the vocab encoder object configuration
         Does not return the mapping (vocab) as it can be large
 
         Returns
         -------
 
         dict
-            a dictionary representation of the post-processor's attributes
+            a dictionary representation of the vocab encoder's attributes
         """
         params = vars(self).copy()
         params.pop("mapping")
         return params
```

### Comparing `bardi-0.3.1/bardi/nlp_engineering/pre_tokenizer.py` & `bardi-0.4.0/bardi/nlp_engineering/pre_tokenizer.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from abc import abstractmethod
 from typing import List, Tuple, Union, Optional
 
 import polars as pl
 import pyarrow as pa
 
+from bardi.nlp_engineering.utils.polars_utils import retain_inputs
 from bardi.nlp_engineering.utils.validations import (
     validate_pyarrow_table,
     validate_str_cols,
 )
 from bardi.pipeline import Step
 
 
@@ -29,29 +30,36 @@
 
     fields : Union[str, List[str]]
         The name of the column(s) containing text.
     split_pattern : str
         A specific pattern of characters used to divide a string
         into smaller segments or tokens.
         By default, the split is done on a single space character.
+    retain_input_fields : Optional[bool]
+        If True, will retain the original contents of the fields specified in
+        `fields` under the new names of: `pretokenizer__<field>`
     """
 
-    def __init__(self, fields: Union[str, List[str]], split_pattern: str = " "):
-        """Constructor method
-        """
+    def __init__(
+        self,
+        fields: Union[str, List[str]],
+        split_pattern: str = " ",
+        retain_input_fields: bool = False,
+    ):
+        """Constructor method"""
         if isinstance(fields, str):
             self.fields = [fields]
         else:
             self.fields = fields
+        self.retain_input_fields = retain_input_fields
         self.split_pattern = split_pattern
 
     @abstractmethod
     def run(self):
-        """Abstract method
-        """
+        """Abstract method"""
         pass
 
 
 class CPUPreTokenizer(PreTokenizer):
     """The pre-tokenizer breaks down text into smaller units
     before further tokenization is applied.
 
@@ -65,19 +73,21 @@
 
     fields : Union[str, List[str]]
         The name of the column(s) containing text.
     split_pattern : str
         A specific pattern of characters used to divide a string
         into smaller segments or tokens.
         By default, the split is done on a single space character.
+    retain_input_fields : Optional[bool]
+        If True, will retain the original contents of the fields specified in
+        `fields` under the new names of: `pretokenizer__<field>`
     """
 
     def __init__(self, *args, **kwargs):
-        """Constructor method
-        """
+        """Constructor method"""
         super().__init__(*args, **kwargs)
 
     def run(
         self, data: pa.Table, artifacts: Optional[dict] = None
     ) -> Tuple[pa.Table, Union[dict, None]]:
         """Runs a CPU-based pre-tokenizer method based on the configuration
         used to create the object of the CPUPreTokenizer class.
@@ -101,22 +111,26 @@
             return None.
         """
         # Perform validations
         validate_pyarrow_table(data=data)
         validate_str_cols(fields=self.fields, data=data)
 
         # Split text fields into lists of tokens
-        df = pl.from_arrow(data).with_columns(
-            [
-                (
-                    pl.col(field)
-                    .str.split(by=self.split_pattern)
-                    .list.eval(pl.element().filter(pl.element() != ""))
-                    .alias(field)
-                )
-                for field in self.fields
-            ]
+        df = (
+            pl.from_arrow(data)
+            .pipe(retain_inputs, self.retain_input_fields, self.fields, self.__class__.__name__)
+            .with_columns(
+                [
+                    (
+                        pl.col(field)
+                        .str.split(by=self.split_pattern)
+                        .list.eval(pl.element().filter(pl.element() != ""))
+                        .alias(field)
+                    )
+                    for field in self.fields
+                ]
+            )
         )
 
         data = df.to_arrow()
 
         return (data, None)
```

### Comparing `bardi-0.3.1/bardi/nlp_engineering/regex_library/pathology_report.py` & `bardi-0.4.0/bardi/nlp_engineering/regex_library/pathology_report.py`

 * *Files identical despite different names*

### Comparing `bardi-0.3.1/bardi/nlp_engineering/regex_library/regex_lib.py` & `bardi-0.4.0/bardi/nlp_engineering/regex_library/regex_lib.py`

 * *Files identical despite different names*

### Comparing `bardi-0.3.1/bardi/nlp_engineering/splitter.py` & `bardi-0.4.0/bardi/nlp_engineering/splitter.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,95 +7,87 @@
 import polars as pl
 import pyarrow as pa
 
 from bardi.nlp_engineering.utils.validations import validate_pyarrow_table
 from bardi.pipeline import DataWriteConfig, Step
 
 MapSplit = NamedTuple(
-    "MapSplit", [("unique_record_cols", List[str]), ("split_mapping", Dict[str, str])]
+    "MapSplit",
+    [
+        ("unique_record_cols", List[str]),
+        ("split_mapping", Dict[str, str]),
+        ("default_split_value", str),
+    ],
 )
-MapSplit.__doc__ = (
-    """Specify the requirements for splitting data exactly in line with 
+MapSplit.__doc__ = """Specify the requirements for splitting data exactly in line with
     an existing data split
     """
-)
-MapSplit.unique_record_cols.__doc__ = (
-    """List of column names of which the combination forms a unique identifier in the
-    dataset. This can be a single column name if that creates a unique identifier,
-    but oftentimes in datasets a combination of fields are required.
+MapSplit.unique_record_cols.__doc__ = """List of column names of which the combination forms
+    a unique identifier in the dataset. This can be a single column name if that creates
+    a unique identifier, but oftentimes in datasets a combination of fields are required.
 
     Note: This set of columns MUST create a unique record or the program will crash.
     """
-)
-MapSplit.split_mapping.__doc__ = (
-    """`Only used for map split type.`
+MapSplit.split_mapping.__doc__ = """`Only used for map split type.`
     A dictionary mapping where the keys are the hash of the concatenated values from
     unique_record_cols, or represented by the following pseudocode, ::
         hash(concat(*unique_record_cols))
     The values are the corresponding split value (train, test, val) or (fold1, fold2, fold3), etc.
     """
-)
+MapSplit.default_split_value.__doc__ = """`Only used for map split type.`
+    A value to be used for split when the `unique_record_cols` cannot be found in the mapping. 
+    """
 
 NewSplit = NamedTuple(
     "NewSplit",
     [
         ("split_proportions", Dict[str, float]),
         ("unique_record_cols", List[str]),
         ("group_cols", List[str]),
         ("label_cols", List[str]),
         ("random_seed", int),
     ],
 )
-NewSplit.__doc__ = (
-    "Specify the requirements for splitting data with a new split from scratch."
-)
-NewSplit.split_proportions.__doc__ = (
-    """`Only used for new split type.`
+NewSplit.__doc__ = "Specify the requirements for splitting data with a new split from scratch."
+NewSplit.split_proportions.__doc__ = """`Only used for new split type.`
     Mapping of split names to split proportions. i.e., ::
         {'train': 0.75, 'test': 0.15, 'val': 0.15}
         {'fold1': 0.25, 'fold2': 0.25, 'fold3': 0.25, 'fold4': 0.25}
     Note: values must add to 1.0.
     """
-)
-NewSplit.unique_record_cols.__doc__ = (
-    """List of column names of which the combination forms a unique identifier in the
+NewSplit.unique_record_cols.__doc__ = """List of column names of which the combination forms a unique identifier in the
     dataset. This can be a single column name if that creates a unique identifier,
     but oftentimes in datasets a combination of fields are required.
 
     Note: This set of columns MUST create a unique record or the program will crash.
     """
-)
-NewSplit.group_cols.__doc__ = (
-    """List of column names that form a 'group' that you would like to keep in discrete
+NewSplit.group_cols.__doc__ = """List of column names that form a 'group' that you would like to keep in discrete
     splits. E.x., if you had multiple medical notes for a single patient,
     you may desire that all notes for a single patient end up in the same split
     to prevent potential information leakage. In this case you would provide
     something like a patient_id.
     """
-)
-NewSplit.label_cols.__doc__ = (
-    """List of column names containing labels. Efforts are made to balance label
+NewSplit.label_cols.__doc__ = """List of column names containing labels. Efforts are made to balance label
     distribution across splits, but this is not guaranteed.
     """
-)
 NewSplit.random_seed.__doc__ = (
     "Required for reproducibility. If you have no preference, try on 42 for size."
 )
 
 
 class Splitter(Step):
     """The splitter adds a 'split' column to the data assigning
     each record to a particular split for downstream model training.
 
     Note
     ----
 
     Avoid the direct instantiation of the Splitter class
     and instead instantiate one of the child classes.
-    
+
     Attributes
     ----------
 
     split_method : Union[MapSplit, NewSplit]
         A named tuple of either MapSplit type or NewSplit
         type. Each contains a different set of values
         used to create the splitter depending upon split type
@@ -110,15 +102,16 @@
 
         Note: This set of columns MUST create a unique record or the program will crash.
     split_mapping : dict[str, str]
         `Only used for map split type.`
         A dictionary mapping where the keys are the hash of the concatenated values from
         unique_record_cols, or represented by the following pseudocode, ::
             hash(concat(*unique_record_cols))
-        The values are the corresponding split value (train, test, val) or (fold1, fold2, fold3), etc.
+        The values are the corresponding split value (train, test, val) or
+        (fold1, fold2, fold3), etc.
     split_proportions : dict[str, float]
         `Only used for new split type.`
         Mapping of split names to split proportions. i.e., ::
             {'train': 0.75, 'test': 0.15, 'val': 0.15}
             {'fold1': 0.25, 'fold2': 0.25, 'fold3': 0.25, 'fold4': 0.25}
         Note: values must add to 1.0.
     num_splits : int
@@ -136,20 +129,20 @@
         Required for reproducibility. If you have no preference, try on `42` for size.
     """
 
     def __init__(
         self,
         split_method: Union[MapSplit, NewSplit],
     ):
-        """Constructor method
-        """
+        """Constructor method"""
         if isinstance(split_method, MapSplit):
             self.split_type = "map"
             self.unique_record_cols = split_method.unique_record_cols
             self.split_mapping = split_method.split_mapping
+            self.default_split_value = split_method.default_split_value
         elif isinstance(split_method, NewSplit):
             self.split_type = "new"
             self.split_proportions = split_method.split_proportions
             self.num_splits = len(self.split_proportions)
             self.unique_record_cols = split_method.unique_record_cols
             self.group_cols = split_method.group_cols
             self.label_cols = split_method.label_cols
@@ -157,16 +150,15 @@
         self._data_write_config: DataWriteConfig = {
             "data_format": "parquet",
             "data_format_args": {"compression": "snappy", "use_dictionary": False},
         }  # Default write config
 
     @abstractmethod
     def run(self):
-        """Abstract method
-        """
+        """Abstract method"""
         pass
 
 
 class CPUSplitter(Splitter):
     """The splitter adds a 'split' column to the data assigning
     each record to a particular split for downstream model training.
 
@@ -175,15 +167,15 @@
     second option is helpful when running comparisons with
     other methods of data processing ensuring that splits are
     exactly the same.
 
     Note
     ----
     This implementation of the LabelProcessor is specific for CPU computation.
-    
+
     To create a splitter, pass the appropriate set of parameters through a defined
     NamedTuple for the type of split you want to create. i.e., ::
 
         CPUSplitter(split_method=NewSplit(
             split_proportions={
                 'train': 0.75,
                 'test': 0.15,
@@ -197,17 +189,17 @@
                 'registry'
             ],
             labels_cols=[
                 'reportability'
             ],
             random_seed=42
         ))
-    
+
     Splitter Method Named Tuples:
-    
+
         *   :mod:`bardi.nlp_engineering.splitter.NewSplit`
         *   :mod:`bardi.nlp_engineering.splitter.MapSplit`
 
     Attributes
     ----------
     split_method : Union[MapSplit, NewSplit]
         A named tuple of either MapSplit type or NewSplit
@@ -224,15 +216,16 @@
 
         Note: This set of columns MUST create a unique record or the program will crash.
     split_mapping : dict[str, str]
         `Only used for map split type.`
         A dictionary mapping where the keys are the hash of the concatenated values from
         unique_record_cols, or represented by the following pseudocode, ::
             hash(concat(*unique_record_cols))
-        The values are the corresponding split value (train, test, val) or (fold1, fold2, fold3), etc.
+        The values are the corresponding split value (train, test, val) or
+        (fold1, fold2, fold3), etc.
     split_proportions : dict[str, float]
         `Only used for new split type.`
         Mapping of split names to split proportions. i.e., ::
             {'train': 0.75, 'test': 0.15, 'val': 0.15}
             {'fold1': 0.25, 'fold2': 0.25, 'fold3': 0.25, 'fold4': 0.25}
         Note: values must add to 1.0.
     num_splits : int
@@ -247,16 +240,15 @@
         List of column names containing labels. Efforts are made to balance label
         distribution across splits, but this is not guaranteed.
     random_seed: int
         Required for reproducibility. If you have no preference, try on `42` for size.
     """
 
     def __init__(self, *args, **kwargs):
-        """Constructor method
-        """
+        """Constructor method"""
         super().__init__(*args, **kwargs)
 
     def run(self, data: pa.Table, artifacts: dict = None) -> Tuple[pa.Table, dict]:
         """Runs a splitter using CPU computation based on the configuration
         used to create the object of the CPUSplitter class
 
         Parameters
@@ -295,48 +287,46 @@
 
             # Combine and hash the columns that form a unique/distinct
             # record and map a dictionary set up as:
             # {id: split} where id is also a combined and hashed
             # combination of the columns forming a unique record
             df = (
                 df.with_columns(
-                    [
-                        pl.concat_str([*self.unique_record_cols])
-                        .hash()
-                        .alias("composite_record_id")
-                    ]
+                    [pl.concat_str([*self.unique_record_cols]).hash().alias("composite_record_id")]
                 )
                 .with_columns(
                     [
                         pl.col("composite_record_id")
                         .cast(pl.Utf8())
-                        .map_dict(self.split_mapping)
+                        .replace(self.split_mapping, default=self.default_split_value)
                         .alias("split")
                     ]
                 )
                 .drop("composite_record_id")
             )
 
         elif self.split_type == "new":
             # Create a new split of the data if an existing desired
             # split does not yet exist
 
             # Get the set of distinct groups from the overall data
             distinct_groups = df.select([*self.group_cols]).unique(maintain_order=True)
             group_count = distinct_groups.height
-            # Generate a permutation of indices of distinct groups.
+
+            # Set random seeds for reporducibility
             np.random.seed(self.random_seed)
+            pl.set_random_seed(self.random_seed)
+
+            # Generate a permutation of indices of distinct groups.
             permuted_indices = np.random.permutation(group_count)
 
             # The splits assignment has to be done with a number
             # so a mapping must be created from a number to the
             # desired split name
-            split_name_maps = {
-                i: key for i, key in enumerate(self.split_proportions.keys())
-            }
+            split_name_maps = {i: key for i, key in enumerate(self.split_proportions.keys())}
 
             # Create a numpy array to hold the split labels (digits)
             split_labels = np.empty(group_count, dtype=int)
             start, end = 0, 0
             # Loop over the split proportion and assign digit
             # labels to the corresponding indices. If 15% of
             # data should be in a given split then we take a next
@@ -350,15 +340,15 @@
             split_labels[permuted_indices[end:]] = i
             split_labels = pl.Series(split_labels)
 
             # Add split labels as a column to distince groups
             # mapped to assigned value back to the name of
             # the split
             splits = distinct_groups.with_columns(
-                split_labels.map_dict(split_name_maps).alias("split")
+                split_labels.replace(split_name_maps).alias("split")
             )
 
             # Join the split set of distinct groups back to the rest
             # of the data. If a group had more than one record in the
             # dataset, this join will ensure those records are mapped
             # to the same split as the others in the group
             df = df.join(splits, on=[*self.group_cols], how="left")
```

### Comparing `bardi-0.3.1/bardi/nlp_engineering/utils/validations.py` & `bardi-0.4.0/bardi/nlp_engineering/utils/validations.py`

 * *Files identical despite different names*

### Comparing `bardi-0.3.1/bardi/pipeline.py` & `bardi-0.4.0/bardi/pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,30 +4,28 @@
 import tracemalloc
 from abc import ABCMeta, abstractmethod
 from datetime import datetime
 from typing import List, Literal, Tuple, TypedDict, Union
 
 import pyarrow as pa
 
-from bardi.data import data_handlers
-from bardi.data.data_handlers import Dataset
+from bardi.data import Dataset, write_file
 
 
 class DataWriteConfig(TypedDict):
     data_format: str
     data_format_args: Union[dict, None]
 
 
 class Step(metaclass=ABCMeta):
     """Blueprint for creating new steps for data pre-processing pipelines"""
 
     @abstractmethod
     def __init__(self):
-        """Constructor method
-        """
+        """Constructor method"""
         self._data_write_config: DataWriteConfig = {
             "data_format": "parquet",
             "data_format_args": {"compression": "snappy", "use_dictionary": False},
         }  # Default write config
 
     @abstractmethod
     def run(
@@ -64,15 +62,15 @@
         Provide a method to customize the write configuration
         used by the step's write_outputs method if desired.
 
         Parameters
         ----------
 
         data_config : DataWriteConfig
-            A typed dictionary defining the data_format (i.e., parquet, csv, etc.) 
+            A typed dictionary defining the data_format (i.e., parquet, csv, etc.)
             and any particular data_format_args available in the pyarrow API.
         """
         self._data_write_config = data_config
 
     def get_parameters(self) -> dict:
         """Default implementation of the get_parameters method.
 
@@ -97,29 +95,29 @@
         """Default implementation of the write_data method.
 
         Reuse existing write patterns that exist in the data handlers.
 
         Parameters
         ----------
 
-        write_path : str 
+        write_path : str
             A directory where a file will be written.
         data : Union[pa.Table, None]
             PyArrow Table of data.
         data_filename : Union[str, None]
             Overwrite default file name (no filetype extension).
         """
         # Add the filename with the appropriate filetype extension to the write path
         if not data_filename:
             data_filename = f"{self.__class__.__name__}Data"
         file_path = os.path.join(
             write_path, (f'{data_filename}.{self._data_write_config["data_format"]}')
         )
         # Call the data handler write_file function
-        data_handlers.write_file(
+        write_file(
             data=data,
             path=file_path,
             format=self._data_write_config["data_format"],
             **self._data_write_config["data_format_args"],
         )
 
     def write_artifacts(self, write_path: str, artifacts: Union[dict, None]):
@@ -138,44 +136,44 @@
         artifacts : Union[dict, None]
             A dictionary of artifacts from the step that should be written to a file
         """
         pass
 
 
 class Pipeline:
-    """Organize Steps into a pipeline to operate on data from a Dataset"""
+    """Organize Steps into a pipeline to operate on data from a Dataset
+
+    Attributes
+    ----------
+
+    dataset : bardi.data.data_handlers.Dataset
+        A bardi dataset object with data to pre-process.
+    write_path : str
+        Directory in the file system to write outputs to.
+    write_outputs : Literal["pipeline-outputs", "debug", False]
+        Configuration for which outputs to write.
+            *   'pipeline-outputs' will write all artifacts and final data.
+            *   'debug' will write all artifacts and data from each step.
+            *   False will not write any files.
+    data_write_config : DataWriteConfig
+        Supply a custom write configuration specifying
+        file types. Default will save data as parquet files.
+    data_filename : str
+        Supply a filename for the final output data.
+    """
 
     def __init__(
         self,
         dataset: Dataset = None,
         write_path: str = None,
         write_outputs: Literal["pipeline-outputs", "debug", False] = "pipeline-outputs",
         data_write_config: DataWriteConfig = None,
         data_filename: str = "bardi_processed_data",
     ):
-        """Create a pipeline for organizing data pre-processing steps.
-
-        Parameters
-        ----------
-
-        dataset : bardi.data.data_handlers.Dataset
-            A bardi dataset object with data to pre-process.
-        write_path : str
-            Directory in the file system to write outputs to.
-        write_outputs : Literal["pipeline-outputs", "debug", False]
-            Configuration for which outputs to write.
-                *   'pipeline-outputs' will write all artifacts and final data.
-                *   'debug' will write all artifacts and data from each step.
-                *   False will not write any files.
-        data_write_config : DataWriteConfig
-            Supply a custom write configuration specifying
-            file types. Default will save data as parquet files.
-        data_filename : str
-            Supply a filename for the final output data.
-        """
+        """Constructor Method"""
         # Reference a bardi dataset object that the pipeline will operate on
         self.dataset: Dataset = dataset
 
         # Pipeline configuration
         self.steps: List[Step] = []
         self.num_steps = 0
         self.write_outputs = write_outputs
@@ -216,17 +214,15 @@
             A bardi Step object to be added to the list of pipeline execution steps.
         """
         if isinstance(step, Step):
             step.set_write_config(data_config=self.data_write_config)
             self.steps.append(step)
             self.num_steps += 1
         else:
-            raise TypeError(
-                "Only objects of type Step may be added to " "a bardi pipeline."
-            )
+            raise TypeError("Only objects of type Step may be added to " "a bardi pipeline.")
 
     def run_pipeline(self) -> None:
         """Calls the run and write_outputs method for each respective step
         object added to the pipeline.
         """
 
         if isinstance(self.dataset, Dataset):
@@ -264,17 +260,15 @@
                 if isinstance(results[0], pa.Table):
                     # Set the pipeline's processed_data attribute to the newest result
                     self.processed_data = results[0]
 
                     # Write the step's data output to a file if pipeline is configured
                     # to do so
                     if self.write_outputs == "debug":
-                        step.write_data(
-                            write_path=self.write_path, data=self.processed_data
-                        )
+                        step.write_data(write_path=self.write_path, data=self.processed_data)
                     elif (
                         step_position == self.num_steps
                         and self.write_outputs == "pipeline-outputs"
                     ):
                         step.write_data(
                             write_path=self.write_path,
                             data=self.processed_data,
@@ -284,17 +278,15 @@
                     # If artifacts were returned by the step, add them to
                     # the pipeline's total set of artifacts
                     self.artifacts = {**self.artifacts, **results[1]}
 
                     # Write the step's artifacts to files if pipeline is configured
                     # to do so
                     if self.write_outputs:
-                        step.write_artifacts(
-                            write_path=self.write_path, artifacts=self.artifacts
-                        )
+                        step.write_artifacts(write_path=self.write_path, artifacts=self.artifacts)
             else:
                 raise TypeError(
                     "Pipeline expected step to return a tuple of "
                     "PyArrow Table of data and a dictionary of "
                     "artifacts. If the step doesn't return one of "
                     "these, that position in the tuple can be "
                     "empty, but it still needs to return a tuple."
```

### Comparing `bardi-0.3.1/bardi.egg-info/PKG-INFO` & `bardi-0.4.0/bardi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,47 @@
 Metadata-Version: 2.1
 Name: bardi
-Version: 0.3.1
+Version: 0.4.0
 Summary: A flexible machine learning data pre-processing pipeline framework.
 Author: Oak Ridge National Laboratory
 Project-URL: Homepage, https://github.com/DOE-NCI-MOSSAIC/bardi
 Project-URL: Documentation, https://doe-nci-mossaic.github.io/bardi/
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: duckdb>=0.8.0
+Requires-Dist: duckdb==0.8.0
 Requires-Dist: gensim>=4.1.2
 Requires-Dist: numpy>=1.21.5
 Requires-Dist: pandas>=1.4.4
 Requires-Dist: polars>=0.19.8
 Requires-Dist: pyarrow>=14.0.1
+Requires-Dist: tokenizers>=0.13.3
+Requires-Dist: transformers>=4.29.2
+Requires-Dist: datasets>=2.12.0
 
 
 # BARDI (Batch-processing Abstraction for Raw Data Integration)
 BARDI is a specialized framework engineered to facilitate the development of reproducible data pre-processing pipelines within machine learning workflows. 
 
 It emphasizes the following key aspects:
-    - Abstraction: By transforming common data pre-processing operations into modular components, Bardi simplifies both the development and upkeep of complex data pipelines.
-    - Efficiency: Utilizing Apache Arrow's columnar memory model for data storage and Polars for computations, Bardi enhances processing speed through multithreading, optimizing the use of available CPU resources.
-    - Modularity: Bardi's design is based on a component-driven architecture, offering users the flexibility to incorporate specific modules tailored to their unique requirements. These modules are crafted to operate seamlessly both as standalone units and within the context of a comprehensive pipeline.
-    - Extensibility: Designed with future growth in mind, Bardi allows for the straightforward addition of new custom steps, thereby broadening its functionality to encompass unaddressed demands and evolving data processing needs.
+
+ * Abstraction: By transforming common data pre-processing operations into modular components, Bardi simplifies both the
+    development and upkeep of complex data pipelines.
+
+ * Efficiency: Utilizing Apache Arrow's columnar memory model for data storage and Polars for computations, Bardi enhances
+    processing speed through multithreading, optimizing the use of available CPU resources.
+
+ * Modularity: Bardi's design is based on a component-driven architecture, offering users the flexibility to incorporate
+    specific modules tailored to their unique requirements. These modules are crafted to operate seamlessly both as standalone
+    units and within the context of a comprehensive pipeline.
+
+ * Extensibility: Designed with future growth in mind, Bardi allows for the straightforward addition of new custom steps,
+    thereby broadening its functionality to encompass unaddressed demands and evolving data processing needs.
 
 Installation
 ============
 
 ``pip install bardi``
 
 _currently not supported on Windows_
```

### Comparing `bardi-0.3.1/bardi.egg-info/SOURCES.txt` & `bardi-0.4.0/bardi.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -13,16 +13,21 @@
 bardi/data/data_handlers.py
 bardi/data/utils/__init__.py
 bardi/data/utils/pyarrow_utils.py
 bardi/nlp_engineering/__init__.py
 bardi/nlp_engineering/embedding_generator.py
 bardi/nlp_engineering/label_processor.py
 bardi/nlp_engineering/normalizer.py
-bardi/nlp_engineering/post_processor.py
 bardi/nlp_engineering/pre_tokenizer.py
 bardi/nlp_engineering/splitter.py
+bardi/nlp_engineering/tokenizer_encoder.py
+bardi/nlp_engineering/tokenizer_trainer.py
+bardi/nlp_engineering/vocab_encoder.py
 bardi/nlp_engineering/regex_library/__init__.py
 bardi/nlp_engineering/regex_library/pathology_report.py
 bardi/nlp_engineering/regex_library/regex_lib.py
 bardi/nlp_engineering/regex_library/regex_set.py
 bardi/nlp_engineering/utils/__init__.py
+bardi/nlp_engineering/utils/helper_utils.py
+bardi/nlp_engineering/utils/polars_utils.py
+bardi/nlp_engineering/utils/tokenizers_lib.py
 bardi/nlp_engineering/utils/validations.py
```

### Comparing `bardi-0.3.1/pyproject.toml` & `bardi-0.4.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 [build-system]
 requires = ["setuptools>=61.0",]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "bardi"
-version="0.3.1"
+version="0.4.0"
 authors = [{ name="Oak Ridge National Laboratory" },]
 description = "A flexible machine learning data pre-processing pipeline framework."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3 :: Only",
     "License :: OSI Approved :: MIT License",
 ]
-dependencies = ["duckdb>=0.8.0",
+dependencies = ["duckdb==0.8.0",
                 "gensim>=4.1.2",
                 "numpy>=1.21.5",
                 "pandas>=1.4.4",
                 "polars>=0.19.8",
                 "pyarrow>=14.0.1",
+                "tokenizers>=0.13.3",
+                "transformers>=4.29.2",
+                "datasets>=2.12.0"
                 ]
 
 [project.urls]
 Homepage = "https://github.com/DOE-NCI-MOSSAIC/bardi"
 Documentation = "https://doe-nci-mossaic.github.io/bardi/"
```

