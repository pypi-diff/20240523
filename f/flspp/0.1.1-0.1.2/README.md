# Comparing `tmp/flspp-0.1.1.tar.gz` & `tmp/flspp-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flspp-0.1.1.tar", max compression
+gzip compressed data, was "flspp-0.1.2.tar", max compression
```

## Comparing `flspp-0.1.1.tar` & `flspp-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1138 2024-05-21 12:31:18.975042 flspp-0.1.1/LICENSE
--rw-r--r--   0        0        0     3625 2024-05-21 12:31:18.975042 flspp-0.1.1/README.md
--rw-r--r--   0        0        0     1531 2024-05-21 12:31:18.975042 flspp-0.1.1/build.py
--rw-r--r--   0        0        0       50 2024-05-21 12:31:19.291047 flspp-0.1.1/flspp/__init__.py
--rw-r--r--   0        0        0     3606 2024-05-21 12:31:19.291047 flspp-0.1.1/flspp/_core.cpp
--rw-r--r--   0        0        0      918 2024-05-21 12:31:19.291047 flspp-0.1.1/flspp/additional_vector_stuff.h
--rw-r--r--   0        0        0     1654 2024-05-21 12:31:19.291047 flspp-0.1.1/flspp/clustering.cpp
--rw-r--r--   0        0        0     1048 2024-05-21 12:31:19.291047 flspp-0.1.1/flspp/clustering.h
--rw-r--r--   0        0        0    67574 2024-05-21 12:31:19.291047 flspp-0.1.1/flspp/clustering_algorithm.cpp
--rw-r--r--   0        0        0    14038 2024-05-21 12:31:19.291047 flspp-0.1.1/flspp/clustering_algorithm.h
--rw-r--r--   0        0        0     3406 2024-05-21 12:31:19.291047 flspp-0.1.1/flspp/core.py
--rw-r--r--   0        0        0      121 2024-05-21 12:31:19.291047 flspp-0.1.1/flspp/makros.cpp
--rw-r--r--   0        0        0      383 2024-05-21 12:31:19.291047 flspp-0.1.1/flspp/makros.h
--rw-r--r--   0        0        0      583 2024-05-21 12:31:19.291047 flspp-0.1.1/flspp/random_generator.cpp
--rw-r--r--   0        0        0     1320 2024-05-21 12:31:19.291047 flspp-0.1.1/flspp/random_generator.h
--rw-r--r--   0        0        0      775 2024-05-21 12:31:19.291047 flspp-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     4383 1970-01-01 00:00:00.000000 flspp-0.1.1/setup.py
--rw-r--r--   0        0        0     4146 1970-01-01 00:00:00.000000 flspp-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1138 2024-05-23 10:33:25.787048 flspp-0.1.2/LICENSE
+-rw-r--r--   0        0        0     3625 2024-05-23 10:33:25.791048 flspp-0.1.2/README.md
+-rw-r--r--   0        0        0     1531 2024-05-23 10:33:25.791048 flspp-0.1.2/build.py
+-rw-r--r--   0        0        0       50 2024-05-23 10:33:26.103047 flspp-0.1.2/flspp/__init__.py
+-rw-r--r--   0        0        0     3615 2024-05-23 10:33:26.103047 flspp-0.1.2/flspp/_core.cpp
+-rw-r--r--   0        0        0      918 2024-05-23 10:33:26.103047 flspp-0.1.2/flspp/additional_vector_stuff.h
+-rw-r--r--   0        0        0     1654 2024-05-23 10:33:26.103047 flspp-0.1.2/flspp/clustering.cpp
+-rw-r--r--   0        0        0     1048 2024-05-23 10:33:26.103047 flspp-0.1.2/flspp/clustering.h
+-rw-r--r--   0        0        0    67574 2024-05-23 10:33:26.103047 flspp-0.1.2/flspp/clustering_algorithm.cpp
+-rw-r--r--   0        0        0    14038 2024-05-23 10:33:26.103047 flspp-0.1.2/flspp/clustering_algorithm.h
+-rw-r--r--   0        0        0     3385 2024-05-23 10:33:26.103047 flspp-0.1.2/flspp/core.py
+-rw-r--r--   0        0        0      121 2024-05-23 10:33:26.103047 flspp-0.1.2/flspp/makros.cpp
+-rw-r--r--   0        0        0      383 2024-05-23 10:33:26.103047 flspp-0.1.2/flspp/makros.h
+-rw-r--r--   0        0        0      583 2024-05-23 10:33:26.103047 flspp-0.1.2/flspp/random_generator.cpp
+-rw-r--r--   0        0        0     1320 2024-05-23 10:33:26.103047 flspp-0.1.2/flspp/random_generator.h
+-rw-r--r--   0        0        0      775 2024-05-23 10:33:26.107047 flspp-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     4383 1970-01-01 00:00:00.000000 flspp-0.1.2/setup.py
+-rw-r--r--   0        0        0     4146 1970-01-01 00:00:00.000000 flspp-0.1.2/PKG-INFO
```

### Comparing `flspp-0.1.1/LICENSE` & `flspp-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `flspp-0.1.1/README.md` & `flspp-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `flspp-0.1.1/build.py` & `flspp-0.1.2/build.py`

 * *Files identical despite different names*

### Comparing `flspp-0.1.1/flspp/_core.cpp` & `flspp-0.1.2/flspp/_core.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 #include <Python.h>
 
 #include "random_generator.h"
 #include "clustering_algorithm.h"
 #include "additional_vector_stuff.h"
 #include "makros.h"
 
