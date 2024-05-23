# Comparing `tmp/brapi_proxy-0.0.2.tar.gz` & `tmp/brapi_proxy-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brapi_proxy-0.0.2.tar", last modified: Thu May 23 08:16:11 2024, max compression
+gzip compressed data, was "brapi_proxy-0.0.3.tar", last modified: Thu May 23 08:30:27 2024, max compression
```

## Comparing `brapi_proxy-0.0.2.tar` & `brapi_proxy-0.0.3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2024-05-23 08:16:11.573313 brapi_proxy-0.0.2/
--rw-r--r--   0 matthijs   (501) staff       (20)     1079 2024-05-23 06:09:10.000000 brapi_proxy-0.0.2/LICENSE
--rw-r--r--   0 matthijs   (501) staff       (20)     4742 2024-05-23 08:16:11.572887 brapi_proxy-0.0.2/PKG-INFO
--rw-r--r--   0 matthijs   (501) staff       (20)     2783 2024-05-23 07:35:32.000000 brapi_proxy-0.0.2/README.md
--rw-r--r--   0 matthijs   (501) staff       (20)     1019 2024-05-23 08:09:21.000000 brapi_proxy-0.0.2/pyproject.toml
--rw-r--r--   0 matthijs   (501) staff       (20)       65 2024-05-22 18:03:35.000000 brapi_proxy-0.0.2/requirements.txt
--rw-r--r--   0 matthijs   (501) staff       (20)       38 2024-05-23 08:16:11.573417 brapi_proxy-0.0.2/setup.cfg
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2024-05-23 08:16:11.561381 brapi_proxy-0.0.2/src/
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2024-05-23 08:16:11.564965 brapi_proxy-0.0.2/src/brapi_proxy/
--rw-r--r--   0 matthijs   (501) staff       (20)       85 2024-05-21 08:26:30.000000 brapi_proxy-0.0.2/src/brapi_proxy/__init__.py
--rw-r--r--   0 matthijs   (501) staff       (20)       22 2024-05-23 07:48:52.000000 brapi_proxy-0.0.2/src/brapi_proxy/_version.py
--rw-r--r--   0 matthijs   (501) staff       (20)     8752 2024-05-22 17:32:53.000000 brapi_proxy-0.0.2/src/brapi_proxy/brapi.py
--rw-r--r--   0 matthijs   (501) staff       (20)      764 2024-05-23 07:12:22.000000 brapi_proxy-0.0.2/src/brapi_proxy/config_demo.ini
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2024-05-23 08:16:11.568550 brapi_proxy-0.0.2/src/brapi_proxy/core/
--rw-r--r--   0 matthijs   (501) staff       (20)      607 2024-05-21 08:29:31.000000 brapi_proxy-0.0.2/src/brapi_proxy/core/__init__.py
--rw-r--r--   0 matthijs   (501) staff       (20)     1921 2024-05-22 17:35:55.000000 brapi_proxy-0.0.2/src/brapi_proxy/core/core_commoncropnames.py
--rw-r--r--   0 matthijs   (501) staff       (20)     2432 2024-05-22 17:35:22.000000 brapi_proxy-0.0.2/src/brapi_proxy/core/core_serverinfo.py
--rw-r--r--   0 matthijs   (501) staff       (20)     7005 2024-05-22 17:37:10.000000 brapi_proxy-0.0.2/src/brapi_proxy/core/core_studies.py
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2024-05-23 08:16:11.571973 brapi_proxy-0.0.2/src/brapi_proxy/genotyping/
--rw-r--r--   0 matthijs   (501) staff       (20)     1745 2024-05-22 17:56:28.000000 brapi_proxy-0.0.2/src/brapi_proxy/genotyping/__init__.py
--rw-r--r--   0 matthijs   (501) staff       (20)    25351 2024-05-23 07:19:21.000000 brapi_proxy-0.0.2/src/brapi_proxy/genotyping/genotyping_allelematrix.py
--rw-r--r--   0 matthijs   (501) staff       (20)     4030 2024-05-22 17:38:37.000000 brapi_proxy-0.0.2/src/brapi_proxy/genotyping/genotyping_callsets.py
--rw-r--r--   0 matthijs   (501) staff       (20)     6179 2024-05-22 17:39:08.000000 brapi_proxy-0.0.2/src/brapi_proxy/genotyping/genotyping_plates.py
--rw-r--r--   0 matthijs   (501) staff       (20)     5926 2024-05-22 17:39:34.000000 brapi_proxy-0.0.2/src/brapi_proxy/genotyping/genotyping_references.py
--rw-r--r--   0 matthijs   (501) staff       (20)     5573 2024-05-22 17:40:06.000000 brapi_proxy-0.0.2/src/brapi_proxy/genotyping/genotyping_referencesets.py
--rw-r--r--   0 matthijs   (501) staff       (20)     6186 2024-05-22 17:40:30.000000 brapi_proxy-0.0.2/src/brapi_proxy/genotyping/genotyping_samples.py
--rw-r--r--   0 matthijs   (501) staff       (20)     3936 2024-05-22 17:41:59.000000 brapi_proxy-0.0.2/src/brapi_proxy/genotyping/genotyping_variants.py
--rw-r--r--   0 matthijs   (501) staff       (20)     5410 2024-05-22 17:42:26.000000 brapi_proxy-0.0.2/src/brapi_proxy/genotyping/genotyping_variantsets.py
--rw-r--r--   0 matthijs   (501) staff       (20)    13760 2024-04-23 07:04:17.000000 brapi_proxy-0.0.2/src/brapi_proxy/handler.py
--rw-r--r--   0 matthijs   (501) staff       (20)     1394 2024-05-23 07:16:51.000000 brapi_proxy-0.0.2/src/brapi_proxy/service.py
-drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2024-05-23 08:16:11.572374 brapi_proxy-0.0.2/src/brapi_proxy.egg-info/
--rw-r--r--   0 matthijs   (501) staff       (20)     4742 2024-05-23 08:16:11.000000 brapi_proxy-0.0.2/src/brapi_proxy.egg-info/PKG-INFO
--rw-r--r--   0 matthijs   (501) staff       (20)     1057 2024-05-23 08:16:11.000000 brapi_proxy-0.0.2/src/brapi_proxy.egg-info/SOURCES.txt
--rw-r--r--   0 matthijs   (501) staff       (20)        1 2024-05-23 08:16:11.000000 brapi_proxy-0.0.2/src/brapi_proxy.egg-info/dependency_links.txt
--rw-r--r--   0 matthijs   (501) staff       (20)       60 2024-05-23 08:16:11.000000 brapi_proxy-0.0.2/src/brapi_proxy.egg-info/entry_points.txt
--rw-r--r--   0 matthijs   (501) staff       (20)       65 2024-05-23 08:16:11.000000 brapi_proxy-0.0.2/src/brapi_proxy.egg-info/requires.txt
--rw-r--r--   0 matthijs   (501) staff       (20)       12 2024-05-23 08:16:11.000000 brapi_proxy-0.0.2/src/brapi_proxy.egg-info/top_level.txt
+drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2024-05-23 08:30:27.576651 brapi_proxy-0.0.3/
+-rw-r--r--   0 matthijs   (501) staff       (20)     1079 2024-05-23 06:09:10.000000 brapi_proxy-0.0.3/LICENSE
+-rw-r--r--   0 matthijs   (501) staff       (20)     4744 2024-05-23 08:30:27.576236 brapi_proxy-0.0.3/PKG-INFO
+-rw-r--r--   0 matthijs   (501) staff       (20)     2783 2024-05-23 07:35:32.000000 brapi_proxy-0.0.3/README.md
+-rw-r--r--   0 matthijs   (501) staff       (20)     1021 2024-05-23 08:23:08.000000 brapi_proxy-0.0.3/pyproject.toml
+-rw-r--r--   0 matthijs   (501) staff       (20)       65 2024-05-22 18:03:35.000000 brapi_proxy-0.0.3/requirements.txt
+-rw-r--r--   0 matthijs   (501) staff       (20)       38 2024-05-23 08:30:27.576730 brapi_proxy-0.0.3/setup.cfg
+drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2024-05-23 08:30:27.559044 brapi_proxy-0.0.3/src/
+drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2024-05-23 08:30:27.563704 brapi_proxy-0.0.3/src/brapi_proxy/
+-rw-r--r--   0 matthijs   (501) staff       (20)       85 2024-05-21 08:26:30.000000 brapi_proxy-0.0.3/src/brapi_proxy/__init__.py
+-rw-r--r--   0 matthijs   (501) staff       (20)       22 2024-05-23 08:28:58.000000 brapi_proxy-0.0.3/src/brapi_proxy/_version.py
+-rw-r--r--   0 matthijs   (501) staff       (20)     8752 2024-05-22 17:32:53.000000 brapi_proxy-0.0.3/src/brapi_proxy/brapi.py
+-rw-r--r--   0 matthijs   (501) staff       (20)      764 2024-05-23 07:12:22.000000 brapi_proxy-0.0.3/src/brapi_proxy/config_demo.ini
+drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2024-05-23 08:30:27.568417 brapi_proxy-0.0.3/src/brapi_proxy/core/
+-rw-r--r--   0 matthijs   (501) staff       (20)      607 2024-05-21 08:29:31.000000 brapi_proxy-0.0.3/src/brapi_proxy/core/__init__.py
+-rw-r--r--   0 matthijs   (501) staff       (20)     1921 2024-05-22 17:35:55.000000 brapi_proxy-0.0.3/src/brapi_proxy/core/core_commoncropnames.py
+-rw-r--r--   0 matthijs   (501) staff       (20)     2432 2024-05-22 17:35:22.000000 brapi_proxy-0.0.3/src/brapi_proxy/core/core_serverinfo.py
+-rw-r--r--   0 matthijs   (501) staff       (20)     7005 2024-05-22 17:37:10.000000 brapi_proxy-0.0.3/src/brapi_proxy/core/core_studies.py
+drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2024-05-23 08:30:27.575206 brapi_proxy-0.0.3/src/brapi_proxy/genotyping/
+-rw-r--r--   0 matthijs   (501) staff       (20)     1745 2024-05-22 17:56:28.000000 brapi_proxy-0.0.3/src/brapi_proxy/genotyping/__init__.py
+-rw-r--r--   0 matthijs   (501) staff       (20)    25351 2024-05-23 07:19:21.000000 brapi_proxy-0.0.3/src/brapi_proxy/genotyping/genotyping_allelematrix.py
+-rw-r--r--   0 matthijs   (501) staff       (20)     4030 2024-05-22 17:38:37.000000 brapi_proxy-0.0.3/src/brapi_proxy/genotyping/genotyping_callsets.py
+-rw-r--r--   0 matthijs   (501) staff       (20)     6179 2024-05-22 17:39:08.000000 brapi_proxy-0.0.3/src/brapi_proxy/genotyping/genotyping_plates.py
+-rw-r--r--   0 matthijs   (501) staff       (20)     5926 2024-05-22 17:39:34.000000 brapi_proxy-0.0.3/src/brapi_proxy/genotyping/genotyping_references.py
+-rw-r--r--   0 matthijs   (501) staff       (20)     5573 2024-05-22 17:40:06.000000 brapi_proxy-0.0.3/src/brapi_proxy/genotyping/genotyping_referencesets.py
+-rw-r--r--   0 matthijs   (501) staff       (20)     6186 2024-05-22 17:40:30.000000 brapi_proxy-0.0.3/src/brapi_proxy/genotyping/genotyping_samples.py
+-rw-r--r--   0 matthijs   (501) staff       (20)     3936 2024-05-22 17:41:59.000000 brapi_proxy-0.0.3/src/brapi_proxy/genotyping/genotyping_variants.py
+-rw-r--r--   0 matthijs   (501) staff       (20)     5410 2024-05-22 17:42:26.000000 brapi_proxy-0.0.3/src/brapi_proxy/genotyping/genotyping_variantsets.py
+-rw-r--r--   0 matthijs   (501) staff       (20)    13760 2024-04-23 07:04:17.000000 brapi_proxy-0.0.3/src/brapi_proxy/handler.py
+-rw-r--r--   0 matthijs   (501) staff       (20)     1394 2024-05-23 07:16:51.000000 brapi_proxy-0.0.3/src/brapi_proxy/service.py
+drwxr-xr-x   0 matthijs   (501) staff       (20)        0 2024-05-23 08:30:27.575784 brapi_proxy-0.0.3/src/brapi_proxy.egg-info/
+-rw-r--r--   0 matthijs   (501) staff       (20)     4744 2024-05-23 08:30:27.000000 brapi_proxy-0.0.3/src/brapi_proxy.egg-info/PKG-INFO
+-rw-r--r--   0 matthijs   (501) staff       (20)     1057 2024-05-23 08:30:27.000000 brapi_proxy-0.0.3/src/brapi_proxy.egg-info/SOURCES.txt
+-rw-r--r--   0 matthijs   (501) staff       (20)        1 2024-05-23 08:30:27.000000 brapi_proxy-0.0.3/src/brapi_proxy.egg-info/dependency_links.txt
+-rw-r--r--   0 matthijs   (501) staff       (20)       60 2024-05-23 08:30:27.000000 brapi_proxy-0.0.3/src/brapi_proxy.egg-info/entry_points.txt
+-rw-r--r--   0 matthijs   (501) staff       (20)       65 2024-05-23 08:30:27.000000 brapi_proxy-0.0.3/src/brapi_proxy.egg-info/requires.txt
+-rw-r--r--   0 matthijs   (501) staff       (20)       12 2024-05-23 08:30:27.000000 brapi_proxy-0.0.3/src/brapi_proxy.egg-info/top_level.txt
```

### Comparing `brapi_proxy-0.0.2/LICENSE` & `brapi_proxy-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `brapi_proxy-0.0.2/PKG-INFO` & `brapi_proxy-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brapi-proxy
-Version: 0.0.2
+Version: 0.0.3
 Summary: A BRAPI server instance that functions as a proxy for endpoints from existing BRAPI services
 Author-email: Matthijs Brouwer <matthijs.brouwer@wur.nl>
 License: MIT License
         
         Copyright (c) 2024 EU H2020 AGENT project
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -24,17 +24,17 @@
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/matthijsbrouwer/brapi-proxy
 Classifier: Topic :: Internet :: Proxy Servers
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: Flask>=3.0.3
 Requires-Dist: flask_restx>=1.3.0
 Requires-Dist: Requests>=2.32.2
 Requires-Dist: waitress>=3.0.0
```

