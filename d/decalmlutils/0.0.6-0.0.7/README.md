# Comparing `tmp/decalmlutils-0.0.6.tar.gz` & `tmp/decalmlutils-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decalmlutils-0.0.6.tar", last modified: Thu May 23 14:57:21 2024, max compression
+gzip compressed data, was "decalmlutils-0.0.7.tar", last modified: Thu May 23 16:18:41 2024, max compression
```

## Comparing `decalmlutils-0.0.6.tar` & `decalmlutils-0.0.7.tar`

### file list

```diff
@@ -1,54 +1,35 @@
-drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2024-05-23 14:57:21.241992 decalmlutils-0.0.6/
--rw-rw-r--   0 richard   (1000) richard   (1000)    11358 2024-02-14 15:27:04.000000 decalmlutils-0.0.6/LICENSE
--rw-r--r--   0 richard   (1000) richard   (1000)     6350 2024-05-23 14:57:21.241992 decalmlutils-0.0.6/PKG-INFO
--rw-rw-r--   0 richard   (1000) richard   (1000)     2117 2024-05-10 21:20:37.000000 decalmlutils-0.0.6/README.md
-drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2024-05-23 14:57:21.233992 decalmlutils-0.0.6/decalmlutils/
-drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2024-05-23 14:57:21.237992 decalmlutils-0.0.6/decalmlutils/decalmlutils.egg-info/
--rw-r--r--   0 richard   (1000) richard   (1000)     6350 2024-05-23 14:57:21.000000 decalmlutils-0.0.6/decalmlutils/decalmlutils.egg-info/PKG-INFO
--rw-rw-r--   0 richard   (1000) richard   (1000)     1300 2024-05-23 14:57:21.000000 decalmlutils-0.0.6/decalmlutils/decalmlutils.egg-info/SOURCES.txt
--rw-rw-r--   0 richard   (1000) richard   (1000)        1 2024-05-23 14:57:21.000000 decalmlutils-0.0.6/decalmlutils/decalmlutils.egg-info/dependency_links.txt
--rw-rw-r--   0 richard   (1000) richard   (1000)      846 2024-05-23 14:57:21.000000 decalmlutils-0.0.6/decalmlutils/decalmlutils.egg-info/requires.txt
--rw-rw-r--   0 richard   (1000) richard   (1000)       11 2024-05-23 14:57:21.000000 decalmlutils-0.0.6/decalmlutils/decalmlutils.egg-info/top_level.txt
-drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2024-05-23 14:57:21.237992 decalmlutils-0.0.6/decalmlutils/io/
--rw-rw-r--   0 richard   (1000) richard   (1000)        0 2024-02-16 14:10:58.000000 decalmlutils-0.0.6/decalmlutils/io/__init__.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     4668 2024-05-10 21:01:49.000000 decalmlutils-0.0.6/decalmlutils/io/context.py
-drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2024-05-23 14:57:21.237992 decalmlutils-0.0.6/decalmlutils/io/disk/
--rw-rw-r--   0 richard   (1000) richard   (1000)        0 2024-02-14 20:50:13.000000 decalmlutils-0.0.6/decalmlutils/io/disk/__init__.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     1699 2024-05-04 09:54:41.000000 decalmlutils-0.0.6/decalmlutils/io/disk/compressed_writer.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     1327 2024-05-10 21:05:06.000000 decalmlutils-0.0.6/decalmlutils/io/disk/geojson.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     3437 2024-05-10 21:05:06.000000 decalmlutils-0.0.6/decalmlutils/io/disk/img.py
--rw-rw-r--   0 richard   (1000) richard   (1000)      682 2024-05-10 21:05:06.000000 decalmlutils-0.0.6/decalmlutils/io/disk/json.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     2191 2024-05-10 21:05:06.000000 decalmlutils-0.0.6/decalmlutils/io/disk/misc.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     5220 2024-05-10 21:01:49.000000 decalmlutils-0.0.6/decalmlutils/io/disk/parquet.py
--rw-rw-r--   0 richard   (1000) richard   (1000)      196 2024-02-14 20:50:13.000000 decalmlutils-0.0.6/decalmlutils/io/disk/yaml.py
--rw-rw-r--   0 richard   (1000) richard   (1000)      966 2024-02-14 21:13:54.000000 decalmlutils-0.0.6/decalmlutils/io/git_.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     2655 2024-05-23 14:52:03.000000 decalmlutils-0.0.6/decalmlutils/io/jira_.py
-drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2024-05-23 14:57:21.237992 decalmlutils-0.0.6/decalmlutils/io/mflow/
--rw-rw-r--   0 richard   (1000) richard   (1000)      469 2024-05-10 21:05:06.000000 decalmlutils-0.0.6/decalmlutils/io/mflow/__init__.py
--rw-rw-r--   0 richard   (1000) richard   (1000)    19247 2024-05-10 21:05:06.000000 decalmlutils-0.0.6/decalmlutils/io/mflow/artifacts.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     2845 2024-05-10 21:22:50.000000 decalmlutils-0.0.6/decalmlutils/io/mflow/cloudwatch_logs.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     4238 2024-02-15 15:48:28.000000 decalmlutils-0.0.6/decalmlutils/io/mflow/decorators.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     4077 2024-05-10 21:05:06.000000 decalmlutils-0.0.6/decalmlutils/io/mflow/deps.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     1029 2024-02-14 22:19:06.000000 decalmlutils-0.0.6/decalmlutils/io/mflow/flows.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     7696 2024-05-10 21:05:06.000000 decalmlutils-0.0.6/decalmlutils/io/mflow/lineage.py
--rw-rw-r--   0 richard   (1000) richard   (1000)    15127 2024-02-15 15:50:10.000000 decalmlutils-0.0.6/decalmlutils/io/mflow/runs.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     1786 2024-02-15 15:48:28.000000 decalmlutils-0.0.6/decalmlutils/io/mflow/tasks.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     2890 2024-05-10 21:05:06.000000 decalmlutils-0.0.6/decalmlutils/io/mflow/workflows.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     7067 2024-05-21 21:12:36.000000 decalmlutils-0.0.6/decalmlutils/io/misc.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     6595 2024-05-23 14:44:07.000000 decalmlutils-0.0.6/decalmlutils/io/slack.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     1284 2024-02-14 21:25:06.000000 decalmlutils-0.0.6/decalmlutils/io/sort.py
-drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2024-05-23 14:57:21.237992 decalmlutils-0.0.6/decalmlutils/metrics/
--rw-rw-r--   0 richard   (1000) richard   (1000)        0 2024-02-16 14:13:02.000000 decalmlutils-0.0.6/decalmlutils/metrics/__init__.py
--rw-rw-r--   0 richard   (1000) richard   (1000)    12437 2024-05-10 21:05:06.000000 decalmlutils-0.0.6/decalmlutils/metrics/misc.py
--rw-rw-r--   0 richard   (1000) richard   (1000)    17049 2024-05-10 21:05:07.000000 decalmlutils-0.0.6/decalmlutils/metrics/prg.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     2143 2024-03-04 16:56:09.000000 decalmlutils-0.0.6/decalmlutils/metrics/rankme.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     1043 2024-05-23 14:38:06.000000 decalmlutils-0.0.6/pyproject.toml
--rw-rw-r--   0 richard   (1000) richard   (1000)       38 2024-05-23 14:57:21.241992 decalmlutils-0.0.6/setup.cfg
--rw-rw-r--   0 richard   (1000) richard   (1000)     3930 2024-05-23 14:54:25.000000 decalmlutils-0.0.6/setup.py
-drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2024-05-23 14:57:21.237992 decalmlutils-0.0.6/tests/
--rw-rw-r--   0 richard   (1000) richard   (1000)        0 2024-02-14 21:27:17.000000 decalmlutils-0.0.6/tests/test_plotting.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     1586 2024-05-10 21:05:07.000000 decalmlutils-0.0.6/tests/test_tensors.py
--rw-rw-r--   0 richard   (1000) richard   (1000)      233 2024-05-10 21:05:07.000000 decalmlutils-0.0.6/tests/test_testing.py
--rw-rw-r--   0 richard   (1000) richard   (1000)        0 2024-02-14 21:25:36.000000 decalmlutils-0.0.6/tests/test_text.py
--rw-rw-r--   0 richard   (1000) richard   (1000)      167 2024-05-23 14:45:15.000000 decalmlutils-0.0.6/tests/test_training.py
--rw-rw-r--   0 richard   (1000) richard   (1000)        0 2024-02-16 17:31:23.000000 decalmlutils-0.0.6/tests/test_web.py
+drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2024-05-23 16:18:41.171460 decalmlutils-0.0.7/
+-rw-rw-r--   0 richard   (1000) richard   (1000)    11358 2024-02-14 15:27:04.000000 decalmlutils-0.0.7/LICENSE
+-rw-r--r--   0 richard   (1000) richard   (1000)     6350 2024-05-23 16:18:41.171460 decalmlutils-0.0.7/PKG-INFO
+-rw-rw-r--   0 richard   (1000) richard   (1000)     2117 2024-05-10 21:20:37.000000 decalmlutils-0.0.7/README.md
+drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2024-05-23 16:18:41.167460 decalmlutils-0.0.7/decalmlutils/
+-rw-rw-r--   0 richard   (1000) richard   (1000)      330 2024-05-23 16:18:32.000000 decalmlutils-0.0.7/decalmlutils/__init__.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)      659 2024-05-10 21:26:05.000000 decalmlutils-0.0.7/decalmlutils/dataframes.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)    22461 2024-05-10 18:40:47.000000 decalmlutils-0.0.7/decalmlutils/debug_info.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     2119 2024-02-16 14:37:48.000000 decalmlutils-0.0.7/decalmlutils/geom.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     2042 2024-05-23 14:29:50.000000 decalmlutils-0.0.7/decalmlutils/logging_utils.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     1435 2024-05-04 10:01:16.000000 decalmlutils-0.0.7/decalmlutils/np_memmap.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)       39 2024-02-14 22:42:19.000000 decalmlutils-0.0.7/decalmlutils/plotting.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     2582 2024-02-16 14:01:25.000000 decalmlutils-0.0.7/decalmlutils/profiling.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     3016 2024-02-16 13:58:24.000000 decalmlutils-0.0.7/decalmlutils/ray_utils.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     4080 2024-02-16 14:05:12.000000 decalmlutils-0.0.7/decalmlutils/tensors.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)      878 2024-02-15 15:26:01.000000 decalmlutils-0.0.7/decalmlutils/testing.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)       46 2024-02-14 20:27:28.000000 decalmlutils-0.0.7/decalmlutils/text.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     1561 2024-05-10 21:28:40.000000 decalmlutils-0.0.7/decalmlutils/training.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)       47 2024-02-14 20:27:28.000000 decalmlutils-0.0.7/decalmlutils/web.py
+drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2024-05-23 16:18:41.167460 decalmlutils-0.0.7/decalmlutils.egg-info/
+-rw-r--r--   0 richard   (1000) richard   (1000)     6350 2024-05-23 16:18:41.000000 decalmlutils-0.0.7/decalmlutils.egg-info/PKG-INFO
+-rw-rw-r--   0 richard   (1000) richard   (1000)      694 2024-05-23 16:18:41.000000 decalmlutils-0.0.7/decalmlutils.egg-info/SOURCES.txt
+-rw-rw-r--   0 richard   (1000) richard   (1000)        1 2024-05-23 16:18:41.000000 decalmlutils-0.0.7/decalmlutils.egg-info/dependency_links.txt
+-rw-rw-r--   0 richard   (1000) richard   (1000)      846 2024-05-23 16:18:41.000000 decalmlutils-0.0.7/decalmlutils.egg-info/requires.txt
+-rw-rw-r--   0 richard   (1000) richard   (1000)       13 2024-05-23 16:18:41.000000 decalmlutils-0.0.7/decalmlutils.egg-info/top_level.txt
+-rw-rw-r--   0 richard   (1000) richard   (1000)     1043 2024-05-23 14:38:06.000000 decalmlutils-0.0.7/pyproject.toml
+-rw-rw-r--   0 richard   (1000) richard   (1000)       38 2024-05-23 16:18:41.171460 decalmlutils-0.0.7/setup.cfg
+-rw-rw-r--   0 richard   (1000) richard   (1000)     3902 2024-05-23 16:18:32.000000 decalmlutils-0.0.7/setup.py
+drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2024-05-23 16:18:41.167460 decalmlutils-0.0.7/tests/
+-rw-rw-r--   0 richard   (1000) richard   (1000)        0 2024-02-14 21:27:17.000000 decalmlutils-0.0.7/tests/test_plotting.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     1586 2024-05-10 21:05:07.000000 decalmlutils-0.0.7/tests/test_tensors.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)      233 2024-05-10 21:05:07.000000 decalmlutils-0.0.7/tests/test_testing.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)        0 2024-02-14 21:25:36.000000 decalmlutils-0.0.7/tests/test_text.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)      167 2024-05-23 14:45:15.000000 decalmlutils-0.0.7/tests/test_training.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)        0 2024-02-16 17:31:23.000000 decalmlutils-0.0.7/tests/test_web.py
```

### Comparing `decalmlutils-0.0.6/LICENSE` & `decalmlutils-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `decalmlutils-0.0.6/PKG-INFO` & `decalmlutils-0.0.7/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decalmlutils
-Version: 0.0.6
+Version: 0.0.7
 Summary: Useful functions when working with Machine Learning in Python
 Home-page: https://github.com/crypdick/decalmlutils
 Author: Richard Decal
 Author-email: public@richarddecal.com
 License: Apache
 Keywords: deep learning pytorch numpy
 Classifier: Development Status :: 5 - Production/Stable
@@ -72,49 +72,49 @@
 Requires-Dist: pytest; extra == "tests"
 Requires-Dist: pytest-cov; extra == "tests"
 Requires-Dist: pytest-env; extra == "tests"
 Requires-Dist: pytest-xdist; extra == "tests"
 Requires-Dist: pytest-mock; extra == "tests"
 Requires-Dist: hypothesis; extra == "tests"
 Provides-Extra: all
-Requires-Dist: boto3; extra == "all"
-Requires-Dist: slack_sdk; extra == "all"
-Requires-Dist: build; extra == "all"
-Requires-Dist: pytest-mock; extra == "all"
-Requires-Dist: pytest-xdist; extra == "all"
 Requires-Dist: ipython; extra == "all"
-Requires-Dist: pytest-env; extra == "all"
-Requires-Dist: GitPython; extra == "all"
-Requires-Dist: scikit-learn; extra == "all"
-Requires-Dist: pytest; extra == "all"
-Requires-Dist: hypothesis; extra == "all"
-Requires-Dist: pyarrow; extra == "all"
+Requires-Dist: requests; extra == "all"
+Requires-Dist: torchvision; extra == "all"
 Requires-Dist: jira; extra == "all"
 Requires-Dist: pre-commit; extra == "all"
+Requires-Dist: build; extra == "all"
+Requires-Dist: pytest-xdist; extra == "all"
 Requires-Dist: watchtower; extra == "all"
-Requires-Dist: ray; extra == "all"
+Requires-Dist: pytest-env; extra == "all"
+Requires-Dist: graphviz; extra == "all"
 Requires-Dist: metaflow; extra == "all"
-Requires-Dist: matplotlib>=3.4.0; extra == "all"
-Requires-Dist: numpy; extra == "all"
-Requires-Dist: twine; extra == "all"
-Requires-Dist: bump2version; extra == "all"
-Requires-Dist: torchvision; extra == "all"
-Requires-Dist: seaborn; extra == "all"
-Requires-Dist: tenacity; extra == "all"
-Requires-Dist: click; extra == "all"
+Requires-Dist: ray; extra == "all"
 Requires-Dist: jinja2; extra == "all"
+Requires-Dist: seaborn; extra == "all"
 Requires-Dist: pyinstrument; extra == "all"
+Requires-Dist: boto3; extra == "all"
+Requires-Dist: hypothesis; extra == "all"
+Requires-Dist: pyarrow; extra == "all"
 Requires-Dist: torch; extra == "all"
-Requires-Dist: graphviz; extra == "all"
 Requires-Dist: pandas; extra == "all"
+Requires-Dist: pytest; extra == "all"
+Requires-Dist: geojson; extra == "all"
+Requires-Dist: bump2version; extra == "all"
+Requires-Dist: slack_sdk; extra == "all"
+Requires-Dist: twine; extra == "all"
+Requires-Dist: matplotlib>=3.4.0; extra == "all"
+Requires-Dist: numpy; extra == "all"
 Requires-Dist: isort; extra == "all"
 Requires-Dist: ruff; extra == "all"
+Requires-Dist: scikit-learn; extra == "all"
+Requires-Dist: tenacity; extra == "all"
+Requires-Dist: click; extra == "all"
 Requires-Dist: pytest-cov; extra == "all"
-Requires-Dist: requests; extra == "all"
-Requires-Dist: geojson; extra == "all"
+Requires-Dist: pytest-mock; extra == "all"
+Requires-Dist: GitPython; extra == "all"
 
 # decalmlutils
 
 [![Build status](https://github.com/crypdick/decalmlutils/actions/workflows/python-app.yml/badge.svg)](https://github.com/crypdick/decalmlutils/actions/workflows/python-app.yml)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
```

