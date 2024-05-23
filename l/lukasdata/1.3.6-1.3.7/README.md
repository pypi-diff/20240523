# Comparing `tmp/lukasdata-1.3.6.tar.gz` & `tmp/lukasdata-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lukasdata-1.3.6.tar", last modified: Sat May 18 14:39:32 2024, max compression
+gzip compressed data, was "lukasdata-1.3.7.tar", last modified: Thu May 23 09:43:47 2024, max compression
```

## Comparing `lukasdata-1.3.6.tar` & `lukasdata-1.3.7.tar`

### file list

```diff
@@ -1,53 +1,58 @@
-drwxrwxrwx   0        0        0        0 2024-05-18 14:39:32.048454 lukasdata-1.3.6/
--rw-rw-rw-   0        0        0      128 2024-05-18 14:39:32.046454 lukasdata-1.3.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-18 14:39:31.951066 lukasdata-1.3.6/cleaning/
--rw-rw-rw-   0        0        0        0 2024-05-11 10:17:58.000000 lukasdata-1.3.6/cleaning/__init__.py
--rw-rw-rw-   0        0        0      416 2024-05-03 13:24:44.000000 lukasdata-1.3.6/cleaning/check_for_all_zeroes.py
--rw-rw-rw-   0        0        0      177 2024-05-18 14:37:26.000000 lukasdata-1.3.6/cleaning/clean_multiple_space.py
--rw-rw-rw-   0        0        0      387 2024-04-26 08:28:12.000000 lukasdata-1.3.6/cleaning/drop_column_with_na.py
--rw-rw-rw-   0        0        0      129 2024-04-26 08:32:10.000000 lukasdata-1.3.6/cleaning/mean_impute.py
--rw-rw-rw-   0        0        0      160 2024-04-26 08:29:44.000000 lukasdata-1.3.6/cleaning/na_counts.py
-drwxrwxrwx   0        0        0        0 2024-05-18 14:39:31.979049 lukasdata-1.3.6/datahandling/
--rw-rw-rw-   0        0        0        0 2024-05-11 10:17:58.000000 lukasdata-1.3.6/datahandling/__init__.py
--rw-rw-rw-   0        0        0      616 2024-04-22 22:29:19.000000 lukasdata-1.3.6/datahandling/change_directory.py
--rw-rw-rw-   0        0        0      184 2023-09-18 11:41:48.000000 lukasdata-1.3.6/datahandling/check_for_mismatches_in_list.py
--rw-rw-rw-   0        0        0      704 2023-10-29 15:04:54.000000 lukasdata-1.3.6/datahandling/create_text_for_all_files_in_pdf_dir.py
--rw-rw-rw-   0        0        0      503 2023-10-28 19:49:49.000000 lukasdata-1.3.6/datahandling/deconstruct_file_name.py
--rw-rw-rw-   0        0        0      178 2024-04-22 22:29:19.000000 lukasdata-1.3.6/datahandling/del_jpg.py
--rw-rw-rw-   0        0        0      334 2024-04-22 22:29:19.000000 lukasdata-1.3.6/datahandling/determine_file_type.py
--rw-rw-rw-   0        0        0      334 2024-04-22 22:29:19.000000 lukasdata-1.3.6/datahandling/dict_to_json.py
--rw-rw-rw-   0        0        0      257 2024-05-14 19:58:00.000000 lukasdata-1.3.6/datahandling/json_to_dict.py
--rw-rw-rw-   0        0        0      132 2024-04-30 10:39:24.000000 lukasdata-1.3.6/datahandling/order_dict.py
--rw-rw-rw-   0        0        0     1171 2023-10-29 14:47:29.000000 lukasdata-1.3.6/datahandling/pdf_to_txt.py
--rw-rw-rw-   0        0        0      193 2024-05-17 17:01:50.000000 lukasdata-1.3.6/datahandling/read_txt.py
--rw-rw-rw-   0        0        0      160 2024-04-22 22:29:19.000000 lukasdata-1.3.6/datahandling/string_to_text.py
-drwxrwxrwx   0        0        0        0 2024-05-18 14:39:31.983046 lukasdata-1.3.6/errorhandling/
--rw-rw-rw-   0        0        0        0 2024-05-11 10:17:58.000000 lukasdata-1.3.6/errorhandling/__init__.py
--rw-rw-rw-   0        0        0      587 2024-05-17 15:57:45.000000 lukasdata-1.3.6/errorhandling/custom_errors.py
-drwxrwxrwx   0        0        0        0 2024-05-18 14:39:31.995281 lukasdata-1.3.6/exploration/
--rw-rw-rw-   0        0        0        0 2024-05-11 10:17:58.000000 lukasdata-1.3.6/exploration/__init__.py
--rw-rw-rw-   0        0        0      440 2024-05-04 13:56:10.000000 lukasdata-1.3.6/exploration/analyze_datasets.py
--rw-rw-rw-   0        0        0      351 2024-04-22 22:29:19.000000 lukasdata-1.3.6/exploration/count_nans.py
--rw-rw-rw-   0        0        0     3566 2024-05-14 10:55:38.000000 lukasdata-1.3.6/exploration/desciptive_statistics.py
--rw-rw-rw-   0        0        0      385 2024-04-26 08:43:39.000000 lukasdata-1.3.6/exploration/get_list_intersection.py
--rw-rw-rw-   0        0        0        0 2024-05-14 10:08:25.000000 lukasdata-1.3.6/exploration/kernel_density_estimation.py
-drwxrwxrwx   0        0        0        0 2024-05-18 14:39:32.044456 lukasdata-1.3.6/lukasdata.egg-info/
--rw-rw-rw-   0        0        0      128 2024-05-18 14:39:31.000000 lukasdata-1.3.6/lukasdata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1336 2024-05-18 14:39:31.000000 lukasdata-1.3.6/lukasdata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-18 14:39:31.000000 lukasdata-1.3.6/lukasdata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2024-05-18 14:39:31.000000 lukasdata-1.3.6/lukasdata.egg-info/requires.txt
--rw-rw-rw-   0        0        0       78 2024-05-18 14:39:31.000000 lukasdata-1.3.6/lukasdata.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-18 14:39:32.030464 lukasdata-1.3.6/machine_learning/
--rw-rw-rw-   0        0        0        0 2024-05-11 10:17:58.000000 lukasdata-1.3.6/machine_learning/__init__.py
--rw-rw-rw-   0        0        0      322 2024-05-08 17:36:02.000000 lukasdata-1.3.6/machine_learning/drop_columns_permutation_score.py
--rw-rw-rw-   0        0        0     2005 2024-05-11 09:53:36.000000 lukasdata-1.3.6/machine_learning/keras_input.py
--rw-rw-rw-   0        0        0     1746 2024-05-14 10:55:46.000000 lukasdata-1.3.6/machine_learning/ml_model.py
--rw-rw-rw-   0        0        0     2400 2024-05-09 08:33:54.000000 lukasdata-1.3.6/machine_learning/permutation_importance.py
-drwxrwxrwx   0        0        0        0 2024-05-18 14:39:32.042457 lukasdata-1.3.6/manipulation/
--rw-rw-rw-   0        0        0        0 2024-05-11 10:17:58.000000 lukasdata-1.3.6/manipulation/__init__.py
--rw-rw-rw-   0        0        0      260 2024-04-29 20:51:11.000000 lukasdata-1.3.6/manipulation/concat_dfs.py
--rw-rw-rw-   0        0        0      332 2024-04-22 22:29:19.000000 lukasdata-1.3.6/manipulation/create_mask.py
--rw-rw-rw-   0        0        0      466 2024-05-13 11:10:36.000000 lukasdata-1.3.6/manipulation/int_columns.py
--rw-rw-rw-   0        0        0      144 2024-04-22 22:29:19.000000 lukasdata-1.3.6/manipulation/list_to_string.py
--rw-rw-rw-   0        0        0       42 2024-05-18 14:39:32.049454 lukasdata-1.3.6/setup.cfg
--rw-rw-rw-   0        0        0      192 2024-05-18 14:39:24.000000 lukasdata-1.3.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 09:43:47.072157 lukasdata-1.3.7/
+-rw-rw-rw-   0        0        0      128 2024-05-23 09:43:47.066161 lukasdata-1.3.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-23 09:43:46.918899 lukasdata-1.3.7/cleaning/
+-rw-rw-rw-   0        0        0        0 2024-05-11 10:17:58.000000 lukasdata-1.3.7/cleaning/__init__.py
+-rw-rw-rw-   0        0        0      416 2024-05-03 13:24:44.000000 lukasdata-1.3.7/cleaning/check_for_all_zeroes.py
+-rw-rw-rw-   0        0        0      177 2024-05-18 14:37:26.000000 lukasdata-1.3.7/cleaning/clean_multiple_space.py
+-rw-rw-rw-   0        0        0      387 2024-04-26 08:28:12.000000 lukasdata-1.3.7/cleaning/drop_column_with_na.py
+-rw-rw-rw-   0        0        0      129 2024-04-26 08:32:10.000000 lukasdata-1.3.7/cleaning/mean_impute.py
+-rw-rw-rw-   0        0        0      317 2024-05-21 21:30:45.000000 lukasdata-1.3.7/cleaning/my_strip.py
+-rw-rw-rw-   0        0        0      160 2024-04-26 08:29:44.000000 lukasdata-1.3.7/cleaning/na_counts.py
+-rw-rw-rw-   0        0        0      130 2024-05-23 09:36:16.000000 lukasdata-1.3.7/cleaning/order_dict_by_key.py
+-rw-rw-rw-   0        0        0      325 2024-05-22 11:05:51.000000 lukasdata-1.3.7/cleaning/replace_umlaut.py
+drwxrwxrwx   0        0        0        0 2024-05-23 09:43:46.986861 lukasdata-1.3.7/datahandling/
+-rw-rw-rw-   0        0        0        0 2024-05-11 10:17:58.000000 lukasdata-1.3.7/datahandling/__init__.py
+-rw-rw-rw-   0        0        0      616 2024-05-23 09:41:11.000000 lukasdata-1.3.7/datahandling/change_directory.py
+-rw-rw-rw-   0        0        0      546 2024-05-21 20:40:00.000000 lukasdata-1.3.7/datahandling/change_encoding.py
+-rw-rw-rw-   0        0        0      184 2023-09-18 11:41:48.000000 lukasdata-1.3.7/datahandling/check_for_mismatches_in_list.py
+-rw-rw-rw-   0        0        0      704 2023-10-29 15:04:54.000000 lukasdata-1.3.7/datahandling/create_text_for_all_files_in_pdf_dir.py
+-rw-rw-rw-   0        0        0      503 2023-10-28 19:49:49.000000 lukasdata-1.3.7/datahandling/deconstruct_file_name.py
+-rw-rw-rw-   0        0        0      178 2024-04-22 22:29:19.000000 lukasdata-1.3.7/datahandling/del_jpg.py
+-rw-rw-rw-   0        0        0      334 2024-04-22 22:29:19.000000 lukasdata-1.3.7/datahandling/determine_file_type.py
+-rw-rw-rw-   0        0        0      334 2024-04-22 22:29:19.000000 lukasdata-1.3.7/datahandling/dict_to_json.py
+-rw-rw-rw-   0        0        0      257 2024-05-14 19:58:00.000000 lukasdata-1.3.7/datahandling/json_to_dict.py
+-rw-rw-rw-   0        0        0      132 2024-04-30 10:39:24.000000 lukasdata-1.3.7/datahandling/order_dict.py
+-rw-rw-rw-   0        0        0     1171 2023-10-29 14:47:29.000000 lukasdata-1.3.7/datahandling/pdf_to_txt.py
+-rw-rw-rw-   0        0        0      193 2024-05-17 17:01:50.000000 lukasdata-1.3.7/datahandling/read_txt.py
+-rw-rw-rw-   0        0        0      160 2024-04-22 22:29:19.000000 lukasdata-1.3.7/datahandling/string_to_text.py
+drwxrwxrwx   0        0        0        0 2024-05-23 09:43:46.991860 lukasdata-1.3.7/errorhandling/
+-rw-rw-rw-   0        0        0        0 2024-05-11 10:17:58.000000 lukasdata-1.3.7/errorhandling/__init__.py
+-rw-rw-rw-   0        0        0      587 2024-05-17 15:57:45.000000 lukasdata-1.3.7/errorhandling/custom_errors.py
+drwxrwxrwx   0        0        0        0 2024-05-23 09:43:47.007849 lukasdata-1.3.7/exploration/
+-rw-rw-rw-   0        0        0        0 2024-05-11 10:17:58.000000 lukasdata-1.3.7/exploration/__init__.py
+-rw-rw-rw-   0        0        0      440 2024-05-04 13:56:10.000000 lukasdata-1.3.7/exploration/analyze_datasets.py
+-rw-rw-rw-   0        0        0      351 2024-04-22 22:29:19.000000 lukasdata-1.3.7/exploration/count_nans.py
+-rw-rw-rw-   0        0        0     3566 2024-05-14 10:55:38.000000 lukasdata-1.3.7/exploration/desciptive_statistics.py
+-rw-rw-rw-   0        0        0      385 2024-04-26 08:43:39.000000 lukasdata-1.3.7/exploration/get_list_intersection.py
+-rw-rw-rw-   0        0        0        0 2024-05-14 10:08:25.000000 lukasdata-1.3.7/exploration/kernel_density_estimation.py
+drwxrwxrwx   0        0        0        0 2024-05-23 09:43:47.064162 lukasdata-1.3.7/lukasdata.egg-info/
+-rw-rw-rw-   0        0        0      128 2024-05-23 09:43:46.000000 lukasdata-1.3.7/lukasdata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1481 2024-05-23 09:43:46.000000 lukasdata-1.3.7/lukasdata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 09:43:46.000000 lukasdata-1.3.7/lukasdata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2024-05-23 09:43:46.000000 lukasdata-1.3.7/lukasdata.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       78 2024-05-23 09:43:46.000000 lukasdata-1.3.7/lukasdata.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-23 09:43:47.049169 lukasdata-1.3.7/machine_learning/
+-rw-rw-rw-   0        0        0        0 2024-05-11 10:17:58.000000 lukasdata-1.3.7/machine_learning/__init__.py
+-rw-rw-rw-   0        0        0      322 2024-05-08 17:36:02.000000 lukasdata-1.3.7/machine_learning/drop_columns_permutation_score.py
+-rw-rw-rw-   0        0        0     2005 2024-05-11 09:53:36.000000 lukasdata-1.3.7/machine_learning/keras_input.py
+-rw-rw-rw-   0        0        0     3768 2024-04-30 19:39:47.000000 lukasdata-1.3.7/machine_learning/missing_forest.py
+-rw-rw-rw-   0        0        0     1746 2024-05-14 10:55:46.000000 lukasdata-1.3.7/machine_learning/ml_model.py
+-rw-rw-rw-   0        0        0     2400 2024-05-09 08:33:54.000000 lukasdata-1.3.7/machine_learning/permutation_importance.py
+drwxrwxrwx   0        0        0        0 2024-05-23 09:43:47.062162 lukasdata-1.3.7/manipulation/
+-rw-rw-rw-   0        0        0        0 2024-05-11 10:17:58.000000 lukasdata-1.3.7/manipulation/__init__.py
+-rw-rw-rw-   0        0        0      260 2024-04-29 20:51:11.000000 lukasdata-1.3.7/manipulation/concat_dfs.py
+-rw-rw-rw-   0        0        0      332 2024-04-22 22:29:19.000000 lukasdata-1.3.7/manipulation/create_mask.py
+-rw-rw-rw-   0        0        0      466 2024-05-13 11:10:36.000000 lukasdata-1.3.7/manipulation/int_columns.py
+-rw-rw-rw-   0        0        0      144 2024-04-22 22:29:19.000000 lukasdata-1.3.7/manipulation/list_to_string.py
+-rw-rw-rw-   0        0        0       42 2024-05-23 09:43:47.072157 lukasdata-1.3.7/setup.cfg
+-rw-rw-rw-   0        0        0      192 2024-05-23 09:43:38.000000 lukasdata-1.3.7/setup.py
```

### Comparing `lukasdata-1.3.6/datahandling/change_directory.py` & `lukasdata-1.3.7/datahandling/change_directory.py`

 * *Files identical despite different names*

### Comparing `lukasdata-1.3.6/datahandling/create_text_for_all_files_in_pdf_dir.py` & `lukasdata-1.3.7/datahandling/create_text_for_all_files_in_pdf_dir.py`

 * *Files identical despite different names*

### Comparing `lukasdata-1.3.6/datahandling/pdf_to_txt.py` & `lukasdata-1.3.7/datahandling/pdf_to_txt.py`

 * *Files identical despite different names*

### Comparing `lukasdata-1.3.6/errorhandling/custom_errors.py` & `lukasdata-1.3.7/errorhandling/custom_errors.py`

 * *Files identical despite different names*

### Comparing `lukasdata-1.3.6/exploration/desciptive_statistics.py` & `lukasdata-1.3.7/exploration/desciptive_statistics.py`

 * *Files identical despite different names*

### Comparing `lukasdata-1.3.6/lukasdata.egg-info/SOURCES.txt` & `lukasdata-1.3.7/lukasdata.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 setup.py
 cleaning/__init__.py
 cleaning/check_for_all_zeroes.py
 cleaning/clean_multiple_space.py
 cleaning/drop_column_with_na.py
 cleaning/mean_impute.py
