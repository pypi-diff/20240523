# Comparing `tmp/soma_integ-0.1.6.tar.gz` & `tmp/soma_integ-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "soma_integ-0.1.6.tar", last modified: Mon May 13 08:44:55 2024, max compression
+gzip compressed data, was "soma_integ-0.1.7.tar", last modified: Thu May 23 15:19:11 2024, max compression
```

## Comparing `soma_integ-0.1.6.tar` & `soma_integ-0.1.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 sobhan.ahmadian.moghadam   (501) staff       (20)        0 2024-05-13 08:44:55.376834 soma_integ-0.1.6/
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)     1073 2024-04-15 11:21:18.000000 soma_integ-0.1.6/LICENSE
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      750 2024-05-13 08:44:55.376606 soma_integ-0.1.6/PKG-INFO
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)        0 2024-04-15 11:15:15.000000 soma_integ-0.1.6/README.md
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      838 2024-05-13 08:44:16.000000 soma_integ-0.1.6/pyproject.toml
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)       38 2024-05-13 08:44:55.376883 soma_integ-0.1.6/setup.cfg
-drwxr-xr-x   0 sobhan.ahmadian.moghadam   (501) staff       (20)        0 2024-05-13 08:44:55.371407 soma_integ-0.1.6/src/
-drwxr-xr-x   0 sobhan.ahmadian.moghadam   (501) staff       (20)        0 2024-05-13 08:44:55.374404 soma_integ-0.1.6/src/soma_integ/
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      432 2024-05-12 19:26:59.000000 soma_integ-0.1.6/src/soma_integ/__init__.py
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)     1597 2024-05-12 08:37:42.000000 soma_integ-0.1.6/src/soma_integ/config.py
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)     3893 2024-05-13 08:22:30.000000 soma_integ-0.1.6/src/soma_integ/data.py
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)     8059 2024-05-13 08:43:19.000000 soma_integ-0.1.6/src/soma_integ/evaluation.py
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      822 2024-05-12 08:37:42.000000 soma_integ-0.1.6/src/soma_integ/methods.py
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)     1632 2024-05-12 08:37:42.000000 soma_integ-0.1.6/src/soma_integ/model.py
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)     8072 2024-05-12 08:37:42.000000 soma_integ-0.1.6/src/soma_integ/optimization.py
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      197 2024-03-04 18:10:58.000000 soma_integ-0.1.6/src/soma_integ/utils.py
-drwxr-xr-x   0 sobhan.ahmadian.moghadam   (501) staff       (20)        0 2024-05-13 08:44:55.376246 soma_integ-0.1.6/src/soma_integ.egg-info/
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      750 2024-05-13 08:44:55.000000 soma_integ-0.1.6/src/soma_integ.egg-info/PKG-INFO
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      474 2024-05-13 08:44:55.000000 soma_integ-0.1.6/src/soma_integ.egg-info/SOURCES.txt
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)        1 2024-05-13 08:44:55.000000 soma_integ-0.1.6/src/soma_integ.egg-info/dependency_links.txt
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)       31 2024-05-13 08:44:55.000000 soma_integ-0.1.6/src/soma_integ.egg-info/requires.txt
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)       11 2024-05-13 08:44:55.000000 soma_integ-0.1.6/src/soma_integ.egg-info/top_level.txt
-drwxr-xr-x   0 sobhan.ahmadian.moghadam   (501) staff       (20)        0 2024-05-13 08:44:55.375962 soma_integ-0.1.6/tests/
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      550 2024-05-12 18:49:52.000000 soma_integ-0.1.6/tests/test_data.py
--rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)     2169 2024-05-13 08:24:55.000000 soma_integ-0.1.6/tests/test_evaluation.py
+drwxr-xr-x   0 sobhan.ahmadian.moghadam   (501) staff       (20)        0 2024-05-23 15:19:11.854502 soma_integ-0.1.7/
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)     1073 2024-04-15 11:21:18.000000 soma_integ-0.1.7/LICENSE
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      750 2024-05-23 15:19:11.854234 soma_integ-0.1.7/PKG-INFO
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)        0 2024-04-15 11:15:15.000000 soma_integ-0.1.7/README.md
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      838 2024-05-23 15:16:41.000000 soma_integ-0.1.7/pyproject.toml
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)       38 2024-05-23 15:19:11.854702 soma_integ-0.1.7/setup.cfg
+drwxr-xr-x   0 sobhan.ahmadian.moghadam   (501) staff       (20)        0 2024-05-23 15:19:11.848570 soma_integ-0.1.7/src/
+drwxr-xr-x   0 sobhan.ahmadian.moghadam   (501) staff       (20)        0 2024-05-23 15:19:11.851745 soma_integ-0.1.7/src/soma_integ/
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      432 2024-05-12 19:26:59.000000 soma_integ-0.1.7/src/soma_integ/__init__.py
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)     1597 2024-05-12 08:37:42.000000 soma_integ-0.1.7/src/soma_integ/config.py
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)     3986 2024-05-23 15:15:49.000000 soma_integ-0.1.7/src/soma_integ/data.py
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)     8059 2024-05-13 08:43:19.000000 soma_integ-0.1.7/src/soma_integ/evaluation.py
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      822 2024-05-12 08:37:42.000000 soma_integ-0.1.7/src/soma_integ/methods.py
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)     1632 2024-05-12 08:37:42.000000 soma_integ-0.1.7/src/soma_integ/model.py
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)     8072 2024-05-12 08:37:42.000000 soma_integ-0.1.7/src/soma_integ/optimization.py
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      197 2024-03-04 18:10:58.000000 soma_integ-0.1.7/src/soma_integ/utils.py
+drwxr-xr-x   0 sobhan.ahmadian.moghadam   (501) staff       (20)        0 2024-05-23 15:19:11.853802 soma_integ-0.1.7/src/soma_integ.egg-info/
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      750 2024-05-23 15:19:11.000000 soma_integ-0.1.7/src/soma_integ.egg-info/PKG-INFO
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      474 2024-05-23 15:19:11.000000 soma_integ-0.1.7/src/soma_integ.egg-info/SOURCES.txt
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)        1 2024-05-23 15:19:11.000000 soma_integ-0.1.7/src/soma_integ.egg-info/dependency_links.txt
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)       31 2024-05-23 15:19:11.000000 soma_integ-0.1.7/src/soma_integ.egg-info/requires.txt
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)       11 2024-05-23 15:19:11.000000 soma_integ-0.1.7/src/soma_integ.egg-info/top_level.txt
+drwxr-xr-x   0 sobhan.ahmadian.moghadam   (501) staff       (20)        0 2024-05-23 15:19:11.853424 soma_integ-0.1.7/tests/
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)      550 2024-05-12 18:49:52.000000 soma_integ-0.1.7/tests/test_data.py
+-rw-r--r--   0 sobhan.ahmadian.moghadam   (501) staff       (20)     2169 2024-05-13 08:24:55.000000 soma_integ-0.1.7/tests/test_evaluation.py
```

### Comparing `soma_integ-0.1.6/LICENSE` & `soma_integ-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `soma_integ-0.1.6/PKG-INFO` & `soma_integ-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soma_integ
-Version: 0.1.6
+Version: 0.1.7
 Summary: A package for integrating implementation and evaluation of machine learning platforms
 Author-email: Sobhan Ahmadian Moghadam <sobhan.ahmadian.moghadam@gmail.com>, Arman Rezaei <arman.x.rezaei@gmail.com>
 Project-URL: Homepage, https://github.com/sobhanAhmadian/soma_integrate
 Project-URL: Issues, https://github.com/sobhanAhmadian/soma_integrate/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `soma_integ-0.1.6/pyproject.toml` & `soma_integ-0.1.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "soma_integ"