### Comparing `decalmlutils-0.0.6/README.md` & `decalmlutils-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `decalmlutils-0.0.6/decalmlutils/decalmlutils.egg-info/PKG-INFO` & `decalmlutils-0.0.7/decalmlutils.egg-info/PKG-INFO`

 * *Files identical despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decalmlutils
-Version: 0.0.6
+Version: 0.0.7
 Summary: Useful functions when working with Machine Learning in Python
 Home-page: https://github.com/crypdick/decalmlutils
 Author: Richard Decal
 Author-email: public@richarddecal.com
 License: Apache
 Keywords: deep learning pytorch numpy
 Classifier: Development Status :: 5 - Production/Stable
@@ -72,49 +72,49 @@
 Requires-Dist: pytest; extra == "tests"
 Requires-Dist: pytest-cov; extra == "tests"
 Requires-Dist: pytest-env; extra == "tests"
 Requires-Dist: pytest-xdist; extra == "tests"
 Requires-Dist: pytest-mock; extra == "tests"
 Requires-Dist: hypothesis; extra == "tests"
 Provides-Extra: all
-Requires-Dist: boto3; extra == "all"
-Requires-Dist: slack_sdk; extra == "all"
-Requires-Dist: build; extra == "all"
-Requires-Dist: pytest-mock; extra == "all"
-Requires-Dist: pytest-xdist; extra == "all"
 Requires-Dist: ipython; extra == "all"
