# Comparing `tmp/phdu-2.4.4.tar.gz` & `tmp/phdu-2.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phdu-2.4.4.tar", last modified: Wed May 22 12:23:13 2024, max compression
+gzip compressed data, was "phdu-2.4.5.tar", last modified: Thu May 23 07:46:08 2024, max compression
```

## Comparing `phdu-2.4.4.tar` & `phdu-2.4.5.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2024-05-22 12:23:13.783862 phdu-2.4.4/
--rw-r--r--   0 jorgemedina  (1236) users      (100)    35149 2022-11-08 11:52:59.000000 phdu-2.4.4/LICENSE.md
--rw-r--r--   0 jorgemedina  (1236) users      (100)     2864 2024-05-22 12:23:13.783862 phdu-2.4.4/PKG-INFO
--rw-r--r--   0 jorgemedina  (1236) users      (100)     1771 2023-03-07 15:21:19.000000 phdu-2.4.4/README.md
-drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2024-05-22 12:23:13.591851 phdu-2.4.4/phdu/
--rw-r--r--   0 jorgemedina  (1236) users      (100)      590 2024-04-05 11:52:28.000000 phdu-2.4.4/phdu/__init__.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     1948 2023-10-04 09:21:45.000000 phdu-2.4.4/phdu/_helper.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     2484 2024-04-05 11:52:28.000000 phdu-2.4.4/phdu/analysis.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     3664 2023-10-19 13:00:53.000000 phdu-2.4.4/phdu/clustering.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     3319 2023-03-14 10:06:15.000000 phdu-2.4.4/phdu/decomposition.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     1333 2024-04-05 11:52:28.000000 phdu-2.4.4/phdu/geometry.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     3183 2024-04-05 11:52:28.000000 phdu-2.4.4/phdu/np_utils.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     6214 2024-04-09 08:31:50.000000 phdu-2.4.4/phdu/pd_utils.py
-drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2024-05-22 12:23:13.659855 phdu-2.4.4/phdu/plots/
--rw-r--r--   0 jorgemedina  (1236) users      (100)       66 2022-11-08 18:00:13.000000 phdu-2.4.4/phdu/plots/__init__.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)        0 2022-11-08 08:30:49.000000 phdu-2.4.4/phdu/plots/_mpl.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     4011 2023-10-19 15:28:08.000000 phdu-2.4.4/phdu/plots/base.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)    23398 2024-05-22 12:22:56.000000 phdu-2.4.4/phdu/plots/plotly_utils.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     3978 2023-03-10 11:02:11.000000 phdu-2.4.4/phdu/script_fmt.py
-drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2024-05-22 12:23:13.727859 phdu-2.4.4/phdu/stats/
--rw-r--r--   0 jorgemedina  (1236) users      (100)      157 2023-03-16 13:28:14.000000 phdu-2.4.4/phdu/stats/__init__.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     2526 2023-02-15 09:17:23.000000 phdu-2.4.4/phdu/stats/_integration.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)      842 2023-04-25 08:51:47.000000 phdu-2.4.4/phdu/stats/_plots.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)      343 2022-11-08 15:54:46.000000 phdu-2.4.4/phdu/stats/_preprocess.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)    33588 2024-05-09 10:51:00.000000 phdu-2.4.4/phdu/stats/bootstrap.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     9411 2023-03-20 23:41:28.000000 phdu-2.4.4/phdu/stats/conf_interval.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)      643 2023-03-16 13:27:55.000000 phdu-2.4.4/phdu/stats/corr.py
-drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2024-05-22 12:23:13.755861 phdu-2.4.4/phdu/stats/rtopy/
--rw-r--r--   0 jorgemedina  (1236) users      (100)       22 2022-11-08 08:30:50.000000 phdu-2.4.4/phdu/stats/rtopy/__init__.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     1306 2022-11-08 18:28:33.000000 phdu-2.4.4/phdu/stats/rtopy/_helper.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     4755 2022-11-08 16:42:50.000000 phdu-2.4.4/phdu/stats/rtopy/resample.py
-drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2024-05-22 12:23:13.779862 phdu-2.4.4/phdu/stats/test/
--rw-r--r--   0 jorgemedina  (1236) users      (100)       25 2022-11-08 11:59:20.000000 phdu-2.4.4/phdu/stats/test/__init__.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)      279 2022-11-08 14:38:29.000000 phdu-2.4.4/phdu/stats/test/_adherence.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)    16550 2023-03-07 15:36:38.000000 phdu-2.4.4/phdu/stats/test/permutation.py
--rw-r--r--   0 jorgemedina  (1236) users      (100)     4437 2024-04-05 11:52:28.000000 phdu-2.4.4/phdu/storage.py
-drwxr-xr-x   0 jorgemedina  (1236) users      (100)        0 2024-05-22 12:23:13.631853 phdu-2.4.4/phdu.egg-info/
--rw-r--r--   0 jorgemedina  (1236) users      (100)     2864 2024-05-22 12:23:13.000000 phdu-2.4.4/phdu.egg-info/PKG-INFO
--rw-r--r--   0 jorgemedina  (1236) users      (100)      786 2024-05-22 12:23:13.000000 phdu-2.4.4/phdu.egg-info/SOURCES.txt
--rw-r--r--   0 jorgemedina  (1236) users      (100)        1 2024-05-22 12:23:13.000000 phdu-2.4.4/phdu.egg-info/dependency_links.txt
--rw-r--r--   0 jorgemedina  (1236) users      (100)      302 2024-05-22 12:23:13.000000 phdu-2.4.4/phdu.egg-info/requires.txt
--rw-r--r--   0 jorgemedina  (1236) users      (100)        5 2024-05-22 12:23:13.000000 phdu-2.4.4/phdu.egg-info/top_level.txt
--rw-r--r--   0 jorgemedina  (1236) users      (100)      106 2024-05-22 12:23:13.791863 phdu-2.4.4/setup.cfg
--rw-r--r--   0 jorgemedina  (1236) users      (100)     1659 2024-05-22 12:23:05.000000 phdu-2.4.4/setup.py
+drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2024-05-23 07:46:08.722937 phdu-2.4.5/
+-rw-r--r--   0 userx     (1000) wheel      (998)    35149 2023-07-31 18:53:26.000000 phdu-2.4.5/LICENSE.md
+-rw-r--r--   0 userx     (1000) wheel      (998)     2864 2024-05-23 07:46:08.722937 phdu-2.4.5/PKG-INFO
+-rw-r--r--   0 userx     (1000) wheel      (998)     1771 2023-07-31 18:53:26.000000 phdu-2.4.5/README.md
+drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2024-05-23 07:46:08.719604 phdu-2.4.5/phdu/
+-rw-r--r--   0 userx     (1000) wheel      (998)      590 2024-02-24 02:21:10.000000 phdu-2.4.5/phdu/__init__.py
+-rw-r--r--   0 userx     (1000) wheel      (998)     1948 2023-09-21 17:52:42.000000 phdu-2.4.5/phdu/_helper.py
+-rw-r--r--   0 userx     (1000) wheel      (998)     2484 2024-02-04 05:18:27.000000 phdu-2.4.5/phdu/analysis.py
+-rw-r--r--   0 userx     (1000) wheel      (998)     3664 2023-10-17 21:07:41.000000 phdu-2.4.5/phdu/clustering.py
+-rw-r--r--   0 userx     (1000) wheel      (998)     3319 2023-07-31 18:53:27.000000 phdu-2.4.5/phdu/decomposition.py
+-rw-r--r--   0 userx     (1000) wheel      (998)     1333 2023-12-05 04:36:26.000000 phdu-2.4.5/phdu/geometry.py
+-rw-r--r--   0 userx     (1000) wheel      (998)     3183 2024-01-23 06:00:25.000000 phdu-2.4.5/phdu/np_utils.py
+-rw-r--r--   0 userx     (1000) wheel      (998)     6214 2024-04-07 07:28:04.000000 phdu-2.4.5/phdu/pd_utils.py
+drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2024-05-23 07:46:08.719604 phdu-2.4.5/phdu/plots/
+-rw-r--r--   0 userx     (1000) wheel      (998)       66 2023-07-31 18:53:27.000000 phdu-2.4.5/phdu/plots/__init__.py
+-rw-r--r--   0 userx     (1000) wheel      (998)        0 2023-07-31 18:53:27.000000 phdu-2.4.5/phdu/plots/_mpl.py
+-rw-r--r--   0 userx     (1000) wheel      (998)     4011 2023-12-05 02:04:31.000000 phdu-2.4.5/phdu/plots/base.py
+-rw-r--r--   0 userx     (1000) wheel      (998)    23398 2024-05-23 07:45:22.000000 phdu-2.4.5/phdu/plots/plotly_utils.py
+-rw-r--r--   0 userx     (1000) wheel      (998)     3978 2023-07-31 18:53:27.000000 phdu-2.4.5/phdu/script_fmt.py
+drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2024-05-23 07:46:08.722937 phdu-2.4.5/phdu/stats/
+-rw-r--r--   0 userx     (1000) wheel      (998)      157 2023-07-31 18:53:27.000000 phdu-2.4.5/phdu/stats/__init__.py
+-rw-r--r--   0 userx     (1000) wheel      (998)     2526 2023-07-31 18:53:27.000000 phdu-2.4.5/phdu/stats/_integration.py
+-rw-r--r--   0 userx     (1000) wheel      (998)      842 2023-07-31 18:53:27.000000 phdu-2.4.5/phdu/stats/_plots.py
+-rw-r--r--   0 userx     (1000) wheel      (998)      343 2023-07-31 18:53:27.000000 phdu-2.4.5/phdu/stats/_preprocess.py
+-rw-r--r--   0 userx     (1000) wheel      (998)    33588 2024-05-23 07:45:54.000000 phdu-2.4.5/phdu/stats/bootstrap.py
+-rw-r--r--   0 userx     (1000) wheel      (998)     9411 2023-07-31 18:53:27.000000 phdu-2.4.5/phdu/stats/conf_interval.py
+-rw-r--r--   0 userx     (1000) wheel      (998)      643 2023-07-31 18:53:27.000000 phdu-2.4.5/phdu/stats/corr.py
+drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2024-05-23 07:46:08.722937 phdu-2.4.5/phdu/stats/rtopy/
+-rw-r--r--   0 userx     (1000) wheel      (998)       22 2023-07-31 18:53:27.000000 phdu-2.4.5/phdu/stats/rtopy/__init__.py
+-rw-r--r--   0 userx     (1000) wheel      (998)     1306 2023-07-31 18:53:27.000000 phdu-2.4.5/phdu/stats/rtopy/_helper.py
+-rw-r--r--   0 userx     (1000) wheel      (998)     4755 2023-07-31 18:53:27.000000 phdu-2.4.5/phdu/stats/rtopy/resample.py
+drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2024-05-23 07:46:08.722937 phdu-2.4.5/phdu/stats/test/
+-rw-r--r--   0 userx     (1000) wheel      (998)       25 2023-07-31 18:53:27.000000 phdu-2.4.5/phdu/stats/test/__init__.py
+-rw-r--r--   0 userx     (1000) wheel      (998)      279 2023-07-31 18:53:27.000000 phdu-2.4.5/phdu/stats/test/_adherence.py
+-rw-r--r--   0 userx     (1000) wheel      (998)    16550 2023-07-31 18:53:27.000000 phdu-2.4.5/phdu/stats/test/permutation.py
+-rw-r--r--   0 userx     (1000) wheel      (998)     4437 2024-02-24 02:19:42.000000 phdu-2.4.5/phdu/storage.py
+drwxr-xr-x   0 userx     (1000) wheel      (998)        0 2024-05-23 07:46:08.719604 phdu-2.4.5/phdu.egg-info/
+-rwxr-xr-x   0 userx     (1000) wheel      (998)     2864 2024-05-23 07:46:08.000000 phdu-2.4.5/phdu.egg-info/PKG-INFO
+-rwxr-xr-x   0 userx     (1000) wheel      (998)      786 2024-05-23 07:46:08.000000 phdu-2.4.5/phdu.egg-info/SOURCES.txt
+-rwxr-xr-x   0 userx     (1000) wheel      (998)        1 2024-05-23 07:46:08.000000 phdu-2.4.5/phdu.egg-info/dependency_links.txt
+-rwxr-xr-x   0 userx     (1000) wheel      (998)      302 2024-05-23 07:46:08.000000 phdu-2.4.5/phdu.egg-info/requires.txt
+-rwxr-xr-x   0 userx     (1000) wheel      (998)        5 2024-05-23 07:46:08.000000 phdu-2.4.5/phdu.egg-info/top_level.txt
+-rw-r--r--   0 userx     (1000) wheel      (998)      106 2024-05-23 07:46:08.726270 phdu-2.4.5/setup.cfg
+-rw-r--r--   0 userx     (1000) wheel      (998)     1659 2024-05-23 07:46:03.000000 phdu-2.4.5/setup.py
```

### Comparing `phdu-2.4.4/LICENSE.md` & `phdu-2.4.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `phdu-2.4.4/PKG-INFO` & `phdu-2.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phdu
-Version: 2.4.4
+Version: 2.4.5
 Summary: Automatically store/load data in a tidy, efficient way. Includes functions for data visualization and analysis.
 Home-page: https://github.com/medinajorge/PhD-utils
 Download-URL: https://github.com/medinajorge/PhD-utils/archive/refs/tags/v1.5-beta.tar.gz
 Author: Jorge Medina Hernández
 Author-email: medinahdezjorge@gmail.com
 Keywords: science,statistics,tidy,project organization,project,organization,path,storage
 Classifier: Programming Language :: Python :: 3
```

