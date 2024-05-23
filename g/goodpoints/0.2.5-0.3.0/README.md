# Comparing `tmp/goodpoints-0.2.5.tar.gz` & `tmp/goodpoints-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "goodpoints-0.2.5.tar", last modified: Thu Oct 19 04:12:14 2023, max compression
+gzip compressed data, was "goodpoints-0.3.0.tar", last modified: Thu May 23 13:37:41 2024, max compression
```

## Comparing `goodpoints-0.2.5.tar` & `goodpoints-0.3.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 lmackey    (501) staff       (20)        0 2023-10-19 04:12:14.363021 goodpoints-0.2.5/
--rw-r--r--   0 lmackey    (501) staff       (20)     1141 2023-10-19 02:33:12.000000 goodpoints-0.2.5/LICENSE
--rw-r--r--   0 lmackey    (501) staff       (20)       50 2023-10-19 02:33:12.000000 goodpoints-0.2.5/MANIFEST.in
--rw-r--r--   0 lmackey    (501) staff       (20)    10775 2023-10-19 04:12:14.361531 goodpoints-0.2.5/PKG-INFO
--rw-r--r--   0 lmackey    (501) staff       (20)    10498 2023-10-19 03:03:21.000000 goodpoints-0.2.5/README.md
-drwxr-xr-x   0 lmackey    (501) staff       (20)        0 2023-10-19 04:12:14.352397 goodpoints-0.2.5/goodpoints/
--rw-r--r--   0 lmackey    (501) staff       (20)        0 2023-10-19 02:35:19.000000 goodpoints-0.2.5/goodpoints/__init__.py
--rw-r--r--   0 lmackey    (501) staff       (20)    12401 2023-10-19 02:35:20.000000 goodpoints-0.2.5/goodpoints/compress.py
--rw-r--r--   0 lmackey    (501) staff       (20)  1202190 2023-10-19 03:28:12.000000 goodpoints-0.2.5/goodpoints/compressc.c
--rw-r--r--   0 lmackey    (501) staff       (20)    18354 2023-10-19 02:35:08.000000 goodpoints-0.2.5/goodpoints/compressc.pyx
--rw-r--r--   0 lmackey    (501) staff       (20)    39749 2023-10-19 02:35:20.000000 goodpoints-0.2.5/goodpoints/ctt.py
--rw-r--r--   0 lmackey    (501) staff       (20)  1129496 2023-10-19 03:28:12.000000 goodpoints-0.2.5/goodpoints/cttc.c
--rw-r--r--   0 lmackey    (501) staff       (20)     8009 2023-10-19 02:35:09.000000 goodpoints-0.2.5/goodpoints/cttc.pyx
--rw-r--r--   0 lmackey    (501) staff       (20)  1632166 2023-10-19 03:28:13.000000 goodpoints-0.2.5/goodpoints/gaussianc.c
--rw-r--r--   0 lmackey    (501) staff       (20)      414 2023-10-19 02:34:58.000000 goodpoints-0.2.5/goodpoints/gaussianc.pxd
--rw-r--r--   0 lmackey    (501) staff       (20)    49474 2023-10-19 02:35:09.000000 goodpoints-0.2.5/goodpoints/gaussianc.pyx
--rw-r--r--   0 lmackey    (501) staff       (20)     2292 2023-10-19 02:35:21.000000 goodpoints-0.2.5/goodpoints/herding.py
--rw-r--r--   0 lmackey    (501) staff       (20)    34933 2023-10-19 03:03:21.000000 goodpoints-0.2.5/goodpoints/kt.py
--rw-r--r--   0 lmackey    (501) staff       (20)  1283638 2023-10-19 03:28:13.000000 goodpoints-0.2.5/goodpoints/ktc.c
--rw-r--r--   0 lmackey    (501) staff       (20)      435 2023-10-19 02:34:59.000000 goodpoints-0.2.5/goodpoints/ktc.pxd
--rw-r--r--   0 lmackey    (501) staff       (20)    28635 2023-10-19 02:35:10.000000 goodpoints-0.2.5/goodpoints/ktc.pyx
--rw-r--r--   0 lmackey    (501) staff       (20)   998195 2023-10-19 04:12:13.000000 goodpoints-0.2.5/goodpoints/sobolevc.c
--rw-r--r--   0 lmackey    (501) staff       (20)      396 2023-10-19 02:34:59.000000 goodpoints-0.2.5/goodpoints/sobolevc.pxd
--rw-r--r--   0 lmackey    (501) staff       (20)     6161 2023-10-19 02:35:10.000000 goodpoints-0.2.5/goodpoints/sobolevc.pyx
--rw-r--r--   0 lmackey    (501) staff       (20)     7721 2023-10-19 02:35:23.000000 goodpoints-0.2.5/goodpoints/tictoc.py
--rw-r--r--   0 lmackey    (501) staff       (20)      756 2023-10-19 02:35:24.000000 goodpoints-0.2.5/goodpoints/util.py
-drwxr-xr-x   0 lmackey    (501) staff       (20)        0 2023-10-19 04:12:14.360706 goodpoints-0.2.5/goodpoints.egg-info/
--rw-r--r--   0 lmackey    (501) staff       (20)    10775 2023-10-19 04:12:14.000000 goodpoints-0.2.5/goodpoints.egg-info/PKG-INFO
--rw-r--r--   0 lmackey    (501) staff       (20)      659 2023-10-19 04:12:14.000000 goodpoints-0.2.5/goodpoints.egg-info/SOURCES.txt
--rw-r--r--   0 lmackey    (501) staff       (20)        1 2023-10-19 04:12:14.000000 goodpoints-0.2.5/goodpoints.egg-info/dependency_links.txt
--rw-r--r--   0 lmackey    (501) staff       (20)        6 2023-10-19 04:12:14.000000 goodpoints-0.2.5/goodpoints.egg-info/requires.txt
--rw-r--r--   0 lmackey    (501) staff       (20)       11 2023-10-19 04:12:14.000000 goodpoints-0.2.5/goodpoints.egg-info/top_level.txt
--rw-r--r--   0 lmackey    (501) staff       (20)      108 2023-10-19 02:33:13.000000 goodpoints-0.2.5/pyproject.toml
--rw-r--r--   0 lmackey    (501) staff       (20)      390 2023-10-19 04:12:14.366852 goodpoints-0.2.5/setup.cfg
--rw-r--r--   0 lmackey    (501) staff       (20)     2033 2023-10-19 04:09:39.000000 goodpoints-0.2.5/setup.py
+drwxr-xr-x   0 lmackey    (501) staff       (20)        0 2024-05-23 13:37:41.318153 goodpoints-0.3.0/
+-rw-r--r--   0 lmackey    (501) staff       (20)     1141 2024-05-23 12:40:58.000000 goodpoints-0.3.0/LICENSE
+-rw-r--r--   0 lmackey    (501) staff       (20)       50 2024-05-23 12:40:58.000000 goodpoints-0.3.0/MANIFEST.in
+-rw-r--r--   0 lmackey    (501) staff       (20)    12353 2024-05-23 13:37:41.317520 goodpoints-0.3.0/PKG-INFO
+-rw-r--r--   0 lmackey    (501) staff       (20)    12076 2024-05-23 12:40:58.000000 goodpoints-0.3.0/README.md
+drwxr-xr-x   0 lmackey    (501) staff       (20)        0 2024-05-23 13:37:41.308944 goodpoints-0.3.0/goodpoints/
+-rw-r--r--   0 lmackey    (501) staff       (20)        0 2024-05-23 12:40:58.000000 goodpoints-0.3.0/goodpoints/__init__.py
+-rw-r--r--   0 lmackey    (501) staff       (20)    12401 2024-05-23 12:40:58.000000 goodpoints-0.3.0/goodpoints/compress.py
+-rw-r--r--   0 lmackey    (501) staff       (20)  1201839 2024-05-23 12:45:39.000000 goodpoints-0.3.0/goodpoints/compressc.c
+-rw-r--r--   0 lmackey    (501) staff       (20)    18354 2024-05-23 12:40:58.000000 goodpoints-0.3.0/goodpoints/compressc.pyx
+-rw-r--r--   0 lmackey    (501) staff       (20)    39749 2024-05-23 12:40:58.000000 goodpoints-0.3.0/goodpoints/ctt.py
+-rw-r--r--   0 lmackey    (501) staff       (20)  1129145 2024-05-23 12:45:39.000000 goodpoints-0.3.0/goodpoints/cttc.c
+-rw-r--r--   0 lmackey    (501) staff       (20)     8009 2024-05-23 12:40:58.000000 goodpoints-0.3.0/goodpoints/cttc.pyx
+-rw-r--r--   0 lmackey    (501) staff       (20)  1631815 2024-05-23 12:45:40.000000 goodpoints-0.3.0/goodpoints/gaussianc.c
+-rw-r--r--   0 lmackey    (501) staff       (20)      414 2024-05-23 12:40:58.000000 goodpoints-0.3.0/goodpoints/gaussianc.pxd
+-rw-r--r--   0 lmackey    (501) staff       (20)    49474 2024-05-23 12:40:58.000000 goodpoints-0.3.0/goodpoints/gaussianc.pyx
+-rw-r--r--   0 lmackey    (501) staff       (20)     2292 2024-05-23 12:40:58.000000 goodpoints-0.3.0/goodpoints/herding.py
+-rw-r--r--   0 lmackey    (501) staff       (20)    34933 2024-05-23 12:40:58.000000 goodpoints-0.3.0/goodpoints/kt.py
+-rw-r--r--   0 lmackey    (501) staff       (20)  1283287 2024-05-23 12:45:40.000000 goodpoints-0.3.0/goodpoints/ktc.c
+-rw-r--r--   0 lmackey    (501) staff       (20)      435 2024-05-23 12:40:58.000000 goodpoints-0.3.0/goodpoints/ktc.pxd
+-rw-r--r--   0 lmackey    (501) staff       (20)    28635 2024-05-23 12:40:58.000000 goodpoints-0.3.0/goodpoints/ktc.pyx
+-rw-r--r--   0 lmackey    (501) staff       (20)   997844 2024-05-23 12:45:41.000000 goodpoints-0.3.0/goodpoints/sobolevc.c
+-rw-r--r--   0 lmackey    (501) staff       (20)      396 2024-05-23 12:40:58.000000 goodpoints-0.3.0/goodpoints/sobolevc.pxd
+-rw-r--r--   0 lmackey    (501) staff       (20)     6161 2024-05-23 12:40:58.000000 goodpoints-0.3.0/goodpoints/sobolevc.pyx
+-rw-r--r--   0 lmackey    (501) staff       (20)     7721 2024-05-23 12:40:58.000000 goodpoints-0.3.0/goodpoints/tictoc.py
+-rw-r--r--   0 lmackey    (501) staff       (20)      756 2024-05-23 12:40:58.000000 goodpoints-0.3.0/goodpoints/util.py
+drwxr-xr-x   0 lmackey    (501) staff       (20)        0 2024-05-23 13:37:41.316657 goodpoints-0.3.0/goodpoints.egg-info/
+-rw-r--r--   0 lmackey    (501) staff       (20)    12353 2024-05-23 13:37:41.000000 goodpoints-0.3.0/goodpoints.egg-info/PKG-INFO
+-rw-r--r--   0 lmackey    (501) staff       (20)      659 2024-05-23 13:37:41.000000 goodpoints-0.3.0/goodpoints.egg-info/SOURCES.txt
+-rw-r--r--   0 lmackey    (501) staff       (20)        1 2024-05-23 13:37:41.000000 goodpoints-0.3.0/goodpoints.egg-info/dependency_links.txt
+-rw-r--r--   0 lmackey    (501) staff       (20)        6 2024-05-23 13:37:41.000000 goodpoints-0.3.0/goodpoints.egg-info/requires.txt
+-rw-r--r--   0 lmackey    (501) staff       (20)       11 2024-05-23 13:37:41.000000 goodpoints-0.3.0/goodpoints.egg-info/top_level.txt
+-rw-r--r--   0 lmackey    (501) staff       (20)      108 2024-05-23 12:40:58.000000 goodpoints-0.3.0/pyproject.toml
+-rw-r--r--   0 lmackey    (501) staff       (20)      390 2024-05-23 13:37:41.319338 goodpoints-0.3.0/setup.cfg
+-rw-r--r--   0 lmackey    (501) staff       (20)     2029 2024-05-23 12:40:58.000000 goodpoints-0.3.0/setup.py
```

### Comparing `goodpoints-0.2.5/LICENSE` & `goodpoints-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `goodpoints-0.2.5/PKG-INFO` & `goodpoints-0.3.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goodpoints
-Version: 0.2.5
+Version: 0.3.0
 Summary: Tools to generate concise high-quality summaries of a probability distribution
 Home-page: https://github.com/microsoft/goodpoints
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 
 # GoodPoints
@@ -12,20 +12,23 @@
 ### A Python package for generating concise, high-quality summaries of a probability distribution
 
 GoodPoints is a collection of tools for compressing a distribution more effectively than independent sampling:
 
 - Given an initial summary of n input points, **kernel thinning** returns s << n output points with comparable integration error across a reproducing kernel Hilbert space
 - **Compress++** reduces the runtime of generic thinning algorithms with minimal loss in accuracy
 - **Compress Then Test** accelerates kernel two-sample testing using high-fidelity compression
+- **Stein Kernel Thinning**, **Stein Recombination**, and **Stein Cholesky** deliver unweighted, simplex-weighted, and constant-preserving coresets that reduce biases due to off-target sampling, tempering, or burn-in
 
 ## Installation
 To install the `goodpoints` package, use the following pip command:
 ```
 pip install goodpoints
 ```
+For **Debiased Distribution Compression**, JAX and additional dependencies are required. See [goodpoints/jax](goodpoints/jax) for more details.
+
 ## Getting started
 The primary kernel thinning function is `thin` in the `kt` module:
 ```python
 from goodpoints import kt
 coreset = kt.thin(X, m, split_kernel, swap_kernel, delta=0.5, seed=None, store_K=False, 
                   meanK=None, unique=False, verbose=False)
     """Returns kernel thinning coreset of size floor(n/2^m) as row indices into X
@@ -108,14 +111,22 @@
       delta: KT-Compress failure probability
       
     Returns: TestResults object.
     """
 ```
 For example uses, please refer to [examples/mmd_test/test.py](examples/mmd_test/test.py).
 
+The primary Debiased Distribution Compression functions are in the `jax.dtc` module, including:
+- Stein Kernel Thinning (`skt`) and Low-rank Stein Kernel Thinning (`lskt`) for equal-weighted coresets
+- Stein Recombination (`sr`) and Low-rank Stein Recombination (`lsr`) for simplex-weighted coresets
+- Stein Cholesky (`sc`) and Low-rank Stein Cholesky (`lsc`) for constant-preserving coresets
+
+Moreover, Debiased Distribution Compression provides JAX implementation of Kernel Thinning, Compress++, and [Stein Thinning](https://arxiv.org/pdf/2005.03952) that can be of independent interest.
+Please refer to [goodpoints/jax/README.md](goodpoints/jax/README.md) for all available functions.
+
 ## Examples
 
 Code in the `examples` directory uses the `goodpoints` package to recreate the experiments of the following research papers.
 ***
 #### [Kernel Thinning](https://arxiv.org/pdf/2105.05842.pdf)
 ```
 @article{dwivedi2021kernel,
@@ -169,14 +180,29 @@
   series={Proceedings of Machine Learning Research},
   month={25--27 Apr},
   publisher={PMLR}
 }
 ```
 See [examples/mmd_test/README.md](examples/mmd_test/README.md).
 
+#### [Debiased Distribution Compression](https://arxiv.org/pdf/2404.12290)
+```
+@InProceedings{li2024debiased,
+    title = {Debiased Distribution Compression},
+    author = {Li, Lingxiao and Dwivedi, Raaz and Mackey, Lester},,
+    booktitle = {Proceedings of the 41st International Conference on Machine Learning},
+    year = {2024},
+    volume = {203},
+    series = {Proceedings of Machine Learning Research},
+    month = {21--27 Jul},
+    publisher = {PMLR},
+}
+```
+See [examples/debias/README.md](examples/debias/README.md).
+
 ## Contributing
 
 This project welcomes contributions and suggestions.  Most contributions require you to agree to a
 Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us
 the rights to use your contribution. For details, visit https://cla.opensource.microsoft.com.
 
 When you submit a pull request, a CLA bot will automatically determine whether you need to provide
```

