# Comparing `tmp/datapad-0.7.3.tar.gz` & `tmp/datapad-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datapad-0.7.3.tar", last modified: Wed May 22 22:31:13 2024, max compression
+gzip compressed data, was "datapad-0.7.4.tar", last modified: Thu May 23 02:04:15 2024, max compression
```

## Comparing `datapad-0.7.3.tar` & `datapad-0.7.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 huy        (501) staff       (20)        0 2024-05-22 22:31:13.223178 datapad-0.7.3/
--rw-r--r--   0 huy        (501) staff       (20)    11340 2019-12-30 21:17:14.000000 datapad-0.7.3/LICENSE
--rw-r--r--   0 huy        (501) staff       (20)     4350 2024-05-22 22:31:13.222789 datapad-0.7.3/PKG-INFO
--rw-r--r--   0 huy        (501) staff       (20)     3176 2024-05-21 19:05:30.000000 datapad-0.7.3/README.md
-drwxr-xr-x   0 huy        (501) staff       (20)        0 2024-05-22 22:31:13.218483 datapad-0.7.3/datapad/
--rw-r--r--   0 huy        (501) staff       (20)      608 2024-05-21 20:05:32.000000 datapad-0.7.3/datapad/__init__.py
--rw-r--r--   0 huy        (501) staff       (20)    13199 2020-01-08 20:06:49.000000 datapad-0.7.3/datapad/fields.py
--rw-r--r--   0 huy        (501) staff       (20)     8208 2024-05-21 20:22:17.000000 datapad-0.7.3/datapad/io.py
--rw-r--r--   0 huy        (501) staff       (20)    26243 2024-05-22 22:28:22.000000 datapad-0.7.3/datapad/sequence.py
--rw-r--r--   0 huy        (501) staff       (20)     2487 2024-05-21 19:54:19.000000 datapad-0.7.3/datapad/tests.py
-drwxr-xr-x   0 huy        (501) staff       (20)        0 2024-05-22 22:31:13.221500 datapad-0.7.3/datapad.egg-info/
--rw-r--r--   0 huy        (501) staff       (20)     4350 2024-05-22 22:31:13.000000 datapad-0.7.3/datapad.egg-info/PKG-INFO
--rw-r--r--   0 huy        (501) staff       (20)      239 2024-05-22 22:31:13.000000 datapad-0.7.3/datapad.egg-info/SOURCES.txt
--rw-r--r--   0 huy        (501) staff       (20)        1 2024-05-22 22:31:13.000000 datapad-0.7.3/datapad.egg-info/dependency_links.txt
--rw-r--r--   0 huy        (501) staff       (20)        8 2024-05-22 22:31:13.000000 datapad-0.7.3/datapad.egg-info/top_level.txt
--rw-r--r--   0 huy        (501) staff       (20)       38 2024-05-22 22:31:13.223329 datapad-0.7.3/setup.cfg
--rw-r--r--   0 huy        (501) staff       (20)     1317 2024-05-22 22:30:41.000000 datapad-0.7.3/setup.py
+drwxr-xr-x   0 huy        (501) staff       (20)        0 2024-05-23 02:04:15.290373 datapad-0.7.4/
+-rw-r--r--   0 huy        (501) staff       (20)    11340 2019-12-30 21:17:14.000000 datapad-0.7.4/LICENSE
+-rw-r--r--   0 huy        (501) staff       (20)     4350 2024-05-23 02:04:15.289962 datapad-0.7.4/PKG-INFO
+-rw-r--r--   0 huy        (501) staff       (20)     3176 2024-05-21 19:05:30.000000 datapad-0.7.4/README.md
+drwxr-xr-x   0 huy        (501) staff       (20)        0 2024-05-23 02:04:15.286325 datapad-0.7.4/datapad/
+-rw-r--r--   0 huy        (501) staff       (20)      613 2024-05-23 02:00:40.000000 datapad-0.7.4/datapad/__init__.py
+-rw-r--r--   0 huy        (501) staff       (20)    13199 2020-01-08 20:06:49.000000 datapad-0.7.4/datapad/fields.py
+-rw-r--r--   0 huy        (501) staff       (20)     8208 2024-05-21 20:22:17.000000 datapad-0.7.4/datapad/io.py
+-rw-r--r--   0 huy        (501) staff       (20)    26498 2024-05-23 02:02:32.000000 datapad-0.7.4/datapad/sequence.py
+-rw-r--r--   0 huy        (501) staff       (20)     2487 2024-05-21 19:54:19.000000 datapad-0.7.4/datapad/tests.py
+drwxr-xr-x   0 huy        (501) staff       (20)        0 2024-05-23 02:04:15.288946 datapad-0.7.4/datapad.egg-info/
+-rw-r--r--   0 huy        (501) staff       (20)     4350 2024-05-23 02:04:15.000000 datapad-0.7.4/datapad.egg-info/PKG-INFO
+-rw-r--r--   0 huy        (501) staff       (20)      239 2024-05-23 02:04:15.000000 datapad-0.7.4/datapad.egg-info/SOURCES.txt
+-rw-r--r--   0 huy        (501) staff       (20)        1 2024-05-23 02:04:15.000000 datapad-0.7.4/datapad.egg-info/dependency_links.txt
+-rw-r--r--   0 huy        (501) staff       (20)        8 2024-05-23 02:04:15.000000 datapad-0.7.4/datapad.egg-info/top_level.txt
+-rw-r--r--   0 huy        (501) staff       (20)       38 2024-05-23 02:04:15.290536 datapad-0.7.4/setup.cfg
+-rw-r--r--   0 huy        (501) staff       (20)     1317 2024-05-23 02:02:51.000000 datapad-0.7.4/setup.py
```

### Comparing `datapad-0.7.3/LICENSE` & `datapad-0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `datapad-0.7.3/PKG-INFO` & `datapad-0.7.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datapad
-Version: 0.7.3
+Version: 0.7.4
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
-Metadata-Version: 2.1 Name: datapad Version: 0.7.3 Summary: Datapad is a
+Metadata-Version: 2.1 Name: datapad Version: 0.7.4 Summary: Datapad is a
 library of lazy data transformations for sequences; similar to spark and linq
 Home-page: https://github.com/huyng/datapad Author: Huy Nguyen Author-email:
 License: UNKNOWN Description: # Datapad: A Fluent API for Exploratory Data
 Analysis
 [https://user-images.githubusercontent.com/121183/71599089-4cfe1080-2afe-11ea-
                             8852-81f00ed8c3fa.jpg]
 _[_h_t_t_p_s_:_/_/_t_r_a_v_i_s_-_c_i_._o_r_g_/_h_u_y_n_g_/_d_a_t_a_p_a_d_._s_v_g_?_b_r_a_n_c_h_=_m_a_s_t_e_r_]_[_h_t_t_p_s_:_/_/_b_a_d_g_e_._f_u_r_y_._i_o_/
```

