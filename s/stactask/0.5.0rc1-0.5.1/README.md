# Comparing `tmp/stactask-0.5.0rc1.tar.gz` & `tmp/stactask-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stactask-0.5.0rc1.tar", last modified: Thu May  9 13:55:11 2024, max compression
+gzip compressed data, was "stactask-0.5.1.tar", last modified: Thu May 23 14:04:22 2024, max compression
```

## Comparing `stactask-0.5.0rc1.tar` & `stactask-0.5.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:55:11.566483 stactask-0.5.0rc1/
--rw-r--r--   0 runner    (1001) docker     (127)    11341 2024-05-09 13:55:02.000000 stactask-0.5.0rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-09 13:55:02.000000 stactask-0.5.0rc1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    12584 2024-05-09 13:55:11.566483 stactask-0.5.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10717 2024-05-09 13:55:02.000000 stactask-0.5.0rc1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-05-09 13:55:02.000000 stactask-0.5.0rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 13:55:11.566483 stactask-0.5.0rc1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:55:11.562483 stactask-0.5.0rc1/stactask/
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-09 13:55:02.000000 stactask-0.5.0rc1/stactask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4135 2024-05-09 13:55:02.000000 stactask-0.5.0rc1/stactask/asset_io.py
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-09 13:55:02.000000 stactask-0.5.0rc1/stactask/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-09 13:55:02.000000 stactask-0.5.0rc1/stactask/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-09 13:55:02.000000 stactask-0.5.0rc1/stactask/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 13:55:02.000000 stactask-0.5.0rc1/stactask/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    20417 2024-05-09 13:55:02.000000 stactask-0.5.0rc1/stactask/task.py
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-05-09 13:55:02.000000 stactask-0.5.0rc1/stactask/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:55:11.566483 stactask-0.5.0rc1/stactask.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12584 2024-05-09 13:55:11.000000 stactask-0.5.0rc1/stactask.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-09 13:55:11.000000 stactask-0.5.0rc1/stactask.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 13:55:11.000000 stactask-0.5.0rc1/stactask.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-09 13:55:11.000000 stactask-0.5.0rc1/stactask.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-09 13:55:11.000000 stactask-0.5.0rc1/stactask.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:55:11.566483 stactask-0.5.0rc1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6943 2024-05-09 13:55:02.000000 stactask-0.5.0rc1/tests/test_task.py
--rw-r--r--   0 runner    (1001) docker     (127)     4897 2024-05-09 13:55:02.000000 stactask-0.5.0rc1/tests/test_task_download.py
--rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-05-09 13:55:02.000000 stactask-0.5.0rc1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:04:22.164937 stactask-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11341 2024-05-23 14:04:12.000000 stactask-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-23 14:04:12.000000 stactask-0.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    12581 2024-05-23 14:04:22.164937 stactask-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10717 2024-05-23 14:04:12.000000 stactask-0.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-05-23 14:04:12.000000 stactask-0.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 14:04:22.164937 stactask-0.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:04:22.160937 stactask-0.5.1/stactask/
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-23 14:04:12.000000 stactask-0.5.1/stactask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4262 2024-05-23 14:04:12.000000 stactask-0.5.1/stactask/asset_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-23 14:04:12.000000 stactask-0.5.1/stactask/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-23 14:04:12.000000 stactask-0.5.1/stactask/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-23 14:04:12.000000 stactask-0.5.1/stactask/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 14:04:12.000000 stactask-0.5.1/stactask/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    20745 2024-05-23 14:04:12.000000 stactask-0.5.1/stactask/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-05-23 14:04:12.000000 stactask-0.5.1/stactask/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:04:22.164937 stactask-0.5.1/stactask.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12581 2024-05-23 14:04:22.000000 stactask-0.5.1/stactask.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-23 14:04:22.000000 stactask-0.5.1/stactask.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 14:04:22.000000 stactask-0.5.1/stactask.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-23 14:04:22.000000 stactask-0.5.1/stactask.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-23 14:04:22.000000 stactask-0.5.1/stactask.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:04:22.164937 stactask-0.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6943 2024-05-23 14:04:12.000000 stactask-0.5.1/tests/test_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4897 2024-05-23 14:04:12.000000 stactask-0.5.1/tests/test_task_download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-05-23 14:04:12.000000 stactask-0.5.1/tests/test_utils.py
```

### Comparing `stactask-0.5.0rc1/LICENSE` & `stactask-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `stactask-0.5.0rc1/PKG-INFO` & `stactask-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stactask
-Version: 0.5.0rc1
+Version: 0.5.1
 Summary: Class interface for running custom algorithms and workflows on STAC Items
 Author-email: Matthew Hanson <matt.a.hanson@gmail.com>
 Maintainer-email: Pete Gadomski <pete.gadomski@gmail.com>
 License: Apache-2.0
 Project-URL: Issues, https://github.com/stac-utils/stactask/issues
 Project-URL: Github, https://github.com/stac-utils/stac-task
 Project-URL: Changelog, https://github.com/stac-utils/stac-task/blob/main/CHANGELOG.md
```

### Comparing `stactask-0.5.0rc1/README.md` & `stactask-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `stactask-0.5.0rc1/pyproject.toml` & `stactask-0.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "stactask"
-version = "0.5.0-pre1"
+version = "0.5.1"
 authors = [{ name = "Matthew Hanson", email = "matt.a.hanson@gmail.com" }]
 maintainers = [{ name = "Pete Gadomski", email = "pete.gadomski@gmail.com" }]
 description = "Class interface for running custom algorithms and workflows on STAC Items"
 readme = "README.md"
 requires-python = ">=3.9"
 keywords = ["pystac", "imagery", "raster", "catalog", "STAC"]
 license = { text = "Apache-2.0" }
