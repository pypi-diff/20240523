# Comparing `tmp/binsreg-2.1.4.tar.gz` & `tmp/binsreg-2.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/rmasini/Library/CloudStorage/Dropbox/binsreg/Python/binsreg/dist/.tmp-9prn06kt/binsreg-2.1.4.tar", last modified: Sun Jan 21 21:13:08 2024, max compression
+gzip compressed data, was "binsreg-2.1.5.tar", last modified: Thu May 23 15:40:14 2024, max compression
```

## Comparing `binsreg-2.1.4.tar` & `binsreg-2.1.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 rmasini    (501) staff       (20)        0 2024-01-21 21:13:08.938752 binsreg-2.1.4/
--rw-r--r--   0 rmasini    (501) staff       (20)     4238 2024-01-21 21:13:08.938464 binsreg-2.1.4/PKG-INFO
--rw-r--r--   0 rmasini    (501) staff       (20)     3512 2023-10-03 01:56:20.000000 binsreg-2.1.4/README.md
--rw-r--r--   0 rmasini    (501) staff       (20)      108 2021-09-05 04:38:28.000000 binsreg-2.1.4/pyproject.toml
--rw-r--r--   0 rmasini    (501) staff       (20)      823 2024-01-21 21:13:08.941555 binsreg-2.1.4/setup.cfg
-drwxr-xr-x   0 rmasini    (501) staff       (20)        0 2024-01-21 21:13:08.869315 binsreg-2.1.4/src/
-drwxr-xr-x   0 rmasini    (501) staff       (20)        0 2024-01-21 21:13:08.900534 binsreg-2.1.4/src/binsreg/
--rw-r--r--   0 rmasini    (501) staff       (20)      189 2021-09-05 04:38:11.000000 binsreg-2.1.4/src/binsreg/__init__.py
--rw-r--r--   0 rmasini    (501) staff       (20)    79486 2023-10-03 02:36:43.000000 binsreg-2.1.4/src/binsreg/binsglm.py
--rw-r--r--   0 rmasini    (501) staff       (20)    42134 2023-10-03 02:36:20.000000 binsreg-2.1.4/src/binsreg/binspwc.py
--rw-r--r--   0 rmasini    (501) staff       (20)    72759 2023-10-03 02:36:34.000000 binsreg-2.1.4/src/binsreg/binsqreg.py
--rw-r--r--   0 rmasini    (501) staff       (20)    72280 2024-01-21 20:51:05.000000 binsreg-2.1.4/src/binsreg/binsreg.py
--rw-r--r--   0 rmasini    (501) staff       (20)    24456 2023-10-03 02:36:57.000000 binsreg-2.1.4/src/binsreg/binsregselect.py
--rw-r--r--   0 rmasini    (501) staff       (20)    46052 2023-10-03 02:36:22.000000 binsreg-2.1.4/src/binsreg/binstest.py
--rw-r--r--   0 rmasini    (501) staff       (20)    60380 2023-10-03 02:58:30.000000 binsreg-2.1.4/src/binsreg/funs.py
-drwxr-xr-x   0 rmasini    (501) staff       (20)        0 2024-01-21 21:13:08.917445 binsreg-2.1.4/src/binsreg.egg-info/
--rw-r--r--   0 rmasini    (501) staff       (20)     4238 2024-01-21 21:13:08.000000 binsreg-2.1.4/src/binsreg.egg-info/PKG-INFO
--rw-r--r--   0 rmasini    (501) staff       (20)      433 2024-01-21 21:13:08.000000 binsreg-2.1.4/src/binsreg.egg-info/SOURCES.txt
--rw-r--r--   0 rmasini    (501) staff       (20)        1 2024-01-21 21:13:08.000000 binsreg-2.1.4/src/binsreg.egg-info/dependency_links.txt
--rw-r--r--   0 rmasini    (501) staff       (20)       55 2024-01-21 21:13:08.000000 binsreg-2.1.4/src/binsreg.egg-info/requires.txt
--rw-r--r--   0 rmasini    (501) staff       (20)        8 2024-01-21 21:13:08.000000 binsreg-2.1.4/src/binsreg.egg-info/top_level.txt
-drwxr-xr-x   0 rmasini    (501) staff       (20)        0 2024-01-21 21:13:08.915508 binsreg-2.1.4/test/
--rw-r--r--   0 rmasini    (501) staff       (20)     5008 2021-09-06 17:46:18.000000 binsreg-2.1.4/test/test_funs.py
--rw-r--r--   0 rmasini    (501) staff       (20)     8799 2023-06-02 17:36:29.000000 binsreg-2.1.4/test/test_pkg.py
+drwxr-xr-x   0 rmasini    (501) staff       (20)        0 2024-05-23 15:40:14.913575 binsreg-2.1.5/
+-rw-r--r--   0 rmasini    (501) staff       (20)     4238 2024-05-23 15:40:14.913281 binsreg-2.1.5/PKG-INFO
+-rw-r--r--   0 rmasini    (501) staff       (20)     3512 2023-10-03 01:56:05.000000 binsreg-2.1.5/README.md
+-rw-r--r--   0 rmasini    (501) staff       (20)      108 2021-09-05 04:38:28.000000 binsreg-2.1.5/pyproject.toml
+-rw-r--r--   0 rmasini    (501) staff       (20)      823 2024-05-23 15:40:14.914313 binsreg-2.1.5/setup.cfg
+drwxr-xr-x   0 rmasini    (501) staff       (20)        0 2024-05-23 15:40:14.886297 binsreg-2.1.5/src/
+drwxr-xr-x   0 rmasini    (501) staff       (20)        0 2024-05-23 15:40:14.904276 binsreg-2.1.5/src/binsreg/
+-rw-r--r--   0 rmasini    (501) staff       (20)      189 2021-09-05 04:38:11.000000 binsreg-2.1.5/src/binsreg/__init__.py
+-rw-r--r--   0 rmasini    (501) staff       (20)    79486 2023-10-03 02:36:43.000000 binsreg-2.1.5/src/binsreg/binsglm.py
+-rw-r--r--   0 rmasini    (501) staff       (20)    42134 2023-10-03 02:36:08.000000 binsreg-2.1.5/src/binsreg/binspwc.py
+-rw-r--r--   0 rmasini    (501) staff       (20)    72759 2023-10-03 02:36:34.000000 binsreg-2.1.5/src/binsreg/binsqreg.py
+-rw-r--r--   0 rmasini    (501) staff       (20)    72413 2024-05-23 15:35:38.000000 binsreg-2.1.5/src/binsreg/binsreg.py
+-rw-r--r--   0 rmasini    (501) staff       (20)    24456 2023-10-03 02:36:57.000000 binsreg-2.1.5/src/binsreg/binsregselect.py
+-rw-r--r--   0 rmasini    (501) staff       (20)    46052 2023-10-03 02:36:00.000000 binsreg-2.1.5/src/binsreg/binstest.py
+-rw-r--r--   0 rmasini    (501) staff       (20)    60515 2024-01-30 17:28:25.000000 binsreg-2.1.5/src/binsreg/funs.py
+drwxr-xr-x   0 rmasini    (501) staff       (20)        0 2024-05-23 15:40:14.912150 binsreg-2.1.5/src/binsreg.egg-info/
+-rw-r--r--   0 rmasini    (501) staff       (20)     4238 2024-05-23 15:40:14.000000 binsreg-2.1.5/src/binsreg.egg-info/PKG-INFO
+-rw-r--r--   0 rmasini    (501) staff       (20)      433 2024-05-23 15:40:14.000000 binsreg-2.1.5/src/binsreg.egg-info/SOURCES.txt
+-rw-r--r--   0 rmasini    (501) staff       (20)        1 2024-05-23 15:40:14.000000 binsreg-2.1.5/src/binsreg.egg-info/dependency_links.txt
+-rw-r--r--   0 rmasini    (501) staff       (20)       55 2024-05-23 15:40:14.000000 binsreg-2.1.5/src/binsreg.egg-info/requires.txt
+-rw-r--r--   0 rmasini    (501) staff       (20)        8 2024-05-23 15:40:14.000000 binsreg-2.1.5/src/binsreg.egg-info/top_level.txt
+drwxr-xr-x   0 rmasini    (501) staff       (20)        0 2024-05-23 15:40:14.910756 binsreg-2.1.5/test/
+-rw-r--r--   0 rmasini    (501) staff       (20)     5008 2021-09-06 17:46:18.000000 binsreg-2.1.5/test/test_funs.py
+-rw-r--r--   0 rmasini    (501) staff       (20)     8799 2023-06-02 17:36:29.000000 binsreg-2.1.5/test/test_pkg.py
```

### Comparing `binsreg-2.1.4/PKG-INFO` & `binsreg-2.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: binsreg
-Version: 2.1.4
+Version: 2.1.5
 Summary: Implements binscatter methods, including partition selection, point estimation, pointwise and uniform inference methods, and graphical procedures.
 Home-page: https://github.com/nppackages/binsreg
 Author: Ricardo Masini
 Author-email: rmasini@princeton.edu
 Project-URL: Bug Tracker, https://github.com/nppackages/binsreg/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `binsreg-2.1.4/README.md` & `binsreg-2.1.5/README.md`

 * *Files identical despite different names*

