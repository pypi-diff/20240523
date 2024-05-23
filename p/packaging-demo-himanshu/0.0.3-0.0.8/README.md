# Comparing `tmp/packaging_demo_himanshu-0.0.3.tar.gz` & `tmp/packaging_demo_himanshu-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "packaging_demo_himanshu-0.0.3.tar", last modified: Wed May 22 17:13:13 2024, max compression
+gzip compressed data, was "packaging_demo_himanshu-0.0.8.tar", last modified: Thu May 23 09:16:09 2024, max compression
```

## Comparing `packaging_demo_himanshu-0.0.3.tar` & `packaging_demo_himanshu-0.0.8.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 himansys  (1000) himansys  (1000)        0 2024-05-22 17:13:13.201678 packaging_demo_himanshu-0.0.3/
--rw-r--r--   0 himansys  (1000) himansys  (1000)      878 2024-05-22 17:13:13.191678 packaging_demo_himanshu-0.0.3/PKG-INFO
--rw-r--r--   0 himansys  (1000) himansys  (1000)       85 2024-05-21 12:22:27.000000 packaging_demo_himanshu-0.0.3/README.md
-drwxr-xr-x   0 himansys  (1000) himansys  (1000)        0 2024-05-22 17:13:13.191678 packaging_demo_himanshu-0.0.3/packaging_demo/
--rw-r--r--   0 himansys  (1000) himansys  (1000)       17 2024-05-21 17:12:44.000000 packaging_demo_himanshu-0.0.3/packaging_demo/__init__.py
--rw-r--r--   0 himansys  (1000) himansys  (1000)      110 2024-05-22 05:58:45.000000 packaging_demo_himanshu-0.0.3/packaging_demo/colorized_demo.py
--rw-r--r--   0 himansys  (1000) himansys  (1000)      231 2024-05-21 16:10:26.000000 packaging_demo_himanshu-0.0.3/packaging_demo/my_file.py
-drwxr-xr-x   0 himansys  (1000) himansys  (1000)        0 2024-05-22 17:13:13.191678 packaging_demo_himanshu-0.0.3/packaging_demo/my_folder/
--rw-r--r--   0 himansys  (1000) himansys  (1000)        0 2024-05-21 12:24:11.000000 packaging_demo_himanshu-0.0.3/packaging_demo/my_folder/__init__.py
--rw-r--r--   0 himansys  (1000) himansys  (1000)      216 2024-05-21 17:00:45.000000 packaging_demo_himanshu-0.0.3/packaging_demo/my_folder/my_nested_file.py
--rw-r--r--   0 himansys  (1000) himansys  (1000)       56 2024-05-21 15:56:48.000000 packaging_demo_himanshu-0.0.3/packaging_demo/my_other_file.py
--rw-r--r--   0 himansys  (1000) himansys  (1000)      837 2024-05-22 03:55:04.000000 packaging_demo_himanshu-0.0.3/packaging_demo/states_info.py
-drwxr-xr-x   0 himansys  (1000) himansys  (1000)        0 2024-05-22 17:13:13.191678 packaging_demo_himanshu-0.0.3/packaging_demo_himanshu.egg-info/
--rw-r--r--   0 himansys  (1000) himansys  (1000)      878 2024-05-22 17:13:13.000000 packaging_demo_himanshu-0.0.3/packaging_demo_himanshu.egg-info/PKG-INFO
--rw-r--r--   0 himansys  (1000) himansys  (1000)      486 2024-05-22 17:13:13.000000 packaging_demo_himanshu-0.0.3/packaging_demo_himanshu.egg-info/SOURCES.txt
--rw-r--r--   0 himansys  (1000) himansys  (1000)        1 2024-05-22 17:13:13.000000 packaging_demo_himanshu-0.0.3/packaging_demo_himanshu.egg-info/dependency_links.txt
--rw-r--r--   0 himansys  (1000) himansys  (1000)      163 2024-05-22 17:13:13.000000 packaging_demo_himanshu-0.0.3/packaging_demo_himanshu.egg-info/requires.txt
--rw-r--r--   0 himansys  (1000) himansys  (1000)       15 2024-05-22 17:13:13.000000 packaging_demo_himanshu-0.0.3/packaging_demo_himanshu.egg-info/top_level.txt
--rw-r--r--   0 himansys  (1000) himansys  (1000)     1925 2024-05-22 17:13:05.000000 packaging_demo_himanshu-0.0.3/pyproject.toml
--rw-r--r--   0 himansys  (1000) himansys  (1000)       38 2024-05-22 17:13:13.201678 packaging_demo_himanshu-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:16:09.965293 packaging_demo_himanshu-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-23 09:16:09.965293 packaging_demo_himanshu-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-23 09:16:05.000000 packaging_demo_himanshu-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:16:09.965293 packaging_demo_himanshu-0.0.8/packaging_demo/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-23 09:16:05.000000 packaging_demo_himanshu-0.0.8/packaging_demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-23 09:16:05.000000 packaging_demo_himanshu-0.0.8/packaging_demo/colorized_demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-23 09:16:05.000000 packaging_demo_himanshu-0.0.8/packaging_demo/my_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:16:09.965293 packaging_demo_himanshu-0.0.8/packaging_demo/my_folder/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 09:16:05.000000 packaging_demo_himanshu-0.0.8/packaging_demo/my_folder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-23 09:16:05.000000 packaging_demo_himanshu-0.0.8/packaging_demo/my_folder/my_nested_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-23 09:16:05.000000 packaging_demo_himanshu-0.0.8/packaging_demo/my_other_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-23 09:16:05.000000 packaging_demo_himanshu-0.0.8/packaging_demo/states_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:16:09.965293 packaging_demo_himanshu-0.0.8/packaging_demo_himanshu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-05-23 09:16:09.000000 packaging_demo_himanshu-0.0.8/packaging_demo_himanshu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-23 09:16:09.000000 packaging_demo_himanshu-0.0.8/packaging_demo_himanshu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 09:16:09.000000 packaging_demo_himanshu-0.0.8/packaging_demo_himanshu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-23 09:16:09.000000 packaging_demo_himanshu-0.0.8/packaging_demo_himanshu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-23 09:16:09.000000 packaging_demo_himanshu-0.0.8/packaging_demo_himanshu.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-05-23 09:16:05.000000 packaging_demo_himanshu-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 09:16:09.965293 packaging_demo_himanshu-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-23 09:16:05.000000 packaging_demo_himanshu-0.0.8/version.txt
```

### Comparing `packaging_demo_himanshu-0.0.3/PKG-INFO` & `packaging_demo_himanshu-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: packaging-demo-himanshu
-Version: 0.0.3
+Version: 0.0.8
 Summary: My package description
 Author-email: Himanshu Kandpal <himanshukandpal0799@gmail.com>
 License: MIT
 Keywords: one,two
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `packaging_demo_himanshu-0.0.3/packaging_demo/states_info.py` & `packaging_demo_himanshu-0.0.8/packaging_demo/states_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,11 +14,11 @@
     cities: List[dict] = json.loads(cities_json_contents)
     matching_cities: List[dict] = [city for city in cities if city["city"]==city]
     if len(matching_cities) == 0:
         return False
     else:
         matched_city = matching_cities[0]
         return matched_city["state"] == state
-    
+
 if __name__=="__main__":
     is_capital = is_city_capital_of_state(city="Montgomery", state="Alabama")
-    print(f"is capital: {is_capital}")
+    print(f"is capital: {is_capital}")
```

