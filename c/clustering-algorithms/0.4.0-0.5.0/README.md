# Comparing `tmp/clustering_algorithms-0.4.0.tar.gz` & `tmp/clustering_algorithms-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clustering_algorithms-0.4.0.tar", last modified: Thu May 16 11:38:38 2024, max compression
+gzip compressed data, was "clustering_algorithms-0.5.0.tar", last modified: Thu May 23 14:47:51 2024, max compression
```

## Comparing `clustering_algorithms-0.4.0.tar` & `clustering_algorithms-0.5.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 user       (502) staff       (20)        0 2024-05-16 11:38:38.544840 clustering_algorithms-0.4.0/
--rw-r--r--   0 user       (502) staff       (20)      595 2024-05-16 11:38:38.544611 clustering_algorithms-0.4.0/PKG-INFO
--rw-r--r--   0 user       (502) staff       (20)      104 2024-03-23 14:37:19.000000 clustering_algorithms-0.4.0/README.md
-drwxr-xr-x   0 user       (502) staff       (20)        0 2024-05-16 11:38:38.543207 clustering_algorithms-0.4.0/clustering_algorithms/
--rw-r--r--   0 user       (502) staff       (20)        0 2024-03-22 15:22:00.000000 clustering_algorithms-0.4.0/clustering_algorithms/__init__.py
--rw-r--r--   0 user       (502) staff       (20)     2377 2024-05-16 11:34:57.000000 clustering_algorithms-0.4.0/clustering_algorithms/c_means.py
--rw-r--r--   0 user       (502) staff       (20)     2289 2024-05-14 16:43:11.000000 clustering_algorithms-0.4.0/clustering_algorithms/clustering_algorithm.py
--rw-r--r--   0 user       (502) staff       (20)      219 2024-05-15 16:21:29.000000 clustering_algorithms-0.4.0/clustering_algorithms/clustering_exception.py
--rw-r--r--   0 user       (502) staff       (20)     2706 2024-05-16 11:34:57.000000 clustering_algorithms-0.4.0/clustering_algorithms/k_means.py
-drwxr-xr-x   0 user       (502) staff       (20)        0 2024-05-16 11:38:38.544399 clustering_algorithms-0.4.0/clustering_algorithms.egg-info/
--rw-r--r--   0 user       (502) staff       (20)      595 2024-05-16 11:38:38.000000 clustering_algorithms-0.4.0/clustering_algorithms.egg-info/PKG-INFO
--rw-r--r--   0 user       (502) staff       (20)      497 2024-05-16 11:38:38.000000 clustering_algorithms-0.4.0/clustering_algorithms.egg-info/SOURCES.txt
--rw-r--r--   0 user       (502) staff       (20)        1 2024-05-16 11:38:38.000000 clustering_algorithms-0.4.0/clustering_algorithms.egg-info/dependency_links.txt
--rw-r--r--   0 user       (502) staff       (20)        6 2024-05-16 11:38:38.000000 clustering_algorithms-0.4.0/clustering_algorithms.egg-info/requires.txt
--rw-r--r--   0 user       (502) staff       (20)       22 2024-05-16 11:38:38.000000 clustering_algorithms-0.4.0/clustering_algorithms.egg-info/top_level.txt
--rw-r--r--   0 user       (502) staff       (20)      632 2024-05-16 11:38:08.000000 clustering_algorithms-0.4.0/pyproject.toml
--rw-r--r--   0 user       (502) staff       (20)       38 2024-05-16 11:38:38.544890 clustering_algorithms-0.4.0/setup.cfg
-drwxr-xr-x   0 user       (502) staff       (20)        0 2024-05-16 11:38:38.544220 clustering_algorithms-0.4.0/tests/
--rw-r--r--   0 user       (502) staff       (20)      338 2024-05-02 08:21:08.000000 clustering_algorithms-0.4.0/tests/test_clustering_algorithm.py
--rw-r--r--   0 user       (502) staff       (20)     2056 2024-05-16 11:34:41.000000 clustering_algorithms-0.4.0/tests/test_k_means.py
+drwxr-xr-x   0 user       (502) staff       (20)        0 2024-05-23 14:47:51.731981 clustering_algorithms-0.5.0/
+-rw-r--r--   0 user       (502) staff       (20)     1067 2024-05-23 09:19:17.000000 clustering_algorithms-0.5.0/LICENSE.txt
+-rw-r--r--   0 user       (502) staff       (20)     2458 2024-05-23 14:47:51.731730 clustering_algorithms-0.5.0/PKG-INFO
+-rw-r--r--   0 user       (502) staff       (20)      704 2024-05-23 09:28:37.000000 clustering_algorithms-0.5.0/README.md
+drwxr-xr-x   0 user       (502) staff       (20)        0 2024-05-23 14:47:51.729789 clustering_algorithms-0.5.0/clustering_algorithms/
+-rw-r--r--   0 user       (502) staff       (20)        0 2024-03-22 15:22:00.000000 clustering_algorithms-0.5.0/clustering_algorithms/__init__.py
+-rw-r--r--   0 user       (502) staff       (20)     2369 2024-05-23 11:38:17.000000 clustering_algorithms-0.5.0/clustering_algorithms/c_means.py
+-rw-r--r--   0 user       (502) staff       (20)     2832 2024-05-23 11:57:17.000000 clustering_algorithms-0.5.0/clustering_algorithms/clustering_algorithm.py
+-rw-r--r--   0 user       (502) staff       (20)      209 2024-05-23 14:19:25.000000 clustering_algorithms-0.5.0/clustering_algorithms/clustering_exception.py
+-rw-r--r--   0 user       (502) staff       (20)     2698 2024-05-23 11:38:17.000000 clustering_algorithms-0.5.0/clustering_algorithms/k_means.py
+drwxr-xr-x   0 user       (502) staff       (20)        0 2024-05-23 14:47:51.731422 clustering_algorithms-0.5.0/clustering_algorithms.egg-info/
+-rw-r--r--   0 user       (502) staff       (20)     2458 2024-05-23 14:47:51.000000 clustering_algorithms-0.5.0/clustering_algorithms.egg-info/PKG-INFO
+-rw-r--r--   0 user       (502) staff       (20)      509 2024-05-23 14:47:51.000000 clustering_algorithms-0.5.0/clustering_algorithms.egg-info/SOURCES.txt
+-rw-r--r--   0 user       (502) staff       (20)        1 2024-05-23 14:47:51.000000 clustering_algorithms-0.5.0/clustering_algorithms.egg-info/dependency_links.txt
+-rw-r--r--   0 user       (502) staff       (20)        6 2024-05-23 14:47:51.000000 clustering_algorithms-0.5.0/clustering_algorithms.egg-info/requires.txt
+-rw-r--r--   0 user       (502) staff       (20)       22 2024-05-23 14:47:51.000000 clustering_algorithms-0.5.0/clustering_algorithms.egg-info/top_level.txt
+-rw-r--r--   0 user       (502) staff       (20)      665 2024-05-23 14:46:51.000000 clustering_algorithms-0.5.0/pyproject.toml
+-rw-r--r--   0 user       (502) staff       (20)       38 2024-05-23 14:47:51.732025 clustering_algorithms-0.5.0/setup.cfg
+drwxr-xr-x   0 user       (502) staff       (20)        0 2024-05-23 14:47:51.731205 clustering_algorithms-0.5.0/tests/
+-rw-r--r--   0 user       (502) staff       (20)      338 2024-05-02 08:21:08.000000 clustering_algorithms-0.5.0/tests/test_clustering_algorithm.py
+-rw-r--r--   0 user       (502) staff       (20)     2056 2024-05-16 11:34:41.000000 clustering_algorithms-0.5.0/tests/test_k_means.py
```

### Comparing `clustering_algorithms-0.4.0/clustering_algorithms/c_means.py` & `clustering_algorithms-0.5.0/clustering_algorithms/c_means.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
     def _fit(self, points: NDArray, centroids: NDArray, weights: NDArray) -> Sequence[NDArray]:
         for iteration in range(self.iterations):
             clusters = np.argmax(weights, axis=1)
             self.log_iteration(iteration, centroids, clusters)
             weights = self.predict(points, centroids)
             new_centroids = self.compute_centroids(points, weights)
