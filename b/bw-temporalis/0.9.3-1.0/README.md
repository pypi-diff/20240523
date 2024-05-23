# Comparing `tmp/bw_temporalis-0.9.3.tar.gz` & `tmp/bw_temporalis-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bw_temporalis-0.9.3.tar", last modified: Fri Mar  8 21:58:10 2024, max compression
+gzip compressed data, was "bw_temporalis-1.0.tar", last modified: Thu May 23 19:01:18 2024, max compression
```

## Comparing `bw_temporalis-0.9.3.tar` & `bw_temporalis-1.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2024-03-08 21:58:10.548790 bw_temporalis-0.9.3/
--rw-r--r--   0 cmutel     (501) staff       (20)     1456 2024-03-08 21:56:26.000000 bw_temporalis-0.9.3/LICENSE
--rw-r--r--   0 cmutel     (501) staff       (20)       30 2024-03-08 21:56:26.000000 bw_temporalis-0.9.3/MANIFEST.in
--rw-r--r--   0 cmutel     (501) staff       (20)     4652 2024-03-08 21:58:10.548688 bw_temporalis-0.9.3/PKG-INFO
--rw-r--r--   0 cmutel     (501) staff       (20)     3063 2024-03-08 21:56:26.000000 bw_temporalis-0.9.3/README.md
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2024-03-08 21:58:10.543563 bw_temporalis-0.9.3/bw_temporalis/
--rw-r--r--   0 cmutel     (501) staff       (20)        6 2024-03-08 21:57:39.000000 bw_temporalis-0.9.3/bw_temporalis/VERSION
--rw-r--r--   0 cmutel     (501) staff       (20)      902 2024-03-08 21:56:26.000000 bw_temporalis-0.9.3/bw_temporalis/__init__.py
--rw-r--r--   0 cmutel     (501) staff       (20)     3287 2024-03-08 21:56:26.000000 bw_temporalis-0.9.3/bw_temporalis/convolution.py
--rw-r--r--   0 cmutel     (501) staff       (20)    12579 2024-03-08 21:56:26.000000 bw_temporalis-0.9.3/bw_temporalis/lca.py
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2024-03-08 21:58:10.542013 bw_temporalis-0.9.3/bw_temporalis/lcia/
--rw-r--r--   0 cmutel     (501) staff       (20)       60 2024-03-08 21:56:26.000000 bw_temporalis-0.9.3/bw_temporalis/lcia/__init__.py
--rw-r--r--   0 cmutel     (501) staff       (20)     4752 2024-03-08 21:56:26.000000 bw_temporalis-0.9.3/bw_temporalis/lcia/climate.py
--rw-r--r--   0 cmutel     (501) staff       (20)    16866 2024-03-08 21:56:26.000000 bw_temporalis-0.9.3/bw_temporalis/temporal_distribution.py
--rw-r--r--   0 cmutel     (501) staff       (20)    10634 2024-03-08 21:56:26.000000 bw_temporalis-0.9.3/bw_temporalis/timeline.py
--rw-r--r--   0 cmutel     (501) staff       (20)     9398 2024-03-08 21:56:26.000000 bw_temporalis-0.9.3/bw_temporalis/utils.py
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2024-03-08 21:58:10.547775 bw_temporalis-0.9.3/bw_temporalis.egg-info/
--rw-r--r--   0 cmutel     (501) staff       (20)     4652 2024-03-08 21:58:10.000000 bw_temporalis-0.9.3/bw_temporalis.egg-info/PKG-INFO
--rw-r--r--   0 cmutel     (501) staff       (20)      876 2024-03-08 21:58:10.000000 bw_temporalis-0.9.3/bw_temporalis.egg-info/SOURCES.txt
--rw-r--r--   0 cmutel     (501) staff       (20)        1 2024-03-08 21:58:10.000000 bw_temporalis-0.9.3/bw_temporalis.egg-info/dependency_links.txt
--rw-r--r--   0 cmutel     (501) staff       (20)        1 2024-03-08 21:58:10.000000 bw_temporalis-0.9.3/bw_temporalis.egg-info/not-zip-safe
--rw-r--r--   0 cmutel     (501) staff       (20)      174 2024-03-08 21:58:10.000000 bw_temporalis-0.9.3/bw_temporalis.egg-info/requires.txt
--rw-r--r--   0 cmutel     (501) staff       (20)       37 2024-03-08 21:58:10.000000 bw_temporalis-0.9.3/bw_temporalis.egg-info/top_level.txt
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2024-03-08 21:58:10.542324 bw_temporalis-0.9.3/docs/
--rw-r--r--   0 cmutel     (501) staff       (20)     1151 2024-03-08 21:56:26.000000 bw_temporalis-0.9.3/docs/conf.py
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2024-03-08 21:58:10.543314 bw_temporalis-0.9.3/examples/
--rw-r--r--   0 cmutel     (501) staff       (20)     1500 2024-03-08 21:56:26.000000 bw_temporalis-0.9.3/examples/__init__.py
--rw-r--r--   0 cmutel     (501) staff       (20)     4350 2024-03-08 21:56:26.000000 bw_temporalis-0.9.3/examples/ia.py
--rw-r--r--   0 cmutel     (501) staff       (20)     6149 2024-03-08 21:56:26.000000 bw_temporalis-0.9.3/examples/inv.py
--rw-r--r--   0 cmutel     (501) staff       (20)       87 2024-03-08 21:56:26.000000 bw_temporalis-0.9.3/pyproject.toml
--rw-r--r--   0 cmutel     (501) staff       (20)     1754 2024-03-08 21:58:10.549237 bw_temporalis-0.9.3/setup.cfg
-drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2024-03-08 21:58:10.547420 bw_temporalis-0.9.3/tests/
--rw-r--r--   0 cmutel     (501) staff       (20)     8786 2024-03-08 21:56:26.000000 bw_temporalis-0.9.3/tests/test_convolution.py
--rw-r--r--   0 cmutel     (501) staff       (20)     3247 2024-03-08 21:56:26.000000 bw_temporalis-0.9.3/tests/test_fixed_td.py
--rw-r--r--   0 cmutel     (501) staff       (20)     6094 2024-03-08 21:56:26.000000 bw_temporalis-0.9.3/tests/test_fixed_time_of_year.py
--rw-r--r--   0 cmutel     (501) staff       (20)     8567 2024-03-08 21:56:26.000000 bw_temporalis-0.9.3/tests/test_fixtures.py
--rw-r--r--   0 cmutel     (501) staff       (20)    13408 2024-03-08 21:56:26.000000 bw_temporalis-0.9.3/tests/test_lca.py
--rw-r--r--   0 cmutel     (501) staff       (20)     4104 2024-03-08 21:56:26.000000 bw_temporalis-0.9.3/tests/test_patched_matrix_lca.py
--rw-r--r--   0 cmutel     (501) staff       (20)     4074 2024-03-08 21:56:26.000000 bw_temporalis-0.9.3/tests/test_serialization.py
--rw-r--r--   0 cmutel     (501) staff       (20)     5991 2024-03-08 21:56:26.000000 bw_temporalis-0.9.3/tests/test_td.py
--rw-r--r--   0 cmutel     (501) staff       (20)     2948 2024-03-08 21:56:26.000000 bw_temporalis-0.9.3/tests/test_tdaware.py
--rw-r--r--   0 cmutel     (501) staff       (20)     8635 2024-03-08 21:56:26.000000 bw_temporalis-0.9.3/tests/test_timeline.py
--rw-r--r--   0 cmutel     (501) staff       (20)    13941 2024-03-08 21:56:26.000000 bw_temporalis-0.9.3/tests/test_utils.py
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2024-05-23 19:01:18.746003 bw_temporalis-1.0/
+-rw-r--r--   0 cmutel     (501) staff       (20)     1456 2024-05-23 18:50:52.000000 bw_temporalis-1.0/LICENSE
+-rw-r--r--   0 cmutel     (501) staff       (20)       30 2024-05-23 18:50:52.000000 bw_temporalis-1.0/MANIFEST.in
+-rw-r--r--   0 cmutel     (501) staff       (20)     4650 2024-05-23 19:01:18.745933 bw_temporalis-1.0/PKG-INFO
+-rw-r--r--   0 cmutel     (501) staff       (20)     3063 2024-05-23 18:50:52.000000 bw_temporalis-1.0/README.md
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2024-05-23 19:01:18.740279 bw_temporalis-1.0/bw_temporalis/
+-rw-r--r--   0 cmutel     (501) staff       (20)        4 2024-05-23 18:59:19.000000 bw_temporalis-1.0/bw_temporalis/VERSION
+-rw-r--r--   0 cmutel     (501) staff       (20)      902 2024-05-23 18:50:52.000000 bw_temporalis-1.0/bw_temporalis/__init__.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     3287 2024-05-23 18:50:52.000000 bw_temporalis-1.0/bw_temporalis/convolution.py
+-rw-r--r--   0 cmutel     (501) staff       (20)    12579 2024-05-23 18:50:52.000000 bw_temporalis-1.0/bw_temporalis/lca.py
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2024-05-23 19:01:18.739104 bw_temporalis-1.0/bw_temporalis/lcia/
+-rw-r--r--   0 cmutel     (501) staff       (20)       60 2024-05-23 18:50:52.000000 bw_temporalis-1.0/bw_temporalis/lcia/__init__.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     4752 2024-05-23 18:50:52.000000 bw_temporalis-1.0/bw_temporalis/lcia/climate.py
+-rw-r--r--   0 cmutel     (501) staff       (20)    16890 2024-05-23 18:51:42.000000 bw_temporalis-1.0/bw_temporalis/temporal_distribution.py
+-rw-r--r--   0 cmutel     (501) staff       (20)    10634 2024-05-23 18:50:52.000000 bw_temporalis-1.0/bw_temporalis/timeline.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     9398 2024-05-23 18:50:52.000000 bw_temporalis-1.0/bw_temporalis/utils.py
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2024-05-23 19:01:18.743225 bw_temporalis-1.0/bw_temporalis.egg-info/
+-rw-r--r--   0 cmutel     (501) staff       (20)     4650 2024-05-23 19:01:18.000000 bw_temporalis-1.0/bw_temporalis.egg-info/PKG-INFO
+-rw-r--r--   0 cmutel     (501) staff       (20)      876 2024-05-23 19:01:18.000000 bw_temporalis-1.0/bw_temporalis.egg-info/SOURCES.txt
+-rw-r--r--   0 cmutel     (501) staff       (20)        1 2024-05-23 19:01:18.000000 bw_temporalis-1.0/bw_temporalis.egg-info/dependency_links.txt
+-rw-r--r--   0 cmutel     (501) staff       (20)        1 2024-05-23 18:51:54.000000 bw_temporalis-1.0/bw_temporalis.egg-info/not-zip-safe
+-rw-r--r--   0 cmutel     (501) staff       (20)      174 2024-05-23 19:01:18.000000 bw_temporalis-1.0/bw_temporalis.egg-info/requires.txt
+-rw-r--r--   0 cmutel     (501) staff       (20)       37 2024-05-23 19:01:18.000000 bw_temporalis-1.0/bw_temporalis.egg-info/top_level.txt
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2024-05-23 19:01:18.739353 bw_temporalis-1.0/docs/
+-rw-r--r--   0 cmutel     (501) staff       (20)     2872 2024-05-23 18:50:52.000000 bw_temporalis-1.0/docs/conf.py
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2024-05-23 19:01:18.739915 bw_temporalis-1.0/examples/
+-rw-r--r--   0 cmutel     (501) staff       (20)     1500 2024-05-23 18:50:52.000000 bw_temporalis-1.0/examples/__init__.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     4350 2024-05-23 18:50:52.000000 bw_temporalis-1.0/examples/ia.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     6149 2024-05-23 18:50:52.000000 bw_temporalis-1.0/examples/inv.py
+-rw-r--r--   0 cmutel     (501) staff       (20)       87 2024-05-23 18:50:52.000000 bw_temporalis-1.0/pyproject.toml
+-rw-r--r--   0 cmutel     (501) staff       (20)     1754 2024-05-23 19:01:18.746322 bw_temporalis-1.0/setup.cfg
+drwxr-xr-x   0 cmutel     (501) staff       (20)        0 2024-05-23 19:01:18.742972 bw_temporalis-1.0/tests/
+-rw-r--r--   0 cmutel     (501) staff       (20)     8786 2024-05-23 18:50:52.000000 bw_temporalis-1.0/tests/test_convolution.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     3247 2024-05-23 18:50:52.000000 bw_temporalis-1.0/tests/test_fixed_td.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     6094 2024-05-23 18:50:52.000000 bw_temporalis-1.0/tests/test_fixed_time_of_year.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     8567 2024-05-23 18:50:52.000000 bw_temporalis-1.0/tests/test_fixtures.py
+-rw-r--r--   0 cmutel     (501) staff       (20)    13408 2024-05-23 18:50:52.000000 bw_temporalis-1.0/tests/test_lca.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     4104 2024-05-23 18:50:52.000000 bw_temporalis-1.0/tests/test_patched_matrix_lca.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     4074 2024-05-23 18:50:52.000000 bw_temporalis-1.0/tests/test_serialization.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     5976 2024-05-23 18:55:54.000000 bw_temporalis-1.0/tests/test_td.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     2948 2024-05-23 18:50:52.000000 bw_temporalis-1.0/tests/test_tdaware.py
+-rw-r--r--   0 cmutel     (501) staff       (20)     8635 2024-05-23 18:50:52.000000 bw_temporalis-1.0/tests/test_timeline.py
+-rw-r--r--   0 cmutel     (501) staff       (20)    13941 2024-05-23 18:50:52.000000 bw_temporalis-1.0/tests/test_utils.py
```

### Comparing `bw_temporalis-0.9.3/LICENSE` & `bw_temporalis-1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bw_temporalis-0.9.3/PKG-INFO` & `bw_temporalis-1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bw_temporalis
-Version: 0.9.3
+Version: 1.0
 Summary: Revision of bw2temporalis for modern Brightway
 Home-page: https://github.com/brightway-lca/bw_temporalis
 Author: Chris Mutel
 Author-email: <cmutel@gmail.com>
 Maintainer: Chris Mutel
 Maintainer-email: <cmutel@gmail.com>
 License: BSD-3-Clause
