# Comparing `tmp/mockseries-0.3.0.tar.gz` & `tmp/mockseries-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mockseries-0.3.0.tar", last modified: Sat Jan 27 17:42:20 2024, max compression
+gzip compressed data, was "mockseries-0.3.1.tar", last modified: Thu May 23 14:36:58 2024, max compression
```

## Comparing `mockseries-0.3.0.tar` & `mockseries-0.3.1.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 17:42:20.896885 mockseries-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-01-27 17:42:08.000000 mockseries-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3410 2024-01-27 17:42:20.896885 mockseries-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-01-27 17:42:08.000000 mockseries-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 17:42:20.888885 mockseries-0.3.0/mockseries/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-01-27 17:42:08.000000 mockseries-0.3.0/mockseries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-01-27 17:42:08.000000 mockseries-0.3.0/mockseries/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 17:42:20.888885 mockseries-0.3.0/mockseries/interaction/
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-01-27 17:42:08.000000 mockseries-0.3.0/mockseries/interaction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-01-27 17:42:08.000000 mockseries-0.3.0/mockseries/interaction/additive_interaction.py
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-01-27 17:42:08.000000 mockseries-0.3.0/mockseries/interaction/interaction.py
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-01-27 17:42:08.000000 mockseries-0.3.0/mockseries/interaction/multiplicative_interaction.py
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-01-27 17:42:08.000000 mockseries-0.3.0/mockseries/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 17:42:20.892885 mockseries-0.3.0/mockseries/noise/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-01-27 17:42:08.000000 mockseries-0.3.0/mockseries/noise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-01-27 17:42:08.000000 mockseries-0.3.0/mockseries/noise/gaussian_noise.py
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-01-27 17:42:08.000000 mockseries-0.3.0/mockseries/noise/noise.py
--rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-01-27 17:42:08.000000 mockseries-0.3.0/mockseries/noise/red_noise.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 17:42:20.892885 mockseries-0.3.0/mockseries/seasonality/
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-01-27 17:42:08.000000 mockseries-0.3.0/mockseries/seasonality/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-01-27 17:42:08.000000 mockseries-0.3.0/mockseries/seasonality/daily_seasonality.py
--rw-r--r--   0 runner    (1001) docker     (127)     6567 2024-01-27 17:42:08.000000 mockseries-0.3.0/mockseries/seasonality/period_seasonality.py
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-01-27 17:42:08.000000 mockseries-0.3.0/mockseries/seasonality/seasonality.py
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-01-27 17:42:08.000000 mockseries-0.3.0/mockseries/seasonality/sinusoidal_seasonality.py
--rw-r--r--   0 runner    (1001) docker     (127)     2437 2024-01-27 17:42:08.000000 mockseries-0.3.0/mockseries/seasonality/weekly_seasonality.py
--rw-r--r--   0 runner    (1001) docker     (127)     2991 2024-01-27 17:42:08.000000 mockseries-0.3.0/mockseries/seasonality/yearly_seasonality.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 17:42:20.892885 mockseries-0.3.0/mockseries/signal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 17:42:08.000000 mockseries-0.3.0/mockseries/signal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-01-27 17:42:08.000000 mockseries-0.3.0/mockseries/signal/composed_signal.py
--rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-01-27 17:42:08.000000 mockseries-0.3.0/mockseries/signal/signal.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 17:42:20.892885 mockseries-0.3.0/mockseries/transition/
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-01-27 17:42:08.000000 mockseries-0.3.0/mockseries/transition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-01-27 17:42:08.000000 mockseries-0.3.0/mockseries/transition/direct_transition.py
--rw-r--r--   0 runner    (1001) docker     (127)     4536 2024-01-27 17:42:08.000000 mockseries-0.3.0/mockseries/transition/lambda_transition.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-01-27 17:42:08.000000 mockseries-0.3.0/mockseries/transition/linear_transition.py
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-01-27 17:42:08.000000 mockseries-0.3.0/mockseries/transition/transition.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 17:42:20.892885 mockseries-0.3.0/mockseries/trend/
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-01-27 17:42:08.000000 mockseries-0.3.0/mockseries/trend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-01-27 17:42:08.000000 mockseries-0.3.0/mockseries/trend/exponential_trend.py
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-01-27 17:42:08.000000 mockseries-0.3.0/mockseries/trend/flat_trend.py
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-01-27 17:42:08.000000 mockseries-0.3.0/mockseries/trend/linear_trend.py
--rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-01-27 17:42:08.000000 mockseries-0.3.0/mockseries/trend/switch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 17:42:20.896885 mockseries-0.3.0/mockseries/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-01-27 17:42:08.000000 mockseries-0.3.0/mockseries/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-01-27 17:42:08.000000 mockseries-0.3.0/mockseries/utils/dates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-01-27 17:42:08.000000 mockseries-0.3.0/mockseries/utils/plot.py
--rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-01-27 17:42:08.000000 mockseries-0.3.0/mockseries/utils/timedeltas.py
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-01-27 17:42:08.000000 mockseries-0.3.0/mockseries/utils/writers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 17:42:20.888885 mockseries-0.3.0/mockseries.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3410 2024-01-27 17:42:20.000000 mockseries-0.3.0/mockseries.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-01-27 17:42:20.000000 mockseries-0.3.0/mockseries.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-27 17:42:20.000000 mockseries-0.3.0/mockseries.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-27 17:42:20.000000 mockseries-0.3.0/mockseries.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-01-27 17:42:20.000000 mockseries-0.3.0/mockseries.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-01-27 17:42:20.000000 mockseries-0.3.0/mockseries.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-27 17:42:20.896885 mockseries-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-01-27 17:42:08.000000 mockseries-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:36:58.790570 mockseries-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-23 14:36:41.000000 mockseries-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-05-23 14:36:58.790570 mockseries-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-05-23 14:36:41.000000 mockseries-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:36:58.782570 mockseries-0.3.1/mockseries/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-23 14:36:41.000000 mockseries-0.3.1/mockseries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-23 14:36:41.000000 mockseries-0.3.1/mockseries/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:36:58.782570 mockseries-0.3.1/mockseries/interaction/
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-23 14:36:41.000000 mockseries-0.3.1/mockseries/interaction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-23 14:36:41.000000 mockseries-0.3.1/mockseries/interaction/additive_interaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-23 14:36:41.000000 mockseries-0.3.1/mockseries/interaction/interaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-23 14:36:41.000000 mockseries-0.3.1/mockseries/interaction/multiplicative_interaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-23 14:36:41.000000 mockseries-0.3.1/mockseries/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:36:58.782570 mockseries-0.3.1/mockseries/noise/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-23 14:36:41.000000 mockseries-0.3.1/mockseries/noise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-23 14:36:41.000000 mockseries-0.3.1/mockseries/noise/gaussian_noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-23 14:36:41.000000 mockseries-0.3.1/mockseries/noise/noise.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-05-23 14:36:41.000000 mockseries-0.3.1/mockseries/noise/red_noise.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:36:58.782570 mockseries-0.3.1/mockseries/seasonality/
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-23 14:36:41.000000 mockseries-0.3.1/mockseries/seasonality/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-05-23 14:36:41.000000 mockseries-0.3.1/mockseries/seasonality/daily_seasonality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6567 2024-05-23 14:36:41.000000 mockseries-0.3.1/mockseries/seasonality/period_seasonality.py
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-23 14:36:41.000000 mockseries-0.3.1/mockseries/seasonality/seasonality.py
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-23 14:36:41.000000 mockseries-0.3.1/mockseries/seasonality/sinusoidal_seasonality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2437 2024-05-23 14:36:41.000000 mockseries-0.3.1/mockseries/seasonality/weekly_seasonality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2991 2024-05-23 14:36:41.000000 mockseries-0.3.1/mockseries/seasonality/yearly_seasonality.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:36:58.782570 mockseries-0.3.1/mockseries/signal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 14:36:41.000000 mockseries-0.3.1/mockseries/signal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-23 14:36:41.000000 mockseries-0.3.1/mockseries/signal/composed_signal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6415 2024-05-23 14:36:41.000000 mockseries-0.3.1/mockseries/signal/signal.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:36:58.786570 mockseries-0.3.1/mockseries/transition/
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-23 14:36:41.000000 mockseries-0.3.1/mockseries/transition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-23 14:36:41.000000 mockseries-0.3.1/mockseries/transition/direct_transition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4536 2024-05-23 14:36:41.000000 mockseries-0.3.1/mockseries/transition/lambda_transition.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-23 14:36:41.000000 mockseries-0.3.1/mockseries/transition/linear_transition.py
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-23 14:36:41.000000 mockseries-0.3.1/mockseries/transition/transition.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:36:58.790570 mockseries-0.3.1/mockseries/trend/
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-23 14:36:41.000000 mockseries-0.3.1/mockseries/trend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-23 14:36:41.000000 mockseries-0.3.1/mockseries/trend/exponential_trend.py
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-05-23 14:36:41.000000 mockseries-0.3.1/mockseries/trend/flat_trend.py
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-05-23 14:36:41.000000 mockseries-0.3.1/mockseries/trend/linear_trend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-05-23 14:36:41.000000 mockseries-0.3.1/mockseries/trend/switch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:36:58.790570 mockseries-0.3.1/mockseries/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-23 14:36:41.000000 mockseries-0.3.1/mockseries/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-05-23 14:36:41.000000 mockseries-0.3.1/mockseries/utils/dates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-05-23 14:36:41.000000 mockseries-0.3.1/mockseries/utils/plot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2103 2024-05-23 14:36:41.000000 mockseries-0.3.1/mockseries/utils/timedeltas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-23 14:36:41.000000 mockseries-0.3.1/mockseries/utils/writers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:36:58.782570 mockseries-0.3.1/mockseries.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-05-23 14:36:58.000000 mockseries-0.3.1/mockseries.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-05-23 14:36:58.000000 mockseries-0.3.1/mockseries.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 14:36:58.000000 mockseries-0.3.1/mockseries.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-23 14:36:58.000000 mockseries-0.3.1/mockseries.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-23 14:36:58.000000 mockseries-0.3.1/mockseries.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-23 14:36:58.000000 mockseries-0.3.1/mockseries.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 14:36:58.790570 mockseries-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-05-23 14:36:41.000000 mockseries-0.3.1/setup.py
```

### Comparing `mockseries-0.3.0/LICENSE` & `mockseries-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mockseries-0.3.0/PKG-INFO` & `mockseries-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mockseries
-Version: 0.3.0
+Version: 0.3.1
 Summary: Easy and intuitive generation of synthetic timeseries.
 Home-page: http://mockseries.catheu.tech/
 Author: Cyril de Catheu
 Author-email: cdecatheu@hey.com
 License: BSD
 Project-URL: Bug Tracker, https://github.com/cyrilou242/mockseries/issues
 Project-URL: Documentation, http://mockseries.catheu.tech/
