# Comparing `tmp/FairFRU-0.2.8.tar.gz` & `tmp/FairFRU-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FairFRU-0.2.8.tar", last modified: Fri May 10 15:22:53 2024, max compression
+gzip compressed data, was "FairFRU-0.2.9.tar", last modified: Thu May 23 13:37:49 2024, max compression
```

## Comparing `FairFRU-0.2.8.tar` & `FairFRU-0.2.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 15:22:53.669583 FairFRU-0.2.8/
-drwxrwxrwx   0        0        0        0 2024-05-10 15:22:53.649582 FairFRU-0.2.8/FairFRU/
--rw-rw-rw-   0        0        0     1927 2024-05-10 15:16:06.000000 FairFRU-0.2.8/FairFRU/FRSpy.py
--rw-rw-rw-   0        0        0      186 2023-12-06 16:42:13.000000 FairFRU-0.2.8/FairFRU/__init__.py
--rw-rw-rw-   0        0        0     3333 2024-05-10 15:17:59.000000 FairFRU-0.2.8/FairFRU/fuzzy_rough_regions.py
--rw-rw-rw-   0        0        0     3143 2024-03-20 11:15:09.000000 FairFRU-0.2.8/FairFRU/fuzzy_rough_uncertainty.py
--rw-rw-rw-   0        0        0     2703 2024-05-10 15:14:46.000000 FairFRU-0.2.8/FairFRU/h5file_create_array.py
-drwxrwxrwx   0        0        0        0 2024-05-10 15:22:53.664659 FairFRU-0.2.8/FairFRU.egg-info/
--rw-rw-rw-   0        0        0      690 2024-05-10 15:22:53.000000 FairFRU-0.2.8/FairFRU.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      288 2024-05-10 15:22:53.000000 FairFRU-0.2.8/FairFRU.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 15:22:53.000000 FairFRU-0.2.8/FairFRU.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-05-10 15:22:53.000000 FairFRU-0.2.8/FairFRU.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      690 2024-05-10 15:22:53.667583 FairFRU-0.2.8/PKG-INFO
--rw-rw-rw-   0        0        0      464 2023-11-23 14:54:33.000000 FairFRU-0.2.8/README.md
--rw-rw-rw-   0        0        0     1091 2023-11-23 14:55:13.000000 FairFRU-0.2.8/license.txt
--rw-rw-rw-   0        0        0       42 2024-05-10 15:22:53.670584 FairFRU-0.2.8/setup.cfg
--rw-rw-rw-   0        0        0      450 2024-05-10 15:21:51.000000 FairFRU-0.2.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 13:37:49.182055 FairFRU-0.2.9/
+drwxrwxrwx   0        0        0        0 2024-05-23 13:37:49.142058 FairFRU-0.2.9/FairFRU/
+-rw-rw-rw-   0        0        0     1927 2024-05-10 15:16:06.000000 FairFRU-0.2.9/FairFRU/FRSpy.py
+-rw-rw-rw-   0        0        0      186 2023-12-06 16:42:13.000000 FairFRU-0.2.9/FairFRU/__init__.py
+-rw-rw-rw-   0        0        0     3331 2024-05-23 11:15:26.000000 FairFRU-0.2.9/FairFRU/fuzzy_rough_regions.py
+-rw-rw-rw-   0        0        0     3223 2024-05-13 14:12:40.000000 FairFRU-0.2.9/FairFRU/fuzzy_rough_uncertainty.py
+-rw-rw-rw-   0        0        0     2709 2024-05-23 13:33:37.000000 FairFRU-0.2.9/FairFRU/h5file_create_array.py
+drwxrwxrwx   0        0        0        0 2024-05-23 13:37:49.172061 FairFRU-0.2.9/FairFRU.egg-info/
+-rw-rw-rw-   0        0        0      690 2024-05-23 13:37:48.000000 FairFRU-0.2.9/FairFRU.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      288 2024-05-23 13:37:48.000000 FairFRU-0.2.9/FairFRU.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 13:37:48.000000 FairFRU-0.2.9/FairFRU.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-23 13:37:48.000000 FairFRU-0.2.9/FairFRU.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      690 2024-05-23 13:37:49.178056 FairFRU-0.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0      464 2023-11-23 14:54:33.000000 FairFRU-0.2.9/README.md
+-rw-rw-rw-   0        0        0     1091 2023-11-23 14:55:13.000000 FairFRU-0.2.9/license.txt
+-rw-rw-rw-   0        0        0       42 2024-05-23 13:37:49.184058 FairFRU-0.2.9/setup.cfg
+-rw-rw-rw-   0        0        0      450 2024-05-23 13:35:10.000000 FairFRU-0.2.9/setup.py
```

### Comparing `FairFRU-0.2.8/FairFRU/FRSpy.py` & `FairFRU-0.2.9/FairFRU/FRSpy.py`

 * *Files identical despite different names*

### Comparing `FairFRU-0.2.8/FairFRU/fuzzy_rough_regions.py` & `FairFRU-0.2.9/FairFRU/fuzzy_rough_regions.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import pandas as pd
 from .FRSpy import FRSpy
 from .h5file_create_array import Writearray
 import h5py
 import pickle
 import os 
 