### Comparing `phdu-2.4.4/README.md` & `phdu-2.4.5/README.md`

 * *Files identical despite different names*

### Comparing `phdu-2.4.4/phdu/__init__.py` & `phdu-2.4.5/phdu/__init__.py`

 * *Files identical despite different names*

### Comparing `phdu-2.4.4/phdu/_helper.py` & `phdu-2.4.5/phdu/_helper.py`

 * *Files identical despite different names*

### Comparing `phdu-2.4.4/phdu/analysis.py` & `phdu-2.4.5/phdu/analysis.py`

 * *Files identical despite different names*

### Comparing `phdu-2.4.4/phdu/clustering.py` & `phdu-2.4.5/phdu/clustering.py`

 * *Files identical despite different names*

### Comparing `phdu-2.4.4/phdu/decomposition.py` & `phdu-2.4.5/phdu/decomposition.py`

 * *Files identical despite different names*

### Comparing `phdu-2.4.4/phdu/geometry.py` & `phdu-2.4.5/phdu/geometry.py`

 * *Files identical despite different names*

### Comparing `phdu-2.4.4/phdu/np_utils.py` & `phdu-2.4.5/phdu/np_utils.py`

 * *Files identical despite different names*

### Comparing `phdu-2.4.4/phdu/pd_utils.py` & `phdu-2.4.5/phdu/pd_utils.py`

 * *Files identical despite different names*

