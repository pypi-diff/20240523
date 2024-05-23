# Comparing `tmp/mosek_license_server-0.9.4.tar.gz` & `tmp/mosek_license_server-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mosek_license_server-0.9.4.tar", max compression
+gzip compressed data, was "mosek_license_server-0.9.5.tar", max compression
```

## Comparing `mosek_license_server-0.9.4.tar` & `mosek_license_server-0.9.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    10761 2024-05-03 18:13:22.742352 mosek_license_server-0.9.4/LICENSE
--rw-r--r--   0        0        0      579 2024-05-03 18:13:22.742352 mosek_license_server-0.9.4/mosek_license/__init__.py
--rw-r--r--   0        0        0     1309 2024-05-03 18:13:22.742352 mosek_license_server-0.9.4/mosek_license/license.py
--rw-r--r--   0        0        0      761 2024-05-03 18:13:42.562429 mosek_license_server-0.9.4/pyproject.toml
--rw-r--r--   0        0        0     3215 2024-05-03 18:13:22.742352 mosek_license_server-0.9.4/readme.md
--rw-r--r--   0        0        0     3915 1970-01-01 00:00:00.000000 mosek_license_server-0.9.4/PKG-INFO
+-rw-r--r--   0        0        0    10761 2024-05-23 02:19:37.315929 mosek_license_server-0.9.5/LICENSE
+-rw-r--r--   0        0        0      579 2024-05-23 02:19:37.315929 mosek_license_server-0.9.5/mosek_license/__init__.py
+-rw-r--r--   0        0        0     1309 2024-05-23 02:19:37.315929 mosek_license_server-0.9.5/mosek_license/license.py
+-rw-r--r--   0        0        0      770 2024-05-23 02:19:58.079855 mosek_license_server-0.9.5/pyproject.toml
+-rw-r--r--   0        0        0     3215 2024-05-23 02:19:37.315929 mosek_license_server-0.9.5/readme.md
+-rw-r--r--   0        0        0     3915 1970-01-01 00:00:00.000000 mosek_license_server-0.9.5/PKG-INFO
```

### Comparing `mosek_license_server-0.9.4/LICENSE` & `mosek_license_server-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `mosek_license_server-0.9.4/mosek_license/__init__.py` & `mosek_license_server-0.9.5/mosek_license/__init__.py`

 * *Files identical despite different names*

### Comparing `mosek_license_server-0.9.4/mosek_license/license.py` & `mosek_license_server-0.9.5/mosek_license/license.py`

 * *Files identical despite different names*

### Comparing `mosek_license_server-0.9.4/pyproject.toml` & `mosek_license_server-0.9.5/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "mosek-license-server"
-version = "v0.9.4"
+version = "v0.9.5"
 description = "Expose a mosek license via a nginx server"
 authors = ["Thomas Schmelzer <thomas.schmelzer@gmail.com>"]
 license = "Apache 2.0"
 readme = "readme.md"
 repository = "https://github.com/tschm/mosek-license-server"
 packages = [{include = "mosek_license"}]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.13"
 
 [tool.poetry.group.test.dependencies]
 numpy = "*"
-mosek = "~10.1.28"
+mosek = ">=10.1.28,<10.3.0"
 pytest = "*"
 pytest-cov = "*"
 pre-commit = "*"
 
 [build-system]
 requires = ["poetry>=1.6.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `mosek_license_server-0.9.4/readme.md` & `mosek_license_server-0.9.5/readme.md`

 * *Files identical despite different names*

### Comparing `mosek_license_server-0.9.4/PKG-INFO` & `mosek_license_server-0.9.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mosek-license-server
-Version: 0.9.4
+Version: 0.9.5
 Summary: Expose a mosek license via a nginx server
 Home-page: https://github.com/tschm/mosek-license-server
 License: Apache 2.0
 Author: Thomas Schmelzer
 Author-email: thomas.schmelzer@gmail.com
 Requires-Python: >=3.9,<3.13
 Classifier: License :: Other/Proprietary License
```