-Requires-Dist: pytest-env; extra == "all"
-Requires-Dist: GitPython; extra == "all"
-Requires-Dist: scikit-learn; extra == "all"
-Requires-Dist: pytest; extra == "all"
-Requires-Dist: hypothesis; extra == "all"
-Requires-Dist: pyarrow; extra == "all"
+Requires-Dist: requests; extra == "all"
+Requires-Dist: torchvision; extra == "all"
 Requires-Dist: jira; extra == "all"
 Requires-Dist: pre-commit; extra == "all"
+Requires-Dist: build; extra == "all"
+Requires-Dist: pytest-xdist; extra == "all"
 Requires-Dist: watchtower; extra == "all"
-Requires-Dist: ray; extra == "all"
+Requires-Dist: pytest-env; extra == "all"
+Requires-Dist: graphviz; extra == "all"
 Requires-Dist: metaflow; extra == "all"
-Requires-Dist: matplotlib>=3.4.0; extra == "all"
-Requires-Dist: numpy; extra == "all"
-Requires-Dist: twine; extra == "all"
-Requires-Dist: bump2version; extra == "all"
-Requires-Dist: torchvision; extra == "all"
-Requires-Dist: seaborn; extra == "all"
-Requires-Dist: tenacity; extra == "all"
-Requires-Dist: click; extra == "all"
+Requires-Dist: ray; extra == "all"
 Requires-Dist: jinja2; extra == "all"
