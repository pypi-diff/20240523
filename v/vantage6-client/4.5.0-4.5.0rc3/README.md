# Comparing `tmp/vantage6-client-4.5.0.tar.gz` & `tmp/vantage6-client-4.5.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vantage6-client-4.5.0.tar", last modified: Thu May 23 15:14:48 2024, max compression
+gzip compressed data, was "vantage6-client-4.5.0rc3.tar", last modified: Wed May 22 15:04:57 2024, max compression
```

## Comparing `vantage6-client-4.5.0.tar` & `vantage6-client-4.5.0rc3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:14:48.150661 vantage6-client-4.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     9688 2024-05-23 15:14:48.150661 vantage6-client-4.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 15:14:48.150661 vantage6-client-4.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-05-23 15:14:32.000000 vantage6-client-4.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:14:48.146661 vantage6-client-4.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4699 2024-05-23 15:14:32.000000 vantage6-client-4.5.0/tests/test_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:14:48.146661 vantage6-client-4.5.0/vantage6/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:14:48.146661 vantage6-client-4.5.0/vantage6/client/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 15:14:32.000000 vantage6-client-4.5.0/vantage6/client/__build__
--rw-r--r--   0 runner    (1001) docker     (127)    68221 2024-05-23 15:14:32.000000 vantage6-client-4.5.0/vantage6/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-23 15:14:32.000000 vantage6-client-4.5.0/vantage6/client/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-23 15:14:32.000000 vantage6-client-4.5.0/vantage6/client/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     8013 2024-05-23 15:14:32.000000 vantage6-client-4.5.0/vantage6/client/filter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:14:48.150661 vantage6-client-4.5.0/vantage6/client/subclients/
--rw-r--r--   0 runner    (1001) docker     (127)     9535 2024-05-23 15:14:32.000000 vantage6-client-4.5.0/vantage6/client/subclients/algorithm.py
--rw-r--r--   0 runner    (1001) docker     (127)     7592 2024-05-23 15:14:32.000000 vantage6-client-4.5.0/vantage6/client/subclients/algorithm_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-05-23 15:14:32.000000 vantage6-client-4.5.0/vantage6/client/subclients/store_role.py
--rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-05-23 15:14:32.000000 vantage6-client-4.5.0/vantage6/client/subclients/store_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     3451 2024-05-23 15:14:32.000000 vantage6-client-4.5.0/vantage6/client/subclients/store_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     5472 2024-05-23 15:14:32.000000 vantage6-client-4.5.0/vantage6/client/subclients/study.py
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-23 15:14:32.000000 vantage6-client-4.5.0/vantage6/client/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:14:48.150661 vantage6-client-4.5.0/vantage6_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9688 2024-05-23 15:14:48.000000 vantage6-client-4.5.0/vantage6_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-23 15:14:48.000000 vantage6-client-4.5.0/vantage6_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 15:14:48.000000 vantage6-client-4.5.0/vantage6_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-23 15:14:48.000000 vantage6-client-4.5.0/vantage6_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-23 15:14:48.000000 vantage6-client-4.5.0/vantage6_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:57.421279 vantage6-client-4.5.0rc3/
+-rw-r--r--   0 runner    (1001) docker     (127)     9691 2024-05-22 15:04:57.421279 vantage6-client-4.5.0rc3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 15:04:57.421279 vantage6-client-4.5.0rc3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-05-22 15:04:46.000000 vantage6-client-4.5.0rc3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:57.417279 vantage6-client-4.5.0rc3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4699 2024-05-22 15:04:46.000000 vantage6-client-4.5.0rc3/tests/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:57.417279 vantage6-client-4.5.0rc3/vantage6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:57.421279 vantage6-client-4.5.0rc3/vantage6/client/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 15:04:46.000000 vantage6-client-4.5.0rc3/vantage6/client/__build__
+-rw-r--r--   0 runner    (1001) docker     (127)    68221 2024-05-22 15:04:46.000000 vantage6-client-4.5.0rc3/vantage6/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-22 15:04:46.000000 vantage6-client-4.5.0rc3/vantage6/client/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-22 15:04:46.000000 vantage6-client-4.5.0rc3/vantage6/client/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8013 2024-05-22 15:04:46.000000 vantage6-client-4.5.0rc3/vantage6/client/filter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:57.421279 vantage6-client-4.5.0rc3/vantage6/client/subclients/
+-rw-r--r--   0 runner    (1001) docker     (127)     9338 2024-05-22 15:04:46.000000 vantage6-client-4.5.0rc3/vantage6/client/subclients/algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7592 2024-05-22 15:04:46.000000 vantage6-client-4.5.0rc3/vantage6/client/subclients/algorithm_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-05-22 15:04:46.000000 vantage6-client-4.5.0rc3/vantage6/client/subclients/store_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-05-22 15:04:46.000000 vantage6-client-4.5.0rc3/vantage6/client/subclients/store_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3451 2024-05-22 15:04:46.000000 vantage6-client-4.5.0rc3/vantage6/client/subclients/store_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5472 2024-05-22 15:04:46.000000 vantage6-client-4.5.0rc3/vantage6/client/subclients/study.py
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-22 15:04:46.000000 vantage6-client-4.5.0rc3/vantage6/client/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:57.421279 vantage6-client-4.5.0rc3/vantage6_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9691 2024-05-22 15:04:57.000000 vantage6-client-4.5.0rc3/vantage6_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-22 15:04:57.000000 vantage6-client-4.5.0rc3/vantage6_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 15:04:57.000000 vantage6-client-4.5.0rc3/vantage6_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-22 15:04:57.000000 vantage6-client-4.5.0rc3/vantage6_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-22 15:04:57.000000 vantage6-client-4.5.0rc3/vantage6_client.egg-info/top_level.txt
```

### Comparing `vantage6-client-4.5.0/PKG-INFO` & `vantage6-client-4.5.0rc3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantage6-client
-Version: 4.5.0
+Version: 4.5.0rc3
 Summary: Vantage6 client
 Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 <h1 align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vantage6-client Version: 4.5.0 Summary: Vantage6
