# Comparing `tmp/sdkfabric_starwars-0.1.3.tar.gz` & `tmp/sdkfabric_starwars-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdkfabric_starwars-0.1.3.tar", last modified: Wed May 22 21:11:13 2024, max compression
+gzip compressed data, was "sdkfabric_starwars-0.1.4.tar", last modified: Thu May 23 21:17:08 2024, max compression
```

## Comparing `sdkfabric_starwars-0.1.3.tar` & `sdkfabric_starwars-0.1.4.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:11:13.088751 sdkfabric_starwars-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-22 21:11:09.000000 sdkfabric_starwars-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-05-22 21:11:13.084751 sdkfabric_starwars-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-22 21:11:09.000000 sdkfabric_starwars-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-22 21:11:09.000000 sdkfabric_starwars-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 21:11:13.088751 sdkfabric_starwars-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 21:11:09.000000 sdkfabric_starwars-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:11:13.080751 sdkfabric_starwars-0.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:11:13.084751 sdkfabric_starwars-0.1.3/src/sdk/
--rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-05-22 21:11:09.000000 sdkfabric_starwars-0.1.3/src/sdk/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-22 21:11:09.000000 sdkfabric_starwars-0.1.3/src/sdk/collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-05-22 21:11:09.000000 sdkfabric_starwars-0.1.3/src/sdk/film.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-22 21:11:09.000000 sdkfabric_starwars-0.1.3/src/sdk/film_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-05-22 21:11:09.000000 sdkfabric_starwars-0.1.3/src/sdk/film_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-22 21:11:09.000000 sdkfabric_starwars-0.1.3/src/sdk/people.py
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-22 21:11:09.000000 sdkfabric_starwars-0.1.3/src/sdk/people_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-05-22 21:11:09.000000 sdkfabric_starwars-0.1.3/src/sdk/people_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-05-22 21:11:09.000000 sdkfabric_starwars-0.1.3/src/sdk/planet.py
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-22 21:11:09.000000 sdkfabric_starwars-0.1.3/src/sdk/planet_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-05-22 21:11:09.000000 sdkfabric_starwars-0.1.3/src/sdk/planet_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-22 21:11:09.000000 sdkfabric_starwars-0.1.3/src/sdk/root.py
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-05-22 21:11:09.000000 sdkfabric_starwars-0.1.3/src/sdk/specie.py
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-22 21:11:09.000000 sdkfabric_starwars-0.1.3/src/sdk/specie_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2131 2024-05-22 21:11:09.000000 sdkfabric_starwars-0.1.3/src/sdk/specie_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-05-22 21:11:09.000000 sdkfabric_starwars-0.1.3/src/sdk/starship.py
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-22 21:11:09.000000 sdkfabric_starwars-0.1.3/src/sdk/starship_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-05-22 21:11:09.000000 sdkfabric_starwars-0.1.3/src/sdk/starship_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-05-22 21:11:09.000000 sdkfabric_starwars-0.1.3/src/sdk/vehicle.py
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-22 21:11:09.000000 sdkfabric_starwars-0.1.3/src/sdk/vehicle_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-05-22 21:11:09.000000 sdkfabric_starwars-0.1.3/src/sdk/vehicle_tag.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:11:13.084751 sdkfabric_starwars-0.1.3/src/sdkfabric_starwars.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-05-22 21:11:13.000000 sdkfabric_starwars-0.1.3/src/sdkfabric_starwars.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-22 21:11:13.000000 sdkfabric_starwars-0.1.3/src/sdkfabric_starwars.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 21:11:13.000000 sdkfabric_starwars-0.1.3/src/sdkfabric_starwars.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-22 21:11:13.000000 sdkfabric_starwars-0.1.3/src/sdkfabric_starwars.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-22 21:11:13.000000 sdkfabric_starwars-0.1.3/src/sdkfabric_starwars.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:17:08.163512 sdkfabric_starwars-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-23 21:17:04.000000 sdkfabric_starwars-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-05-23 21:17:08.163512 sdkfabric_starwars-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-23 21:17:04.000000 sdkfabric_starwars-0.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-23 21:17:04.000000 sdkfabric_starwars-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 21:17:08.163512 sdkfabric_starwars-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 21:17:04.000000 sdkfabric_starwars-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:17:08.155511 sdkfabric_starwars-0.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:17:08.163512 sdkfabric_starwars-0.1.4/src/sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-05-23 21:17:04.000000 sdkfabric_starwars-0.1.4/src/sdk/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-05-23 21:17:04.000000 sdkfabric_starwars-0.1.4/src/sdk/collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-05-23 21:17:04.000000 sdkfabric_starwars-0.1.4/src/sdk/film.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-23 21:17:04.000000 sdkfabric_starwars-0.1.4/src/sdk/film_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-05-23 21:17:04.000000 sdkfabric_starwars-0.1.4/src/sdk/film_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-23 21:17:04.000000 sdkfabric_starwars-0.1.4/src/sdk/people.py
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-23 21:17:04.000000 sdkfabric_starwars-0.1.4/src/sdk/people_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-05-23 21:17:04.000000 sdkfabric_starwars-0.1.4/src/sdk/people_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-05-23 21:17:04.000000 sdkfabric_starwars-0.1.4/src/sdk/planet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-05-23 21:17:04.000000 sdkfabric_starwars-0.1.4/src/sdk/planet_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2130 2024-05-23 21:17:04.000000 sdkfabric_starwars-0.1.4/src/sdk/planet_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-23 21:17:04.000000 sdkfabric_starwars-0.1.4/src/sdk/root.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-05-23 21:17:04.000000 sdkfabric_starwars-0.1.4/src/sdk/species.py
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-23 21:17:04.000000 sdkfabric_starwars-0.1.4/src/sdk/species_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-05-23 21:17:04.000000 sdkfabric_starwars-0.1.4/src/sdk/species_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-05-23 21:17:04.000000 sdkfabric_starwars-0.1.4/src/sdk/starship.py
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-23 21:17:04.000000 sdkfabric_starwars-0.1.4/src/sdk/starship_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-05-23 21:17:04.000000 sdkfabric_starwars-0.1.4/src/sdk/starship_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1581 2024-05-23 21:17:04.000000 sdkfabric_starwars-0.1.4/src/sdk/vehicle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-23 21:17:04.000000 sdkfabric_starwars-0.1.4/src/sdk/vehicle_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-05-23 21:17:04.000000 sdkfabric_starwars-0.1.4/src/sdk/vehicle_tag.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:17:08.163512 sdkfabric_starwars-0.1.4/src/sdkfabric_starwars.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-05-23 21:17:08.000000 sdkfabric_starwars-0.1.4/src/sdkfabric_starwars.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-23 21:17:08.000000 sdkfabric_starwars-0.1.4/src/sdkfabric_starwars.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 21:17:08.000000 sdkfabric_starwars-0.1.4/src/sdkfabric_starwars.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-23 21:17:08.000000 sdkfabric_starwars-0.1.4/src/sdkfabric_starwars.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-23 21:17:08.000000 sdkfabric_starwars-0.1.4/src/sdkfabric_starwars.egg-info/top_level.txt
```

### Comparing `sdkfabric_starwars-0.1.3/LICENSE` & `sdkfabric_starwars-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sdkfabric_starwars-0.1.3/PKG-INFO` & `sdkfabric_starwars-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdkfabric-starwars
-Version: 0.1.3
+Version: 0.1.4
 Summary: Starwars Python SDK managed by SDK Fabric
 Author-email: Christoph Kappestein <christoph.kappestein@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/sdk-fabric/starwars-python
 Project-URL: Issues, https://github.com/sdk-fabric/starwars-python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sdkfabric_starwars-0.1.3/README.md` & `sdkfabric_starwars-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `sdkfabric_starwars-0.1.3/pyproject.toml` & `sdkfabric_starwars-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "sdkfabric-starwars"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
   { name="Christoph Kappestein", email="christoph.kappestein@gmail.com" },
 ]
 description = "Starwars Python SDK managed by SDK Fabric"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {text = "MIT"}
