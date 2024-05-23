# Comparing `tmp/roofAI-4.21.1.tar.gz` & `tmp/roofai-4.22.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roofAI-4.21.1.tar", last modified: Tue May 21 02:34:11 2024, max compression
+gzip compressed data, was "roofai-4.22.1.tar", last modified: Thu May 23 04:23:35 2024, max compression
```

## Comparing `roofAI-4.21.1.tar` & `roofai-4.22.1.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-21 02:34:11.366267 roofAI-4.21.1/
--rw-r--r--   0 kamangir   (502) staff       (20)     7048 2023-10-03 04:10:45.000000 roofAI-4.21.1/LICENSE
--rw-r--r--   0 kamangir   (502) staff       (20)       24 2024-05-20 04:50:37.000000 roofAI-4.21.1/MANIFEST.in
--rw-r--r--   0 kamangir   (502) staff       (20)     4248 2024-05-21 02:34:11.365609 roofAI-4.21.1/PKG-INFO
--rw-r--r--   0 kamangir   (502) staff       (20)     3117 2024-05-19 23:19:15.000000 roofAI-4.21.1/README.md
--rw-r--r--   0 kamangir   (502) staff       (20)      318 2024-05-20 22:40:00.000000 roofAI-4.21.1/requirements.txt
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-21 02:34:11.362118 roofAI-4.21.1/roofAI/
--rw-r--r--   0 kamangir   (502) staff       (20)      106 2024-05-21 02:34:06.000000 roofAI-4.21.1/roofAI/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)      751 2024-03-04 07:11:52.000000 roofAI-4.21.1/roofAI/__main__.py
--rw-r--r--   0 kamangir   (502) staff       (20)       87 2024-03-24 00:16:41.000000 roofAI-4.21.1/roofAI/logger.py
--rw-r--r--   0 kamangir   (502) staff       (20)       17 2023-10-03 04:10:45.000000 roofAI-4.21.1/roofAI/urls.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-21 02:34:11.364675 roofAI-4.21.1/roofAI.egg-info/
--rw-r--r--   0 kamangir   (502) staff       (20)     4248 2024-05-21 02:34:11.000000 roofAI-4.21.1/roofAI.egg-info/PKG-INFO
--rw-r--r--   0 kamangir   (502) staff       (20)      274 2024-05-21 02:34:11.000000 roofAI-4.21.1/roofAI.egg-info/SOURCES.txt
--rw-r--r--   0 kamangir   (502) staff       (20)        1 2024-05-21 02:34:11.000000 roofAI-4.21.1/roofAI.egg-info/dependency_links.txt
--rw-r--r--   0 kamangir   (502) staff       (20)      319 2024-05-21 02:34:11.000000 roofAI-4.21.1/roofAI.egg-info/requires.txt
--rw-r--r--   0 kamangir   (502) staff       (20)        7 2024-05-21 02:34:11.000000 roofAI-4.21.1/roofAI.egg-info/top_level.txt
--rw-r--r--   0 kamangir   (502) staff       (20)       38 2024-05-21 02:34:11.366432 roofAI-4.21.1/setup.cfg
--rw-r--r--   0 kamangir   (502) staff       (20)      654 2024-05-20 21:25:01.000000 roofAI-4.21.1/setup.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-23 04:23:35.299263 roofai-4.22.1/
+-rw-r--r--   0 kamangir   (502) staff       (20)     7048 2023-10-03 04:10:45.000000 roofai-4.22.1/LICENSE
+-rw-r--r--   0 kamangir   (502) staff       (20)       24 2024-05-20 04:50:37.000000 roofai-4.22.1/MANIFEST.in
+-rw-r--r--   0 kamangir   (502) staff       (20)     4602 2024-05-23 04:23:35.298655 roofai-4.22.1/PKG-INFO
+-rw-r--r--   0 kamangir   (502) staff       (20)     3117 2024-05-19 23:19:15.000000 roofai-4.22.1/README.md
+-rw-r--r--   0 kamangir   (502) staff       (20)       81 2024-05-23 04:22:10.000000 roofai-4.22.1/pyproject.toml
+-rw-r--r--   0 kamangir   (502) staff       (20)      318 2024-05-20 22:40:00.000000 roofai-4.22.1/requirements.txt
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-23 04:23:35.293563 roofai-4.22.1/roofAI/
+-rw-r--r--   0 kamangir   (502) staff       (20)      106 2024-05-23 04:23:29.000000 roofai-4.22.1/roofAI/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      751 2024-03-04 07:11:52.000000 roofai-4.22.1/roofAI/__main__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)       87 2024-03-24 00:16:41.000000 roofai-4.22.1/roofAI/logger.py
+-rw-r--r--   0 kamangir   (502) staff       (20)       17 2023-10-03 04:10:45.000000 roofai-4.22.1/roofAI/urls.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-23 04:23:35.297556 roofai-4.22.1/roofAI.egg-info/
+-rw-r--r--   0 kamangir   (502) staff       (20)     4602 2024-05-23 04:23:35.000000 roofai-4.22.1/roofAI.egg-info/PKG-INFO
+-rw-r--r--   0 kamangir   (502) staff       (20)      289 2024-05-23 04:23:35.000000 roofai-4.22.1/roofAI.egg-info/SOURCES.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)        1 2024-05-23 04:23:35.000000 roofai-4.22.1/roofAI.egg-info/dependency_links.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)      319 2024-05-23 04:23:35.000000 roofai-4.22.1/roofAI.egg-info/requires.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)        7 2024-05-23 04:23:35.000000 roofai-4.22.1/roofAI.egg-info/top_level.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       38 2024-05-23 04:23:35.299391 roofai-4.22.1/setup.cfg
+-rw-r--r--   0 kamangir   (502) staff       (20)      222 2024-05-23 04:23:01.000000 roofai-4.22.1/setup.py
```

### Comparing `roofAI-4.21.1/LICENSE` & `roofai-4.22.1/LICENSE`

 * *Files identical despite different names*

### Comparing `roofAI-4.21.1/PKG-INFO` & `roofai-4.22.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,19 @@
 Metadata-Version: 2.1
 Name: roofAI
