# Comparing `tmp/sdkfabric_notion-0.1.2.tar.gz` & `tmp/sdkfabric_notion-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdkfabric_notion-0.1.2.tar", last modified: Mon May 20 06:41:48 2024, max compression
+gzip compressed data, was "sdkfabric_notion-0.1.3.tar", last modified: Thu May 23 21:17:20 2024, max compression
```

## Comparing `sdkfabric_notion-0.1.2.tar` & `sdkfabric_notion-0.1.3.tar`

### file list

```diff
@@ -1,32 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 06:41:48.664296 sdkfabric_notion-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-20 06:41:42.000000 sdkfabric_notion-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-20 06:41:48.664296 sdkfabric_notion-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-05-20 06:41:42.000000 sdkfabric_notion-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-20 06:41:42.000000 sdkfabric_notion-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 06:41:48.664296 sdkfabric_notion-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 06:41:42.000000 sdkfabric_notion-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 06:41:48.660296 sdkfabric_notion-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 06:41:48.664296 sdkfabric_notion-0.1.2/src/sdk/
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-20 06:41:42.000000 sdkfabric_notion-0.1.2/src/sdk/block.py
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-20 06:41:42.000000 sdkfabric_notion-0.1.2/src/sdk/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-20 06:41:42.000000 sdkfabric_notion-0.1.2/src/sdk/database.py
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-20 06:41:42.000000 sdkfabric_notion-0.1.2/src/sdk/database_annotations.py
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-20 06:41:42.000000 sdkfabric_notion-0.1.2/src/sdk/database_cover.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-20 06:41:42.000000 sdkfabric_notion-0.1.2/src/sdk/database_icon.py
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-20 06:41:42.000000 sdkfabric_notion-0.1.2/src/sdk/database_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-20 06:41:42.000000 sdkfabric_notion-0.1.2/src/sdk/database_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-20 06:41:42.000000 sdkfabric_notion-0.1.2/src/sdk/database_text.py
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-20 06:41:42.000000 sdkfabric_notion-0.1.2/src/sdk/database_title.py
--rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-05-20 06:41:42.000000 sdkfabric_notion-0.1.2/src/sdk/page.py
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-20 06:41:42.000000 sdkfabric_notion-0.1.2/src/sdk/page_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-05-20 06:41:42.000000 sdkfabric_notion-0.1.2/src/sdk/page_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-20 06:41:42.000000 sdkfabric_notion-0.1.2/src/sdk/person.py
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-20 06:41:42.000000 sdkfabric_notion-0.1.2/src/sdk/user.py
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-20 06:41:42.000000 sdkfabric_notion-0.1.2/src/sdk/user_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-05-20 06:41:42.000000 sdkfabric_notion-0.1.2/src/sdk/user_tag.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 06:41:48.664296 sdkfabric_notion-0.1.2/src/sdkfabric_notion.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-20 06:41:48.000000 sdkfabric_notion-0.1.2/src/sdkfabric_notion.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-20 06:41:48.000000 sdkfabric_notion-0.1.2/src/sdkfabric_notion.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 06:41:48.000000 sdkfabric_notion-0.1.2/src/sdkfabric_notion.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-20 06:41:48.000000 sdkfabric_notion-0.1.2/src/sdkfabric_notion.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-20 06:41:48.000000 sdkfabric_notion-0.1.2/src/sdkfabric_notion.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:17:20.145251 sdkfabric_notion-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-23 21:17:16.000000 sdkfabric_notion-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-23 21:17:20.145251 sdkfabric_notion-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-05-23 21:17:16.000000 sdkfabric_notion-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-23 21:17:16.000000 sdkfabric_notion-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 21:17:20.145251 sdkfabric_notion-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 21:17:16.000000 sdkfabric_notion-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:17:20.141251 sdkfabric_notion-0.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:17:20.145251 sdkfabric_notion-0.1.3/src/sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-23 21:17:16.000000 sdkfabric_notion-0.1.3/src/sdk/block.py
+-rw-r--r--   0 runner    (1001) docker     (127)      960 2024-05-23 21:17:16.000000 sdkfabric_notion-0.1.3/src/sdk/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-23 21:17:16.000000 sdkfabric_notion-0.1.3/src/sdk/comment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-23 21:17:16.000000 sdkfabric_notion-0.1.3/src/sdk/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-23 21:17:16.000000 sdkfabric_notion-0.1.3/src/sdk/database_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-23 21:17:16.000000 sdkfabric_notion-0.1.3/src/sdk/database_cover.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-23 21:17:16.000000 sdkfabric_notion-0.1.3/src/sdk/database_icon.py
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-23 21:17:16.000000 sdkfabric_notion-0.1.3/src/sdk/database_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-23 21:17:16.000000 sdkfabric_notion-0.1.3/src/sdk/database_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-23 21:17:16.000000 sdkfabric_notion-0.1.3/src/sdk/database_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-23 21:17:16.000000 sdkfabric_notion-0.1.3/src/sdk/database_title.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1372 2024-05-23 21:17:16.000000 sdkfabric_notion-0.1.3/src/sdk/page.py
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-23 21:17:16.000000 sdkfabric_notion-0.1.3/src/sdk/page_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-05-23 21:17:16.000000 sdkfabric_notion-0.1.3/src/sdk/page_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-23 21:17:16.000000 sdkfabric_notion-0.1.3/src/sdk/person.py
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-23 21:17:16.000000 sdkfabric_notion-0.1.3/src/sdk/rich_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-23 21:17:16.000000 sdkfabric_notion-0.1.3/src/sdk/rich_text_annotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-23 21:17:16.000000 sdkfabric_notion-0.1.3/src/sdk/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-23 21:17:16.000000 sdkfabric_notion-0.1.3/src/sdk/user_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-05-23 21:17:16.000000 sdkfabric_notion-0.1.3/src/sdk/user_tag.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:17:20.145251 sdkfabric_notion-0.1.3/src/sdkfabric_notion.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-23 21:17:20.000000 sdkfabric_notion-0.1.3/src/sdkfabric_notion.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-23 21:17:20.000000 sdkfabric_notion-0.1.3/src/sdkfabric_notion.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 21:17:20.000000 sdkfabric_notion-0.1.3/src/sdkfabric_notion.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-23 21:17:20.000000 sdkfabric_notion-0.1.3/src/sdkfabric_notion.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-23 21:17:20.000000 sdkfabric_notion-0.1.3/src/sdkfabric_notion.egg-info/top_level.txt
```

### Comparing `sdkfabric_notion-0.1.2/LICENSE` & `sdkfabric_notion-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sdkfabric_notion-0.1.2/PKG-INFO` & `sdkfabric_notion-0.1.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdkfabric-notion
-Version: 0.1.2
+Version: 0.1.3
 Summary: Notion Python SDK managed by SDK Fabric
 Author-email: Christoph Kappestein <christoph.kappestein@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/sdk-fabric/notion-python
 Project-URL: Issues, https://github.com/sdk-fabric/notion-python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sdkfabric_notion-0.1.2/README.md` & `sdkfabric_notion-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `sdkfabric_notion-0.1.2/pyproject.toml` & `sdkfabric_notion-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "sdkfabric-notion"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   { name="Christoph Kappestein", email="christoph.kappestein@gmail.com" },
 ]
 description = "Notion Python SDK managed by SDK Fabric"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {text = "MIT"}