-def compute_membership_values(df, case_name, path, columns, complete = True, hide_progress = False):
+def compute_membership_values(df, case_name, path, columns, complete = False, hide_progress = False):
   '''
   A function that computes the membership values to fuzzy-rough regions.
 
   Attributes
   ------------
   df : pandas DataFrame
     Contains all variables in the dataset plus the decision variable which must be located in the LAST column
@@ -22,15 +22,15 @@
   path : str
     path to file
   
   columns: list of strings
     a list of the column names to be suppressed or removed from the dataset. after removal, the fuzzy-rough
     set regions will be computed using the rest of the data
   
-  complete : bool
+  complete : False
     if True, the membership values to the fuzzy-rought regions are create using the complete set of data. 
     if this object already exists, you can set it to False to save time if dealing with large dataset
   '''
 
   # rename the column names cause they contain illegal characters and h5 cannot index columns properly
   df.columns = list(map(lambda x: re.sub('=<', 'less',x), list(df.columns)))
   df.columns = list(map(lambda x: re.sub('=>', 'more',x), list(df.columns)))
@@ -38,15 +38,15 @@
 
   # fr values to fuzzy rough regions
 
   target = df.iloc[:,-1]
   membership = pd.get_dummies(target)
   file_name = os.path.join(path, "matrix_"+case_name+".h5")
 
-  if complete == True:
+  if not complete:
     h5file = open_file(file_name, mode="w", title=case_name) # create h5 file to store distance matrix
 
     group = h5file.create_group("/", 'full', 'Distances after removing full') # full
     Writearray(df.iloc[:,:-1], 0.5, 'full').sim_array(h5file = h5file, group = group, hide_progress = hide_progress)
 
     h5file.close()
```

### Comparing `FairFRU-0.2.8/FairFRU/fuzzy_rough_uncertainty.py` & `FairFRU-0.2.9/FairFRU/fuzzy_rough_uncertainty.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     '''
     
     # load membership values
     mem_dic = {}
     for root, dirs, files in os.walk(path, topdown=False):
         for name in files:
             if 'pickle' in name:
-                att_name = re.findall(r"(.*?)\_", name)[0]
+                att_name = re.findall(r"(.*?)_mem.pickle", name)[0] # there is an issue when there _ in name, only picks first word, yikes
                 file_path_name = os.path.join(root, name) 
                 with open(file_path_name, 'rb') as handle: 
                     mem_dic_att = pickle.load(handle)
                     mem_dic[att_name] = mem_dic_att
 
     for col in columns:
         # l2 -----------------------
```

### Comparing `FairFRU-0.2.8/FairFRU/h5file_create_array.py` & `FairFRU-0.2.9/FairFRU/h5file_create_array.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         '''
         self.variable = variable
         self.numeric = [False if df[col].dtype == 'object' else True for col in df]
         self.nominal = [True if df[col].dtype == 'object' else False for col in df]
 
         num = df.loc[:,self.numeric]
         scaled=np.subtract(num,np.min(num,axis=0))/np.subtract(np.max(num,axis=0),np.min(num,axis=0))
-        df[df.columns[self.numeric]] = scaled.round(3).astype('float32')
+        df.loc[:,df.columns[self.numeric]] = scaled.round(3).astype('float32')
 
         self.df = df.values
         self.alpha = alpha
 
     def sim_array(self, h5file, group, hide_progress = False):
        for instance in tqdm(range(0,len(self.df)), desc=self.variable+' building similarity matrix', disable=hide_progress):
           sim = self.similarity(instance)
```

### Comparing `FairFRU-0.2.8/FairFRU.egg-info/PKG-INFO` & `FairFRU-0.2.9/FairFRU.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FairFRU
-Version: 0.2.8
+Version: 0.2.9
 Summary: A bias measure using the fuzzy rough set theory
 Author: Lisa Koutsoviti, Gonzalo Napoles
 Description-Content-Type: text/markdown
 License-File: license.txt
 
 # Using fuzzy-rough sets to measure bias in pattern classification problems
```

### Comparing `FairFRU-0.2.8/PKG-INFO` & `FairFRU-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FairFRU
-Version: 0.2.8
+Version: 0.2.9
 Summary: A bias measure using the fuzzy rough set theory
 Author: Lisa Koutsoviti, Gonzalo Napoles
 Description-Content-Type: text/markdown
 License-File: license.txt
 
 # Using fuzzy-rough sets to measure bias in pattern classification problems
```

### Comparing `FairFRU-0.2.8/license.txt` & `FairFRU-0.2.9/license.txt`

 * *Files identical despite different names*

