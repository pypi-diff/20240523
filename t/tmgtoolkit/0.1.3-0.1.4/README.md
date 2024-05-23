# Comparing `tmp/tmgtoolkit-0.1.3.tar.gz` & `tmp/tmgtoolkit-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tmgtoolkit-0.1.3.tar", last modified: Sat May 11 19:40:47 2024, max compression
+gzip compressed data, was "tmgtoolkit-0.1.4.tar", last modified: Thu May 23 21:42:08 2024, max compression
```

## Comparing `tmgtoolkit-0.1.3.tar` & `tmgtoolkit-0.1.4.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 ej        (1000) wheel      (998)        0 2024-05-11 19:40:47.958154 tmgtoolkit-0.1.3/
--rw-r--r--   0 ej        (1000) wheel      (998)    34916 2024-04-10 06:55:31.000000 tmgtoolkit-0.1.3/LICENSE.md
--rw-r--r--   0 ej        (1000) wheel      (998)     1259 2024-05-11 19:40:47.958154 tmgtoolkit-0.1.3/PKG-INFO
--rw-r--r--   0 ej        (1000) wheel      (998)      563 2024-04-10 07:01:19.000000 tmgtoolkit-0.1.3/README.md
--rw-r--r--   0 ej        (1000) wheel      (998)      103 2024-04-10 07:09:13.000000 tmgtoolkit-0.1.3/pyproject.toml
--rw-r--r--   0 ej        (1000) wheel      (998)      754 2024-05-11 19:40:47.958154 tmgtoolkit-0.1.3/setup.cfg
-drwxr-xr-x   0 ej        (1000) wheel      (998)        0 2024-05-11 19:40:47.951487 tmgtoolkit-0.1.3/src/
-drwxr-xr-x   0 ej        (1000) wheel      (998)        0 2024-05-11 19:40:47.954821 tmgtoolkit-0.1.3/src/tmgtoolkit/
--rw-r--r--   0 ej        (1000) wheel      (998)        0 2024-04-09 14:32:51.000000 tmgtoolkit-0.1.3/src/tmgtoolkit/__init__.py
--rw-r--r--   0 ej        (1000) wheel      (998)     5159 2024-05-11 14:14:37.000000 tmgtoolkit-0.1.3/src/tmgtoolkit/constants.py
--rw-r--r--   0 ej        (1000) wheel      (998)    16033 2024-05-10 15:04:33.000000 tmgtoolkit-0.1.3/src/tmgtoolkit/plotting.py
--rw-r--r--   0 ej        (1000) wheel      (998)    13745 2024-05-10 15:04:51.000000 tmgtoolkit-0.1.3/src/tmgtoolkit/spm.py
--rw-r--r--   0 ej        (1000) wheel      (998)    18630 2024-04-28 11:37:20.000000 tmgtoolkit-0.1.3/src/tmgtoolkit/time_series.py
--rw-r--r--   0 ej        (1000) wheel      (998)    11910 2024-05-11 14:13:54.000000 tmgtoolkit-0.1.3/src/tmgtoolkit/tmgio.py
-drwxr-xr-x   0 ej        (1000) wheel      (998)        0 2024-05-11 19:40:47.954821 tmgtoolkit-0.1.3/src/tmgtoolkit.egg-info/
--rw-r--r--   0 ej        (1000) wheel      (998)     1259 2024-05-11 19:40:47.000000 tmgtoolkit-0.1.3/src/tmgtoolkit.egg-info/PKG-INFO
--rw-r--r--   0 ej        (1000) wheel      (998)      410 2024-05-11 19:40:47.000000 tmgtoolkit-0.1.3/src/tmgtoolkit.egg-info/SOURCES.txt
--rw-r--r--   0 ej        (1000) wheel      (998)        1 2024-05-11 19:40:47.000000 tmgtoolkit-0.1.3/src/tmgtoolkit.egg-info/dependency_links.txt
--rw-r--r--   0 ej        (1000) wheel      (998)       50 2024-05-11 19:40:47.000000 tmgtoolkit-0.1.3/src/tmgtoolkit.egg-info/requires.txt
--rw-r--r--   0 ej        (1000) wheel      (998)       11 2024-05-11 19:40:47.000000 tmgtoolkit-0.1.3/src/tmgtoolkit.egg-info/top_level.txt
-drwxr-xr-x   0 ej        (1000) wheel      (998)        0 2024-05-11 19:40:47.954821 tmgtoolkit-0.1.3/tests/
--rw-r--r--   0 ej        (1000) wheel      (998)       85 2024-04-17 09:39:29.000000 tmgtoolkit-0.1.3/tests/test_mwe.py
+drwxr-xr-x   0 ej        (1000) wheel      (998)        0 2024-05-23 21:42:08.187594 tmgtoolkit-0.1.4/
+-rw-r--r--   0 ej        (1000) wheel      (998)    34916 2024-04-10 06:55:31.000000 tmgtoolkit-0.1.4/LICENSE.md
+-rw-r--r--   0 ej        (1000) wheel      (998)     1259 2024-05-23 21:42:08.187594 tmgtoolkit-0.1.4/PKG-INFO
+-rw-r--r--   0 ej        (1000) wheel      (998)      563 2024-04-10 07:01:19.000000 tmgtoolkit-0.1.4/README.md
+-rw-r--r--   0 ej        (1000) wheel      (998)      103 2024-04-10 07:09:13.000000 tmgtoolkit-0.1.4/pyproject.toml
+-rw-r--r--   0 ej        (1000) wheel      (998)      754 2024-05-23 21:42:08.187594 tmgtoolkit-0.1.4/setup.cfg
+drwxr-xr-x   0 ej        (1000) wheel      (998)        0 2024-05-23 21:42:08.180928 tmgtoolkit-0.1.4/src/
+drwxr-xr-x   0 ej        (1000) wheel      (998)        0 2024-05-23 21:42:08.184261 tmgtoolkit-0.1.4/src/tmgtoolkit/
+-rw-r--r--   0 ej        (1000) wheel      (998)        0 2024-04-09 14:32:51.000000 tmgtoolkit-0.1.4/src/tmgtoolkit/__init__.py
+-rw-r--r--   0 ej        (1000) wheel      (998)     6958 2024-05-20 20:55:42.000000 tmgtoolkit-0.1.4/src/tmgtoolkit/constants.py
+-rw-r--r--   0 ej        (1000) wheel      (998)    16033 2024-05-10 15:04:33.000000 tmgtoolkit-0.1.4/src/tmgtoolkit/plotting.py
+-rw-r--r--   0 ej        (1000) wheel      (998)    13745 2024-05-10 15:04:51.000000 tmgtoolkit-0.1.4/src/tmgtoolkit/spm.py
+-rw-r--r--   0 ej        (1000) wheel      (998)    18744 2024-05-14 21:23:52.000000 tmgtoolkit-0.1.4/src/tmgtoolkit/time_series.py
+-rw-r--r--   0 ej        (1000) wheel      (998)    15481 2024-05-21 17:51:44.000000 tmgtoolkit-0.1.4/src/tmgtoolkit/tmgio.py
+drwxr-xr-x   0 ej        (1000) wheel      (998)        0 2024-05-23 21:42:08.187594 tmgtoolkit-0.1.4/src/tmgtoolkit.egg-info/
+-rw-r--r--   0 ej        (1000) wheel      (998)     1259 2024-05-23 21:42:08.000000 tmgtoolkit-0.1.4/src/tmgtoolkit.egg-info/PKG-INFO
+-rw-r--r--   0 ej        (1000) wheel      (998)      443 2024-05-23 21:42:08.000000 tmgtoolkit-0.1.4/src/tmgtoolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 ej        (1000) wheel      (998)        1 2024-05-23 21:42:08.000000 tmgtoolkit-0.1.4/src/tmgtoolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 ej        (1000) wheel      (998)       50 2024-05-23 21:42:08.000000 tmgtoolkit-0.1.4/src/tmgtoolkit.egg-info/requires.txt
+-rw-r--r--   0 ej        (1000) wheel      (998)       11 2024-05-23 21:42:08.000000 tmgtoolkit-0.1.4/src/tmgtoolkit.egg-info/top_level.txt
+drwxr-xr-x   0 ej        (1000) wheel      (998)        0 2024-05-23 21:42:08.187594 tmgtoolkit-0.1.4/tests/
+-rw-r--r--   0 ej        (1000) wheel      (998)       85 2024-05-19 13:02:48.000000 tmgtoolkit-0.1.4/tests/test_mwe.py
+-rw-r--r--   0 ej        (1000) wheel      (998)     7349 2024-05-20 20:56:27.000000 tmgtoolkit-0.1.4/tests/test_split_data_for_spm.py
```

### Comparing `tmgtoolkit-0.1.3/LICENSE.md` & `tmgtoolkit-0.1.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `tmgtoolkit-0.1.3/PKG-INFO` & `tmgtoolkit-0.1.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tmgtoolkit
-Version: 0.1.3
+Version: 0.1.4
 Summary: Time series analysis of tensiomyography (TMG) data
 Home-page: https://github.com/ejmastnak/tmgtoolkit
 Author: Elijan Mastnak
 Author-email: admin@ejmastnak.com
 Project-URL: Bug Tracker, https://github.com/ejmastnak/tmgtoolkit/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `tmgtoolkit-0.1.3/README.md` & `tmgtoolkit-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `tmgtoolkit-0.1.3/setup.cfg` & `tmgtoolkit-0.1.4/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = tmgtoolkit
-version = 0.1.3
+version = 0.1.4
 author = Elijan Mastnak
 author_email = admin@ejmastnak.com
 description = Time series analysis of tensiomyography (TMG) data
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/ejmastnak/tmgtoolkit
 project_urls =
```

