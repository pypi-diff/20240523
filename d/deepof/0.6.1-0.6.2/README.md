# Comparing `tmp/deepof-0.6.1.tar.gz` & `tmp/deepof-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepof-0.6.1.tar", max compression
+gzip compressed data, was "deepof-0.6.2.tar", max compression
```

## Comparing `deepof-0.6.1.tar` & `deepof-0.6.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1070 2023-11-06 00:21:53.366438 deepof-0.6.1/LICENSE
--rw-r--r--   0        0        0     9801 2024-04-10 15:21:33.390157 deepof-0.6.1/README.md
--rw-r--r--   0        0        0     6148 2023-11-15 10:38:41.176080 deepof-0.6.1/deepof/.DS_Store
--rw-r--r--   0        0        0       38 2023-11-06 00:21:53.366751 deepof-0.6.1/deepof/__init__.py
--rw-r--r--   0        0        0    29664 2023-11-06 00:21:53.368751 deepof-0.6.1/deepof/annotation_utils.py
--rw-r--r--   0        0        0   103948 2024-04-01 13:48:27.887411 deepof-0.6.1/deepof/data.py
--rw-r--r--   0        0        0    15179 2023-11-06 00:21:53.369068 deepof-0.6.1/deepof/deepof_train_embeddings.py
--rw-r--r--   0        0        0     8268 2023-11-06 00:21:53.369153 deepof-0.6.1/deepof/hypermodels.py
--rw-r--r--   0        0        0    61514 2023-12-03 17:30:37.818174 deepof-0.6.1/deepof/model_utils.py
--rw-r--r--   0        0        0    78570 2023-11-06 00:21:53.369434 deepof-0.6.1/deepof/models.py
--rw-r--r--   0        0        0    49719 2023-12-08 11:46:57.236557 deepof-0.6.1/deepof/post_hoc.py
--rw-r--r--   0        0        0     6148 2023-11-15 10:38:41.178048 deepof-0.6.1/deepof/trained_models/.DS_Store
--rw-r--r--   0        0        0        0 2023-11-06 00:21:53.369733 deepof-0.6.1/deepof/trained_models/.gitkeep
--rw-r--r--   0        0        0      133 2023-12-03 17:30:37.819353 deepof-0.6.1/deepof/trained_models/deepof_supervised/deepof_supervised_huddle_estimator.pkl
--rw-r--r--   0        0        0    76742 2023-11-06 00:21:53.369979 deepof-0.6.1/deepof/utils.py
--rw-r--r--   0        0        0   100735 2024-04-01 13:48:27.889276 deepof-0.6.1/deepof/visuals.py
--rw-r--r--   0        0        0     3211 2024-04-10 16:13:41.009681 deepof-0.6.1/pyproject.toml
--rw-r--r--   0        0        0    12476 1970-01-01 00:00:00.000000 deepof-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-11-06 00:21:53.366438 deepof-0.6.2/LICENSE
+-rw-r--r--   0        0        0     9943 2024-05-23 16:18:29.285219 deepof-0.6.2/README.md
+-rw-r--r--   0        0        0     6148 2023-11-15 10:38:41.176080 deepof-0.6.2/deepof/.DS_Store
+-rw-r--r--   0        0        0       38 2023-11-06 00:21:53.366751 deepof-0.6.2/deepof/__init__.py
+-rw-r--r--   0        0        0    29664 2023-11-06 00:21:53.368751 deepof-0.6.2/deepof/annotation_utils.py
+-rw-r--r--   0        0        0   103948 2024-04-01 13:48:27.887411 deepof-0.6.2/deepof/data.py
+-rw-r--r--   0        0        0    15179 2023-11-06 00:21:53.369068 deepof-0.6.2/deepof/deepof_train_embeddings.py
+-rw-r--r--   0        0        0     8268 2023-11-06 00:21:53.369153 deepof-0.6.2/deepof/hypermodels.py
+-rw-r--r--   0        0        0    61514 2023-12-03 17:30:37.818174 deepof-0.6.2/deepof/model_utils.py
+-rw-r--r--   0        0        0    78570 2023-11-06 00:21:53.369434 deepof-0.6.2/deepof/models.py
+-rw-r--r--   0        0        0    49719 2023-12-08 11:46:57.236557 deepof-0.6.2/deepof/post_hoc.py
+-rw-r--r--   0        0        0     6148 2024-05-23 16:27:51.494103 deepof-0.6.2/deepof/trained_models/.DS_Store
+-rw-r--r--   0        0        0        0 2023-11-06 00:21:53.369733 deepof-0.6.2/deepof/trained_models/.gitkeep
+-rw-r--r--   0        0        0 10139395 2024-05-23 14:48:39.466694 deepof-0.6.2/deepof/trained_models/deepof_supervised/deepof_supervised_huddle_estimator.pkl
+-rw-r--r--   0        0        0    76742 2023-11-06 00:21:53.369979 deepof-0.6.2/deepof/utils.py
+-rw-r--r--   0        0        0   100735 2024-04-01 13:48:27.889276 deepof-0.6.2/deepof/visuals.py
+-rw-r--r--   0        0        0     3227 2024-05-23 16:18:29.281360 deepof-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0    12647 1970-01-01 00:00:00.000000 deepof-0.6.2/PKG-INFO
```

### Comparing `deepof-0.6.1/LICENSE` & `deepof-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `deepof-0.6.1/README.md` & `deepof-0.6.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 [![Pipeline](https://gitlab.mpcdf.mpg.de/lucasmir/deepof/badges/master/pipeline.svg)](https://gitlab.mpcdf.mpg.de/lucasmir/deepof/-/pipelines)
 [![Coverage](https://gitlab.mpcdf.mpg.de/lucasmir/deepof/badges/master/coverage.svg)](https://coverage.readthedocs.io/en/coverage-5.3/)
 [![Documentation Status](https://readthedocs.org/projects/deepof/badge/?version=latest)](https://deepof.readthedocs.io/en/latest)
 [![CodeFactor](https://www.codefactor.io/repository/github/lucasmiranda42/deepof/badge)](https://www.codefactor.io/repository/github/lucasmiranda42/deepof)
-[![Version](https://img.shields.io/badge/release-v0.6.1-informational)](https://pypi.org/project/deepof/)
+[![Version](https://img.shields.io/badge/release-v0.6.2-informational)](https://pypi.org/project/deepof/)
 [![MLFPM](https://img.shields.io/badge/funding-MLFPM-informational)](https://mlfpm.eu/)
 [![Black](https://img.shields.io/badge/code%20style-black-black)](https://github.com/psf/black)
 [![DOI](https://joss.theoj.org/papers/10.21105/joss.05394/status.svg)](https://doi.org/10.21105/joss.05394)
+[![Docker](https://img.shields.io/badge/docker-latest-informational)](https://hub.docker.com/repository/docker/lucasmiranda42/deepof/general)
 
 <br>
 
 <div align="center">
   <img width="350" height="350" src="https://gitlab.mpcdf.mpg.de/lucasmir/deepof/-/raw/master/logos/deepOF_logo_w_text.png">
 </div>
```

