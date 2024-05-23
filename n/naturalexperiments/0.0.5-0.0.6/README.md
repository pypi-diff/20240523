# Comparing `tmp/naturalexperiments-0.0.5.tar.gz` & `tmp/naturalexperiments-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "naturalexperiments-0.0.5.tar", last modified: Thu May 23 12:06:27 2024, max compression
+gzip compressed data, was "naturalexperiments-0.0.6.tar", last modified: Thu May 23 12:24:04 2024, max compression
```

## Comparing `naturalexperiments-0.0.5.tar` & `naturalexperiments-0.0.6.tar`

### file list

```diff
@@ -1,46 +1,45 @@
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 12:06:27.997515 naturalexperiments-0.0.5/
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1071 2024-05-22 20:16:39.000000 naturalexperiments-0.0.5/LICENSE
--rw-r--r--   0 rtealwitter   (501) staff       (20)      604 2024-05-23 12:06:27.997328 naturalexperiments-0.0.5/PKG-INFO
--rw-r--r--   0 rtealwitter   (501) staff       (20)      101 2024-05-22 20:16:39.000000 naturalexperiments-0.0.5/README.md
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 12:06:27.988552 naturalexperiments-0.0.5/naturalexperiments/
--rw-r--r--   0 rtealwitter   (501) staff       (20)      120 2024-05-22 20:42:14.000000 naturalexperiments-0.0.5/naturalexperiments/__init__.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)    11440 2024-05-22 20:42:14.000000 naturalexperiments-0.0.5/naturalexperiments/benchmark.py
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 12:06:27.989408 naturalexperiments-0.0.5/naturalexperiments/data/
--rw-r--r--   0 rtealwitter   (501) staff       (20)      338 2024-05-22 20:42:14.000000 naturalexperiments-0.0.5/naturalexperiments/data/__init__.py
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 12:06:27.989941 naturalexperiments-0.0.5/naturalexperiments/data/acic/
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1988 2024-05-22 21:47:02.000000 naturalexperiments-0.0.5/naturalexperiments/data/acic/__init__.py
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 12:06:27.990159 naturalexperiments-0.0.5/naturalexperiments/data/ihdp/
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1553 2024-05-23 00:23:10.000000 naturalexperiments-0.0.5/naturalexperiments/data/ihdp/__init__.py
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 12:06:27.990423 naturalexperiments-0.0.5/naturalexperiments/data/jobs/
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1356 2024-05-23 00:17:37.000000 naturalexperiments-0.0.5/naturalexperiments/data/jobs/__init__.py
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 12:06:27.990698 naturalexperiments-0.0.5/naturalexperiments/data/news/
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1436 2024-05-23 11:56:32.000000 naturalexperiments-0.0.5/naturalexperiments/data/news/__init__.py
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 12:06:27.991182 naturalexperiments-0.0.5/naturalexperiments/data/rorco/
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1215 2024-05-22 21:42:52.000000 naturalexperiments-0.0.5/naturalexperiments/data/rorco/__init__.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)    15535 2024-05-22 21:34:07.000000 naturalexperiments-0.0.5/naturalexperiments/data/rorco/rorco_preprocess.py
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 12:06:27.991443 naturalexperiments-0.0.5/naturalexperiments/data/twins/
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1810 2024-05-23 12:04:17.000000 naturalexperiments-0.0.5/naturalexperiments/data/twins/__init__.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)     5996 2024-05-22 20:42:14.000000 naturalexperiments-0.0.5/naturalexperiments/data_summary.py
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 12:06:27.994772 naturalexperiments-0.0.5/naturalexperiments/estimators/
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1545 2024-05-22 20:42:14.000000 naturalexperiments-0.0.5/naturalexperiments/estimators/__init__.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)      683 2024-05-22 20:42:14.000000 naturalexperiments-0.0.5/naturalexperiments/estimators/catenet.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)      136 2024-05-22 20:42:14.000000 naturalexperiments-0.0.5/naturalexperiments/estimators/direct_difference.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)      330 2024-05-22 20:42:14.000000 naturalexperiments-0.0.5/naturalexperiments/estimators/direct_prediction.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1750 2024-05-22 20:42:14.000000 naturalexperiments-0.0.5/naturalexperiments/estimators/double_double.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)      629 2024-05-22 20:42:14.000000 naturalexperiments-0.0.5/naturalexperiments/estimators/doubly_robust.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)      138 2024-05-22 20:42:14.000000 naturalexperiments-0.0.5/naturalexperiments/estimators/horvitz_thompson.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)      234 2024-05-22 20:42:14.000000 naturalexperiments-0.0.5/naturalexperiments/estimators/learned_direct.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1419 2024-05-22 20:42:14.000000 naturalexperiments-0.0.5/naturalexperiments/estimators/off_policy.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)      488 2024-05-22 20:42:14.000000 naturalexperiments-0.0.5/naturalexperiments/estimators/propensity_stratification.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)      436 2024-05-22 20:42:14.000000 naturalexperiments-0.0.5/naturalexperiments/estimators/regression_discontinuity.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)      872 2024-05-22 20:42:14.000000 naturalexperiments-0.0.5/naturalexperiments/estimators/tmle.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)     3438 2024-05-22 20:42:14.000000 naturalexperiments-0.0.5/naturalexperiments/model.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)      507 2024-05-23 12:05:42.000000 naturalexperiments-0.0.5/naturalexperiments/test.py
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1662 2024-05-22 20:42:14.000000 naturalexperiments-0.0.5/naturalexperiments/utils.py
-drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 12:06:27.995028 naturalexperiments-0.0.5/naturalexperiments.egg-info/
--rw-r--r--   0 rtealwitter   (501) staff       (20)      604 2024-05-23 12:06:27.000000 naturalexperiments-0.0.5/naturalexperiments.egg-info/PKG-INFO
--rw-r--r--   0 rtealwitter   (501) staff       (20)     1285 2024-05-23 12:06:27.000000 naturalexperiments-0.0.5/naturalexperiments.egg-info/SOURCES.txt
--rw-r--r--   0 rtealwitter   (501) staff       (20)        1 2024-05-23 12:06:27.000000 naturalexperiments-0.0.5/naturalexperiments.egg-info/dependency_links.txt
--rw-r--r--   0 rtealwitter   (501) staff       (20)       19 2024-05-23 12:06:27.000000 naturalexperiments-0.0.5/naturalexperiments.egg-info/top_level.txt
--rw-r--r--   0 rtealwitter   (501) staff       (20)       38 2024-05-23 12:06:27.997559 naturalexperiments-0.0.5/setup.cfg
--rw-r--r--   0 rtealwitter   (501) staff       (20)      719 2024-05-23 12:05:22.000000 naturalexperiments-0.0.5/setup.py
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 12:24:04.846246 naturalexperiments-0.0.6/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     1071 2024-05-22 20:16:39.000000 naturalexperiments-0.0.6/LICENSE
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      604 2024-05-23 12:24:04.846032 naturalexperiments-0.0.6/PKG-INFO
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      101 2024-05-22 20:16:39.000000 naturalexperiments-0.0.6/README.md
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 12:24:04.842299 naturalexperiments-0.0.6/naturalexperiments/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      120 2024-05-22 20:42:14.000000 naturalexperiments-0.0.6/naturalexperiments/__init__.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)    11440 2024-05-22 20:42:14.000000 naturalexperiments-0.0.6/naturalexperiments/benchmark.py
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 12:24:04.843003 naturalexperiments-0.0.6/naturalexperiments/data/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      338 2024-05-22 20:42:14.000000 naturalexperiments-0.0.6/naturalexperiments/data/__init__.py
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 12:24:04.843142 naturalexperiments-0.0.6/naturalexperiments/data/acic/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     1988 2024-05-22 21:47:02.000000 naturalexperiments-0.0.6/naturalexperiments/data/acic/__init__.py
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 12:24:04.843273 naturalexperiments-0.0.6/naturalexperiments/data/ihdp/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     1553 2024-05-23 00:23:10.000000 naturalexperiments-0.0.6/naturalexperiments/data/ihdp/__init__.py
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 12:24:04.843403 naturalexperiments-0.0.6/naturalexperiments/data/jobs/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     1356 2024-05-23 00:17:37.000000 naturalexperiments-0.0.6/naturalexperiments/data/jobs/__init__.py
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 12:24:04.843526 naturalexperiments-0.0.6/naturalexperiments/data/news/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     1436 2024-05-23 11:56:32.000000 naturalexperiments-0.0.6/naturalexperiments/data/news/__init__.py
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 12:24:04.843781 naturalexperiments-0.0.6/naturalexperiments/data/rorco/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     1215 2024-05-22 21:42:52.000000 naturalexperiments-0.0.6/naturalexperiments/data/rorco/__init__.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)    15535 2024-05-22 21:34:07.000000 naturalexperiments-0.0.6/naturalexperiments/data/rorco/rorco_preprocess.py
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 12:24:04.844030 naturalexperiments-0.0.6/naturalexperiments/data/twins/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     1810 2024-05-23 12:04:17.000000 naturalexperiments-0.0.6/naturalexperiments/data/twins/__init__.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     6139 2024-05-23 12:21:06.000000 naturalexperiments-0.0.6/naturalexperiments/data_summary.py
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 12:24:04.845664 naturalexperiments-0.0.6/naturalexperiments/estimators/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     1545 2024-05-22 20:42:14.000000 naturalexperiments-0.0.6/naturalexperiments/estimators/__init__.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      683 2024-05-22 20:42:14.000000 naturalexperiments-0.0.6/naturalexperiments/estimators/catenet.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      136 2024-05-22 20:42:14.000000 naturalexperiments-0.0.6/naturalexperiments/estimators/direct_difference.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      330 2024-05-22 20:42:14.000000 naturalexperiments-0.0.6/naturalexperiments/estimators/direct_prediction.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     1750 2024-05-22 20:42:14.000000 naturalexperiments-0.0.6/naturalexperiments/estimators/double_double.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      629 2024-05-22 20:42:14.000000 naturalexperiments-0.0.6/naturalexperiments/estimators/doubly_robust.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      138 2024-05-22 20:42:14.000000 naturalexperiments-0.0.6/naturalexperiments/estimators/horvitz_thompson.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      234 2024-05-22 20:42:14.000000 naturalexperiments-0.0.6/naturalexperiments/estimators/learned_direct.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     1419 2024-05-22 20:42:14.000000 naturalexperiments-0.0.6/naturalexperiments/estimators/off_policy.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      488 2024-05-22 20:42:14.000000 naturalexperiments-0.0.6/naturalexperiments/estimators/propensity_stratification.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      436 2024-05-22 20:42:14.000000 naturalexperiments-0.0.6/naturalexperiments/estimators/regression_discontinuity.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      872 2024-05-22 20:42:14.000000 naturalexperiments-0.0.6/naturalexperiments/estimators/tmle.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     3438 2024-05-22 20:42:14.000000 naturalexperiments-0.0.6/naturalexperiments/model.py
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     1662 2024-05-22 20:42:14.000000 naturalexperiments-0.0.6/naturalexperiments/utils.py
+drwxr-xr-x   0 rtealwitter   (501) staff       (20)        0 2024-05-23 12:24:04.845834 naturalexperiments-0.0.6/naturalexperiments.egg-info/
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      604 2024-05-23 12:24:04.000000 naturalexperiments-0.0.6/naturalexperiments.egg-info/PKG-INFO
+-rw-r--r--   0 rtealwitter   (501) staff       (20)     1258 2024-05-23 12:24:04.000000 naturalexperiments-0.0.6/naturalexperiments.egg-info/SOURCES.txt
+-rw-r--r--   0 rtealwitter   (501) staff       (20)        1 2024-05-23 12:24:04.000000 naturalexperiments-0.0.6/naturalexperiments.egg-info/dependency_links.txt
+-rw-r--r--   0 rtealwitter   (501) staff       (20)       19 2024-05-23 12:24:04.000000 naturalexperiments-0.0.6/naturalexperiments.egg-info/top_level.txt
+-rw-r--r--   0 rtealwitter   (501) staff       (20)       38 2024-05-23 12:24:04.846289 naturalexperiments-0.0.6/setup.cfg
+-rw-r--r--   0 rtealwitter   (501) staff       (20)      719 2024-05-23 12:23:25.000000 naturalexperiments-0.0.6/setup.py
```

### Comparing `naturalexperiments-0.0.5/LICENSE` & `naturalexperiments-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.5/PKG-INFO` & `naturalexperiments-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naturalexperiments
-Version: 0.0.5
+Version: 0.0.6
 Summary: Estimators and datasets for treatment effect estimation in natural experiments.
 Home-page: https://github.com/rtealwitter/naturalexperiments
 Author: R. Teal Witter
 Author-email: rtealwitter@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `naturalexperiments-0.0.5/naturalexperiments/benchmark.py` & `naturalexperiments-0.0.6/naturalexperiments/benchmark.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.5/naturalexperiments/data/acic/__init__.py` & `naturalexperiments-0.0.6/naturalexperiments/data/acic/__init__.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.5/naturalexperiments/data/ihdp/__init__.py` & `naturalexperiments-0.0.6/naturalexperiments/data/ihdp/__init__.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.5/naturalexperiments/data/jobs/__init__.py` & `naturalexperiments-0.0.6/naturalexperiments/data/jobs/__init__.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.5/naturalexperiments/data/news/__init__.py` & `naturalexperiments-0.0.6/naturalexperiments/data/news/__init__.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.5/naturalexperiments/data/rorco/__init__.py` & `naturalexperiments-0.0.6/naturalexperiments/data/rorco/__init__.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.5/naturalexperiments/data/rorco/rorco_preprocess.py` & `naturalexperiments-0.0.6/naturalexperiments/data/rorco/rorco_preprocess.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.5/naturalexperiments/data/twins/__init__.py` & `naturalexperiments-0.0.6/naturalexperiments/data/twins/__init__.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.5/naturalexperiments/data_summary.py` & `naturalexperiments-0.0.6/naturalexperiments/data_summary.py`

 * *Files 5% similar despite different names*