```

### Comparing `sdkfabric_notion-0.1.2/src/sdk/block.py` & `sdkfabric_notion-0.1.3/src/sdk/block.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_notion-0.1.2/src/sdk/client.py` & `sdkfabric_notion-0.1.3/src/sdk/client.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_notion-0.1.2/src/sdk/database.py` & `sdkfabric_notion-0.1.3/src/sdk/database.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_notion-0.1.2/src/sdk/database_annotations.py` & `sdkfabric_notion-0.1.3/src/sdk/database_annotations.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_notion-0.1.2/src/sdk/database_tag.py` & `sdkfabric_notion-0.1.3/src/sdk/database_tag.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_notion-0.1.2/src/sdk/database_title.py` & `sdkfabric_notion-0.1.3/src/sdk/database_title.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_notion-0.1.2/src/sdk/page.py` & `sdkfabric_notion-0.1.3/src/sdk/page.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_notion-0.1.2/src/sdk/page_tag.py` & `sdkfabric_notion-0.1.3/src/sdk/page_tag.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_notion-0.1.2/src/sdk/user.py` & `sdkfabric_notion-0.1.3/src/sdk/user.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_notion-0.1.2/src/sdk/user_collection.py` & `sdkfabric_notion-0.1.3/src/sdk/user_collection.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_notion-0.1.2/src/sdk/user_tag.py` & `sdkfabric_notion-0.1.3/src/sdk/user_tag.py`

 * *Files identical despite different names*

### Comparing `sdkfabric_notion-0.1.2/src/sdkfabric_notion.egg-info/PKG-INFO` & `sdkfabric_notion-0.1.3/src/sdkfabric_notion.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdkfabric-notion
-Version: 0.1.2
+Version: 0.1.3
 Summary: Notion Python SDK managed by SDK Fabric
 Author-email: Christoph Kappestein <christoph.kappestein@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/sdk-fabric/notion-python
 Project-URL: Issues, https://github.com/sdk-fabric/notion-python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sdkfabric_notion-0.1.2/src/sdkfabric_notion.egg-info/SOURCES.txt` & `sdkfabric_notion-0.1.3/src/sdkfabric_notion.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
 src/sdk/block.py
 src/sdk/client.py
+src/sdk/comment.py
 src/sdk/database.py
 src/sdk/database_annotations.py
 src/sdk/database_cover.py
 src/sdk/database_icon.py
 src/sdk/database_id.py
 src/sdk/database_tag.py
 src/sdk/database_text.py
 src/sdk/database_title.py
 src/sdk/page.py
 src/sdk/page_id.py
 src/sdk/page_tag.py
 src/sdk/person.py
+src/sdk/rich_text.py
+src/sdk/rich_text_annotation.py
 src/sdk/user.py
 src/sdk/user_collection.py
 src/sdk/user_tag.py
 src/sdkfabric_notion.egg-info/PKG-INFO
 src/sdkfabric_notion.egg-info/SOURCES.txt
 src/sdkfabric_notion.egg-info/dependency_links.txt
 src/sdkfabric_notion.egg-info/requires.txt
```