-            if np.all(new_centroids == centroids):  # type: ignore
+            if self.should_stop(centroids, new_centroids):
                 break
             centroids = new_centroids
         return centroids, clusters, weights
 
     def predict(self, points: NDArray, centroids: NDArray) -> NDArray:
         nn_weights = self.distances(points, centroids) ** (-2 / (self.m - 1))
         return nn_weights / np.sum(nn_weights, axis=1, keepdims=True)
```

### Comparing `clustering_algorithms-0.4.0/clustering_algorithms/clustering_algorithm.py` & `clustering_algorithms-0.5.0/clustering_algorithms/clustering_algorithm.py`

 * *Files 21% similar despite different names*

```diff
@@ -7,21 +7,23 @@
 # mypy: disable-error-code=empty-body
 class ClusteringAlgorithm:
     """
     An abstract clustering algorithm.
     Clustering algorithms produce models that are set of centroids.
     """
 
-    def __init__(self, k: int, iterations: int = 1):
+    def __init__(self, k: int, iterations: int = 1, tolerance: float = 0.0):
         """
         :param k: the number of clusters
         :param iterations: the number of iterations
+        :param tolerance: the maximal distance between generation n-1 and generation n centroids
         """
         self.iterations = iterations
         self.k = k
+        self.tolerance = tolerance
 
     def init(self, points: NDArray, method: str = "random") -> Union[NDArray, Sequence[NDArray]]:
         """
         Inits the model.
         :param points: the training set
         :param method: the init method, defaults to "random"
         :return: a sequence of arrays starting with, at least: a set of centroids
@@ -60,7 +62,16 @@
         """
         This is where you want to do something when an iteration has completed.
         :param iteration: the iteration number
         :param centroids: the computed centroids
         :param clusters: the computed clusters
         """
         pass
+
+    def should_stop(self, centroids: NDArray, new_centroids: NDArray) -> bool:
+        """
+        Returns a boolean indicating if the algorithm should stop.
+        :param centroids: the previous centroids
+        :param new_centroids: the new centroids
+        :return: a boolean
+        """
+        return np.mean(np.linalg.norm(new_centroids - centroids, axis=1)) <= self.tolerance
```

### Comparing `clustering_algorithms-0.4.0/clustering_algorithms/k_means.py` & `clustering_algorithms-0.5.0/clustering_algorithms/k_means.py`

 * *Files 9% similar despite different names*

```diff
@@ -52,14 +52,14 @@
     def _fit(self, points: NDArray, centroids: NDArray) -> Sequence[NDArray]:
         for iteration in range(self.iterations):
             clusters = self.predict(points, centroids)
             if len(np.unique(clusters)) < self.k:
                 raise ClusteringException(TOO_FEW_CLUSTERS)
             self.log_iteration(iteration, centroids, clusters)
             new_centroids = self.compute_centroids(points, clusters)
-            if np.all(new_centroids == centroids):  # type: ignore
+            if self.should_stop(centroids, new_centroids):
                 break
             centroids = new_centroids
         return centroids, clusters
 
     def predict(self, points: NDArray, centroids: NDArray) -> NDArray:
         return np.argmin(self.distances(points, centroids), axis=1)
```

### Comparing `clustering_algorithms-0.4.0/pyproject.toml` & `clustering_algorithms-0.5.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 [project]
 name = "clustering_algorithms"
-version = "0.4.0"
+version = "0.5.0"
 authors = [
   { name="Yan Georget", email="yan.georget@gmail.com" },
 ]
 description = "Clustering algorithms powered by Numpy"
 readme = "README.md"
+license = {file = "LICENSE.txt"}
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "numpy",
```

### Comparing `clustering_algorithms-0.4.0/tests/test_k_means.py` & `clustering_algorithms-0.5.0/tests/test_k_means.py`

 * *Files identical despite different names*

