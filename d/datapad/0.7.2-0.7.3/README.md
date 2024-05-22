# Comparing `tmp/datapad-0.7.2.tar.gz` & `tmp/datapad-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datapad-0.7.2.tar", last modified: Tue May 21 20:23:32 2024, max compression
+gzip compressed data, was "datapad-0.7.3.tar", last modified: Wed May 22 22:31:13 2024, max compression
```

## Comparing `datapad-0.7.2.tar` & `datapad-0.7.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 huy        (501) staff       (20)        0 2024-05-21 20:23:32.915057 datapad-0.7.2/
--rw-r--r--   0 huy        (501) staff       (20)    11340 2019-12-30 21:17:14.000000 datapad-0.7.2/LICENSE
--rw-r--r--   0 huy        (501) staff       (20)     4350 2024-05-21 20:23:32.914795 datapad-0.7.2/PKG-INFO
--rw-r--r--   0 huy        (501) staff       (20)     3176 2024-05-21 19:05:30.000000 datapad-0.7.2/README.md
-drwxr-xr-x   0 huy        (501) staff       (20)        0 2024-05-21 20:23:32.910267 datapad-0.7.2/datapad/
--rw-r--r--   0 huy        (501) staff       (20)      608 2024-05-21 20:05:32.000000 datapad-0.7.2/datapad/__init__.py
--rw-r--r--   0 huy        (501) staff       (20)    13199 2020-01-08 20:06:49.000000 datapad-0.7.2/datapad/fields.py
--rw-r--r--   0 huy        (501) staff       (20)     8208 2024-05-21 20:22:17.000000 datapad-0.7.2/datapad/io.py
--rw-r--r--   0 huy        (501) staff       (20)    25915 2024-05-21 19:08:51.000000 datapad-0.7.2/datapad/sequence.py
--rw-r--r--   0 huy        (501) staff       (20)     2487 2024-05-21 19:54:19.000000 datapad-0.7.2/datapad/tests.py
-drwxr-xr-x   0 huy        (501) staff       (20)        0 2024-05-21 20:23:32.914353 datapad-0.7.2/datapad.egg-info/
--rw-r--r--   0 huy        (501) staff       (20)     4350 2024-05-21 20:23:32.000000 datapad-0.7.2/datapad.egg-info/PKG-INFO
--rw-r--r--   0 huy        (501) staff       (20)      239 2024-05-21 20:23:32.000000 datapad-0.7.2/datapad.egg-info/SOURCES.txt
--rw-r--r--   0 huy        (501) staff       (20)        1 2024-05-21 20:23:32.000000 datapad-0.7.2/datapad.egg-info/dependency_links.txt
--rw-r--r--   0 huy        (501) staff       (20)        8 2024-05-21 20:23:32.000000 datapad-0.7.2/datapad.egg-info/top_level.txt
--rw-r--r--   0 huy        (501) staff       (20)       38 2024-05-21 20:23:32.915173 datapad-0.7.2/setup.cfg
--rw-r--r--   0 huy        (501) staff       (20)     1317 2024-05-21 20:22:47.000000 datapad-0.7.2/setup.py
+drwxr-xr-x   0 huy        (501) staff       (20)        0 2024-05-22 22:31:13.223178 datapad-0.7.3/
+-rw-r--r--   0 huy        (501) staff       (20)    11340 2019-12-30 21:17:14.000000 datapad-0.7.3/LICENSE
+-rw-r--r--   0 huy        (501) staff       (20)     4350 2024-05-22 22:31:13.222789 datapad-0.7.3/PKG-INFO
+-rw-r--r--   0 huy        (501) staff       (20)     3176 2024-05-21 19:05:30.000000 datapad-0.7.3/README.md
+drwxr-xr-x   0 huy        (501) staff       (20)        0 2024-05-22 22:31:13.218483 datapad-0.7.3/datapad/
+-rw-r--r--   0 huy        (501) staff       (20)      608 2024-05-21 20:05:32.000000 datapad-0.7.3/datapad/__init__.py
+-rw-r--r--   0 huy        (501) staff       (20)    13199 2020-01-08 20:06:49.000000 datapad-0.7.3/datapad/fields.py
+-rw-r--r--   0 huy        (501) staff       (20)     8208 2024-05-21 20:22:17.000000 datapad-0.7.3/datapad/io.py
+-rw-r--r--   0 huy        (501) staff       (20)    26243 2024-05-22 22:28:22.000000 datapad-0.7.3/datapad/sequence.py
+-rw-r--r--   0 huy        (501) staff       (20)     2487 2024-05-21 19:54:19.000000 datapad-0.7.3/datapad/tests.py
+drwxr-xr-x   0 huy        (501) staff       (20)        0 2024-05-22 22:31:13.221500 datapad-0.7.3/datapad.egg-info/
+-rw-r--r--   0 huy        (501) staff       (20)     4350 2024-05-22 22:31:13.000000 datapad-0.7.3/datapad.egg-info/PKG-INFO
+-rw-r--r--   0 huy        (501) staff       (20)      239 2024-05-22 22:31:13.000000 datapad-0.7.3/datapad.egg-info/SOURCES.txt
+-rw-r--r--   0 huy        (501) staff       (20)        1 2024-05-22 22:31:13.000000 datapad-0.7.3/datapad.egg-info/dependency_links.txt
+-rw-r--r--   0 huy        (501) staff       (20)        8 2024-05-22 22:31:13.000000 datapad-0.7.3/datapad.egg-info/top_level.txt
+-rw-r--r--   0 huy        (501) staff       (20)       38 2024-05-22 22:31:13.223329 datapad-0.7.3/setup.cfg
+-rw-r--r--   0 huy        (501) staff       (20)     1317 2024-05-22 22:30:41.000000 datapad-0.7.3/setup.py
```

### Comparing `datapad-0.7.2/LICENSE` & `datapad-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `datapad-0.7.2/PKG-INFO` & `datapad-0.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datapad
-Version: 0.7.2
+Version: 0.7.3
 Summary: Datapad is a library of lazy data transformations for sequences; similar to spark and linq
 Home-page: https://github.com/huyng/datapad
 Author: Huy Nguyen
 Author-email: 
 License: UNKNOWN
 Description: <!--
         Copyright 2019 Huy Nguyen
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: datapad Version: 0.7.2 Summary: Datapad is a
+Metadata-Version: 2.1 Name: datapad Version: 0.7.3 Summary: Datapad is a
 library of lazy data transformations for sequences; similar to spark and linq
 Home-page: https://github.com/huyng/datapad Author: Huy Nguyen Author-email:
 License: UNKNOWN Description: # Datapad: A Fluent API for Exploratory Data
 Analysis
 [https://user-images.githubusercontent.com/121183/71599089-4cfe1080-2afe-11ea-
                             8852-81f00ed8c3fa.jpg]
 _[_h_t_t_p_s_:_/_/_t_r_a_v_i_s_-_c_i_._o_r_g_/_h_u_y_n_g_/_d_a_t_a_p_a_d_._s_v_g_?_b_r_a_n_c_h_=_m_a_s_t_e_r_]_[_h_t_t_p_s_:_/_/_b_a_d_g_e_._f_u_r_y_._i_o_/
```