### Comparing `datapad-0.7.3/README.md` & `datapad-0.7.4/README.md`

 * *Files identical despite different names*

### Comparing `datapad-0.7.3/datapad/__init__.py` & `datapad-0.7.4/datapad/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 #    Software distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 
 from . import io
 from . import fields
-from .sequence import Sequence
+from .sequence import Sequence, Seq
```

### Comparing `datapad-0.7.3/datapad/fields.py` & `datapad-0.7.4/datapad/fields.py`

 * *Files identical despite different names*

### Comparing `datapad-0.7.3/datapad/io.py` & `datapad-0.7.4/datapad/io.py`

 * *Files identical despite different names*

### Comparing `datapad-0.7.3/datapad/sequence.py` & `datapad-0.7.4/datapad/sequence.py`

 * *Files 0% similar despite different names*

```diff
@@ -413,15 +413,15 @@
         ['a', 'b', 'c']
         """
         odict = collections.OrderedDict.fromkeys(list(self))
         return Sequence(_iterable=odict.keys())
 
     def zip_with_index(self):
         """
-        Add an to each item in sequence
+        Add an index to each item in sequence (e.g. enumerate)
 
         >>> seq = Sequence(['a', 'b', 'c'])
         >>> seq.zip_with_index().collect()
         [(0, 'a'), (1, 'b'), (2, 'c')]
         """
         seq = Sequence(_iterable=enumerate(self._iterable))
         return seq
@@ -584,26 +584,27 @@
         >>> seq.collect()
         []
 
         """
         result = list(self.all())
         return result
 
-    def sort(self, key=None):
+    def sort(self, key=None, reverse=False):
         """
         Eagerly sorts your sequence and returns a
         newly created sequence containing the sorted items.
         WARNING: this function loads the entirety of your sequence
         into memory.
 
         >>> seq = Sequence([2, 1, 0, 4, 3])
         >>> seq.sort().collect()
         [0, 1, 2, 3, 4]
         """