```

### Comparing `bw_temporalis-0.9.3/README.md` & `bw_temporalis-1.0/README.md`

 * *Files identical despite different names*

### Comparing `bw_temporalis-0.9.3/bw_temporalis/__init__.py` & `bw_temporalis-1.0/bw_temporalis/__init__.py`

 * *Files identical despite different names*

### Comparing `bw_temporalis-0.9.3/bw_temporalis/convolution.py` & `bw_temporalis-1.0/bw_temporalis/convolution.py`

 * *Files identical despite different names*

### Comparing `bw_temporalis-0.9.3/bw_temporalis/lca.py` & `bw_temporalis-1.0/bw_temporalis/lca.py`

 * *Files identical despite different names*

### Comparing `bw_temporalis-0.9.3/bw_temporalis/lcia/climate.py` & `bw_temporalis-1.0/bw_temporalis/lcia/climate.py`

 * *Files identical despite different names*

### Comparing `bw_temporalis-0.9.3/bw_temporalis/temporal_distribution.py` & `bw_temporalis-1.0/bw_temporalis/temporal_distribution.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,15 +138,16 @@
         elif isinstance(other, TemporalDistributionBase) and other._mul_comes_first:
             return other * self
         elif isinstance(other, TemporalDistribution):
             if (
                 self.base_time_type == datetime_type
                 and other.base_time_type == datetime_type
             ):
