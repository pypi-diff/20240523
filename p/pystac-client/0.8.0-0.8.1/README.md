# Comparing `tmp/pystac_client-0.8.0.tar.gz` & `tmp/pystac_client-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pystac_client-0.8.0.tar", last modified: Fri May 17 14:16:36 2024, max compression
+gzip compressed data, was "pystac_client-0.8.1.tar", last modified: Thu May 23 14:51:14 2024, max compression
```

## Comparing `pystac_client-0.8.0.tar` & `pystac_client-0.8.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:16:36.781440 pystac_client-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-17 14:16:27.000000 pystac_client-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-17 14:16:27.000000 pystac_client-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5104 2024-05-17 14:16:36.781440 pystac_client-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-05-17 14:16:27.000000 pystac_client-0.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-05-17 14:16:27.000000 pystac_client-0.8.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:16:36.777439 pystac_client-0.8.0/pystac_client/
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-17 14:16:27.000000 pystac_client-0.8.0/pystac_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-05-17 14:16:27.000000 pystac_client-0.8.0/pystac_client/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11531 2024-05-17 14:16:27.000000 pystac_client-0.8.0/pystac_client/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    26442 2024-05-17 14:16:27.000000 pystac_client-0.8.0/pystac_client/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     7839 2024-05-17 14:16:27.000000 pystac_client-0.8.0/pystac_client/collection_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-05-17 14:16:27.000000 pystac_client-0.8.0/pystac_client/conformance.py
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-17 14:16:27.000000 pystac_client-0.8.0/pystac_client/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-17 14:16:27.000000 pystac_client-0.8.0/pystac_client/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    32836 2024-05-17 14:16:27.000000 pystac_client-0.8.0/pystac_client/item_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-05-17 14:16:27.000000 pystac_client-0.8.0/pystac_client/mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 14:16:27.000000 pystac_client-0.8.0/pystac_client/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    12498 2024-05-17 14:16:27.000000 pystac_client-0.8.0/pystac_client/stac_api_io.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-17 14:16:27.000000 pystac_client-0.8.0/pystac_client/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-05-17 14:16:27.000000 pystac_client-0.8.0/pystac_client/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:16:36.777439 pystac_client-0.8.0/pystac_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5104 2024-05-17 14:16:36.000000 pystac_client-0.8.0/pystac_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-17 14:16:36.000000 pystac_client-0.8.0/pystac_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 14:16:36.000000 pystac_client-0.8.0/pystac_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-17 14:16:36.000000 pystac_client-0.8.0/pystac_client.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-17 14:16:36.000000 pystac_client-0.8.0/pystac_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-17 14:16:36.000000 pystac_client-0.8.0/pystac_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 14:16:36.781440 pystac_client-0.8.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 14:16:36.777439 pystac_client-0.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     9247 2024-05-17 14:16:27.000000 pystac_client-0.8.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    27234 2024-05-17 14:16:27.000000 pystac_client-0.8.0/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3366 2024-05-17 14:16:27.000000 pystac_client-0.8.0/tests/test_collection_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    30015 2024-05-17 14:16:27.000000 pystac_client-0.8.0/tests/test_item_search.py
--rw-r--r--   0 runner    (1001) docker     (127)     9519 2024-05-17 14:16:27.000000 pystac_client-0.8.0/tests/test_stac_api_io.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:51:14.386716 pystac_client-0.8.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-23 14:51:06.000000 pystac_client-0.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-23 14:51:06.000000 pystac_client-0.8.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5104 2024-05-23 14:51:14.386716 pystac_client-0.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1582 2024-05-23 14:51:06.000000 pystac_client-0.8.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-05-23 14:51:06.000000 pystac_client-0.8.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:51:14.382717 pystac_client-0.8.1/pystac_client/
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-23 14:51:06.000000 pystac_client-0.8.1/pystac_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-05-23 14:51:06.000000 pystac_client-0.8.1/pystac_client/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11531 2024-05-23 14:51:06.000000 pystac_client-0.8.1/pystac_client/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26442 2024-05-23 14:51:06.000000 pystac_client-0.8.1/pystac_client/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7839 2024-05-23 14:51:06.000000 pystac_client-0.8.1/pystac_client/collection_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-05-23 14:51:06.000000 pystac_client-0.8.1/pystac_client/conformance.py
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-23 14:51:06.000000 pystac_client-0.8.1/pystac_client/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-23 14:51:06.000000 pystac_client-0.8.1/pystac_client/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32832 2024-05-23 14:51:06.000000 pystac_client-0.8.1/pystac_client/item_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-05-23 14:51:06.000000 pystac_client-0.8.1/pystac_client/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 14:51:06.000000 pystac_client-0.8.1/pystac_client/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    12498 2024-05-23 14:51:06.000000 pystac_client-0.8.1/pystac_client/stac_api_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-23 14:51:06.000000 pystac_client-0.8.1/pystac_client/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-05-23 14:51:06.000000 pystac_client-0.8.1/pystac_client/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:51:14.382717 pystac_client-0.8.1/pystac_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5104 2024-05-23 14:51:14.000000 pystac_client-0.8.1/pystac_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-23 14:51:14.000000 pystac_client-0.8.1/pystac_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 14:51:14.000000 pystac_client-0.8.1/pystac_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-23 14:51:14.000000 pystac_client-0.8.1/pystac_client.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-23 14:51:14.000000 pystac_client-0.8.1/pystac_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-23 14:51:14.000000 pystac_client-0.8.1/pystac_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 14:51:14.386716 pystac_client-0.8.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:51:14.382717 pystac_client-0.8.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     9247 2024-05-23 14:51:06.000000 pystac_client-0.8.1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27234 2024-05-23 14:51:06.000000 pystac_client-0.8.1/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3366 2024-05-23 14:51:06.000000 pystac_client-0.8.1/tests/test_collection_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30474 2024-05-23 14:51:06.000000 pystac_client-0.8.1/tests/test_item_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9519 2024-05-23 14:51:06.000000 pystac_client-0.8.1/tests/test_stac_api_io.py
```

### Comparing `pystac_client-0.8.0/LICENSE` & `pystac_client-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pystac_client-0.8.0/PKG-INFO` & `pystac_client-0.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystac-client
-Version: 0.8.0
+Version: 0.8.1
 Summary: Python library for working with SpatioTemporal Asset Catalog (STAC) APIs.
 Author-email: Jon Duckworth <duckontheweb@gmail.com>, Matthew Hanson <matt.a.hanson@gmail.com>
 Maintainer-email: Pete Gadomski <pete.gadomski@gmail.com>
 License: Apache-2.0
 Project-URL: homepage, https://github.com/stac-utils/pystac-client
 Project-URL: documentation, https://pystac-client.readthedocs.io
 Project-URL: repository, https://github.com/stac-utils/pystac-client.git
