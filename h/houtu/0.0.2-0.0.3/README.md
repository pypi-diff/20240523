# Comparing `tmp/houtu-0.0.2.tar.gz` & `tmp/houtu-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "houtu-0.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "houtu-0.0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `houtu-0.0.2.tar` & `houtu-0.0.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1075 2023-06-15 13:50:34.614586 houtu-0.0.2/LICENSE
--rw-r--r--   0        0        0      183 2023-06-15 13:50:34.614586 houtu-0.0.2/houtu/__init__.py
--rw-r--r--   0        0        0  6170036 2023-06-15 13:50:34.622586 houtu-0.0.2/houtu/data/cities1000.txt.xz
--rw-r--r--   0        0        0    15063 2023-06-15 13:50:34.626586 houtu-0.0.2/houtu/geocoding.py
--rw-r--r--   0        0        0      402 2023-06-15 13:50:34.626586 houtu-0.0.2/houtu/utils.py
--rw-r--r--   0        0        0     1312 2023-06-15 13:50:34.626586 houtu-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     3264 2023-06-15 13:50:34.626586 houtu-0.0.2/readme.md
--rw-r--r--   0        0        0     4283 1970-01-01 00:00:00.000000 houtu-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1075 2024-05-23 17:11:39.470348 houtu-0.0.3/LICENSE
+-rw-r--r--   0        0        0      181 2024-05-23 17:11:39.470348 houtu-0.0.3/houtu/__init__.py
+-rw-r--r--   0        0        0  6170036 2024-05-23 17:11:39.474348 houtu-0.0.3/houtu/data/cities1000.txt.xz
+-rw-r--r--   0        0        0    19396 2024-05-23 17:11:39.474348 houtu-0.0.3/houtu/geocoding.py
+-rw-r--r--   0        0        0     2613 2024-05-23 17:11:39.474348 houtu-0.0.3/houtu/utils.py
+-rw-r--r--   0        0        0     1476 2024-05-23 17:11:39.474348 houtu-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3268 2024-05-23 17:11:39.474348 houtu-0.0.3/readme.md
+-rw-r--r--   0        0        0     4460 1970-01-01 00:00:00.000000 houtu-0.0.3/PKG-INFO
```

### Comparing `houtu-0.0.2/LICENSE` & `houtu-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `houtu-0.0.2/houtu/data/cities1000.txt.xz` & `houtu-0.0.3/houtu/data/cities1000.txt.xz`

 * *Files identical despite different names*

### Comparing `houtu-0.0.2/houtu/geocoding.py` & `houtu-0.0.3/houtu/geocoding.py`

 * *Files 12% similar despite different names*

