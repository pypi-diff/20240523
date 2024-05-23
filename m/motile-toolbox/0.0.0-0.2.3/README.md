# Comparing `tmp/motile_toolbox-0.0.0.tar.gz` & `tmp/motile_toolbox-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "motile_toolbox-0.0.0.tar", last modified: Tue May 14 13:16:16 2024, max compression
+gzip compressed data, was "motile_toolbox-0.2.3.tar", last modified: Thu May 23 01:16:32 2024, max compression
```

## Comparing `motile_toolbox-0.0.0.tar` & `motile_toolbox-0.2.3.tar`

### file list

```diff
@@ -1,29 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:16:16.361076 motile_toolbox-0.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-05-14 13:16:16.361076 motile_toolbox-0.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-05-14 13:16:11.000000 motile_toolbox-0.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-05-14 13:16:11.000000 motile_toolbox-0.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 13:16:16.361076 motile_toolbox-0.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:16:16.357076 motile_toolbox-0.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:16:16.357076 motile_toolbox-0.0.0/src/motile_toolbox/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-14 13:16:11.000000 motile_toolbox-0.0.0/src/motile_toolbox/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:16:16.361076 motile_toolbox-0.0.0/src/motile_toolbox/candidate_graph/
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-14 13:16:11.000000 motile_toolbox-0.0.0/src/motile_toolbox/candidate_graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-05-14 13:16:11.000000 motile_toolbox-0.0.0/src/motile_toolbox/candidate_graph/compute_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-14 13:16:11.000000 motile_toolbox-0.0.0/src/motile_toolbox/candidate_graph/conflict_sets.py
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-05-14 13:16:11.000000 motile_toolbox-0.0.0/src/motile_toolbox/candidate_graph/graph_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-14 13:16:11.000000 motile_toolbox-0.0.0/src/motile_toolbox/candidate_graph/graph_to_nx.py
--rw-r--r--   0 runner    (1001) docker     (127)     4485 2024-05-14 13:16:11.000000 motile_toolbox-0.0.0/src/motile_toolbox/candidate_graph/iou.py
--rw-r--r--   0 runner    (1001) docker     (127)     5849 2024-05-14 13:16:11.000000 motile_toolbox-0.0.0/src/motile_toolbox/candidate_graph/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:16:16.361076 motile_toolbox-0.0.0/src/motile_toolbox/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-14 13:16:11.000000 motile_toolbox-0.0.0/src/motile_toolbox/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3869 2024-05-14 13:16:11.000000 motile_toolbox-0.0.0/src/motile_toolbox/utils/loading_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-05-14 13:16:11.000000 motile_toolbox-0.0.0/src/motile_toolbox/utils/relabel_segmentation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:16:16.361076 motile_toolbox-0.0.0/src/motile_toolbox/visualization/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-14 13:16:11.000000 motile_toolbox-0.0.0/src/motile_toolbox/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3912 2024-05-14 13:16:11.000000 motile_toolbox-0.0.0/src/motile_toolbox/visualization/napari_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 13:16:16.361076 motile_toolbox-0.0.0/src/motile_toolbox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-05-14 13:16:16.000000 motile_toolbox-0.0.0/src/motile_toolbox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-14 13:16:16.000000 motile_toolbox-0.0.0/src/motile_toolbox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 13:16:16.000000 motile_toolbox-0.0.0/src/motile_toolbox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-14 13:16:16.000000 motile_toolbox-0.0.0/src/motile_toolbox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-14 13:16:16.000000 motile_toolbox-0.0.0/src/motile_toolbox.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:16:32.668871 motile_toolbox-0.2.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:16:32.660871 motile_toolbox-0.2.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-23 01:16:20.000000 motile_toolbox-0.2.3/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-23 01:16:20.000000 motile_toolbox-0.2.3/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:16:32.664871 motile_toolbox-0.2.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      377 2024-05-23 01:16:20.000000 motile_toolbox-0.2.3/.github/workflows/black.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-23 01:16:20.000000 motile_toolbox-0.2.3/.github/workflows/deploy.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-23 01:16:20.000000 motile_toolbox-0.2.3/.github/workflows/docs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-23 01:16:20.000000 motile_toolbox-0.2.3/.github/workflows/mypy.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-05-23 01:16:20.000000 motile_toolbox-0.2.3/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-05-23 01:16:20.000000 motile_toolbox-0.2.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-23 01:16:20.000000 motile_toolbox-0.2.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-05-23 01:16:32.668871 motile_toolbox-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-05-23 01:16:20.000000 motile_toolbox-0.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-23 01:16:20.000000 motile_toolbox-0.2.3/conda_config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-23 01:16:20.000000 motile_toolbox-0.2.3/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-05-23 01:16:20.000000 motile_toolbox-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 01:16:32.668871 motile_toolbox-0.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:16:32.660871 motile_toolbox-0.2.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:16:32.664871 motile_toolbox-0.2.3/src/motile_toolbox/
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-23 01:16:20.000000 motile_toolbox-0.2.3/src/motile_toolbox/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:16:32.664871 motile_toolbox-0.2.3/src/motile_toolbox/candidate_graph/
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-23 01:16:20.000000 motile_toolbox-0.2.3/src/motile_toolbox/candidate_graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-05-23 01:16:20.000000 motile_toolbox-0.2.3/src/motile_toolbox/candidate_graph/compute_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-23 01:16:20.000000 motile_toolbox-0.2.3/src/motile_toolbox/candidate_graph/conflict_sets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-05-23 01:16:20.000000 motile_toolbox-0.2.3/src/motile_toolbox/candidate_graph/graph_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-23 01:16:20.000000 motile_toolbox-0.2.3/src/motile_toolbox/candidate_graph/graph_to_nx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4485 2024-05-23 01:16:20.000000 motile_toolbox-0.2.3/src/motile_toolbox/candidate_graph/iou.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5849 2024-05-23 01:16:20.000000 motile_toolbox-0.2.3/src/motile_toolbox/candidate_graph/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:16:32.664871 motile_toolbox-0.2.3/src/motile_toolbox/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-23 01:16:20.000000 motile_toolbox-0.2.3/src/motile_toolbox/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3869 2024-05-23 01:16:20.000000 motile_toolbox-0.2.3/src/motile_toolbox/utils/loading_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-05-23 01:16:20.000000 motile_toolbox-0.2.3/src/motile_toolbox/utils/relabel_segmentation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:16:32.664871 motile_toolbox-0.2.3/src/motile_toolbox/visualization/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-23 01:16:20.000000 motile_toolbox-0.2.3/src/motile_toolbox/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3912 2024-05-23 01:16:20.000000 motile_toolbox-0.2.3/src/motile_toolbox/visualization/napari_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:16:32.668871 motile_toolbox-0.2.3/src/motile_toolbox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-05-23 01:16:32.000000 motile_toolbox-0.2.3/src/motile_toolbox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-05-23 01:16:32.000000 motile_toolbox-0.2.3/src/motile_toolbox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 01:16:32.000000 motile_toolbox-0.2.3/src/motile_toolbox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-23 01:16:32.000000 motile_toolbox-0.2.3/src/motile_toolbox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-23 01:16:32.000000 motile_toolbox-0.2.3/src/motile_toolbox.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:16:32.664871 motile_toolbox-0.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     9971 2024-05-23 01:16:20.000000 motile_toolbox-0.2.3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:16:32.668871 motile_toolbox-0.2.3/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-23 01:16:20.000000 motile_toolbox-0.2.3/tests/data/attribution.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4218 2024-05-23 01:16:20.000000 motile_toolbox-0.2.3/tests/data/sample_tracks.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:16:32.668871 motile_toolbox-0.2.3/tests/test_candidate_graph/
+-rw-r--r--   0 runner    (1001) docker     (127)     3058 2024-05-23 01:16:20.000000 motile_toolbox-0.2.3/tests/test_candidate_graph/test_compute_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-05-23 01:16:20.000000 motile_toolbox-0.2.3/tests/test_candidate_graph/test_conflict_sets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-23 01:16:20.000000 motile_toolbox-0.2.3/tests/test_candidate_graph/test_graph_to_nx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-05-23 01:16:20.000000 motile_toolbox-0.2.3/tests/test_candidate_graph/test_iou.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3372 2024-05-23 01:16:20.000000 motile_toolbox-0.2.3/tests/test_candidate_graph/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 01:16:32.668871 motile_toolbox-0.2.3/tests/test_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-05-23 01:16:20.000000 motile_toolbox-0.2.3/tests/test_utils/test_loading_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-05-23 01:16:20.000000 motile_toolbox-0.2.3/tests/test_utils/test_relabel_segmentation.py
```

### Comparing `motile_toolbox-0.0.0/PKG-INFO` & `motile_toolbox-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: motile_toolbox
-Version: 0.0.0
+Version: 0.2.3
 Summary: A toolbox for tracking with (motile)[https://github.com/funkelab/motile].
 Author-email: Funke Lab <malinmayorc@janelia.hhmi.org>
 License: BSD 3-Clause License
 Project-URL: homepage, https://github.com/funkelab/motile_toolbox
 Project-URL: repository, https://github.com/funkelab/motile_toolbox
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

### Comparing `motile_toolbox-0.0.0/README.md` & `motile_toolbox-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `motile_toolbox-0.0.0/pyproject.toml` & `motile_toolbox-0.2.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [build-system]
 build-backend = "setuptools.build_meta"
-requires = ["setuptools", "wheel"]
+requires = ["setuptools>=64", "wheel", "setuptools_scm>=8"]
 
 [project]
 name = "motile_toolbox"
 description = "A toolbox for tracking with (motile)[https://github.com/funkelab/motile]."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -38,14 +38,16 @@
   'pytest-unordered'
 ]
 
 [project.urls]
 homepage = "https://github.com/funkelab/motile_toolbox"
 repository = "https://github.com/funkelab/motile_toolbox"
 