@@ -24,15 +24,15 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Typing :: Typed
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
-Requires-Python: >=3.9,<=3.12
+Requires-Python: >=3.9,<3.13
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center">
   <img src="https://github.com/cyrilou242/mockseries/blob/main/website/static/img/mockingbird200.png">
 </p>
```

### Comparing `mockseries-0.3.0/README.md` & `mockseries-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `mockseries-0.3.0/mockseries/noise/gaussian_noise.py` & `mockseries-0.3.1/mockseries/noise/gaussian_noise.py`

 * *Files identical despite different names*

### Comparing `mockseries-0.3.0/mockseries/noise/red_noise.py` & `mockseries-0.3.1/mockseries/noise/red_noise.py`

 * *Files identical despite different names*

### Comparing `mockseries-0.3.0/mockseries/seasonality/daily_seasonality.py` & `mockseries-0.3.1/mockseries/seasonality/daily_seasonality.py`

 * *Files identical despite different names*

### Comparing `mockseries-0.3.0/mockseries/seasonality/period_seasonality.py` & `mockseries-0.3.1/mockseries/seasonality/period_seasonality.py`

 * *Files identical despite different names*

### Comparing `mockseries-0.3.0/mockseries/seasonality/sinusoidal_seasonality.py` & `mockseries-0.3.1/mockseries/seasonality/sinusoidal_seasonality.py`

 * *Files identical despite different names*