```diff
@@ -113,23 +113,21 @@
         huE = np.hypot(u, E)
 
         # eqn. 4b
         try:
             Beta = np.arctan(huE / u * z / np.hypot(x, y))
         except ZeroDivisionError:
             raise
-            if z >= 0:
+            if z >= 0:  # type: ignore[unreachable]
                 Beta = np.pi / 2
             else:
                 Beta = -np.pi / 2
 
         # eqn. 13
-        eps = ((cls.B * u - cls.A * huE + E**2) * np.sin(Beta)) / (
-            cls.A * huE * 1 / np.cos(Beta) - E**2 * np.cos(Beta)
-        )
+        eps = ((cls.B * u - cls.A * huE + E**2) * np.sin(Beta)) / (cls.A * huE * 1 / np.cos(Beta) - E**2 * np.cos(Beta))
 
         Beta += eps
 
         lat = np.arctan(cls.A / cls.B * np.tan(Beta))
         lon = np.arctan2(y, x)
 
         # eqn. 7
@@ -142,16 +140,15 @@
         assert lat.shape == lon.shape == alt.shape
         return np.stack([lat, lon, alt], axis=-1)
 
 
 def toint(s: str) -> Optional[int]:
     if s:
         return int(s)
-    else:
-        return None
+    return None
 
 
 def get_data(path: str, keep_dups: bool = False) -> Cities:
     """Read data from tsv file. Expect the following columns:
 
     cols = ("geonameid", "name", "asciiname", "alternatenames", "latitude", "longitude", "feature class",
         "feature code", "country code", "cc2", "admin1 code", "admin2", "admin3", "admin4", "population",
@@ -229,37 +226,55 @@
 def _select_cities(cities: List[City], indices: np.ndarray) -> List[List[City]]:
     out = []
     for i in range(indices.shape[0]):
         out.append([cities[idx] for idx in indices[i]])
     return out
 
 
-class ReverseGeocodeKdScipy:
+class ReverseGeocodeBase:
+    cities: List[City]
+
+    def __init__(self, path: Optional[str] = None) -> None:
+        pass
+
+    @overload
+    def query(
+        self, query_arr: np.ndarray, k: int, form: str, return_distance: Literal[True]
+    ) -> Tuple[np.ndarray, np.ndarray, List[List[City]]]: ...
+
+    @overload
+    def query(
+        self, query_arr: np.ndarray, k: int, form: str, return_distance: Literal[False]
+    ) -> Tuple[np.ndarray, List[List[City]]]: ...
+
+    def query(self, query_arr, k=2, form="radians", return_distance=True):
+        raise NotImplementedError
+
+
+class ReverseGeocodeKdScipy(ReverseGeocodeBase):
     def __init__(self, path: Optional[str] = None) -> None:
         from scipy.spatial import KDTree
 
         if path is None:
             path = files(__package__).joinpath("data/cities1000.txt.xz")
 
         arr, self.cities = get_data(path)
         arr = WGS84.geodetic2ecef(arr)
         assert arr.dtype == np.float32
         self.tree = KDTree(arr)
 
     @overload
     def query(
         self, query_arr: np.ndarray, k: int, form: str, return_distance: Literal[True]
-    ) -> Tuple[np.ndarray, np.ndarray, List[List[City]]]:
-        ...
+    ) -> Tuple[np.ndarray, np.ndarray, List[List[City]]]: ...
 
     @overload
     def query(
         self, query_arr: np.ndarray, k: int, form: str, return_distance: Literal[False]
-    ) -> Tuple[np.ndarray, List[List[City]]]:
-        ...
+    ) -> Tuple[np.ndarray, List[List[City]]]: ...
 
     def query(self, query_arr, k=2, form="radians", return_distance=True):
         query_arr = _check_input(query_arr, k, form, "ecef")
 
         distances, indices = self.tree.query(query_arr, k)
         if k == 1:
             distances = distances[..., None]
@@ -272,15 +287,122 @@
 
         if return_distance:
             return coords, distances, cities
         else:
             return coords, cities
 
 
-class ReverseGeocodeKdLearn:
+class ReverseGeocodeVpTreePython(ReverseGeocodeBase):
+    """https://github.com/RickardSjogren/vptree"""
+
+    @staticmethod
+    def _euclidean(p1, p2):
+        diff = p2[1] - p1[1]
+        return np.sqrt(np.sum(diff * diff, axis=-1))
+
+    def __init__(self, path: Optional[str] = None) -> None:
+        from vptree import VPTree
+
+        if path is None:
+            path = files(__package__).joinpath("data/cities1000.txt.xz")
+
+        arr, self.cities = get_data(path)
+        arr = WGS84.geodetic2ecef(arr)
+        assert arr.dtype == np.float32
+        arr_with_index = [(i, v) for i, v in zip(range(len(arr)), arr)]
+        try:
+            self.tree = VPTree(arr_with_index, self._euclidean)
+        except ValueError as e:
+            if str(e).startswith("setting an array element with a sequence"):
+                raise ImportError("vptree version is too old. currently git master branch is required")
+
+    @overload
+    def query(
+        self, query_arr: np.ndarray, k: int, form: str, return_distance: Literal[True]
+    ) -> Tuple[np.ndarray, np.ndarray, List[List[City]]]: ...
+
+    @overload
+    def query(
+        self, query_arr: np.ndarray, k: int, form: str, return_distance: Literal[False]
+    ) -> Tuple[np.ndarray, List[List[City]]]: ...
+
+    def query(self, query_arr, k=2, form="radians", return_distance=True):
+        query_arr = _check_input(query_arr, k, form, "ecef")
+
+        indices = []
+        coords = []
+        distances = []
+
+        for query in query_arr:
+            query = (0, query)
+            neighbors = self.tree.get_n_nearest_neighbors(query, k)
+            _distances, pairs = zip(*neighbors)
+            _indices, _coords = zip(*pairs)
+            indices.append(_indices)
+            coords.append(_coords)
+            distances.append(_distances)
+
+        indices = np.array(indices, dtype=np.int64)
+        coords = np.array(coords, dtype=np.float32)
+        distances = np.array(distances, dtype=np.float32)
+        cities = _select_cities(self.cities, indices)
+
+        coords = WGS84.ecef2geodetic(coords)
+        coords = coords[..., :2]  # ignore altitude
+
+        if return_distance:
+            return coords, distances, cities
+        else:
+            return coords, cities
+
+
+class ReverseGeocodeVpTreeSimd(ReverseGeocodeBase):
+    """https://github.com/pablocael/pynear"""
+
+    def __init__(self, path: Optional[str] = None) -> None:
+        from pynear import VPTreeL2Index
+
+        if path is None:
+            path = files(__package__).joinpath("data/cities1000.txt.xz")
+
+        arr, self.cities = get_data(path)
+        self.arr = WGS84.geodetic2ecef(arr)
+        assert arr.dtype == np.float32
+        self.tree = VPTreeL2Index()
+        self.tree.set(self.arr)
+
+    @overload
+    def query(
+        self, query_arr: np.ndarray, k: int, form: str, return_distance: Literal[True]
+    ) -> Tuple[np.ndarray, np.ndarray, List[List[City]]]: ...
+
+    @overload
+    def query(
+        self, query_arr: np.ndarray, k: int, form: str, return_distance: Literal[False]
+    ) -> Tuple[np.ndarray, List[List[City]]]: ...
+
+    def query(self, query_arr, k=2, form="radians", return_distance=True):
+        query_arr = _check_input(query_arr, k, form, "ecef")
+
+        indices, distances = self.tree.searchKNN(query_arr, k)
+        indices = np.array(indices, dtype=np.int64)[:, ::-1]
+        distances = np.array(distances, dtype=np.float32)[:, ::-1]
+        cities = _select_cities(self.cities, indices)
+
+        coords = self.arr[indices]
+        coords = WGS84.ecef2geodetic(coords)
+        coords = coords[..., :2]  # ignore altitude
+
+        if return_distance:
+            return coords, distances, cities
+        else:
+            return coords, cities
+
+
+class ReverseGeocodeKdLearn(ReverseGeocodeBase):
     def __init__(self, path: Optional[str] = None) -> None:
         from sklearn.neighbors import KDTree
 
         if path is None:
             path = files(__package__).joinpath("data/cities1000.txt.xz")
 
         arr, self.cities = get_data(path)
@@ -288,22 +410,20 @@
         assert arr.dtype == np.float32
         self.tree = KDTree(arr)  # copy is made here since input is float32 and float64 is needed
         # assert self.tree.data.base is arr
 
     @overload
     def query(
         self, query_arr: np.ndarray, k: int, form: str, return_distance: Literal[True]
-    ) -> Tuple[np.ndarray, np.ndarray, List[List[City]]]:
-        ...
+    ) -> Tuple[np.ndarray, np.ndarray, List[List[City]]]: ...
 
     @overload
     def query(
         self, query_arr: np.ndarray, k: int, form: str, return_distance: Literal[False]
-    ) -> Tuple[np.ndarray, List[List[City]]]:
-        ...
+    ) -> Tuple[np.ndarray, List[List[City]]]: ...
 
     def query(self, query_arr, k=2, form="radians", return_distance=True):
         query_arr = _check_input(query_arr, k, form, "ecef")
 
         if return_distance:
             distances, indices = self.tree.query(query_arr, k, return_distance)
         else:
@@ -320,33 +440,31 @@
 
         if return_distance:
             return coords, distances, cities
         else:
             return coords, cities
 
 
-class ReverseGeocodeBruteEuclidic:
+class ReverseGeocodeBruteEuclidic(ReverseGeocodeBase):
     def __init__(self, path: Optional[str] = None) -> None:
         if path is None:
             path = files(__package__).joinpath("data/cities1000.txt.xz")
 
         arr, self.cities = get_data(path)
         self.arr = WGS84.geodetic2ecef(arr)
 
     @overload
     def query(
         self, query_arr: np.ndarray, k: int, form: str, return_distance: Literal[True]
-    ) -> Tuple[np.ndarray, np.ndarray, List[List[City]]]:
-        ...
+    ) -> Tuple[np.ndarray, np.ndarray, List[List[City]]]: ...
 
     @overload
     def query(
         self, query_arr: np.ndarray, k: int, form: str, return_distance: Literal[False]
-    ) -> Tuple[np.ndarray, List[List[City]]]:
-        ...
+    ) -> Tuple[np.ndarray, List[List[City]]]: ...
 
     def query(self, query_arr, k=2, form="radians", return_distance=True):
         query_arr = _check_input(query_arr, k, form, "ecef")
 
         distances = euclidean_distances(query_arr, self.arr, squared=True)
 
         indices = np.argpartition(distances, range(k), axis=-1)[:, :k]
@@ -361,34 +479,32 @@
 
         if return_distance:
             return coords, distances, cities
         else:
             return coords, cities
 
 
-class ReverseGeocodeBruteHaversine:
+class ReverseGeocodeBruteHaversine(ReverseGeocodeBase):
     radius = earth_radii["Spherical Earth Approx. of Radius (RE)"]  # see opt_geocoding.py
 
     def __init__(self, path: Optional[str] = None) -> None:
         if path is None:
             path = files(__package__).joinpath("data/cities1000.txt.xz")
 
         self.arr, self.cities = get_data(path)
 
     @overload
     def query(
         self, query_arr: np.ndarray, k: int, form: str, return_distance: Literal[True]
-    ) -> Tuple[np.ndarray, np.ndarray, List[List[City]]]:
-        ...
+    ) -> Tuple[np.ndarray, np.ndarray, List[List[City]]]: ...
 
     @overload
     def query(
         self, query_arr: np.ndarray, k: int, form: str, return_distance: Literal[False]
-    ) -> Tuple[np.ndarray, List[List[City]]]:
-        ...
+    ) -> Tuple[np.ndarray, List[List[City]]]: ...
 
     def query(self, query_arr, k=2, form="radians", return_distance=True):
         query_arr = _check_input(query_arr, k, form, "radians")
 
         distances = haversine_distances(query_arr, self.arr)
         indices = np.argpartition(distances, range(k), axis=-1)[:, :k]
         cities = _select_cities(self.cities, indices)
@@ -400,37 +516,35 @@
 
         if return_distance:
             return coords, distances, cities
         else:
             return coords, cities
 
 
-class ReverseGeocodeBallHaversine:
+class ReverseGeocodeBallHaversine(ReverseGeocodeBase):
     radius = earth_radii["Spherical Earth Approx. of Radius (RE)"]  # see opt_geocoding.py
 
     def __init__(self, path: Optional[str] = None) -> None:
         from sklearn.neighbors import BallTree
 
         if path is None:
             path = files(__package__).joinpath("data/cities1000.txt.xz")
 
         arr, self.cities = get_data(path)
         self.bt = BallTree(arr, metric="haversine")
 
     @overload
     def query(
         self, query_arr: np.ndarray, k: int, form: str, return_distance: Literal[True]
-    ) -> Tuple[np.ndarray, np.ndarray, List[List[City]]]:
-        ...
+    ) -> Tuple[np.ndarray, np.ndarray, List[List[City]]]: ...
 
     @overload
     def query(
         self, query_arr: np.ndarray, k: int, form: str, return_distance: Literal[False]
-    ) -> Tuple[np.ndarray, List[List[City]]]:
-        ...
+    ) -> Tuple[np.ndarray, List[List[City]]]: ...
 
     def query(self, query_arr, k=2, form="radians", return_distance=True):
         query_arr = _check_input(query_arr, k, form, "radians")
 
         if return_distance:
             distances, indices = self.bt.query(query_arr, k, return_distance)
         else:
@@ -445,14 +559,14 @@
         coords = coords[indices]
 
         if return_distance:
             return coords, distances, cities
         else:
             return coords, cities
 
-    def lat_lon(self, lat: float, lon: float) -> Tuple[List[float], float, City]:
+    def lat_lon(self, lat: float, lon: float, form: str) -> Tuple[List[float], float, City]:
         query_arr = np.array([[lat, lon]], dtype=np.float32)
-        coords, distances, cities = self.query(query_arr, k=1)
+        coords, distances, cities = self.query(query_arr, 1, form, True)
         return coords[0, 0].tolist(), distances[0, 0], cities[0][0]
 
 
 ReverseGeocode = ReverseGeocodeBallHaversine
```