### Comparing `phdu-2.4.4/phdu/plots/base.py` & `phdu-2.4.5/phdu/plots/base.py`

 * *Files identical despite different names*

### Comparing `phdu-2.4.4/phdu/plots/plotly_utils.py` & `phdu-2.4.5/phdu/plots/plotly_utils.py`

 * *Files identical despite different names*

### Comparing `phdu-2.4.4/phdu/script_fmt.py` & `phdu-2.4.5/phdu/script_fmt.py`

 * *Files identical despite different names*

### Comparing `phdu-2.4.4/phdu/stats/_integration.py` & `phdu-2.4.5/phdu/stats/_integration.py`

 * *Files identical despite different names*

### Comparing `phdu-2.4.4/phdu/stats/_plots.py` & `phdu-2.4.5/phdu/stats/_plots.py`

 * *Files identical despite different names*

### Comparing `phdu-2.4.4/phdu/stats/bootstrap.py` & `phdu-2.4.5/phdu/stats/bootstrap.py`

 * *Files 0% similar despite different names*

```diff
@@ -295,15 +295,15 @@
     """
     B = a.shape[axis]
     if account_equal:
         return ((a < score).sum(axis=axis) + (a <= score).sum(axis=axis)) / (2 * B)
     else:
         return (a < score).sum(axis=axis) / B
 
-def _resample(data, data2, use_numba, statistic, R, n_min=5, smooth=False, aggregator=_nb_mean, **kwargs):
+def _resample(data, data2, use_numba, statistic, R, n_min=1, smooth=False, aggregator=_nb_mean, **kwargs):
     """
     Resample using normal resampling if data2 is None.
     Else uses block resampling with data and data2.
     """
     if data2 is None:
         if data.ndim == 1:
             data = data[:, None]
@@ -357,15 +357,15 @@
         else:
             theta_hat_b = resample_func(data, data2, statistic, R=R, output_len=output_len, **resample_kwargs, **kwargs).squeeze()
             # if stack_data and is_block:
             #     data = np.hstack(data)
             #     data2 = np.hstack(data2)
     return data, data2, theta_hat_b, sample_stat, N
 
-def CI_bca(data, statistic, data2=None, alternative='two-sided', alpha=0.05, R=int(1e5), account_equal=False, use_numba=True, n_min=5, aggregator=_nb_mean, **kwargs):
+def CI_bca(data, statistic, data2=None, alternative='two-sided', alpha=0.05, R=int(1e5), account_equal=False, use_numba=True, n_min=1, aggregator=_nb_mean, **kwargs):
     """
     If data2 is provided, assumes a block resampling and statistic takes two arguments.
     Optional kwargs for aggregating data, data2 before computing the statistic:
             aggregator = @njit
                          def nb_mean(x):
                              return np.mean(x)
     """
@@ -590,15 +590,15 @@
         CI = np.vstack((-np.inf * np.ones((output_len)), np.percentile(boot_sample, alpha_ptg[0] if alpha_iter else 100-alpha_ptg, axis=0))).T
     elif alternative == 'greater':
         CI = np.vstack((np.percentile(boot_sample, alpha_ptg[0] if alpha_iter else alpha_ptg, axis=0), np.inf * np.ones((output_len)))).T
     else:
         raise ValueError(f"alternative '{alternative}' not valid. Available: 'two-sided', 'less', 'greater'.")
     return CI
 
-def CI_percentile(data, statistic, data2=None, R=int(1e5), alpha=0.05, smooth=False, alternative='two-sided', n_min=3, use_numba=True, **kwargs):
+def CI_percentile(data, statistic, data2=None, R=int(1e5), alpha=0.05, smooth=False, alternative='two-sided', n_min=1, use_numba=True, **kwargs):
     """
     If data2 is provided, statistic takes two arguments and assumes block resampling if the input data are tuples.
     Optional kwargs for aggregating data, data2 before computing the statistic:
             aggregator = @njit
                          def nb_mean(x):
                              return np.mean(x)
     """
```

