# Comparing `tmp/vantage6-algorithm-tools-4.5.0.tar.gz` & `tmp/vantage6-algorithm-tools-4.5.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vantage6-algorithm-tools-4.5.0.tar", last modified: Thu May 23 15:14:48 2024, max compression
+gzip compressed data, was "vantage6-algorithm-tools-4.5.0rc3.tar", last modified: Wed May 22 15:04:57 2024, max compression
```

## Comparing `vantage6-algorithm-tools-4.5.0.tar` & `vantage6-algorithm-tools-4.5.0rc3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:14:48.522662 vantage6-algorithm-tools-4.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     9705 2024-05-23 15:14:48.522662 vantage6-algorithm-tools-4.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 15:14:48.522662 vantage6-algorithm-tools-4.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-05-23 15:14:32.000000 vantage6-algorithm-tools-4.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:14:48.518662 vantage6-algorithm-tools-4.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-23 15:14:32.000000 vantage6-algorithm-tools-4.5.0/tests/algorithm_module.py
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-23 15:14:32.000000 vantage6-algorithm-tools-4.5.0/tests/test_deserialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-05-23 15:14:32.000000 vantage6-algorithm-tools-4.5.0/tests/test_docker_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-23 15:14:32.000000 vantage6-algorithm-tools-4.5.0/tests/test_serialization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:14:48.518662 vantage6-algorithm-tools-4.5.0/vantage6/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:14:48.518662 vantage6-algorithm-tools-4.5.0/vantage6/algorithm/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:14:48.518662 vantage6-algorithm-tools-4.5.0/vantage6/algorithm/client/
--rw-r--r--   0 runner    (1001) docker     (127)    23970 2024-05-23 15:14:32.000000 vantage6-algorithm-tools-4.5.0/vantage6/algorithm/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-23 15:14:32.000000 vantage6-algorithm-tools-4.5.0/vantage6/algorithm/client/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:14:48.522662 vantage6-algorithm-tools-4.5.0/vantage6/algorithm/tools/
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-23 15:14:32.000000 vantage6-algorithm-tools-4.5.0/vantage6/algorithm/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17141 2024-05-23 15:14:32.000000 vantage6-algorithm-tools-4.5.0/vantage6/algorithm/tools/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     4161 2024-05-23 15:14:32.000000 vantage6-algorithm-tools-4.5.0/vantage6/algorithm/tools/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    23495 2024-05-23 15:14:32.000000 vantage6-algorithm-tools-4.5.0/vantage6/algorithm/tools/mock_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:14:48.522662 vantage6-algorithm-tools-4.5.0/vantage6/algorithm/tools/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-05-23 15:14:32.000000 vantage6-algorithm-tools-4.5.0/vantage6/algorithm/tools/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-05-23 15:14:32.000000 vantage6-algorithm-tools-4.5.0/vantage6/algorithm/tools/preprocessing/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4638 2024-05-23 15:14:32.000000 vantage6-algorithm-tools-4.5.0/vantage6/algorithm/tools/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     6423 2024-05-23 15:14:32.000000 vantage6-algorithm-tools-4.5.0/vantage6/algorithm/tools/wrap.py
--rw-r--r--   0 runner    (1001) docker     (127)     8746 2024-05-23 15:14:32.000000 vantage6-algorithm-tools-4.5.0/vantage6/algorithm/tools/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:14:48.522662 vantage6-algorithm-tools-4.5.0/vantage6_algorithm_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9705 2024-05-23 15:14:48.000000 vantage6-algorithm-tools-4.5.0/vantage6_algorithm_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-23 15:14:48.000000 vantage6-algorithm-tools-4.5.0/vantage6_algorithm_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 15:14:48.000000 vantage6-algorithm-tools-4.5.0/vantage6_algorithm_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-23 15:14:48.000000 vantage6-algorithm-tools-4.5.0/vantage6_algorithm_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-23 15:14:48.000000 vantage6-algorithm-tools-4.5.0/vantage6_algorithm_tools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:57.813282 vantage6-algorithm-tools-4.5.0rc3/
+-rw-r--r--   0 runner    (1001) docker     (127)     9708 2024-05-22 15:04:57.813282 vantage6-algorithm-tools-4.5.0rc3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 15:04:57.813282 vantage6-algorithm-tools-4.5.0rc3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-05-22 15:04:46.000000 vantage6-algorithm-tools-4.5.0rc3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:57.809282 vantage6-algorithm-tools-4.5.0rc3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-22 15:04:46.000000 vantage6-algorithm-tools-4.5.0rc3/tests/algorithm_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-22 15:04:46.000000 vantage6-algorithm-tools-4.5.0rc3/tests/test_deserialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4254 2024-05-22 15:04:46.000000 vantage6-algorithm-tools-4.5.0rc3/tests/test_docker_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-22 15:04:46.000000 vantage6-algorithm-tools-4.5.0rc3/tests/test_serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:57.809282 vantage6-algorithm-tools-4.5.0rc3/vantage6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:57.809282 vantage6-algorithm-tools-4.5.0rc3/vantage6/algorithm/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:57.809282 vantage6-algorithm-tools-4.5.0rc3/vantage6/algorithm/client/
+-rw-r--r--   0 runner    (1001) docker     (127)    23970 2024-05-22 15:04:46.000000 vantage6-algorithm-tools-4.5.0rc3/vantage6/algorithm/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-22 15:04:46.000000 vantage6-algorithm-tools-4.5.0rc3/vantage6/algorithm/client/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:57.813282 vantage6-algorithm-tools-4.5.0rc3/vantage6/algorithm/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-22 15:04:46.000000 vantage6-algorithm-tools-4.5.0rc3/vantage6/algorithm/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17141 2024-05-22 15:04:46.000000 vantage6-algorithm-tools-4.5.0rc3/vantage6/algorithm/tools/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4161 2024-05-22 15:04:46.000000 vantage6-algorithm-tools-4.5.0rc3/vantage6/algorithm/tools/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23350 2024-05-22 15:04:46.000000 vantage6-algorithm-tools-4.5.0rc3/vantage6/algorithm/tools/mock_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:57.813282 vantage6-algorithm-tools-4.5.0rc3/vantage6/algorithm/tools/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-05-22 15:04:46.000000 vantage6-algorithm-tools-4.5.0rc3/vantage6/algorithm/tools/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-05-22 15:04:46.000000 vantage6-algorithm-tools-4.5.0rc3/vantage6/algorithm/tools/preprocessing/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4638 2024-05-22 15:04:46.000000 vantage6-algorithm-tools-4.5.0rc3/vantage6/algorithm/tools/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6423 2024-05-22 15:04:46.000000 vantage6-algorithm-tools-4.5.0rc3/vantage6/algorithm/tools/wrap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8746 2024-05-22 15:04:46.000000 vantage6-algorithm-tools-4.5.0rc3/vantage6/algorithm/tools/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:04:57.813282 vantage6-algorithm-tools-4.5.0rc3/vantage6_algorithm_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9708 2024-05-22 15:04:57.000000 vantage6-algorithm-tools-4.5.0rc3/vantage6_algorithm_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-22 15:04:57.000000 vantage6-algorithm-tools-4.5.0rc3/vantage6_algorithm_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 15:04:57.000000 vantage6-algorithm-tools-4.5.0rc3/vantage6_algorithm_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-22 15:04:57.000000 vantage6-algorithm-tools-4.5.0rc3/vantage6_algorithm_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-22 15:04:57.000000 vantage6-algorithm-tools-4.5.0rc3/vantage6_algorithm_tools.egg-info/top_level.txt
```

### Comparing `vantage6-algorithm-tools-4.5.0/PKG-INFO` & `vantage6-algorithm-tools-4.5.0rc3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantage6-algorithm-tools
-Version: 4.5.0
+Version: 4.5.0rc3
 Summary: Vantage6 algorithm tools
 Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 <h1 align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vantage6-algorithm-tools Version: 4.5.0 Summary:
+Metadata-Version: 2.1 Name: vantage6-algorithm-tools Version: 4.5.0rc3 Summary:
 Vantage6 algorithm tools Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.6 Description-Content-Type: text/markdown Provides-Extra:
 dev
                                     ************
                                _[[_vv_aa_nn_tt_aa_gg_ee_66_]] ************
       ******** AA PPrriivvaaccyy EEnnhhaanncciinngg TTeecchhnnoollooggyy ((PPEETT)) OOppeerraattiioonnss ppllaattffoorrmm ********
    ******** [[!![[RReelleeaassee]]((hhttttppss::////ggiitthhuubb..ccoomm//vvaannttaaggee66//vvaannttaaggee66//aaccttiioonnss//wwoorrkkfflloowwss//
```

### Comparing `vantage6-algorithm-tools-4.5.0/setup.py` & `vantage6-algorithm-tools-4.5.0rc3/setup.py`

 * *Files identical despite different names*

### Comparing `vantage6-algorithm-tools-4.5.0/tests/test_docker_wrapper.py` & `vantage6-algorithm-tools-4.5.0rc3/tests/test_docker_wrapper.py`

 * *Files identical despite different names*

### Comparing `vantage6-algorithm-tools-4.5.0/tests/test_serialization.py` & `vantage6-algorithm-tools-4.5.0rc3/tests/test_serialization.py`

 * *Files identical despite different names*

### Comparing `vantage6-algorithm-tools-4.5.0/vantage6/algorithm/client/__init__.py` & `vantage6-algorithm-tools-4.5.0rc3/vantage6/algorithm/client/__init__.py`

 * *Files identical despite different names*

### Comparing `vantage6-algorithm-tools-4.5.0/vantage6/algorithm/client/_version.py` & `vantage6-algorithm-tools-4.5.0rc3/vantage6/algorithm/client/_version.py`

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

### Comparing `vantage6-algorithm-tools-4.5.0/vantage6/algorithm/tools/decorators.py` & `vantage6-algorithm-tools-4.5.0rc3/vantage6/algorithm/tools/decorators.py`

 * *Files identical despite different names*

### Comparing `vantage6-algorithm-tools-4.5.0/vantage6/algorithm/tools/exceptions.py` & `vantage6-algorithm-tools-4.5.0rc3/vantage6/algorithm/tools/exceptions.py`

 * *Files identical despite different names*

### Comparing `vantage6-algorithm-tools-4.5.0/vantage6/algorithm/tools/mock_client.py` & `vantage6-algorithm-tools-4.5.0rc3/vantage6/algorithm/tools/mock_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -235,17 +235,15 @@
 
                 # detect which decorators are used and provide the mock client
                 # and/or mocked data that is required to the method
                 mocked_kwargs = {}
                 if getattr(method, "wrapped_in_algorithm_client_decorator", False):
                     mocked_kwargs["mock_client"] = client_copy
                 if getattr(method, "wrapped_in_data_decorator", False):
-                    # make a copy of the data to avoid modifying the original data of
-                    # subsequent tasks
-                    mocked_kwargs["mock_data"] = [d.copy() for d in data]
+                    mocked_kwargs["mock_data"] = data
 
                 result = method(*args, **kwargs, **mocked_kwargs)
 
                 self.last_result_id += 1
                 self.parent.results.append(
                     {
                         "id": self.last_result_id,
```

### Comparing `vantage6-algorithm-tools-4.5.0/vantage6/algorithm/tools/preprocessing/__init__.py` & `vantage6-algorithm-tools-4.5.0rc3/vantage6/algorithm/tools/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `vantage6-algorithm-tools-4.5.0/vantage6/algorithm/tools/preprocessing/functions.py` & `vantage6-algorithm-tools-4.5.0rc3/vantage6/algorithm/tools/preprocessing/functions.py`

 * *Files identical despite different names*

### Comparing `vantage6-algorithm-tools-4.5.0/vantage6/algorithm/tools/util.py` & `vantage6-algorithm-tools-4.5.0rc3/vantage6/algorithm/tools/util.py`

 * *Files identical despite different names*

### Comparing `vantage6-algorithm-tools-4.5.0/vantage6/algorithm/tools/wrap.py` & `vantage6-algorithm-tools-4.5.0rc3/vantage6/algorithm/tools/wrap.py`

 * *Files identical despite different names*

### Comparing `vantage6-algorithm-tools-4.5.0/vantage6/algorithm/tools/wrappers.py` & `vantage6-algorithm-tools-4.5.0rc3/vantage6/algorithm/tools/wrappers.py`

 * *Files identical despite different names*

### Comparing `vantage6-algorithm-tools-4.5.0/vantage6_algorithm_tools.egg-info/PKG-INFO` & `vantage6-algorithm-tools-4.5.0rc3/vantage6_algorithm_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantage6-algorithm-tools
-Version: 4.5.0
+Version: 4.5.0rc3
 Summary: Vantage6 algorithm tools
 Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 <h1 align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: vantage6-algorithm-tools Version: 4.5.0 Summary:
+Metadata-Version: 2.1 Name: vantage6-algorithm-tools Version: 4.5.0rc3 Summary:
 Vantage6 algorithm tools Home-page: https://github.com/vantage6/vantage6
 Requires-Python: >=3.6 Description-Content-Type: text/markdown Provides-Extra:
 dev
                                     ************
                                _[[_vv_aa_nn_tt_aa_gg_ee_66_]] ************
       ******** AA PPrriivvaaccyy EEnnhhaanncciinngg TTeecchhnnoollooggyy ((PPEETT)) OOppeerraattiioonnss ppllaattffoorrmm ********
    ******** [[!![[RReelleeaassee]]((hhttttppss::////ggiitthhuubb..ccoomm//vvaannttaaggee66//vvaannttaaggee66//aaccttiioonnss//wwoorrkkfflloowwss//
```

### Comparing `vantage6-algorithm-tools-4.5.0/vantage6_algorithm_tools.egg-info/SOURCES.txt` & `vantage6-algorithm-tools-4.5.0rc3/vantage6_algorithm_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