### Comparing `deepof-0.6.1/deepof/.DS_Store` & `deepof-0.6.2/deepof/.DS_Store`

 * *Files identical despite different names*

### Comparing `deepof-0.6.1/deepof/annotation_utils.py` & `deepof-0.6.2/deepof/annotation_utils.py`

 * *Files identical despite different names*

### Comparing `deepof-0.6.1/deepof/data.py` & `deepof-0.6.2/deepof/data.py`

 * *Files identical despite different names*

### Comparing `deepof-0.6.1/deepof/deepof_train_embeddings.py` & `deepof-0.6.2/deepof/deepof_train_embeddings.py`

 * *Files identical despite different names*

### Comparing `deepof-0.6.1/deepof/hypermodels.py` & `deepof-0.6.2/deepof/hypermodels.py`

 * *Files identical despite different names*

### Comparing `deepof-0.6.1/deepof/model_utils.py` & `deepof-0.6.2/deepof/model_utils.py`

 * *Files identical despite different names*

### Comparing `deepof-0.6.1/deepof/models.py` & `deepof-0.6.2/deepof/models.py`

 * *Files identical despite different names*

### Comparing `deepof-0.6.1/deepof/post_hoc.py` & `deepof-0.6.2/deepof/post_hoc.py`

 * *Files identical despite different names*