### Comparing `houtu-0.0.2/pyproject.toml` & `houtu-0.0.3/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,53 +1,61 @@
 [build-system]
 build-backend = "flit_core.buildapi"
 requires = [
-  "flit_core<4,>=3.2",
+  "flit-core<4,>=3.2",
 ]
 
 [project]
 name = "houtu"
-readme = {file = "readme.md", content-type = "text/markdown"}
-license = {file = "LICENSE"}
-authors = [{name = "Dobatymo", email = "dobatymo@users.noreply.github.com"}]
+readme = { file = "readme.md", content-type = "text/markdown" }
+license = { file = "LICENSE" }
+authors = [
+  { name = "Dobatymo", email = "dobatymo@users.noreply.github.com" },
+]
 requires-python = ">=3.8"
 classifiers = [
   "Intended Audience :: Developers",
   "License :: OSI Approved :: MIT License",
   "Programming Language :: Python :: 3 :: Only",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3.12",
   "Topic :: Scientific/Engineering :: GIS",
 ]
 dynamic = [
   "description",
   "version",
 ]
 dependencies = [
   "importlib-resources",
   "numpy",
   "scikit-learn",
   "scipy>=1.6",
 ]
-[project.optional-dependencies]
-optimize = [
+optional-dependencies.optimize = [
   "geopy",
   "pymap3d",
 ]
-test = [
+optional-dependencies.optional = [
+  "pynear>=0.1",
+  "vptree>=1.3",
+]
+optional-dependencies.test = [
   "genutility[cache]",
 ]
-[project.urls]
-Home = "https://github.com/Dobatymo/houtu"
+urls.Home = "https://github.com/Dobatymo/houtu"
 
 [tool.black]
 line-length = 120
 
+[tool.ruff]
+line-length = 120
+
 [tool.isort]
 profile = "black"
 line_length = 120
 
 [tool.mypy]
 allow_redefinition = true
 ignore_missing_imports = true
@@ -55,8 +63,10 @@
 warn_redundant_casts = true
 warn_unused_configs = true
 warn_unused_ignores = true
 warn_unreachable = true
 strict_equality = true
 
 [tool.bandit]
-skips = ["B101"]
+skips = [
+  "B101",
+]
```

### Comparing `houtu-0.0.2/readme.md` & `houtu-0.0.3/readme.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # houtu
 
-Offline fast reverse geocoding. Named after the Chinese Goddess of the Earth Houtu.
+Offline fast reverse geocoding. Named after the Chinese Goddess of the Earth *Houtu*.
 
 Various implementations are included.
 - Naive computation of haversine distance matrix. Coordinates are not converted.
 - Using ball-tree with haversine metric. Coordinates are not converted.
-- Naive computation of euclidic distance matrix. Coordinates are converted from geodetic to ECEF and back.
-- Using kd-tree with euclidic metric. Coordinates are converted from geodetic to ECEF and back.
+- Naive computation of Euclidean distance matrix. Coordinates are converted from geodetic to ECEF and back.
+- Using kd-tree with Euclidean metric. Coordinates are converted from geodetic to ECEF and back.
 
 ## Install
 
 - requires Python 3.8+
 - run `pip install houtu`
 
 ## Use
```

### Comparing `houtu-0.0.2/PKG-INFO` & `houtu-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,42 +1,46 @@
 Metadata-Version: 2.1
 Name: houtu
-Version: 0.0.2
-Summary: Offline fast reverse geocoding. Named after the Chinese Goddess of the Earth Houtu. 
+Version: 0.0.3
+Summary: Offline fast reverse geocoding. Named after the Chinese Goddess of the Earth Houtu.
 Author-email: Dobatymo <dobatymo@users.noreply.github.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: GIS
 Requires-Dist: importlib-resources
 Requires-Dist: numpy
 Requires-Dist: scikit-learn
 Requires-Dist: scipy>=1.6
 Requires-Dist: geopy ; extra == "optimize"
 Requires-Dist: pymap3d ; extra == "optimize"
+Requires-Dist: pynear>=0.1 ; extra == "optional"
+Requires-Dist: vptree>=1.3 ; extra == "optional"
 Requires-Dist: genutility[cache] ; extra == "test"
 Project-URL: Home, https://github.com/Dobatymo/houtu
 Provides-Extra: optimize
+Provides-Extra: optional
 Provides-Extra: test
 
 # houtu
 
-Offline fast reverse geocoding. Named after the Chinese Goddess of the Earth Houtu.
+Offline fast reverse geocoding. Named after the Chinese Goddess of the Earth *Houtu*.
 
 Various implementations are included.
 - Naive computation of haversine distance matrix. Coordinates are not converted.
 - Using ball-tree with haversine metric. Coordinates are not converted.
-- Naive computation of euclidic distance matrix. Coordinates are converted from geodetic to ECEF and back.
-- Using kd-tree with euclidic metric. Coordinates are converted from geodetic to ECEF and back.
+- Naive computation of Euclidean distance matrix. Coordinates are converted from geodetic to ECEF and back.
+- Using kd-tree with Euclidean metric. Coordinates are converted from geodetic to ECEF and back.
 
 ## Install
 
 - requires Python 3.8+
 - run `pip install houtu`
 
 ## Use
```

