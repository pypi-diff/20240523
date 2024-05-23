# Comparing `tmp/dagster-embedded-elt-0.23.6.tar.gz` & `tmp/dagster-embedded-elt-0.23.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-embedded-elt-0.23.6.tar", last modified: Thu May 16 20:12:27 2024, max compression
+gzip compressed data, was "dagster-embedded-elt-0.23.7.tar", last modified: Thu May 23 20:56:30 2024, max compression
```

## Comparing `dagster-embedded-elt-0.23.6.tar` & `dagster-embedded-elt-0.23.7.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:12:27.699878 dagster-embedded-elt-0.23.6/
--rw-r--r--   0 root         (0) root         (0)    11349 2024-05-16 20:06:23.000000 dagster-embedded-elt-0.23.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)       97 2024-05-16 20:06:23.000000 dagster-embedded-elt-0.23.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      744 2024-05-16 20:12:27.699878 dagster-embedded-elt-0.23.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      146 2024-05-16 20:06:23.000000 dagster-embedded-elt-0.23.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:12:27.695878 dagster-embedded-elt-0.23.6/dagster_embedded_elt/
--rw-r--r--   0 root         (0) root         (0)      163 2024-05-16 20:06:23.000000 dagster-embedded-elt-0.23.6/dagster_embedded_elt/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:12:27.699878 dagster-embedded-elt-0.23.6/dagster_embedded_elt/dlt/
--rw-r--r--   0 root         (0) root         (0)      270 2024-05-16 20:06:23.000000 dagster-embedded-elt-0.23.6/dagster_embedded_elt/dlt/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3947 2024-05-16 20:06:23.000000 dagster-embedded-elt-0.23.6/dagster_embedded_elt/dlt/asset_decorator.py
--rw-r--r--   0 root         (0) root         (0)      129 2024-05-16 20:06:23.000000 dagster-embedded-elt-0.23.6/dagster_embedded_elt/dlt/constants.py
--rw-r--r--   0 root         (0) root         (0)     7033 2024-05-16 20:06:23.000000 dagster-embedded-elt-0.23.6/dagster_embedded_elt/dlt/resource.py
--rw-r--r--   0 root         (0) root         (0)     1563 2024-05-16 20:06:23.000000 dagster-embedded-elt-0.23.6/dagster_embedded_elt/dlt/translator.py
--rw-r--r--   0 root         (0) root         (0)        8 2024-05-16 20:06:23.000000 dagster-embedded-elt-0.23.6/dagster_embedded_elt/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:12:27.699878 dagster-embedded-elt-0.23.6/dagster_embedded_elt/sling/
--rw-r--r--   0 root         (0) root         (0)      718 2024-05-16 20:06:23.000000 dagster-embedded-elt-0.23.6/dagster_embedded_elt/sling/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5804 2024-05-16 20:06:23.000000 dagster-embedded-elt-0.23.6/dagster_embedded_elt/sling/asset_decorator.py
--rw-r--r--   0 root         (0) root         (0)     4162 2024-05-16 20:06:23.000000 dagster-embedded-elt-0.23.6/dagster_embedded_elt/sling/asset_defs.py
--rw-r--r--   0 root         (0) root         (0)     8087 2024-05-16 20:06:23.000000 dagster-embedded-elt-0.23.6/dagster_embedded_elt/sling/dagster_sling_translator.py
--rw-r--r--   0 root         (0) root         (0)    20594 2024-05-16 20:06:23.000000 dagster-embedded-elt-0.23.6/dagster_embedded_elt/sling/resources.py
--rw-r--r--   0 root         (0) root         (0)     1106 2024-05-16 20:06:23.000000 dagster-embedded-elt-0.23.6/dagster_embedded_elt/sling/sling_replication.py
--rw-r--r--   0 root         (0) root         (0)       23 2024-05-16 20:06:23.000000 dagster-embedded-elt-0.23.6/dagster_embedded_elt/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:12:27.695878 dagster-embedded-elt-0.23.6/dagster_embedded_elt.egg-info/
--rw-r--r--   0 root         (0) root         (0)      744 2024-05-16 20:12:27.000000 dagster-embedded-elt-0.23.6/dagster_embedded_elt.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      886 2024-05-16 20:12:27.000000 dagster-embedded-elt-0.23.6/dagster_embedded_elt.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-16 20:12:27.000000 dagster-embedded-elt-0.23.6/dagster_embedded_elt.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-16 20:12:27.000000 dagster-embedded-elt-0.23.6/dagster_embedded_elt.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       52 2024-05-16 20:12:27.000000 dagster-embedded-elt-0.23.6/dagster_embedded_elt.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       21 2024-05-16 20:12:27.000000 dagster-embedded-elt-0.23.6/dagster_embedded_elt.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      124 2024-05-16 20:06:23.000000 dagster-embedded-elt-0.23.6/integration.yaml
--rw-r--r--   0 root         (0) root         (0)      167 2024-05-16 20:12:27.699878 dagster-embedded-elt-0.23.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1427 2024-05-16 20:06:23.000000 dagster-embedded-elt-0.23.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:56:30.176526 dagster-embedded-elt-0.23.7/
+-rw-r--r--   0 root         (0) root         (0)    11349 2024-05-23 20:50:32.000000 dagster-embedded-elt-0.23.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       97 2024-05-23 20:50:32.000000 dagster-embedded-elt-0.23.7/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      744 2024-05-23 20:56:30.176526 dagster-embedded-elt-0.23.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      146 2024-05-23 20:50:32.000000 dagster-embedded-elt-0.23.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:56:30.176526 dagster-embedded-elt-0.23.7/dagster_embedded_elt/
+-rw-r--r--   0 root         (0) root         (0)      163 2024-05-23 20:50:32.000000 dagster-embedded-elt-0.23.7/dagster_embedded_elt/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:56:30.176526 dagster-embedded-elt-0.23.7/dagster_embedded_elt/dlt/
+-rw-r--r--   0 root         (0) root         (0)      270 2024-05-23 20:50:32.000000 dagster-embedded-elt-0.23.7/dagster_embedded_elt/dlt/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3947 2024-05-23 20:50:32.000000 dagster-embedded-elt-0.23.7/dagster_embedded_elt/dlt/asset_decorator.py
+-rw-r--r--   0 root         (0) root         (0)      129 2024-05-23 20:50:32.000000 dagster-embedded-elt-0.23.7/dagster_embedded_elt/dlt/constants.py
+-rw-r--r--   0 root         (0) root         (0)     7076 2024-05-23 20:50:32.000000 dagster-embedded-elt-0.23.7/dagster_embedded_elt/dlt/resource.py
+-rw-r--r--   0 root         (0) root         (0)     1563 2024-05-23 20:50:32.000000 dagster-embedded-elt-0.23.7/dagster_embedded_elt/dlt/translator.py
+-rw-r--r--   0 root         (0) root         (0)        8 2024-05-23 20:50:32.000000 dagster-embedded-elt-0.23.7/dagster_embedded_elt/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:56:30.176526 dagster-embedded-elt-0.23.7/dagster_embedded_elt/sling/
+-rw-r--r--   0 root         (0) root         (0)      718 2024-05-23 20:50:32.000000 dagster-embedded-elt-0.23.7/dagster_embedded_elt/sling/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6011 2024-05-23 20:50:32.000000 dagster-embedded-elt-0.23.7/dagster_embedded_elt/sling/asset_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     4162 2024-05-23 20:50:32.000000 dagster-embedded-elt-0.23.7/dagster_embedded_elt/sling/asset_defs.py
+-rw-r--r--   0 root         (0) root         (0)     8087 2024-05-23 20:50:32.000000 dagster-embedded-elt-0.23.7/dagster_embedded_elt/sling/dagster_sling_translator.py
+-rw-r--r--   0 root         (0) root         (0)    20594 2024-05-23 20:50:32.000000 dagster-embedded-elt-0.23.7/dagster_embedded_elt/sling/resources.py
+-rw-r--r--   0 root         (0) root         (0)     1106 2024-05-23 20:50:32.000000 dagster-embedded-elt-0.23.7/dagster_embedded_elt/sling/sling_replication.py
+-rw-r--r--   0 root         (0) root         (0)       23 2024-05-23 20:50:32.000000 dagster-embedded-elt-0.23.7/dagster_embedded_elt/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 20:56:30.176526 dagster-embedded-elt-0.23.7/dagster_embedded_elt.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      744 2024-05-23 20:56:29.000000 dagster-embedded-elt-0.23.7/dagster_embedded_elt.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      886 2024-05-23 20:56:29.000000 dagster-embedded-elt-0.23.7/dagster_embedded_elt.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-23 20:56:29.000000 dagster-embedded-elt-0.23.7/dagster_embedded_elt.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-23 20:56:29.000000 dagster-embedded-elt-0.23.7/dagster_embedded_elt.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       52 2024-05-23 20:56:29.000000 dagster-embedded-elt-0.23.7/dagster_embedded_elt.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2024-05-23 20:56:29.000000 dagster-embedded-elt-0.23.7/dagster_embedded_elt.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      124 2024-05-23 20:50:32.000000 dagster-embedded-elt-0.23.7/integration.yaml
+-rw-r--r--   0 root         (0) root         (0)      167 2024-05-23 20:56:30.180526 dagster-embedded-elt-0.23.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1427 2024-05-23 20:50:32.000000 dagster-embedded-elt-0.23.7/setup.py
```

### Comparing `dagster-embedded-elt-0.23.6/LICENSE` & `dagster-embedded-elt-0.23.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-embedded-elt-0.23.6/dagster_embedded_elt/dlt/asset_decorator.py` & `dagster-embedded-elt-0.23.7/dagster_embedded_elt/dlt/asset_decorator.py`

 * *Files identical despite different names*

### Comparing `dagster-embedded-elt-0.23.6/dagster_embedded_elt/dlt/resource.py` & `dagster-embedded-elt-0.23.7/dagster_embedded_elt/dlt/resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -161,16 +161,19 @@
                     for dlt_source_resource in asset_key_dlt_source_resource_mapping.values()
                     if dlt_source_resource
                 ]
             )
 
         load_info = dlt_pipeline.run(dlt_source, **kwargs)
 