### Comparing `deepof-0.6.1/deepof/utils.py` & `deepof-0.6.2/deepof/utils.py`

 * *Files identical despite different names*

### Comparing `deepof-0.6.1/deepof/visuals.py` & `deepof-0.6.2/deepof/visuals.py`

 * *Files identical despite different names*

### Comparing `deepof-0.6.1/pyproject.toml` & `deepof-0.6.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "deepof"
-version = "0.6.1"
+version = "0.6.2"
 description = ""
 authors = ["lucas_miranda <lucas_miranda@psych.mpg.de>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.11"
 scikit-learn = "1.2.0"
@@ -17,19 +17,19 @@
 opencv-python = "^4.6.0.66"
 llvmlite = "^0.39.1"
 shap = "^0.41.0"
 networkx = "^2.8.7"
 dask-image = "^2022.9.0"
 seglearn = "^1.2.5"
 keras-tuner = {version = "^1.0.3", markers="platform_machine != 'arm64' or platform_system != 'Darwin'"}
-tensorflow-macos = {version = "2.11.0", markers="platform_machine == 'arm64' and platform_system == 'Darwin'"}
-tensorflow = {version = "2.11.0", markers="platform_machine != 'arm64' or platform_system != 'Darwin'"}
+tensorflow-macos = {version = "2.12.0", markers="platform_machine == 'arm64' or platform_system == 'Darwin'"}
+tensorflow = {version = "2.12.0", markers="platform_machine != 'arm64' or platform_system != 'Darwin'"}
 keras-tcn-macos = {version = "^1.0", markers="platform_machine == 'arm64' and platform_system == 'Darwin'"}
 keras-tcn = {version = "^3.5.0", markers="platform_machine != 'arm64' or platform_system != 'Darwin'"}
-tensorflow-probability = "0.19.0"
+tensorflow-probability = "0.20.1"
 tifffile = "^2022.8.12"
 ipykernel = "^6.16.0"
 statsmodels = "^0.13.2"
 umap-learn = "^0.5.3"
 ipywidgets = "^8.0.2"
 openpyxl = "^3.0.10"
 kaleido = "0.2.1"
@@ -55,14 +55,15 @@
     {version="2.0.1", source="PyPI", markers="sys_platform != 'linux'"},
     {version="2.0.1", source="pytorch-cpu", markers="sys_platform == 'linux'"}
 ]
 torchvision = [
     {version="0.15.2", source="PyPI", markers="sys_platform != 'linux'"},
     {version="0.15.2", source="pytorch-cpu", markers="sys_platform == 'linux'"}
 ]
+keras = "2.12"
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.8.0"
 pytest = "^7.1.3"
 hypothesis = "^6.56.1"
 sphynx = "^0.0.3"
 sphinx-press-theme = "^0.8.0"
@@ -92,29 +93,29 @@
 
 [build-system]
 requires = ["poetry==1.4.1"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.bumpver]
-current_version = "0.6.1"
+current_version = "0.6.2"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 tag_message = "{new_version}"
 tag_scope = "default"
 pre_commit_hook = ""
 post_commit_hook = ""
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
 "pyproject.toml" = [
-    'version = "{version}"',
-    'current_version = "{version}"',
+    '^version = "{version}"',
+    '^current_version = "{version}"',
 ]
 "setup.py" = [
     'version="{version}"',
 ]
 "docs/source/conf.py" = [
     'release = "{version}"',
 ]
```

### Comparing `deepof-0.6.1/PKG-INFO` & `deepof-0.6.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepof
-Version: 0.6.1
+Version: 0.6.2
 Summary: 
 Author: lucas_miranda
 Author-email: lucas_miranda@psych.mpg.de
 Requires-Python: >=3.9,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -17,14 +17,15 @@
 Requires-Dist: imageio-ffmpeg (>=0.4.7,<0.5.0)
 Requires-Dist: imblearn (>=0.0,<0.1)
 Requires-Dist: ipykernel (>=6.16.0,<7.0.0)
 Requires-Dist: ipywidgets (>=8.0.2,<9.0.0)
 Requires-Dist: joblib (>=1.2.0,<2.0.0)
 Requires-Dist: jupyter-client (==7.3.2)
 Requires-Dist: kaleido (==0.2.1)