### Comparing `goodpoints-0.2.5/README.md` & `goodpoints-0.3.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -3,20 +3,23 @@
 ### A Python package for generating concise, high-quality summaries of a probability distribution
 
 GoodPoints is a collection of tools for compressing a distribution more effectively than independent sampling:
 
 - Given an initial summary of n input points, **kernel thinning** returns s << n output points with comparable integration error across a reproducing kernel Hilbert space
 - **Compress++** reduces the runtime of generic thinning algorithms with minimal loss in accuracy
 - **Compress Then Test** accelerates kernel two-sample testing using high-fidelity compression
+- **Stein Kernel Thinning**, **Stein Recombination**, and **Stein Cholesky** deliver unweighted, simplex-weighted, and constant-preserving coresets that reduce biases due to off-target sampling, tempering, or burn-in
 
 ## Installation
 To install the `goodpoints` package, use the following pip command:
 ```
 pip install goodpoints
 ```
+For **Debiased Distribution Compression**, JAX and additional dependencies are required. See [goodpoints/jax](goodpoints/jax) for more details.
+
 ## Getting started
 The primary kernel thinning function is `thin` in the `kt` module:
 ```python
 from goodpoints import kt
 coreset = kt.thin(X, m, split_kernel, swap_kernel, delta=0.5, seed=None, store_K=False, 
                   meanK=None, unique=False, verbose=False)
     """Returns kernel thinning coreset of size floor(n/2^m) as row indices into X
@@ -99,14 +102,22 @@
       delta: KT-Compress failure probability
       
     Returns: TestResults object.
     """
 ```
 For example uses, please refer to [examples/mmd_test/test.py](examples/mmd_test/test.py).
 
