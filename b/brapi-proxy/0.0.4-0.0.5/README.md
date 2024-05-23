# Comparing `tmp/brapi_proxy-0.0.4.tar.gz` & `tmp/brapi_proxy-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brapi_proxy-0.0.4.tar", last modified: Thu May 23 09:11:41 2024, max compression
+gzip compressed data, was "brapi_proxy-0.0.5.tar", last modified: Thu May 23 11:39:16 2024, max compression
```

## Comparing `brapi_proxy-0.0.4.tar` & `brapi_proxy-0.0.5.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2024-05-23 09:11:41.078004 brapi_proxy-0.0.4/
--rw-r--r--   0 matthijs   (501) staff       (20)     1079 2024-05-23 06:09:10.000000 brapi_proxy-0.0.4/LICENSE
--rw-r--r--   0 matthijs   (501) staff       (20)     4935 2024-05-23 09:11:41.077495 brapi_proxy-0.0.4/PKG-INFO
--rw-r--r--   0 matthijs   (501) staff       (20)     2974 2024-05-23 09:08:53.000000 brapi_proxy-0.0.4/README.md
--rw-r--r--   0 matthijs   (501) staff       (20)     1021 2024-05-23 08:23:08.000000 brapi_proxy-0.0.4/pyproject.toml
--rw-r--r--   0 matthijs   (501) staff       (20)       65 2024-05-22 18:03:35.000000 brapi_proxy-0.0.4/requirements.txt
--rw-r--r--   0 matthijs   (501) staff       (20)       38 2024-05-23 09:11:41.078099 brapi_proxy-0.0.4/setup.cfg
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2024-05-23 09:11:41.050260 brapi_proxy-0.0.4/src/
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2024-05-23 09:11:41.058519 brapi_proxy-0.0.4/src/brapi_proxy/
--rw-r--r--   0 matthijs   (501) staff       (20)       85 2024-05-21 08:26:30.000000 brapi_proxy-0.0.4/src/brapi_proxy/__init__.py
--rw-r--r--   0 matthijs   (501) staff       (20)       22 2024-05-23 09:10:46.000000 brapi_proxy-0.0.4/src/brapi_proxy/_version.py
--rw-r--r--   0 matthijs   (501) staff       (20)     8757 2024-05-23 09:08:40.000000 brapi_proxy-0.0.4/src/brapi_proxy/brapi.py
--rw-r--r--   0 matthijs   (501) staff       (20)      769 2024-05-23 09:08:23.000000 brapi_proxy-0.0.4/src/brapi_proxy/config_demo.ini
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2024-05-23 09:11:41.066063 brapi_proxy-0.0.4/src/brapi_proxy/core/
--rw-r--r--   0 matthijs   (501) staff       (20)      607 2024-05-21 08:29:31.000000 brapi_proxy-0.0.4/src/brapi_proxy/core/__init__.py
--rw-r--r--   0 matthijs   (501) staff       (20)     1921 2024-05-22 17:35:55.000000 brapi_proxy-0.0.4/src/brapi_proxy/core/core_commoncropnames.py
--rw-r--r--   0 matthijs   (501) staff       (20)     2432 2024-05-22 17:35:22.000000 brapi_proxy-0.0.4/src/brapi_proxy/core/core_serverinfo.py
--rw-r--r--   0 matthijs   (501) staff       (20)     7005 2024-05-22 17:37:10.000000 brapi_proxy-0.0.4/src/brapi_proxy/core/core_studies.py
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2024-05-23 09:11:41.076088 brapi_proxy-0.0.4/src/brapi_proxy/genotyping/
--rw-r--r--   0 matthijs   (501) staff       (20)     1745 2024-05-22 17:56:28.000000 brapi_proxy-0.0.4/src/brapi_proxy/genotyping/__init__.py
--rw-r--r--   0 matthijs   (501) staff       (20)    25351 2024-05-23 07:19:21.000000 brapi_proxy-0.0.4/src/brapi_proxy/genotyping/genotyping_allelematrix.py
--rw-r--r--   0 matthijs   (501) staff       (20)     4030 2024-05-22 17:38:37.000000 brapi_proxy-0.0.4/src/brapi_proxy/genotyping/genotyping_callsets.py
--rw-r--r--   0 matthijs   (501) staff       (20)     6179 2024-05-22 17:39:08.000000 brapi_proxy-0.0.4/src/brapi_proxy/genotyping/genotyping_plates.py
--rw-r--r--   0 matthijs   (501) staff       (20)     5926 2024-05-22 17:39:34.000000 brapi_proxy-0.0.4/src/brapi_proxy/genotyping/genotyping_references.py
--rw-r--r--   0 matthijs   (501) staff       (20)     5573 2024-05-22 17:40:06.000000 brapi_proxy-0.0.4/src/brapi_proxy/genotyping/genotyping_referencesets.py
--rw-r--r--   0 matthijs   (501) staff       (20)     6186 2024-05-22 17:40:30.000000 brapi_proxy-0.0.4/src/brapi_proxy/genotyping/genotyping_samples.py
--rw-r--r--   0 matthijs   (501) staff       (20)     3936 2024-05-22 17:41:59.000000 brapi_proxy-0.0.4/src/brapi_proxy/genotyping/genotyping_variants.py
--rw-r--r--   0 matthijs   (501) staff       (20)     5410 2024-05-22 17:42:26.000000 brapi_proxy-0.0.4/src/brapi_proxy/genotyping/genotyping_variantsets.py
--rw-r--r--   0 matthijs   (501) staff       (20)    13760 2024-04-23 07:04:17.000000 brapi_proxy-0.0.4/src/brapi_proxy/handler.py
--rw-r--r--   0 matthijs   (501) staff       (20)     1394 2024-05-23 07:16:51.000000 brapi_proxy-0.0.4/src/brapi_proxy/service.py
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2024-05-23 09:11:41.076878 brapi_proxy-0.0.4/src/brapi_proxy.egg-info/
--rw-r--r--   0 matthijs   (501) staff       (20)     4935 2024-05-23 09:11:41.000000 brapi_proxy-0.0.4/src/brapi_proxy.egg-info/PKG-INFO
--rw-r--r--   0 matthijs   (501) staff       (20)     1057 2024-05-23 09:11:41.000000 brapi_proxy-0.0.4/src/brapi_proxy.egg-info/SOURCES.txt
--rw-r--r--   0 matthijs   (501) staff       (20)        1 2024-05-23 09:11:41.000000 brapi_proxy-0.0.4/src/brapi_proxy.egg-info/dependency_links.txt
--rw-r--r--   0 matthijs   (501) staff       (20)       60 2024-05-23 09:11:41.000000 brapi_proxy-0.0.4/src/brapi_proxy.egg-info/entry_points.txt
--rw-r--r--   0 matthijs   (501) staff       (20)       65 2024-05-23 09:11:41.000000 brapi_proxy-0.0.4/src/brapi_proxy.egg-info/requires.txt
--rw-r--r--   0 matthijs   (501) staff       (20)       12 2024-05-23 09:11:41.000000 brapi_proxy-0.0.4/src/brapi_proxy.egg-info/top_level.txt
+drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2024-05-23 11:39:16.436184 brapi_proxy-0.0.5/
+-rw-r--r--   0 matthijs   (501) staff       (20)     1079 2024-05-23 06:09:10.000000 brapi_proxy-0.0.5/LICENSE
+-rw-r--r--   0 matthijs   (501) staff       (20)     4980 2024-05-23 11:39:16.435836 brapi_proxy-0.0.5/PKG-INFO
+-rw-r--r--   0 matthijs   (501) staff       (20)     3002 2024-05-23 11:37:23.000000 brapi_proxy-0.0.5/README.md
+-rw-r--r--   0 matthijs   (501) staff       (20)     1038 2024-05-23 09:26:28.000000 brapi_proxy-0.0.5/pyproject.toml
+-rw-r--r--   0 matthijs   (501) staff       (20)       65 2024-05-22 18:03:35.000000 brapi_proxy-0.0.5/requirements.txt
+-rw-r--r--   0 matthijs   (501) staff       (20)       38 2024-05-23 11:39:16.436251 brapi_proxy-0.0.5/setup.cfg
+drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2024-05-23 11:39:16.426243 brapi_proxy-0.0.5/src/
+drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2024-05-23 11:39:16.429303 brapi_proxy-0.0.5/src/brapi_proxy/
+-rw-r--r--   0 matthijs   (501) staff       (20)       85 2024-05-21 08:26:30.000000 brapi_proxy-0.0.5/src/brapi_proxy/__init__.py
+-rw-r--r--   0 matthijs   (501) staff       (20)       22 2024-05-23 11:37:44.000000 brapi_proxy-0.0.5/src/brapi_proxy/_version.py
+-rw-r--r--   0 matthijs   (501) staff       (20)     8845 2024-05-23 11:35:30.000000 brapi_proxy-0.0.5/src/brapi_proxy/brapi.py
+-rw-r--r--   0 matthijs   (501) staff       (20)      780 2024-05-23 11:36:33.000000 brapi_proxy-0.0.5/src/brapi_proxy/config_demo.ini
+drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2024-05-23 11:39:16.432177 brapi_proxy-0.0.5/src/brapi_proxy/core/
+-rw-r--r--   0 matthijs   (501) staff       (20)      607 2024-05-21 08:29:31.000000 brapi_proxy-0.0.5/src/brapi_proxy/core/__init__.py
+-rw-r--r--   0 matthijs   (501) staff       (20)     1921 2024-05-22 17:35:55.000000 brapi_proxy-0.0.5/src/brapi_proxy/core/core_commoncropnames.py
+-rw-r--r--   0 matthijs   (501) staff       (20)     2432 2024-05-22 17:35:22.000000 brapi_proxy-0.0.5/src/brapi_proxy/core/core_serverinfo.py
+-rw-r--r--   0 matthijs   (501) staff       (20)     7005 2024-05-22 17:37:10.000000 brapi_proxy-0.0.5/src/brapi_proxy/core/core_studies.py
+drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2024-05-23 11:39:16.435027 brapi_proxy-0.0.5/src/brapi_proxy/genotyping/
+-rw-r--r--   0 matthijs   (501) staff       (20)     1745 2024-05-22 17:56:28.000000 brapi_proxy-0.0.5/src/brapi_proxy/genotyping/__init__.py
+-rw-r--r--   0 matthijs   (501) staff       (20)    25351 2024-05-23 07:19:21.000000 brapi_proxy-0.0.5/src/brapi_proxy/genotyping/genotyping_allelematrix.py
+-rw-r--r--   0 matthijs   (501) staff       (20)     4030 2024-05-22 17:38:37.000000 brapi_proxy-0.0.5/src/brapi_proxy/genotyping/genotyping_callsets.py
+-rw-r--r--   0 matthijs   (501) staff       (20)     6179 2024-05-22 17:39:08.000000 brapi_proxy-0.0.5/src/brapi_proxy/genotyping/genotyping_plates.py
+-rw-r--r--   0 matthijs   (501) staff       (20)     5926 2024-05-22 17:39:34.000000 brapi_proxy-0.0.5/src/brapi_proxy/genotyping/genotyping_references.py
+-rw-r--r--   0 matthijs   (501) staff       (20)     5573 2024-05-22 17:40:06.000000 brapi_proxy-0.0.5/src/brapi_proxy/genotyping/genotyping_referencesets.py
+-rw-r--r--   0 matthijs   (501) staff       (20)     6186 2024-05-22 17:40:30.000000 brapi_proxy-0.0.5/src/brapi_proxy/genotyping/genotyping_samples.py
+-rw-r--r--   0 matthijs   (501) staff       (20)     3936 2024-05-22 17:41:59.000000 brapi_proxy-0.0.5/src/brapi_proxy/genotyping/genotyping_variants.py
+-rw-r--r--   0 matthijs   (501) staff       (20)     5410 2024-05-22 17:42:26.000000 brapi_proxy-0.0.5/src/brapi_proxy/genotyping/genotyping_variantsets.py
+-rw-r--r--   0 matthijs   (501) staff       (20)    13760 2024-04-23 07:04:17.000000 brapi_proxy-0.0.5/src/brapi_proxy/handler.py
+-rw-r--r--   0 matthijs   (501) staff       (20)     1394 2024-05-23 07:16:51.000000 brapi_proxy-0.0.5/src/brapi_proxy/service.py
+drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2024-05-23 11:39:16.435450 brapi_proxy-0.0.5/src/brapi_proxy.egg-info/
+-rw-r--r--   0 matthijs   (501) staff       (20)     4980 2024-05-23 11:39:16.000000 brapi_proxy-0.0.5/src/brapi_proxy.egg-info/PKG-INFO
+-rw-r--r--   0 matthijs   (501) staff       (20)     1057 2024-05-23 11:39:16.000000 brapi_proxy-0.0.5/src/brapi_proxy.egg-info/SOURCES.txt
+-rw-r--r--   0 matthijs   (501) staff       (20)        1 2024-05-23 11:39:16.000000 brapi_proxy-0.0.5/src/brapi_proxy.egg-info/dependency_links.txt
+-rw-r--r--   0 matthijs   (501) staff       (20)       60 2024-05-23 11:39:16.000000 brapi_proxy-0.0.5/src/brapi_proxy.egg-info/entry_points.txt
+-rw-r--r--   0 matthijs   (501) staff       (20)       65 2024-05-23 11:39:16.000000 brapi_proxy-0.0.5/src/brapi_proxy.egg-info/requires.txt
+-rw-r--r--   0 matthijs   (501) staff       (20)       12 2024-05-23 11:39:16.000000 brapi_proxy-0.0.5/src/brapi_proxy.egg-info/top_level.txt
```

### Comparing `brapi_proxy-0.0.4/LICENSE` & `brapi_proxy-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `brapi_proxy-0.0.4/PKG-INFO` & `brapi_proxy-0.0.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: brapi-proxy
-Version: 0.0.4
-Summary: A BRAPI server instance that functions as a proxy for endpoints from existing BRAPI services
+Version: 0.0.5
+Summary: A BRAPI server instance that functions as a proxy to merge and combine endpoints from existing BRAPI services
 Author-email: Matthijs Brouwer <matthijs.brouwer@wur.nl>
 License: MIT License
         
         Copyright (c) 2024 EU H2020 AGENT project
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -37,15 +37,15 @@
 Requires-Dist: flask_restx>=1.3.0
 Requires-Dist: Requests>=2.32.2
 Requires-Dist: waitress>=3.0.0
 
 # BrAPI proxy solution
 
 
-A [BrAPI](https://brapi.org/) server instance that functions as a proxy for endpoints from existing BrAPI services.
+A [BrAPI](https://brapi.org/) server instance that functions as a proxy to merge and combine endpoints from existing BrAPI services.
 
 ## Installation
 
 - **Step 1: Install BrAPI Proxy**
   - To install the BrAPI Proxy, run the following command:
     ```sh
     pip install brapi_proxy