### Comparing `binsreg-2.1.4/setup.cfg` & `binsreg-2.1.5/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = binsreg
-version = 2.1.4
+version = 2.1.5
 author = Ricardo Masini
 author_email = rmasini@princeton.edu
 description = Implements binscatter methods, including partition selection, point estimation, pointwise and uniform inference methods, and graphical procedures.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/nppackages/binsreg
 project_urls =
```

### Comparing `binsreg-2.1.4/src/binsreg/binsglm.py` & `binsreg-2.1.5/src/binsreg/binsglm.py`

 * *Files identical despite different names*

### Comparing `binsreg-2.1.4/src/binsreg/binspwc.py` & `binsreg-2.1.5/src/binsreg/binspwc.py`

 * *Files identical despite different names*

### Comparing `binsreg-2.1.4/src/binsreg/binsqreg.py` & `binsreg-2.1.5/src/binsreg/binsqreg.py`

 * *Files identical despite different names*

### Comparing `binsreg-2.1.4/src/binsreg/binsreg.py` & `binsreg-2.1.5/src/binsreg/binsreg.py`

 * *Files 1% similar despite different names*

```diff
@@ -298,14 +298,15 @@
                     imse_b_dpi : Bias constant in IMSE, DPI selection.
                     cval_by : A vector of critical values for constructing confidence band for each group.
                     options : A list containing options passed to the function, as well as N_by (total sample size for each group),
                               Ndist_by (number of distinct values in  x for each group), Nclust_by (number of clusters for each group),
                               and nbins_by (number of bins for each group), and byvals (number of distinct values in by).
                               The degree and smoothness of polynomials for dots, line, confidence intervals and confidence band for each group are saved
                               in dots, line, ci, and cb.
