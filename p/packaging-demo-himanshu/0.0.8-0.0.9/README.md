# Comparing `tmp/packaging_demo_himanshu-0.0.8.tar.gz` & `tmp/packaging_demo_himanshu-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "packaging_demo_himanshu-0.0.8.tar", last modified: Thu May 23 09:16:09 2024, max compression
+gzip compressed data, was "packaging_demo_himanshu-0.0.9.tar", last modified: Thu May 23 09:36:31 2024, max compression
```

## Comparing `packaging_demo_himanshu-0.0.8.tar` & `packaging_demo_himanshu-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:16:09.965293 packaging_demo_himanshu-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-23 09:16:09.965293 packaging_demo_himanshu-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-23 09:16:05.000000 packaging_demo_himanshu-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:16:09.965293 packaging_demo_himanshu-0.0.8/packaging_demo/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-23 09:16:05.000000 packaging_demo_himanshu-0.0.8/packaging_demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-23 09:16:05.000000 packaging_demo_himanshu-0.0.8/packaging_demo/colorized_demo.py
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-23 09:16:05.000000 packaging_demo_himanshu-0.0.8/packaging_demo/my_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:16:09.965293 packaging_demo_himanshu-0.0.8/packaging_demo/my_folder/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 09:16:05.000000 packaging_demo_himanshu-0.0.8/packaging_demo/my_folder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-23 09:16:05.000000 packaging_demo_himanshu-0.0.8/packaging_demo/my_folder/my_nested_file.py
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-23 09:16:05.000000 packaging_demo_himanshu-0.0.8/packaging_demo/my_other_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-23 09:16:05.000000 packaging_demo_himanshu-0.0.8/packaging_demo/states_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:16:09.965293 packaging_demo_himanshu-0.0.8/packaging_demo_himanshu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-23 09:16:09.000000 packaging_demo_himanshu-0.0.8/packaging_demo_himanshu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-23 09:16:09.000000 packaging_demo_himanshu-0.0.8/packaging_demo_himanshu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 09:16:09.000000 packaging_demo_himanshu-0.0.8/packaging_demo_himanshu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-23 09:16:09.000000 packaging_demo_himanshu-0.0.8/packaging_demo_himanshu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-23 09:16:09.000000 packaging_demo_himanshu-0.0.8/packaging_demo_himanshu.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-05-23 09:16:05.000000 packaging_demo_himanshu-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 09:16:09.965293 packaging_demo_himanshu-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-23 09:16:05.000000 packaging_demo_himanshu-0.0.8/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:36:31.472225 packaging_demo_himanshu-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-23 09:36:31.472225 packaging_demo_himanshu-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-23 09:36:26.000000 packaging_demo_himanshu-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:36:31.468225 packaging_demo_himanshu-0.0.9/packaging_demo/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-23 09:36:26.000000 packaging_demo_himanshu-0.0.9/packaging_demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-23 09:36:26.000000 packaging_demo_himanshu-0.0.9/packaging_demo/colorized_demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-23 09:36:26.000000 packaging_demo_himanshu-0.0.9/packaging_demo/my_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:36:31.468225 packaging_demo_himanshu-0.0.9/packaging_demo/my_folder/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 09:36:26.000000 packaging_demo_himanshu-0.0.9/packaging_demo/my_folder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-23 09:36:26.000000 packaging_demo_himanshu-0.0.9/packaging_demo/my_folder/my_nested_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-23 09:36:26.000000 packaging_demo_himanshu-0.0.9/packaging_demo/my_other_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-23 09:36:26.000000 packaging_demo_himanshu-0.0.9/packaging_demo/states_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:36:31.472225 packaging_demo_himanshu-0.0.9/packaging_demo_himanshu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-23 09:36:31.000000 packaging_demo_himanshu-0.0.9/packaging_demo_himanshu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-23 09:36:31.000000 packaging_demo_himanshu-0.0.9/packaging_demo_himanshu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 09:36:31.000000 packaging_demo_himanshu-0.0.9/packaging_demo_himanshu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-23 09:36:31.000000 packaging_demo_himanshu-0.0.9/packaging_demo_himanshu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-23 09:36:31.000000 packaging_demo_himanshu-0.0.9/packaging_demo_himanshu.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-05-23 09:36:26.000000 packaging_demo_himanshu-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 09:36:31.472225 packaging_demo_himanshu-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-23 09:36:26.000000 packaging_demo_himanshu-0.0.9/version.txt
```

### Comparing `packaging_demo_himanshu-0.0.8/PKG-INFO` & `packaging_demo_himanshu-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: packaging-demo-himanshu
-Version: 0.0.8
+Version: 0.0.9
 Summary: My package description
 Author-email: Himanshu Kandpal <himanshukandpal0799@gmail.com>
 License: MIT
 Keywords: one,two
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `packaging_demo_himanshu-0.0.8/packaging_demo/states_info.py` & `packaging_demo_himanshu-0.0.9/packaging_demo/states_info.py`

 * *Files identical despite different names*

### Comparing `packaging_demo_himanshu-0.0.8/packaging_demo_himanshu.egg-info/PKG-INFO` & `packaging_demo_himanshu-0.0.9/packaging_demo_himanshu.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: packaging-demo-himanshu
-Version: 0.0.8
+Version: 0.0.9
 Summary: My package description
 Author-email: Himanshu Kandpal <himanshukandpal0799@gmail.com>
 License: MIT
 Keywords: one,two
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `packaging_demo_himanshu-0.0.8/pyproject.toml` & `packaging_demo_himanshu-0.0.9/pyproject.toml`

 * *Files identical despite different names*

