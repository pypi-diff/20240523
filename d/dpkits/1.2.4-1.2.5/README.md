# Comparing `tmp/dpkits-1.2.4.tar.gz` & `tmp/dpkits-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dpkits-1.2.4.tar", last modified: Tue May 21 08:46:58 2024, max compression
+gzip compressed data, was "dpkits-1.2.5.tar", last modified: Thu May 23 03:24:17 2024, max compression
```

## Comparing `dpkits-1.2.4.tar` & `dpkits-1.2.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 08:46:58.211915 dpkits-1.2.4/
--rw-rw-rw-   0        0        0     1091 2023-08-31 09:04:23.000000 dpkits-1.2.4/LICENSE
--rw-rw-rw-   0        0        0    12196 2024-05-21 08:46:58.209912 dpkits-1.2.4/PKG-INFO
--rw-rw-rw-   0        0        0    11652 2023-10-06 10:25:52.000000 dpkits-1.2.4/README.md
--rw-rw-rw-   0        0        0      626 2024-05-21 08:44:34.000000 dpkits-1.2.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-21 08:46:58.211915 dpkits-1.2.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-21 08:46:58.138457 dpkits-1.2.4/src/
-drwxrwxrwx   0        0        0        0 2024-05-21 08:46:58.173342 dpkits-1.2.4/src/dpkits/
--rw-rw-rw-   0        0        0      565 2024-01-11 08:02:54.000000 dpkits-1.2.4/src/dpkits/__init__.py
--rw-rw-rw-   0        0        0    28970 2024-05-15 03:48:44.000000 dpkits-1.2.4/src/dpkits/ap_data_converter.py
--rw-rw-rw-   0        0        0     9948 2023-10-04 08:35:50.000000 dpkits-1.2.4/src/dpkits/calculate_lsm.py
--rw-rw-rw-   0        0        0    11069 2024-01-31 04:23:09.000000 dpkits-1.2.4/src/dpkits/codeframe_reader.py
--rw-rw-rw-   0        0        0     5209 2024-05-06 08:45:27.000000 dpkits-1.2.4/src/dpkits/data_analysis.py
--rw-rw-rw-   0        0        0     3241 2024-05-16 11:03:27.000000 dpkits-1.2.4/src/dpkits/data_processing.py
--rw-rw-rw-   0        0        0     8198 2024-03-29 03:28:36.000000 dpkits-1.2.4/src/dpkits/data_transpose.py
--rw-rw-rw-   0        0        0    26578 2024-05-10 10:00:29.000000 dpkits-1.2.4/src/dpkits/table_formater.py
--rw-rw-rw-   0        0        0    66209 2024-05-21 07:59:21.000000 dpkits-1.2.4/src/dpkits/table_generator.py
-drwxrwxrwx   0        0        0        0 2024-05-21 08:46:58.207917 dpkits-1.2.4/src/dpkits.egg-info/
--rw-rw-rw-   0        0        0    12196 2024-05-21 08:46:58.000000 dpkits-1.2.4/src/dpkits.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      428 2024-05-21 08:46:58.000000 dpkits-1.2.4/src/dpkits.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 08:46:58.000000 dpkits-1.2.4/src/dpkits.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-21 08:46:58.000000 dpkits-1.2.4/src/dpkits.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-23 03:24:17.160061 dpkits-1.2.5/
+-rw-rw-rw-   0        0        0     1091 2023-08-31 09:04:23.000000 dpkits-1.2.5/LICENSE
+-rw-rw-rw-   0        0        0    12196 2024-05-23 03:24:17.158047 dpkits-1.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0    11652 2023-10-06 10:25:52.000000 dpkits-1.2.5/README.md
+-rw-rw-rw-   0        0        0      626 2024-05-23 03:23:38.000000 dpkits-1.2.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-23 03:24:17.160061 dpkits-1.2.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-23 03:24:17.090657 dpkits-1.2.5/src/
+drwxrwxrwx   0        0        0        0 2024-05-23 03:24:17.127811 dpkits-1.2.5/src/dpkits/
+-rw-rw-rw-   0        0        0      565 2024-01-11 08:02:54.000000 dpkits-1.2.5/src/dpkits/__init__.py
+-rw-rw-rw-   0        0        0    28970 2024-05-15 03:48:44.000000 dpkits-1.2.5/src/dpkits/ap_data_converter.py
+-rw-rw-rw-   0        0        0     9948 2023-10-04 08:35:50.000000 dpkits-1.2.5/src/dpkits/calculate_lsm.py
+-rw-rw-rw-   0        0        0    11069 2024-01-31 04:23:09.000000 dpkits-1.2.5/src/dpkits/codeframe_reader.py
+-rw-rw-rw-   0        0        0     5209 2024-05-06 08:45:27.000000 dpkits-1.2.5/src/dpkits/data_analysis.py
+-rw-rw-rw-   0        0        0     3241 2024-05-16 11:03:27.000000 dpkits-1.2.5/src/dpkits/data_processing.py
+-rw-rw-rw-   0        0        0     8198 2024-03-29 03:28:36.000000 dpkits-1.2.5/src/dpkits/data_transpose.py
+-rw-rw-rw-   0        0        0    26578 2024-05-10 10:00:29.000000 dpkits-1.2.5/src/dpkits/table_formater.py
+-rw-rw-rw-   0        0        0    67364 2024-05-23 03:12:24.000000 dpkits-1.2.5/src/dpkits/table_generator.py
+drwxrwxrwx   0        0        0        0 2024-05-23 03:24:17.155969 dpkits-1.2.5/src/dpkits.egg-info/
+-rw-rw-rw-   0        0        0    12196 2024-05-23 03:24:17.000000 dpkits-1.2.5/src/dpkits.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      428 2024-05-23 03:24:17.000000 dpkits-1.2.5/src/dpkits.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 03:24:17.000000 dpkits-1.2.5/src/dpkits.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-23 03:24:17.000000 dpkits-1.2.5/src/dpkits.egg-info/top_level.txt
```

### Comparing `dpkits-1.2.4/LICENSE` & `dpkits-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dpkits-1.2.4/PKG-INFO` & `dpkits-1.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dpkits
-Version: 1.2.4
+Version: 1.2.5
 Summary: A small package for data processing
 Author-email: Hung Dao <hung.daotuan.1991@gmail.com>
 Project-URL: Homepage, https://github.com/HungDaoHD/packaging_dpkits
 Project-URL: Bug Tracker, https://github.com/HungDaoHD/packaging_dpkits/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dpkits-1.2.4/README.md` & `dpkits-1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `dpkits-1.2.4/pyproject.toml` & `dpkits-1.2.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dpkits"