### Comparing `phdu-2.4.4/phdu/stats/conf_interval.py` & `phdu-2.4.5/phdu/stats/conf_interval.py`

 * *Files identical despite different names*

### Comparing `phdu-2.4.4/phdu/stats/corr.py` & `phdu-2.4.5/phdu/stats/corr.py`

 * *Files identical despite different names*

### Comparing `phdu-2.4.4/phdu/stats/rtopy/_helper.py` & `phdu-2.4.5/phdu/stats/rtopy/_helper.py`

 * *Files identical despite different names*

### Comparing `phdu-2.4.4/phdu/stats/rtopy/resample.py` & `phdu-2.4.5/phdu/stats/rtopy/resample.py`

 * *Files identical despite different names*

### Comparing `phdu-2.4.4/phdu/stats/test/permutation.py` & `phdu-2.4.5/phdu/stats/test/permutation.py`

 * *Files identical despite different names*

### Comparing `phdu-2.4.4/phdu/storage.py` & `phdu-2.4.5/phdu/storage.py`

 * *Files identical despite different names*

### Comparing `phdu-2.4.4/phdu.egg-info/PKG-INFO` & `phdu-2.4.5/phdu.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phdu
-Version: 2.4.4
+Version: 2.4.5
 Summary: Automatically store/load data in a tidy, efficient way. Includes functions for data visualization and analysis.
 Home-page: https://github.com/medinajorge/PhD-utils
 Download-URL: https://github.com/medinajorge/PhD-utils/archive/refs/tags/v1.5-beta.tar.gz
 Author: Jorge Medina Hernández
 Author-email: medinahdezjorge@gmail.com
 Keywords: science,statistics,tidy,project organization,project,organization,path,storage
 Classifier: Programming Language :: Python :: 3
```

### Comparing `phdu-2.4.4/phdu.egg-info/SOURCES.txt` & `phdu-2.4.5/phdu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `phdu-2.4.4/setup.py` & `phdu-2.4.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='phdu',
-    version='2.4.4',
+    version='2.4.5',
     author="Jorge Medina Hernández",
     author_email='medinahdezjorge@gmail.com',
     packages=find_packages("."),
     url='https://github.com/medinajorge/PhD-utils',
     download_url='https://github.com/medinajorge/PhD-utils/archive/refs/tags/v1.5-beta.tar.gz',
     description="Automatically store/load data in a tidy, efficient way. Includes functions for data visualization and analysis.",
     long_description=open('README.md').read(),
```
