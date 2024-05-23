# Comparing `tmp/rashdf-0.1.1.tar.gz` & `tmp/rashdf-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rashdf-0.1.1.tar", last modified: Thu May  2 19:20:29 2024, max compression
+gzip compressed data, was "rashdf-0.2.0.tar", last modified: Thu May 23 13:38:25 2024, max compression
```

## Comparing `rashdf-0.1.1.tar` & `rashdf-0.2.0.tar`

### file list

```diff
@@ -1,23 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:20:29.771280 rashdf-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-02 19:20:17.000000 rashdf-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4180 2024-05-02 19:20:29.771280 rashdf-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-05-02 19:20:17.000000 rashdf-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-05-02 19:20:17.000000 rashdf-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 19:20:29.771280 rashdf-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:20:29.767280 rashdf-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:20:29.771280 rashdf-0.1.1/src/rashdf/
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-02 19:20:17.000000 rashdf-0.1.1/src/rashdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-05-02 19:20:17.000000 rashdf-0.1.1/src/rashdf/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    14846 2024-05-02 19:20:17.000000 rashdf-0.1.1/src/rashdf/geom.py
--rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-05-02 19:20:17.000000 rashdf-0.1.1/src/rashdf/plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     7337 2024-05-02 19:20:17.000000 rashdf-0.1.1/src/rashdf/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:20:29.771280 rashdf-0.1.1/src/rashdf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4180 2024-05-02 19:20:29.000000 rashdf-0.1.1/src/rashdf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-02 19:20:29.000000 rashdf-0.1.1/src/rashdf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 19:20:29.000000 rashdf-0.1.1/src/rashdf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-02 19:20:29.000000 rashdf-0.1.1/src/rashdf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-02 19:20:29.000000 rashdf-0.1.1/src/rashdf.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:20:29.771280 rashdf-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3649 2024-05-02 19:20:17.000000 rashdf-0.1.1/tests/test_geom.py
--rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-05-02 19:20:17.000000 rashdf-0.1.1/tests/test_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-02 19:20:17.000000 rashdf-0.1.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:38:25.252539 rashdf-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-23 13:38:15.000000 rashdf-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5125 2024-05-23 13:38:25.252539 rashdf-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4315 2024-05-23 13:38:15.000000 rashdf-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-23 13:38:15.000000 rashdf-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 13:38:25.252539 rashdf-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:38:25.248539 rashdf-0.2.0/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     4944 2024-05-23 13:38:15.000000 rashdf-0.2.0/src/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:38:25.248539 rashdf-0.2.0/src/rashdf/
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-23 13:38:15.000000 rashdf-0.2.0/src/rashdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2384 2024-05-23 13:38:15.000000 rashdf-0.2.0/src/rashdf/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16612 2024-05-23 13:38:15.000000 rashdf-0.2.0/src/rashdf/geom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-05-23 13:38:15.000000 rashdf-0.2.0/src/rashdf/plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7925 2024-05-23 13:38:15.000000 rashdf-0.2.0/src/rashdf/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:38:25.252539 rashdf-0.2.0/src/rashdf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5125 2024-05-23 13:38:25.000000 rashdf-0.2.0/src/rashdf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-23 13:38:25.000000 rashdf-0.2.0/src/rashdf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 13:38:25.000000 rashdf-0.2.0/src/rashdf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-23 13:38:25.000000 rashdf-0.2.0/src/rashdf.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-23 13:38:25.000000 rashdf-0.2.0/src/rashdf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-23 13:38:25.000000 rashdf-0.2.0/src/rashdf.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:38:25.252539 rashdf-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-05-23 13:38:15.000000 rashdf-0.2.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-05-23 13:38:15.000000 rashdf-0.2.0/tests/test_geom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-05-23 13:38:15.000000 rashdf-0.2.0/tests/test_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-05-23 13:38:15.000000 rashdf-0.2.0/tests/test_utils.py
```

### Comparing `rashdf-0.1.1/LICENSE` & `rashdf-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rashdf-0.1.1/PKG-INFO` & `rashdf-0.2.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: rashdf
-Version: 0.1.1
+Version: 0.2.0
 Summary: Read data from HEC-RAS HDF files.
 Project-URL: repository, https://github.com/fema-ffrd/rashdf
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: h5py
 Requires-Dist: geopandas