+Requires-Dist: seaborn; extra == "all"
 Requires-Dist: pyinstrument; extra == "all"
+Requires-Dist: boto3; extra == "all"
+Requires-Dist: hypothesis; extra == "all"
+Requires-Dist: pyarrow; extra == "all"
 Requires-Dist: torch; extra == "all"
-Requires-Dist: graphviz; extra == "all"
 Requires-Dist: pandas; extra == "all"
+Requires-Dist: pytest; extra == "all"
+Requires-Dist: geojson; extra == "all"
+Requires-Dist: bump2version; extra == "all"
+Requires-Dist: slack_sdk; extra == "all"
+Requires-Dist: twine; extra == "all"
+Requires-Dist: matplotlib>=3.4.0; extra == "all"
+Requires-Dist: numpy; extra == "all"
 Requires-Dist: isort; extra == "all"
 Requires-Dist: ruff; extra == "all"
+Requires-Dist: scikit-learn; extra == "all"
+Requires-Dist: tenacity; extra == "all"
+Requires-Dist: click; extra == "all"
 Requires-Dist: pytest-cov; extra == "all"
-Requires-Dist: requests; extra == "all"
-Requires-Dist: geojson; extra == "all"
+Requires-Dist: pytest-mock; extra == "all"
+Requires-Dist: GitPython; extra == "all"
 
 # decalmlutils
 
 [![Build status](https://github.com/crypdick/decalmlutils/actions/workflows/python-app.yml/badge.svg)](https://github.com/crypdick/decalmlutils/actions/workflows/python-app.yml)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
```

### Comparing `decalmlutils-0.0.6/decalmlutils/decalmlutils.egg-info/requires.txt` & `decalmlutils-0.0.7/decalmlutils.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -2,49 +2,49 @@
 ftfy>=5.8
 beartype
 pydantic
 pydantic-settings
 natsort
 
 [all]
-boto3
-slack_sdk
-build
-pytest-mock
-pytest-xdist
 ipython
-pytest-env
-GitPython
-scikit-learn
-pytest
-hypothesis
-pyarrow
+requests
+torchvision
 jira
 pre-commit
+build
+pytest-xdist
 watchtower
-ray
+pytest-env
+graphviz
 metaflow
-matplotlib>=3.4.0
-numpy
-twine
-bump2version
-torchvision
-seaborn
-tenacity
-click
+ray
 jinja2
+seaborn
 pyinstrument
+boto3
+hypothesis
+pyarrow
 torch
-graphviz
 pandas
+pytest
+geojson
+bump2version
+slack_sdk
+twine
+matplotlib>=3.4.0
+numpy
 isort
 ruff
+scikit-learn
+tenacity
+click
 pytest-cov
-requests
-geojson
+pytest-mock
+GitPython
 
 [aws]
 boto3
 watchtower
 tenacity
 
 [dev]
```

### Comparing `decalmlutils-0.0.6/pyproject.toml` & `decalmlutils-0.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `decalmlutils-0.0.6/setup.py` & `decalmlutils-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,25 +82,24 @@
 extras = {
     **_extras,
     "all": list({dep for deps in _extras.values() for dep in deps}),
 }
 
 setup(
     name="decalmlutils",
-    version="0.0.6",
+    version="0.0.7",
     author="Richard Decal",
     author_email="public@richarddecal.com",
     description="Useful functions when working with Machine Learning in Python",
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     keywords="deep learning pytorch numpy",
     license="Apache",
     url="https://github.com/crypdick/decalmlutils",
-    package_dir={"": "decalmlutils"},
-    packages=find_packages("decalmlutils"),
+    packages=find_packages(include=["decalmlutils"]),
     install_requires=base_reqs,
     extras_require=extras,
     python_requires=">=3.9.0",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Intended Audience :: Education",
```

### Comparing `decalmlutils-0.0.6/tests/test_tensors.py` & `decalmlutils-0.0.7/tests/test_tensors.py`

 * *Files identical despite different names*

