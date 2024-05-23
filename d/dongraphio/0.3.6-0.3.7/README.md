# Comparing `tmp/dongraphio-0.3.6.tar.gz` & `tmp/dongraphio-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dongraphio-0.3.6.tar", max compression
+gzip compressed data, was "dongraphio-0.3.7.tar", max compression
```

## Comparing `dongraphio-0.3.6.tar` & `dongraphio-0.3.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1498 2024-05-22 18:54:48.578560 dongraphio-0.3.6/LICENSE.txt
--rw-r--r--   0        0        0     1424 2024-05-22 18:59:54.009037 dongraphio-0.3.6/pyproject.toml
--rw-r--r--   0        0        0     1461 2024-05-22 18:54:48.568815 dongraphio-0.3.6/README.md
--rw-r--r--   0        0        0      211 2024-05-22 18:57:11.704747 dongraphio-0.3.6/src/dongraphio/__init__.py
--rw-r--r--   0        0        0      133 2024-05-22 18:54:42.344284 dongraphio-0.3.6/src/dongraphio/base_models/__init__.py
--rw-r--r--   0        0        0    14906 2024-05-22 18:54:42.351343 dongraphio-0.3.6/src/dongraphio/base_models/grapher_logic.py
--rw-r--r--   0        0        0     5390 2024-05-22 19:01:15.437477 dongraphio-0.3.6/src/dongraphio/base_models/isochrones_logic.py
--rw-r--r--   0        0        0     2750 2024-05-22 18:54:42.347119 dongraphio-0.3.6/src/dongraphio/base_models/matrix_logic.py
--rw-r--r--   0        0        0     5628 2024-05-22 18:54:42.363628 dongraphio-0.3.6/src/dongraphio/dongraphio.py
--rw-r--r--   0        0        0     1056 2024-05-22 18:54:42.337542 dongraphio-0.3.6/src/dongraphio/enums.py
--rw-r--r--   0        0        0      466 2024-05-22 18:57:11.710084 dongraphio-0.3.6/src/dongraphio/utils/__init__.py
--rw-r--r--   0        0        0     1262 2024-05-22 18:54:42.333656 dongraphio-0.3.6/src/dongraphio/utils/geometry_utils.py
--rw-r--r--   0        0        0    19283 2024-05-22 18:54:42.325919 dongraphio-0.3.6/src/dongraphio/utils/graph_utils.py
--rw-r--r--   0        0        0     2606 2024-05-22 18:54:42.327912 dongraphio-0.3.6/src/dongraphio/utils/matrix_utils.py
--rw-r--r--   0        0        0     1713 2024-05-22 18:54:42.322735 dongraphio-0.3.6/src/dongraphio/utils/osm_worker.py
--rw-r--r--   0        0        0     1738 2024-05-22 18:54:42.324415 dongraphio-0.3.6/src/dongraphio/utils/tsp_solver.py
--rw-r--r--   0        0        0     2504 1970-01-01 00:00:00.000000 dongraphio-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0     1498 2024-05-23 10:26:37.987404 dongraphio-0.3.7/LICENSE.txt
+-rw-r--r--   0        0        0     1424 2024-05-23 10:26:37.998408 dongraphio-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0     1461 2024-05-23 10:26:37.982852 dongraphio-0.3.7/README.md
+-rw-r--r--   0        0        0      211 2024-05-23 10:26:37.719589 dongraphio-0.3.7/src/dongraphio/__init__.py
+-rw-r--r--   0        0        0      133 2024-05-23 10:26:37.719589 dongraphio-0.3.7/src/dongraphio/base_models/__init__.py
+-rw-r--r--   0        0        0    14870 2024-05-23 10:26:37.735216 dongraphio-0.3.7/src/dongraphio/base_models/grapher_logic.py
+-rw-r--r--   0        0        0     5390 2024-05-23 10:26:37.735216 dongraphio-0.3.7/src/dongraphio/base_models/isochrones_logic.py
+-rw-r--r--   0        0        0     2750 2024-05-23 10:26:37.719589 dongraphio-0.3.7/src/dongraphio/base_models/matrix_logic.py
+-rw-r--r--   0        0        0     5626 2024-05-23 10:26:37.735216 dongraphio-0.3.7/src/dongraphio/dongraphio.py
+-rw-r--r--   0        0        0     1056 2024-05-23 10:26:37.719589 dongraphio-0.3.7/src/dongraphio/enums.py
+-rw-r--r--   0        0        0      466 2024-05-23 10:26:37.703963 dongraphio-0.3.7/src/dongraphio/utils/__init__.py
+-rw-r--r--   0        0        0     1262 2024-05-23 10:26:37.719589 dongraphio-0.3.7/src/dongraphio/utils/geometry_utils.py
+-rw-r--r--   0        0        0    19279 2024-05-23 10:26:37.719589 dongraphio-0.3.7/src/dongraphio/utils/graph_utils.py
+-rw-r--r--   0        0        0     2606 2024-05-23 10:26:37.719589 dongraphio-0.3.7/src/dongraphio/utils/matrix_utils.py
+-rw-r--r--   0        0        0     1713 2024-05-23 10:26:37.703963 dongraphio-0.3.7/src/dongraphio/utils/osm_worker.py
+-rw-r--r--   0        0        0     1738 2024-05-23 10:26:37.703963 dongraphio-0.3.7/src/dongraphio/utils/tsp_solver.py
+-rw-r--r--   0        0        0     2504 1970-01-01 00:00:00.000000 dongraphio-0.3.7/PKG-INFO
```

### Comparing `dongraphio-0.3.6/LICENSE.txt` & `dongraphio-0.3.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dongraphio-0.3.6/pyproject.toml` & `dongraphio-0.3.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dongraphio"
-version = "0.3.6"
+version = "0.3.7"
 license = "BSD-3-Clause"
 description = "Small utility library containing graph algorighms used in other projects"
 authors = ["Danila <63115678+DDonnyy@users.noreply.github.com>"]
 readme = "README.md"
 
 packages = [{ include = "dongraphio", from = "src" }]