+Requires-Dist: pyarrow
 Provides-Extra: dev
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 
 # rashdf
 [![CI](https://github.com/fema-ffrd/rashdf/actions/workflows/continuous-integration.yml/badge.svg?branch=main)](https://github.com/fema-ffrd/rashdf/actions/workflows/continuous-integration.yml)
@@ -73,14 +74,56 @@
 'Run Time Window': [datetime.datetime(2024, 3, 27, 9, 31, 52),
 datetime.datetime(2024, 3, 27, 9, 32, 15)],
 'Solution': 'Unsteady Finished Successfully',
 'Time Solution Went Unstable': None,
 'Time Stamp Solution Went Unstable': 'Not Applicable'}
 ```
 
+## CLI
+The `rashdf` command-line interface allows export directly to a variety of formats, enabled
+by GeoPandas.
+```
+$ rashdf <sub-command> <hdf-file> [<output-path>] [<options>]
+```
+
+CLI help:
+```
+$ rashdf --help
+```
+
+Print the output formats supported by Fiona:
+```
+$ rashdf --fiona-drivers
+```
+
+Help for a specific subcommand:
+```
+$ rashdf mesh_cell_polygons --help
+```
+
+Example: export mesh cell faces to an ESRI Shapefile
+```
+$ rashdf mesh_cell_faces BigRiver.g01.hdf big-river-mesh-cell-faces.shp
+```
+
+Example: export mesh cell points to GeoParquet
+```
+$ rashdf mesh_cell_points LittleCreek.g01.hdf --parquet little-creek-mesh-cell-points.parquet
+```
+
+Example: export breaklines to OGC GeoPackage and reproject to a different CRS
+```
+$ rashdf breaklines Whitemarsh.p01.hdf whitemarsh-breaklines.gpkg --to-crs EPSG:4326
+```
+
+Example: write structures GeoJSON to `stdout`:
+```
+$ rashdf structures Potomac.p01.hdf
+```
+
 ## Documentation
 Coming soon.
 
 ## Developer Setup
 Create a virtual environment in the project directory:
 ```
 $ python -m venv venv-rashdf
```

### Comparing `rashdf-0.1.1/README.md` & `rashdf-0.2.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -51,14 +51,56 @@
 'Run Time Window': [datetime.datetime(2024, 3, 27, 9, 31, 52),
 datetime.datetime(2024, 3, 27, 9, 32, 15)],
 'Solution': 'Unsteady Finished Successfully',
 'Time Solution Went Unstable': None,
 'Time Stamp Solution Went Unstable': 'Not Applicable'}
 ```
 
+## CLI
+The `rashdf` command-line interface allows export directly to a variety of formats, enabled
+by GeoPandas.
+```
+$ rashdf <sub-command> <hdf-file> [<output-path>] [<options>]
+```
+
+CLI help:
+```
+$ rashdf --help
+```
+
+Print the output formats supported by Fiona:
+```
+$ rashdf --fiona-drivers
+```
+
+Help for a specific subcommand:
+```
+$ rashdf mesh_cell_polygons --help
+```
+
+Example: export mesh cell faces to an ESRI Shapefile
+```
+$ rashdf mesh_cell_faces BigRiver.g01.hdf big-river-mesh-cell-faces.shp
+```
+
+Example: export mesh cell points to GeoParquet
+```
+$ rashdf mesh_cell_points LittleCreek.g01.hdf --parquet little-creek-mesh-cell-points.parquet
+```
+
+Example: export breaklines to OGC GeoPackage and reproject to a different CRS
+```
+$ rashdf breaklines Whitemarsh.p01.hdf whitemarsh-breaklines.gpkg --to-crs EPSG:4326
+```
+
+Example: write structures GeoJSON to `stdout`:
+```
+$ rashdf structures Potomac.p01.hdf
+```
+
 ## Documentation
 Coming soon.
 
 ## Developer Setup
 Create a virtual environment in the project directory:
 ```
 $ python -m venv venv-rashdf
```

### Comparing `rashdf-0.1.1/pyproject.toml` & `rashdf-0.2.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -8,23 +8,26 @@
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
 ]