-version = "1.2.4"
+version = "1.2.5"
 authors = [
   { name="Hung Dao", email="hung.daotuan.1991@gmail.com" },
 ]
 description = "A small package for data processing"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `dpkits-1.2.4/src/dpkits/__init__.py` & `dpkits-1.2.5/src/dpkits/__init__.py`

 * *Files identical despite different names*

### Comparing `dpkits-1.2.4/src/dpkits/ap_data_converter.py` & `dpkits-1.2.5/src/dpkits/ap_data_converter.py`

 * *Files identical despite different names*

### Comparing `dpkits-1.2.4/src/dpkits/calculate_lsm.py` & `dpkits-1.2.5/src/dpkits/calculate_lsm.py`

 * *Files identical despite different names*

### Comparing `dpkits-1.2.4/src/dpkits/codeframe_reader.py` & `dpkits-1.2.5/src/dpkits/codeframe_reader.py`

 * *Files identical despite different names*

### Comparing `dpkits-1.2.4/src/dpkits/data_analysis.py` & `dpkits-1.2.5/src/dpkits/data_analysis.py`

 * *Files identical despite different names*

### Comparing `dpkits-1.2.4/src/dpkits/data_processing.py` & `dpkits-1.2.5/src/dpkits/data_processing.py`

 * *Files identical despite different names*

### Comparing `dpkits-1.2.4/src/dpkits/data_transpose.py` & `dpkits-1.2.5/src/dpkits/data_transpose.py`

 * *Files identical despite different names*

### Comparing `dpkits-1.2.4/src/dpkits/table_formater.py` & `dpkits-1.2.5/src/dpkits/table_formater.py`

 * *Files identical despite different names*

### Comparing `dpkits-1.2.4/src/dpkits/table_generator.py` & `dpkits-1.2.5/src/dpkits/table_generator.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,16 +26,20 @@
 
         self.dict_unnetted_qres = dict()
         for idx in self.df_info.index:
             if 'net_code' in self.df_info.at[idx, 'val_lbl'].keys():
                 self.dict_unnetted_qres.update({self.df_info.at[idx, 'var_name']: self.unnetted_qre_val(self.df_info.at[idx, 'val_lbl'])})
 
 
+        # Check matching of data và defines
         self.check_value_df_data_vs_df_info()
 
+        # Check duplicate value of MA qres
+        self.check_duplicate_value_ma_vars()
+
         try:
             check_perm = open(xlsx_name)
             check_perm.close()
         except PermissionError:
             print(f'\x1b[31;20mPermission Error when access file: {xlsx_name}', 'Processing terminated.')
             exit()
         except FileNotFoundError:
@@ -77,14 +81,38 @@
             print('\x1b[31;20m\nPlease check values not in codelist:\n', df_data)
             exit()
 
         print("Check value - df_data & df_info - Done")
 
 
 