-        seq = Sequence(_iterable=sorted(list(self._iterable), key=key))
+        seq = Sequence(_iterable=sorted(
+            list(self._iterable), key=key, reverse=reverse))
         return seq
 
     def groupby(self, key=None, getter=None, eager_group=True):
         """
         Groups sequence using key function,
 
         Note: you must ensure elements are sorted by groups before
@@ -825,32 +826,37 @@
         >>> seq = Sequence(range(1000))
         >>> _ = seq.map(lambda x: x*2).progress().collect()
         """
 
         def _report(iterable):
             import time
             import sys
+
             t0 = time.time()
-            t_interval = 0
+            t_interval_avg = 0
+            t_last_print = time.time()
             i = 0
+
             for i, elem in enumerate(iterable):
                 yield elem
-                t_interval = time.time() - t0
 
                 # only print if time interval has elapse more 300 ms to
-                # avoid oversaturating outputs.
-                if t_interval > .300:
+                # avoid oversaturating output.
+                t1 = time.time()
+                if (t1 - t_last_print) > .300:
+                    t_interval_avg = (t1 - t0)/(i+1)
+                    t_last_print = t1
                     print('- secs/element: %.6fs, processed: %d' %
-                          (t_interval/(i+1), i+1),
+                          (t_interval_avg, i+1),
                           end='\r',
                           file=sys.stderr)
 
             print("", file=sys.stderr)
             print('- total time: %.3fs, processed: %d' %
-                  (t_interval, i),
+                  (t_interval_avg, i),
                   file=sys.stderr)
 
         seq = Sequence(_iterable=_report(self._iterable))
         return seq
 
     def dump(self, sink):
         """
@@ -869,10 +875,13 @@
 
         return sink(self)
 
     def __repr__(self):
         return '<Sequence at %s>' % hex(id(self))
 
 
+# syntatic sugar so one can do dp.Seq
+Seq = Sequence
+
 if __name__ == "__main__":
     import doctest
     doctest.testmod()
```

### Comparing `datapad-0.7.3/datapad/tests.py` & `datapad-0.7.4/datapad/tests.py`

 * *Files identical despite different names*

### Comparing `datapad-0.7.3/datapad.egg-info/PKG-INFO` & `datapad-0.7.4/datapad.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datapad
-Version: 0.7.3
+Version: 0.7.4
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
-Metadata-Version: 2.1 Name: datapad Version: 0.7.3 Summary: Datapad is a
+Metadata-Version: 2.1 Name: datapad Version: 0.7.4 Summary: Datapad is a
 library of lazy data transformations for sequences; similar to spark and linq
 Home-page: https://github.com/huyng/datapad Author: Huy Nguyen Author-email:
 License: UNKNOWN Description: # Datapad: A Fluent API for Exploratory Data
 Analysis
 [https://user-images.githubusercontent.com/121183/71599089-4cfe1080-2afe-11ea-
                             8852-81f00ed8c3fa.jpg]
 _[_h_t_t_p_s_:_/_/_t_r_a_v_i_s_-_c_i_._o_r_g_/_h_u_y_n_g_/_d_a_t_a_p_a_d_._s_v_g_?_b_r_a_n_c_h_=_m_a_s_t_e_r_]_[_h_t_t_p_s_:_/_/_b_a_d_g_e_._f_u_r_y_._i_o_/
```

### Comparing `datapad-0.7.3/setup.py` & `datapad-0.7.4/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,31 +9,32 @@
 #        http://www.apache.org/licenses/LICENSE-2.0
 #
 #    Software distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 
+from os import path
+from setuptools import setup
 import os
 os.environ['NOSE_DOCTEST_EXTENSION'] = 'txt'
 os.environ['NOSE_WITH_DOCTEST'] = 'True'
 os.environ['NOSE_WITH_DOCTESTS'] = 'True'
-from setuptools import setup
+
 
 # read the contents of your README file
-from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 
 setup(
     name='datapad',
-    version='0.7.3',
+    version='0.7.4',
     description='Datapad is a library of lazy data transformations for sequences; similar to spark and linq',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Huy Nguyen',
     author_email='',
     url='https://github.com/huyng/datapad',
-    packages=['datapad'],
+    packages=['datapad']
 )
```

