# Comparing `tmp/privue-0.1.tar.gz` & `tmp/privue-0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "privue-0.1.tar", last modified: Thu May 23 17:19:02 2024, max compression
+gzip compressed data, was "privue-0.11.tar", last modified: Thu May 23 17:28:19 2024, max compression
```

## Comparing `privue-0.1.tar` & `privue-0.11.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 17:19:02.233744 privue-0.1/
--rw-rw-rw-   0        0        0       51 2024-05-23 17:19:02.232746 privue-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-23 17:19:02.165958 privue-0.1/privue/
--rw-rw-rw-   0        0        0        0 2024-05-22 21:43:34.000000 privue-0.1/privue/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 17:19:02.191195 privue-0.1/privue/client/
--rw-rw-rw-   0        0        0      159 2024-05-22 21:59:04.000000 privue-0.1/privue/client/__init__.py
--rw-rw-rw-   0        0        0     8929 2024-05-23 17:16:52.000000 privue-0.1/privue/client/client.py
-drwxrwxrwx   0        0        0        0 2024-05-23 17:19:02.220139 privue-0.1/privue/errors/
--rw-rw-rw-   0        0        0       40 2024-05-22 21:59:10.000000 privue-0.1/privue/errors/__init__.py
--rw-rw-rw-   0        0        0       48 2024-05-22 21:50:56.000000 privue-0.1/privue/errors/errors.py
-drwxrwxrwx   0        0        0        0 2024-05-23 17:19:02.226151 privue-0.1/privue/server/
--rw-rw-rw-   0        0        0      119 2024-05-22 21:59:23.000000 privue-0.1/privue/server/__init__.py
--rw-rw-rw-   0        0        0     8170 2024-05-23 17:17:00.000000 privue-0.1/privue/server/server.py
-drwxrwxrwx   0        0        0        0 2024-05-23 17:19:02.230749 privue-0.1/privue/util/
--rw-rw-rw-   0        0        0      190 2024-05-23 12:25:50.000000 privue-0.1/privue/util/__init__.py
--rw-rw-rw-   0        0        0    11652 2024-05-23 17:17:09.000000 privue-0.1/privue/util/util.py
-drwxrwxrwx   0        0        0        0 2024-05-23 17:19:02.187206 privue-0.1/privue.egg-info/
--rw-rw-rw-   0        0        0       51 2024-05-23 17:19:02.000000 privue-0.1/privue.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      370 2024-05-23 17:19:02.000000 privue-0.1/privue.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 17:19:02.000000 privue-0.1/privue.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-05-23 17:19:02.000000 privue-0.1/privue.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-23 17:19:02.000000 privue-0.1/privue.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-23 17:19:02.233744 privue-0.1/setup.cfg
--rw-rw-rw-   0        0        0      149 2024-05-23 17:16:34.000000 privue-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 17:28:19.729409 privue-0.11/
+-rw-rw-rw-   0        0        0      140 2024-05-23 17:28:19.728411 privue-0.11/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-23 17:28:19.687521 privue-0.11/privue/
+-rw-rw-rw-   0        0        0        0 2024-05-22 21:43:34.000000 privue-0.11/privue/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 17:28:19.715446 privue-0.11/privue/client/
+-rw-rw-rw-   0        0        0      140 2024-05-23 17:24:19.000000 privue-0.11/privue/client/__init__.py
+-rw-rw-rw-   0        0        0     8929 2024-05-23 17:16:52.000000 privue-0.11/privue/client/client.py
+drwxrwxrwx   0        0        0        0 2024-05-23 17:28:19.719434 privue-0.11/privue/errors/
+-rw-rw-rw-   0        0        0       40 2024-05-22 21:59:10.000000 privue-0.11/privue/errors/__init__.py
+-rw-rw-rw-   0        0        0       48 2024-05-22 21:50:56.000000 privue-0.11/privue/errors/errors.py
+drwxrwxrwx   0        0        0        0 2024-05-23 17:28:19.723424 privue-0.11/privue/server/
+-rw-rw-rw-   0        0        0      119 2024-05-22 21:59:23.000000 privue-0.11/privue/server/__init__.py
+-rw-rw-rw-   0        0        0     8170 2024-05-23 17:17:00.000000 privue-0.11/privue/server/server.py
+drwxrwxrwx   0        0        0        0 2024-05-23 17:28:19.726416 privue-0.11/privue/util/
+-rw-rw-rw-   0        0        0      187 2024-05-23 17:25:01.000000 privue-0.11/privue/util/__init__.py
+-rw-rw-rw-   0        0        0    11646 2024-05-23 17:25:28.000000 privue-0.11/privue/util/util.py
+drwxrwxrwx   0        0        0        0 2024-05-23 17:28:19.710465 privue-0.11/privue.egg-info/
+-rw-rw-rw-   0        0        0      140 2024-05-23 17:28:19.000000 privue-0.11/privue.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      370 2024-05-23 17:28:19.000000 privue-0.11/privue.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 17:28:19.000000 privue-0.11/privue.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-05-23 17:28:19.000000 privue-0.11/privue.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 17:28:19.000000 privue-0.11/privue.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-23 17:28:19.729409 privue-0.11/setup.cfg
+-rw-rw-rw-   0        0        0      150 2024-05-23 17:27:46.000000 privue-0.11/setup.py
```

### Comparing `privue-0.1/privue/client/client.py` & `privue-0.11/privue/client/client.py`

 * *Files identical despite different names*

### Comparing `privue-0.1/privue/server/server.py` & `privue-0.11/privue/server/server.py`

 * *Files identical despite different names*

### Comparing `privue-0.1/privue/util/util.py` & `privue-0.11/privue/util/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 import numpy as np
 import pandas as pd
 import privue.client.client as client
 import privue.server.server as server
 from typing import List, Dict
 
 
-def privatize_json_string(input_json_str : str, epsilon : float, max_value_per_attr_list : List[float], min_value_per_attr_list : List[float], bucket_amount_per_attr_list : List[int]):
+def privatize_json_str(input_json_str : str, epsilon : float, max_value_per_attr_list : List[float], min_value_per_attr_list : List[float], bucket_amount_per_attr_list : List[int]):
     """Returns a JSON string of the required format for estimation
 
     This function is a generalized version of the get_private_vector_multiple_attr function,
     which accommodates JSON string, in the specified format for privatization, as input. 
     It receives a list for each property and a list of values which correspond in their order.
     The epsilon privacy budget is shared across all values, as described in the spl technique - guaranteeing the entire array of privatized values is epsilon-LDP.
 
@@ -80,15 +80,15 @@
         An array of privatized binary vectors, which satisfies epsilon-LDP definition.
         
     Raises:
         ValuePropertyMissing: If a value is missing one of it's properties (number of values must be non-zero)
     """
     with open(input_json_file_path, 'r') as input_json_str:
         input_json_str = input_json_str.read()
-    return privatize_json_string(input_json_str, epsilon, max_value_per_attr_list, min_value_per_attr_list, bucket_amount_per_attr_list)
+    return privatize_json_str(input_json_str, epsilon, max_value_per_attr_list, min_value_per_attr_list, bucket_amount_per_attr_list)
    
         
 def _get_tensor_list_from_privatized_json_obj(input_json_obj : Dict) -> List[np.ndarray]:
     """Returns a NDarray list required for average estimation from JSON object.
 
     Args:
         input_json_obj: a JSON object of the required format for estimation
```