```

### Comparing `dongraphio-0.3.6/README.md` & `dongraphio-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `dongraphio-0.3.6/src/dongraphio/base_models/grapher_logic.py` & `dongraphio-0.3.7/src/dongraphio/base_models/grapher_logic.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 pd.options.mode.chained_assignment = None
 tqdm.pandas()
 
 
 class BuildsGrapher(BaseModel):
     city_osm_id: int
     city_crs: int
-    keep_city_boundary: bool = True
     public_transport_speeds: Optional[dict] = None
     walk_speed: Optional[dict] = None
     drive_speed: Optional[dict] = None
     gdf_files: Optional[dict] = None
     truncate_by_edge: Optional[bool] = False
 
     def get_intermodal_graph(self) -> nx.MultiDiGraph:
```

### Comparing `dongraphio-0.3.6/src/dongraphio/base_models/isochrones_logic.py` & `dongraphio-0.3.7/src/dongraphio/base_models/isochrones_logic.py`

 * *Files identical despite different names*

### Comparing `dongraphio-0.3.6/src/dongraphio/base_models/matrix_logic.py` & `dongraphio-0.3.7/src/dongraphio/base_models/matrix_logic.py`

 * *Files identical despite different names*

### Comparing `dongraphio-0.3.6/src/dongraphio/dongraphio.py` & `dongraphio-0.3.7/src/dongraphio/dongraphio.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         Returns:
             nx.MultiDiGraph: The intermodal graph representing the city.
         """
         # if not all(graph_type in self.graphs for graph_type in GraphType):
         #     raise ValueError("Some graph types are missing")
         logger.info("Creating intermodal graph from OSM...")
         self._intermodal_graph = BuildsGrapher(
-            city_osm_id=city_osm_id, city_crs=self.city_crs, keep_city_boundary=keep_city_boundary
+            city_osm_id=city_osm_id, city_crs=self.city_crs, truncate_by_edge=keep_city_boundary
         ).get_intermodal_graph()
         return self._intermodal_graph
 
     def get_adjacency_matrix(
         self,
         gdf_from: gpd.GeoDataFrame,
         gdf_to: gpd.GeoDataFrame,
```

### Comparing `dongraphio-0.3.6/src/dongraphio/enums.py` & `dongraphio-0.3.7/src/dongraphio/enums.py`

 * *Files identical despite different names*

### Comparing `dongraphio-0.3.6/src/dongraphio/utils/geometry_utils.py` & `dongraphio-0.3.7/src/dongraphio/utils/geometry_utils.py`

 * *Files identical despite different names*

### Comparing `dongraphio-0.3.6/src/dongraphio/utils/graph_utils.py` & `dongraphio-0.3.7/src/dongraphio/utils/graph_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     route = pd.DataFrame(loc["members"])
     ways = route[route["type"] == "way"]
     if len(ways) > 0:
         ways = ways["geometry"].reset_index(drop=True)
         ways = ways.apply(pd.DataFrame)
         ways = ways.apply(lambda x: LineString(list(zip(x["lon"], x["lat"]))))
         ways = gpd.GeoDataFrame(ways.rename("geometry")).set_crs(4326)
-        if ways.within(boundary).all() or not use_boundary:
+        if ways.within(boundary).all() or use_boundary:
             # fix topological errors and then make LineString from MultiLineString
             ways = _get_linestring(ways.to_crs(city_crs))
         else:
             ways = None
     else:
         ways = None
```

### Comparing `dongraphio-0.3.6/src/dongraphio/utils/matrix_utils.py` & `dongraphio-0.3.7/src/dongraphio/utils/matrix_utils.py`

 * *Files identical despite different names*

### Comparing `dongraphio-0.3.6/src/dongraphio/utils/osm_worker.py` & `dongraphio-0.3.7/src/dongraphio/utils/osm_worker.py`

 * *Files identical despite different names*

### Comparing `dongraphio-0.3.6/src/dongraphio/utils/tsp_solver.py` & `dongraphio-0.3.7/src/dongraphio/utils/tsp_solver.py`

 * *Files identical despite different names*

### Comparing `dongraphio-0.3.6/PKG-INFO` & `dongraphio-0.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dongraphio
-Version: 0.3.6
+Version: 0.3.7
 Summary: Small utility library containing graph algorighms used in other projects
 License: BSD-3-Clause
 Author: Danila
 Author-email: 63115678+DDonnyy@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
```