@@ -118,14 +118,15 @@
 
 Include at least the `brapi` section:
 
 ```config
 [brapi]
 port=8080
 host=0.0.0.0
+location=/
 threads=4
 debug=False
 version=2.1
 ```
 
 **Optional: Authorization**
```

### Comparing `brapi_proxy-0.0.4/README.md` & `brapi_proxy-0.0.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # BrAPI proxy solution
 
 
-A [BrAPI](https://brapi.org/) server instance that functions as a proxy for endpoints from existing BrAPI services.
+A [BrAPI](https://brapi.org/) server instance that functions as a proxy to merge and combine endpoints from existing BrAPI services.
 
 ## Installation
 
 - **Step 1: Install BrAPI Proxy**
   - To install the BrAPI Proxy, run the following command:
     ```sh
     pip install brapi_proxy
@@ -78,14 +78,15 @@
 
 Include at least the `brapi` section:
 
 ```config
 [brapi]
 port=8080
 host=0.0.0.0
+location=/
 threads=4
 debug=False
 version=2.1
 ```
 
 **Optional: Authorization**
```

### Comparing `brapi_proxy-0.0.4/pyproject.toml` & `brapi_proxy-0.0.5/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [project]
 name = "brapi-proxy"
 authors = [
   { name="Matthijs Brouwer", email="matthijs.brouwer@wur.nl" },
 ]
-description = "A BRAPI server instance that functions as a proxy for endpoints from existing BRAPI services"
+description = "A BRAPI server instance that functions as a proxy to merge and combine endpoints from existing BRAPI services"
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">=3.10"
 dynamic = ["dependencies","version"]
 classifiers = [
     "Topic :: Internet :: Proxy Servers",
     "Topic :: Scientific/Engineering :: Bio-Informatics",
```

### Comparing `brapi_proxy-0.0.4/src/brapi_proxy/brapi.py` & `brapi_proxy-0.0.5/src/brapi_proxy/brapi.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,15 +58,16 @@
         """
         #--- initialize Flask application ---
         app = Flask(__name__, static_url_path="/static",
                     static_folder=os.path.join(self.location,"static"),
                     template_folder=os.path.join(self.location,"templates"))
         app.config["location"] = self.location
         #blueprint
-        blueprint = Blueprint("brapi", __name__, url_prefix="/")
+        server_location = self.config.get("brapi","location", fallback="/")
+        blueprint = Blueprint("brapi", __name__, url_prefix=server_location)
         authorizations = {
             "apikey": {
                 "type": "apiKey",
                 "in": "header",
                 "name": "Authorization"
             }
         }
```

### Comparing `brapi_proxy-0.0.4/src/brapi_proxy/config_demo.ini` & `brapi_proxy-0.0.5/src/brapi_proxy/config_demo.ini`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 [brapi]
 port=8080
 host=0.0.0.0
+location=/
 threads=4
 debug=False
 version=2.1
 
 [serverinfo]
 serverDescription=Demo-version proxy to combine multiple BrAPI services
 serverName=BrAPI-Proxy
```

### Comparing `brapi_proxy-0.0.4/src/brapi_proxy/core/__init__.py` & `brapi_proxy-0.0.5/src/brapi_proxy/core/__init__.py`

 * *Files identical despite different names*

### Comparing `brapi_proxy-0.0.4/src/brapi_proxy/core/core_commoncropnames.py` & `brapi_proxy-0.0.5/src/brapi_proxy/core/core_commoncropnames.py`

 * *Files identical despite different names*

### Comparing `brapi_proxy-0.0.4/src/brapi_proxy/core/core_serverinfo.py` & `brapi_proxy-0.0.5/src/brapi_proxy/core/core_serverinfo.py`

 * *Files identical despite different names*

### Comparing `brapi_proxy-0.0.4/src/brapi_proxy/core/core_studies.py` & `brapi_proxy-0.0.5/src/brapi_proxy/core/core_studies.py`

 * *Files identical despite different names*

### Comparing `brapi_proxy-0.0.4/src/brapi_proxy/genotyping/__init__.py` & `brapi_proxy-0.0.5/src/brapi_proxy/genotyping/__init__.py`

 * *Files identical despite different names*

### Comparing `brapi_proxy-0.0.4/src/brapi_proxy/genotyping/genotyping_allelematrix.py` & `brapi_proxy-0.0.5/src/brapi_proxy/genotyping/genotyping_allelematrix.py`

 * *Files identical despite different names*

### Comparing `brapi_proxy-0.0.4/src/brapi_proxy/genotyping/genotyping_callsets.py` & `brapi_proxy-0.0.5/src/brapi_proxy/genotyping/genotyping_callsets.py`

 * *Files identical despite different names*

### Comparing `brapi_proxy-0.0.4/src/brapi_proxy/genotyping/genotyping_plates.py` & `brapi_proxy-0.0.5/src/brapi_proxy/genotyping/genotyping_plates.py`

 * *Files identical despite different names*

### Comparing `brapi_proxy-0.0.4/src/brapi_proxy/genotyping/genotyping_references.py` & `brapi_proxy-0.0.5/src/brapi_proxy/genotyping/genotyping_references.py`

 * *Files identical despite different names*

### Comparing `brapi_proxy-0.0.4/src/brapi_proxy/genotyping/genotyping_referencesets.py` & `brapi_proxy-0.0.5/src/brapi_proxy/genotyping/genotyping_referencesets.py`

 * *Files identical despite different names*

### Comparing `brapi_proxy-0.0.4/src/brapi_proxy/genotyping/genotyping_samples.py` & `brapi_proxy-0.0.5/src/brapi_proxy/genotyping/genotyping_samples.py`

 * *Files identical despite different names*

### Comparing `brapi_proxy-0.0.4/src/brapi_proxy/genotyping/genotyping_variants.py` & `brapi_proxy-0.0.5/src/brapi_proxy/genotyping/genotyping_variants.py`

 * *Files identical despite different names*

### Comparing `brapi_proxy-0.0.4/src/brapi_proxy/genotyping/genotyping_variantsets.py` & `brapi_proxy-0.0.5/src/brapi_proxy/genotyping/genotyping_variantsets.py`

 * *Files identical despite different names*

### Comparing `brapi_proxy-0.0.4/src/brapi_proxy/handler.py` & `brapi_proxy-0.0.5/src/brapi_proxy/handler.py`

 * *Files identical despite different names*

### Comparing `brapi_proxy-0.0.4/src/brapi_proxy/service.py` & `brapi_proxy-0.0.5/src/brapi_proxy/service.py`

 * *Files identical despite different names*

### Comparing `brapi_proxy-0.0.4/src/brapi_proxy.egg-info/PKG-INFO` & `brapi_proxy-0.0.5/src/brapi_proxy.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: brapi-proxy
-Version: 0.0.4
-Summary: A BRAPI server instance that functions as a proxy for endpoints from existing BRAPI services
+Version: 0.0.5
+Summary: A BRAPI server instance that functions as a proxy to merge and combine endpoints from existing BRAPI services
 Author-email: Matthijs Brouwer <matthijs.brouwer@wur.nl>
 License: MIT License
         
         Copyright (c) 2024 EU H2020 AGENT project
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -37,15 +37,15 @@
 Requires-Dist: flask_restx>=1.3.0
 Requires-Dist: Requests>=2.32.2
 Requires-Dist: waitress>=3.0.0
 
 # BrAPI proxy solution
 
 
-A [BrAPI](https://brapi.org/) server instance that functions as a proxy for endpoints from existing BrAPI services.
+A [BrAPI](https://brapi.org/) server instance that functions as a proxy to merge and combine endpoints from existing BrAPI services.
 
 ## Installation
 
 - **Step 1: Install BrAPI Proxy**
   - To install the BrAPI Proxy, run the following command:
     ```sh
     pip install brapi_proxy
@@ -118,14 +118,15 @@
 
 Include at least the `brapi` section:
 
 ```config
 [brapi]
 port=8080
 host=0.0.0.0
+location=/
 threads=4
 debug=False
 version=2.1
 ```
 
 **Optional: Authorization**
```

### Comparing `brapi_proxy-0.0.4/src/brapi_proxy.egg-info/SOURCES.txt` & `brapi_proxy-0.0.5/src/brapi_proxy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