-version = "0.1.1"
-dependencies = ["h5py", "geopandas"]
+version = "0.2.0"
+dependencies = ["h5py", "geopandas", "pyarrow"]
 
 [project.optional-dependencies]
 dev = ["pre-commit", "ruff", "pytest"]
 
 [project.urls]
 repository = "https://github.com/fema-ffrd/rashdf"
 
+[project.scripts]
+rashdf = "cli:main"
+
 [tool.pytest.ini_options]
 pythonpath = "src"
 testpaths = "tests"
 
 # TODO: linting for docstrings.
 # https://github.com/fema-ffrd/rashdf/issues/15
 # [tool.ruff.lint]
```

### Comparing `rashdf-0.1.1/src/rashdf/base.py` & `rashdf-0.2.0/src/rashdf/base.py`

 * *Files identical despite different names*

### Comparing `rashdf-0.1.1/src/rashdf/geom.py` & `rashdf-0.2.0/src/rashdf/geom.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 from .base import RasHdf
-from .utils import convert_ras_hdf_string, get_first_hdf_group, hdf5_attrs_to_dict
+from .utils import (
+    convert_ras_hdf_string,
+    get_first_hdf_group,
+    hdf5_attrs_to_dict,
+    convert_ras_hdf_value,
+)
 
 import numpy as np
+import pandas as pd
 from geopandas import GeoDataFrame
 from pyproj import CRS
 from shapely import (
     Polygon,
     Point,
     LineString,
     MultiLineString,
@@ -76,15 +82,15 @@
         return GeoDataFrame(
             {"mesh_name": mesh_area_names, "geometry": mesh_area_polygons},
             geometry="geometry",
             crs=self.projection(),
         )
 
     def mesh_cell_polygons(self) -> GeoDataFrame:
-        """Return the 2D flow mesh cell polygons.
+        """Return 2D flow mesh cell polygons.
 
         Returns
         -------
         GeoDataFrame
             A GeoDataFrame containing the 2D flow mesh cell polygons if 2D areas exist.
         """
         mesh_area_names = self.mesh_area_names()
@@ -130,15 +136,15 @@
                         )
                     ).geoms[0]
                 )(face_id_lists)
             )
         return GeoDataFrame(cell_dict, geometry="geometry", crs=self.projection())
 
     def mesh_cell_points(self) -> GeoDataFrame:
-        """Return the 2D flow mesh cell points.
+        """Return 2D flow mesh cell points.
 
         Returns
         -------
         GeoDataFrame
             A GeoDataFrame containing the 2D flow mesh cell points if 2D areas exist.
         """
         mesh_area_names = self.mesh_area_names()
@@ -156,15 +162,15 @@
                 np.vectorize(lambda coords: Point(coords), signature="(n)->()")(
                     cell_pnt_coords
                 )
             )
         return GeoDataFrame(pnt_dict, geometry="geometry", crs=self.projection())
 
     def mesh_cell_faces(self) -> GeoDataFrame:
-        """Return the 2D flow mesh cell faces.
+        """Return 2D flow mesh cell faces.
 
         Returns
         -------
         GeoDataFrame
             A GeoDataFrame containing the 2D flow mesh cell faces if 2D areas exist.
         """
         mesh_area_names = self.mesh_area_names()
@@ -236,15 +242,15 @@
             )
 
         d2_flow_area_attrs = hdf5_attrs_to_dict(d2_flow_area.attrs)
 
         return d2_flow_area_attrs
 
     def bc_lines(self) -> GeoDataFrame:
-        """Return the 2D mesh area boundary condition lines.
+        """Return 2D mesh area boundary condition lines.
 
         Returns
         -------
         GeoDataFrame
             A GeoDataFrame containing the 2D mesh area boundary condition lines if they exist.
         """
         if "/Geometry/Boundary Condition Lines" not in self:
@@ -285,15 +291,15 @@
                 "geometry": geoms,
             },
             geometry="geometry",
             crs=self.projection(),
         )
 
     def breaklines(self) -> GeoDataFrame:
-        """Return the 2D mesh area breaklines.
+        """Return 2D mesh area breaklines.
 
         Returns
         -------
         GeoDataFrame
             A GeoDataFrame containing the 2D mesh area breaklines if they exist.
         """
         if "/Geometry/2D Flow Area Break Lines" not in self:
@@ -327,15 +333,15 @@
         return GeoDataFrame(
             {"bl_id": bl_line_ids, "name": names, "geometry": geoms},
             geometry="geometry",
             crs=self.projection(),
         )
 
     def refinement_regions(self) -> GeoDataFrame:
-        """Return the 2D mesh area refinement regions.
+        """Return 2D mesh area refinement regions.
 
         Returns
         -------
         GeoDataFrame
             A GeoDataFrame containing the 2D mesh area refinement regions if they exist.
         """
         if "/Geometry/2D Flow Area Refinement Regions" not in self:
@@ -360,29 +366,75 @@
                 )
         return GeoDataFrame(
             {"rr_id": rr_ids, "name": names, "geometry": geoms},
             geometry="geometry",
             crs=self.projection(),
         )
 
+    def structures(self, datetime_to_str: bool = False) -> GeoDataFrame:
+        """Return the model structures.
+
+        Returns
+        -------
+        GeoDataFrame
+            A GeoDataFrame containing the model structures if they exist.
+        """
+        if "/Geometry/Structures" not in self:
+            return GeoDataFrame()
+        struct_data = self["/Geometry/Structures"]
+        v_conv_val = np.vectorize(convert_ras_hdf_value)
+        sd_attrs = struct_data["Attributes"][()]
+        struct_dict = {"struct_id": range(sd_attrs.shape[0])}
+        struct_dict.update(
+            {name: v_conv_val(sd_attrs[name]) for name in sd_attrs.dtype.names}
+        )
+        geoms = list()
+        for pnt_start, pnt_cnt, part_start, part_cnt in struct_data["Centerline Info"][
+            ()
+        ]:
+            points = struct_data["Centerline Points"][()][
+                pnt_start : pnt_start + pnt_cnt
+            ]
+            if part_cnt == 1:
+                geoms.append(LineString(points))
+            else:
+                parts = struct_data["Centerline Parts"][()][
+                    part_start : part_start + part_cnt
+                ]
+                geoms.append(
+                    MultiLineString(
+                        list(
+                            points[part_pnt_start : part_pnt_start + part_pnt_cnt]
+                            for part_pnt_start, part_pnt_cnt in parts
+                        )
+                    )
+                )
+        struct_gdf = GeoDataFrame(
+            struct_dict,
+            geometry=geoms,
+            crs=self.projection(),
+        )
+        if datetime_to_str:
+            struct_gdf["Last Edited"] = struct_gdf["Last Edited"].apply(
+                lambda x: pd.Timestamp.isoformat(x)
+            )
+        return struct_gdf
+
     def connections(self) -> GeoDataFrame:
         raise NotImplementedError
 
     def ic_points(self) -> GeoDataFrame:
         raise NotImplementedError
 
     def reference_lines(self) -> GeoDataFrame:
         raise NotImplementedError
 
     def reference_points(self) -> GeoDataFrame:
         raise NotImplementedError
 
-    def structures(self) -> GeoDataFrame:
-        raise NotImplementedError
-
     def pump_stations(self) -> GeoDataFrame:
         raise NotImplementedError
 
     def mannings_calibration_regions(self) -> GeoDataFrame:
         raise NotImplementedError
 
     def classification_polygons(self) -> GeoDataFrame:
```

### Comparing `rashdf-0.1.1/src/rashdf/plan.py` & `rashdf-0.2.0/src/rashdf/plan.py`

 * *Files identical despite different names*

### Comparing `rashdf-0.1.1/src/rashdf/utils.py` & `rashdf-0.2.0/src/rashdf/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-import numpy as np
 import h5py
-from typing import Any, List, Tuple, Union, Optional
+import numpy as np
+import pandas as pd
 
 from datetime import datetime, timedelta
 import re
+from typing import Any, List, Tuple, Union, Optional
 
 
 def parse_ras_datetime(datetime_str: str) -> datetime:
     """Parse a datetime string from a RAS file into a datetime object.
 
     Parameters
     ----------
@@ -217,7 +218,28 @@
     ----------
         Optional[h5py.Group]: The first HDF5 group in the parent group, or None if no group is found.
     """
     for _, item in parent_group.items():
         if isinstance(item, h5py.Group):
             return item
     return None