-std::vector<Point> array_to_vector(double **array, int rows, int columns)
+std::vector<Point> array_to_vector(double *array, int rows, int columns)
 {
 
     std::vector<Point> points;
 
     for (int i = 0; i < rows; ++i)
     {
         std::vector<double> row;
         for (int j = 0; j < columns; ++j)
         {
-            row.push_back(array[i][j]);
+            row.push_back(array[i * columns + j]);
         }
         Point p = Point(columns, i, row);
         points.push_back(p);
     }
 
     return points;
 }
@@ -35,15 +35,15 @@
 // (https://stackoverflow.com/a/22288874/1509433). The _WIN32 macro covers the Visual
 // Studio compiler (MSVC) and MinGW. The __CYGWIN__ macro covers gcc and clang under
 // Cygwin.
 #if defined(_WIN32) || defined(__CYGWIN__)
     __declspec(dllexport)
 #endif
     double
-    cluster(double **array,
+    cluster(double *array,
             uint n,
             uint d,
             uint k,
             uint lloyd_iterations,
             uint local_search_iterations,
             std::uint64_t seed,
             int *labels,
```

### Comparing `flspp-0.1.1/flspp/additional_vector_stuff.h` & `flspp-0.1.2/flspp/additional_vector_stuff.h`

 * *Files identical despite different names*

### Comparing `flspp-0.1.1/flspp/clustering.cpp` & `flspp-0.1.2/flspp/clustering.cpp`

 * *Files identical despite different names*

### Comparing `flspp-0.1.1/flspp/clustering.h` & `flspp-0.1.2/flspp/clustering.h`

 * *Files identical despite different names*

### Comparing `flspp-0.1.1/flspp/clustering_algorithm.cpp` & `flspp-0.1.2/flspp/clustering_algorithm.cpp`

 * *Files identical despite different names*

### Comparing `flspp-0.1.1/flspp/clustering_algorithm.h` & `flspp-0.1.2/flspp/clustering_algorithm.h`

 * *Files identical despite different names*

### Comparing `flspp-0.1.1/flspp/core.py` & `flspp-0.1.2/flspp/core.py`

 * *Files 10% similar despite different names*

```diff
@@ -41,37 +41,38 @@
         X: Sequence[Sequence[float]],
         y: Any = None,
         sample_weight: Optional[Sequence[float]] = None,
     ) -> "FLSpp":
         if sample_weight is not None:
             raise NotImplementedError("Sample weights are not yet supported.")
 
-        X = self._validate_data(
+        _X = self._validate_data(
             X,
             accept_sparse="csr",
             dtype=[np.float64, np.float32],
             order="C",
             accept_large_sparse=False,
         )
 
         sample_weight = _check_sample_weight(sample_weight, X, dtype=type(X))
         self._n_threads = _openmp_effective_n_threads()
 
-        n_samples = len(X)
-        self.n_features_in_ = len(X[0])
+        n_samples = _X.shape[0]
+        self.n_features_in_ = _X.shape[1]
 
         if n_samples < self.n_clusters:
             raise ValueError(
                 f"n_samples={n_samples} should be >= n_clusters={self.n_clusters}."
             )
 
+        assert isinstance(_X, np.ndarray), type(_X)
+
+        _X = np.ascontiguousarray(_X)
         # Declare c types
-        c_array = (ctypes.POINTER(ctypes.c_double) * n_samples)()
-        for i in range(n_samples):
-            c_array[i] = (ctypes.c_double * self.n_features_in_)(*X[i])  # type: ignore
+        c_array = _X.ctypes.data_as(ctypes.POINTER(ctypes.c_double))
         c_n = ctypes.c_uint(n_samples)
         c_d = ctypes.c_uint(self.n_features_in_)
         c_k = ctypes.c_uint(self.n_clusters)
         c_ll_iterations = ctypes.c_uint(self.lloyd_iterations)
         c_ls_iterations = ctypes.c_uint(self.local_search_iterations)
         c_random_state = ctypes.c_size_t(self.random_state)
         c_labels = (ctypes.c_int * n_samples)()
```

### Comparing `flspp-0.1.1/flspp/random_generator.cpp` & `flspp-0.1.2/flspp/random_generator.cpp`

 * *Files identical despite different names*

### Comparing `flspp-0.1.1/flspp/random_generator.h` & `flspp-0.1.2/flspp/random_generator.h`

 * *Files identical despite different names*

### Comparing `flspp-0.1.1/pyproject.toml` & `flspp-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flspp"
-version = "0.1.1"
+version = "0.1.2"
 description = ""
 authors = ["Lukas Drexler <lukas.drexler@hhu.de>", "Giulia Baldini <giulia.baldini@hhu.de>"]
 readme = "README.md"
 packages = [
     { include = "flspp" }
 ]
```

### Comparing `flspp-0.1.1/setup.py` & `flspp-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['numpy>=1.26.4,<2.0.0', 'scikit-learn>=1.4.2,<2.0.0']
 
 setup_kwargs = {
     'name': 'flspp',
-    'version': '0.1.1',
+    'version': '0.1.2',
     'description': '',
     'long_description': '[![Build Status](https://github.com/algo-hhu/FLSpp/actions/workflows/mypy-flake-test.yml/badge.svg)](https://github.com/algo-hhu/FLSpp/actions)\n[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)\n[![Supported Python version](https://img.shields.io/badge/python-3.9+-blue.svg)](https://www.python.org/downloads/release/python-390/)\n[![Stable Version](https://img.shields.io/pypi/v/flspp?label=stable)](https://pypi.org/project/flspp/)\n\n# FLS++\n\nAn implementation of the FLS++ algorithm for k-means Clustering, as presented in [1]. This is an improvement of the LS++ algorithm presented by Lattanzi and Sohler in [2].\n\nOne can think of the algorithm as working in 3 phases:\n\n1. Initializing centers with k-means++ (as presented in [3]).\n2. Improving the center set by performing local search swaps (for details, see [1]).\n3. Converging the solution with LLoyd\'s algorithm (also known as "the" k-means algorithm).\n\nIn [2] it is shown that `O(k log log k)` local search iterations yield a constant factor approximation. However, in both [1] and [2] it is shown that, in practice, a very small number of iterations (e.g. 20) already yields very good results, at very reasonable runtime.\n\nThe interface is built in the same way as scikit-learn\'s KMeans for better compatibility.\n\nIn the following plots, we compare the performance of FLS++ (GFLS++) with various local search steps (5, 10, 15) with k-means++ (kM++), greedy k-means++ (GkM++) and the local search algorithm [2] with 25 local search steps (GLS++). The results are computed for the [KDD Phy Test](https://www.kdd.org/kdd-cup/view/kdd-cup-2004/data) and the [Tower](https://www.worldscientific.com/doi/abs/10.1142/S0218195908002787) datasets and averaged over 50 runs.\n\n![Boxplot Comparison for FLS++](https://github.com/algo-hhu/FLSpp/blob/main/images/boxplots.png)\n\n## References\n\n[1] Theo Conrads, Lukas Drexler, Joshua Könen, Daniel R. Schmidt and Melanie Schmidt. "Local Search k-means++ with Foresight" (2024)\n\n[2] Silvio Lattanzi and Christian Sohler. A better k-means++ algorithm via local search. In Proc.444\nof the 36th ICML, volume 97 of Proceedings of Machine Learning Research, pages 3662–3671.445\nPMLR, 09–15 Jun 2019\n\n[3] David Arthur and Sergei Vassilvitskii. K-means++: The advantages of careful seeding. In409\nProceedings of the 18th SODA, page 1027–1035, USA, 2007\n\n## Installation\n\n```bash\npip install flspp\n```\n\n## Example\n\n```python\nfrom flspp import FLSpp\n\nexample_data = [\n    [1.0, 1.0, 1.0],\n    [1.1, 1.1, 1.1],\n    [1.2, 1.2, 1.2],\n    [2.0, 2.0, 2.0],\n    [2.1, 2.1, 2.1],\n    [2.2, 2.2, 2.2],\n]\n\nflspp = FLSpp(n_clusters=2)\nlabels = flspp.fit_predict(example_data)\ncenters = flspp.cluster_centers_\n\nprint(labels) # [1, 1, 1, 0, 0, 0]\nprint(centers) # [[2.1, 2.1, 2.1], [1.1, 1.1, 1.1]]\n```\n\n## Development\n\nInstall [poetry](https://python-poetry.org/docs/#installation)\n```bash\ncurl -sSL https://install.python-poetry.org | python3 -\n```\n\nInstall clang\n```bash\nsudo apt-get install clang\n```\n\nSet clang variables\n```bash\nexport CXX=/usr/bin/clang++\nexport CC=/usr/bin/clang\n```\n\nInstall the package\n```bash\npoetry install\n```\n\nIf the installation does not work and you do not see the C++ output, you can build the package to see the stack trace\n```bash\npoetry build\n```\n\nRun the tests\n```bash\npoetry run python -m unittest discover tests -v\n```\n\n## Citation\n\nIf you use this code, please cite the following paper:\n\n```\nTheo Conrads, Lukas Drexler, Joshua Könen, Daniel R. Schmidt and Melanie Schmidt. "Local Search k-means++ with Foresight" (2024). Accepted at SEA 2024.\n```\n',
     'author': 'Lukas Drexler',
     'author_email': 'lukas.drexler@hhu.de',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `flspp-0.1.1/PKG-INFO` & `flspp-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flspp
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: Lukas Drexler
 Author-email: lukas.drexler@hhu.de
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

