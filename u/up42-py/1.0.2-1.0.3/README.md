# Comparing `tmp/up42_py-1.0.2.tar.gz` & `tmp/up42_py-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "up42_py-1.0.2.tar", max compression
+gzip compressed data, was "up42_py-1.0.3.tar", max compression
```

## Comparing `up42_py-1.0.2.tar` & `up42_py-1.0.3.tar`

### file list

```diff
@@ -1,27 +1,26 @@
--rw-r--r--   0        0        0     1061 2024-05-15 11:22:44.134850 up42_py-1.0.2/LICENSE
--rw-r--r--   0        0        0     2927 2024-05-15 11:22:44.134850 up42_py-1.0.2/README.md
--rw-r--r--   0        0        0     1785 2024-05-15 11:22:44.154850 up42_py-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     1731 2024-05-15 11:22:44.162850 up42_py-1.0.2/up42/__init__.py
--rw-r--r--   0        0        0     7963 2024-05-15 11:22:44.162850 up42_py-1.0.2/up42/asset.py
--rw-r--r--   0        0        0     3754 2024-05-15 11:22:44.162850 up42_py-1.0.2/up42/asset_searcher.py
--rw-r--r--   0        0        0     5068 2024-05-15 11:22:44.162850 up42_py-1.0.2/up42/auth.py
--rw-r--r--   0        0        0    20308 2024-05-15 11:22:44.162850 up42_py-1.0.2/up42/catalog.py
--rw-r--r--   0        0        0      706 2024-05-15 11:22:44.162850 up42_py-1.0.2/up42/data/aoi_berlin.geojson
--rw-r--r--   0        0        0      703 2024-05-15 11:22:44.162850 up42_py-1.0.2/up42/data/aoi_washington.geojson
--rw-r--r--   0        0        0      135 2024-05-15 11:22:44.162850 up42_py-1.0.2/up42/host.py
--rw-r--r--   0        0        0        0 2024-05-15 11:22:44.162850 up42_py-1.0.2/up42/http/__init__.py
--rw-r--r--   0        0        0     1782 2024-05-15 11:22:44.162850 up42_py-1.0.2/up42/http/client.py
--rw-r--r--   0        0        0      482 2024-05-15 11:22:44.162850 up42_py-1.0.2/up42/http/config.py
--rw-r--r--   0        0        0      673 2024-05-15 11:22:44.162850 up42_py-1.0.2/up42/http/http_adapter.py
--rw-r--r--   0        0        0     3378 2024-05-15 11:22:44.162850 up42_py-1.0.2/up42/http/oauth.py
--rw-r--r--   0        0        0     1113 2024-05-15 11:22:44.162850 up42_py-1.0.2/up42/http/session.py
--rw-r--r--   0        0        0     1885 2024-05-15 11:22:44.162850 up42_py-1.0.2/up42/initialization.py
--rw-r--r--   0        0        0     3424 2024-05-15 11:22:44.162850 up42_py-1.0.2/up42/main.py
--rw-r--r--   0        0        0     8372 2024-05-15 11:22:44.162850 up42_py-1.0.2/up42/order.py
--rw-r--r--   0        0        0      910 2024-05-15 11:22:44.162850 up42_py-1.0.2/up42/stac_client.py
--rw-r--r--   0        0        0     8485 2024-05-15 11:22:44.162850 up42_py-1.0.2/up42/storage.py
--rw-r--r--   0        0        0    10622 2024-05-15 11:22:44.162850 up42_py-1.0.2/up42/tasking.py
--rw-r--r--   0        0        0     3287 2024-05-15 11:22:44.162850 up42_py-1.0.2/up42/tools.py
--rw-r--r--   0        0        0    15164 2024-05-15 11:22:44.162850 up42_py-1.0.2/up42/utils.py
--rw-r--r--   0        0        0     6749 2024-05-15 11:22:44.162850 up42_py-1.0.2/up42/webhooks.py
--rw-r--r--   0        0        0     3964 1970-01-01 00:00:00.000000 up42_py-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1061 2024-05-23 14:01:24.305753 up42_py-1.0.3/LICENSE
+-rw-r--r--   0        0        0     2927 2024-05-23 14:01:24.305753 up42_py-1.0.3/README.md
+-rw-r--r--   0        0        0     1805 2024-05-23 14:01:24.325754 up42_py-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1731 2024-05-23 14:01:24.333754 up42_py-1.0.3/up42/__init__.py
+-rw-r--r--   0        0        0     7699 2024-05-23 14:01:24.333754 up42_py-1.0.3/up42/asset.py
+-rw-r--r--   0        0        0     3754 2024-05-23 14:01:24.333754 up42_py-1.0.3/up42/asset_searcher.py
+-rw-r--r--   0        0        0     4989 2024-05-23 14:01:24.333754 up42_py-1.0.3/up42/auth.py
+-rw-r--r--   0        0        0    20308 2024-05-23 14:01:24.333754 up42_py-1.0.3/up42/catalog.py
+-rw-r--r--   0        0        0      706 2024-05-23 14:01:24.333754 up42_py-1.0.3/up42/data/aoi_berlin.geojson
+-rw-r--r--   0        0        0      703 2024-05-23 14:01:24.333754 up42_py-1.0.3/up42/data/aoi_washington.geojson
+-rw-r--r--   0        0        0      135 2024-05-23 14:01:24.333754 up42_py-1.0.3/up42/host.py
+-rw-r--r--   0        0        0        0 2024-05-23 14:01:24.333754 up42_py-1.0.3/up42/http/__init__.py
+-rw-r--r--   0        0        0     1695 2024-05-23 14:01:24.333754 up42_py-1.0.3/up42/http/client.py
+-rw-r--r--   0        0        0      482 2024-05-23 14:01:24.333754 up42_py-1.0.3/up42/http/config.py
+-rw-r--r--   0        0        0      673 2024-05-23 14:01:24.333754 up42_py-1.0.3/up42/http/http_adapter.py
+-rw-r--r--   0        0        0     3378 2024-05-23 14:01:24.333754 up42_py-1.0.3/up42/http/oauth.py
+-rw-r--r--   0        0        0     1113 2024-05-23 14:01:24.333754 up42_py-1.0.3/up42/http/session.py
+-rw-r--r--   0        0        0     1885 2024-05-23 14:01:24.333754 up42_py-1.0.3/up42/initialization.py
+-rw-r--r--   0        0        0     3424 2024-05-23 14:01:24.333754 up42_py-1.0.3/up42/main.py
+-rw-r--r--   0        0        0     8372 2024-05-23 14:01:24.337754 up42_py-1.0.3/up42/order.py
+-rw-r--r--   0        0        0     8470 2024-05-23 14:01:24.337754 up42_py-1.0.3/up42/storage.py
+-rw-r--r--   0        0        0    10622 2024-05-23 14:01:24.337754 up42_py-1.0.3/up42/tasking.py
+-rw-r--r--   0        0        0     3287 2024-05-23 14:01:24.337754 up42_py-1.0.3/up42/tools.py
+-rw-r--r--   0        0        0    15643 2024-05-23 14:01:24.337754 up42_py-1.0.3/up42/utils.py
+-rw-r--r--   0        0        0     6749 2024-05-23 14:01:24.337754 up42_py-1.0.3/up42/webhooks.py
+-rw-r--r--   0        0        0     4005 1970-01-01 00:00:00.000000 up42_py-1.0.3/PKG-INFO
```

### Comparing `up42_py-1.0.2/LICENSE` & `up42_py-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `up42_py-1.0.2/README.md` & `up42_py-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `up42_py-1.0.2/pyproject.toml` & `up42_py-1.0.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "up42-py"
-version = "1.0.2"
+version = "1.0.3"
 description = "Python SDK for UP42, the geospatial marketplace and developer platform."
 authors = ["UP42 GmbH <support@up42.com>"]
 license = "https://github.com/up42/up42-py/blob/master/LICENSE"
 readme = "README.md"
 packages = [
     { include = "up42", from = "." },
 ]
