# Comparing `tmp/daffodil-0.4.4.tar.gz` & `tmp/daffodil-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "daffodil-0.4.4.tar", last modified: Thu May  2 22:45:27 2024, max compression
+gzip compressed data, was "daffodil-0.5.0.tar", last modified: Thu May 23 20:05:01 2024, max compression
```

## Comparing `daffodil-0.4.4.tar` & `daffodil-0.5.0.tar`

### file list

```diff
@@ -1,26 +1,28 @@
-drwxrwxrwx   0        0        0        0 2024-05-02 22:45:27.187680 daffodil-0.4.4/
--rw-rw-rw-   0        0        0     1090 2024-02-28 17:20:31.000000 daffodil-0.4.4/LICENSE
--rw-rw-rw-   0        0        0    54019 2024-05-02 22:45:27.185680 daffodil-0.4.4/PKG-INFO
--rw-rw-rw-   0        0        0    53364 2024-05-01 01:35:13.000000 daffodil-0.4.4/README.md
--rw-rw-rw-   0        0        0      819 2024-05-02 22:41:23.000000 daffodil-0.4.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-02 22:45:27.188679 daffodil-0.4.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-02 22:45:27.111715 daffodil-0.4.4/src/
-drwxrwxrwx   0        0        0        0 2024-05-02 22:45:27.136681 daffodil-0.4.4/src/daffodil/
--rw-rw-rw-   0        0        0        4 2024-05-02 03:32:58.000000 daffodil-0.4.4/src/daffodil/__init__.py
--rw-rw-rw-   0        0        0   201066 2024-05-02 22:40:46.000000 daffodil-0.4.4/src/daffodil/daf.py
-drwxrwxrwx   0        0        0        0 2024-05-02 22:45:27.173681 daffodil-0.4.4/src/daffodil/lib/
--rw-rw-rw-   0        0        0        4 2024-05-02 03:32:58.000000 daffodil-0.4.4/src/daffodil/lib/__init__.py
--rw-rw-rw-   0        0        0    43220 2024-05-02 16:49:22.000000 daffodil-0.4.4/src/daffodil/lib/daf_indexing.py
--rw-rw-rw-   0        0        0    31645 2024-05-02 16:49:22.000000 daffodil-0.4.4/src/daffodil/lib/daf_md.py
--rw-rw-rw-   0        0        0     7708 2024-05-02 16:49:22.000000 daffodil-0.4.4/src/daffodil/lib/daf_pandas.py
--rw-rw-rw-   0        0        0     5174 2024-05-02 03:32:58.000000 daffodil-0.4.4/src/daffodil/lib/daf_types.py
--rw-rw-rw-   0        0        0    51696 2024-05-02 22:19:24.000000 daffodil-0.4.4/src/daffodil/lib/daf_utils.py
--rw-rw-rw-   0        0        0     5796 2024-05-02 03:32:58.000000 daffodil-0.4.4/src/daffodil/lib/md_demo.py
-drwxrwxrwx   0        0        0        0 2024-05-02 22:45:27.180680 daffodil-0.4.4/src/daffodil.egg-info/
--rw-rw-rw-   0        0        0    54019 2024-05-02 22:45:27.000000 daffodil-0.4.4/src/daffodil.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      482 2024-05-02 22:45:27.000000 daffodil-0.4.4/src/daffodil.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-02 22:45:27.000000 daffodil-0.4.4/src/daffodil.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2024-05-02 22:45:27.000000 daffodil-0.4.4/src/daffodil.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-02 22:45:27.000000 daffodil-0.4.4/src/daffodil.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-02 22:45:27.176684 daffodil-0.4.4/tests/
--rw-rw-rw-   0        0        0   164684 2024-05-02 16:49:22.000000 daffodil-0.4.4/tests/test_daf.py
+drwxrwxrwx   0        0        0        0 2024-05-23 20:05:01.763474 daffodil-0.5.0/
+-rw-rw-rw-   0        0        0     1090 2024-02-28 17:20:31.000000 daffodil-0.5.0/LICENSE
+-rw-rw-rw-   0        0        0    54140 2024-05-23 20:05:01.759474 daffodil-0.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0    53485 2024-05-23 19:59:10.000000 daffodil-0.5.0/README.md
+-rw-rw-rw-   0        0        0      819 2024-05-23 19:55:35.000000 daffodil-0.5.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-23 20:05:01.763474 daffodil-0.5.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-23 20:05:01.709478 daffodil-0.5.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-23 20:05:01.724471 daffodil-0.5.0/src/daffodil/
+-rw-rw-rw-   0        0        0        4 2024-05-02 03:32:58.000000 daffodil-0.5.0/src/daffodil/__init__.py
+-rw-rw-rw-   0        0        0   221370 2024-05-23 19:58:46.000000 daffodil-0.5.0/src/daffodil/daf.py
+-rw-rw-rw-   0        0        0    10430 2024-05-15 18:08:46.000000 daffodil-0.5.0/src/daffodil/keyedlist.py
+drwxrwxrwx   0        0        0        0 2024-05-23 20:05:01.750476 daffodil-0.5.0/src/daffodil/lib/
+-rw-rw-rw-   0        0        0        4 2024-05-02 03:32:58.000000 daffodil-0.5.0/src/daffodil/lib/__init__.py
+-rw-rw-rw-   0        0        0    43214 2024-05-15 19:07:31.000000 daffodil-0.5.0/src/daffodil/lib/daf_indexing.py
+-rw-rw-rw-   0        0        0    31645 2024-05-02 16:49:22.000000 daffodil-0.5.0/src/daffodil/lib/daf_md.py
+-rw-rw-rw-   0        0        0     7708 2024-05-02 16:49:22.000000 daffodil-0.5.0/src/daffodil/lib/daf_pandas.py
+-rw-rw-rw-   0        0        0     5174 2024-05-02 03:32:58.000000 daffodil-0.5.0/src/daffodil/lib/daf_types.py
+-rw-rw-rw-   0        0        0    51588 2024-05-20 23:41:53.000000 daffodil-0.5.0/src/daffodil/lib/daf_utils.py
+-rw-rw-rw-   0        0        0     5796 2024-05-02 03:32:58.000000 daffodil-0.5.0/src/daffodil/lib/md_demo.py
+drwxrwxrwx   0        0        0        0 2024-05-23 20:05:01.757474 daffodil-0.5.0/src/daffodil.egg-info/
+-rw-rw-rw-   0        0        0    54140 2024-05-23 20:05:01.000000 daffodil-0.5.0/src/daffodil.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      532 2024-05-23 20:05:01.000000 daffodil-0.5.0/src/daffodil.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 20:05:01.000000 daffodil-0.5.0/src/daffodil.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2024-05-23 20:05:01.000000 daffodil-0.5.0/src/daffodil.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-23 20:05:01.000000 daffodil-0.5.0/src/daffodil.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-23 20:05:01.754505 daffodil-0.5.0/tests/
+-rw-rw-rw-   0        0        0   164590 2024-05-15 19:07:31.000000 daffodil-0.5.0/tests/test_daf.py
+-rw-rw-rw-   0        0        0     2202 2024-05-09 16:48:49.000000 daffodil-0.5.0/tests/test_keyedlist.py
```

### Comparing `daffodil-0.4.4/LICENSE` & `daffodil-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `daffodil-0.4.4/PKG-INFO` & `daffodil-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: daffodil
-Version: 0.4.4
+Version: 0.5.0
 Summary: Daffodil provides lightweight and fast 2-D dataframes
 Author-email: Ray Lutz <raylutz@cognisys.com>
 License: MIT
 Project-URL: Homepage, https://github.com/raylutz/daffodil
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -32,15 +32,16 @@
 as these design tradeoffs are being evaluated and the final initial design resolved. Please see GitHub issues to
 weigh in on the design.
 
 ## Data Model
 The Daffodil data model is really very simple. The core array is a list-of-lists (lol), optionally with one or two associated
 dictionaries, one for the column names and one for row keys.
 
-![pydf_table](https://github.com/raylutz/daffodil/assets/14955977/05c54a27-8d8e-47b6-ae73-957709a5d398)
+![image](https://github.com/raylutz/daffodil/assets/14955977/fa33237c-2075-4bbe-81e1-a6c1e324f46a)
+
 
 Daffodil uses standard python data types, and can mix data types in rows and columns, and can store any type 
 within a cell, even another Daffodil instance. 
 
 It works well in traditional Pythonic processing paradigms, such as in loops, allowing fast row appends, 
 insertions and other operations that column-oriented packages like Pandas handle poorly or don't offer at all.
 Selecting, inserting, appending rows does not make a copy of the data but uses references the way 
@@ -329,15 +330,15 @@
 
        
 ## Common Usage Pattern
        
 One common usage pattern allows iteration over the rows and appending to another Daf instance. For example:
     
         # read csv file into 2-D array, handling column headers, respecting data types and unflattening
-        my_daf = Daf.from_csv(file_path).apply_dtypes(my_daf_dtypes)
+        my_daf = Daf.from_csv(file_path).apply_dtypes(dtypes=my_daf_dtypes)
     
         # create a new (empty) table to be built as we scan the input.
         new_daf = Daf()
         
         # scan the input my_daf row by row and construct the output. Pandas can't do this efficiently.
         for original_row in my_daf:  
             new_row = transform_row(original_row)
@@ -346,23 +347,23 @@
             # here the column names are initialized as the first dictionary is appended.
             
         # create a flat csv file with any python objects flattened using JSON.
         new_daf.flatten().to_csv(file_path)        
 
 This common pattern can be abbreviated using the apply() method:
 
-        my_daf = Daf.from_csv(file_path).apply_dtypes(my_daf_dtypes)
+        my_daf = Daf.from_csv(file_path).apply_dtypes(dtypes=my_daf_dtypes)
         
         new_daf = my_daf.apply(transform_row)
         
         new_daf.flatten().to_csv(file_path)
 
 Or
 
-        Daf.from_csv(file_path).apply_dtypes(my_daf_dtypes).apply(transform_row).flatten().to_csv(file_path)
+        Daf.from_csv(file_path).apply_dtypes(dtypes=my_daf_dtypes).apply(transform_row).flatten().to_csv(file_path)
 
 And further extension of this pattern can apply the transformation to a set of csv files described by a chunk_manifest.
 The chunk manifest essentially provides metadata and instructions for accessing the source data, which may be many 1000s
 of chunks, each of which will fit in memory.
 
         chunk_manifest_daf = Daf.from_csv(file_path)  
         result_manifest_daf = chunk_manifest_daf.manifest_apply(transform_row)
@@ -524,25 +525,26 @@
 #### return list of row keyfield values, if keyfield is defined.
 
     my_daf.keys()    
     
 ### Indexing: inspecting values in a daf array
 
 Daffodil offers easy-to-used indexing of rows, columns, individual cells or any ranges.
-Will generally return the simplest type possible, such as cell contents, a list or daf if retmode == 'val'
-otherwise, if retmode == 'obj', then a full daf object is returned.
+if retmode == 'val', then it will generally return the simplest type possible, such as cell contents, a list or daf 
+otherwise, if retmode == 'obj', then a full daf object is returned. If you desired a list or dict, then it is 
+convenient to just use the .to_list() or .to_dict() methods.
 
 if retmode is 'val':
 - if only one cell is selected, return a single value.
 - If only one row is selected, return a list.
 - if only one col is selected, return a list.
 - if multiple columns are specified, they will be returned in the original orientation in a consistent daf instance copied from the original, and with the data specified.
 
 Please note: operations on columns is relatively inefficient. Try to avoid working on one column at a time.
-Instead, use .apply() or .reduce() and handle any manipulations of all columns at the same time, and select them with the cols parameter at that time.
+Instead, use .apply() or .reduce() and handle any manipulations without dropping columns, and select them with the cols parameter at that time.
 
       `my_daf[2, 3]`     -- select cell at row 2, col 3 and return value.
       `my_daf[2]`        -- select row 2, including all columns, return a list.
       `my_daf[2, :]`     -- same as above
       `my_daf[-1, :]`    -- select the last row
       `my_daf[:5]`       -- select first 5 rows; like `head()` in other dataframe packages.
       `my_daf[:-5]`      -- select last 5 rows; like `tail()` in other dataframe packages.
@@ -631,19 +633,19 @@
     my_daf.append(other_daf)    
 
 
 ### selecting and removing records by keys
 
 #### select one record using keyfield.
 
-    record_da = my_daf.select_record_da(keyvalue)
+    record = my_daf.select_record(keyvalue)
     
 or
 
-   record_list = my_daf[keyvalue].to_dict()
+    record_list = my_daf[keyvalue].to_list()
    
 Note that this syntax differs from Pandas, which normally references a column if square brackets are used with no other
 syntax.
 
 #### select multiple records using the keyfield and return a daf.
 
     new_daf = my_daf[keyvalue_list]
```

### Comparing `daffodil-0.4.4/README.md` & `daffodil-0.5.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,16 @@
 as these design tradeoffs are being evaluated and the final initial design resolved. Please see GitHub issues to
 weigh in on the design.
 
 ## Data Model
 The Daffodil data model is really very simple. The core array is a list-of-lists (lol), optionally with one or two associated
 dictionaries, one for the column names and one for row keys.
 