### Comparing `mockseries-0.3.0/mockseries/seasonality/weekly_seasonality.py` & `mockseries-0.3.1/mockseries/seasonality/weekly_seasonality.py`

 * *Files identical despite different names*

### Comparing `mockseries-0.3.0/mockseries/seasonality/yearly_seasonality.py` & `mockseries-0.3.1/mockseries/seasonality/yearly_seasonality.py`

 * *Files identical despite different names*

### Comparing `mockseries-0.3.0/mockseries/signal/composed_signal.py` & `mockseries-0.3.1/mockseries/signal/composed_signal.py`

 * *Files identical despite different names*

### Comparing `mockseries-0.3.0/mockseries/signal/signal.py` & `mockseries-0.3.1/mockseries/signal/signal.py`

 * *Files identical despite different names*

### Comparing `mockseries-0.3.0/mockseries/transition/lambda_transition.py` & `mockseries-0.3.1/mockseries/transition/lambda_transition.py`

 * *Files identical despite different names*

### Comparing `mockseries-0.3.0/mockseries/transition/linear_transition.py` & `mockseries-0.3.1/mockseries/transition/linear_transition.py`

 * *Files identical despite different names*

### Comparing `mockseries-0.3.0/mockseries/trend/exponential_trend.py` & `mockseries-0.3.1/mockseries/trend/exponential_trend.py`

 * *Files identical despite different names*