+The primary Debiased Distribution Compression functions are in the `jax.dtc` module, including:
+- Stein Kernel Thinning (`skt`) and Low-rank Stein Kernel Thinning (`lskt`) for equal-weighted coresets
+- Stein Recombination (`sr`) and Low-rank Stein Recombination (`lsr`) for simplex-weighted coresets
+- Stein Cholesky (`sc`) and Low-rank Stein Cholesky (`lsc`) for constant-preserving coresets
+
+Moreover, Debiased Distribution Compression provides JAX implementation of Kernel Thinning, Compress++, and [Stein Thinning](https://arxiv.org/pdf/2005.03952) that can be of independent interest.
+Please refer to [goodpoints/jax/README.md](goodpoints/jax/README.md) for all available functions.
+
 ## Examples
 
 Code in the `examples` directory uses the `goodpoints` package to recreate the experiments of the following research papers.
 ***
 #### [Kernel Thinning](https://arxiv.org/pdf/2105.05842.pdf)
 ```
 @article{dwivedi2021kernel,
@@ -160,14 +171,29 @@
   series={Proceedings of Machine Learning Research},
   month={25--27 Apr},
   publisher={PMLR}
 }
 ```
 See [examples/mmd_test/README.md](examples/mmd_test/README.md).
 
+#### [Debiased Distribution Compression](https://arxiv.org/pdf/2404.12290)
+```
+@InProceedings{li2024debiased,
+    title = {Debiased Distribution Compression},
+    author = {Li, Lingxiao and Dwivedi, Raaz and Mackey, Lester},,
+    booktitle = {Proceedings of the 41st International Conference on Machine Learning},
+    year = {2024},
+    volume = {203},
+    series = {Proceedings of Machine Learning Research},
+    month = {21--27 Jul},
+    publisher = {PMLR},
+}
+```
+See [examples/debias/README.md](examples/debias/README.md).
+
 ## Contributing
 
 This project welcomes contributions and suggestions.  Most contributions require you to agree to a
 Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us
 the rights to use your contribution. For details, visit https://cla.opensource.microsoft.com.
 
 When you submit a pull request, a CLA bot will automatically determine whether you need to provide
```

### Comparing `goodpoints-0.2.5/goodpoints/compress.py` & `goodpoints-0.3.0/goodpoints/compress.py`

 * *Files identical despite different names*

### Comparing `goodpoints-0.2.5/goodpoints/compressc.c` & `goodpoints-0.3.0/goodpoints/compressc.c`

 * *Files 1% similar despite different names*

```diff
@@ -1556,177 +1556,177 @@
   Py_ssize_t strides[8];
   Py_ssize_t suboffsets[8];
 } __Pyx_memviewslice;
 #define __Pyx_MemoryView_Len(m)  (m.shape[0])
 
 /* #### Code section: numeric_typedefs ### */
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":730
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":730
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":731
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":731
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":732
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":732
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":733
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":733
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":737
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":737
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":738
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":738
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":739
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":739
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":740
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":740
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":744
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":744
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":745
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":745
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":754
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":754
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":755
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":755
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":757
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":757
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":758
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":758
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":760
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":760
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":761
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":761
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":763
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":763
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":764
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":764
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":765
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":765
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1762,42 +1762,42 @@
 struct __pyx_obj_5numpy_6random_13bit_generator_SeedSequence;
 struct __pyx_obj_5numpy_6random_13bit_generator_SeedlessSequence;
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":767
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":767
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":768
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":768
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":769
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":769
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":771
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":771
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -18106,261 +18106,261 @@
   __Pyx_XDECREF(__pyx_v_parts);
   __Pyx_XDECREF(__pyx_v_extents);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":245
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_7ndarray_4base_base(PyArrayObject *__pyx_v_self) {
   PyObject *__pyx_r;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":248
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":248
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  *             return PyArray_BASE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_BASE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":245
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":251
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
 static CYTHON_INLINE PyArray_Descr *__pyx_f_5numpy_7ndarray_5descr_descr(PyArrayObject *__pyx_v_self) {
   PyArray_Descr *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyArray_Descr *__pyx_t_1;
   __Pyx_RefNannySetupContext("descr", 0);
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":254
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":254
  *             """Returns an owned reference to the dtype of the array.
  *             """
  *             return <dtype>PyArray_DESCR(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
   __pyx_t_1 = PyArray_DESCR(__pyx_v_self);
   __Pyx_INCREF((PyObject *)((PyArray_Descr *)__pyx_t_1));
   __pyx_r = ((PyArray_Descr *)__pyx_t_1);
   goto __pyx_L0;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":251
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":257
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_7ndarray_4ndim_ndim(PyArrayObject *__pyx_v_self) {
   int __pyx_r;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":260
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":260
  *             """Returns the number of dimensions in the array.
  *             """
  *             return PyArray_NDIM(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_NDIM(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":257
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":263
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_5shape_shape(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":268
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":268
  *             Can return NULL for 0-dimensional arrays.
  *             """
  *             return PyArray_DIMS(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_DIMS(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":263
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":271
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_7strides_strides(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":275
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":275
  *             The number of elements matches the number of dimensions of the array (ndim).
  *             """
  *             return PyArray_STRIDES(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_STRIDES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":271
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":278
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
 static CYTHON_INLINE npy_intp __pyx_f_5numpy_7ndarray_4size_size(PyArrayObject *__pyx_v_self) {
   npy_intp __pyx_r;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":281
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":281
  *             """Returns the total size (in number of elements) of the array.
  *             """
  *             return PyArray_SIZE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_SIZE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":278
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":284
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
 static CYTHON_INLINE char *__pyx_f_5numpy_7ndarray_4data_data(PyArrayObject *__pyx_v_self) {
   char *__pyx_r;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":290
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":290
  *             of `PyArray_DATA()` instead, which returns a 'void*'.
  *             """
  *             return PyArray_BYTES(self)             # <<<<<<<<<<<<<<
  * 
  *     ctypedef unsigned char      npy_bool
  */
   __pyx_r = PyArray_BYTES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":284
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":773
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -18369,29 +18369,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":774
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":774
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 774, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":773
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -18402,15 +18402,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":776
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -18419,29 +18419,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":777
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":777
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 777, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":776
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -18452,15 +18452,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":779
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -18469,29 +18469,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":780
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":780
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 780, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":779
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -18502,15 +18502,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":782
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -18519,29 +18519,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":783
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":783
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 783, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":782
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -18552,15 +18552,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":785
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -18569,29 +18569,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":786
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":786
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 786, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":785
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -18602,89 +18602,89 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":788
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":789
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = PyDataType_HASSUBARRAY(__pyx_v_d);
   if (__pyx_t_1) {
 
-    /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":790
+    /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":790
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":789
+    /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":792
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":792
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":788
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":967
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":967
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
@@ -18692,33 +18692,33 @@
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":968
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":968
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":969
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":969
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(2, 969, __pyx_L1_error)
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":967
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":967
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
@@ -18726,96 +18726,96 @@
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_AddTraceback("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":971
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":971
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":972
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":972
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":973
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":973
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = (__pyx_v_base == NULL);
   if (__pyx_t_1) {
 
-    /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":974
+    /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":974
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":973
+    /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":973
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":975
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":975
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":971
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":971
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":979
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":979
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -18831,15 +18831,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":980
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":980
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -18847,68 +18847,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":981
+      /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":981
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 981, __pyx_L3_error)
 
-      /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":980
+      /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":980
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":982
+    /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":982
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 982, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":983
+      /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":983
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__15, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 983, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 983, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":980
+    /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":980
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -18916,15 +18916,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":979
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":979
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -18939,15 +18939,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":985
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":985
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -18963,15 +18963,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -18979,68 +18979,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":987
+      /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":987
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 987, __pyx_L3_error)
 
-      /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
+      /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":988
+    /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":988
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 988, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":989
+      /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":989
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__16, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 989, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 989, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
+    /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -19048,15 +19048,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":985
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":985
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19071,15 +19071,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":991
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":991
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19095,15 +19095,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -19111,68 +19111,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":993
+      /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":993
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 993, __pyx_L3_error)
 
-      /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
+      /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":994
+    /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":994
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 994, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":995
+      /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":995
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * 
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__16, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 995, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 995, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
+    /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -19180,15 +19180,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":991
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":991
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19203,176 +19203,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":998
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":998
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1010
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1010
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":998
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":998
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1013
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1013
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1025
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1025
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1013
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1013
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1028
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1028
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1035
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1035
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1028
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1028
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1038
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1038
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1042
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1042
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1038
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1038
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1045
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1045
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1049
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1049
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1045
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1045
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -22603,26 +22603,26 @@
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0x82a3537, 0x6ae9995, 0xb068931) = (name))" % __pyx_checksum
  */
   __pyx_tuple__8 = PyTuple_Pack(3, __pyx_int_136983863, __pyx_int_112105877, __pyx_int_184977713); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__8);
   __Pyx_GIVEREF(__pyx_tuple__8);
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":983
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":983
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__15 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(2, 983, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__15);
   __Pyx_GIVEREF(__pyx_tuple__15);
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":989
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":989
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__16 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(2, 989, __pyx_L1_error)
```

### Comparing `goodpoints-0.2.5/goodpoints/compressc.pyx` & `goodpoints-0.3.0/goodpoints/compressc.pyx`

 * *Files identical despite different names*

### Comparing `goodpoints-0.2.5/goodpoints/ctt.py` & `goodpoints-0.3.0/goodpoints/ctt.py`

 * *Files identical despite different names*

### Comparing `goodpoints-0.2.5/goodpoints/cttc.c` & `goodpoints-0.3.0/goodpoints/cttc.c`

 * *Files 0% similar despite different names*

```diff
@@ -1552,177 +1552,177 @@
   Py_ssize_t strides[8];
   Py_ssize_t suboffsets[8];
 } __Pyx_memviewslice;
 #define __Pyx_MemoryView_Len(m)  (m.shape[0])
 
 /* #### Code section: numeric_typedefs ### */
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":730
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":730
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":731
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":731
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":732
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":732
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":733
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":733
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":737
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":737
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":738
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":738
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":739
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":739
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":740
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":740
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":744
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":744
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":745
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":745
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":754
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":754
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":755
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":755
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":757
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":757
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":758
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":758
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":760
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":760
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":761
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":761
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":763
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":763
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":764
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":764
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":765
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":765
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1755,42 +1755,42 @@
 
 /*--- Type declarations ---*/
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":767
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":767
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":768
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":768
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":769
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":769
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":771
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":771
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -17488,261 +17488,261 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":245
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_7ndarray_4base_base(PyArrayObject *__pyx_v_self) {
   PyObject *__pyx_r;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":248
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":248
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  *             return PyArray_BASE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_BASE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":245
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":251
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
 static CYTHON_INLINE PyArray_Descr *__pyx_f_5numpy_7ndarray_5descr_descr(PyArrayObject *__pyx_v_self) {
   PyArray_Descr *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyArray_Descr *__pyx_t_1;
   __Pyx_RefNannySetupContext("descr", 0);
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":254
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":254
  *             """Returns an owned reference to the dtype of the array.
  *             """
  *             return <dtype>PyArray_DESCR(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
   __pyx_t_1 = PyArray_DESCR(__pyx_v_self);
   __Pyx_INCREF((PyObject *)((PyArray_Descr *)__pyx_t_1));
   __pyx_r = ((PyArray_Descr *)__pyx_t_1);
   goto __pyx_L0;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":251
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":257
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_7ndarray_4ndim_ndim(PyArrayObject *__pyx_v_self) {
   int __pyx_r;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":260
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":260
  *             """Returns the number of dimensions in the array.
  *             """
  *             return PyArray_NDIM(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_NDIM(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":257
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":263
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_5shape_shape(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":268
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":268
  *             Can return NULL for 0-dimensional arrays.
  *             """
  *             return PyArray_DIMS(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_DIMS(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":263
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":271
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_7strides_strides(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":275
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":275
  *             The number of elements matches the number of dimensions of the array (ndim).
  *             """
  *             return PyArray_STRIDES(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_STRIDES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":271
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":278
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
 static CYTHON_INLINE npy_intp __pyx_f_5numpy_7ndarray_4size_size(PyArrayObject *__pyx_v_self) {
   npy_intp __pyx_r;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":281
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":281
  *             """Returns the total size (in number of elements) of the array.
  *             """
  *             return PyArray_SIZE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_SIZE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":278
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":284
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
 static CYTHON_INLINE char *__pyx_f_5numpy_7ndarray_4data_data(PyArrayObject *__pyx_v_self) {
   char *__pyx_r;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":290
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":290
  *             of `PyArray_DATA()` instead, which returns a 'void*'.
  *             """
  *             return PyArray_BYTES(self)             # <<<<<<<<<<<<<<
  * 
  *     ctypedef unsigned char      npy_bool
  */
   __pyx_r = PyArray_BYTES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":284
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":773
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -17751,29 +17751,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":774
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":774
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 774, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":773
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -17784,15 +17784,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":776
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -17801,29 +17801,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":777
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":777
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 777, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":776
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -17834,15 +17834,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":779
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -17851,29 +17851,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":780
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":780
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 780, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":779
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -17884,15 +17884,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":782
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -17901,29 +17901,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":783
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":783
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 783, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":782
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -17934,15 +17934,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":785
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -17951,29 +17951,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":786
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":786
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 786, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":785
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -17984,89 +17984,89 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":788
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":789
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = PyDataType_HASSUBARRAY(__pyx_v_d);
   if (__pyx_t_1) {
 
-    /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":790
+    /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":790
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":789
+    /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":792
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":792
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":788
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":967
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":967
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
@@ -18074,33 +18074,33 @@
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":968
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":968
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":969
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":969
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(2, 969, __pyx_L1_error)
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":967
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":967
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
@@ -18108,96 +18108,96 @@
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_AddTraceback("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":971
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":971
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":972
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":972
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":973
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":973
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = (__pyx_v_base == NULL);
   if (__pyx_t_1) {
 
-    /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":974
+    /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":974
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":973
+    /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":973
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":975
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":975
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":971
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":971
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":979
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":979
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -18213,15 +18213,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":980
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":980
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -18229,68 +18229,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":981
+      /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":981
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 981, __pyx_L3_error)
 
-      /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":980
+      /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":980
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":982
+    /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":982
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 982, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":983
+      /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":983
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 983, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 983, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":980
+    /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":980
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -18298,15 +18298,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":979
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":979
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -18321,15 +18321,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":985
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":985
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -18345,15 +18345,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -18361,68 +18361,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":987
+      /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":987
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 987, __pyx_L3_error)
 
-      /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
+      /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":988
+    /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":988
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 988, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":989
+      /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":989
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 989, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 989, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
+    /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -18430,15 +18430,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":985
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":985
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -18453,15 +18453,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":991
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":991
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -18477,15 +18477,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -18493,68 +18493,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":993
+      /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":993
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 993, __pyx_L3_error)
 
-      /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
+      /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":994
+    /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":994
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 994, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":995
+      /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":995
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * 
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 995, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 995, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
+    /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -18562,15 +18562,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":991
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":991
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -18585,176 +18585,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":998
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":998
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1010
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1010
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":998
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":998
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1013
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1013
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1025
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1025
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1013
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1013
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1028
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1028
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1035
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1035
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1028
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1028
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1038
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1038
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1042
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1042
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1038
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1038
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1045
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1045
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1049
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1049
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1045
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1045
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -21495,26 +21495,26 @@
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0x82a3537, 0x6ae9995, 0xb068931) = (name))" % __pyx_checksum
  */
   __pyx_tuple__8 = PyTuple_Pack(3, __pyx_int_136983863, __pyx_int_112105877, __pyx_int_184977713); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__8);
   __Pyx_GIVEREF(__pyx_tuple__8);
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":983
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":983
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(2, 983, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__9);
   __Pyx_GIVEREF(__pyx_tuple__9);
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":989
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":989
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(2, 989, __pyx_L1_error)
```

### Comparing `goodpoints-0.2.5/goodpoints/cttc.pyx` & `goodpoints-0.3.0/goodpoints/cttc.pyx`

 * *Files identical despite different names*

### Comparing `goodpoints-0.2.5/goodpoints/gaussianc.c` & `goodpoints-0.3.0/goodpoints/gaussianc.c`

 * *Files 0% similar despite different names*

```diff
@@ -1555,177 +1555,177 @@
   Py_ssize_t strides[8];
   Py_ssize_t suboffsets[8];
 } __Pyx_memviewslice;
 #define __Pyx_MemoryView_Len(m)  (m.shape[0])
 
 /* #### Code section: numeric_typedefs ### */
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":730
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":730
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":731
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":731
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":732
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":732
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":733
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":733
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":737
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":737
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":738
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":738
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":739
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":739
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":740
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":740
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":744
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":744
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":745
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":745
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":754
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":754
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":755
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":755
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":757
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":757
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":758
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":758
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":760
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":760
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":761
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":761
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":763
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":763
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":764
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":764
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":765
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":765
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1758,42 +1758,42 @@
 
 /*--- Type declarations ---*/
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":767
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":767
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":768
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":768
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":769
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":769
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":771
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":771
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -17888,261 +17888,261 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":245
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_7ndarray_4base_base(PyArrayObject *__pyx_v_self) {
   PyObject *__pyx_r;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":248
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":248
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  *             return PyArray_BASE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_BASE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":245
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":251
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
 static CYTHON_INLINE PyArray_Descr *__pyx_f_5numpy_7ndarray_5descr_descr(PyArrayObject *__pyx_v_self) {
   PyArray_Descr *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyArray_Descr *__pyx_t_1;
   __Pyx_RefNannySetupContext("descr", 0);
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":254
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":254
  *             """Returns an owned reference to the dtype of the array.
  *             """
  *             return <dtype>PyArray_DESCR(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
   __pyx_t_1 = PyArray_DESCR(__pyx_v_self);
   __Pyx_INCREF((PyObject *)((PyArray_Descr *)__pyx_t_1));
   __pyx_r = ((PyArray_Descr *)__pyx_t_1);
   goto __pyx_L0;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":251
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":257
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_7ndarray_4ndim_ndim(PyArrayObject *__pyx_v_self) {
   int __pyx_r;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":260
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":260
  *             """Returns the number of dimensions in the array.
  *             """
  *             return PyArray_NDIM(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_NDIM(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":257
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":263
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_5shape_shape(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":268
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":268
  *             Can return NULL for 0-dimensional arrays.
  *             """
  *             return PyArray_DIMS(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_DIMS(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":263
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":271
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_7strides_strides(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":275
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":275
  *             The number of elements matches the number of dimensions of the array (ndim).
  *             """
  *             return PyArray_STRIDES(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_STRIDES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":271
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":278
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
 static CYTHON_INLINE npy_intp __pyx_f_5numpy_7ndarray_4size_size(PyArrayObject *__pyx_v_self) {
   npy_intp __pyx_r;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":281
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":281
  *             """Returns the total size (in number of elements) of the array.
  *             """
  *             return PyArray_SIZE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_SIZE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":278
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":284
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
 static CYTHON_INLINE char *__pyx_f_5numpy_7ndarray_4data_data(PyArrayObject *__pyx_v_self) {
   char *__pyx_r;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":290
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":290
  *             of `PyArray_DATA()` instead, which returns a 'void*'.
  *             """
  *             return PyArray_BYTES(self)             # <<<<<<<<<<<<<<
  * 
  *     ctypedef unsigned char      npy_bool
  */
   __pyx_r = PyArray_BYTES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":284
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":773
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -18151,29 +18151,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":774
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":774
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 774, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":773
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -18184,15 +18184,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":776
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -18201,29 +18201,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":777
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":777
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 777, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":776
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -18234,15 +18234,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":779
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -18251,29 +18251,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":780
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":780
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 780, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":779
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -18284,15 +18284,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":782
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -18301,29 +18301,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":783
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":783
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 783, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":782
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -18334,15 +18334,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":785
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -18351,29 +18351,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":786
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":786
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 786, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":785
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -18384,89 +18384,89 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":788
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":789
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = PyDataType_HASSUBARRAY(__pyx_v_d);
   if (__pyx_t_1) {
 
-    /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":790
+    /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":790
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":789
+    /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":792
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":792
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":788
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":967
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":967
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
@@ -18474,33 +18474,33 @@
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":968
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":968
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":969
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":969
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(2, 969, __pyx_L1_error)
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":967
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":967
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
@@ -18508,96 +18508,96 @@
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_AddTraceback("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":971
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":971
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":972
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":972
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":973
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":973
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = (__pyx_v_base == NULL);
   if (__pyx_t_1) {
 
-    /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":974
+    /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":974
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":973
+    /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":973
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":975
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":975
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":971
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":971
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":979
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":979
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -18613,15 +18613,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":980
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":980
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -18629,68 +18629,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":981
+      /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":981
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 981, __pyx_L3_error)
 
-      /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":980
+      /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":980
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":982
+    /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":982
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 982, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":983
+      /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":983
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 983, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 983, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":980
+    /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":980
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -18698,15 +18698,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":979
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":979
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -18721,15 +18721,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":985
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":985
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -18745,15 +18745,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -18761,68 +18761,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":987
+      /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":987
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 987, __pyx_L3_error)
 
-      /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
+      /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":988
+    /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":988
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 988, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":989
+      /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":989
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 989, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 989, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
+    /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -18830,15 +18830,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":985
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":985
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -18853,15 +18853,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":991
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":991
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -18877,15 +18877,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -18893,68 +18893,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":993
+      /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":993
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 993, __pyx_L3_error)
 
-      /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
+      /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":994
+    /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":994
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 994, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":995
+      /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":995
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * 
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 995, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 995, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
+    /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -18962,15 +18962,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":991
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":991
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -18985,176 +18985,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":998
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":998
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1010
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1010
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":998
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":998
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1013
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1013
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1025
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1025
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1013
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1013
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1028
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1028
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1035
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1035
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1028
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1028
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1038
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1038
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1042
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1042
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1038
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1038
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1045
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1045
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1049
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1049
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1045
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1045
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -31316,26 +31316,26 @@
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0x82a3537, 0x6ae9995, 0xb068931) = (name))" % __pyx_checksum
  */
   __pyx_tuple__8 = PyTuple_Pack(3, __pyx_int_136983863, __pyx_int_112105877, __pyx_int_184977713); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__8);
   __Pyx_GIVEREF(__pyx_tuple__8);
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":983
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":983
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(2, 983, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__9);
   __Pyx_GIVEREF(__pyx_tuple__9);
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":989
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":989
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(2, 989, __pyx_L1_error)
```

### Comparing `goodpoints-0.2.5/goodpoints/gaussianc.pyx` & `goodpoints-0.3.0/goodpoints/gaussianc.pyx`

 * *Files identical despite different names*

### Comparing `goodpoints-0.2.5/goodpoints/herding.py` & `goodpoints-0.3.0/goodpoints/herding.py`

 * *Files identical despite different names*

### Comparing `goodpoints-0.2.5/goodpoints/kt.py` & `goodpoints-0.3.0/goodpoints/kt.py`

 * *Files identical despite different names*

### Comparing `goodpoints-0.2.5/goodpoints/ktc.c` & `goodpoints-0.3.0/goodpoints/ktc.c`

 * *Files 0% similar despite different names*

```diff
@@ -1558,177 +1558,177 @@
   Py_ssize_t strides[8];
   Py_ssize_t suboffsets[8];
 } __Pyx_memviewslice;
 #define __Pyx_MemoryView_Len(m)  (m.shape[0])
 
 /* #### Code section: numeric_typedefs ### */
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":730
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":730
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":731
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":731
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":732
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":732
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":733
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":733
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":737
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":737
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":738
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":738
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":739
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":739
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":740
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":740
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":744
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":744
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":745
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":745
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":754
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":754
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":755
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":755
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":757
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":757
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":758
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":758
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":760
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":760
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":761
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":761
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":763
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":763
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":764
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":764
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":765
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":765
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1764,42 +1764,42 @@
 struct __pyx_obj_5numpy_6random_13bit_generator_SeedSequence;
 struct __pyx_obj_5numpy_6random_13bit_generator_SeedlessSequence;
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":767
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":767
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":768
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":768
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":769
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":769
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":771
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":771
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -18121,261 +18121,261 @@
   __Pyx_XDECREF(__pyx_v_parts);
   __Pyx_XDECREF(__pyx_v_extents);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":245
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_7ndarray_4base_base(PyArrayObject *__pyx_v_self) {
   PyObject *__pyx_r;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":248
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":248
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  *             return PyArray_BASE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_BASE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":245
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":251
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
 static CYTHON_INLINE PyArray_Descr *__pyx_f_5numpy_7ndarray_5descr_descr(PyArrayObject *__pyx_v_self) {
   PyArray_Descr *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyArray_Descr *__pyx_t_1;
   __Pyx_RefNannySetupContext("descr", 0);
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":254
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":254
  *             """Returns an owned reference to the dtype of the array.
  *             """
  *             return <dtype>PyArray_DESCR(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
   __pyx_t_1 = PyArray_DESCR(__pyx_v_self);
   __Pyx_INCREF((PyObject *)((PyArray_Descr *)__pyx_t_1));
   __pyx_r = ((PyArray_Descr *)__pyx_t_1);
   goto __pyx_L0;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":251
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":257
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_7ndarray_4ndim_ndim(PyArrayObject *__pyx_v_self) {
   int __pyx_r;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":260
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":260
  *             """Returns the number of dimensions in the array.
  *             """
  *             return PyArray_NDIM(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_NDIM(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":257
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":263
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_5shape_shape(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":268
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":268
  *             Can return NULL for 0-dimensional arrays.
  *             """
  *             return PyArray_DIMS(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_DIMS(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":263
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":271
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_7strides_strides(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":275
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":275
  *             The number of elements matches the number of dimensions of the array (ndim).
  *             """
  *             return PyArray_STRIDES(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_STRIDES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":271
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":278
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
 static CYTHON_INLINE npy_intp __pyx_f_5numpy_7ndarray_4size_size(PyArrayObject *__pyx_v_self) {
   npy_intp __pyx_r;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":281
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":281
  *             """Returns the total size (in number of elements) of the array.
  *             """
  *             return PyArray_SIZE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_SIZE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":278
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":284
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
 static CYTHON_INLINE char *__pyx_f_5numpy_7ndarray_4data_data(PyArrayObject *__pyx_v_self) {
   char *__pyx_r;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":290
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":290
  *             of `PyArray_DATA()` instead, which returns a 'void*'.
  *             """
  *             return PyArray_BYTES(self)             # <<<<<<<<<<<<<<
  * 
  *     ctypedef unsigned char      npy_bool
  */
   __pyx_r = PyArray_BYTES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":284
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":773
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -18384,29 +18384,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":774
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":774
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 774, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":773
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -18417,15 +18417,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":776
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -18434,29 +18434,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":777
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":777
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 777, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":776
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -18467,15 +18467,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":779
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -18484,29 +18484,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":780
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":780
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 780, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":779
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -18517,15 +18517,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":782
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -18534,29 +18534,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":783
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":783
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 783, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":782
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -18567,15 +18567,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":785
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -18584,29 +18584,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":786
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":786
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 786, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":785
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -18617,89 +18617,89 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":788
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":789
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = PyDataType_HASSUBARRAY(__pyx_v_d);
   if (__pyx_t_1) {
 
-    /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":790
+    /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":790
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":789
+    /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":792
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":792
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":788
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":967
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":967
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
@@ -18707,33 +18707,33 @@
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":968
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":968
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":969
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":969
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(2, 969, __pyx_L1_error)
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":967
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":967
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
@@ -18741,96 +18741,96 @@
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_AddTraceback("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":971
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":971
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":972
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":972
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":973
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":973
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = (__pyx_v_base == NULL);
   if (__pyx_t_1) {
 
-    /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":974
+    /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":974
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":973
+    /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":973
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":975
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":975
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":971
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":971
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":979
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":979
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -18846,15 +18846,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":980
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":980
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -18862,68 +18862,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":981
+      /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":981
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 981, __pyx_L3_error)
 
-      /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":980
+      /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":980
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":982
+    /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":982
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 982, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":983
+      /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":983
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__15, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 983, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 983, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":980
+    /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":980
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -18931,15 +18931,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":979
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":979
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -18954,15 +18954,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":985
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":985
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -18978,15 +18978,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -18994,68 +18994,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":987
+      /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":987
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 987, __pyx_L3_error)
 
-      /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
+      /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":988
+    /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":988
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 988, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":989
+      /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":989
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__16, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 989, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 989, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
+    /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -19063,15 +19063,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":985
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":985
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19086,15 +19086,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":991
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":991
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19110,15 +19110,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -19126,68 +19126,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":993
+      /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":993
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 993, __pyx_L3_error)
 
-      /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
+      /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":994
+    /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":994
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 994, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":995
+      /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":995
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * 
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__16, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 995, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 995, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
+    /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -19195,15 +19195,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":991
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":991
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19218,176 +19218,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":998
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":998
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1010
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1010
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":998
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":998
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1013
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1013
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1025
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1025
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1013
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1013
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1028
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1028
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1035
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1035
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1028
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1028
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1038
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1038
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1042
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1042
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1038
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1038
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1045
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1045
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1049
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1049
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1045
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1045
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -24961,26 +24961,26 @@
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0x82a3537, 0x6ae9995, 0xb068931) = (name))" % __pyx_checksum
  */
   __pyx_tuple__8 = PyTuple_Pack(3, __pyx_int_136983863, __pyx_int_112105877, __pyx_int_184977713); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__8);
   __Pyx_GIVEREF(__pyx_tuple__8);
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":983
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":983
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__15 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(2, 983, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__15);
   __Pyx_GIVEREF(__pyx_tuple__15);
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":989
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":989
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__16 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(2, 989, __pyx_L1_error)
```

### Comparing `goodpoints-0.2.5/goodpoints/ktc.pyx` & `goodpoints-0.3.0/goodpoints/ktc.pyx`

 * *Files identical despite different names*

### Comparing `goodpoints-0.2.5/goodpoints/sobolevc.c` & `goodpoints-0.3.0/goodpoints/sobolevc.c`

 * *Files 0% similar despite different names*

```diff
@@ -1552,177 +1552,177 @@
   Py_ssize_t strides[8];
   Py_ssize_t suboffsets[8];
 } __Pyx_memviewslice;
 #define __Pyx_MemoryView_Len(m)  (m.shape[0])
 
 /* #### Code section: numeric_typedefs ### */
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":730
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":730
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":731
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":731
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":732
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":732
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":733
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":733
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":737
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":737
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":738
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":738
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":739
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":739
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":740
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":740
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":744
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":744
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":745
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":745
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":754
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":754
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":755
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":755
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":757
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":757
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":758
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":758
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":760
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":760
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":761
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":761
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":763
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":763
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":764
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":764
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":765
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":765
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1755,42 +1755,42 @@
 
 /*--- Type declarations ---*/
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":767
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":767
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":768
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":768
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":769
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":769
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":771
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":771
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -17197,261 +17197,261 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":245
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_7ndarray_4base_base(PyArrayObject *__pyx_v_self) {
   PyObject *__pyx_r;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":248
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":248
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  *             return PyArray_BASE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_BASE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":245
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":251
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
 static CYTHON_INLINE PyArray_Descr *__pyx_f_5numpy_7ndarray_5descr_descr(PyArrayObject *__pyx_v_self) {
   PyArray_Descr *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyArray_Descr *__pyx_t_1;
   __Pyx_RefNannySetupContext("descr", 0);
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":254
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":254
  *             """Returns an owned reference to the dtype of the array.
  *             """
  *             return <dtype>PyArray_DESCR(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
   __pyx_t_1 = PyArray_DESCR(__pyx_v_self);
   __Pyx_INCREF((PyObject *)((PyArray_Descr *)__pyx_t_1));
   __pyx_r = ((PyArray_Descr *)__pyx_t_1);
   goto __pyx_L0;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":251
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":257
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_7ndarray_4ndim_ndim(PyArrayObject *__pyx_v_self) {
   int __pyx_r;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":260
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":260
  *             """Returns the number of dimensions in the array.
  *             """
  *             return PyArray_NDIM(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_NDIM(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":257
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":263
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_5shape_shape(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":268
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":268
  *             Can return NULL for 0-dimensional arrays.
  *             """
  *             return PyArray_DIMS(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_DIMS(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":263
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":271
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_7strides_strides(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":275
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":275
  *             The number of elements matches the number of dimensions of the array (ndim).
  *             """
  *             return PyArray_STRIDES(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_STRIDES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":271
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":278
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
 static CYTHON_INLINE npy_intp __pyx_f_5numpy_7ndarray_4size_size(PyArrayObject *__pyx_v_self) {
   npy_intp __pyx_r;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":281
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":281
  *             """Returns the total size (in number of elements) of the array.
  *             """
  *             return PyArray_SIZE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_SIZE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":278
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":284
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
 static CYTHON_INLINE char *__pyx_f_5numpy_7ndarray_4data_data(PyArrayObject *__pyx_v_self) {
   char *__pyx_r;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":290
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":290
  *             of `PyArray_DATA()` instead, which returns a 'void*'.
  *             """
  *             return PyArray_BYTES(self)             # <<<<<<<<<<<<<<
  * 
  *     ctypedef unsigned char      npy_bool
  */
   __pyx_r = PyArray_BYTES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":284
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":773
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -17460,29 +17460,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":774
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":774
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 774, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":773
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -17493,15 +17493,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":776
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -17510,29 +17510,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":777
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":777
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 777, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":776
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -17543,15 +17543,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":779
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -17560,29 +17560,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":780
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":780
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 780, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":779
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -17593,15 +17593,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":782
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -17610,29 +17610,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":783
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":783
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 783, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":782
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -17643,15 +17643,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":785
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -17660,29 +17660,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":786
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":786
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 786, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":785
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -17693,89 +17693,89 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":788
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":789
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = PyDataType_HASSUBARRAY(__pyx_v_d);
   if (__pyx_t_1) {
 
-    /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":790
+    /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":790
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":789
+    /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":792
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":792
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":788
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":967
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":967
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
@@ -17783,33 +17783,33 @@
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":968
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":968
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":969
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":969
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(2, 969, __pyx_L1_error)
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":967
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":967
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
@@ -17817,96 +17817,96 @@
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_AddTraceback("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":971
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":971
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":972
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":972
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":973
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":973
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = (__pyx_v_base == NULL);
   if (__pyx_t_1) {
 
-    /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":974
+    /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":974
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":973
+    /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":973
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":975
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":975
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":971
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":971
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":979
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":979
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -17922,15 +17922,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":980
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":980
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -17938,68 +17938,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":981
+      /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":981
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 981, __pyx_L3_error)
 
-      /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":980
+      /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":980
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":982
+    /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":982
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 982, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":983
+      /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":983
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 983, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 983, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":980
+    /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":980
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -18007,15 +18007,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":979
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":979
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -18030,15 +18030,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":985
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":985
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -18054,15 +18054,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -18070,68 +18070,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":987
+      /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":987
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 987, __pyx_L3_error)
 
-      /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
+      /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":988
+    /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":988
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 988, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":989
+      /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":989
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 989, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 989, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
+    /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -18139,15 +18139,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":985
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":985
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -18162,15 +18162,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":991
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":991
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -18186,15 +18186,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -18202,68 +18202,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":993
+      /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":993
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 993, __pyx_L3_error)
 
-      /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
+      /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":994
+    /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":994
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 994, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":995
+      /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":995
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * 
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 995, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 995, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
+    /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -18271,15 +18271,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":991
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":991
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -18294,176 +18294,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":998
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":998
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1010
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1010
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":998
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":998
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1013
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1013
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1025
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1025
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1013
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1013
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1028
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1028
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1035
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1035
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1028
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1028
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1038
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1038
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1042
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1042
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1038
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1038
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1045
+/* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1045
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1049
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1049
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1045
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1045
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -20236,26 +20236,26 @@
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0x82a3537, 0x6ae9995, 0xb068931) = (name))" % __pyx_checksum
  */
   __pyx_tuple__8 = PyTuple_Pack(3, __pyx_int_136983863, __pyx_int_112105877, __pyx_int_184977713); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__8);
   __Pyx_GIVEREF(__pyx_tuple__8);
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":983
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":983
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(2, 983, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__9);
   __Pyx_GIVEREF(__pyx_tuple__9);
 
-  /* "../../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":989
+  /* "../../opt/anaconda3/envs/goodpoints/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":989
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(2, 989, __pyx_L1_error)
```

### Comparing `goodpoints-0.2.5/goodpoints/sobolevc.pyx` & `goodpoints-0.3.0/goodpoints/sobolevc.pyx`

 * *Files identical despite different names*

### Comparing `goodpoints-0.2.5/goodpoints/tictoc.py` & `goodpoints-0.3.0/goodpoints/tictoc.py`

 * *Files identical despite different names*

### Comparing `goodpoints-0.2.5/goodpoints/util.py` & `goodpoints-0.3.0/goodpoints/util.py`

 * *Files identical despite different names*

### Comparing `goodpoints-0.2.5/goodpoints.egg-info/PKG-INFO` & `goodpoints-0.3.0/goodpoints.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: goodpoints
-Version: 0.2.5
+Version: 0.3.0
 Summary: Tools to generate concise high-quality summaries of a probability distribution
 Home-page: https://github.com/microsoft/goodpoints
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 
 # GoodPoints
@@ -12,20 +12,23 @@
 ### A Python package for generating concise, high-quality summaries of a probability distribution
 
 GoodPoints is a collection of tools for compressing a distribution more effectively than independent sampling:
 
 - Given an initial summary of n input points, **kernel thinning** returns s << n output points with comparable integration error across a reproducing kernel Hilbert space
 - **Compress++** reduces the runtime of generic thinning algorithms with minimal loss in accuracy
 - **Compress Then Test** accelerates kernel two-sample testing using high-fidelity compression
+- **Stein Kernel Thinning**, **Stein Recombination**, and **Stein Cholesky** deliver unweighted, simplex-weighted, and constant-preserving coresets that reduce biases due to off-target sampling, tempering, or burn-in
 
 ## Installation
 To install the `goodpoints` package, use the following pip command:
 ```
 pip install goodpoints
 ```
+For **Debiased Distribution Compression**, JAX and additional dependencies are required. See [goodpoints/jax](goodpoints/jax) for more details.
+
 ## Getting started
 The primary kernel thinning function is `thin` in the `kt` module:
 ```python
 from goodpoints import kt
 coreset = kt.thin(X, m, split_kernel, swap_kernel, delta=0.5, seed=None, store_K=False, 
                   meanK=None, unique=False, verbose=False)
     """Returns kernel thinning coreset of size floor(n/2^m) as row indices into X
@@ -108,14 +111,22 @@
       delta: KT-Compress failure probability
       
     Returns: TestResults object.
     """
 ```
 For example uses, please refer to [examples/mmd_test/test.py](examples/mmd_test/test.py).
 
+The primary Debiased Distribution Compression functions are in the `jax.dtc` module, including:
+- Stein Kernel Thinning (`skt`) and Low-rank Stein Kernel Thinning (`lskt`) for equal-weighted coresets
+- Stein Recombination (`sr`) and Low-rank Stein Recombination (`lsr`) for simplex-weighted coresets
+- Stein Cholesky (`sc`) and Low-rank Stein Cholesky (`lsc`) for constant-preserving coresets
+
+Moreover, Debiased Distribution Compression provides JAX implementation of Kernel Thinning, Compress++, and [Stein Thinning](https://arxiv.org/pdf/2005.03952) that can be of independent interest.
+Please refer to [goodpoints/jax/README.md](goodpoints/jax/README.md) for all available functions.
+
 ## Examples
 
 Code in the `examples` directory uses the `goodpoints` package to recreate the experiments of the following research papers.
 ***
 #### [Kernel Thinning](https://arxiv.org/pdf/2105.05842.pdf)
 ```
 @article{dwivedi2021kernel,
@@ -169,14 +180,29 @@
   series={Proceedings of Machine Learning Research},
   month={25--27 Apr},
   publisher={PMLR}
 }
 ```
 See [examples/mmd_test/README.md](examples/mmd_test/README.md).
 
+#### [Debiased Distribution Compression](https://arxiv.org/pdf/2404.12290)
+```
+@InProceedings{li2024debiased,
+    title = {Debiased Distribution Compression},
+    author = {Li, Lingxiao and Dwivedi, Raaz and Mackey, Lester},,
+    booktitle = {Proceedings of the 41st International Conference on Machine Learning},
+    year = {2024},
+    volume = {203},
+    series = {Proceedings of Machine Learning Research},
+    month = {21--27 Jul},
+    publisher = {PMLR},
+}
+```
+See [examples/debias/README.md](examples/debias/README.md).
+
 ## Contributing
 
 This project welcomes contributions and suggestions.  Most contributions require you to agree to a
 Contributor License Agreement (CLA) declaring that you have the right to, and actually do, grant us
 the rights to use your contribution. For details, visit https://cla.opensource.microsoft.com.
 
 When you submit a pull request, a CLA bot will automatically determine whether you need to provide
```

### Comparing `goodpoints-0.2.5/goodpoints.egg-info/SOURCES.txt` & `goodpoints-0.3.0/goodpoints.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `goodpoints-0.2.5/setup.py` & `goodpoints-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,37 +19,37 @@
     ),
     Extension(
         "goodpoints.compressc", [join("goodpoints","compressc.pyx")],
         extra_compile_args=['-O3'],
         language="c", include_dirs=[numpy.get_include()],
         library_dirs=[lib_path_npyrandom,lib_path_npymath],
         libraries=['npyrandom','npymath','m'],
-    ), 
+    ),
     Extension(
         "goodpoints.cttc", [join("goodpoints","cttc.pyx")],
         extra_compile_args=['-O3'],
         language="c", include_dirs=[numpy.get_include()],
         library_dirs=[lib_path_npyrandom,lib_path_npymath],
         libraries=['npyrandom','npymath','m'],
-    ), 
+    ),
     Extension(
         "goodpoints.gaussianc", [join("goodpoints","gaussianc.pyx")],
         extra_compile_args=['-O3'],
         language="c", include_dirs=[numpy.get_include()],
         library_dirs=[lib_path_npyrandom,lib_path_npymath],
         libraries=['npyrandom','npymath','m'],
     ),
     Extension(
         "goodpoints.sobolevc", [join("goodpoints","sobolevc.pyx")],
         extra_compile_args=['-O3'],
         language="c", include_dirs=[numpy.get_include()],
         library_dirs=[lib_path_npyrandom,lib_path_npymath],
         libraries=['npyrandom','npymath','m'],
-    ), 
+    ),
 ]
 
-# Path to Cython declaration (PXD) files 
+# Path to Cython declaration (PXD) files
 include_path = ["goodpoints"]
 
 setup(include_package_data=True,
       ext_modules=cythonize(extensions, language_level = "3",
                             include_path=include_path))
```