### Comparing `datapad-0.7.2/README.md` & `datapad-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `datapad-0.7.2/datapad/__init__.py` & `datapad-0.7.3/datapad/__init__.py`

 * *Files identical despite different names*

### Comparing `datapad-0.7.2/datapad/fields.py` & `datapad-0.7.3/datapad/fields.py`

 * *Files identical despite different names*

### Comparing `datapad-0.7.2/datapad/io.py` & `datapad-0.7.3/datapad/io.py`

 * *Files identical despite different names*

### Comparing `datapad-0.7.2/datapad/sequence.py` & `datapad-0.7.3/datapad/sequence.py`

 * *Files 2% similar despite different names*

```diff
@@ -826,22 +826,32 @@
         >>> _ = seq.map(lambda x: x*2).progress().collect()
         """
 
         def _report(iterable):
             import time
             import sys
             t0 = time.time()
+            t_interval = 0
+            i = 0
             for i, elem in enumerate(iterable):
                 yield elem
-                t1 = time.time()
-                print('- secs/element: %.6fs, processed: %d' %
-                      ((t1-t0)/(i+1), (i+1)), end='\r', file=sys.stderr)
+                t_interval = time.time() - t0
+
+                # only print if time interval has elapse more 300 ms to
+                # avoid oversaturating outputs.
+                if t_interval > .300:
+                    print('- secs/element: %.6fs, processed: %d' %
+                          (t_interval/(i+1), i+1),
+                          end='\r',
+                          file=sys.stderr)
 
             print("", file=sys.stderr)
-            print('- total time: %.3fs' % (time.time()-t0), file=sys.stderr)
+            print('- total time: %.3fs, processed: %d' %
+                  (t_interval, i),
+                  file=sys.stderr)
 
         seq = Sequence(_iterable=_report(self._iterable))
         return seq
 
     def dump(self, sink):
         """
         Dump sequence into a sink function that will greedily consume
```

### Comparing `datapad-0.7.2/datapad/tests.py` & `datapad-0.7.3/datapad/tests.py`

 * *Files identical despite different names*

### Comparing `datapad-0.7.2/datapad.egg-info/PKG-INFO` & `datapad-0.7.3/datapad.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datapad
-Version: 0.7.2
+Version: 0.7.3
 Summary: Datapad is a library of lazy data transformations for sequences; similar to spark and linq
 Home-page: https://github.com/huyng/datapad
 Author: Huy Nguyen
 Author-email: 
 License: UNKNOWN
 Description: <!--
         Copyright 2019 Huy Nguyen
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: datapad Version: 0.7.2 Summary: Datapad is a
+Metadata-Version: 2.1 Name: datapad Version: 0.7.3 Summary: Datapad is a
 library of lazy data transformations for sequences; similar to spark and linq
 Home-page: https://github.com/huyng/datapad Author: Huy Nguyen Author-email:
 License: UNKNOWN Description: # Datapad: A Fluent API for Exploratory Data
 Analysis
 [https://user-images.githubusercontent.com/121183/71599089-4cfe1080-2afe-11ea-
                             8852-81f00ed8c3fa.jpg]
 _[_h_t_t_p_s_:_/_/_t_r_a_v_i_s_-_c_i_._o_r_g_/_h_u_y_n_g_/_d_a_t_a_p_a_d_._s_v_g_?_b_r_a_n_c_h_=_m_a_s_t_e_r_]_[_h_t_t_p_s_:_/_/_b_a_d_g_e_._f_u_r_y_._i_o_/
```

### Comparing `datapad-0.7.2/setup.py` & `datapad-0.7.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 
 setup(
     name='datapad',
-    version='0.7.2',
+    version='0.7.3',
     description='Datapad is a library of lazy data transformations for sequences; similar to spark and linq',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Huy Nguyen',
     author_email='',
     url='https://github.com/huyng/datapad',
     packages=['datapad'],
```