+        load_info.raise_on_failed_jobs()
+
         has_asset_def: bool = bool(context and context.has_assets_def)
 
         for asset_key, dlt_source_resource in asset_key_dlt_source_resource_mapping.items():
             metadata = self.extract_resource_metadata(dlt_source_resource, load_info)
+
             if has_asset_def:
                 yield MaterializeResult(asset_key=asset_key, metadata=metadata)
 
             else:
                 yield AssetMaterialization(asset_key=asset_key, metadata=metadata)
```

### Comparing `dagster-embedded-elt-0.23.6/dagster_embedded_elt/dlt/translator.py` & `dagster-embedded-elt-0.23.7/dagster_embedded_elt/dlt/translator.py`

 * *Files identical despite different names*

### Comparing `dagster-embedded-elt-0.23.6/dagster_embedded_elt/sling/__init__.py` & `dagster-embedded-elt-0.23.7/dagster_embedded_elt/sling/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-embedded-elt-0.23.6/dagster_embedded_elt/sling/asset_decorator.py` & `dagster-embedded-elt-0.23.7/dagster_embedded_elt/sling/asset_decorator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from copy import deepcopy
 from typing import Any, Callable, Iterable, Mapping, Optional
 
 from dagster import (
     AssetsDefinition,
     AssetSpec,
     BackfillPolicy,
     PartitionsDefinition,
@@ -36,16 +37,21 @@
     """
     default_dagster_meta = replication_config.get("defaults", {}).get("meta", {}).get("dagster", {})
     if not default_dagster_meta:
         yield from streams
     else:
         for stream in streams:
             name = stream["name"]
-            config = vars(stream["config"])
-            config["meta"] = deep_merge_dicts(default_dagster_meta, config["meta"])
+            config = deepcopy(stream["config"])
+            if not config:
+                config = {"meta": {"dagster": default_dagster_meta}}
+            else:
+                config["meta"] = deep_merge_dicts(
+                    {"dagster": default_dagster_meta}, config.get("meta", {})
+                )
             yield {"name": name, "config": config}
 
 
 def sling_assets(
     *,
     replication_config: SlingReplicationParam,
     dagster_sling_translator: Optional[DagsterSlingTranslator] = None,
```

### Comparing `dagster-embedded-elt-0.23.6/dagster_embedded_elt/sling/asset_defs.py` & `dagster-embedded-elt-0.23.7/dagster_embedded_elt/sling/asset_defs.py`

 * *Files identical despite different names*

### Comparing `dagster-embedded-elt-0.23.6/dagster_embedded_elt/sling/dagster_sling_translator.py` & `dagster-embedded-elt-0.23.7/dagster_embedded_elt/sling/dagster_sling_translator.py`

 * *Files identical despite different names*

### Comparing `dagster-embedded-elt-0.23.6/dagster_embedded_elt/sling/resources.py` & `dagster-embedded-elt-0.23.7/dagster_embedded_elt/sling/resources.py`

 * *Files identical despite different names*

### Comparing `dagster-embedded-elt-0.23.6/dagster_embedded_elt/sling/sling_replication.py` & `dagster-embedded-elt-0.23.7/dagster_embedded_elt/sling/sling_replication.py`

 * *Files identical despite different names*

### Comparing `dagster-embedded-elt-0.23.6/dagster_embedded_elt.egg-info/SOURCES.txt` & `dagster-embedded-elt-0.23.7/dagster_embedded_elt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagster-embedded-elt-0.23.6/setup.py` & `dagster-embedded-elt-0.23.7/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_embedded_elt_tests*"]),
     python_requires=">=3.8,<3.13",
-    install_requires=["dagster==1.7.6", "sling>=1.1.5", "dlt>=0.4"],
+    install_requires=["dagster==1.7.7", "sling>=1.1.5", "dlt>=0.4"],
     zip_safe=False,
     extras_require={
         "test": [
             "duckdb",
         ]
     },
 )
```

