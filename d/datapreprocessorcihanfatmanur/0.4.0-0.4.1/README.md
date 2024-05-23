# Comparing `tmp/datapreprocessorcihanfatmanur-0.4.0.tar.gz` & `tmp/datapreprocessorcihanfatmanur-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datapreprocessorcihanfatmanur-0.4.0.tar", last modified: Thu May 23 15:33:52 2024, max compression
+gzip compressed data, was "datapreprocessorcihanfatmanur-0.4.1.tar", last modified: Thu May 23 15:43:08 2024, max compression
```

## Comparing `datapreprocessorcihanfatmanur-0.4.0.tar` & `datapreprocessorcihanfatmanur-0.4.1.tar`

### file list

```diff
@@ -1,11 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 15:33:52.420004 datapreprocessorcihanfatmanur-0.4.0/
--rw-rw-rw-   0        0        0      374 2024-05-23 15:33:52.416139 datapreprocessorcihanfatmanur-0.4.0/PKG-INFO
--rw-rw-rw-   0        0        0     3967 2024-05-22 19:36:42.000000 datapreprocessorcihanfatmanur-0.4.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-23 15:33:52.410335 datapreprocessorcihanfatmanur-0.4.0/datapreprocessorcihanfatmanur.egg-info/
--rw-rw-rw-   0        0        0      374 2024-05-23 15:33:52.000000 datapreprocessorcihanfatmanur-0.4.0/datapreprocessorcihanfatmanur.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      282 2024-05-23 15:33:52.000000 datapreprocessorcihanfatmanur-0.4.0/datapreprocessorcihanfatmanur.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 15:33:52.000000 datapreprocessorcihanfatmanur-0.4.0/datapreprocessorcihanfatmanur.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2024-05-23 15:33:52.000000 datapreprocessorcihanfatmanur-0.4.0/datapreprocessorcihanfatmanur.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 15:33:52.000000 datapreprocessorcihanfatmanur-0.4.0/datapreprocessorcihanfatmanur.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-23 15:33:52.420634 datapreprocessorcihanfatmanur-0.4.0/setup.cfg
--rw-rw-rw-   0        0        0      501 2024-05-23 15:33:47.000000 datapreprocessorcihanfatmanur-0.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 15:43:08.278448 datapreprocessorcihanfatmanur-0.4.1/
+-rw-rw-rw-   0        0        0     4535 2024-05-23 15:43:08.278448 datapreprocessorcihanfatmanur-0.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3967 2024-05-22 19:36:42.000000 datapreprocessorcihanfatmanur-0.4.1/README.md
+-rw-rw-rw-   0        0        0      692 2024-05-23 15:43:08.278448 datapreprocessorcihanfatmanur-0.4.1/setup.cfg
+-rw-rw-rw-   0        0        0      501 2024-05-23 15:42:42.000000 datapreprocessorcihanfatmanur-0.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 15:43:08.210129 datapreprocessorcihanfatmanur-0.4.1/src/
+drwxrwxrwx   0        0        0        0 2024-05-23 15:43:08.241862 datapreprocessorcihanfatmanur-0.4.1/src/dataPreprocessor/
+-rw-rw-rw-   0        0        0      573 2024-05-21 12:59:39.000000 datapreprocessorcihanfatmanur-0.4.1/src/dataPreprocessor/__init__.py
+-rw-rw-rw-   0        0        0      696 2024-05-21 11:42:32.000000 datapreprocessorcihanfatmanur-0.4.1/src/dataPreprocessor/categorical_encoder.py
+-rw-rw-rw-   0        0        0      339 2024-05-21 11:42:35.000000 datapreprocessorcihanfatmanur-0.4.1/src/dataPreprocessor/data_type_converter.py
+-rw-rw-rw-   0        0        0      418 2024-05-21 11:42:35.000000 datapreprocessorcihanfatmanur-0.4.1/src/dataPreprocessor/datetime_handler.py
+-rw-rw-rw-   0        0        0      368 2024-05-21 13:05:57.000000 datapreprocessorcihanfatmanur-0.4.1/src/dataPreprocessor/feature_engineer.py
+-rw-rw-rw-   0        0        0      608 2024-05-21 11:42:34.000000 datapreprocessorcihanfatmanur-0.4.1/src/dataPreprocessor/missing_value_handler.py
+-rw-rw-rw-   0        0        0      437 2024-05-21 11:42:34.000000 datapreprocessorcihanfatmanur-0.4.1/src/dataPreprocessor/outlier_handler.py
+-rw-rw-rw-   0        0        0      494 2024-05-21 11:42:34.000000 datapreprocessorcihanfatmanur-0.4.1/src/dataPreprocessor/scaler.py
+-rw-rw-rw-   0        0        0      688 2024-05-21 11:42:33.000000 datapreprocessorcihanfatmanur-0.4.1/src/dataPreprocessor/text_cleaner.py
+drwxrwxrwx   0        0        0        0 2024-05-23 15:43:08.277882 datapreprocessorcihanfatmanur-0.4.1/src/datapreprocessorcihanfatmanur.egg-info/
+-rw-rw-rw-   0        0        0     4535 2024-05-23 15:43:08.000000 datapreprocessorcihanfatmanur-0.4.1/src/datapreprocessorcihanfatmanur.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      669 2024-05-23 15:43:08.000000 datapreprocessorcihanfatmanur-0.4.1/src/datapreprocessorcihanfatmanur.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 15:43:08.000000 datapreprocessorcihanfatmanur-0.4.1/src/datapreprocessorcihanfatmanur.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2024-05-23 15:43:08.000000 datapreprocessorcihanfatmanur-0.4.1/src/datapreprocessorcihanfatmanur.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-23 15:43:08.000000 datapreprocessorcihanfatmanur-0.4.1/src/datapreprocessorcihanfatmanur.egg-info/top_level.txt
```

### Comparing `datapreprocessorcihanfatmanur-0.4.0/README.md` & `datapreprocessorcihanfatmanur-0.4.1/README.md`

 * *Files identical despite different names*