-version = "0.1.6"
+version = "0.1.7"
 dependencies = ["numpy", "scikit-learn"]
 authors = [
     { name = "Sobhan Ahmadian Moghadam", email = "sobhan.ahmadian.moghadam@gmail.com" },
     { name = "Arman Rezaei", email = "arman.x.rezaei@gmail.com" },
 ]
 description = "A package for integrating implementation and evaluation of machine learning platforms"
 readme = "README.md"
```

### Comparing `soma_integ-0.1.6/src/soma_integ/config.py` & `soma_integ-0.1.7/src/soma_integ/config.py`

 * *Files identical despite different names*

### Comparing `soma_integ-0.1.6/src/soma_integ/data.py` & `soma_integ-0.1.7/src/soma_integ/data.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,15 +25,16 @@
     Abstract base class for train-test splitters in cross-validation.
 
     Args:
         k (int): number of folds.
         data (Data): data object.
     """
 
-    def __init__(self, k: int, data: Data):
+    def __init__(self, k: int, data: Data, seed=42):
+        self.rng = random.Random(seed)  # rng should be create before get_subsets
         self.k = k
         self.data = data
         self.data_size = self.get_data_size()
         self.subsets = self.get_subsets()
 
     @abc.abstractmethod
     def split(self, i):
@@ -67,15 +68,15 @@
             dict: A dictionary containing subsets of data, where the keys represent the subset index and the values
                     represent the indices of the elements in the subset.
         """
         subsets = dict()
         subset_size = int(self.data_size / self.k)
         remain = list(range(0, self.data_size))
         for i in range(self.k - 1):
-            subsets[i] = random.sample(remain, subset_size)
+            subsets[i] = self.rng.sample(remain, subset_size)
             remain = list(set(remain).difference(subsets[i]))
         subsets[self.k - 1] = remain
         return subsets
 
 
 class PytorchData(Data):
     """
```

### Comparing `soma_integ-0.1.6/src/soma_integ/evaluation.py` & `soma_integ-0.1.7/src/soma_integ/evaluation.py`

 * *Files identical despite different names*

### Comparing `soma_integ-0.1.6/src/soma_integ/methods.py` & `soma_integ-0.1.7/src/soma_integ/methods.py`

 * *Files identical despite different names*

### Comparing `soma_integ-0.1.6/src/soma_integ/model.py` & `soma_integ-0.1.7/src/soma_integ/model.py`

 * *Files identical despite different names*

### Comparing `soma_integ-0.1.6/src/soma_integ/optimization.py` & `soma_integ-0.1.7/src/soma_integ/optimization.py`

 * *Files identical despite different names*

### Comparing `soma_integ-0.1.6/src/soma_integ.egg-info/PKG-INFO` & `soma_integ-0.1.7/src/soma_integ.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: soma_integ
-Version: 0.1.6
+Version: 0.1.7
 Summary: A package for integrating implementation and evaluation of machine learning platforms
 Author-email: Sobhan Ahmadian Moghadam <sobhan.ahmadian.moghadam@gmail.com>, Arman Rezaei <arman.x.rezaei@gmail.com>
 Project-URL: Homepage, https://github.com/sobhanAhmadian/soma_integrate
 Project-URL: Issues, https://github.com/sobhanAhmadian/soma_integrate/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `soma_integ-0.1.6/tests/test_data.py` & `soma_integ-0.1.7/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `soma_integ-0.1.6/tests/test_evaluation.py` & `soma_integ-0.1.7/tests/test_evaluation.py`

 * *Files identical despite different names*