```

### Comparing `sdkfabric_starwars-0.1.3/src/sdk/client.py` & `sdkfabric_starwars-0.1.4/src/sdk/client.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 import sdkgen
 from requests import RequestException
 from typing import List
 
 from .people_tag import PeopleTag
 from .film_tag import FilmTag
 from .starship_tag import StarshipTag
+from .species_tag import SpeciesTag
 from .vehicle_tag import VehicleTag
-from .specie_tag import SpecieTag
 from .planet_tag import PlanetTag
 
 class Client(sdkgen.ClientAbstract):
     def __init__(self, base_url: str, credentials: sdkgen.CredentialsInterface):
         super().__init__(base_url, credentials)
 
     def people(self) -> PeopleTag:
@@ -33,22 +33,22 @@
 
     def starship(self) -> StarshipTag:
         return StarshipTag(
             self.http_client,
             self.parser
         )
 
-    def vehicle(self) -> VehicleTag:
-        return VehicleTag(
+    def species(self) -> SpeciesTag:
+        return SpeciesTag(
             self.http_client,
             self.parser
         )
 
-    def specie(self) -> SpecieTag:
-        return SpecieTag(
+    def vehicle(self) -> VehicleTag:
+        return VehicleTag(
             self.http_client,
             self.parser
         )
 
     def planet(self) -> PlanetTag:
         return PlanetTag(
             self.http_client,
```

### Comparing `sdkfabric_starwars-0.1.3/src/sdk/collection.py` & `sdkfabric_starwars-0.1.4/src/sdk/collection.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_starwars-0.1.3/src/sdk/film.py` & `sdkfabric_starwars-0.1.4/src/sdk/film.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_starwars-0.1.3/src/sdk/film_tag.py` & `sdkfabric_starwars-0.1.4/src/sdk/film_tag.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_starwars-0.1.3/src/sdk/people.py` & `sdkfabric_starwars-0.1.4/src/sdk/people.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_starwars-0.1.3/src/sdk/people_tag.py` & `sdkfabric_starwars-0.1.4/src/sdk/people_tag.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_starwars-0.1.3/src/sdk/planet.py` & `sdkfabric_starwars-0.1.4/src/sdk/planet.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_starwars-0.1.3/src/sdk/planet_tag.py` & `sdkfabric_starwars-0.1.4/src/sdk/planet_tag.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_starwars-0.1.3/src/sdk/root.py` & `sdkfabric_starwars-0.1.4/src/sdk/root.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_starwars-0.1.3/src/sdk/specie.py` & `sdkfabric_starwars-0.1.4/src/sdk/species.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """
-specie automatically generated by SDKgen please do not edit this file manually
+species automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 from pydantic import BaseModel, Field, GetCoreSchemaHandler
 from pydantic_core import CoreSchema, core_schema
 from typing import Any, Dict, Generic, List, Optional, TypeVar, Union
 import datetime
 
 
 # A Species is a type of person or character within the Star Wars Universe.
-class Specie(BaseModel):
+class Species(BaseModel):
     name: Optional[str] = Field(default=None, alias="name")
     classification: Optional[str] = Field(default=None, alias="classification")
     designation: Optional[str] = Field(default=None, alias="designation")
     average_height: Optional[str] = Field(default=None, alias="average_height")
     average_lifespan: Optional[str] = Field(default=None, alias="average_lifespan")
     eye_colors: Optional[str] = Field(default=None, alias="eye_colors")
     hair_colors: Optional[str] = Field(default=None, alias="hair_colors")
```

### Comparing `sdkfabric_starwars-0.1.3/src/sdk/specie_tag.py` & `sdkfabric_starwars-0.1.4/src/sdk/vehicle_tag.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,71 +1,71 @@
 """
-SpecieTag automatically generated by SDKgen please do not edit this file manually
+VehicleTag automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 import requests
 import sdkgen
 from requests import RequestException
 from typing import List
 
-from .specie import Specie
-from .specie_collection import SpecieCollection
+from .vehicle import Vehicle
+from .vehicle_collection import VehicleCollection
 
-class SpecieTag(sdkgen.TagAbstract):
+class VehicleTag(sdkgen.TagAbstract):
     def __init__(self, http_client: requests.Session, parser: sdkgen.Parser):
         super().__init__(http_client, parser)
 
 
-    def get_all(self, search: str) -> SpecieCollection:
+    def get_all(self, search: str) -> VehicleCollection:
         """
-        Get all the species
+        Get all the vehicles
         """
         try:
             path_params = {}
 
             query_params = {}
             query_params["search"] = search
 
             query_struct_names = []
 
-            url = self.parser.url("/species", path_params)
+            url = self.parser.url("/vehicles", path_params)
 
             headers = {}
 
             response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return SpecieCollection.model_validate_json(json_data=response.content)
+                return VehicleCollection.model_validate_json(json_data=response.content)
 
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    def get(self, id: str) -> Specie:
+    def get(self, id: str) -> Vehicle:
         """
-        Get a specific species
+        Get a specific vehicle
         """
         try:
             path_params = {}
             path_params["id"] = id
 
             query_params = {}
 
             query_struct_names = []
 
-            url = self.parser.url("/species/:id", path_params)
+            url = self.parser.url("/vehicles/:id", path_params)
 
             headers = {}
 
             response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return Specie.model_validate_json(json_data=response.content)
+                return Vehicle.model_validate_json(json_data=response.content)
 
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
```

### Comparing `sdkfabric_starwars-0.1.3/src/sdk/starship.py` & `sdkfabric_starwars-0.1.4/src/sdk/starship.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_starwars-0.1.3/src/sdk/starship_tag.py` & `sdkfabric_starwars-0.1.4/src/sdk/starship_tag.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_starwars-0.1.3/src/sdk/vehicle.py` & `sdkfabric_starwars-0.1.4/src/sdk/vehicle.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_starwars-0.1.3/src/sdk/vehicle_tag.py` & `sdkfabric_starwars-0.1.4/src/sdk/species_tag.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,71 +1,71 @@
 """
-VehicleTag automatically generated by SDKgen please do not edit this file manually
+SpeciesTag automatically generated by SDKgen please do not edit this file manually
 https://sdkgen.app
 """
 
 import requests
 import sdkgen
 from requests import RequestException
 from typing import List
 
-from .vehicle import Vehicle
-from .vehicle_collection import VehicleCollection
+from .species import Species
+from .species_collection import SpeciesCollection
 
-class VehicleTag(sdkgen.TagAbstract):
+class SpeciesTag(sdkgen.TagAbstract):
     def __init__(self, http_client: requests.Session, parser: sdkgen.Parser):
         super().__init__(http_client, parser)
 
 
-    def get_all(self, search: str) -> VehicleCollection:
+    def get_all(self, search: str) -> SpeciesCollection:
         """
-        Get all the vehicles
+        Get all the species
         """
         try:
             path_params = {}
 
             query_params = {}
             query_params["search"] = search
 
             query_struct_names = []
 
-            url = self.parser.url("/vehicles", path_params)
+            url = self.parser.url("/species", path_params)
 
             headers = {}
 
             response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return VehicleCollection.model_validate_json(json_data=response.content)
+                return SpeciesCollection.model_validate_json(json_data=response.content)
 
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
 
-    def get(self, id: str) -> Vehicle:
+    def get(self, id: str) -> Species:
         """
-        Get a specific vehicle
+        Get a specific species
         """
         try:
             path_params = {}
             path_params["id"] = id
 
             query_params = {}
 
             query_struct_names = []
 
-            url = self.parser.url("/vehicles/:id", path_params)
+            url = self.parser.url("/species/:id", path_params)
 
             headers = {}
 
             response = self.http_client.get(url, headers=headers, params=self.parser.query(query_params, query_struct_names))
 
             if response.status_code >= 200 and response.status_code < 300:
-                return Vehicle.model_validate_json(json_data=response.content)
+                return Species.model_validate_json(json_data=response.content)
 
 
             raise sdkgen.UnknownStatusCodeException("The server returned an unknown status code")
         except RequestException as e:
             raise sdkgen.ClientException("An unknown error occurred: " + str(e))
```

### Comparing `sdkfabric_starwars-0.1.3/src/sdkfabric_starwars.egg-info/PKG-INFO` & `sdkfabric_starwars-0.1.4/src/sdkfabric_starwars.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdkfabric-starwars
-Version: 0.1.3
+Version: 0.1.4
 Summary: Starwars Python SDK managed by SDK Fabric
 Author-email: Christoph Kappestein <christoph.kappestein@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/sdk-fabric/starwars-python
 Project-URL: Issues, https://github.com/sdk-fabric/starwars-python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sdkfabric_starwars-0.1.3/src/sdkfabric_starwars.egg-info/SOURCES.txt` & `sdkfabric_starwars-0.1.4/src/sdkfabric_starwars.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 src/sdk/people.py
 src/sdk/people_collection.py
 src/sdk/people_tag.py
 src/sdk/planet.py
 src/sdk/planet_collection.py
 src/sdk/planet_tag.py
 src/sdk/root.py
-src/sdk/specie.py
-src/sdk/specie_collection.py
-src/sdk/specie_tag.py
+src/sdk/species.py
+src/sdk/species_collection.py
+src/sdk/species_tag.py
 src/sdk/starship.py
 src/sdk/starship_collection.py
 src/sdk/starship_tag.py
 src/sdk/vehicle.py
 src/sdk/vehicle_collection.py
 src/sdk/vehicle_tag.py
 src/sdkfabric_starwars.egg-info/PKG-INFO
```