```

### Comparing `stactask-0.5.0rc1/stactask/asset_io.py` & `stactask-0.5.1/stactask/asset_io.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,38 +17,41 @@
 
 
 async def download_item_assets(
     item: Item,
     path_template: str = "${collection}/${id}",
     config: Optional[DownloadConfig] = None,
     keep_non_downloaded: bool = True,
+    file_name: Optional[str] = "item.json",
 ) -> Item:
     return await stac_asset.download_item(
         item=item.clone(),
         directory=LayoutTemplate(path_template).substitute(item),
-        file_name="item.json",
+        file_name=file_name,
         config=config,
         keep_non_downloaded=keep_non_downloaded,
     )
 
 
 async def download_items_assets(
     items: Iterable[Item],
     path_template: str = "${collection}/${id}",
     config: Optional[DownloadConfig] = None,
     keep_non_downloaded: bool = True,
+    file_name: Optional[str] = "item.json",
 ) -> list[Item]:
     return await asyncio.gather(
         *[
             asyncio.create_task(
                 download_item_assets(
                     item=item,
                     path_template=path_template,
                     config=config,
                     keep_non_downloaded=keep_non_downloaded,
+                    file_name=file_name,
                 )
             )
             for item in items
         ]
     )
```

### Comparing `stactask-0.5.0rc1/stactask/logging.py` & `stactask-0.5.1/stactask/logging.py`

 * *Files identical despite different names*

### Comparing `stactask-0.5.0rc1/stactask/task.py` & `stactask-0.5.1/stactask/task.py`

 * *Files 9% similar despite different names*

```diff
@@ -239,65 +239,71 @@
 
     def download_item_assets(
         self,
         item: Item,
         path_template: str = "${collection}/${id}",
         config: Optional[DownloadConfig] = None,
         keep_non_downloaded: bool = True,
+        file_name: Optional[str] = "item.json",
     ) -> Item:
         """Download provided asset keys for the given item. Assets are
         saved in workdir in a directory (as specified by path_template), and
         the items are updated with the new asset hrefs.
 
         Args:
             item (pystac.Item): STAC Item for which assets need be downloaded.
-            assets (Optional[list[str]]): List of asset keys to download.
-                Defaults to all assets.
             path_template (Optional[str]): String to be interpolated to specify
                 where to store downloaded files.
+            config (Optional[DownloadConfig]): Configuration for downloading an item
+                and its assets.
             keep_original_filenames (Optional[bool]): Controls whether original
                 file names should be used, or asset key + extension.
+            file_name (Optional[str]): The name of the item file to save.
         """
         return asyncio.get_event_loop().run_until_complete(
             download_item_assets(
                 item,
                 path_template=str(self._workdir / path_template),
                 config=config,
                 keep_non_downloaded=keep_non_downloaded,
+                file_name=file_name,
             )
         )
 
     def download_items_assets(
         self,
         items: Iterable[Item],
         path_template: str = "${collection}/${id}",
         config: Optional[DownloadConfig] = None,
         keep_non_downloaded: bool = True,
+        file_name: Optional[str] = "item.json",
     ) -> list[Item]:
         """Download provided asset keys for the given items. Assets are
         saved in workdir in a directory (as specified by path_template), and
         the items are updated with the new asset hrefs.
 
         Args:
             items (list[pystac.Item]): List of STAC Items for which assets need
                 be downloaded.
-            assets (Optional[list[str]]): List of asset keys to download.
-                Defaults to all assets.
             path_template (Optional[str]): String to be interpolated to specify
                 where to store downloaded files.
+            config (Optional[DownloadConfig]): Configuration for downloading items
+                and their assets.
             keep_original_filenames (Optional[bool]): Controls whether original
                 file names should be used, or asset key + extension.
+            file_name (Optional[str]): The name of the item file to save.
         """
         return list(
             asyncio.get_event_loop().run_until_complete(
                 download_items_assets(
                     items,
                     path_template=str(self._workdir / path_template),
                     config=config,
                     keep_non_downloaded=keep_non_downloaded,
+                    file_name=file_name,
                 )
             )
         )
 
     def upload_item_assets_to_s3(
         self,
         item: Item,
```

### Comparing `stactask-0.5.0rc1/stactask/utils.py` & `stactask-0.5.1/stactask/utils.py`

 * *Files identical despite different names*

### Comparing `stactask-0.5.0rc1/stactask.egg-info/PKG-INFO` & `stactask-0.5.1/stactask.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stactask
-Version: 0.5.0rc1
+Version: 0.5.1
 Summary: Class interface for running custom algorithms and workflows on STAC Items
 Author-email: Matthew Hanson <matt.a.hanson@gmail.com>
 Maintainer-email: Pete Gadomski <pete.gadomski@gmail.com>
 License: Apache-2.0
 Project-URL: Issues, https://github.com/stac-utils/stactask/issues
 Project-URL: Github, https://github.com/stac-utils/stac-task
 Project-URL: Changelog, https://github.com/stac-utils/stac-task/blob/main/CHANGELOG.md
```

### Comparing `stactask-0.5.0rc1/tests/test_task.py` & `stactask-0.5.1/tests/test_task.py`

 * *Files identical despite different names*

### Comparing `stactask-0.5.0rc1/tests/test_task_download.py` & `stactask-0.5.1/tests/test_task_download.py`

 * *Files identical despite different names*

### Comparing `stactask-0.5.0rc1/tests/test_utils.py` & `stactask-0.5.1/tests/test_utils.py`

 * *Files identical despite different names*