+        NOTE: The 'data_by' pandas dataframe index runs from 0 to nbins-1. However, the variable 'data_by.bin_id' runs from 1 to bins.
     
     See Also
     --------
     binsregselect, binsglm, binsqreg, binstest, binspwc.
     
     Example
     ------- 
@@ -1111,15 +1112,15 @@
         if w_sub is not None: 
             if isinstance(at, str):
                 if at=="mean":
                     eval_w = colWeightedMeans(x=w_sub, w=weights_sub)
                 elif at=="median":
                     eval_w = colWeightedMedians(x=w_sub, w=weights_sub)
                 elif at=="zero": eval_w = np.zeros(nwvar)
-            else: eval_w = np.array(at).reshape(-1,1)
+            else: eval_w = np.array(at).reshape(-1)
         else: eval_w = None
 
         ##################################
         # Dots and CIs for Small eN case
         ##################################
 
         if dotsmean+dotsgrid != 0 and fewobs:
```

### Comparing `binsreg-2.1.4/src/binsreg/binsregselect.py` & `binsreg-2.1.5/src/binsreg/binsregselect.py`

 * *Files identical despite different names*

### Comparing `binsreg-2.1.4/src/binsreg/binstest.py` & `binsreg-2.1.5/src/binsreg/binstest.py`

 * *Files identical despite different names*

### Comparing `binsreg-2.1.4/src/binsreg/funs.py` & `binsreg-2.1.5/src/binsreg/funs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1298,9 +1298,11 @@
     
     # bias constant
     imse_b = genB(y, x, w, p, s, deriv, knot, weights=weights) * J_rot**(2*(ord-deriv))
 
     # variance constant
     genV_val = genV(y, x, w, p, s, deriv, knot, vce, cluster, weights=weights)
     imse_v = genV_val / (J_rot**(1+2*deriv))
+    aux_num = (imse_b*2*(ord-deriv)/((1+2*deriv)*imse_v))
+    aux= np.ceil((imse_b*2*(ord-deriv)/((1+2*deriv)*imse_v))**(1/(2*ord+1)))
     J_dpi = int(np.ceil((imse_b*2*(ord-deriv)/((1+2*deriv)*imse_v))**(1/(2*ord+1))))
     return J_dpi, imse_v, imse_b
```

### Comparing `binsreg-2.1.4/src/binsreg.egg-info/PKG-INFO` & `binsreg-2.1.5/src/binsreg.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: binsreg
-Version: 2.1.4
+Version: 2.1.5
 Summary: Implements binscatter methods, including partition selection, point estimation, pointwise and uniform inference methods, and graphical procedures.
 Home-page: https://github.com/nppackages/binsreg
 Author: Ricardo Masini
 Author-email: rmasini@princeton.edu
 Project-URL: Bug Tracker, https://github.com/nppackages/binsreg/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `binsreg-2.1.4/test/test_funs.py` & `binsreg-2.1.5/test/test_funs.py`

 * *Files identical despite different names*

### Comparing `binsreg-2.1.4/test/test_pkg.py` & `binsreg-2.1.5/test/test_pkg.py`

 * *Files identical despite different names*

