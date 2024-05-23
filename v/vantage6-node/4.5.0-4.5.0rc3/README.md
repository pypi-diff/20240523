# Comparing `tmp/vantage6-node-4.5.0.tar.gz` & `tmp/vantage6-node-4.5.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vantage6-node-4.5.0.tar", last modified: Thu May 23 15:14:49 2024, max compression
+gzip compressed data, was "vantage6-node-4.5.0rc3.tar", last modified: Wed May 22 15:04:58 2024, max compression
```

## Comparing `vantage6-node-4.5.0.tar` & `vantage6-node-4.5.0rc3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:14:49.374664 vantage6-node-4.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     9684 2024-05-23 15:14:49.374664 vantage6-node-4.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 15:14:49.374664 vantage6-node-4.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-05-23 15:14:32.000000 vantage6-node-4.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:14:49.370664 vantage6-node-4.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 15:14:32.000000 vantage6-node-4.5.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 15:14:32.000000 vantage6-node-4.5.0/tests/test_ssh_tunnel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:14:49.366664 vantage6-node-4.5.0/vantage6/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:14:49.370664 vantage6-node-4.5.0/vantage6/node/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 15:14:32.000000 vantage6-node-4.5.0/vantage6/node/__build__
--rw-r--r--   0 runner    (1001) docker     (127)    42130 2024-05-23 15:14:32.000000 vantage6-node-4.5.0/vantage6/node/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-23 15:14:32.000000 vantage6-node-4.5.0/vantage6/node/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:14:49.370664 vantage6-node-4.5.0/vantage6/node/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 15:14:32.000000 vantage6-node-4.5.0/vantage6/node/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6988 2024-05-23 15:14:32.000000 vantage6-node-4.5.0/vantage6/node/cli/node.py
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-05-23 15:14:32.000000 vantage6-node-4.5.0/vantage6/node/context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:14:49.370664 vantage6-node-4.5.0/vantage6/node/docker/
--rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-05-23 15:14:32.000000 vantage6-node-4.5.0/vantage6/node/docker/docker_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    27837 2024-05-23 15:14:32.000000 vantage6-node-4.5.0/vantage6/node/docker/docker_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-23 15:14:32.000000 vantage6-node-4.5.0/vantage6/node/docker/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     9146 2024-05-23 15:14:32.000000 vantage6-node-4.5.0/vantage6/node/docker/squid.py
--rw-r--r--   0 runner    (1001) docker     (127)     9601 2024-05-23 15:14:32.000000 vantage6-node-4.5.0/vantage6/node/docker/ssh_tunnel.py
--rw-r--r--   0 runner    (1001) docker     (127)    25105 2024-05-23 15:14:32.000000 vantage6-node-4.5.0/vantage6/node/docker/task_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    25549 2024-05-23 15:14:32.000000 vantage6-node-4.5.0/vantage6/node/docker/vpn_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-05-23 15:14:32.000000 vantage6-node-4.5.0/vantage6/node/globals.py
--rw-r--r--   0 runner    (1001) docker     (127)    12047 2024-05-23 15:14:32.000000 vantage6-node-4.5.0/vantage6/node/proxy_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     6273 2024-05-23 15:14:32.000000 vantage6-node-4.5.0/vantage6/node/socket.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:14:49.370664 vantage6-node-4.5.0/vantage6/node/util/
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-23 15:14:32.000000 vantage6-node-4.5.0/vantage6/node/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3849 2024-05-23 15:14:32.000000 vantage6-node-4.5.0/vantage6/node/util/colorer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:14:49.374664 vantage6-node-4.5.0/vantage6_node.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9684 2024-05-23 15:14:49.000000 vantage6-node-4.5.0/vantage6_node.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      820 2024-05-23 15:14:49.000000 vantage6-node-4.5.0/vantage6_node.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 15:14:49.000000 vantage6-node-4.5.0/vantage6_node.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-23 15:14:49.000000 vantage6-node-4.5.0/vantage6_node.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-23 15:14:49.000000 vantage6-node-4.5.0/vantage6_node.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-23 15:14:49.000000 vantage6-node-4.5.0/vantage6_node.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:58.697289 vantage6-node-4.5.0rc3/
+-rw-r--r--   0 runner    (1001) docker     (127)     9687 2024-05-22 15:04:58.697289 vantage6-node-4.5.0rc3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 15:04:58.697289 vantage6-node-4.5.0rc3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-05-22 15:04:46.000000 vantage6-node-4.5.0rc3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:58.693289 vantage6-node-4.5.0rc3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:46.000000 vantage6-node-4.5.0rc3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:46.000000 vantage6-node-4.5.0rc3/tests/test_ssh_tunnel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:58.693289 vantage6-node-4.5.0rc3/vantage6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:58.693289 vantage6-node-4.5.0rc3/vantage6/node/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 15:04:46.000000 vantage6-node-4.5.0rc3/vantage6/node/__build__
+-rw-r--r--   0 runner    (1001) docker     (127)    42130 2024-05-22 15:04:46.000000 vantage6-node-4.5.0rc3/vantage6/node/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-22 15:04:46.000000 vantage6-node-4.5.0rc3/vantage6/node/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:58.693289 vantage6-node-4.5.0rc3/vantage6/node/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:46.000000 vantage6-node-4.5.0rc3/vantage6/node/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6988 2024-05-22 15:04:46.000000 vantage6-node-4.5.0rc3/vantage6/node/cli/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-05-22 15:04:46.000000 vantage6-node-4.5.0rc3/vantage6/node/context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:58.697289 vantage6-node-4.5.0rc3/vantage6/node/docker/
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-05-22 15:04:46.000000 vantage6-node-4.5.0rc3/vantage6/node/docker/docker_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27837 2024-05-22 15:04:46.000000 vantage6-node-4.5.0rc3/vantage6/node/docker/docker_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-22 15:04:46.000000 vantage6-node-4.5.0rc3/vantage6/node/docker/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9146 2024-05-22 15:04:46.000000 vantage6-node-4.5.0rc3/vantage6/node/docker/squid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9601 2024-05-22 15:04:46.000000 vantage6-node-4.5.0rc3/vantage6/node/docker/ssh_tunnel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25105 2024-05-22 15:04:46.000000 vantage6-node-4.5.0rc3/vantage6/node/docker/task_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25549 2024-05-22 15:04:46.000000 vantage6-node-4.5.0rc3/vantage6/node/docker/vpn_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-05-22 15:04:46.000000 vantage6-node-4.5.0rc3/vantage6/node/globals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12125 2024-05-22 15:04:46.000000 vantage6-node-4.5.0rc3/vantage6/node/proxy_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6273 2024-05-22 15:04:46.000000 vantage6-node-4.5.0rc3/vantage6/node/socket.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:58.697289 vantage6-node-4.5.0rc3/vantage6/node/util/
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-22 15:04:46.000000 vantage6-node-4.5.0rc3/vantage6/node/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3849 2024-05-22 15:04:46.000000 vantage6-node-4.5.0rc3/vantage6/node/util/colorer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:58.697289 vantage6-node-4.5.0rc3/vantage6_node.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9687 2024-05-22 15:04:58.000000 vantage6-node-4.5.0rc3/vantage6_node.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-05-22 15:04:58.000000 vantage6-node-4.5.0rc3/vantage6_node.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 15:04:58.000000 vantage6-node-4.5.0rc3/vantage6_node.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-22 15:04:58.000000 vantage6-node-4.5.0rc3/vantage6_node.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      301 2024-05-22 15:04:58.000000 vantage6-node-4.5.0rc3/vantage6_node.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-22 15:04:58.000000 vantage6-node-4.5.0rc3/vantage6_node.egg-info/top_level.txt
```

### Comparing `vantage6-node-4.5.0/PKG-INFO` & `vantage6-node-4.5.0rc3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantage6-node
-Version: 4.5.0
+Version: 4.5.0rc3
 Summary: vantage6 node
 Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 <h1 align="center">
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: vantage6-node Version: 4.5.0 Summary: vantage6 node
-Home-page: https://github.com/vantage6/vantage6 Requires-Python: >=3.10
+Metadata-Version: 2.1 Name: vantage6-node Version: 4.5.0rc3 Summary: vantage6
+node Home-page: https://github.com/vantage6/vantage6 Requires-Python: >=3.10
 Description-Content-Type: text/markdown Provides-Extra: dev
                                     ************
                                _[[_vv_aa_nn_tt_aa_gg_ee_66_]] ************
       ******** AA PPrriivvaaccyy EEnnhhaanncciinngg TTeecchhnnoollooggyy ((PPEETT)) OOppeerraattiioonnss ppllaattffoorrmm ********
    ******** [[!![[RReelleeaassee]]((hhttttppss::////ggiitthhuubb..ccoomm//vvaannttaaggee66//vvaannttaaggee66//aaccttiioonnss//wwoorrkkfflloowwss//
 rreelleeaassee..yymmll//bbaaddggee..ssvvgg))]]((hhttttppss::////ggiitthhuubb..ccoomm//vvaannttaaggee66//vvaannttaaggee66//aaccttiioonnss//wwoorrkkfflloowwss//
 rreelleeaassee..yymmll)) [[!![[PPyyPPII vvaannttaaggee66]]((hhttttppss::////bbaaddggee..ffuurryy..iioo//ppyy//vvaannttaaggee66..ssvvgg))]]((hhttttppss::////
```

### Comparing `vantage6-node-4.5.0/setup.py` & `vantage6-node-4.5.0rc3/setup.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-4.5.0/vantage6/node/__init__.py` & `vantage6-node-4.5.0rc3/vantage6/node/__init__.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-4.5.0/vantage6/node/_version.py` & `vantage6-node-4.5.0rc3/vantage6/node/_version.py`

 * *Files 2% similar despite different names*

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

### Comparing `vantage6-node-4.5.0/vantage6/node/cli/node.py` & `vantage6-node-4.5.0rc3/vantage6/node/cli/node.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-4.5.0/vantage6/node/context.py` & `vantage6-node-4.5.0rc3/vantage6/node/context.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-4.5.0/vantage6/node/docker/docker_base.py` & `vantage6-node-4.5.0rc3/vantage6/node/docker/docker_base.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-4.5.0/vantage6/node/docker/docker_manager.py` & `vantage6-node-4.5.0rc3/vantage6/node/docker/docker_manager.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-4.5.0/vantage6/node/docker/exceptions.py` & `vantage6-node-4.5.0rc3/vantage6/node/docker/exceptions.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-4.5.0/vantage6/node/docker/squid.py` & `vantage6-node-4.5.0rc3/vantage6/node/docker/squid.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-4.5.0/vantage6/node/docker/ssh_tunnel.py` & `vantage6-node-4.5.0rc3/vantage6/node/docker/ssh_tunnel.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-4.5.0/vantage6/node/docker/task_manager.py` & `vantage6-node-4.5.0rc3/vantage6/node/docker/task_manager.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-4.5.0/vantage6/node/docker/vpn_manager.py` & `vantage6-node-4.5.0rc3/vantage6/node/docker/vpn_manager.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-4.5.0/vantage6/node/globals.py` & `vantage6-node-4.5.0rc3/vantage6/node/globals.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-4.5.0/vantage6/node/proxy_server.py` & `vantage6-node-4.5.0rc3/vantage6/node/proxy_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -292,15 +292,15 @@
         response = make_request("post", "task", data, headers=headers)
     except Exception:
         log.exception("post task failed")
         return {
             "msg": "Request failed, see node logs"
         }, HTTPStatus.INTERNAL_SERVER_ERROR
 
-    return response.content, response.status_code
+    return response.content, response.status_code, response.headers.items()
 
 
 @app.route("/result", methods=["GET"])
 def proxy_result() -> Response:
     """
     Obtain and decrypt all results to belong to a certain task
 
@@ -341,15 +341,15 @@
 
     # Attempt to decrypt the results. The endpoint should have returned
     # a list of results
     results = get_response_json_and_handle_exceptions(response)
     for result in results["data"]:
         result = decrypt_result(result)
 
-    return results, response.status_code
+    return results, response.status_code, response.headers.items()
 
 
 @app.route("/result/<int:id>", methods=["GET"])
 def proxy_results(id_: int) -> Response:
     """
     Obtain and decrypt the algorithm result from the vantage6 server to be used
     by an algorithm container.
@@ -380,15 +380,15 @@
             "msg": "Request failed, see node logs..."
         }, HTTPStatus.INTERNAL_SERVER_ERROR
 
     # Try to decrypt the results
     result = get_response_json_and_handle_exceptions(response)
     result = decrypt_result(result)
 
-    return result, response.status_code
+    return result, response.status_code, response.headers.items()
 
 
 @app.route(
     "/<path:central_server_path>", methods=["GET", "POST", "PATCH", "PUT", "DELETE"]
 )
 def proxy(central_server_path: str) -> Response:
     """
```

### Comparing `vantage6-node-4.5.0/vantage6/node/socket.py` & `vantage6-node-4.5.0rc3/vantage6/node/socket.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-4.5.0/vantage6/node/util/colorer.py` & `vantage6-node-4.5.0rc3/vantage6/node/util/colorer.py`

 * *Files identical despite different names*

### Comparing `vantage6-node-4.5.0/vantage6_node.egg-info/PKG-INFO` & `vantage6-node-4.5.0rc3/vantage6_node.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantage6-node
-Version: 4.5.0
+Version: 4.5.0rc3
 Summary: vantage6 node
 Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 <h1 align="center">
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
-Metadata-Version: 2.1 Name: vantage6-node Version: 4.5.0 Summary: vantage6 node
-Home-page: https://github.com/vantage6/vantage6 Requires-Python: >=3.10
+Metadata-Version: 2.1 Name: vantage6-node Version: 4.5.0rc3 Summary: vantage6
+node Home-page: https://github.com/vantage6/vantage6 Requires-Python: >=3.10
 Description-Content-Type: text/markdown Provides-Extra: dev
                                     ************
                                _[[_vv_aa_nn_tt_aa_gg_ee_66_]] ************
       ******** AA PPrriivvaaccyy EEnnhhaanncciinngg TTeecchhnnoollooggyy ((PPEETT)) OOppeerraattiioonnss ppllaattffoorrmm ********
    ******** [[!![[RReelleeaassee]]((hhttttppss::////ggiitthhuubb..ccoomm//vvaannttaaggee66//vvaannttaaggee66//aaccttiioonnss//wwoorrkkfflloowwss//
 rreelleeaassee..yymmll//bbaaddggee..ssvvgg))]]((hhttttppss::////ggiitthhuubb..ccoomm//vvaannttaaggee66//vvaannttaaggee66//aaccttiioonnss//wwoorrkkfflloowwss//
 rreelleeaassee..yymmll)) [[!![[PPyyPPII vvaannttaaggee66]]((hhttttppss::////bbaaddggee..ffuurryy..iioo//ppyy//vvaannttaaggee66..ssvvgg))]]((hhttttppss::////
```

### Comparing `vantage6-node-4.5.0/vantage6_node.egg-info/SOURCES.txt` & `vantage6-node-4.5.0rc3/vantage6_node.egg-info/SOURCES.txt`

 * *Files identical despite different names*