@@ -43,15 +43,15 @@
 Requires-Dist: pytest-benchmark~=4.0.0; extra == "dev"
 Requires-Dist: pytest-console-scripts~=1.4.0; extra == "dev"
 Requires-Dist: pytest-cov~=5.0; extra == "dev"
 Requires-Dist: pytest-recording~=0.13; extra == "dev"
 Requires-Dist: pytest~=8.0; extra == "dev"
 Requires-Dist: recommonmark~=0.7.1; extra == "dev"
 Requires-Dist: requests-mock~=1.12; extra == "dev"
-Requires-Dist: ruff==0.4.4; extra == "dev"
+Requires-Dist: ruff==0.4.5; extra == "dev"
 Requires-Dist: tomli~=2.0; python_version < "3.11" and extra == "dev"
 Requires-Dist: types-python-dateutil<2.10.0,>=2.8.19; extra == "dev"
 Requires-Dist: types-requests~=2.31.0; extra == "dev"
 Requires-Dist: urllib3<2; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: Sphinx~=7.3; extra == "docs"
 Requires-Dist: boto3~=1.26; extra == "docs"
```

### Comparing `pystac_client-0.8.0/README.md` & `pystac_client-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `pystac_client-0.8.0/pyproject.toml` & `pystac_client-0.8.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     "pytest-benchmark~=4.0.0",
     "pytest-console-scripts~=1.4.0",
     "pytest-cov~=5.0",
     "pytest-recording~=0.13",
     "pytest~=8.0",
     "recommonmark~=0.7.1",
     "requests-mock~=1.12",
-    "ruff==0.4.4",
+    "ruff==0.4.5",
     "tomli~=2.0; python_version<'3.11'",
     "types-python-dateutil>=2.8.19,<2.10.0",
     "types-requests~=2.31.0",
     # temporary pin https://github.com/stac-utils/pystac-client/issues/509
     "urllib3<2",
 ]
 docs = [
```

### Comparing `pystac_client-0.8.0/pystac_client/_utils.py` & `pystac_client-0.8.1/pystac_client/_utils.py`

 * *Files identical despite different names*