### Comparing `brapi_proxy-0.0.2/README.md` & `brapi_proxy-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `brapi_proxy-0.0.2/pyproject.toml` & `brapi_proxy-0.0.3/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 name = "brapi-proxy"
 authors = [
   { name="Matthijs Brouwer", email="matthijs.brouwer@wur.nl" },
 ]
 description = "A BRAPI server instance that functions as a proxy for endpoints from existing BRAPI services"
 readme = "README.md"
 license = {file = "LICENSE"}
-requires-python = ">=3.8"
+requires-python = ">=3.10"
 dynamic = ["dependencies","version"]
 classifiers = [
     "Topic :: Internet :: Proxy Servers",
     "Topic :: Scientific/Engineering :: Bio-Informatics",
-    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.10",
     "Operating System :: OS Independent"
 ]
 
 [project.urls]
 Homepage = "https://github.com/matthijsbrouwer/brapi-proxy"
 
 [project.scripts]
```

### Comparing `brapi_proxy-0.0.2/src/brapi_proxy/brapi.py` & `brapi_proxy-0.0.3/src/brapi_proxy/brapi.py`

 * *Files identical despite different names*

### Comparing `brapi_proxy-0.0.2/src/brapi_proxy/config_demo.ini` & `brapi_proxy-0.0.3/src/brapi_proxy/config_demo.ini`

 * *Files identical despite different names*

### Comparing `brapi_proxy-0.0.2/src/brapi_proxy/core/__init__.py` & `brapi_proxy-0.0.3/src/brapi_proxy/core/__init__.py`

 * *Files identical despite different names*

### Comparing `brapi_proxy-0.0.2/src/brapi_proxy/core/core_commoncropnames.py` & `brapi_proxy-0.0.3/src/brapi_proxy/core/core_commoncropnames.py`

 * *Files identical despite different names*

### Comparing `brapi_proxy-0.0.2/src/brapi_proxy/core/core_serverinfo.py` & `brapi_proxy-0.0.3/src/brapi_proxy/core/core_serverinfo.py`

 * *Files identical despite different names*

### Comparing `brapi_proxy-0.0.2/src/brapi_proxy/core/core_studies.py` & `brapi_proxy-0.0.3/src/brapi_proxy/core/core_studies.py`

 * *Files identical despite different names*

### Comparing `brapi_proxy-0.0.2/src/brapi_proxy/genotyping/__init__.py` & `brapi_proxy-0.0.3/src/brapi_proxy/genotyping/__init__.py`

 * *Files identical despite different names*

### Comparing `brapi_proxy-0.0.2/src/brapi_proxy/genotyping/genotyping_allelematrix.py` & `brapi_proxy-0.0.3/src/brapi_proxy/genotyping/genotyping_allelematrix.py`

 * *Files identical despite different names*

### Comparing `brapi_proxy-0.0.2/src/brapi_proxy/genotyping/genotyping_callsets.py` & `brapi_proxy-0.0.3/src/brapi_proxy/genotyping/genotyping_callsets.py`

 * *Files identical despite different names*

### Comparing `brapi_proxy-0.0.2/src/brapi_proxy/genotyping/genotyping_plates.py` & `brapi_proxy-0.0.3/src/brapi_proxy/genotyping/genotyping_plates.py`

 * *Files identical despite different names*

### Comparing `brapi_proxy-0.0.2/src/brapi_proxy/genotyping/genotyping_references.py` & `brapi_proxy-0.0.3/src/brapi_proxy/genotyping/genotyping_references.py`

 * *Files identical despite different names*

### Comparing `brapi_proxy-0.0.2/src/brapi_proxy/genotyping/genotyping_referencesets.py` & `brapi_proxy-0.0.3/src/brapi_proxy/genotyping/genotyping_referencesets.py`

 * *Files identical despite different names*

### Comparing `brapi_proxy-0.0.2/src/brapi_proxy/genotyping/genotyping_samples.py` & `brapi_proxy-0.0.3/src/brapi_proxy/genotyping/genotyping_samples.py`

 * *Files identical despite different names*

### Comparing `brapi_proxy-0.0.2/src/brapi_proxy/genotyping/genotyping_variants.py` & `brapi_proxy-0.0.3/src/brapi_proxy/genotyping/genotyping_variants.py`

 * *Files identical despite different names*

### Comparing `brapi_proxy-0.0.2/src/brapi_proxy/genotyping/genotyping_variantsets.py` & `brapi_proxy-0.0.3/src/brapi_proxy/genotyping/genotyping_variantsets.py`

 * *Files identical despite different names*

### Comparing `brapi_proxy-0.0.2/src/brapi_proxy/handler.py` & `brapi_proxy-0.0.3/src/brapi_proxy/handler.py`

 * *Files identical despite different names*

### Comparing `brapi_proxy-0.0.2/src/brapi_proxy/service.py` & `brapi_proxy-0.0.3/src/brapi_proxy/service.py`

 * *Files identical despite different names*

### Comparing `brapi_proxy-0.0.2/src/brapi_proxy.egg-info/PKG-INFO` & `brapi_proxy-0.0.3/src/brapi_proxy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brapi-proxy
-Version: 0.0.2
+Version: 0.0.3
 Summary: A BRAPI server instance that functions as a proxy for endpoints from existing BRAPI services
 Author-email: Matthijs Brouwer <matthijs.brouwer@wur.nl>
 License: MIT License
         
         Copyright (c) 2024 EU H2020 AGENT project
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -24,17 +24,17 @@
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/matthijsbrouwer/brapi-proxy
 Classifier: Topic :: Internet :: Proxy Servers
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: Flask>=3.0.3
 Requires-Dist: flask_restx>=1.3.0
 Requires-Dist: Requests>=2.32.2
 Requires-Dist: waitress>=3.0.0
```

### Comparing `brapi_proxy-0.0.2/src/brapi_proxy.egg-info/SOURCES.txt` & `brapi_proxy-0.0.3/src/brapi_proxy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