```diff
@@ -93,21 +93,21 @@
     if z is not None:
         propensity = estimate_propensity(X, z)
 
     else:
         beta = np.random.normal(size=X.shape[1])
         var = X @ beta
         propensity = (var - var.min() ) / (var.max() - var.min())
-        propensity = np.clip(propensity.values, 0.01,.99)
+        propensity = np.clip(propensity, 0.01,.99)
         # Sample z from a Bernoulli distribution with propensity
         z = np.random.binomial(1, propensity)
     
     return propensity, z
 
-def plot_all_data(dataloaders, folder='../images/'):
+def plot_all_data(dataloaders, folder=''):
     for dataname, dataloader in dataloaders.items(): 
         X, y, z = dataloader()
 
         propensity, z = wrap_estimate_propensity(X, z)
 
         plot_propensity(propensity, dataname, filename=folder+'propensity_hist_'+dataname+'.pdf')
         plot_propensity_calibration(propensity, z, dataname, filename=folder+'propensity_calibration_'+dataname+'.pdf')
@@ -125,16 +125,18 @@
         # Number of variables
         m = X.shape[1]
         # Percent treated 
         rate_treated = sig_round(np.mean(z) * 100)
         # Cross entropy of propensity score and z
         cross_entropy = sig_round(compute_cross_entropy(propensity, z))
         # Correlation between propensity and y1
+        #corr_y1 = sig_round(np.corrcoef(propensity[z==1], y['y1'][z==1])[0,1])
         corr_y1 = sig_round(compute_distance_correlation(propensity[z==1], y['y1'][z==1].values))
         # Correlation between propensity and y0
+        #corr_y0 = sig_round(np.corrcoef(propensity[z==0], y['y0'][z==0])[0,1])
         corr_y0 = sig_round(compute_distance_correlation(propensity[z==0], y['y0'][z==0].values))
 
         table += [[dataname, n, m, rate_treated, cross_entropy, corr_y1, corr_y0]]
 
     headers = ['Dataset', 'Size', 'Variables', '% Treated', 'Cross Entropy', 'Corr(y1, p)', 'Corr(y0, p)']
 
     if print_md:
```