-                raise ValueError("Can't multiply two datetime arrays")
+                # The user insists that they know, we follow them
+                return other
             elif self.base_time_type == datetime_type:
                 date, amount = temporal_convolution_datetime_timedelta(
                     first_date=self.date,
                     first_amount=self.amount,
                     second_date=other.date,
                     second_amount=other.amount,
                 )
```

### Comparing `bw_temporalis-0.9.3/bw_temporalis/timeline.py` & `bw_temporalis-1.0/bw_temporalis/timeline.py`

 * *Files identical despite different names*

### Comparing `bw_temporalis-0.9.3/bw_temporalis/utils.py` & `bw_temporalis-1.0/bw_temporalis/utils.py`

 * *Files identical despite different names*

### Comparing `bw_temporalis-0.9.3/bw_temporalis.egg-info/PKG-INFO` & `bw_temporalis-1.0/bw_temporalis.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bw_temporalis
-Version: 0.9.3
+Version: 1.0
 Summary: Revision of bw2temporalis for modern Brightway
 Home-page: https://github.com/brightway-lca/bw_temporalis
 Author: Chris Mutel
 Author-email: <cmutel@gmail.com>
 Maintainer: Chris Mutel
 Maintainer-email: <cmutel@gmail.com>
 License: BSD-3-Clause
