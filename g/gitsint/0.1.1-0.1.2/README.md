# Comparing `tmp/gitsint-0.1.1.tar.gz` & `tmp/gitsint-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitsint-0.1.1.tar", max compression
+gzip compressed data, was "gitsint-0.1.2.tar", max compression
```

## Comparing `gitsint-0.1.1.tar` & `gitsint-0.1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1066 2024-05-20 15:53:16.177005 gitsint-0.1.1/LICENSE
--rw-r--r--   0        0        0    35149 2024-05-19 09:46:11.286809 gitsint-0.1.1/LICENSE.md
--rw-r--r--   0        0        0     4685 2024-05-20 21:27:19.000210 gitsint-0.1.1/README.md
--rw-r--r--   0        0        0     4685 2024-05-20 21:34:44.671467 gitsint-0.1.1/gitsint/README.md
--rw-r--r--   0        0        0    12459 2024-05-20 21:33:45.161504 gitsint-0.1.1/gitsint/__init__.py
--rw-r--r--   0        0        0      266 2024-05-19 09:46:11.286809 gitsint-0.1.1/gitsint/instruments.py
--rw-r--r--   0        0        0        0 2024-05-19 09:46:11.286809 gitsint-0.1.1/gitsint/modules/__init__.py
--rw-r--r--   0        0        0        0 2024-05-19 09:46:11.286809 gitsint-0.1.1/gitsint/modules/profile/__init__.py
--rw-r--r--   0        0        0     2453 2024-05-20 19:54:10.549360 gitsint-0.1.1/gitsint/modules/profile/friends.py
--rw-r--r--   0        0        0      385 2024-05-20 19:47:09.923659 gitsint-0.1.1/gitsint/modules/profile/profile.py
--rw-r--r--   0        0        0        0 2024-05-19 09:46:11.296809 gitsint-0.1.1/gitsint/modules/repos/__init__.py
--rw-r--r--   0        0        0     8601 2024-05-20 15:47:29.310895 gitsint-0.1.1/gitsint/modules/repos/repository.py
--rw-r--r--   0        0        0      858 2024-05-20 21:35:09.651617 gitsint-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     5616 1970-01-01 00:00:00.000000 gitsint-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-05-20 15:53:16.177005 gitsint-0.1.2/LICENSE
+-rw-r--r--   0        0        0    35149 2024-05-19 09:46:11.286809 gitsint-0.1.2/LICENSE.md
+-rw-r--r--   0        0        0     4685 2024-05-20 21:27:19.000210 gitsint-0.1.2/README.md
+-rw-r--r--   0        0        0     4685 2024-05-20 21:34:44.671467 gitsint-0.1.2/gitsint/README.md
+-rw-r--r--   0        0        0    12450 2024-05-23 20:39:33.885108 gitsint-0.1.2/gitsint/__init__.py
+-rw-r--r--   0        0        0      266 2024-05-19 09:46:11.286809 gitsint-0.1.2/gitsint/instruments.py
+-rw-r--r--   0        0        0        0 2024-05-19 09:46:11.286809 gitsint-0.1.2/gitsint/modules/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-19 09:46:11.286809 gitsint-0.1.2/gitsint/modules/profile/__init__.py
+-rw-r--r--   0        0        0     2453 2024-05-20 19:54:10.549360 gitsint-0.1.2/gitsint/modules/profile/friends.py
+-rw-r--r--   0        0        0      839 2024-05-23 20:38:59.876833 gitsint-0.1.2/gitsint/modules/profile/profile.py
+-rw-r--r--   0        0        0        0 2024-05-19 09:46:11.296809 gitsint-0.1.2/gitsint/modules/repos/__init__.py
+-rw-r--r--   0        0        0     8601 2024-05-20 15:47:29.310895 gitsint-0.1.2/gitsint/modules/repos/repository.py
+-rw-r--r--   0        0        0      858 2024-05-23 20:39:23.236159 gitsint-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     5616 1970-01-01 00:00:00.000000 gitsint-0.1.2/PKG-INFO
```

### Comparing `gitsint-0.1.1/LICENSE` & `gitsint-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gitsint-0.1.1/LICENSE.md` & `gitsint-0.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `gitsint-0.1.1/README.md` & `gitsint-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `gitsint-0.1.1/gitsint/README.md` & `gitsint-0.1.2/gitsint/README.md`

 * *Files identical despite different names*

### Comparing `gitsint-0.1.1/gitsint/__init__.py` & `gitsint-0.1.2/gitsint/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 import os
 
 DEBUG        = True
 OUTPUT_PATH  = os.path.abspath(os.path.join(os.path.dirname(__file__), "../output"))
 json_data = []
 username_FORMAT = r'\b[A-Za-z0-9._%+-]+@[A-Za-z0-9.-]+\.[A-Z|a-z]{2,}\b'
 
-__version__ = "0.1.0"
+__version__ = "0.1.2"
 
 
 def import_submodules(package, recursive=True):
     """Get all the Gitint submodules"""
     if isinstance(package, str):
         package = importlib.import_module(package)
     results = {}
@@ -107,15 +107,14 @@
     if 'message' in res:
         if res['message'] == "Not Found":   # Just to be double sure
             res= "Error: User not found"
         elif res['message'].startswith("API rate limit exceeded"):
             res = "Error: API rate limit exceeded, please try again later or give a --token argument"
         elif res['message'].startswith("Bad credentials"):
             res = "Error: Bad credentials, please check your --token argument"
-        
     return res
 
 
 
 
 def print_result(data,args,user,start_time,functions):
     def print_color(text,color,args):
```

### Comparing `gitsint-0.1.1/gitsint/modules/profile/friends.py` & `gitsint-0.1.2/gitsint/modules/profile/friends.py`

 * *Files identical despite different names*

### Comparing `gitsint-0.1.1/gitsint/modules/repos/repository.py` & `gitsint-0.1.2/gitsint/modules/repos/repository.py`

 * *Files identical despite different names*

### Comparing `gitsint-0.1.1/pyproject.toml` & `gitsint-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gitsint"
-version = "0.1.1"
+version = "0.1.2"
 description = "Gitsint allows you to check everything from a github user. It's a powerfull github osint tool"
 authors = ["Zerostats"]
 license = "MIT"
 readme = "README.md"
 
 
 [tool.poetry.dependencies]
```

### Comparing `gitsint-0.1.1/PKG-INFO` & `gitsint-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitsint
-Version: 0.1.1
+Version: 0.1.2
 Summary: Gitsint allows you to check everything from a github user. It's a powerfull github osint tool
 License: MIT
 Author: Zerostats
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