### Comparing `tmgtoolkit-0.1.3/src/tmgtoolkit/plotting.py` & `tmgtoolkit-0.1.4/src/tmgtoolkit/plotting.py`

 * *Files identical despite different names*

### Comparing `tmgtoolkit-0.1.3/src/tmgtoolkit/spm.py` & `tmgtoolkit-0.1.4/src/tmgtoolkit/spm.py`

 * *Files identical despite different names*

### Comparing `tmgtoolkit-0.1.3/src/tmgtoolkit/time_series.py` & `tmgtoolkit-0.1.4/src/tmgtoolkit/time_series.py`

 * *Files 1% similar despite different names*

```diff
@@ -366,14 +366,16 @@
     Returns
     ----------
     time : float
         Approximate independent variable value, in units of `t`, corresponding
         to `idx`; loosely, an estimate of the value t(idx) if `t` were
         continuous.
     """
+    assert 0 <= idx < t.shape[0], "Index {} is out of bounds for time array with shape {}.".format(idx, t.shape)
+
     if idx.is_integer():
         return float(t[int(idx)])
 
     idx_floor = math.floor(idx)
     idx_ceil = math.ceil(idx)
     ratio = (idx - idx_floor)/(idx_ceil - idx_floor)
```

### Comparing `tmgtoolkit-0.1.3/src/tmgtoolkit.egg-info/PKG-INFO` & `tmgtoolkit-0.1.4/src/tmgtoolkit.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tmgtoolkit
-Version: 0.1.3
+Version: 0.1.4
 Summary: Time series analysis of tensiomyography (TMG) data
 Home-page: https://github.com/ejmastnak/tmgtoolkit
 Author: Elijan Mastnak
 Author-email: admin@ejmastnak.com
 Project-URL: Bug Tracker, https://github.com/ejmastnak/tmgtoolkit/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