+Metadata-Version: 2.1 Name: vantage6-client Version: 4.5.0rc3 Summary: Vantage6
 client Home-page: https://github.com/vantage6/vantage6 Requires-Python: >=3.10
 Description-Content-Type: text/markdown Provides-Extra: dev
                                     ************
                                _[[_vv_aa_nn_tt_aa_gg_ee_66_]] ************
       ******** AA PPrriivvaaccyy EEnnhhaanncciinngg TTeecchhnnoollooggyy ((PPEETT)) OOppeerraattiioonnss ppllaattffoorrmm ********
    ******** [[!![[RReelleeaassee]]((hhttttppss::////ggiitthhuubb..ccoomm//vvaannttaaggee66//vvaannttaaggee66//aaccttiioonnss//wwoorrkkfflloowwss//
 rreelleeaassee..yymmll//bbaaddggee..ssvvgg))]]((hhttttppss::////ggiitthhuubb..ccoomm//vvaannttaaggee66//vvaannttaaggee66//aaccttiioonnss//wwoorrkkfflloowwss//
```

### Comparing `vantage6-client-4.5.0/setup.py` & `vantage6-client-4.5.0rc3/setup.py`

 * *Files identical despite different names*

### Comparing `vantage6-client-4.5.0/tests/test_client.py` & `vantage6-client-4.5.0rc3/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `vantage6-client-4.5.0/vantage6/client/__init__.py` & `vantage6-client-4.5.0rc3/vantage6/client/__init__.py`

 * *Files identical despite different names*

### Comparing `vantage6-client-4.5.0/vantage6/client/_version.py` & `vantage6-client-4.5.0rc3/vantage6/client/_version.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with open(os.path.join(here, "__build__")) as fp:
     __build__ = json.load(fp)
 
 # Module version
-version_info = (4, 5, 0, "final", __build__, 0)
+version_info = (4, 5, 0, "candidate", __build__, 0)
 
 # Module version stage suffix map
 _specifier_ = {"alpha": "a", "beta": "b", "candidate": "rc", "final": ""}
 version = f"{version_info[0]}.{version_info[1]}.{version_info[2]}"
 pre_release = (
     ""
     if version_info[3] == "final"
```

### Comparing `vantage6-client-4.5.0/vantage6/client/filter.py` & `vantage6-client-4.5.0rc3/vantage6/client/filter.py`

 * *Files identical despite different names*

### Comparing `vantage6-client-4.5.0/vantage6/client/subclients/algorithm.py` & `vantage6-client-4.5.0rc3/vantage6/client/subclients/algorithm.py`

 * *Files 2% similar despite different names*

```diff
@@ -180,20 +180,20 @@
             is_for_algorithm_store=True,
             headers=self.parent.util._get_server_url_header(),
         )
 
     def update(
         self,
         id_: int,
-        name: str = None,
-        description: str = None,
-        image: str = None,
-        partitioning: str = None,
-        vantage6_version: str = None,
-        functions: List[dict] = None,
+        name: str,
+        description: str,
+        image: str,
+        partitioning: str,
+        vantage6_version: str,
+        functions: List[dict],
     ) -> dict:
         """
         Update an algorithm in the algorithm store
 
         Parameters
         ----------
         id_ : int
@@ -254,28 +254,21 @@
                         List of column names to visualize
 
         Returns
         -------
         dict
             The updated algorithm
         """
-        body = {}
-        if name:
-            body["name"] = name
-        if description:
-            body["description"] = description
-        if image:
-            body["image"] = image
-        if partitioning:
-            body["partitioning"] = partitioning
-        if vantage6_version:
-            body["vantage6_version"] = vantage6_version
-        if functions:
-            body["functions"] = functions
-
         return self.parent.request(
             f"algorithm/{id_}",
             method="PATCH",
             is_for_algorithm_store=True,
             headers=self.parent.util._get_server_url_header(),
-            json=body,
+            json={
+                "name": name,
+                "image": image,
+                "partitioning": partitioning,
+                "vantage6_version": vantage6_version,
+                "functions": functions,
+                "description": description,
+            },
         )
```

### Comparing `vantage6-client-4.5.0/vantage6/client/subclients/algorithm_store.py` & `vantage6-client-4.5.0rc3/vantage6/client/subclients/algorithm_store.py`

 * *Files identical despite different names*

### Comparing `vantage6-client-4.5.0/vantage6/client/subclients/store_role.py` & `vantage6-client-4.5.0rc3/vantage6/client/subclients/store_role.py`

 * *Files identical despite different names*

### Comparing `vantage6-client-4.5.0/vantage6/client/subclients/store_rule.py` & `vantage6-client-4.5.0rc3/vantage6/client/subclients/store_rule.py`

 * *Files identical despite different names*

### Comparing `vantage6-client-4.5.0/vantage6/client/subclients/store_user.py` & `vantage6-client-4.5.0rc3/vantage6/client/subclients/store_user.py`

 * *Files identical despite different names*

### Comparing `vantage6-client-4.5.0/vantage6/client/subclients/study.py` & `vantage6-client-4.5.0rc3/vantage6/client/subclients/study.py`

 * *Files identical despite different names*

### Comparing `vantage6-client-4.5.0/vantage6_client.egg-info/PKG-INFO` & `vantage6-client-4.5.0rc3/vantage6_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantage6-client
-Version: 4.5.0
+Version: 4.5.0rc3
 Summary: Vantage6 client
 Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 <h1 align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vantage6-client Version: 4.5.0 Summary: Vantage6
+Metadata-Version: 2.1 Name: vantage6-client Version: 4.5.0rc3 Summary: Vantage6
 client Home-page: https://github.com/vantage6/vantage6 Requires-Python: >=3.10
 Description-Content-Type: text/markdown Provides-Extra: dev
                                     ************
                                _[[_vv_aa_nn_tt_aa_gg_ee_66_]] ************
       ******** AA PPrriivvaaccyy EEnnhhaanncciinngg TTeecchhnnoollooggyy ((PPEETT)) OOppeerraattiioonnss ppllaattffoorrmm ********
    ******** [[!![[RReelleeaassee]]((hhttttppss::////ggiitthhuubb..ccoomm//vvaannttaaggee66//vvaannttaaggee66//aaccttiioonnss//wwoorrkkfflloowwss//
 rreelleeaassee..yymmll//bbaaddggee..ssvvgg))]]((hhttttppss::////ggiitthhuubb..ccoomm//vvaannttaaggee66//vvaannttaaggee66//aaccttiioonnss//wwoorrkkfflloowwss//
```

### Comparing `vantage6-client-4.5.0/vantage6_client.egg-info/SOURCES.txt` & `vantage6-client-4.5.0rc3/vantage6_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