### Comparing `mockseries-0.3.0/mockseries/trend/linear_trend.py` & `mockseries-0.3.1/mockseries/trend/linear_trend.py`

 * *Files identical despite different names*

### Comparing `mockseries-0.3.0/mockseries/trend/switch.py` & `mockseries-0.3.1/mockseries/trend/switch.py`

 * *Files identical despite different names*

### Comparing `mockseries-0.3.0/mockseries/utils/dates.py` & `mockseries-0.3.1/mockseries/utils/dates.py`

 * *Files identical despite different names*

### Comparing `mockseries-0.3.0/mockseries/utils/plot.py` & `mockseries-0.3.1/mockseries/utils/plot.py`

 * *Files identical despite different names*

### Comparing `mockseries-0.3.0/mockseries/utils/timedeltas.py` & `mockseries-0.3.1/mockseries/utils/timedeltas.py`

 * *Files identical despite different names*

### Comparing `mockseries-0.3.0/mockseries/utils/writers.py` & `mockseries-0.3.1/mockseries/utils/writers.py`

 * *Files identical despite different names*

### Comparing `mockseries-0.3.0/mockseries.egg-info/PKG-INFO` & `mockseries-0.3.1/mockseries.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mockseries
-Version: 0.3.0
+Version: 0.3.1
 Summary: Easy and intuitive generation of synthetic timeseries.
 Home-page: http://mockseries.catheu.tech/
 Author: Cyril de Catheu
 Author-email: cdecatheu@hey.com
 License: BSD
 Project-URL: Bug Tracker, https://github.com/cyrilou242/mockseries/issues
 Project-URL: Documentation, http://mockseries.catheu.tech/
@@ -24,15 +24,15 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Typing :: Typed
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
-Requires-Python: >=3.9,<=3.12
+Requires-Python: >=3.9,<3.13
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <p align="center">
   <img src="https://github.com/cyrilou242/mockseries/blob/main/website/static/img/mockingbird200.png">
 </p>
```

### Comparing `mockseries-0.3.0/mockseries.egg-info/SOURCES.txt` & `mockseries-0.3.1/mockseries.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mockseries-0.3.0/setup.py` & `mockseries-0.3.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="mockseries",
-    version="0.3.0",
+    version="0.3.1",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     url="http://mockseries.catheu.tech/",
     license="BSD",
     author="Cyril de Catheu",
     author_email="cdecatheu@hey.com",
@@ -40,14 +40,14 @@
         "Typing :: Typed",
         "Operating System :: OS Independent",
         "Operating System :: Microsoft :: Windows",
         "Operating System :: POSIX",
         "Operating System :: Unix",
         "Operating System :: MacOS",
     ],
-    python_requires=">=3.9,<=3.12",
+    python_requires=">=3.9,<3.13",
     entry_points={
         "console_scripts": [
             "mockseries = mockseries.main:main",
         ],
     },
 )
```