### Comparing `pystac_client-0.8.0/pystac_client/cli.py` & `pystac_client-0.8.1/pystac_client/cli.py`

 * *Files identical despite different names*

### Comparing `pystac_client-0.8.0/pystac_client/client.py` & `pystac_client-0.8.1/pystac_client/client.py`

 * *Files identical despite different names*

### Comparing `pystac_client-0.8.0/pystac_client/collection_client.py` & `pystac_client-0.8.1/pystac_client/collection_client.py`

 * *Files identical despite different names*

### Comparing `pystac_client-0.8.0/pystac_client/conformance.py` & `pystac_client-0.8.1/pystac_client/conformance.py`

 * *Files identical despite different names*

### Comparing `pystac_client-0.8.0/pystac_client/item_search.py` & `pystac_client-0.8.1/pystac_client/item_search.py`

 * *Files 0% similar despite different names*

```diff
@@ -629,20 +629,20 @@
         for field in fields:
             if field.startswith("-"):
                 excludes.append(field[1:])
             elif field.startswith("+"):
                 includes.append(field[1:])
             else:
                 includes.append(field)
-        return {"includes": includes, "excludes": excludes}
+        return {"include": includes, "exclude": excludes}
 
     @staticmethod
     def _fields_dict_to_str(fields: Fields) -> str:
-        includes = [f"+{x}" for x in fields.get("includes", [])]
-        excludes = [f"-{x}" for x in fields.get("excludes", [])]
+        includes = [f"+{x}" for x in fields.get("include", [])]
+        excludes = [f"-{x}" for x in fields.get("exclude", [])]
         return ",".join(chain(includes, excludes))
 
     @staticmethod
     def _format_intersects(value: Optional[IntersectsLike]) -> Optional[Intersects]:
         if value is None:
             return None
         if isinstance(value, dict):
```

### Comparing `pystac_client-0.8.0/pystac_client/mixins.py` & `pystac_client-0.8.1/pystac_client/mixins.py`

 * *Files identical despite different names*

### Comparing `pystac_client-0.8.0/pystac_client/stac_api_io.py` & `pystac_client-0.8.1/pystac_client/stac_api_io.py`

 * *Files identical despite different names*

### Comparing `pystac_client-0.8.0/pystac_client/warnings.py` & `pystac_client-0.8.1/pystac_client/warnings.py`

 * *Files identical despite different names*

### Comparing `pystac_client-0.8.0/pystac_client.egg-info/PKG-INFO` & `pystac_client-0.8.1/pystac_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystac-client
-Version: 0.8.0
+Version: 0.8.1
 Summary: Python library for working with SpatioTemporal Asset Catalog (STAC) APIs.
 Author-email: Jon Duckworth <duckontheweb@gmail.com>, Matthew Hanson <matt.a.hanson@gmail.com>
 Maintainer-email: Pete Gadomski <pete.gadomski@gmail.com>
 License: Apache-2.0
 Project-URL: homepage, https://github.com/stac-utils/pystac-client
 Project-URL: documentation, https://pystac-client.readthedocs.io
 Project-URL: repository, https://github.com/stac-utils/pystac-client.git
@@ -43,15 +43,15 @@
 Requires-Dist: pytest-benchmark~=4.0.0; extra == "dev"
 Requires-Dist: pytest-console-scripts~=1.4.0; extra == "dev"
 Requires-Dist: pytest-cov~=5.0; extra == "dev"
 Requires-Dist: pytest-recording~=0.13; extra == "dev"
 Requires-Dist: pytest~=8.0; extra == "dev"
 Requires-Dist: recommonmark~=0.7.1; extra == "dev"
 Requires-Dist: requests-mock~=1.12; extra == "dev"
-Requires-Dist: ruff==0.4.4; extra == "dev"
+Requires-Dist: ruff==0.4.5; extra == "dev"
 Requires-Dist: tomli~=2.0; python_version < "3.11" and extra == "dev"
 Requires-Dist: types-python-dateutil<2.10.0,>=2.8.19; extra == "dev"
 Requires-Dist: types-requests~=2.31.0; extra == "dev"
 Requires-Dist: urllib3<2; extra == "dev"
 Provides-Extra: docs
 Requires-Dist: Sphinx~=7.3; extra == "docs"
 Requires-Dist: boto3~=1.26; extra == "docs"