@@ -20,14 +20,15 @@
 python = ">=3.9, <4"
 requests = "^2.31.0"
 tqdm = "^4.66.0"
 geojson = "3.1.0"
 geopandas = "^0.13.2"
 pystac-client = "^0.7.2"
 pyproj = "^3.6.1"
+tenacity = "^8.3.0"
 
 
 [tool.poetry.dev-dependencies]
 nbconvert = "^7.16.2"
 black = "^24.3.0"
 requests-mock = "^1.9.3"
 pylint = "^3.0.3"
```

### Comparing `up42_py-1.0.2/up42/__init__.py` & `up42_py-1.0.3/up42/__init__.py`

 * *Files identical despite different names*

### Comparing `up42_py-1.0.2/up42/asset.py` & `up42_py-1.0.3/up42/asset.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 import pathlib
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 import pystac
 import pystac_client
+import tenacity as tnc
 
 from up42 import auth as up42_auth
-from up42 import host, stac_client, utils
+from up42 import host, utils
 
 logger = utils.get_logger(__name__)
 
 MAX_ITEM = 50
 LIMIT = 50
 
 NOT_PROVIDED = object()
+_retry = tnc.retry(
+    stop=tnc.stop_after_attempt(5),
+    wait=tnc.wait_exponential(multiplier=1),
+    reraise=True,
+)
 
 
 class Asset:
     """
     The Asset class enables access to the UP42 assets in the storage. Assets are results
     of orders or results of jobs with download blocks.
 
@@ -48,52 +54,49 @@
     def asset_id(self) -> dict:
         return self.info.get("id")
 
     def _get_info(self, asset_id: str):
         url = host.endpoint(f"/v2/assets/{asset_id}/metadata")
         return self.auth.request(request_type="GET", url=url)
 
-    @property
     def _stac_search(self) -> Tuple[pystac_client.Client, pystac_client.ItemSearch]:
-        url = host.endpoint("/v2/assets/stac")
-        pystac_client_aux = stac_client.PySTACAuthClient(auth=self.auth).open(url=url)
+        stac_client = utils.stac_client(self.auth.client.auth)
         stac_search_parameters = {
             "max_items": MAX_ITEM,
             "limit": LIMIT,
             "filter": {
                 "op": "=",
                 "args": [
                     {"property": "asset_id"},
                     self.asset_id,
                 ],
             },
         }
-        pystac_asset_search = pystac_client_aux.search(filter=stac_search_parameters)
-        return (pystac_client_aux, pystac_asset_search)
+        return stac_client, stac_client.search(filter=stac_search_parameters)
 
     @property
-    def stac_info(self) -> Optional[pystac.Collection]:
+    @_retry
+    def stac_info(self) -> Union[pystac.Collection, pystac_client.CollectionClient]:
         """
         Gets the storage STAC information for the asset as a FeatureCollection.
         One asset can contain multiple STAC items (e.g. the PAN and multispectral images).
         """
-        pystac_client_aux, pystac_asset_search = self._stac_search
-        resulting_item = pystac_asset_search.item_collection()
-        if resulting_item is None:
+        stac_client, stac_search = self._stac_search()
+        items = stac_search.item_collection()
+        if not items:
             raise ValueError(f"No STAC metadata information available for this asset {self.asset_id}")
-        collection_id = resulting_item[0].collection_id
-        return pystac_client_aux.get_collection(collection_id)
+        return stac_client.get_collection(items[0].collection_id)
 
     @property
+    @_retry
     def stac_items(self) -> pystac.ItemCollection:
         """Returns the stac items from an UP42 asset STAC representation."""
         try:
-            _, pystac_asset_search = self._stac_search
-            resulting_items = pystac_asset_search.item_collection()
-            return resulting_items
+            _, stac_search = self._stac_search()
+            return stac_search.item_collection()
         except Exception as exc:
             raise ValueError(f"No STAC metadata information available for this asset {self.asset_id}") from exc
 
     def update_metadata(
         self,
         title: Union[Optional[str], object] = NOT_PROVIDED,
         tags: Union[Optional[List[str]], object] = NOT_PROVIDED,
@@ -161,25 +164,19 @@
             output_directory = pathlib.Path.cwd() / f"asset_{self.asset_id}"
         else:
             output_directory = pathlib.Path(output_directory)
         output_directory.mkdir(parents=True, exist_ok=True)
         logger.info("Download directory: %s", output_directory)
 
         download_url = self._get_download_url()
-        if unpacking:
-            out_filepaths = utils.download_archive(
-                download_url=download_url,
-                output_directory=output_directory,
-            )
-        else:
-            out_filepaths = utils.download_file(
-                download_url=download_url,
-                output_directory=output_directory,
-            )
-
+        download = utils.download_archive if unpacking else utils.download_file
+        out_filepaths = download(
+            download_url=download_url,
+            output_directory=output_directory,
+        )
         self.results = out_filepaths
         return out_filepaths
 
     def download_stac_asset(
         self,
         stac_asset: pystac.Asset,
         output_directory: Union[str, pathlib.Path, None] = None,
```

### Comparing `up42_py-1.0.2/up42/asset_searcher.py` & `up42_py-1.0.3/up42/asset_searcher.py`

 * *Files identical despite different names*

### Comparing `up42_py-1.0.2/up42/auth.py` & `up42_py-1.0.3/up42/auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,25 +49,21 @@
         Args:
             cfg_file: File path to the cfg.json with {username: "...", password: "..."}.
             username: The username for the UP42 account (email UP42 console).
             password: Password for the UP42 console login.
         """
         self.workspace_id: Optional[str] = None
         credential_sources = get_credential_sources(cfg_file, username, password)