+
+
+def df_datetimes_to_str(df: pd.DataFrame) -> pd.DataFrame:
+    """Convert any datetime64 columns in a DataFrame to strings.
+
+    Parameters
+    ----------
+    df : DataFrame
+        The DataFrame to convert.
+
+    Returns
+    -------
+    DataFrame
+        The DataFrame with any datetime64 columns converted to strings.
+    """
+    df_result = df.copy()
+    for col in df.select_dtypes(include=["datetime64"]).columns:
+        df_result[col] = df[col].apply(
+            lambda x: pd.Timestamp(x).isoformat() if pd.notnull(x) else None
+        )
+    return df_result
```

### Comparing `rashdf-0.1.1/src/rashdf.egg-info/PKG-INFO` & `rashdf-0.2.0/src/rashdf.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: rashdf
-Version: 0.1.1
+Version: 0.2.0
 Summary: Read data from HEC-RAS HDF files.
 Project-URL: repository, https://github.com/fema-ffrd/rashdf
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: h5py
 Requires-Dist: geopandas
+Requires-Dist: pyarrow
 Provides-Extra: dev
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 
 # rashdf
 [![CI](https://github.com/fema-ffrd/rashdf/actions/workflows/continuous-integration.yml/badge.svg?branch=main)](https://github.com/fema-ffrd/rashdf/actions/workflows/continuous-integration.yml)
@@ -73,14 +74,56 @@
 'Run Time Window': [datetime.datetime(2024, 3, 27, 9, 31, 52),
 datetime.datetime(2024, 3, 27, 9, 32, 15)],
 'Solution': 'Unsteady Finished Successfully',
 'Time Solution Went Unstable': None,
 'Time Stamp Solution Went Unstable': 'Not Applicable'}
 ```
 
+## CLI
+The `rashdf` command-line interface allows export directly to a variety of formats, enabled
+by GeoPandas.
+```
+$ rashdf <sub-command> <hdf-file> [<output-path>] [<options>]
+```
+
+CLI help:
+```
+$ rashdf --help
+```
+
+Print the output formats supported by Fiona:
+```
+$ rashdf --fiona-drivers
+```
+
+Help for a specific subcommand:
+```
+$ rashdf mesh_cell_polygons --help
+```
+
+Example: export mesh cell faces to an ESRI Shapefile
+```
+$ rashdf mesh_cell_faces BigRiver.g01.hdf big-river-mesh-cell-faces.shp
+```
+
+Example: export mesh cell points to GeoParquet
+```
+$ rashdf mesh_cell_points LittleCreek.g01.hdf --parquet little-creek-mesh-cell-points.parquet
+```
+
+Example: export breaklines to OGC GeoPackage and reproject to a different CRS
+```
+$ rashdf breaklines Whitemarsh.p01.hdf whitemarsh-breaklines.gpkg --to-crs EPSG:4326
+```
+
+Example: write structures GeoJSON to `stdout`:
+```
+$ rashdf structures Potomac.p01.hdf
+```
+
 ## Documentation
 Coming soon.
 
 ## Developer Setup
 Create a virtual environment in the project directory:
 ```
 $ python -m venv venv-rashdf
```

### Comparing `rashdf-0.1.1/tests/test_geom.py` & `rashdf-0.2.0/tests/test_geom.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,7 +94,13 @@
 def test_get_geom_2d_flow_area_attrs(tmp_path):
     test_hdf = tmp_path / "test.hdf"
     _create_hdf_with_group_attrs(
         test_hdf, f"{RasGeomHdf.FLOW_AREA_2D_PATH}/group", TEST_ATTRS
     )
     ras_hdf = RasGeomHdf(test_hdf)
     assert ras_hdf.get_geom_2d_flow_area_attrs() == TEST_ATTRS
+
+
+def test_structs():
+    structs_json = TEST_JSON / "structures.json"
+    with RasGeomHdf(MUNCIE_G05) as ghdf:
+        assert _gdf_matches_json(ghdf.structures(datetime_to_str=True), structs_json)
```

### Comparing `rashdf-0.1.1/tests/test_plan.py` & `rashdf-0.2.0/tests/test_plan.py`

 * *Files identical despite different names*