### Comparing `packaging_demo_himanshu-0.0.3/packaging_demo_himanshu.egg-info/PKG-INFO` & `packaging_demo_himanshu-0.0.8/packaging_demo_himanshu.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: packaging-demo-himanshu
-Version: 0.0.3
+Version: 0.0.8
 Summary: My package description
 Author-email: Himanshu Kandpal <himanshukandpal0799@gmail.com>
 License: MIT
 Keywords: one,two
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `packaging_demo_himanshu-0.0.3/pyproject.toml` & `packaging_demo_himanshu-0.0.8/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 
 [tool.setuptools.package-data]
 package_demo = ["*.json"]
 ##### ---- The 'project' table was defined in PEP 621 ----
 
 [project]
 name = "packaging-demo-himanshu"
-version = "0.0.3"
 authors = [
     {name = "Himanshu Kandpal", email = "himanshukandpal0799@gmail.com"},
 ]
 description = "My package description"
 readme = "README.md"
 requires-python = ">=3.7"
 keywords = ["one", "two"]
@@ -23,23 +22,25 @@
 classifiers = [
     "Programming Language :: Python :: 3",
 ]
 dependencies = [
     "numpy",
     "fastapi",
 ]
-
+dynamic = ["version"]
 ##### ---- End of the 'project' table ----
 
 [project.optional-dependencies]
 test = ["pytest", "pytest-cov"]
 release = ["build", "twine", "pre-commit"]
 static-code-qa = ["pre-commit"]
 dev = ["packaging-demo-himanshu[test, release, static-code-qa]"]
 
+[tool.setuptools.dynamic]
+version = {file = "version.txt"}
 
 [tool.black]
 line-length = 119
 exclude = "venv"
 
 [tool.flake8]
 docstring-convention = "all"
@@ -79,8 +80,8 @@
 unfixable = ["B"]
 
 line-length = 99
 
 # Ignore `E402` (import violations) in all `__init__.py` files, and in `path/to/file.py`.
 [tool.ruff.per-file-ignores]
 "__init__.py" = ["E402"]
-"path/to/file.py" = ["E402"]
+"path/to/file.py" = ["E402"]
```