+Requires-Dist: keras (==2.12)
 Requires-Dist: keras-tcn (>=3.5.0,<4.0.0) ; platform_machine != "arm64" or platform_system != "Darwin"
 Requires-Dist: keras-tcn-macos (>=1.0,<2.0) ; platform_machine == "arm64" and platform_system == "Darwin"
 Requires-Dist: keras-tuner (>=1.0.3,<2.0.0) ; platform_machine != "arm64" or platform_system != "Darwin"
 Requires-Dist: llvmlite (>=0.39.1,<0.40.0)
 Requires-Dist: lxml (>=4.9.1,<5.0.0)
 Requires-Dist: matplotlib (==3.7.2)
 Requires-Dist: moviepy (>=1.0.3,<2.0.0)
@@ -41,35 +42,36 @@
 Requires-Dist: shap (>=0.41.0,<0.42.0)
 Requires-Dist: sktime (>=0.24.0,<0.25.0)
 Requires-Dist: sleap-io (>=0.0.9,<0.0.10)
 Requires-Dist: spektral (==1.3.1)
 Requires-Dist: statannotations (>=0.5.0,<0.6.0)
 Requires-Dist: statsmodels (>=0.13.2,<0.14.0)
 Requires-Dist: tables (==3.8.0)
-Requires-Dist: tensorflow (==2.11.0) ; platform_machine != "arm64" or platform_system != "Darwin"
-Requires-Dist: tensorflow-macos (==2.11.0) ; platform_machine == "arm64" and platform_system == "Darwin"
-Requires-Dist: tensorflow-probability (==0.19.0)
+Requires-Dist: tensorflow (==2.12.0) ; platform_machine != "arm64" or platform_system != "Darwin"
+Requires-Dist: tensorflow-macos (==2.12.0) ; platform_machine == "arm64" or platform_system == "Darwin"
+Requires-Dist: tensorflow-probability (==0.20.1)
 Requires-Dist: tifffile (>=2022.8.12,<2023.0.0)
 Requires-Dist: torch (==2.0.1) ; sys_platform != "linux"
 Requires-Dist: torch (==2.0.1) ; sys_platform == "linux"
 Requires-Dist: torchvision (==0.15.2) ; sys_platform != "linux"
 Requires-Dist: torchvision (==0.15.2) ; sys_platform == "linux"
 Requires-Dist: tornado (==6.1)
 Requires-Dist: tqdm (>=4.64.1,<5.0.0)
 Requires-Dist: umap-learn (>=0.5.3,<0.6.0)
 Description-Content-Type: text/markdown
 
 [![Pipeline](https://gitlab.mpcdf.mpg.de/lucasmir/deepof/badges/master/pipeline.svg)](https://gitlab.mpcdf.mpg.de/lucasmir/deepof/-/pipelines)
 [![Coverage](https://gitlab.mpcdf.mpg.de/lucasmir/deepof/badges/master/coverage.svg)](https://coverage.readthedocs.io/en/coverage-5.3/)
 [![Documentation Status](https://readthedocs.org/projects/deepof/badge/?version=latest)](https://deepof.readthedocs.io/en/latest)
 [![CodeFactor](https://www.codefactor.io/repository/github/lucasmiranda42/deepof/badge)](https://www.codefactor.io/repository/github/lucasmiranda42/deepof)
-[![Version](https://img.shields.io/badge/release-v0.6.1-informational)](https://pypi.org/project/deepof/)
+[![Version](https://img.shields.io/badge/release-v0.6.2-informational)](https://pypi.org/project/deepof/)
 [![MLFPM](https://img.shields.io/badge/funding-MLFPM-informational)](https://mlfpm.eu/)
 [![Black](https://img.shields.io/badge/code%20style-black-black)](https://github.com/psf/black)
 [![DOI](https://joss.theoj.org/papers/10.21105/joss.05394/status.svg)](https://doi.org/10.21105/joss.05394)
+[![Docker](https://img.shields.io/badge/docker-latest-informational)](https://hub.docker.com/repository/docker/lucasmiranda42/deepof/general)
 
 <br>
 
 <div align="center">
   <img width="350" height="350" src="https://gitlab.mpcdf.mpg.de/lucasmir/deepof/-/raw/master/logos/deepOF_logo_w_text.png">
 </div>
```