### Comparing `naturalexperiments-0.0.5/naturalexperiments/estimators/__init__.py` & `naturalexperiments-0.0.6/naturalexperiments/estimators/__init__.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.5/naturalexperiments/estimators/catenet.py` & `naturalexperiments-0.0.6/naturalexperiments/estimators/catenet.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.5/naturalexperiments/estimators/double_double.py` & `naturalexperiments-0.0.6/naturalexperiments/estimators/double_double.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.5/naturalexperiments/estimators/doubly_robust.py` & `naturalexperiments-0.0.6/naturalexperiments/estimators/doubly_robust.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.5/naturalexperiments/estimators/off_policy.py` & `naturalexperiments-0.0.6/naturalexperiments/estimators/off_policy.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.5/naturalexperiments/estimators/tmle.py` & `naturalexperiments-0.0.6/naturalexperiments/estimators/tmle.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.5/naturalexperiments/model.py` & `naturalexperiments-0.0.6/naturalexperiments/model.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.5/naturalexperiments/utils.py` & `naturalexperiments-0.0.6/naturalexperiments/utils.py`

 * *Files identical despite different names*

### Comparing `naturalexperiments-0.0.5/naturalexperiments.egg-info/PKG-INFO` & `naturalexperiments-0.0.6/naturalexperiments.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: naturalexperiments
-Version: 0.0.5
+Version: 0.0.6
 Summary: Estimators and datasets for treatment effect estimation in natural experiments.
 Home-page: https://github.com/rtealwitter/naturalexperiments
 Author: R. Teal Witter
 Author-email: rtealwitter@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `naturalexperiments-0.0.5/naturalexperiments.egg-info/SOURCES.txt` & `naturalexperiments-0.0.6/naturalexperiments.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 LICENSE
 README.md
 setup.py
 naturalexperiments/__init__.py
 naturalexperiments/benchmark.py
 naturalexperiments/data_summary.py
 naturalexperiments/model.py
-naturalexperiments/test.py
 naturalexperiments/utils.py
 naturalexperiments.egg-info/PKG-INFO
 naturalexperiments.egg-info/SOURCES.txt
 naturalexperiments.egg-info/dependency_links.txt
 naturalexperiments.egg-info/top_level.txt
 naturalexperiments/data/__init__.py
 naturalexperiments/data/acic/__init__.py
```

### Comparing `naturalexperiments-0.0.5/setup.py` & `naturalexperiments-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="naturalexperiments",
-    version="0.0.5",
+    version="0.0.6",
     author="R. Teal Witter",
     author_email="rtealwitter@gmail.com",
     description="Estimators and datasets for treatment effect estimation in natural experiments.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/rtealwitter/naturalexperiments",
     packages=setuptools.find_packages(),
```