+    def check_duplicate_value_ma_vars(self):
+
+        df_info_ma = self.df_info.query(r"var_name.str.contains('^\w+_1$') & var_type.str.contains('MA')")
+
+        for qre_ma in df_info_ma['var_name'].values.tolist():
+
+            prefix, suffix = qre_ma.rsplit('_', 1)
+            df_data_qre_ma = self.df_data.filter(regex=f"^{prefix}_[0-9]+$")
+            df_data_qre_ma = df_data_qre_ma.T
+
+            for col in df_data_qre_ma.columns:
+                df_data_qre_ma[col] = df_data_qre_ma[col].drop_duplicates(keep='first')
+
+
+            self.df_data.loc[:, list(df_data_qre_ma.index)] = df_data_qre_ma.T
+
+
+
+
+
+
+
+
+
     def convert_md_to_mc(self, df_data: pd.DataFrame, df_info: pd.DataFrame):
 
         df_info_qre_ma_all_1st_col = df_info.query("var_type.isin(['MA', 'MA_mtr']) & var_name.str.contains('[A-Za-z]+_1$')").copy()
 
         for idx in df_info_qre_ma_all_1st_col.index:
             qre = df_info_qre_ma_all_1st_col.at[idx, 'var_name'].rsplit('_', 1)[0]
 
@@ -1104,27 +1132,37 @@
                     continue
 
                 if item not in lst_ran_col:
                     lst_ran_col.append(item)
 
                 df_filter = dict_header_col_name[item]['df_data'].loc[:, lst_qre_col].copy()
 
+                # df_filter = dict_header_col_name[item]['df_data'].loc[:, lst_qre_col].copy().T
+                #
+                # for idx_col in df_filter.columns:
+                #     df_filter[idx_col] = df_filter[idx_col].drop_duplicates(keep='first')
+                #
+                # df_filter = df_filter.T
+
+
                 if df_filter.empty:
                     continue
 
                 if lst_sub_cat:
                     dict_re_qre_val = {int(k): 1 if k in lst_sub_cat else 0 for k, v in qre_val.items()}
 
                 else:
                     dict_re_qre_val = {int(k): 1 if k == cat else 0 for k, v in qre_val.items()}
 
                 df_filter.replace(dict_re_qre_val, inplace=True)
 
-                df_fil_base = df_filter[lst_qre_col].dropna(how='all')
-                df_filter.loc[df_fil_base.index, 'ma_val_sum'] = df_filter.loc[df_fil_base.index, lst_qre_col].sum(axis='columns')
+                # df_fil_base = df_filter[lst_qre_col].dropna(how='all')
+                df_fil_base = df_filter.dropna(how='all')
+
+                df_filter.loc[df_fil_base.index, 'ma_val_sum'] = df_filter.loc[df_fil_base.index, :].sum(axis='columns')
 
                 if lst_sub_cat or qre_type == 'MA_comb':
                     df_filter.loc[df_filter['ma_val_sum'] > 1, 'ma_val_sum'] = 1
 
                 dict_pair_to_sig.update({item: df_filter['ma_val_sum']})
 
                 # UPDATE FOR WEIGHTED TABLE
@@ -1452,17 +1490,14 @@
                 # df_qre = self.add_num_qre_to_tbl_sig(df_qre, qre_info, dict_header_col_name, 'std', lst_sig_pair, sig_type, lst_sig_lvl, weight_var)
                 # df_qre = self.add_num_qre_to_tbl_sig(df_qre, qre_info, dict_header_col_name, 'min', lst_sig_pair, sig_type, lst_sig_lvl, weight_var)
                 # df_qre = self.add_num_qre_to_tbl_sig(df_qre, qre_info, dict_header_col_name, 'max', lst_sig_pair, sig_type, lst_sig_lvl, weight_var)
                 # df_qre = self.add_num_qre_to_tbl_sig(df_qre, qre_info, dict_header_col_name, '25%', lst_sig_pair, sig_type, lst_sig_lvl, weight_var)
                 # df_qre = self.add_num_qre_to_tbl_sig(df_qre, qre_info, dict_header_col_name, '50%', lst_sig_pair, sig_type, lst_sig_lvl, weight_var)
                 # df_qre = self.add_num_qre_to_tbl_sig(df_qre, qre_info, dict_header_col_name, '75%', lst_sig_pair, sig_type, lst_sig_lvl, weight_var)
 
-
-
-
             elif qre_type in ['MA', 'MA_mtr', 'MA_comb', 'MA_Rank']:
 
                 # if 'Q1a' in qre_name:
                 #     a = 1
 
                 if f'{qre_name}_1' in self.dict_unnetted_qres.keys() and f'{qre_name}_2' in self.dict_unnetted_qres.keys():
                     qre_val_unnetted = self.dict_unnetted_qres[f'{qre_name}_1']
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `dpkits-1.2.4/src/dpkits.egg-info/PKG-INFO` & `dpkits-1.2.5/src/dpkits.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dpkits
-Version: 1.2.4
+Version: 1.2.5
 Summary: A small package for data processing
 Author-email: Hung Dao <hung.daotuan.1991@gmail.com>
 Project-URL: Homepage, https://github.com/HungDaoHD/packaging_dpkits
 Project-URL: Bug Tracker, https://github.com/HungDaoHD/packaging_dpkits/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