```

### Comparing `pystac_client-0.8.0/pystac_client.egg-info/SOURCES.txt` & `pystac_client-0.8.1/pystac_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pystac_client-0.8.0/pystac_client.egg-info/requires.txt` & `pystac_client-0.8.1/pystac_client.egg-info/requires.txt`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 pytest-benchmark~=4.0.0
 pytest-console-scripts~=1.4.0
 pytest-cov~=5.0
 pytest-recording~=0.13
 pytest~=8.0
 recommonmark~=0.7.1
 requests-mock~=1.12
-ruff==0.4.4
+ruff==0.4.5
 types-python-dateutil<2.10.0,>=2.8.19
 types-requests~=2.31.0
 urllib3<2
 
 [dev:python_version < "3.11"]
 tomli~=2.0
```

### Comparing `pystac_client-0.8.0/tests/test_cli.py` & `pystac_client-0.8.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `pystac_client-0.8.0/tests/test_client.py` & `pystac_client-0.8.1/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `pystac_client-0.8.0/tests/test_collection_client.py` & `pystac_client-0.8.1/tests/test_collection_client.py`

 * *Files identical despite different names*

### Comparing `pystac_client-0.8.0/tests/test_item_search.py` & `pystac_client-0.8.1/tests/test_item_search.py`

 * *Files 1% similar despite different names*

```diff
@@ -464,31 +464,31 @@
             ItemSearch(url=SEARCH_URL, fields=1)  # type: ignore
 
         with pytest.raises(Exception):
             ItemSearch(url=SEARCH_URL, fields=[1])  # type: ignore
 
         search = ItemSearch(url=SEARCH_URL, fields="id,collection,+foo,-bar")
         assert search.get_parameters()["fields"] == {
-            "excludes": ["bar"],
-            "includes": ["id", "collection", "foo"],
+            "exclude": ["bar"],
+            "include": ["id", "collection", "foo"],
         }
 
         search = ItemSearch(url=SEARCH_URL, fields=["id", "collection", "+foo", "-bar"])
         assert search.get_parameters()["fields"] == {
-            "excludes": ["bar"],
-            "includes": ["id", "collection", "foo"],
+            "exclude": ["bar"],
+            "include": ["id", "collection", "foo"],
         }
 
         search = ItemSearch(
             url=SEARCH_URL,
-            fields={"excludes": ["bar"], "includes": ["id", "collection"]},
+            fields={"exclude": ["bar"], "include": ["id", "collection"]},
         )
         assert search.get_parameters()["fields"] == {
-            "excludes": ["bar"],
-            "includes": ["id", "collection"],
+            "exclude": ["bar"],
+            "include": ["id", "collection"],
         }
 
         search = ItemSearch(
             url=SEARCH_URL, method="GET", fields="id,collection,+foo,-bar"
         )
         assert search.get_parameters()["fields"] == "+id,+collection,+foo,-bar"
 
@@ -496,15 +496,15 @@
             url=SEARCH_URL, method="GET", fields=["id", "collection", "+foo", "-bar"]
         )
         assert search.get_parameters()["fields"] == "+id,+collection,+foo,-bar"
 
         search = ItemSearch(
             url=SEARCH_URL,
             method="GET",
-            fields={"excludes": ["bar"], "includes": ["id", "collection"]},
+            fields={"exclude": ["bar"], "include": ["id", "collection"]},
         )
         assert search.get_parameters()["fields"] == "+id,+collection,-bar"
 
 
 class TestItemSearch:
     @pytest.fixture(scope="function")
     def astraea_api(self) -> Client:
@@ -831,7 +831,22 @@
 def test_naive_datetime() -> None:
     search = ItemSearch(
         url="https://earth-search.aws.element84.com/v1/search",
         datetime=datetime(2024, 5, 14, 4, 25, 42, tzinfo=None),
         method="POST",
     )
     assert search.get_parameters()["datetime"] == "2024-05-14T04:25:42Z"
+
+
+@pytest.mark.vcr
+def test_fields() -> None:
+    search = ItemSearch(
+        url="https://earth-search.aws.element84.com/v1/search",
+        collections=["sentinel-2-c1-l2a"],
+        intersects={"type": "Point", "coordinates": [-105.1019, 40.1672]},
+        max_items=1,
+        fields=["-geometry", "-assets", "-links"],
+    )
+    item = next(search.items_as_dicts())
+    assert "geometry" not in item
+    assert "assets" not in item
+    assert "links" not in item
```

### Comparing `pystac_client-0.8.0/tests/test_stac_api_io.py` & `pystac_client-0.8.1/tests/test_stac_api_io.py`

 * *Files identical despite different names*