-![pydf_table](https://github.com/raylutz/daffodil/assets/14955977/05c54a27-8d8e-47b6-ae73-957709a5d398)
+![image](https://github.com/raylutz/daffodil/assets/14955977/fa33237c-2075-4bbe-81e1-a6c1e324f46a)
+
 
 Daffodil uses standard python data types, and can mix data types in rows and columns, and can store any type 
 within a cell, even another Daffodil instance. 
 
 It works well in traditional Pythonic processing paradigms, such as in loops, allowing fast row appends, 
 insertions and other operations that column-oriented packages like Pandas handle poorly or don't offer at all.
 Selecting, inserting, appending rows does not make a copy of the data but uses references the way 
@@ -310,15 +311,15 @@
 
        
 ## Common Usage Pattern
        
 One common usage pattern allows iteration over the rows and appending to another Daf instance. For example:
     
         # read csv file into 2-D array, handling column headers, respecting data types and unflattening
-        my_daf = Daf.from_csv(file_path).apply_dtypes(my_daf_dtypes)
+        my_daf = Daf.from_csv(file_path).apply_dtypes(dtypes=my_daf_dtypes)
     
         # create a new (empty) table to be built as we scan the input.
         new_daf = Daf()
         
         # scan the input my_daf row by row and construct the output. Pandas can't do this efficiently.
         for original_row in my_daf:  
             new_row = transform_row(original_row)
@@ -327,23 +328,23 @@
             # here the column names are initialized as the first dictionary is appended.
             
         # create a flat csv file with any python objects flattened using JSON.
         new_daf.flatten().to_csv(file_path)        
 
 This common pattern can be abbreviated using the apply() method:
 
-        my_daf = Daf.from_csv(file_path).apply_dtypes(my_daf_dtypes)
+        my_daf = Daf.from_csv(file_path).apply_dtypes(dtypes=my_daf_dtypes)
         
         new_daf = my_daf.apply(transform_row)
         
         new_daf.flatten().to_csv(file_path)
 
 Or
 
-        Daf.from_csv(file_path).apply_dtypes(my_daf_dtypes).apply(transform_row).flatten().to_csv(file_path)
+        Daf.from_csv(file_path).apply_dtypes(dtypes=my_daf_dtypes).apply(transform_row).flatten().to_csv(file_path)
 
 And further extension of this pattern can apply the transformation to a set of csv files described by a chunk_manifest.
 The chunk manifest essentially provides metadata and instructions for accessing the source data, which may be many 1000s
 of chunks, each of which will fit in memory.
 
         chunk_manifest_daf = Daf.from_csv(file_path)  
         result_manifest_daf = chunk_manifest_daf.manifest_apply(transform_row)
@@ -505,25 +506,26 @@
 #### return list of row keyfield values, if keyfield is defined.
 
     my_daf.keys()    
     
 ### Indexing: inspecting values in a daf array
 
 Daffodil offers easy-to-used indexing of rows, columns, individual cells or any ranges.
-Will generally return the simplest type possible, such as cell contents, a list or daf if retmode == 'val'
-otherwise, if retmode == 'obj', then a full daf object is returned.
+if retmode == 'val', then it will generally return the simplest type possible, such as cell contents, a list or daf 
+otherwise, if retmode == 'obj', then a full daf object is returned. If you desired a list or dict, then it is 
+convenient to just use the .to_list() or .to_dict() methods.
 
 if retmode is 'val':
 - if only one cell is selected, return a single value.
 - If only one row is selected, return a list.
 - if only one col is selected, return a list.
 - if multiple columns are specified, they will be returned in the original orientation in a consistent daf instance copied from the original, and with the data specified.
 
 Please note: operations on columns is relatively inefficient. Try to avoid working on one column at a time.
-Instead, use .apply() or .reduce() and handle any manipulations of all columns at the same time, and select them with the cols parameter at that time.
+Instead, use .apply() or .reduce() and handle any manipulations without dropping columns, and select them with the cols parameter at that time.
 
       `my_daf[2, 3]`     -- select cell at row 2, col 3 and return value.
       `my_daf[2]`        -- select row 2, including all columns, return a list.
       `my_daf[2, :]`     -- same as above
       `my_daf[-1, :]`    -- select the last row
       `my_daf[:5]`       -- select first 5 rows; like `head()` in other dataframe packages.
       `my_daf[:-5]`      -- select last 5 rows; like `tail()` in other dataframe packages.
@@ -612,19 +614,19 @@
     my_daf.append(other_daf)    
 
 
 ### selecting and removing records by keys
 
 #### select one record using keyfield.
 
-    record_da = my_daf.select_record_da(keyvalue)
+    record = my_daf.select_record(keyvalue)
     
 or
 
-   record_list = my_daf[keyvalue].to_dict()
+    record_list = my_daf[keyvalue].to_list()
    
 Note that this syntax differs from Pandas, which normally references a column if square brackets are used with no other
 syntax.
 
 #### select multiple records using the keyfield and return a daf.
 
     new_daf = my_daf[keyvalue_list]
```

### Comparing `daffodil-0.4.4/pyproject.toml` & `daffodil-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "daffodil"
-version = "0.4.4"
+version = "0.5.0"
 authors = [
     {name = "Ray Lutz", email = "raylutz@cognisys.com"},
 ]
 description = "Daffodil provides lightweight and fast 2-D dataframes"
 readme = "README.md"
 requires-python = ">=3.6"
```

### Comparing `daffodil-0.4.4/src/daffodil/daf.py` & `daffodil-0.5.0/src/daffodil/daf.py`

 * *Files 3% similar despite different names*

```diff
@@ -87,16 +87,16 @@
                 set_keyfield()
                 daf_utils.is_d1_in_d2()
                 improved set_cols() to test sanitize_cols flag.
                 .len(), num_cols(), shape(), len()
                 row_idx_of()   (REMOVE!)
                 remove_key -- keyfield not set. (remove)
                 get_existing_keys
-                select_record_da -- row_idx >= len(self.lol)
-                _basic_get_record_da -- no hd, include_cols
+                select_record -- row_idx >= len(self.lol)
+                _basic_get_record -- no hd, include_cols
                 select_first_row_by_dict    
                 select_where_idxs
                 select_cols
                 calc_cols
                     no hd defined.
                     include_cols > 10
                     exclude_cols > 10
@@ -189,23 +189,55 @@
             Lambdas now importing daffodil
 
     v0.4.4  (2024-05-02)
             Improved unflattening to handle f-string type flattening, including tuples.
             fixed bug in set_dtypes()
             added daf_utils.safe_eval()
             
-            
+    v0.5.0  (2024-05-23)
+            Added split_where(self, where: Callable) which makes a single pass and splits the daf array in two
+                true_daf, false_daf.
+            Added to Daffodil multi_groupby(), reduce_dodaf_to_daf() and multi_groupby_reduce()
+            Added class KeyedList() to provide a new data item that functions like a dict but is a dex plus list.
+                can result in much better performance by not redistributing values in the dict structure.
+                This is not yet integrated into daffodil, but should be.
+                
+            Removed '_da' from many Daffodil methods and for keyword parameters, to allow future upgrade to KeyList.
+                select_record_da()      -> select_record()
+                record_append()
+                _basic_get_record_da    -> _basic_get_record
+                assign_record_da()      -> assign_record()
+                assign_record_da_irow   -> assign_record_irow
+                update_by_keylist()
+                update_record_da_irow   -> update_record_irow
+            changed test_daf accordingly.
+                
+            Added _build_hd() to consistently build header dict structure.
+            Added to_json() and from_json() methods to allow generation of custom JSONEncoder.
+            Changed nomenclature in KeyedList class from dex to hd.
+            Added from_json and to_json to KeyedList class to allow custom JSONEncoder to be developed.
+            
+            select_record() silently returns {} if self is empty.
+            mark chunks saved to local_mirror if not use_lambdas
+            
+            fixed _itermode vs. itermode.
+            Added .strip() method.
+            correct icols when providing a single str column name, and when column names have more than one character each.
+            Added 'flatten' in '.to_list' method which will combine lol to a single list.
+            Added .num_rows() which will more robustly calculate the number of rows in edge cases.
+            Fix unflattening issue discovered when running edge_test_utils.py.
+            Updated documentation to reflect new approach to dtypes and flattening.
+             
+    v0.5.1  (pending)
+    
             
     TODO
-            Update documentation to reflect new approach to dtypes and flattening.
-            tests: need to add 
-                unflattening f-string formatted str data.
+            add use of pickledjson to express contents of individual cells when not jsonable.
+            tests: need to add
                 __str__ and __repr__
-                .isin <-- keep this?
-                normalize() <-- keep this? (not used)
                 
                 apply_dtypes()
                 from_csv_buff()
                 from_numpy()
                 to_csv_buff()
                 append()  
                     empty data item
@@ -227,15 +259,15 @@
                         len(keys_ls) > 10 and len(self.kd) > 30
                         smaller cases
                 iloc                (remove?)
                     no hd
                 icol_to_la          (remove?)
                     unique
                     omit_nulls
-                assign_record_da          (remove?)
+                assign_record       (remove?)
                     no keyfield defined.
                 update_by_keylist <-- remove?
                 insert_irow()
                 set_col_irows() <-- remove.
                 set_icol()  <-- remove.
                 set_icol_irows() <-- remove.
                 find_replace
@@ -325,96 +357,135 @@
                 clean_numeric_str
                 is_numeric
             daf_indexing
                 many cases
             daf_md
                 not tested at all.
                 
-"""            
+"""     
+
+"""
+    To update the package:
+        1. run all tests and demos to verify validity of the version.
+            in tests:
+                python test_daf.py
+                python test_keyedlist.py
+                python daf_demo.py
+                python daf_benchmarks.py
+        2. Increment version number in pyproject.toml
+        3. build the release
+                python -m build --sdist
+        4. Upload it
+                twine upload dist/*
+                
+        
+"""       
     
     
-#VERSION  = 'v0.4.4'
-#VERSDATE = '2024-05-02'  
+#VERSION  = 'v0.5.0'
+#VERSDATE = '2024-05-23'  
 
 import os
 import sys
 import io
 import csv
 import copy
 import re
+import json
 #import numpy as np
     
 sys.path.append(os.path.dirname(os.path.dirname(os.path.realpath(__file__))))
 
 from daffodil.lib.daf_types import T_ls, T_lola, T_di, T_hllola, T_loda, T_da, T_li, T_dtype_dict, \
-                            T_dola, T_dodi, T_la, T_lota, T_doda, T_buff, T_ds, T_lb, T_rli # , T_df
+                            T_dola, T_dodi, T_la, T_lota, T_doda, T_buff, T_ds, T_lb, T_rli
                      
 import daffodil.lib.daf_utils    as utils
 import daffodil.lib.daf_md       as md
 import daffodil.lib.daf_pandas   as daf_pandas
 
+from daffodil.keyedlist import KeyedList
+
+
 from typing import List, Dict, Any, Tuple, Optional, Union, cast, Type, Callable, Iterable #
 def fake_function(a: Optional[List[Dict[str, Tuple[int,Union[Any, str]]]]] = None) -> Optional[int]:
     return None or cast(int, 0)       # pragma: no cover
 
 T_Pydf = Type['Daf']
 T_Daf = Type['Daf']
+T_dodaf = Dict[str, T_Daf]
+
 logs = utils                # alias
 
 
 class Daf:
     RETMODE_OBJ  = 'obj'
     RETMODE_VAL  = 'val'
     
+    ITERMODE_DICT = 'dict' 
+    ITERMODE_KEYEDLIST = 'keyedlist'
+    
 
     def __init__(self, 
-            lol:        Optional[T_lola]        = None,     # Optional List[List[Any]] to initialize the data array. 
+            lol:        Optional[T_lola]        = None,     # used to initialize the data array.
+            hd:         Optional[T_di]          = None,     # used to initialize the hd array. If used, then cols not needed.
+            kd:         Optional[T_di]          = None,     # used to initialize the kd array if no keyfield is set.
             cols:       Optional[T_ls]          = None,     # Optional column names to use.
             dtypes:     Optional[T_dtype_dict]  = None,     # Optional dtype_dict describing the desired type of each column.
                                                             #   also used to define column names if provided and cols not provided.
             keyfield:   str                     = '',       # A field of the columns to be used as a key.
                                                             # can be set even if columns not set yet.
             name:       str                     = '',       # An optional name of the Daf array.
             use_copy:   bool                    = False,    # If True, make a deep copy of the lol data.
             disp_cols:  Optional[T_ls]          = None,     # Optional list of strings to use for display, if initialized.
-            retmode:    str                     = 'obj'     # default return value
+
+            retmode:    str                     = 'obj',    # default retmode
+            itermode:   str                     = 'dict',   # default itermode, either 'dict' or 'keyedlist'
         ):
         if lol is None:
             lol = []
         if dtypes is None:
             dtypes = {}
         if cols is None:
             cols = []
             
         self.name           = name              # str
         self.keyfield       = keyfield          # str
-        self.hd             = {}                # hd_di
+        
+        if hd is not None:
+            self.hd         = hd                # hd_di
+        else:
+            self.hd         = {}
         
         if use_copy:
             self.lol        = copy.deepcopy(lol)
         else:
             self.lol        = lol
         
-        self.kd             = {}
+        if kd is not None:
+            self.kd         = kd
+        else:
+            self.kd         = {}
+            
         self.dtypes         = dtypes
         
         self.md_max_rows    = 10    # default number of rows when used with __repr__ and __str__
         self.md_max_cols    = 10    # default number of cols when used with __repr__ and __str__
 
-        self._retmode       = retmode      # return mode can be either RETMODE_OBJ or RETMODE_VAL
+        self._retmode       = retmode       # retmode can be either RETMODE_OBJ or RETMODE_VAL
+        self._itermode      = itermode      # itermode can be either ITERMODE_DICT or ITERMODE_KEYEDLIST
 
         # Initialize iterator variables        
         self._iter_index = 0
 
         if not cols:
             if dtypes:
-                # see https://github.com/raylutz/daffodil/issues/6
-                self.hd = dict(zip(dtypes.keys(), range(len(dtypes.keys()))))
-                #self.hd = {col: idx for idx, col in enumerate(dtypes.keys())}
+                self.hd = type(self)._build_hd(dtypes.keys())
         else:
+            if isinstance(cols, str):
+                cols = [cols]
             # cols will be sanitized only if necessary.
             self._cols_to_hd(cols)
             if len(cols) != len(self.hd):
                 cols = utils._sanitize_cols(cols=cols)
                 self._cols_to_hd(cols)
                 if len(cols) != len(self.hd):                
                     import pdb; pdb.set_trace() #temp
@@ -443,56 +514,74 @@
     @retmode.setter
     def retmode(self, new_retmode):
         if new_retmode in [self.RETMODE_OBJ, self.RETMODE_VAL]:
             self._retmode = new_retmode
         else:
             raise ValueError("Invalid retmode")
 
+    @property
+    def itermode(self):
+        return self._itermode
+        
+    @itermode.setter
+    def itermode(self, new_itermode):
+        if new_itermode in [self.ITERMODE_DICT, self.ITERMODE_KEYEDLIST]:
+            self._itermode = new_itermode
+        else:
+            raise ValueError("Invalid itermode")
+
     def __iter__(self):
         self._iter_index = 0
         return self
 
-    def __next__(self) -> Dict[str, int]:
+    def __next__(self) -> Union[Dict[str, int], KeyedList]:
         if self._iter_index < len(self.lol):
-            row_dict = dict(zip(self.hd.keys(), self.lol[self._iter_index]))
-            self._iter_index += 1
-            return row_dict
+            if self._itermode == self.ITERMODE_DICT:
+                row_dict = dict(zip(self.hd.keys(), self.lol[self._iter_index]))
+                self._iter_index += 1
+                return row_dict
+            elif self._itermode == self.ITERMODE_KEYEDLIST:
+                row_klist = KeyedList(self.hd, self.lol[self._iter_index])
+                self._iter_index += 1
+                return row_klist
+            else:
+                raise NotImplementedError
         else:
             self._iter_index = 0
             raise StopIteration
 
     def __bool__(self):
         """ test daf for existance and not empty 
-            test exists in test_daf.py            
+            test exists in test_daf.py 
+
+            if self is a single value, test the value.  # not implemented.
+            
         """
+        # if len(self.lol) == 1 and self.lol[0] == 1:
+            # return bool(self.lol[0][0])
+        
         return bool(self.num_cols())
 
 
     def __len__(self):
         """ Return the number of rows in the Daf instance.
         """
         # unit tested
-        return len(self.lol)
-        
-        
-    def len(self):
-        # unit tested
-
-        return len(self.lol)
+        return self.num_rows()
         
         
     def shape(self):
         """ return the number of rows and cols in the daf data array
             number of columns is based on the first record
         """
         # test exists in test_daf.py
         
         if not len(self): return (0, 0)
         
-        return (len(self.lol), self.num_cols()) 
+        return (self.num_rows(), self.num_cols()) 
         
         
     def __eq__(self, other):
         # test exists in test_daf.py            
 
         if not isinstance(other, Daf):
             return False
@@ -521,38 +610,64 @@
         try:
             result = len(self.lol[0])
         except Exception:
             import pdb; pdb.set_trace() #temp
             pass
         return result
 
+
+    def num_rows(self):
+        # unit tested
+        if not self.lol:
+            return 0
+
+        return len(self.lol)
+        
+        
+    def len(self):
+        return self.num_rows()
+        
+        
     #===========================
     # copying convenience function to mimic pandas syntax.
     
 
     def copy(self, deep: bool=False) -> 'Daf':
     
         if deep:
             return copy.deepcopy(self)
         return copy.copy(self)
         
 
     #===========================
     # column names
+    @staticmethod
+    def _build_hd(keys: Iterable):
+        # it is necessary to rebuild hd whenever it the array or cols is changed.
+        # this is equivalent to:
+        #   {col: idx for idx, col in enumerate(keys)}
+        # but this is substantially faster
+        # see https://github.com/raylutz/daffodil/issues/6
+        # self.hd = {col: idx for idx, col in enumerate(dtypes.keys())}
+        
+        # usage here: self.hd = type(self)._build_hd(keys)
+
+        return dict(zip(keys, range(len(keys))))
+
     def columns(self):
         """ Return the column names 
         """
         # test exists in test_daf.py            
         return list(self.hd.keys())
         
         
     def _cols_to_hd(self, cols: T_ls):
         """ rebuild internal hd from cols provided """
         # see https://github.com/raylutz/daffodil/issues/6
-        self.hd = dict(zip(cols, range(len(cols))))
+        self.hd = type(self)._build_hd(cols)
         #self.hd = {col:idx for idx, col in enumerate(cols)}
         
         
     @staticmethod
     def isin(listlike1: Union[T_da, T_la], listlike2: Union[T_da, T_la]) -> T_lb:
         """ creates a boolean mask (list of bools) for each item in list1 which is in list2
         
@@ -665,15 +780,15 @@
         
         # # from utilities import utils
 
         # for key in defined_cols:
         
             # record_da = utils.set_cols_da(da, defined_cols)
             
-            # self.update_record_da_irow(irow, record_da)
+            # self.update_record_irow(irow, record_da)
             
         # return self
         
 
     def rename_cols(self, from_to_dict: T_ds):
         """ rename columns using the from_to_dict provided. 
             respects dtypes and rebuilds hd
@@ -769,15 +884,15 @@
     @staticmethod
     def _build_kd(col_idx: int, lol: T_lola) -> T_di:
         """ build key dictionary from col_idx col of lol """        
         
         key_col = utils.select_col_of_lol_by_col_idx(lol, col_idx)
 
         # see https://github.com/raylutz/daffodil/issues/6
-        kd = dict(zip(key_col, range(len(key_col))))
+        kd = Daf._build_hd(key_col)
         #kd = {key: index for index, key in enumerate(key_col)}
         return kd
         
         
     # def row_idx_of(self, rowkey: str) -> int:
         # """ return row_idx of key provided or -1 if not able to do it.
         # """
@@ -803,14 +918,23 @@
     # dtypes
     
     def set_dtypes(self, 
             default_type: Type = str, 
             typ_to_cols_dict: Optional[Dict[Type, T_ls]] = None,
             ) -> 'Daf':
             
+        """ set dtypes from default and dol where the key of the dict is the type, 
+            and the list is the column names of that type.
+            Useful if most columns are the same type and there are only a few exceptions.
+            
+            Otherwise, simply set my_daf.dtypes = dtypes dict, and then 
+            apply_dtypes() when reading files and 
+            flatten() when writing.
+        """
+            
         if not self.hd:
             raise NotImplementedError ("self.hd must be defined to use .set_dtypes()")
         
         dtypes = {}
         
         col_to_typ_dict = utils.invert_dol_to_dict(typ_to_cols_dict)
         
@@ -854,20 +978,20 @@
         if not self.lol or not self.lol[0]:
             # this can sometimes happen, no worries.
             return self
             
         # first calculate all columns to consider, that are not str or str and unflatten
         cols = self.hd.keys()
         for col in cols:
-            if isinstance(self.dtypes, dict):
+            if isinstance(self.dtypes, dict):           # this is the normal case, where each column is defined.
                 if col not in self.dtypes:
                     continue
                 desired_type = self.dtypes[col]
             else:
-                desired_type = self.dtypes
+                desired_type = self.dtypes              # only one type is defined.
                 
             if (    desired_type == str and from_str or 
                     desired_type in [list, dict] and not unflatten
                 ):
                 continue
         
             icol = self.hd[col]
@@ -976,15 +1100,15 @@
         # # from utilities import utils
 
         # for irow, da in enumerate(self):
             # record_da = copy.deepcopy(da)
             # for col in cols:
                 # if col in da:
                     # record_da[col] = utils.json_encode(record_da[col])        
-            # self.update_record_da_irow(irow, record_da)        
+            # self.update_record_irow(irow, record_da)        
             
         # return self
     
     
     # def flatten(self):
 
         # if not self or not self.dtypes or not self.hd:
@@ -996,16 +1120,29 @@
             # return self
        
         # self._flatten_cols(cols=flatten_cols)
             
         # return self
         
         
+    def strip(self, chrs: str=' ') -> 'Daf':
+    
+        """ remove leading or trailing characters in the string chrs from each str value in the array.
+            modifies in-place.  Ignores non str values.
+        
+            each character in chrs treated seperately, such as strip('"()') removes quotes and parens.
+        """    
+    
+        for row_la in self.lol:
+            for icol in range(len(row_la)):
+                if isinstance(row_la[icol], str) and row_la[icol]:
+                    row_la[icol] = row_la[icol].strip(chrs)
 
-
+        return self
+       
 
     def _safe_tofloat(val: Any) -> Union[float, str]:
         try:
             return float(val)
         except ValueError:
             return 0.0
     
@@ -1019,15 +1156,15 @@
             if lol is provided, it is used in the new Daf.
          """
         if self is None:
             return Daf()
             
         new_cols = cols if cols else self.columns()
         
-        new_daf = Daf(cols=new_cols, lol=lol, keyfield=self.keyfield, dtypes=copy.deepcopy(self.dtypes))
+        new_daf = Daf(cols=new_cols, lol=lol, keyfield=self.keyfield, dtypes=copy.copy(self.dtypes))
         
         return new_daf
         
         
     def set_lol(self, new_lol: T_lola) -> 'Daf':
         """ set the lol with the value passed, leaving other settings, 
             and recalculating kd if required (i.e. if keyfield is defined).
@@ -1293,15 +1430,15 @@
             ) -> 'Daf':
         """ read excel file from a buffer and convert to daf.
         """
         
         # from utilities import xlsx_utils
 
         csv_buff = utils.xlsx_to_csv(excel_buff)
-
+        
         my_daf  = cls.from_csv_buff(
                         csv_buff, 
                         keyfield    = keyfield,         # field to use as unique key, if not ''
                         dtypes      = dtypes,           # dictionary of types to apply if set.
                         noheader    = noheader,         # if True, do not try to initialize columns in header dict.
                         user_format = user_format,      # if True, preprocess the file and omit comment lines.
                         unflatten   = unflatten,        # unflatten fields that are defined as dict or list.
@@ -1343,14 +1480,16 @@
         
         data_lol = utils.buff_csv_to_lol(csv_buff, user_format=user_format, sep=sep, include_cols=include_cols, dtypes=dtypes)
         
         cols = []
         if not noheader:
             cols = data_lol.pop(0)        # return the first item and shorten the list.
         
+        #breakpoint()
+        
         my_daf = cls(lol=data_lol, cols=cols, keyfield=keyfield, dtypes=dtypes)
         
         # the following will act nicely if there is no dtypes defined.
         my_daf.apply_dtypes(unflatten=unflatten)
    
         return my_daf
     
@@ -1376,14 +1515,16 @@
     def to_csv_buff(
             self, 
             line_terminator: Optional[str]=None,
             include_header: bool=True,
             ) -> T_buff:
         """ this function writes the daf array to a csv buffer, including the header if include_header==True.
             The buffer can be saved to a local file or uploaded to a storage service like s3.
+            
+            Use .flatten() before calling this and use JSON encoding for any objects that are not str, int, float, or bool.
         """
     
         if line_terminator is None:
             line_terminator = '\r\n'
     
         f = io.StringIO(newline = '')           # Use newline='' to ensure consistent line endings
         
@@ -1457,15 +1598,15 @@
            if casting is not possible, it will raise an error.
         
         """
     
         import numpy as np
         return np.array(self.lol)
         
-
+    # DEPRECATED
     @classmethod
     def from_hllola(cls, hllol: T_hllola, keyfield: str='', dtypes: Optional[T_dtype_dict]=None) -> 'Daf':
         """ Create Daf instance from hllola type.
             This is used for all DB. loading.
             test exists in test_daf.py
             
             DEPRECATED
@@ -1488,14 +1629,16 @@
         
         Args:
             spreadsheet_id (str): The ID of the Google Sheet.
             
         Returns:
             Daf instance
             
+        # NOT OPERATIONAL
+            
         """
         
         # Set up credentials for the Google Sheets API
         SCOPES = ['https://www.googleapis.com/auth/spreadsheets']
         SERVICE_ACCOUNT_FILE = 'path/to/your/service_account.json'
         
         creds = service_account.Credentials.from_service_account_file(SERVICE_ACCOUNT_FILE, scopes=SCOPES)
@@ -1526,14 +1669,15 @@
         gs_daf = cls(cols=cols, lol=lol)
         
         return gs_daf
         
         
     def to_googlesheet(self, spreadsheet_id: str, sheetname: str = 'Sheet1') -> 'Daf':
         """ export data from daf structure to googlesheet. """
+        # NOT OPERATIONAL
     
         from googleapiclient.discovery import build
         from google.oauth2 import service_account
 
         # Set up credentials for the Google Sheets API
         SCOPES = ['https://www.googleapis.com/auth/spreadsheets']       # this might be okay.
         SERVICE_ACCOUNT_FILE = 'path/to/your/service_account.json'      # probably wrong.
@@ -1570,56 +1714,98 @@
         
         response = response     # fool linter
 
         print('Data successfully written to Google Sheets.')
         
         return self
 
+    #===========================
+    # JSON compatible representation.
+
+    def to_json(self) -> str:
+        # Serialize Daf object to a JSON-compatible dictionary
+        daf_dict = {
+            'name': self.name,
+            'lol': self.lol,
+            'hd': self.hd,
+            'kd': self.kd,
+            'dtypes': self.dtypes,
+            'keyfield': self.keyfield,
+            '_retmode': self._retmode,
+            '_itermode': self._itermode,
+        }
+        # Convert dictionary to JSON string
+        return json.dumps(daf_dict)
+
+    @classmethod
+    def from_json(cls, json_str: str) -> 'Daf':
+        # Deserialize JSON string into a Daf object
+        daf_dict = json.loads(json_str)
+        return cls(lol=daf_dict.get('lol', []),
+                   hd=daf_dict.get('hd', {}),
+                   kd=daf_dict.get('kd', {}),
+                   dtypes=daf_dict.get('dtypes', {}),
+                   keyfield=daf_dict.get('keyfield', ''),
+                   name=daf_dict.get('name', ''),
+                   retmode=daf_dict.get('_retmode', 'obj'),
+                   itermode=daf_dict.get('_itermode', 'dict'))
+
 
     #===========================
     # convert to other format
     
+    # DEPRECATED
     def to_hllola(self) -> T_hllola:
         """ Create hllola from daf 
             test exists in test_daf.py
             
             DEPRECATED
         """    
         return (list(self.hd.keys()), self.lol)
         
     #===========================
     # append
         
-    def append(self, data_item: Union[T_Daf, T_loda, T_da, T_la]):
+    def append(self, data_item: Union[T_Daf, T_loda, T_da, T_la, KeyedList]):
         """ general append method can handle appending one record as T_da or T_la, many records as T_loda or T_daf
             if the data item is None or empty, do not append.
         """
         # test exists in test_daf.py for all three cases
         
         if not data_item:
             return self
         
-        if isinstance(data_item, dict):
+        if isinstance(data_item, (dict, KeyedList)):
             self.record_append(data_item)
             
         elif isinstance(data_item, list):
             if isinstance(data_item[0], dict):
                 # lod type
                 self.extend(data_item)
             else:
                 # simple list.
                 if self.hd:
                     # columns are defined, and keyfield might also be defined
                     # create a dict.
                     da = dict(zip(self.hd.keys(), data_item))
-                    self.record_append(da)
+                    self.record_append(da)  # <-- this takes care of respecing the row kd.
                 else:    
                     # no columns defined, therefore just append to lol.
                     self.lol.append(data_item)
                 
+        elif isinstance(data_item, KeyedList):
+            # hd matches.
+            if self.hd == data_item.hd:
+                self.lol.append(data_item.values)        
+                if self.kd and self.keyfield:
+                    self.kd[data_item[self.keyfield]] = len(self.kd)
+            else:
+                da = data_item.to_dict()
+                self.record_append(da)  # <-- this takes care of respecing the row kd.
+                
         elif isinstance(data_item, Daf):  # type: ignore
             self.concat(data_item)
         else:    
             raise RuntimeError    # pragma: no cover
             
         return self
         
@@ -1648,15 +1834,17 @@
             self.kd = other_instance.kd
             self.keyfield = other_instance.keyfield
             self._rebuild_kd()   # only if the keyfield is set.
             return self
             
         # fields must match exactly!
         if self.hd != other_instance.hd:
-            raise KeyError ("keys in daf do not match lod keys")
+            print(f"keys mismatch: daf: ({list(self.hd.keys())}) \nother_instance: ({list(other_instance.hd.keys())})")
+            breakpoint()    # assertion break
+            raise KeyError
         
         # simply append the rows from daf.lol to the end of self.lol
         for idx in range(len(other_instance.lol)):
             rec_la = other_instance.lol[idx]
             self.lol.append(rec_la)
         self._rebuild_kd()   # only if the keyfield is set.
 
@@ -1696,60 +1884,60 @@
             # the following will either append or insert
             # depending on the keyvalue.
             self.record_append(record_da)    
             
         return self            
             
 
-    def record_append(self, record_da: T_da):
+    def record_append(self, record: Union[T_da, KeyedList]):
         """ perform append of one record into daf (T_da is Dict[str, Any]) 
             This directly modifies daf
             if keyfield is '', then insert without respect to the key value
             otherwise, allow only one record per key.
             
             if the daf is empty, it will adopt the structure of record_da.
             Each new append will add to the end of the daf.lol and will
             update the kd.
             
             If the keys in the record_da have a different order, they will
             be reordered and then appended correctly.
         """
             # test exists in test_daf.py
         
-        if not record_da:
+        if not record:
             return self
             
         if not self.lol and not self.hd:
             # new daf, adopt structure of lod.
             # but there is only one header and data is lol
-            # this saves space.
+            # this makes daffodil arrays about 2/3 smaller.
             
             # see https://github.com/raylutz/daffodil/issues/6
-            self.hd = dict(zip(record_da.keys(), range(len(record_da.keys()))))
+            self.hd = type(self)._build_hd(record.keys())
             
             #self.hd = {col_name: index for index, col_name in enumerate(record_da.keys())}
-            self.lol = [list(record_da.values())]
+            self.lol = [list(record.values())]
             self._rebuild_kd()   # only if the keyfield is set.
             return self
             
         # check if fields match exactly.
         reorder = False
-        if list(self.hd.keys()) != list(record_da.keys()):
+        if list(self.hd.keys()) != list(record.keys()):
             reorder = True
         
         if reorder:
             # construct a dict with exactly the cols specified.
             # defaults to '' at this point.
-            rec_la = [record_da.get(col, '') for col in self.hd]
+            rec_la = [record.get(col, '') for col in self.hd]
         else:
-            rec_la = list(record_da.values())
+            rec_la = list(record.values())
             
         if self.keyfield:
             # insert will overwrite any existing key with the same value.
-            keyval = record_da[self.keyfield]
+            keyval = record[self.keyfield]
             
             # the following, see https://github.com/raylutz/daffodil/issues/7
             if keyval in self.kd:
                 self.lol[self.kd[keyval]] = rec_la
             # idx = self.kd.get(keyval, -1)
             # if idx >= 0:
                 # self.lol[idx] = rec_la
@@ -1976,39 +2164,39 @@
         if num_irows == 1 and num_icols == 0:
         
             irow = irows[0]
             
             if isinstance(value, list):
                 self.lol[irow] = value
             elif isinstance(value, dict):
-                self.assign_record_da_irow(irow, record_da=value)
+                self.assign_record_irow(irow, record=value)
             elif isinstance(value, type(self)):
                 self.lol[irow] = value
             else:
                 # set the same value in the row for all columns.
                 self.lol[irow] = [value] * len(self.lol[irow])
                 
         if num_irows == 1 and num_icols == 1:
         
             irow = irows[0]
             icol = icols[0]
             
             if isinstance(value, dict):
-                self.assign_record_da_irow(irow, record_da=value)
+                self.assign_record_irow(irow, record=value)
             else:    
                 self.lol[irow][icol] = value
                 
         elif num_irows > 1 and num_icols == 0:
             
             if isinstance(value, list):
                 for irow in irows:
                     self.lol[irow] = value
             elif isinstance(value, dict):
                 for irow in irows:
-                    self.assign_record_da_irow(irow, record_da=value)
+                    self.assign_record_irow(irow, record=value)
             elif isinstance(value, type(self)):
                 for source_row, irow in enumerate(irows):
                     self.lol[irow] = value[source_row]
             else:
                 # set the same value in the row for all columns.
                 for irow in irows:
                     self.lol[irow] = [value] * len(self.lol[irow])
@@ -2026,15 +2214,15 @@
                         self.lol[irow][icol] = value[source_idx]
                     except Exception:
                         import pdb; pdb.set_trace() #temp
                     
             # elif isinstance(value, dict):
                 # # this is the same as cols=0 bc dict updates the corresponding cols.
                 # for irow in irows:
-                    # self.assign_record_da_irow(irow, record_da=value)
+                    # self.assign_record_irow(irow, record=value)
                 
             elif isinstance(value, type(self)):
                 for source_idx, irow in enumerate(irows):
                     self.lol[irow][icol] = value[source_idx][0]
                 
             else:
                 # set the same value in the row for all selected columns.
@@ -2051,15 +2239,15 @@
                             self.lol[irow][icol] = value[source_col]
                         except Exception:
                             import pdb; pdb.set_trace() #temp
                     
             elif isinstance(value, dict):
                 # this is the same as cols=0 bc dict updates the corresponding cols.
                 for irow in irows:
-                    self.assign_record_da_irow(irow, record_da=value)
+                    self.assign_record_irow(irow, record=value)
                 
             elif isinstance(value, type(self)):
                 for irow in irows:
                     for source_col, icol in enumerate(icols):
                         self.lol[irow][icol] = value[source_col]
                 
             else:
@@ -2158,15 +2346,16 @@
             idxs = []
             for gkey in gkeys:
                 # For the following, see https://github.com/raylutz/daffodil/issues/6
                 try:
                     idxs.append(keydict[gkey])                
                 except KeyError:
                     if not silent_error:
-                        logs.sts(f"{logs.prog_loc()} Cannot find key '{gkey}' in {axis} in dataframe '{name}'", 3) 
+                        logs.sts(f"{logs.prog_loc()} Cannot find key '{gkey}' in {axis} in dataframe '{name}'", 3)
+                        #breakpoint()
                         raise 
                     
             
         elif isinstance(gkeys, slice):     # can be list of integer or strings (or anything hashable)
             gkeys_range = range(gkeys.start or 0, gkeys.stop or len(keydict), gkeys.step or 1)
             idxs = []
             for gkey in gkeys_range:
@@ -2294,15 +2483,15 @@
         
         if isinstance(icols, int):
             # simple single row selection
             icol = icols
             if not flip:
                 col_sliced_lol = [[row[icol]] for row in self.lol]
                 if orig_cols:
-                    sliced_cols = orig_cols[icol]
+                    sliced_cols = [orig_cols[icol]]
             else: # flip
                 col_sliced_lol = [row[icol] for row in self.lol]
             
         elif isinstance(icols, slice):
             slice_spec = icols
             icols_range = range(slice_spec.start or 0, slice_spec.stop or 0, slice_spec.step or 1)
             
@@ -2350,45 +2539,48 @@
         
         return new_daf
     
     #=============================================
     # the following methods might be absorbed into the above.
     #
     
-    def select_record_da(self, key: str, silent_error: bool=True) -> T_da:
+    def select_record(self, key: str, silent_error: bool=True) -> T_da:
         """ Select one record from daf using the key and return as a single T_da dict.
         
-            May be better to simply use 
-            
-                selected_daf = select_krows(krows=key)
-                
-            to select one row from the array, and then use:
-
-                selected_daf[0, 'fieldname']   to select fields like you would when using a dict.
-        
-            test exists in test_daf.py
+            returns {} if not self
+            assertion break if keyfield not defined.
+            if key not found, return {} if silent_error, else raise KeyError exception.
+                   
+            TODO Update for returning KeyedList
         """
         
+        if not self:
+            return {}
+        
         if not self.keyfield:
-            raise RuntimeError
+            logs.sts(f"{logs.prog_loc()} LOGIC ERROR. No keyfield is defined, required for select_record():\n{self}")
+            #breakpoint()    # temp
+            raise RuntimeError ("No keyfield is defined, required for select_record()")
             
         if key in self.kd:
-            return self._basic_get_record_da(self.kd[key])
+            return self._basic_get_record(self.kd[key])
 
         if silent_error:
             return {}
             
         raise KeyError    
 
         
-    def _basic_get_record_da(self, irow: int, include_cols: Optional[T_ls]=None) -> T_da:
+    def _basic_get_record(self, irow: int, include_cols: Optional[T_ls]=None) -> T_da:
         """ return a record at irow as dict 
             include only "include_cols" if it is defined
             note, this requires that hd is defined.
             if no column header exists, this will generate a new one using spreadsheet convention.
+            
+            TODO Update to return KeyedList as an option.
         """
         if not self.hd:
             cols = utils._generate_spreadsheet_column_names_list(num_cols=self.num_cols())
             self.set_cols(cols)
         
         if include_cols:
             return {col:self.lol[irow][self.hd[col]] for col in include_cols if col in self.hd}
@@ -2400,17 +2592,17 @@
         # """ Select multiple records from daf using row indexes and create new daf.
             
         # """
         
         # selected_daf = self.clone_empty()
         
         # for row_idx in irows_li:
-            # record_da = self._basic_get_record_da(row_idx)
+            # record = self._basic_get_record(row_idx)
         
-            # selected_daf.append(record_da)
+            # selected_daf.append(record)
                       
         # return selected_daf
         
         
     def select_records_daf(self, keys_ls: T_ls, inverse:bool=False) -> 'Daf':
         """ Select multiple records from daf using the keys and return as a single daf.
             If inverse is true, select records that are not included in the keys.
@@ -2434,15 +2626,20 @@
 
         if num_rows >= 1 and num_cols >= 1:
             return self.lol[irow][icol]
 
         return default
         
 
-    def to_list(self, irow: Optional[int]=None, icol: Optional[int]=None, unique=False) -> list:
+    def to_list(self, 
+        irow: Optional[int]=None,   # select a row 
+        icol: Optional[int]=None,   # or column.
+        unique=False,               # reduce to unique values
+        flatten=False,              # if items is the list are lists, combine them into one list.
+        ) -> list:
         """ return data from a daf array as a list
             defaults to the most obvious list if irow and icol not specified.
                 from irow 0, if num_rows is 1 and num_cols >= 1
                 from icol 0, if num_rows >= 1 and num_cols == 1
             otherwise, choose irow or icol specified.
                 if irow, specified, ignore icol.
                 if irow=None and icol specified, then use icol.
@@ -2463,14 +2660,23 @@
         elif irow is not None and num_rows:
             result_la = self.lol[irow]
         elif icol and num_cols:
             result_la = self.icol(icol)
         else:
             result_la = []
             
+        if flatten:
+            new_list = []
+            for sublist in result_la:
+                if isinstance(sublist, list):
+                    new_list += sublist
+                else:
+                    new_list += [sublist]
+            result_la = new_list        
+            
         if unique and result_la:
             result_la = list(dict.fromkeys(result_la))
             
         return result_la
 
 
     def to_dict(self, irow: int=0, include_cols: Optional[T_ls]=None) -> T_da:
@@ -2487,21 +2693,23 @@
         """
         return self.iloc(irow, include_cols)
         
 
     def iloc(self, irow: int=0, include_cols: Optional[T_ls]=None) -> T_da:
         """ Select one record from daf using the idx and return as a single T_da dict
             test exists in test_daf.py
+            
+            TODO allow KeyedList return value.
         """
         
         if irow < 0 or irow >= len(self.lol) or not self.lol or not self.lol[irow]:
             return {}
             
         if self.hd: 
-            return self._basic_get_record_da(irow, include_cols)
+            return self._basic_get_record(irow, include_cols)
                 
         colnames = utils._generate_spreadsheet_column_names_list(num_cols=len(self.lol[irow]))
         return dict(zip(colnames, self.lol[irow]))
         
 
     def select_by_dict_to_lod(self, selector_da: T_da, expectmax: int=-1, inverse: bool=False) -> T_loda:
         """ Select rows in daf which match the fields specified in d, returning lod 
@@ -2565,15 +2773,15 @@
         """
         # unit test exists.
 
         result_lol = [list(row.values()) for row in self if where(row)]
 
         daf = Daf(cols=self.columns(), lol=result_lol, keyfield=self.keyfield, dtypes=self.dtypes)
 
-        return daf    
+        return daf
         
 
     def select_where_idxs(self, where: Callable) -> T_li:
         """
         Select rows in Daf based on the provided where condition
         variable 'row' is the current row being evaluated
         and return list of indexes.
@@ -2583,14 +2791,42 @@
         
         """
         # unit test exists.
         
         return [idx for idx, row in enumerate(self) if where(row)]
 
 
+    def split_where(self, where: Callable) -> Tuple['Daf', 'Daf']:
+        """
+        Select rows in Daf based on the provided where condition,
+        and split into two Daf objects, for True and False.
+        
+        Note: this does a shallow copy of the lines and any changes to
+        the split objects will change the original daf object.
+
+        # Example Usage
+        
+            true_daf, false_daf = original_daf.split_where(lambda row: bool(int(row['colname']) > 5))
+        
+        """
+        true_lol = []
+        false_lol = []
+        
+        for idx, row_da in enumerate(self):
+            if where(row_da):
+                true_lol.append(self.lol[idx])
+            else:
+                false_lol.append(self.lol[idx])
+
+        true_daf = Daf(cols=self.columns(), lol=true_lol, keyfield=self.keyfield, dtypes=self.dtypes)
+        false_daf = Daf(cols=self.columns(), lol=false_lol, keyfield=self.keyfield, dtypes=self.dtypes)
+
+        return true_daf, false_daf
+
+
     def col(self, colname: str, unique: bool=False, omit_nulls: bool=False, silent_error:bool=False) -> list:
         """ alias for col_to_la()
             can also use column ranges and then transpose()
             test exists in test_daf.py
         """
         return self.col_to_la(colname, unique, omit_nulls=omit_nulls, silent_error=silent_error)
 
@@ -2737,104 +2973,127 @@
         
         # return Daf(lol=new_lol, cols=new_cols, dtypes=new_dtypes)
         
 
     #=========================
     #   modify records
         
-    def assign_record_da(self, record_da: T_da):
+    def assign_record(self, record: T_da):
         """ Assign one record in daf using the key using a single T_da dict.
+        
+            TODO Upate to accept KeyedList
+        
             unit tests exist
         """
         
         if not self.keyfield:
             raise RuntimeError("No keyfield estabished for daf.")
             
         keyfield = self.keyfield
-        if keyfield not in record_da:
+        if keyfield not in record:
             raise RuntimeError("No keyfield in dict.")
             
-        if self and list(record_da.keys()) != list(self.hd.keys()):
+        if self and list(record.keys()) != list(self.hd.keys()):
             raise RuntimeError("record fields not equal to daf columns")
             
-        keyval = record_da[keyfield]
+        keyval = record[keyfield]
 
         # for the following, see https://github.com/raylutz/daffodil/issues/7
         if keyval in self.kd:
             # assign the record, normalize the fields.
-            self.lol[self.kd[keyval]] = [record_da.get(col, '') for col in self.hd]
+            self.lol[self.kd[keyval]] = [record.get(col, '') for col in self.hd]
         else:
             # otherwise add it.
-            self.append(record_da)
+            self.append(record)
             
         # row_idx = self.kd.get(keyval, -1)
         # if row_idx < 0 or row_idx >= len(self.lol):
             # self.append(record_da)
         # else:
             # #normal_record_da = Daf.normalize_record_da(record_da, cols=self.columns(), dtypes=self.dtypes)   
             # self.lol[row_idx] = [record_da.get(col, '') for col in self.hd]
         
 
-    def assign_record_da_irow(self, irow: int=-1, record_da: Optional[T_da]=None):
+    def assign_record_irow(self, irow: int=-1, record: Optional[T_da]=None):
         """ Assign one record in daf using the iloc using a single T_da dict.
+        
+            TODO Update to accept KeyedList
+        
             unit tests exist
         """
         
-        if record_da is None:
+        if record is None:
             return
         
         if irow < 0 or irow >= len(self.lol):
-            self.append(record_da)
+            self.append(record)
         else:
             #normal_record_da = Daf.normalize_record_da(record_da, cols=self.columns(), dtypes=self.dtypes)   
-            self.lol[irow] = [record_da.get(col, '') for col in self.hd]
+            self.lol[irow] = [record.get(col, '') for col in self.hd]
         
 
-    def update_by_keylist(self, keylist: Optional[T_ls]=None, record_da: Optional[T_da]=None):
-        """ Update selected records in daf by keylist using record_da
+    def update_by_keylist(self, keylist: Optional[T_ls]=None, record: Optional[T_da]=None):
+        """ Update selected records in daf by keylist using record
             only update those columns that have dict keys
             but keep all other dict items intact in that row if not updated.
+            
+            Equivalent to: my_daf[keylist] = record
+            
+            DEPRECATE?
         """
         
-        if record_da is None or not self.lol or not self.hd or not self.keyfield or not keylist:
+        if record is None or not self.lol or not self.hd or not self.keyfield or not keylist:
             return
 
         for key in keylist:
             if key in self.kd:
-                self.update_record_da_irow(self.kd[key], record_da)
+                self.update_record_irow(self.kd[key], record)
             
         
 
-    def update_record_da_irow(self, irow: int=-1, record_da: Optional[T_da]=None):
+    def update_record_irow(self, irow: int=-1, record: Optional[T_da]=None):
         """ Update one record in daf at iloc using a single T_da dict,
             and only update those columns that have dict keys
             but keep all other dict items intact in that row.
+            
+            Equivalent to my_daf[irow] = record
+            
+            DEPRECATE?
+            
+            TODO: Allow record to be KeyedList
+            
             unit tests exist
         """
         
-        if record_da is None or not self.lol or not self.hd:
+        if record is None or not self.lol or not self.hd:
             return
         
         if irow < 0 or irow >= len(self.lol):
             return
         
         # see https://github.com/raylutz/daffodil/issues/7
-        for colname, val in record_da.items():
+        for colname, val in record.items():
             if colname in self.hd:
-                self.lol[irow][self.hd[colname]] = record_da[colname]
+                self.lol[irow][self.hd[colname]] = record[colname]
             # icol = self.hd.get(colname, -1)
             # if icol >= 0:
                 # self.lol[irow][icol] = record_da[colname]
         
 
     def assign_icol(self, icol: int=-1, col_la: Optional[T_la]=None, default: Any=''):
         """ modify icol by index using col_la 
             use default if col_la not long enough to fill all cells.
             Also, if col_la not provided, use default to fill all cells in the column.
             if icol == -1, append column on the right side.
+            
+            Equivalent to  my_daf[:, icol] = col_la
+            
+            Except that icol can be -1 and it will append.
+            DEPRECATE?
+            
         """
         # from utilities import utils
 
         self.lol = utils.assign_col_in_lol_at_icol(icol, col_la, lol=self.lol, default=default)
         
         
         
@@ -2888,14 +3147,18 @@
         self._rebuild_kd()
 
 
     def assign_col(self, colname: str, la: Optional[T_la]=None, default: Any=''):
         """ modify col by colname using la 
             use default if la not long enough.
             test exists in test_daf.py
+            
+            Equivalent to my_daf[:, colname] = la
+            
+            DEPRECATE?
         """
         
         if colname in self.hd:
             self.assign_icol(self.hd[colname], la, default)
         
         return self
 
@@ -2911,14 +3174,15 @@
     def insert_col(
             self, 
             colname: str, 
             col_la: Optional[T_la]=None, 
             icol: int=-1, 
             default: Any='',
             ): #, keyfield:str=''):
+            
         """ add col by colname and set to la at icol
             if la is not long enough for a full column, use the default.
             if colname exists, overwrite it.
             Can use to set a constant value by not passing col_la and setting default.
             use set_keyfield() if this column will become the keyfield.
             unit tested
         """
@@ -2956,35 +3220,55 @@
         num_rows = len(self)
         col_la = list(range(startat, startat + num_rows))
     
         self.insert_col(colname, col_la, icol)
 
 
     def set_col_irows(self, colname: str, irows: T_li, val: Any):
-        """ set a given icol and list of irows to val """
+        """ set a given icol and list of irows to val 
+        
+            Equivalent to my_daf[irows, colname] = val
+            
+            DEPRECATE?
+        
+        """
         
         # see https://github.com/raylutz/daffodil/issues/7
         try:
             icol = self.hd[colname]
         except KeyError:
             return self
 
         self.set_icol_irows(icol, irows, val)
         
         return self
     
 
     def set_icol(self, icol: int, val: Any):
     
+        """ Equivalent to my_daf[:, icol] = val
+        
+            DEPRECATE?
+        """
+    
+    
         for irow in range(len(self.lol)):
             self.lol[irow][icol] = val
+            
+        return self
         
 
     def set_icol_irows(self, icol: int, irows: T_li, val: Any):
-        """ set a given icol and list of irows to val """
+        """ set a given icol and list of irows to val 
+        
+            Equivalent to my_daf[irows, icol] = val
+        
+            DEPRECATE?
+        
+        """
         
         for irow in irows:
             if irow >= len(self.lol) or irow < 0:
                 continue
         
             self.lol[irow][icol] = val        
     
@@ -3030,15 +3314,24 @@
     #=========================
     #   sort
             
     def sort_by_colname(self, colname:str, reverse: bool=False, length_priority: bool=False) -> 'Daf':
         """ sort the data by a given colname, using length priority unless specified.
             sorts in place. Make a copy if you need the original order.
         """
-        colidx = self.hd[colname]
+        if not self:
+            return self
+        
+        try:
+            colidx = self.hd[colname]
+        except Exception as err:
+            print(f"{err}")
+            breakpoint()    # assertion break
+            pass
+            
         self.lol = utils.sort_lol_by_col(self.lol, colidx, reverse=reverse, length_priority=length_priority)
         self._rebuild_kd()
         return self
         
     #=========================
     #   apply formulas
 
@@ -3553,15 +3846,15 @@
             if omit_nulls and fieldval=='':
                 continue
             
             if fieldval not in result_dodaf:
                 result_dodaf[fieldval] = self.clone_empty()
                 
             this_daf = result_dodaf[fieldval]
-            this_daf.record_append(record_da=da)
+            this_daf.record_append(da)
             result_dodaf[fieldval] = this_daf
     
         return result_dodaf
     
 
     def groupby_cols(self, colnames: T_ls) -> Dict[Tuple[str, ...], 'Daf']:
         """ given a daf, break into a number of daf's based on colnames specified. 
@@ -3578,15 +3871,15 @@
             fieldval_tuple = tuple(da[colname] for colname in colnames)
             if fieldval_tuple not in result_dodaf:
                 result_dodaf[fieldval_tuple] = this_daf = self.clone_empty()
             
             else:
                 this_daf = result_dodaf[fieldval_tuple]
                 
-            this_daf.record_append(record_da=da)
+            this_daf.record_append(da)
             result_dodaf[fieldval_tuple] = this_daf
     
         return result_dodaf
 
 
     def groupby_cols_reduce(
             self, 
@@ -3716,66 +4009,205 @@
 
         return result_daf
     
 
     def groupby_reduce(
             self, 
             colname:        str, 
-            func:           Callable[[T_da, T_da], Union[T_da, T_la]], 
+            func:           Callable[['Daf', T_da], Union[T_da, T_la]], # function reduces one grouped daf to one record. 
             by:             str='row',                                  # determines how the func is applied.
             reduce_cols:    Optional[T_la]=None,                        # columns included in the reduce operation.
             diagnose:       bool=False,
             **kwargs:       Any,
             ) -> 'Daf':
         """ given a daf, break into a number of daf's based on colname specified. 
             For each group, apply callable.
             returns daf with one row per group, with keyfield the groupby value in colname.
             
         """
         
         if diagnose:
             logs.sts(f"{logs.prog_loc()} starting groupby '{colname}' operation", 3)
         grouped_dodaf = self.groupby(colname)
+        result_daf = Daf.reduce_dodaf_to_daf(
+            func            = func,             # function reduces one grouped daf to one record. 
+            colname         = colname, 
+            grouped_dodaf   = grouped_dodaf, 
+            reduce_cols     = reduce_cols,
+            by              = by,
+            diagnose        = diagnose,
+            **kwargs,
+            )
+        return result_daf
+        
+    
+    def multi_groupby(
+            self, 
+            groupby_colnames: T_ls, 
+            colnames: Optional[T_ls]=None,
+            omit_nulls: bool=False,         # do not group to values in column that are null ('')
+            ) -> Dict[str, Dict[str, 'Daf']]:   # result_dododaf
+            
+        """ given a daf, break into a number of daf's based on a list of colnames specified. 
+            For each groupby_colname, for each discrete value, create a daf table with all cols,
+            including colname, and provide a dodaf structure for each groupby_colname.
+            
+            Please note that each daf array which is built the value of each colname is not reduced.
+            
+            {groupby_colname1:
+                {value1: Daf,
+                 value2: Daf,
+                 ...
+                 valuen: Daf,
+                }
+             groupby_colname2:
+                {value1: Daf,
+                 value2: Daf,
+                 ...
+                 valuen: Daf,
+                }
+            ...
+            }
+            
+        """
+        if isinstance(groupby_colnames, str):
+            groupby_colnames = [groupby_colnames]
+        
+        result_dododaf: Dict[str, Dict[str, 'Daf']] = {}
+        
+        # the following makes a single pass through Daf array, and
+        # allocates the record to one daf for each colname, for each colvalue.
+        # these daf arrays are not reduced here.
+        
+        # (TODO this loop would be better to iterate through list items rather than dicts.)
+        
+        for da in self:
+            for col in groupby_colnames:
+                if col not in result_dododaf:
+                    result_dododaf[col] = {}
+            
+                fieldval = da[col]
+                if omit_nulls and fieldval=='':
+                    continue
+            
+                if fieldval not in result_dododaf[col]:
+                    result_dododaf[col][fieldval] = self.clone_empty()
+                
+                this_daf = result_dododaf[col][fieldval]
+                this_daf.record_append(da)
+                result_dododaf[col][fieldval] = this_daf
+    
+        return result_dododaf
+        
+    
+
+    @staticmethod
+    def reduce_dodaf_to_daf(
+            colname:        str, 
+            func:           Callable[[T_da, T_da], Union[T_da, T_la]], 
+            grouped_dodaf:  T_dodaf, 
+            reduce_cols:    Optional[T_la]=None,    # columns included in the reduce operation, None = all except for colname.
+            diagnose:       bool=False,
+            **kwargs:       Any,
+            ) -> 'Daf':
+        """ after splitting a daf into a number of mutually exclusive daf objects based on the value in colname,
+            combine these using reduction function func, resulting in a single record for each Daf array.
+            Then append these records into the resulting Daf array, containing one record per value in column 'colname'
+            Other than columns specified in 'reduce_cols', other columns are '' unless they are single-valued.
+        """
         
         if diagnose:
             logs.sts(f"{logs.prog_loc()} Grouped into {len(grouped_dodaf)} groups.", 3)
             
+            # display the first three daf arrays and the last
+            
             for group_num, (colval, this_daf) in enumerate(grouped_dodaf.items()):
                 if group_num < 3 or group_num >= len(grouped_dodaf) - 1:
                     logs.sts(f"## Group {group_num}: {colname}={colval}\n\n{this_daf}\n\n", 3)
             
         
         result_daf = Daf(keyfield = colname)
         
         for group_num, (colval, this_daf) in enumerate(grouped_dodaf.items()):
         
             # maybe remove colname from cols here
         
             if diagnose:
                 logs.sts(f"## Group {group_num}: {colname}={colval}\n\n{this_daf}\n\n", 3)
-            reduction_da = this_daf.reduce(func, by=by, cols=reduce_cols, **kwargs)
+            reduction_da = this_daf.reduce(func, cols=reduce_cols, **kwargs)
+                    # def reduce(
+                            # self, 
+                            # func: Callable[[T_da, T_da], Union[T_da, T_la]], 
+                            # by: str='row', 
+                            # cols: Optional[Iterable]=None,                  # columns included in the reduce operation.
+                            # initial_da: Optional[T_da]=None,
+                            # **kwargs: Any,
+                            # ) -> Union[T_da, T_la]:
             
             if diagnose:
                 logs.sts(f"Post reduction: {Daf.from_lod([reduction_da])=}", 3)
             
-            # add colname:colval to the dict
-            reduction_da = {colname: colval, **reduction_da}
+            # add colname:colval to the dict, as it is removed by the reduction func.
+            reduction_da[colname] = colval
             
             if diagnose:
                 logs.sts(f"Post add colname:colval to the dict: {Daf.from_lod([reduction_da])=}", 3)
 
             # this will also maintain the kd.
             result_daf.append(reduction_da)
 
         if diagnose:
             logs.sts(f"{logs.prog_loc()} result_daf:\n\n{result_daf}", 3)
 
         return result_daf
 
         
+    def multi_groupby_reduce(
+            self, 
+            colnames:       T_ls, 
+            func:           Callable[[T_da, T_da], Union[T_da, T_la]],  # function reduces one grouped daf to one record.
+            by:             str='row',                                  # determines how the func is applied.
+            reduce_cols:    Optional[T_la]=None,                        # columns included in the reduce operation.
+            diagnose:       bool=False,
+            **kwargs:       Any,
+            ) -> Dict[str, 'Daf']:
+        """ given a daf, break into a number of daf's based on colnames specified. 
+            For each group, apply callable.
+            returns dodaf with one daf per colname.
+            In each of those dafs, there is row per value in the colname, with keyfield the groupby value in colname.
+        """
+        
+        if diagnose:
+            logs.sts(f"{logs.prog_loc()} starting multi-groupby '{colnames}' operation", 3)
+        multi_grouped_dododaf = self.multi_groupby(colnames)
+        
+        result_dodaf: T_dodaf = {}
+        
+        for colname, grouped_dodaf in multi_grouped_dododaf.items():
+        
+            result_dodaf[colname] = Daf.reduce_dodaf_to_daf(
+                func            = func,         # function reduces one grouped daf to one record.
+                colname         = colname, 
+                grouped_dodaf   = grouped_dodaf, 
+                reduce_cols     = reduce_cols,
+                diagnose        = diagnose,
+                **kwargs,
+                )
+        if diagnose:
+            logs.sts(f"{logs.prog_loc()} Grouped into {len(result_dodaf)} groups.", 3)
+            
+            for group_num, (colval, this_daf) in enumerate(result_dodaf.items()):
+                if group_num < 3 or group_num >= len(grouped_dodaf) - 1:
+                    logs.sts(f"## Group {group_num}: {colname}={colval}\n\n{this_daf}\n\n", 3)
+
+        return result_dodaf
+        
+        
+            
+        
     #===================================
     # apply / reduce convenience methods
 
     # def daf_sum(
             # self, 
             # by: str = 'row', 
             # cols: Optional[T_la]=None,
@@ -3912,26 +4344,33 @@
                 
             #allcols = self.hd.keys()
 
             if cols is None:
                 cols_iter = self.hd.keys()
             elif isinstance(cols, str):
                 cols_iter = [cols]
-            elif isinstance(cols, list) and len(cols) > 10:    
-                cols_iter = dict.fromkeys(cols)
+            # elif isinstance(cols, list) and len(cols) > 10:    
+                # cols_iter = dict.fromkeys(cols)
             else:
-                cols_iter = cols
-                
+                cols_iter = {col: None for col in self.hd.keys() if col in cols}
+                           
             if initial_da:
                 reduction_da = initial_da
             else:
                 reduction_da = dict.fromkeys(cols_iter, 0)
     
             for row_da in self:
-                reduction_da = func(row_da, reduction_da, cols_iter, **kwargs)
+                try:
+                    reduction_da = func(row_da, reduction_da, cols_iter, **kwargs)
+                except Exception as err:
+                    print(f"err = {err}")
+                    breakpoint()    # perm: investigate why reduction function not working
+                    pass
+                # def count_values_da(row_da: T_da, reduction_da: T_da, cols_iter: Iterable, omit_nulls: bool=False) -> T_dodi:
+                # def sum_da         (row_da: T_da, reduction_da: T_da, cols_iter: Iterable, astype: Optional[Type]=None, diagnose:bool=False
 
             # normalize the result so it contains all columns
             result_da = {key: reduction_da.get(key,'') for key in self.hd.keys()}
                 
             return result_da    
                 
         elif by == 'col':
@@ -3944,32 +4383,35 @@
 
         else:
             raise NotImplementedError
         return [] # for mypy only.
         
         
     @staticmethod
-    def sum_da(row_da: T_da,                   # the current row from the daf array.
-                accum_da: T_da,                 # an accumulated result. Must be initialized for all columns in cols.
-                cols: Iterable,                 # defines the active columns. Can be a list, keys(), range, or slice
+    def sum_da( row_da: T_da,                   # the current row from the daf array.
+                reduction_da: T_da,             # an accumulated result. Must be initialized for all columns in cols.
+                cols_iter: Iterable,            # defines the active columns. Can be a list, keys(), range, or slice
+                *,
                 astype: Optional[Type]=None,    # a type like int, float, str to cast the value if it is not that type. Optional.
                 diagnose:bool=False
                 ) -> T_da:     # result_da
         """ sum values in row and accum dicts per colunms provided. 
             will safely skip data that can't be summed.
+            First three args should be provided by position only to avoid naming issues among different reductions.
         """
+        # def sum_da         (row_da: T_da, reduction_da: T_da, cols_iter: Iterable, astype: Optional[Type]=None, diagnose:bool=False
 
         diagnose = diagnose
         #nan_indicator = ''
 
         # for col, value in row_da.items():       # doing it this way requires a check for existence in each loop.
             # if col not in cols:                 # this check is not needed in the version below.
                 # continue                        # 251 vs 207.
 
-        for col in cols:
+        for col in cols_iter:
             
             # if value == nan_indicator:        # this makes the loop take 10x longer (2162) (1044% of original)
             # if isinstance(value, str):        # this makes the loop take 42% longer (294)
             # if isinstance(value, str) and value == '':  # same (294)
             # if value is None or isinstance(value, str) and not value:     (350) vs 207 = 69% longer
             # if value == '':                     # this makes the loop take 10x longer (2105) (1044% of original)
             # if isinstance(value, str) and not value:    # this makes the loop take 50% longer (305)
@@ -4025,29 +4467,29 @@
                     if astype==int and isinstance(value, (str, float, bool)):
                         value = int(float(value or 0))
                     elif astype==float and isinstance(value, (str, int, bool)):    
                         value = float(value or 0)
                     elif astype==str and isinstance(value, (float, int, bool)):
                         value = str(value)
                     
-                    accum_da[col] += value
+                    reduction_da[col] += value
             
                 except Exception:
                     continue
                     
             else:
                 try:
-                    accum_da[col] += row_da[col]
+                    reduction_da[col] += row_da[col]
                 
                 except Exception:
                         continue
 
 
                 
-        return accum_da
+        return reduction_da
 
         
     @staticmethod
     def sum_da2(row_da: T_da,                   # the current row from the daf array.
                 accum_da: T_da,                 # an accumulated result. Must be initialized for all columns in cols.
                 cols: Iterable,                 # defines the active columns. Can be a list, keys(), range, or slice
                 astype: Optional[Type]=None,    # a type like int, float, str to cast the value if it is not that type. Optional.
@@ -4258,24 +4700,39 @@
             
         return self.reduce(func=type(self).count_values_da, by=by, cols=cols)
 
 
     def groupsum_daf(
             self,
             colname:str, 
-            #func: Callable[[T_da, T_da, Optional[T_la]], Union[T_da, T_la]], 
             by: str='row',                                  # determines how the func is applied.
             reduce_cols: Optional[T_la]=None,               # columns included in the reduce operation.
+            # keyfield: str=colname,                        # provide this for when no keyfield is desired?
+                                                            # current operation sets keyfield to colname.
             ) -> 'Daf':
     
         result_daf = self.groupby_reduce(colname=colname, func=self.__class__.sum_da, by=by, reduce_cols=reduce_cols)
         
         return result_daf
 
 
+    def multi_groupsum(
+            self,
+            colnames: T_ls,                                 # colnames to group over individually 
+            by: str='row',                                  # determines how the func is applied.
+            reduce_cols: Optional[T_la]=None,               # columns included in the reduce operation.
+            # keyfield: str=colname,                        # provide this for when no keyfield is desired?
+                                                            # current operation sets keyfield to colname.
+            ) -> Dict[str, 'Daf']:
+    
+        result_dodaf = self.multi_groupby_reduce(colnames=colnames, func=self.__class__.sum_da, by=by, reduce_cols=reduce_cols)
+        
+        return result_dodaf
+
+
     def set_col2_from_col1_using_regex_select(self, col1: str, col2: str='', regex: str=''):
     
         """ given two cols that already exist, apply regex select to col1 to create col2
             regex should include parens that enclose the desired portion of col1.
         """
         
         # from utilities import utils
@@ -4382,41 +4839,71 @@
         result_da = {key: (d1_da.get(key, 0) or 0) - (d2_da.get(key, 0) or 0)
                         for key in keys_list}
                 
         return result_da
 
 
     @staticmethod
-    def count_values_da(row_da: T_da, result_dodi: T_dodi, cols: Iterable) -> T_dodi:
+    def count_values_da(
+            row_da: T_da, 
+            reduction_da: T_da, 
+            cols_iter: Iterable, 
+            *, 
+            omit_nulls: bool=False,
+            
+            ) -> T_dodi:
         """ incrementally build the result_dodi, which is the valuecounts for each item in row_da.
             can be used to calculate valuecounts over all rows and chunks.
             
             row_da may be scalar values (typically strings that are to be counted)
             but may also be a dodi of totals from a set of chunks that are to be combined.
             
             Intended use is to use this to calculate valuecounts by scanning all rows of a daf.
             Return a dodi.
             Put those in a daf table and then scan those combined values and create a singular result.
             
-            This is a reducing and accumulating operation. Can be used with daf.reduce()
+            This is a reducing and accumulating operation. Can be used with daf.reduce().
+            
+            For example:
+                value_counts_dodi = {}
+                cols_of_interest  = ['gender', 'location']
+            
+                value_counts_dodi = my_daf.reduce(count_values_da, value_counts_dodi, cols_of_interest, omit_nulls=True)
+                
+            results in (something like this):
+            
+                value_counts_dodi = {'gender': {'Male': 2435, 'Female': 2489}, 'location':{'north': 2433, 'south': 345}}
             
         """
     
         # if cols is None:
             # cols_dict = {}
         # else:
             # cols_dict = dict.fromkeys(cols)
             
-        if not result_dodi:
-            result_dodi = {}
+        if not reduction_da:
+            reduction_da = {}
+            
+        result_dodi = reduction_da
         
-        for col in cols:
+        for col in cols_iter:
 
             val = row_da[col]
             
+            if omit_nulls and isinstance(val, str) and not val:
+                continue
+            
+            if val and isinstance(val, list):
+                # val is a list of values
+                if col not in result_dodi:
+                    result_dodi[col] = val
+                else:    
+                    result_dodi[col].append(val)
+                continue
+                
             if val and isinstance(val, dict):
                 # val is a dict of values determined in another pass.
                 if col not in result_dodi:
                     result_dodi[col] = val
                 else:    
                     result_dodi[col] = Daf.sum_da(val, result_dodi[col])
                 continue
@@ -4570,30 +5057,33 @@
         return valuecounts_di
 
 
     def valuecounts_for_colnames_ls(
             self, 
             colnames_ls: Optional[T_ls]=None, 
             sort: bool=False, 
-            reverse: bool=True
+            reverse: bool=True,
+            omit_nulls: bool=False,
             ) -> T_dodi:
         """ return value counts for a set of columns or all columns if no colnames_ls are provided.
             sort if noted from most prevalent to least in each column.
+            
+            Note: This is an inefficient algorithm
         """
     
         if not colnames_ls:
             colnames_ls = self.columns()
             
         colnames_ls = cast(T_ls, colnames_ls)    
 
         valuecounts_dodi: T_dodi = {}
         
         for colname in colnames_ls:
             valuecounts_dodi[colname] = \
-                self.valuecounts_for_colname(colname, sort=sort, reverse=reverse)
+                self.valuecounts_for_colname(colname, sort=sort, reverse=reverse, omit_nulls=omit_nulls)
 
         return valuecounts_dodi
     
 
     def valuecounts_for_colname_selectedby_colname(
             self, 
             colname: str, 
@@ -4715,15 +5205,15 @@
         info_dod = {}
 
         # from utilities import utils
 
         for col_def_ta in col_def_lot:
             col_name, col_dtype, col_format, col_profile = col_def_ta
             
-            col_data_la = self.col(col_name)
+            col_data_la = self[:, col_name].to_list()
             
             info_dod[col_name] = utils.list_stats(col_data_la, profile=col_profile)
             
         return info_dod
 
    
     def transpose(self, new_keyfield:str='', new_cols:Optional[T_la]=None, include_header:bool = False) -> 'Daf':
@@ -4883,15 +5373,15 @@
             omit_header         = not header_exists, 
             shorten_text        = shorten_text, 
             max_text_len        = max_text_len, 
             smart_fmt           = smart_fmt,
             
             )
         if include_summary:    
-            mdstr += f"\n\[{len(self.lol)} rows x {len(self.hd)} cols; keyfield={self.keyfield}; {len(self.kd)} keys ] ({self.name or type(self).__name__})\n"
+            mdstr += f"\n\[{len(self.lol)} rows x {len(self.hd)} cols; keyfield='{self.keyfield}'; {len(self.kd)} keys ] ({self.name or type(self).__name__})\n"
         return mdstr
         
 
     def to_md_cols(
             self, 
             max_rows:       int     = 0,         # limit the maximum number of row by keeping leading and trailing rows.
             max_cols:       int     = 0,         # limit the maximum number of cols by keeping leading and trailing cols.
@@ -4939,15 +5429,15 @@
         if colnames_ls:
             result_lol = [colnames_ls] + result_lol
 
         # no limits, return summary.
         if not max_rows and not max_cols:
             return result_lol
 
-        num_rows    = len(self.lol) if self.lol else 0
+        num_rows    = self.num_rows()
         num_cols    = self.num_cols()
 
         if max_rows and num_rows <= max_rows:
             # Get all the rows, but potentially limit columns
             result_lol = utils.reduce_lol_cols(result_lol, max_cols=max_cols)
         
         else:
@@ -5014,9 +5504,11 @@
 Pydf.select_records_pydf     = Daf.select_records_daf
 Pydf.pydf_sum                = Daf.daf_sum
 Pydf.pydf_valuecount         = Daf.daf_valuecount
 Pydf.groupsum_pydf           = Daf.groupsum_daf
 Pydf.gen_stats_pydf          = Daf.gen_stats_daf
 Pydf.value_counts_pydf       = Daf.value_counts_daf
 
+Daf.groupsum                 = Daf.groupsum_daf
+
 Pydf.md_pydf_table = Pydf.to_md
```

### Comparing `daffodil-0.4.4/src/daffodil/lib/daf_indexing.py` & `daffodil-0.5.0/src/daffodil/lib/daf_indexing.py`

 * *Files 1% similar despite different names*

```diff
@@ -522,15 +522,15 @@
         # Assigning a row based on a single integer index and a value which is a list.
         # will trigger an error if the list is not the right length for the row.
         if isinstance(value, list):
             self.lol[irow] = value
             
         # if value is a dict, use it and make sure the right columns are assigned per dict keys.    
         elif isinstance(value, dict):
-            self.assign_record_da_irow(irow, record_da=value)
+            self.assign_record_irow(irow, record=value)
         else:
             # set the same value in the row for all columns.
             self.lol[irow] = [value] * len(self.lol[irow])
         
     elif isinstance(slice_spec, list) and isinstance(value, self.__class__):
         # assign a number of rows to the data in daf provided.
         row_indices = self._row_indices_from_rowlist(slice_spec)
```

### Comparing `daffodil-0.4.4/src/daffodil/lib/daf_md.py` & `daffodil-0.5.0/src/daffodil/lib/daf_md.py`

 * *Files identical despite different names*

### Comparing `daffodil-0.4.4/src/daffodil/lib/daf_pandas.py` & `daffodil-0.5.0/src/daffodil/lib/daf_pandas.py`

 * *Files identical despite different names*

### Comparing `daffodil-0.4.4/src/daffodil/lib/daf_types.py` & `daffodil-0.5.0/src/daffodil/lib/daf_types.py`

 * *Files identical despite different names*

### Comparing `daffodil-0.4.4/src/daffodil/lib/daf_utils.py` & `daffodil-0.5.0/src/daffodil/lib/daf_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -455,14 +455,18 @@
         if isinstance(val, str):
             new_val = val
         elif isinstance(val, bool):
             new_val = 1 if val else 0
         else:    
             new_val = f"{val}"
         
+    elif desired_type == list and isinstance(val, list) or desired_type == dict and isinstance(val, dict):
+        # no conversion required.
+        new_val = val
+
     else:
         breakpoint() #perm
         error_beep()
         pass
                  
     return new_val
     
@@ -473,21 +477,21 @@
         allows correct JSON or python objects stringified with f"{obj}"
     
     """
 
 
     val = val.strip()
     
-    if val and isinstance(val, str) and val.strip()[0] in ('[', '{', '('):
-        obj_val = json_decode(val)
+    if val and isinstance(val, str) and val[0] in ('[', '{', '('):
+        obj_val = json_decode(val)  # this returns '' on failure
         
-    if not obj_val:
+    if obj_val == '':
         obj_val = safe_eval(val)
         
-    if not obj_val:
+    if obj_val == '':
         return val
         
     return obj_val
     
     
 def safe_eval(value: str) -> Optional[Any]:
     """ un-stringify an object without risk of using eval. """
@@ -873,17 +877,17 @@
         does not alter lol
     
     """
     
     if not max_cols or not lol:
         return lol
         
-    col_num = len(lol[0])
+    num_cols = len(lol[0])
 
-    if col_num <= max_cols:
+    if num_cols <= max_cols:
         return lol
         
     first_col_num = math.ceil(max_cols/2)
     last_col_num  = max_cols - first_col_num
     
     result_lol = [row_la[:first_col_num] + [divider_str] + row_la[-last_col_num:]
                                 for row_la in lol]   
@@ -1113,24 +1117,14 @@
         dod_key = da[keyfield]
         if remove_keyfield:
             del da[keyfield]
         dod[dod_key] = da
     return dod        
     
 
-def safe_eval(value: str) -> Optional[Any]:
-    """ un-stringify an object without risk of using eval for malicious actions. """
-    
-    try:
-        parsed_value = ast.literal_eval(value)
-        return parsed_value
-    except (SyntaxError, ValueError):
-        return None
-        
-        
 def safe_min(listlike: List[Any]) -> Any:
     # note! Using try/except in to guard for the length of list is not specific enough. 
     #   We still need failure under other conditions.
 
     if len(listlike) < 1:
         return 0
     return min(listlike)
```

### Comparing `daffodil-0.4.4/src/daffodil/lib/md_demo.py` & `daffodil-0.5.0/src/daffodil/lib/md_demo.py`

 * *Files identical despite different names*

### Comparing `daffodil-0.4.4/src/daffodil.egg-info/PKG-INFO` & `daffodil-0.5.0/src/daffodil.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: daffodil
-Version: 0.4.4
+Version: 0.5.0
 Summary: Daffodil provides lightweight and fast 2-D dataframes
 Author-email: Ray Lutz <raylutz@cognisys.com>
 License: MIT
 Project-URL: Homepage, https://github.com/raylutz/daffodil
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -32,15 +32,16 @@
 as these design tradeoffs are being evaluated and the final initial design resolved. Please see GitHub issues to
 weigh in on the design.
 
 ## Data Model
 The Daffodil data model is really very simple. The core array is a list-of-lists (lol), optionally with one or two associated
 dictionaries, one for the column names and one for row keys.
 
-![pydf_table](https://github.com/raylutz/daffodil/assets/14955977/05c54a27-8d8e-47b6-ae73-957709a5d398)
+![image](https://github.com/raylutz/daffodil/assets/14955977/fa33237c-2075-4bbe-81e1-a6c1e324f46a)
+
 
 Daffodil uses standard python data types, and can mix data types in rows and columns, and can store any type 
 within a cell, even another Daffodil instance. 
 
 It works well in traditional Pythonic processing paradigms, such as in loops, allowing fast row appends, 
 insertions and other operations that column-oriented packages like Pandas handle poorly or don't offer at all.
 Selecting, inserting, appending rows does not make a copy of the data but uses references the way 
@@ -329,15 +330,15 @@
 
        
 ## Common Usage Pattern
        
 One common usage pattern allows iteration over the rows and appending to another Daf instance. For example:
     
         # read csv file into 2-D array, handling column headers, respecting data types and unflattening
-        my_daf = Daf.from_csv(file_path).apply_dtypes(my_daf_dtypes)
+        my_daf = Daf.from_csv(file_path).apply_dtypes(dtypes=my_daf_dtypes)
     
         # create a new (empty) table to be built as we scan the input.
         new_daf = Daf()
         
         # scan the input my_daf row by row and construct the output. Pandas can't do this efficiently.
         for original_row in my_daf:  
             new_row = transform_row(original_row)
@@ -346,23 +347,23 @@
             # here the column names are initialized as the first dictionary is appended.
             
         # create a flat csv file with any python objects flattened using JSON.
         new_daf.flatten().to_csv(file_path)        
 
 This common pattern can be abbreviated using the apply() method:
 
-        my_daf = Daf.from_csv(file_path).apply_dtypes(my_daf_dtypes)
+        my_daf = Daf.from_csv(file_path).apply_dtypes(dtypes=my_daf_dtypes)
         
         new_daf = my_daf.apply(transform_row)
         
         new_daf.flatten().to_csv(file_path)
 
 Or
 
-        Daf.from_csv(file_path).apply_dtypes(my_daf_dtypes).apply(transform_row).flatten().to_csv(file_path)
+        Daf.from_csv(file_path).apply_dtypes(dtypes=my_daf_dtypes).apply(transform_row).flatten().to_csv(file_path)
 
 And further extension of this pattern can apply the transformation to a set of csv files described by a chunk_manifest.
 The chunk manifest essentially provides metadata and instructions for accessing the source data, which may be many 1000s
 of chunks, each of which will fit in memory.
 
         chunk_manifest_daf = Daf.from_csv(file_path)  
         result_manifest_daf = chunk_manifest_daf.manifest_apply(transform_row)
@@ -524,25 +525,26 @@
 #### return list of row keyfield values, if keyfield is defined.
 
     my_daf.keys()    
     
 ### Indexing: inspecting values in a daf array
 
 Daffodil offers easy-to-used indexing of rows, columns, individual cells or any ranges.
-Will generally return the simplest type possible, such as cell contents, a list or daf if retmode == 'val'
-otherwise, if retmode == 'obj', then a full daf object is returned.
+if retmode == 'val', then it will generally return the simplest type possible, such as cell contents, a list or daf 
+otherwise, if retmode == 'obj', then a full daf object is returned. If you desired a list or dict, then it is 
+convenient to just use the .to_list() or .to_dict() methods.
 
 if retmode is 'val':
 - if only one cell is selected, return a single value.
 - If only one row is selected, return a list.
 - if only one col is selected, return a list.
 - if multiple columns are specified, they will be returned in the original orientation in a consistent daf instance copied from the original, and with the data specified.
 
 Please note: operations on columns is relatively inefficient. Try to avoid working on one column at a time.
-Instead, use .apply() or .reduce() and handle any manipulations of all columns at the same time, and select them with the cols parameter at that time.
+Instead, use .apply() or .reduce() and handle any manipulations without dropping columns, and select them with the cols parameter at that time.
 
       `my_daf[2, 3]`     -- select cell at row 2, col 3 and return value.
       `my_daf[2]`        -- select row 2, including all columns, return a list.
       `my_daf[2, :]`     -- same as above
       `my_daf[-1, :]`    -- select the last row
       `my_daf[:5]`       -- select first 5 rows; like `head()` in other dataframe packages.
       `my_daf[:-5]`      -- select last 5 rows; like `tail()` in other dataframe packages.
@@ -631,19 +633,19 @@
     my_daf.append(other_daf)    
 
 
 ### selecting and removing records by keys
 
 #### select one record using keyfield.
 
-    record_da = my_daf.select_record_da(keyvalue)
+    record = my_daf.select_record(keyvalue)
     
 or
 
-   record_list = my_daf[keyvalue].to_dict()
+    record_list = my_daf[keyvalue].to_list()
    
 Note that this syntax differs from Pandas, which normally references a column if square brackets are used with no other
 syntax.
 
 #### select multiple records using the keyfield and return a daf.
 
     new_daf = my_daf[keyvalue_list]
```

### Comparing `daffodil-0.4.4/tests/test_daf.py` & `daffodil-0.5.0/tests/test_daf.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # test_daf
 # copyright (c) 2024 Ray Lutz
 
 import os
-import sys
 import unittest
 import numpy as np
 import pandas as pd
 #from io import BytesIO
 from pathlib import Path
+
+import sys
 sys.path.append(os.path.join(os.path.dirname(sys.path[0]), 'src'))
 
 from daffodil.daf import Daf
 from daffodil.lib import daf_utils as utils
 
 class TestDaf(unittest.TestCase):
 
@@ -1381,44 +1382,44 @@
         daf = Daf(cols=cols, lol=lol, keyfield='col1', dtypes={'col1': int, 'col2': str})
 
         keylist = [4, 5, 6]
 
         with self.assertRaises(KeyError):
             daf.remove_keylist(keylist, silent_error=False)
 
-    # select_record_da
-    def test_select_record_da_existing_key(self):
+    # select_record
+    def test_select_record_existing_key(self):
         cols = ['col1', 'col2']
         lol = [[1, 'a'], [2, 'b'], [3, 'c']]
         daf = Daf(cols=cols, lol=lol, keyfield='col1', dtypes={'col1': int, 'col2': str})
 
         key = 2
-        record_da = daf.select_record_da(key)
+        record_da = daf.select_record(key)
 
         self.assertEqual(record_da, {'col1': 2, 'col2': 'b'})
 
-    def test_select_record_da_nonexistent_key(self):
+    def test_select_record_nonexistent_key(self):
         cols = ['col1', 'col2']
         lol = [[1, 'a'], [2, 'b'], [3, 'c']]
         daf = Daf(cols=cols, lol=lol, keyfield='col1', dtypes={'col1': int, 'col2': str})
 
         key = 4
-        record_da = daf.select_record_da(key)
+        record_da = daf.select_record(key)
 
         self.assertEqual(record_da, {})
 
-    def test_select_record_da_no_keyfield(self):
+    def test_select_record_no_keyfield(self):
         cols = ['col1', 'col2']
         lol = [[1, 'a'], [2, 'b'], [3, 'c']]
         daf = Daf(cols=cols, lol=lol, keyfield='', dtypes={'col1': int, 'col2': str})
 
         key = 'col1'
 
         with self.assertRaises(RuntimeError):
-            daf.select_record_da(key)
+            daf.select_record(key)
 
     # iloc / irow
     def test_iloc_existing_row_idx(self):
         cols = ['col1', 'col2']
         lol = [[1, 'a'], [2, 'b'], [3, 'c']]
         daf = Daf(cols=cols, lol=lol, keyfield='col1', dtypes={'col1': int, 'col2': str})
 
@@ -1995,159 +1996,159 @@
     # assign_record
     def test_assign_record_empty_daf(self):
         cols = []
         lol = []
         daf = Daf(cols=cols, lol=lol, keyfield='col1', dtypes={})
 
         record_da = {'col1': 1, 'col2': 'a'}
-        daf.assign_record_da(record_da)
+        daf.assign_record(record_da)
 
         expected_lol = [[1, 'a']]
         self.assertEqual(daf.lol, expected_lol)
 
     def test_assign_record_nonempty_daf_add_new_record(self):
         cols = ['col1', 'col2']
         lol = [[1, 'a'], [2, 'b'], [3, 'c']]
         daf = Daf(cols=cols, lol=lol, keyfield='col1', dtypes={'col1': int, 'col2': str})
 
         record_da = {'col1': 4, 'col2': 'd'}
-        daf.assign_record_da(record_da)
+        daf.assign_record(record_da)
 
         expected_lol = [[1, 'a'], [2, 'b'], [3, 'c'], [4, 'd']]
         self.assertEqual(daf.lol, expected_lol)
 
     def test_assign_record_nonempty_daf_update_existing_record(self):
         cols = ['col1', 'col2']
         lol = [[1, 'a'], [2, 'b'], [3, 'c']]
         daf = Daf(cols=cols, lol=lol, keyfield='col1', dtypes={'col1': int, 'col2': str})
 
         record_da = {'col1': 2, 'col2': 'x'}
-        daf.assign_record_da(record_da)
+        daf.assign_record(record_da)
 
         expected_lol = [[1, 'a'], [2, 'x'], [3, 'c']]
         self.assertEqual(daf.lol, expected_lol)
 
     def test_assign_record_missing_keyfield(self):
         cols = ['col1', 'col2']
         lol = [[1, 'a'], [2, 'b'], [3, 'c']]
         daf = Daf(cols=cols, lol=lol, keyfield='col1', dtypes={'col1': int, 'col2': str})
 
         record_da = {'col2': 'x'}
         with self.assertRaises(RuntimeError):
-            daf.assign_record_da(record_da)
+            daf.assign_record(record_da)
 
     def test_assign_record_fields_not_equal_to_columns(self):
         cols = ['col1', 'col2']
         lol = [[1, 'a'], [2, 'b'], [3, 'c']]
         daf = Daf(cols=cols, lol=lol, keyfield='col1', dtypes={'col1': int, 'col2': str})
 
         record_da = {'col1': 4, 'col2': 'd', 'col3': 'extra'}
         with self.assertRaises(RuntimeError):
-            daf.assign_record_da(record_da)
+            daf.assign_record(record_da)
 
     # assign_record_irow
     def test_assign_record_irow_empty_daf(self):
         cols = []
         lol = []
         daf = Daf(cols=cols, lol=lol, keyfield='col1', dtypes={})
 
         record_da = {'col1': 1, 'col2': 'a'}
-        daf.assign_record_da_irow(irow=0, record_da=record_da)
+        daf.assign_record_irow(irow=0, record=record_da)
 
         expected_lol = [[1, 'a']]
         self.assertEqual(daf.lol, expected_lol)
 
     def test_assign_record_irow_nonempty_daf_add_new_record(self):
         cols = ['col1', 'col2']
         lol = [[1, 'a'], [2, 'b'], [3, 'c']]
         daf = Daf(cols=cols, lol=lol, keyfield='col1', dtypes={'col1': int, 'col2': str})
 
         record_da = {'col1': 4, 'col2': 'd'}
-        daf.assign_record_da_irow(irow=3, record_da=record_da)
+        daf.assign_record_irow(irow=3, record=record_da)
 
         expected_lol = [[1, 'a'], [2, 'b'], [3, 'c'], [4, 'd']]
         self.assertEqual(daf.lol, expected_lol)
 
     def test_assign_record_irow_nonempty_daf_update_existing_record(self):
         cols = ['col1', 'col2']
         lol = [[1, 'a'], [2, 'b'], [3, 'c']]
         daf = Daf(cols=cols, lol=lol, keyfield='col1', dtypes={'col1': int, 'col2': str})
 
         record_da = {'col1': 2, 'col2': 'x'}
-        daf.assign_record_da_irow(irow=1, record_da=record_da)
+        daf.assign_record_irow(irow=1, record=record_da)
 
         expected_lol = [[1, 'a'], [2, 'x'], [3, 'c']]
         self.assertEqual(daf.lol, expected_lol)
 
     def test_assign_record_irow_invalid_irow(self):
         cols = ['col1', 'col2']
         lol = [[1, 'a'], 
                [2, 'b'], 
                [3, 'c']]
         daf = Daf(cols=cols, lol=lol, keyfield='col1', dtypes={'col1': int, 'col2': str})
 
         record_da = {'col1': 4, 'col2': 'd'}
         
-        daf.assign_record_da_irow(irow=5, record_da=record_da)
+        daf.assign_record_irow(irow=5, record=record_da)
 
         expected_lol = [[1, 'a'], 
                         [2, 'b'], 
                         [3, 'c'],
                         [4, 'd'],
                         ]
         self.assertEqual(daf.lol, expected_lol)
 
-    def test_assign_record_irow_missing_record_da(self):
+    def test_assign_record_irow_missing_record(self):
         cols = ['col1', 'col2']
         lol = [[1, 'a'], [2, 'b'], [3, 'c']]
         daf = Daf(cols=cols, lol=lol, keyfield='col1', dtypes={'col1': int, 'col2': str})
 
-        daf.assign_record_da_irow(irow=1, record_da=None)
+        daf.assign_record_irow(irow=1, record=None)
 
         expected_lol = [[1, 'a'], [2, 'b'], [3, 'c']]
         self.assertEqual(daf.lol, expected_lol)
 
    # update_record_irow
     def test_update_record_irow_empty_daf(self):
         cols = []
         lol = []
         daf = Daf(cols=cols, lol=lol, keyfield='col1', dtypes={})
 
         record_da = {'col1': 1, 'col2': 'a'}
-        daf.update_record_da_irow(irow=0, record_da=record_da)
+        daf.update_record_irow(irow=0, record=record_da)
 
         self.assertEqual(daf.lol, [])
 
     def test_update_record_irow_nonempty_daf_update_existing_record(self):
         cols = ['col1', 'col2']
         lol = [[1, 'a'], [2, 'b'], [3, 'c']]
         daf = Daf(cols=cols, lol=lol, keyfield='col1', dtypes={'col1': int, 'col2': str})
 
         record_da = {'col1': 2, 'col2': 'x', 'col3': 'extra'}
-        daf.update_record_da_irow(irow=1, record_da=record_da)
+        daf.update_record_irow(irow=1, record=record_da)
 
         expected_lol = [[1, 'a'], [2, 'x'], [3, 'c']]
         self.assertEqual(daf.lol, expected_lol)
 
     def test_update_record_irow_invalid_irow(self):
         cols = ['col1', 'col2']
         lol = [[1, 'a'], [2, 'b'], [3, 'c']]
         daf = Daf(cols=cols, lol=lol, keyfield='col1', dtypes={'col1': int, 'col2': str})
 
         record_da = {'col1': 4, 'col2': 'd'}
-        daf.update_record_da_irow(irow=5, record_da=record_da)
+        daf.update_record_irow(irow=5, record=record_da)
 
         self.assertEqual(daf.lol, lol)
 
-    def test_update_record_irow_missing_record_da(self):
+    def test_update_record_irow_missing_record(self):
         cols = ['col1', 'col2']
         lol = [[1, 'a'], [2, 'b'], [3, 'c']]
         daf = Daf(cols=cols, lol=lol, keyfield='col1', dtypes={'col1': int, 'col2': str})
 
-        daf.update_record_da_irow(irow=1, record_da=None)
+        daf.update_record_irow(irow=1, record=None)
 
         expected_lol = [[1, 'a'], [2, 'b'], [3, 'c']]
         self.assertEqual(daf.lol, expected_lol)
 
     # def test_update_record_irow_missing_hd(self):
         # cols = ['col1', 'col2']
         # hd = {'col1': 0, 'col2': 1}
```