-        self._client = create_client(credential_sources, host.endpoint("/oauth/token"))
+        self.client = create_client(credential_sources, host.endpoint("/oauth/token"))
         self._get_workspace()
         logger.info("Authentication with UP42 successful!")
 
     @property
-    def token(self) -> str:
-        return self._client.token
-
-    @property
     def session(self) -> requests.Session:
-        return self._client.session
+        return self.client.session
 
     def _get_workspace(self) -> None:
         """Get user id belonging to authenticated account."""
         url = host.endpoint("/users/me")
         resp = self.request("GET", url)
         self.workspace_id = resp["data"]["id"]
```

### Comparing `up42_py-1.0.2/up42/catalog.py` & `up42_py-1.0.3/up42/catalog.py`

 * *Files identical despite different names*

### Comparing `up42_py-1.0.2/up42/data/aoi_berlin.geojson` & `up42_py-1.0.3/up42/data/aoi_berlin.geojson`

 * *Files identical despite different names*

### Comparing `up42_py-1.0.2/up42/data/aoi_washington.geojson` & `up42_py-1.0.3/up42/data/aoi_washington.geojson`

 * *Files identical despite different names*

### Comparing `up42_py-1.0.2/up42/http/client.py` & `up42_py-1.0.3/up42/http/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,18 +10,14 @@
 
 
 class Client:
     def __init__(self, auth: oauth.Up42Auth, create_session: SessionFactory):
         self.auth = auth
         self.session = create_session(auth)
 