+cleaning/my_strip.py
 cleaning/na_counts.py
+cleaning/order_dict_by_key.py
+cleaning/replace_umlaut.py
 datahandling/__init__.py
 datahandling/change_directory.py
+datahandling/change_encoding.py
 datahandling/check_for_mismatches_in_list.py
 datahandling/create_text_for_all_files_in_pdf_dir.py
 datahandling/deconstruct_file_name.py
 datahandling/del_jpg.py
 datahandling/determine_file_type.py
 datahandling/dict_to_json.py
 datahandling/json_to_dict.py
@@ -30,14 +34,15 @@
 lukasdata.egg-info/SOURCES.txt
 lukasdata.egg-info/dependency_links.txt
 lukasdata.egg-info/requires.txt
 lukasdata.egg-info/top_level.txt
 machine_learning/__init__.py
 machine_learning/drop_columns_permutation_score.py
 machine_learning/keras_input.py
+machine_learning/missing_forest.py
 machine_learning/ml_model.py
 machine_learning/permutation_importance.py
 manipulation/__init__.py
 manipulation/concat_dfs.py
 manipulation/create_mask.py
 manipulation/int_columns.py
 manipulation/list_to_string.py
```

### Comparing `lukasdata-1.3.6/machine_learning/keras_input.py` & `lukasdata-1.3.7/machine_learning/keras_input.py`

 * *Files identical despite different names*

### Comparing `lukasdata-1.3.6/machine_learning/ml_model.py` & `lukasdata-1.3.7/machine_learning/ml_model.py`

 * *Files identical despite different names*

### Comparing `lukasdata-1.3.6/machine_learning/permutation_importance.py` & `lukasdata-1.3.7/machine_learning/permutation_importance.py`

 * *Files identical despite different names*