-Version: 4.21.1
+Version: 4.22.1
 Summary: 🏛️ everything AI about roofs.
-Author: arash@kamangir.net
+Home-page: https://github.com/kamangir/roofAI
+Author: Arash Abadpour (Kamangir)
+Author-email: arash@kamangir.net
+License: Public Domain
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Unix Shell
+Classifier: License :: Public Domain
+Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: blueness
 Requires-Dist: abcli
 Requires-Dist: notebooks_and_scripts
 Requires-Dist: albumentations[imgaug]==1.3.0
 Requires-Dist: boto3
@@ -31,15 +38,15 @@
 Requires-Dist: torch
 Requires-Dist: tqdm
 
 # roofAI 🏛️
 
 everything AI about roofs. 🏛️
 
-🔷 [datasets](https://github.com/kamangir/roofAI/raw/main/roofAI/dataset) 🔷 [notebooks](https://github.com/kamangir/roofAI/raw/main/notebooks/) 🔷 [semseg](https://github.com/kamangir/roofAI/raw/main/roofAI/semseg) 🔷 [inference](https://github.com/kamangir/roofAI/raw/main/roofAI/inference) 🔷 [QGIS](https://github.com/kamangir/roofAI/raw/main/roofAI/QGIS/console/) 🔷 [sagemaker](https://github.com/kamangir/roofAI/raw/main/roofAI/semseg/sagemaker/) 🔷
+🔷 [datasets](https://raw.githubusercontent.com/kamangir/roofAI/main/roofAI/dataset) 🔷 [notebooks](https://raw.githubusercontent.com/kamangir/roofAI/main/notebooks/) 🔷 [semseg](https://raw.githubusercontent.com/kamangir/roofAI/main/roofAI/semseg) 🔷 [inference](https://raw.githubusercontent.com/kamangir/roofAI/main/roofAI/inference) 🔷 [QGIS](https://raw.githubusercontent.com/kamangir/roofAI/main/roofAI/QGIS/console/) 🔷 [sagemaker](https://raw.githubusercontent.com/kamangir/roofAI/main/roofAI/semseg/sagemaker/) 🔷
 
 ```bash
  > roof help
 roofAI inference create \
 	[dryrun,model] \
 	[.|<object-name>] \
 	[--verbose 1] \
```

### Comparing `roofAI-4.21.1/README.md` & `roofai-4.22.1/README.md`

 * *Files identical despite different names*

### Comparing `roofAI-4.21.1/roofAI/__main__.py` & `roofai-4.22.1/roofAI/__main__.py`

 * *Files identical despite different names*

### Comparing `roofAI-4.21.1/roofAI.egg-info/PKG-INFO` & `roofai-4.22.1/roofAI.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,19 @@
 Metadata-Version: 2.1
 Name: roofAI
-Version: 4.21.1
+Version: 4.22.1
 Summary: 🏛️ everything AI about roofs.
-Author: arash@kamangir.net
+Home-page: https://github.com/kamangir/roofAI
+Author: Arash Abadpour (Kamangir)
+Author-email: arash@kamangir.net
+License: Public Domain
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Unix Shell
+Classifier: License :: Public Domain
+Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: blueness
 Requires-Dist: abcli
 Requires-Dist: notebooks_and_scripts
 Requires-Dist: albumentations[imgaug]==1.3.0
 Requires-Dist: boto3
@@ -31,15 +38,15 @@
 Requires-Dist: torch
 Requires-Dist: tqdm
 
 # roofAI 🏛️
 
 everything AI about roofs. 🏛️
 
-🔷 [datasets](https://github.com/kamangir/roofAI/raw/main/roofAI/dataset) 🔷 [notebooks](https://github.com/kamangir/roofAI/raw/main/notebooks/) 🔷 [semseg](https://github.com/kamangir/roofAI/raw/main/roofAI/semseg) 🔷 [inference](https://github.com/kamangir/roofAI/raw/main/roofAI/inference) 🔷 [QGIS](https://github.com/kamangir/roofAI/raw/main/roofAI/QGIS/console/) 🔷 [sagemaker](https://github.com/kamangir/roofAI/raw/main/roofAI/semseg/sagemaker/) 🔷
+🔷 [datasets](https://raw.githubusercontent.com/kamangir/roofAI/main/roofAI/dataset) 🔷 [notebooks](https://raw.githubusercontent.com/kamangir/roofAI/main/notebooks/) 🔷 [semseg](https://raw.githubusercontent.com/kamangir/roofAI/main/roofAI/semseg) 🔷 [inference](https://raw.githubusercontent.com/kamangir/roofAI/main/roofAI/inference) 🔷 [QGIS](https://raw.githubusercontent.com/kamangir/roofAI/main/roofAI/QGIS/console/) 🔷 [sagemaker](https://raw.githubusercontent.com/kamangir/roofAI/main/roofAI/semseg/sagemaker/) 🔷
 
 ```bash
  > roof help
 roofAI inference create \
 	[dryrun,model] \
 	[.|<object-name>] \
 	[--verbose 1] \
```