-    @property
-    def token(self) -> str:
-        return self.auth.token.access_token
-
 
 def _merge(
     left: Optional[config.CredentialsSettings],
     right: Optional[config.CredentialsSettings],
 ):
     if all([left, right]):
         raise MultipleCredentialsSources("Multiple sources of credentials provided")
```

### Comparing `up42_py-1.0.2/up42/http/http_adapter.py` & `up42_py-1.0.3/up42/http/http_adapter.py`

 * *Files identical despite different names*

### Comparing `up42_py-1.0.2/up42/http/oauth.py` & `up42_py-1.0.3/up42/http/oauth.py`

 * *Files identical despite different names*

### Comparing `up42_py-1.0.2/up42/http/session.py` & `up42_py-1.0.3/up42/http/session.py`

 * *Files identical despite different names*

### Comparing `up42_py-1.0.2/up42/initialization.py` & `up42_py-1.0.3/up42/initialization.py`

 * *Files identical despite different names*

### Comparing `up42_py-1.0.2/up42/main.py` & `up42_py-1.0.3/up42/main.py`

 * *Files identical despite different names*

### Comparing `up42_py-1.0.2/up42/order.py` & `up42_py-1.0.3/up42/order.py`

 * *Files identical despite different names*

### Comparing `up42_py-1.0.2/up42/storage.py` & `up42_py-1.0.3/up42/storage.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 import geojson  # type: ignore
 import geopandas  # type: ignore
 from shapely import geometry as shp_geometry  # type: ignore
 
 from up42 import asset, asset_searcher
 from up42 import auth as up42_auth