```

### Comparing `bw_temporalis-0.9.3/bw_temporalis.egg-info/SOURCES.txt` & `bw_temporalis-1.0/bw_temporalis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bw_temporalis-0.9.3/examples/__init__.py` & `bw_temporalis-1.0/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `bw_temporalis-0.9.3/examples/ia.py` & `bw_temporalis-1.0/examples/ia.py`

 * *Files identical despite different names*

### Comparing `bw_temporalis-0.9.3/examples/inv.py` & `bw_temporalis-1.0/examples/inv.py`

 * *Files identical despite different names*

### Comparing `bw_temporalis-0.9.3/setup.cfg` & `bw_temporalis-1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `bw_temporalis-0.9.3/tests/test_convolution.py` & `bw_temporalis-1.0/tests/test_convolution.py`

 * *Files identical despite different names*

### Comparing `bw_temporalis-0.9.3/tests/test_fixed_td.py` & `bw_temporalis-1.0/tests/test_fixed_td.py`

 * *Files identical despite different names*

### Comparing `bw_temporalis-0.9.3/tests/test_fixed_time_of_year.py` & `bw_temporalis-1.0/tests/test_fixed_time_of_year.py`

 * *Files identical despite different names*

### Comparing `bw_temporalis-0.9.3/tests/test_fixtures.py` & `bw_temporalis-1.0/tests/test_fixtures.py`

 * *Files identical despite different names*