+[tool.setuptools_scm]
+
 [tool.coverage.run]
 omit = ["src/motile_toolbox/visualization/*"]
 
 # https://github.com/charliermarsh/ruff
 [tool.ruff]
 line-length = 88
 target-version = "py38"
```

### Comparing `motile_toolbox-0.0.0/src/motile_toolbox/candidate_graph/compute_graph.py` & `motile_toolbox-0.2.3/src/motile_toolbox/candidate_graph/compute_graph.py`

 * *Files identical despite different names*

### Comparing `motile_toolbox-0.0.0/src/motile_toolbox/candidate_graph/conflict_sets.py` & `motile_toolbox-0.2.3/src/motile_toolbox/candidate_graph/conflict_sets.py`

 * *Files identical despite different names*

### Comparing `motile_toolbox-0.0.0/src/motile_toolbox/candidate_graph/graph_attributes.py` & `motile_toolbox-0.2.3/src/motile_toolbox/candidate_graph/graph_attributes.py`

 * *Files identical despite different names*

### Comparing `motile_toolbox-0.0.0/src/motile_toolbox/candidate_graph/graph_to_nx.py` & `motile_toolbox-0.2.3/src/motile_toolbox/candidate_graph/graph_to_nx.py`

 * *Files identical despite different names*

### Comparing `motile_toolbox-0.0.0/src/motile_toolbox/candidate_graph/iou.py` & `motile_toolbox-0.2.3/src/motile_toolbox/candidate_graph/iou.py`

 * *Files identical despite different names*

### Comparing `motile_toolbox-0.0.0/src/motile_toolbox/candidate_graph/utils.py` & `motile_toolbox-0.2.3/src/motile_toolbox/candidate_graph/utils.py`

 * *Files identical despite different names*

### Comparing `motile_toolbox-0.0.0/src/motile_toolbox/utils/loading_utils.py` & `motile_toolbox-0.2.3/src/motile_toolbox/utils/loading_utils.py`

 * *Files identical despite different names*

### Comparing `motile_toolbox-0.0.0/src/motile_toolbox/utils/relabel_segmentation.py` & `motile_toolbox-0.2.3/src/motile_toolbox/utils/relabel_segmentation.py`

 * *Files identical despite different names*

### Comparing `motile_toolbox-0.0.0/src/motile_toolbox/visualization/napari_utils.py` & `motile_toolbox-0.2.3/src/motile_toolbox/visualization/napari_utils.py`

 * *Files identical despite different names*

### Comparing `motile_toolbox-0.0.0/src/motile_toolbox.egg-info/PKG-INFO` & `motile_toolbox-0.2.3/src/motile_toolbox.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: motile_toolbox
-Version: 0.0.0
+Version: 0.2.3
 Summary: A toolbox for tracking with (motile)[https://github.com/funkelab/motile].
 Author-email: Funke Lab <malinmayorc@janelia.hhmi.org>
 License: BSD 3-Clause License
 Project-URL: homepage, https://github.com/funkelab/motile_toolbox
 Project-URL: repository, https://github.com/funkelab/motile_toolbox
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