-from up42 import host, order, stac_client, utils
+from up42 import host, order, utils
 
 logger = utils.get_logger(__name__)
 
 
 class AllowedStatuses(enum.Enum):
     CREATED = "CREATED"
     BEING_PLACED = "BEING_PLACED"
@@ -44,26 +44,31 @@
         self.workspace_id = auth.workspace_id
 
     def __repr__(self):
         return f"Storage(workspace_id: {self.workspace_id})"
 
     @property
     def pystac_client(self):
-        url = host.endpoint("/v2/assets/stac")
-        pystac_client_auth = stac_client.PySTACAuthClient(auth=self.auth).open(url=url)
-        return pystac_client_auth
+        return utils.stac_client(self.auth.client.auth)
 
     def get_assets(
         self,
         created_after: Optional[Union[str, datetime.datetime]] = None,
         created_before: Optional[Union[str, datetime.datetime]] = None,
         acquired_after: Optional[Union[str, datetime.datetime]] = None,
         acquired_before: Optional[Union[str, datetime.datetime]] = None,
         geometry: Optional[
-            Union[dict, geojson.Feature, geojson.FeatureCollection, list, geopandas.GeoDataFrame, shp_geometry.Polygon]
+            Union[
+                dict,
+                geojson.Feature,
+                geojson.FeatureCollection,
+                list,
+                geopandas.GeoDataFrame,
+                shp_geometry.Polygon,
+            ]
         ] = None,
         workspace_id: Optional[str] = None,
         collection_names: Optional[List[str]] = None,
         producer_names: Optional[List[str]] = None,
         tags: Optional[List[str]] = None,
         sources: Optional[List[str]] = None,
         search: Optional[str] = None,
```

### Comparing `up42_py-1.0.2/up42/tasking.py` & `up42_py-1.0.3/up42/tasking.py`

 * *Files identical despite different names*

### Comparing `up42_py-1.0.2/up42/tools.py` & `up42_py-1.0.3/up42/tools.py`

 * *Files identical despite different names*

### Comparing `up42_py-1.0.2/up42/utils.py` & `up42_py-1.0.3/up42/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,24 +5,27 @@
 import json
 import logging
 import pathlib
 import tarfile
 import tempfile
 import warnings
 import zipfile
-from typing import List, Optional, Union, cast
+from typing import Callable, List, Optional, Union, cast
 from urllib import parse
 
 import geojson  # type: ignore
 import geopandas  # type: ignore
+import pystac_client
 import requests
 import shapely  # type: ignore
 import tqdm
 from shapely import geometry  # type: ignore
 
+from up42 import host
+
 TIMEOUT = 120  # seconds
 CHUNK_SIZE = 1024
 
 
 def get_filename(signed_url: str, default_filename: str) -> str:
     """
     Returns the filename from the signed URL
@@ -407,7 +410,17 @@
     if path_or_dict and isinstance(path_or_dict, (str, pathlib.Path)):
         try:
             with open(path_or_dict, encoding="utf-8") as file:
                 return json.load(file)
         except FileNotFoundError as ex:
             raise ValueError(f"File {path_or_dict} does not exist!") from ex
     return cast(Optional[dict], path_or_dict)
+
+
+def stac_client(auth: requests.auth.AuthBase):
+    # pystac client accepts both returning and non-returning request modifiers
+    # requests.auth.AuthBase is a returning request modifier interface
+    request_modifier = cast(Callable[[requests.Request], Optional[requests.Request]], auth)
+    return pystac_client.Client.open(
+        url=host.endpoint("/v2/assets/stac/"),
+        request_modifier=request_modifier,
+    )
```

### Comparing `up42_py-1.0.2/up42/webhooks.py` & `up42_py-1.0.3/up42/webhooks.py`

 * *Files identical despite different names*

### Comparing `up42_py-1.0.2/PKG-INFO` & `up42_py-1.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: up42-py
-Version: 1.0.2
+Version: 1.0.3
 Summary: Python SDK for UP42, the geospatial marketplace and developer platform.
 License: https://github.com/up42/up42-py/blob/master/LICENSE
 Author: UP42 GmbH
 Author-email: support@up42.com
 Requires-Python: >=3.9,<4
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -17,14 +17,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: geojson (==3.1.0)
 Requires-Dist: geopandas (>=0.13.2,<0.14.0)
 Requires-Dist: pyproj (>=3.6.1,<4.0.0)
 Requires-Dist: pystac-client (>=0.7.2,<0.8.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: tenacity (>=8.3.0,<9.0.0)
 Requires-Dist: tqdm (>=4.66.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 <p align="center">
     <strong>Python SDK for UP42, the geospatial marketplace and developer platform.</strong>
 </p>
```

#### html2text {}

```diff
@@ -1,21 +1,22 @@
-Metadata-Version: 2.1 Name: up42-py Version: 1.0.2 Summary: Python SDK for
+Metadata-Version: 2.1 Name: up42-py Version: 1.0.3 Summary: Python SDK for
 UP42, the geospatial marketplace and developer platform. License: https://
 github.com/up42/up42-py/blob/master/LICENSE Author: UP42 GmbH Author-email:
 support@up42.com Requires-Python: >=3.9,<4 Classifier: Development Status :: 4
 - Beta Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: MIT License Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent Classifier: Programming Language
 :: Python :: 3 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Requires-
 Dist: geojson (==3.1.0) Requires-Dist: geopandas (>=0.13.2,<0.14.0) Requires-
 Dist: pyproj (>=3.6.1,<4.0.0) Requires-Dist: pystac-client (>=0.7.2,<0.8.0)
-Requires-Dist: requests (>=2.31.0,<3.0.0) Requires-Dist: tqdm (>=4.66.0,<5.0.0)
-Description-Content-Type: text/markdown
+Requires-Dist: requests (>=2.31.0,<3.0.0) Requires-Dist: tenacity
+(>=8.3.0,<9.0.0) Requires-Dist: tqdm (>=4.66.0,<5.0.0) Description-Content-
+Type: text/markdown
     PPyytthhoonn SSDDKK ffoorr UUPP4422,, tthhee ggeeoossppaattiiaall mmaarrkkeettppllaaccee aanndd ddeevveellooppeerr ppllaattffoorrmm..
 ![](docs/assets/github-banner-3.jpg)
       _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/_u_p_4_2_-_p_y_?_c_o_l_o_r_=_b_r_i_g_h_t_g_r_e_e_n_][https://
 sonarcloud.io/api/project_badges/measure?project=up42_up42-py&metric=coverage]
         _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_t_w_i_t_t_e_r_/_f_o_l_l_o_w_/_U_P_4_2___._s_v_g_?_s_t_y_l_e_=_s_o_c_i_a_l_]
                 _DD_oo_cc_uu_mm_ee_nn_tt_aa_tt_ii_oo_nn ?  ?â??¢ ?  _UU_PP_44_22_.._cc_oo_mm ?  ?â??¢ ?  _SS_uu_pp_pp_oo_rr_tt
 ## Highlights - Python package for easy access to [UP42's](http://www.up42.com)
```

