# Comparing `tmp/felt_python-0.0.1.tar.gz` & `tmp/felt_python-0.0.2.tar.gz`

## Comparing `felt_python-0.0.1.tar` & `felt_python-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,16 @@
--rw-r--r--   0        0        0     7794 2020-02-02 00:00:00.000000 felt_python-0.0.1/testing.ipynb
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 felt_python-0.0.1/felt_python/__init__.py
--rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 felt_python-0.0.1/felt_python/api.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 felt_python-0.0.1/felt_python/exceptions.py
--rw-r--r--   0        0        0     4440 2020-02-02 00:00:00.000000 felt_python-0.0.1/felt_python/layers.py
--rw-r--r--   0        0        0     1204 2020-02-02 00:00:00.000000 felt_python-0.0.1/felt_python/maps.py
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 felt_python-0.0.1/tests/fixtures/null-island-points-sample.geojson
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 felt_python-0.0.1/tests/fixtures/null-island-points.geojson
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 felt_python-0.0.1/.gitignore
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 felt_python-0.0.1/LICENSE
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 felt_python-0.0.1/README.md
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 felt_python-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 felt_python-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     4140 2020-02-02 00:00:00.000000 felt_python-0.0.2/testing_elements.ipynb
+-rw-r--r--   0        0        0     7097 2020-02-02 00:00:00.000000 felt_python-0.0.2/testing_layers.ipynb
+-rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 felt_python-0.0.2/felt_python/__init__.py
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 felt_python-0.0.2/felt_python/api.py
+-rw-r--r--   0        0        0     1998 2020-02-02 00:00:00.000000 felt_python-0.0.2/felt_python/elements.py
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 felt_python-0.0.2/felt_python/exceptions.py
+-rw-r--r--   0        0        0     4683 2020-02-02 00:00:00.000000 felt_python-0.0.2/felt_python/layers.py
+-rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 felt_python-0.0.2/felt_python/maps.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 felt_python-0.0.2/tests/fixtures/null-island-points-sample.geojson
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 felt_python-0.0.2/tests/fixtures/null-island-points.geojson
+-rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 felt_python-0.0.2/tests/fixtures/null-island-polygons-wkt.csv
+-rw-r--r--   0        0        0     3088 2020-02-02 00:00:00.000000 felt_python-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 felt_python-0.0.2/LICENSE
+-rw-r--r--   0        0        0     2293 2020-02-02 00:00:00.000000 felt_python-0.0.2/README.md
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 felt_python-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2948 2020-02-02 00:00:00.000000 felt_python-0.0.2/PKG-INFO
```

### Comparing `felt_python-0.0.1/testing.ipynb` & `felt_python-0.0.2/testing_layers.ipynb`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.969167751736111%*

 * *Differences: {"'cells'": "{0: {'source': ['# Testing Layers']}, 1: {'source': {insert: [(10, '    "*

 * *            "upload_geodataframe,\\n'), (13, '    get_layer_details,\\n'), (17, "*

 * *            '\'os.environ["FELT_API_TOKEN"] = "<YOUR_API_TOKEN>"\')], delete: [16, 12]}}, 7: '*

 * *            "{'source': ['layer_resp = upload_file(map_id, "*

 * *            '"tests/fixtures/null-island-points-sample.geojson", "The Points Layer")\\n\', '*

 * *            '\'layer_id = layer_resp["attributes"]["first_layer_id"]\']}, 8: {\'cell_type\': ' […]*

```diff
@@ -1,15 +1,15 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
             "id": "a8c2b3f0-9f10-414c-8a55-964721167c97",
             "metadata": {},
             "source": [
-                "# Testing felt-python"
+                "# Testing Layers"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "fc85a763-cd96-4eab-85d1-d82adfe0eea1",
             "metadata": {},
@@ -21,21 +21,22 @@
                 "    create_map,\n",
                 "    delete_map,\n",
                 "    get_map_details,\n",
                 "    list_layers,\n",
                 "    upload_file,\n",
                 "    upload_url,\n",
                 "    upload_dataframe,\n",
+                "    upload_geodataframe,\n",
                 "    refresh_file_layer,\n",
                 "    refresh_url_layer,\n",
-                "    get_layer_style,\n",
+                "    get_layer_details,\n",
                 "    update_layer_style\n",
                 ")\n",
                 "\n",
-                "os.environ[\"FELT_API_TOKEN\"] = \"felt_pat_wZOSz45T+BoT89uRzfeu3eRQkUj9iQxvXplMSU8Erpo\""
+                "os.environ[\"FELT_API_TOKEN\"] = \"<YOUR_API_TOKEN>\""
             ]
         },
         {
             "cell_type": "markdown",
             "id": "d902938d-78e3-4d2b-97a2-1c63e5662083",
             "metadata": {},
             "source": [
@@ -77,104 +78,70 @@
             "source": [
                 "# Layers\n",
                 "\n",
                 "Create layers from file, URL and (Geo)DataFrame uploads"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "36b3e73b-2b38-444d-8be2-d05b1605f4b8",
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "map_id"
-            ]
-        },
-        {
             "cell_type": "markdown",
             "id": "ba8dc97e-7c91-4e61-b7a7-ea86892cc046",
             "metadata": {},
             "source": [
                 "## Upload a file"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "bd6045fa-a226-4072-8e4a-924470638347",
             "metadata": {},
             "outputs": [],
             "source": [
-                "layer_resp = upload_file(map_id, \"tests/fixtures/null-island-points-sample.geojson\", \"The Points Layer\")"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "85caab2b-149d-48ae-abef-d08ab8682ddb",
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "# Ideally, the new layer ID would be present here\n",
-                "layer_resp.content"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "1e50cb62-00de-4a7e-8a5e-119003e56549",
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "# Let's fetch it\n",
-                "layers = list_layers(map_id)"
+                "layer_resp = upload_file(map_id, \"tests/fixtures/null-island-points-sample.geojson\", \"The Points Layer\")\n",
+                "layer_id = layer_resp[\"attributes\"][\"first_layer_id\"]"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "76d5735c-ddba-46a8-9b9c-24ac1d4b1e59",
+            "cell_type": "markdown",
+            "id": "62dd0688",
             "metadata": {},
-            "outputs": [],
             "source": [
-                "layer_id = layers[0][\"id\"]"
+                "# Check upload status"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "414b4e92-7c1a-4693-bd7c-748fc40e56ba",
+            "id": "39488500",
             "metadata": {},
             "outputs": [],
             "source": [
-                "layer_id"
+                "get_layer_details(map_id, layer_id)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "050e2bc0-30e4-4f4b-83cf-9e22f91df1e8",
             "metadata": {},
             "source": [
-                "## Attempt to refresh file upload\n",
+                "### Refresh file upload\n",
                 "\n",
-                "**Note**: Refreshing here fails because `list_layers` and `url_import` return layer group IDs but the v1 refresh endpoints need _layer_ IDs. Styling works with both layer IDs _and_ layer group IDs which explains the mismatch"
+                "Wait for upload to finish first"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "22190774-d547-4802-bc68-c71d38ef8968",
             "metadata": {
                 "scrolled": true
             },
             "outputs": [],
             "source": [
-                "# Refresh not working, always says layer_id not found\n",
-                "# refresh_file_layer(map_id, layer_id, file_name=\"tests/fixtures/null-island-points.geojson\")"
+                "refresh_file_layer(map_id, layer_id, file_name=\"tests/fixtures/null-island-points.geojson\")"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "1d33a1eb-6c8a-471f-b1a7-f83bac440db0",
             "metadata": {},
             "source": [
@@ -186,43 +153,35 @@
             "execution_count": null,
             "id": "07d46bab-6721-451e-8f63-83017f2cf974",
             "metadata": {},
             "outputs": [],
             "source": [
                 "live_earthquakes_url = \"https://earthquake.usgs.gov/earthquakes/feed/v1.0/summary/all_hour.geojson\"\n",
                 "url_upload = upload_url(map_id, live_earthquakes_url, \"Live Earthquakes\")\n",
-                "url_upload_id = url_upload[\"relationships\"][\"datasets\"][\"data\"][0][\"id\"]"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "id": "9293ceca-391d-4003-a3b8-dea79a74657b",
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "url_upload"
+                "url_layer_id = url_upload[\"attributes\"][\"first_layer_id\"]"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "feaa457c-9695-4451-a783-45bb476e1574",
             "metadata": {},
             "source": [
-                "Refreshing works this time because we've fetched the layer ID instead of the layer group ID"
+                "### Refresh URL upload\n",
+                "\n",
+                "Wait for upload to finish first"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "a7021996-4d4a-4276-89e0-88e8d501bfe0",
             "metadata": {},
             "outputs": [],
             "source": [
-                "refresh_url_layer(map_id, url_upload_id)"
+                "refresh_url_layer(map_id, url_layer_id)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "adc9d25b-a64c-4c7d-8463-20d13dcad10a",
             "metadata": {},
             "source": [
@@ -240,15 +199,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "6519d2bb-6223-490b-9eee-7e0d54052092",
             "metadata": {},
             "outputs": [],
             "source": [
-                "current_style = get_layer_style(map_id, layer_id)\n",
+                "current_style = get_layer_details(map_id, layer_id)[\"attributes\"][\"style\"]\n",
                 "current_style"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "c37f77cc-fcba-4906-a76c-23ad51abd618",
             "metadata": {},
@@ -270,39 +229,59 @@
             ]
         },
         {
             "cell_type": "markdown",
             "id": "1649c24f-845b-4144-b710-45ff72852c18",
             "metadata": {},
             "source": [
-                "# (Geo)DataFrames"
+                "# DataFrames and GeoDataFrames"
+            ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": null,
+            "id": "f96b00c0",
+            "metadata": {},
+            "outputs": [],
+            "source": [
+                "import pandas as pd\n",
+                "\n",
+                "df = pd.read_csv(\"tests/fixtures/null-island-polygons-wkt.csv\")\n",
+                "upload_dataframe(map_id, df, \"Polygons from a CSV\")"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "6db22864-1ebd-4b3d-9aec-7594e856b5a0",
             "metadata": {},
             "outputs": [],
             "source": [
                 "import geopandas as gpd\n",
                 "\n",
-                "gdf = gpd.read_file('tests/fixtures/null-island-points.geojson')"
+                "gdf = gpd.read_file('tests/fixtures/null-island-points.geojson')\n",
+                "upload_geodataframe(map_id, gdf, layer_name=\"GeoPandas Upload\")"
+            ]
+        },
+        {
+            "cell_type": "markdown",
+            "id": "0176c22b",
+            "metadata": {},
+            "source": [
+                "## List all uploaded layers"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
-            "id": "9b75184e-f2be-4bc6-8ba7-ba1e2812d6a6",
-            "metadata": {
-                "scrolled": true
-            },
+            "id": "32bfb2c2",
+            "metadata": {},
             "outputs": [],
             "source": [
-                "upload_dataframe(map_id, gdf, layer_name=\"GeoPandas FTW\")"
+                "list_layers(map_id)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "e3574d06-bfbd-46bc-a86e-b70be7167cbf",
             "metadata": {},
             "source": [
```

### Comparing `felt_python-0.0.1/felt_python/__init__.py` & `felt_python-0.0.2/felt_python/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,21 +5,29 @@
     get_map_details,
     update_map,
 )
 from felt_python.exceptions import AuthError
 from felt_python.layers import (
     list_layers,
     upload_file,
+    upload_geodataframe,
     upload_dataframe,
     upload_url,
     refresh_file_layer,
     refresh_url_layer,
-    get_layer_style,
+    get_layer_details,
     update_layer_style,
 )
+from felt_python.elements import (
+    list_elements,
+    list_element_groups,
+    list_elements_in_group,
+    post_elements,
+    delete_element,
+)
 
 __doc__ = """
 The official Python client for the Felt API
 ===========================================
 
 **felt-python** is a Python client for the Felt API. It provides convenient wrappers for
 common operations like creating, deleting and updating maps and data layers.
@@ -31,15 +39,21 @@
 __all__ = [
     "create_map",
     "delete_map",
     "get_map_details",
     "update_map",
     "list_layers",
     "upload_file",
+    "upload_geodataframe",
     "upload_dataframe",
     "upload_url",
     "refresh_file_layer",
     "refresh_url_layer",
-    "get_layer_style",
+    "get_layer_details",
     "update_layer_style",
     "AuthError",
+    "list_elements",
+    "list_element_groups",
+    "list_elements_in_group",
+    "post_elements",
+    "delete_element",
 ]
```

### Comparing `felt_python-0.0.1/felt_python/api.py` & `felt_python-0.0.2/felt_python/api.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,49 +1,52 @@
+"""Wrapper for API calls using requests"""
 import os
-import requests
 import typing
 
 from urllib.parse import urljoin
 
+import requests
+
 from uritemplate import URITemplate
 
 from .exceptions import AuthError
 
 
-V1_URL = "https://felt.com/api/v1/"
-V2_URL = "https://felt.com/api/v2/"
-MAPS_TEMPLATE = URITemplate(urljoin(V2_URL, "maps{/map_id}"))
-LAYERS_TEMPLATE = URITemplate(urljoin(V1_URL, "maps{/map_id}/layers{/layer_id}"))
-UPLOAD_TEMPLATE = URITemplate(urljoin(V2_URL, "maps{/map_id}/upload"))
-URL_IMPORT_TEMPLATE = URITemplate(urljoin(V1_URL, "maps{/map_id}/layers/url_import"))
-REFRESH_FILE_TEMPLATE = URITemplate(
-    urljoin(V1_URL, "maps{/map_id}/refresh{/layer_id}/file")
+BASE_URL = "https://felt.com/api/v2/"
+MAPS_TEMPLATE = URITemplate(urljoin(BASE_URL, "maps{/map_id}"))
+LAYERS_TEMPLATE = URITemplate(urljoin(BASE_URL, "maps{/map_id}/layers{/layer_id}"))
+UPLOAD_TEMPLATE = URITemplate(urljoin(BASE_URL, "maps{/map_id}/upload"))
+REFRESH_TEMPLATE = URITemplate(
+    urljoin(BASE_URL, "maps{/map_id}/layers{/layer_id}/refresh")
+)
+UPDATE_STYLE_TEMPLATE = URITemplate(
+    urljoin(BASE_URL, "maps{/map_id}/layers{/layer_id}/update_style")
 )
-REFRESH_URL_TEMPLATE = URITemplate(
-    urljoin(V1_URL, "maps{/map_id}/refresh{/layer_id}/url")
+ELEMENTS_TEMPLATE = URITemplate(
+    urljoin(BASE_URL, "maps{/map_id}/elements{/element_id}")
 )
-LAYER_STYLE_TEMPLATE = URITemplate(
-    urljoin(V1_URL, "maps{/map_id}/layers{/layer_id}/style")
+ELEMENT_GROUPS_TEMPLATE = URITemplate(
+    urljoin(BASE_URL, "maps{/map_id}/element_groups{/element_group_id}")
 )
 
 
 def make_request(
     url: str,
     method: typing.Union[requests.get, requests.post, requests.patch, requests.delete],
     params: dict | None = None,
     json: dict | None = None,
     api_token: str | None = None,
 ):
     """Basic wrapper for requests that adds auth"""
     if not api_token:
         try:
             api_token = os.environ["FELT_API_TOKEN"]
-        except KeyError:
+        except KeyError as exc:
             raise AuthError(
                 "No API token found. Pass explicitly or set the FELT_API_TOKEN environment variable"
-            )
+            ) from exc
 
     headers = {"Authorization": f"Bearer {api_token}"}
     response = method(url, params=params, json=json, headers=headers)
     if not response.ok:
         raise Exception(f"Request failed: {response.content}")
     return response
```

### Comparing `felt_python-0.0.1/felt_python/layers.py` & `felt_python-0.0.2/felt_python/layers.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,19 @@
 """Layers"""
-import json
 import os
 import tempfile
 
-import geopandas as gpd
-import pandas as pd
 import requests
 
 from .api import (
     make_request,
     LAYERS_TEMPLATE,
-    URL_IMPORT_TEMPLATE,
-    REFRESH_FILE_TEMPLATE,
-    REFRESH_URL_TEMPLATE,
+    REFRESH_TEMPLATE,
+    UPDATE_STYLE_TEMPLATE,
     UPLOAD_TEMPLATE,
-    LAYER_STYLE_TEMPLATE,
 )
 
 
 def list_layers(map_id: str, api_token: str | None = None):
     """List layers on a map"""
     response = make_request(
         url=LAYERS_TEMPLATE.expand(map_id=map_id),
@@ -30,124 +25,141 @@
 
 def _request_and_upload(
     url: str,
     file_name: str,
     layer_name: str | None = None,
     api_token: str | None = None,
 ):
-    """Upload or refresh a file"""
-    json_payload = {"file_names": [file_name]}
-    if layer_name:
-        json_payload["name"] = layer_name
+    """Upload or refresh a file
+
+    Both upload_file and refresh_file_layer use this function to handle the
+    request and file upload. The only difference is that the upload endpoint
+    requires a layer name while the refresh endpoint does not.
+    """
+    json_payload = {"name": layer_name} if layer_name else None
     layer_response = make_request(
         url=url, method=requests.post, api_token=api_token, json=json_payload
     )
     presigned_upload = layer_response.json()
 
     url = presigned_upload["data"]["attributes"]["url"]
     presigned_attributes = presigned_upload["data"]["attributes"][
         "presigned_attributes"
     ]
     with open(file_name, "rb") as file_obj:
-        output = requests.post(
+        requests.post(
             url,
             # Order is important, file should come at the end
             files={**presigned_attributes, "file": file_obj},
         )
-    return output
+    return layer_response.json()["data"]
 
 
 def upload_file(
     map_id: str,
     file_name: str,
-    layer_name: str | None = None,
+    layer_name: str,
     api_token: str | None = None,
 ):
     """Upload a file to a Felt map"""
     return _request_and_upload(
         url=UPLOAD_TEMPLATE.expand(map_id=map_id),
         file_name=file_name,
         layer_name=layer_name,
         api_token=api_token,
     )
 
 
 def upload_dataframe(
     map_id: str,
-    dataframe: pd.DataFrame | gpd.GeoDataFrame,
-    layer_name: str | None = None,
+    dataframe: "pd.DataFrame",
+    layer_name: str,
     api_token: str | None = None,
 ):
-    """Upload a (Geo)Pandas (Geo)DataFrame to a Felt map"""
+    """Upload a Pandas DataFrame to a Felt map"""
     with tempfile.TemporaryDirectory() as tempdir:
-        if isinstance(dataframe, gpd.GeoDataFrame):
-            file_name = os.path.join(tempdir, "geodataframe.gpkg")
-            dataframe.to_file(file_name)
-        else:
-            file_name = os.path.join(tempdir, "dataframe.csv")
-            dataframe.to_csv(file_name)
+        file_name = os.path.join(tempdir, "dataframe.csv")
+        dataframe.to_csv(file_name)
+        return upload_file(
+            map_id,
+            file_name,
+            layer_name,
+            api_token,
+        )
+
+
+def upload_geodataframe(
+    map_id: str,
+    geodataframe: "gpd.GeoDataFrame",
+    layer_name: str,
+    api_token: str | None = None,
+):
+    """Upload a GeoPandas GeoDataFrame to a Felt map"""
+    with tempfile.TemporaryDirectory() as tempdir:
+        file_name = os.path.join(tempdir, "geodataframe.gpkg")
+        geodataframe.to_file(file_name)
         return upload_file(
             map_id,
             file_name,
             layer_name,
             api_token,
         )
 
 
 def refresh_file_layer(
     map_id: str, layer_id: str, file_name: str, api_token: str | None = None
 ):
     """Refresh a layer originated from a file upload"""
     return _request_and_upload(
-        url=REFRESH_FILE_TEMPLATE.expand(map_id=map_id, layer_id=layer_id),
+        url=REFRESH_TEMPLATE.expand(map_id=map_id, layer_id=layer_id),
         file_name=file_name,
         api_token=api_token,
     )
 
 
 def upload_url(
     map_id: str,
     layer_url: str,
-    layer_name: str | None = None,
+    layer_name: str,
     api_token: str | None = None,
 ):
     """Upload a URL to a Felt map"""
-    json_payload = {"layer_url": layer_url}
-    if layer_name:
-        json_payload["name"] = layer_name
     layer_response = make_request(
-        url=URL_IMPORT_TEMPLATE.expand(map_id=map_id),
+        url=UPLOAD_TEMPLATE.expand(map_id=map_id),
         method=requests.post,
         api_token=api_token,
-        json=json_payload,
+        json={
+            "import_url": layer_url,
+            "name": layer_name,
+        },
     )
     return layer_response.json()["data"]
 
 
 def refresh_url_layer(map_id: str, layer_id: str, api_token: str | None = None):
     """Refresh a layer originated from a URL upload"""
     layer_response = make_request(
-        url=REFRESH_URL_TEMPLATE.expand(
+        url=REFRESH_TEMPLATE.expand(
             map_id=map_id,
             layer_id=layer_id,
         ),
         method=requests.post,
         api_token=api_token,
     )
     return layer_response.json()["data"]
 
 
-def get_layer_style(
+def get_layer_details(
     map_id: str,
     layer_id: str,
     api_token: str | None = None,
 ):
     """Get style of a layer"""
     response = make_request(
-        url=LAYER_STYLE_TEMPLATE.expand(
+        url=LAYERS_TEMPLATE.expand(
             map_id=map_id,
             layer_id=layer_id,
         ),
         method=requests.get,
         api_token=api_token,
     )
     return response.json()["data"]
@@ -157,16 +169,16 @@
     map_id: str,
     layer_id: str,
     style: dict,
     api_token: str | None = None,
 ):
     """Style a layer"""
     response = make_request(
-        url=LAYER_STYLE_TEMPLATE.expand(
+        url=UPDATE_STYLE_TEMPLATE.expand(
             map_id=map_id,
             layer_id=layer_id,
         ),
-        method=requests.patch,
-        json={"style": json.dumps(style)},
+        method=requests.post,
+        json={"style": style},
         api_token=api_token,
     )
     return response.json()["data"]
```

### Comparing `felt_python-0.0.1/felt_python/maps.py` & `felt_python-0.0.2/felt_python/maps.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         api_token=api_token,
     )
     return response.json()["data"]
 
 
 def delete_map(map_id: str, api_token: str | None = None):
     """Delete a map"""
-    response = make_request(
+    make_request(
         url=MAPS_TEMPLATE.expand(map_id=map_id),
         method=requests.delete,
         api_token=api_token,
     )
 
 
 def get_map_details(map_id: str, api_token: str | None = None):
```

### Comparing `felt_python-0.0.1/tests/fixtures/null-island-points-sample.geojson` & `felt_python-0.0.2/tests/fixtures/null-island-points-sample.geojson`

 * *Files identical despite different names*

### Comparing `felt_python-0.0.1/tests/fixtures/null-island-points.geojson` & `felt_python-0.0.2/tests/fixtures/null-island-points.geojson`

 * *Files identical despite different names*

### Comparing `felt_python-0.0.1/.gitignore` & `felt_python-0.0.2/.gitignore`

 * *Files 4% similar despite different names*

```diff
@@ -154,7 +154,9 @@
 
 # PyCharm
 #  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 #.idea/
+
+.DS_Store
```

### Comparing `felt_python-0.0.1/LICENSE` & `felt_python-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `felt_python-0.0.1/pyproject.toml` & `felt_python-0.0.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 
 [project]
 name = "felt-python"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Álvaro Arredondo", email="alvaro@felt.com" },
   { name="Chris Loer", email="chris@felt.com" },
 ]
 description = "The official Felt API client library"
 readme = "README.md"
 requires-python = ">=3.6"
 dependencies = [
-  "geopandas",
-  "pandas",
   "requests",
   "uritemplate",
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