### Comparing `bw_temporalis-0.9.3/tests/test_lca.py` & `bw_temporalis-1.0/tests/test_lca.py`

 * *Files identical despite different names*

### Comparing `bw_temporalis-0.9.3/tests/test_patched_matrix_lca.py` & `bw_temporalis-1.0/tests/test_patched_matrix_lca.py`

 * *Files identical despite different names*

### Comparing `bw_temporalis-0.9.3/tests/test_serialization.py` & `bw_temporalis-1.0/tests/test_serialization.py`

 * *Files identical despite different names*

### Comparing `bw_temporalis-0.9.3/tests/test_td.py` & `bw_temporalis-1.0/tests/test_td.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,21 +15,19 @@
         TD(None, None)
     with pytest.raises(ValueError):
         TD(np.arange(5), np.array([2, 2, 2, 2]))
     with pytest.raises(ValueError):
         TD(np.arange(5), np.ones(5) * 2)
 
 
-def test_mul_wrong_type(simple):
+def test_mul_fixed_by_fixed(simple):
     first = TD(np.arange(0, 5, dtype="datetime64[D]"), np.ones(5) * 2)
     second = TD(np.array((-1, 0, 1), dtype="datetime64[D]"), np.ones(3).astype(float))
-    with pytest.raises(ValueError):
-        first * second
-    with pytest.raises(ValueError):
-        second * first
+    assert np.array_equal(first * second, second)
+    assert np.array_equal(second * first, first)
 
 
 def test_mul_td(simple):
     td2 = TD(np.array((-1, 0, 1), dtype="timedelta64[D]"), np.ones(3).astype(float))
 
     multiplied = simple * td2
```

### Comparing `bw_temporalis-0.9.3/tests/test_tdaware.py` & `bw_temporalis-1.0/tests/test_tdaware.py`

 * *Files identical despite different names*

### Comparing `bw_temporalis-0.9.3/tests/test_timeline.py` & `bw_temporalis-1.0/tests/test_timeline.py`

 * *Files identical despite different names*

### Comparing `bw_temporalis-0.9.3/tests/test_utils.py` & `bw_temporalis-1.0/tests/test_utils.py`

 * *Files identical despite different names*

