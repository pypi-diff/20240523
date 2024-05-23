# Comparing `tmp/decalmlutils-0.0.5.tar.gz` & `tmp/decalmlutils-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decalmlutils-0.0.5.tar", last modified: Tue May 21 21:21:22 2024, max compression
+gzip compressed data, was "decalmlutils-0.0.6.tar", last modified: Thu May 23 14:57:21 2024, max compression
```

## Comparing `decalmlutils-0.0.5.tar` & `decalmlutils-0.0.6.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2024-05-21 21:21:22.436585 decalmlutils-0.0.5/
--rw-rw-r--   0 richard   (1000) richard   (1000)    11358 2024-02-14 15:27:04.000000 decalmlutils-0.0.5/LICENSE
--rw-r--r--   0 richard   (1000) richard   (1000)     6350 2024-05-21 21:21:22.436585 decalmlutils-0.0.5/PKG-INFO
--rw-rw-r--   0 richard   (1000) richard   (1000)     2117 2024-05-10 21:20:37.000000 decalmlutils-0.0.5/README.md
-drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2024-05-21 21:21:22.432584 decalmlutils-0.0.5/decalmlutils/
-drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2024-05-21 21:21:22.432584 decalmlutils-0.0.5/decalmlutils/decalmlutils.egg-info/
--rw-r--r--   0 richard   (1000) richard   (1000)     6350 2024-05-21 21:21:22.000000 decalmlutils-0.0.5/decalmlutils/decalmlutils.egg-info/PKG-INFO
--rw-rw-r--   0 richard   (1000) richard   (1000)     1300 2024-05-21 21:21:22.000000 decalmlutils-0.0.5/decalmlutils/decalmlutils.egg-info/SOURCES.txt
--rw-rw-r--   0 richard   (1000) richard   (1000)        1 2024-05-21 21:21:22.000000 decalmlutils-0.0.5/decalmlutils/decalmlutils.egg-info/dependency_links.txt
--rw-rw-r--   0 richard   (1000) richard   (1000)      846 2024-05-21 21:21:22.000000 decalmlutils-0.0.5/decalmlutils/decalmlutils.egg-info/requires.txt
--rw-rw-r--   0 richard   (1000) richard   (1000)       11 2024-05-21 21:21:22.000000 decalmlutils-0.0.5/decalmlutils/decalmlutils.egg-info/top_level.txt
-drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2024-05-21 21:21:22.432584 decalmlutils-0.0.5/decalmlutils/io/
--rw-rw-r--   0 richard   (1000) richard   (1000)        0 2024-02-16 14:10:58.000000 decalmlutils-0.0.5/decalmlutils/io/__init__.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     4668 2024-05-10 21:01:49.000000 decalmlutils-0.0.5/decalmlutils/io/context.py
-drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2024-05-21 21:21:22.432584 decalmlutils-0.0.5/decalmlutils/io/disk/
--rw-rw-r--   0 richard   (1000) richard   (1000)        0 2024-02-14 20:50:13.000000 decalmlutils-0.0.5/decalmlutils/io/disk/__init__.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     1699 2024-05-04 09:54:41.000000 decalmlutils-0.0.5/decalmlutils/io/disk/compressed_writer.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     1327 2024-05-10 21:05:06.000000 decalmlutils-0.0.5/decalmlutils/io/disk/geojson.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     3437 2024-05-10 21:05:06.000000 decalmlutils-0.0.5/decalmlutils/io/disk/img.py
--rw-rw-r--   0 richard   (1000) richard   (1000)      682 2024-05-10 21:05:06.000000 decalmlutils-0.0.5/decalmlutils/io/disk/json.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     2191 2024-05-10 21:05:06.000000 decalmlutils-0.0.5/decalmlutils/io/disk/misc.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     5220 2024-05-10 21:01:49.000000 decalmlutils-0.0.5/decalmlutils/io/disk/parquet.py
--rw-rw-r--   0 richard   (1000) richard   (1000)      196 2024-02-14 20:50:13.000000 decalmlutils-0.0.5/decalmlutils/io/disk/yaml.py
--rw-rw-r--   0 richard   (1000) richard   (1000)      966 2024-02-14 21:13:54.000000 decalmlutils-0.0.5/decalmlutils/io/git_.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     2767 2024-05-10 21:05:05.000000 decalmlutils-0.0.5/decalmlutils/io/jira_.py
-drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2024-05-21 21:21:22.432584 decalmlutils-0.0.5/decalmlutils/io/mflow/
--rw-rw-r--   0 richard   (1000) richard   (1000)      469 2024-05-10 21:05:06.000000 decalmlutils-0.0.5/decalmlutils/io/mflow/__init__.py
--rw-rw-r--   0 richard   (1000) richard   (1000)    19247 2024-05-10 21:05:06.000000 decalmlutils-0.0.5/decalmlutils/io/mflow/artifacts.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     2845 2024-05-10 21:22:50.000000 decalmlutils-0.0.5/decalmlutils/io/mflow/cloudwatch_logs.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     4238 2024-02-15 15:48:28.000000 decalmlutils-0.0.5/decalmlutils/io/mflow/decorators.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     4077 2024-05-10 21:05:06.000000 decalmlutils-0.0.5/decalmlutils/io/mflow/deps.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     1029 2024-02-14 22:19:06.000000 decalmlutils-0.0.5/decalmlutils/io/mflow/flows.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     7696 2024-05-10 21:05:06.000000 decalmlutils-0.0.5/decalmlutils/io/mflow/lineage.py
--rw-rw-r--   0 richard   (1000) richard   (1000)    15127 2024-02-15 15:50:10.000000 decalmlutils-0.0.5/decalmlutils/io/mflow/runs.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     1786 2024-02-15 15:48:28.000000 decalmlutils-0.0.5/decalmlutils/io/mflow/tasks.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     2890 2024-05-10 21:05:06.000000 decalmlutils-0.0.5/decalmlutils/io/mflow/workflows.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     7067 2024-05-21 21:12:36.000000 decalmlutils-0.0.5/decalmlutils/io/misc.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     6697 2024-05-10 21:05:05.000000 decalmlutils-0.0.5/decalmlutils/io/slack.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     1284 2024-02-14 21:25:06.000000 decalmlutils-0.0.5/decalmlutils/io/sort.py
-drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2024-05-21 21:21:22.432584 decalmlutils-0.0.5/decalmlutils/metrics/
--rw-rw-r--   0 richard   (1000) richard   (1000)        0 2024-02-16 14:13:02.000000 decalmlutils-0.0.5/decalmlutils/metrics/__init__.py
--rw-rw-r--   0 richard   (1000) richard   (1000)    12437 2024-05-10 21:05:06.000000 decalmlutils-0.0.5/decalmlutils/metrics/misc.py
--rw-rw-r--   0 richard   (1000) richard   (1000)    17049 2024-05-10 21:05:07.000000 decalmlutils-0.0.5/decalmlutils/metrics/prg.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     2143 2024-03-04 16:56:09.000000 decalmlutils-0.0.5/decalmlutils/metrics/rankme.py
--rw-rw-r--   0 richard   (1000) richard   (1000)      993 2024-05-10 21:05:05.000000 decalmlutils-0.0.5/pyproject.toml
--rw-rw-r--   0 richard   (1000) richard   (1000)       38 2024-05-21 21:21:22.436585 decalmlutils-0.0.5/setup.cfg
--rw-rw-r--   0 richard   (1000) richard   (1000)     3930 2024-05-21 21:16:30.000000 decalmlutils-0.0.5/setup.py
-drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2024-05-21 21:21:22.432584 decalmlutils-0.0.5/tests/
--rw-rw-r--   0 richard   (1000) richard   (1000)        0 2024-02-14 21:27:17.000000 decalmlutils-0.0.5/tests/test_plotting.py
--rw-rw-r--   0 richard   (1000) richard   (1000)     1586 2024-05-10 21:05:07.000000 decalmlutils-0.0.5/tests/test_tensors.py
--rw-rw-r--   0 richard   (1000) richard   (1000)      233 2024-05-10 21:05:07.000000 decalmlutils-0.0.5/tests/test_testing.py
--rw-rw-r--   0 richard   (1000) richard   (1000)        0 2024-02-14 21:25:36.000000 decalmlutils-0.0.5/tests/test_text.py
--rw-rw-r--   0 richard   (1000) richard   (1000)      416 2024-05-10 21:05:06.000000 decalmlutils-0.0.5/tests/test_training.py
--rw-rw-r--   0 richard   (1000) richard   (1000)        0 2024-02-16 17:31:23.000000 decalmlutils-0.0.5/tests/test_web.py
+drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2024-05-23 14:57:21.241992 decalmlutils-0.0.6/
+-rw-rw-r--   0 richard   (1000) richard   (1000)    11358 2024-02-14 15:27:04.000000 decalmlutils-0.0.6/LICENSE
+-rw-r--r--   0 richard   (1000) richard   (1000)     6350 2024-05-23 14:57:21.241992 decalmlutils-0.0.6/PKG-INFO
+-rw-rw-r--   0 richard   (1000) richard   (1000)     2117 2024-05-10 21:20:37.000000 decalmlutils-0.0.6/README.md
+drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2024-05-23 14:57:21.233992 decalmlutils-0.0.6/decalmlutils/
+drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2024-05-23 14:57:21.237992 decalmlutils-0.0.6/decalmlutils/decalmlutils.egg-info/
+-rw-r--r--   0 richard   (1000) richard   (1000)     6350 2024-05-23 14:57:21.000000 decalmlutils-0.0.6/decalmlutils/decalmlutils.egg-info/PKG-INFO
+-rw-rw-r--   0 richard   (1000) richard   (1000)     1300 2024-05-23 14:57:21.000000 decalmlutils-0.0.6/decalmlutils/decalmlutils.egg-info/SOURCES.txt
+-rw-rw-r--   0 richard   (1000) richard   (1000)        1 2024-05-23 14:57:21.000000 decalmlutils-0.0.6/decalmlutils/decalmlutils.egg-info/dependency_links.txt
+-rw-rw-r--   0 richard   (1000) richard   (1000)      846 2024-05-23 14:57:21.000000 decalmlutils-0.0.6/decalmlutils/decalmlutils.egg-info/requires.txt
+-rw-rw-r--   0 richard   (1000) richard   (1000)       11 2024-05-23 14:57:21.000000 decalmlutils-0.0.6/decalmlutils/decalmlutils.egg-info/top_level.txt
+drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2024-05-23 14:57:21.237992 decalmlutils-0.0.6/decalmlutils/io/
+-rw-rw-r--   0 richard   (1000) richard   (1000)        0 2024-02-16 14:10:58.000000 decalmlutils-0.0.6/decalmlutils/io/__init__.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     4668 2024-05-10 21:01:49.000000 decalmlutils-0.0.6/decalmlutils/io/context.py
+drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2024-05-23 14:57:21.237992 decalmlutils-0.0.6/decalmlutils/io/disk/
+-rw-rw-r--   0 richard   (1000) richard   (1000)        0 2024-02-14 20:50:13.000000 decalmlutils-0.0.6/decalmlutils/io/disk/__init__.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     1699 2024-05-04 09:54:41.000000 decalmlutils-0.0.6/decalmlutils/io/disk/compressed_writer.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     1327 2024-05-10 21:05:06.000000 decalmlutils-0.0.6/decalmlutils/io/disk/geojson.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     3437 2024-05-10 21:05:06.000000 decalmlutils-0.0.6/decalmlutils/io/disk/img.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)      682 2024-05-10 21:05:06.000000 decalmlutils-0.0.6/decalmlutils/io/disk/json.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     2191 2024-05-10 21:05:06.000000 decalmlutils-0.0.6/decalmlutils/io/disk/misc.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     5220 2024-05-10 21:01:49.000000 decalmlutils-0.0.6/decalmlutils/io/disk/parquet.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)      196 2024-02-14 20:50:13.000000 decalmlutils-0.0.6/decalmlutils/io/disk/yaml.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)      966 2024-02-14 21:13:54.000000 decalmlutils-0.0.6/decalmlutils/io/git_.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     2655 2024-05-23 14:52:03.000000 decalmlutils-0.0.6/decalmlutils/io/jira_.py
+drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2024-05-23 14:57:21.237992 decalmlutils-0.0.6/decalmlutils/io/mflow/
+-rw-rw-r--   0 richard   (1000) richard   (1000)      469 2024-05-10 21:05:06.000000 decalmlutils-0.0.6/decalmlutils/io/mflow/__init__.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)    19247 2024-05-10 21:05:06.000000 decalmlutils-0.0.6/decalmlutils/io/mflow/artifacts.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     2845 2024-05-10 21:22:50.000000 decalmlutils-0.0.6/decalmlutils/io/mflow/cloudwatch_logs.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     4238 2024-02-15 15:48:28.000000 decalmlutils-0.0.6/decalmlutils/io/mflow/decorators.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     4077 2024-05-10 21:05:06.000000 decalmlutils-0.0.6/decalmlutils/io/mflow/deps.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     1029 2024-02-14 22:19:06.000000 decalmlutils-0.0.6/decalmlutils/io/mflow/flows.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     7696 2024-05-10 21:05:06.000000 decalmlutils-0.0.6/decalmlutils/io/mflow/lineage.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)    15127 2024-02-15 15:50:10.000000 decalmlutils-0.0.6/decalmlutils/io/mflow/runs.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     1786 2024-02-15 15:48:28.000000 decalmlutils-0.0.6/decalmlutils/io/mflow/tasks.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     2890 2024-05-10 21:05:06.000000 decalmlutils-0.0.6/decalmlutils/io/mflow/workflows.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     7067 2024-05-21 21:12:36.000000 decalmlutils-0.0.6/decalmlutils/io/misc.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     6595 2024-05-23 14:44:07.000000 decalmlutils-0.0.6/decalmlutils/io/slack.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     1284 2024-02-14 21:25:06.000000 decalmlutils-0.0.6/decalmlutils/io/sort.py
+drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2024-05-23 14:57:21.237992 decalmlutils-0.0.6/decalmlutils/metrics/
+-rw-rw-r--   0 richard   (1000) richard   (1000)        0 2024-02-16 14:13:02.000000 decalmlutils-0.0.6/decalmlutils/metrics/__init__.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)    12437 2024-05-10 21:05:06.000000 decalmlutils-0.0.6/decalmlutils/metrics/misc.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)    17049 2024-05-10 21:05:07.000000 decalmlutils-0.0.6/decalmlutils/metrics/prg.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     2143 2024-03-04 16:56:09.000000 decalmlutils-0.0.6/decalmlutils/metrics/rankme.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     1043 2024-05-23 14:38:06.000000 decalmlutils-0.0.6/pyproject.toml
+-rw-rw-r--   0 richard   (1000) richard   (1000)       38 2024-05-23 14:57:21.241992 decalmlutils-0.0.6/setup.cfg
+-rw-rw-r--   0 richard   (1000) richard   (1000)     3930 2024-05-23 14:54:25.000000 decalmlutils-0.0.6/setup.py
+drwxrwxr-x   0 richard   (1000) richard   (1000)        0 2024-05-23 14:57:21.237992 decalmlutils-0.0.6/tests/
+-rw-rw-r--   0 richard   (1000) richard   (1000)        0 2024-02-14 21:27:17.000000 decalmlutils-0.0.6/tests/test_plotting.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)     1586 2024-05-10 21:05:07.000000 decalmlutils-0.0.6/tests/test_tensors.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)      233 2024-05-10 21:05:07.000000 decalmlutils-0.0.6/tests/test_testing.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)        0 2024-02-14 21:25:36.000000 decalmlutils-0.0.6/tests/test_text.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)      167 2024-05-23 14:45:15.000000 decalmlutils-0.0.6/tests/test_training.py
+-rw-rw-r--   0 richard   (1000) richard   (1000)        0 2024-02-16 17:31:23.000000 decalmlutils-0.0.6/tests/test_web.py
```

### Comparing `decalmlutils-0.0.5/LICENSE` & `decalmlutils-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `decalmlutils-0.0.5/PKG-INFO` & `decalmlutils-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decalmlutils
-Version: 0.0.5
+Version: 0.0.6
 Summary: Useful functions when working with Machine Learning in Python
 Home-page: https://github.com/crypdick/decalmlutils
 Author: Richard Decal
 Author-email: public@richarddecal.com
 License: Apache
 Keywords: deep learning pytorch numpy
 Classifier: Development Status :: 5 - Production/Stable
@@ -73,48 +73,48 @@
 Requires-Dist: pytest-cov; extra == "tests"
 Requires-Dist: pytest-env; extra == "tests"
 Requires-Dist: pytest-xdist; extra == "tests"
 Requires-Dist: pytest-mock; extra == "tests"
 Requires-Dist: hypothesis; extra == "tests"
 Provides-Extra: all
 Requires-Dist: boto3; extra == "all"
-Requires-Dist: numpy; extra == "all"
-Requires-Dist: pyarrow; extra == "all"
-Requires-Dist: bump2version; extra == "all"
-Requires-Dist: isort; extra == "all"
-Requires-Dist: hypothesis; extra == "all"
-Requires-Dist: pytest-env; extra == "all"
-Requires-Dist: scikit-learn; extra == "all"
-Requires-Dist: torchvision; extra == "all"
-Requires-Dist: ruff; extra == "all"
-Requires-Dist: GitPython; extra == "all"
-Requires-Dist: geojson; extra == "all"
-Requires-Dist: seaborn; extra == "all"
-Requires-Dist: tenacity; extra == "all"
 Requires-Dist: slack_sdk; extra == "all"
 Requires-Dist: build; extra == "all"
-Requires-Dist: jira; extra == "all"
 Requires-Dist: pytest-mock; extra == "all"
 Requires-Dist: pytest-xdist; extra == "all"
-Requires-Dist: pytest-cov; extra == "all"
-Requires-Dist: twine; extra == "all"
 Requires-Dist: ipython; extra == "all"
-Requires-Dist: pandas; extra == "all"
+Requires-Dist: pytest-env; extra == "all"
+Requires-Dist: GitPython; extra == "all"
+Requires-Dist: scikit-learn; extra == "all"
 Requires-Dist: pytest; extra == "all"
-Requires-Dist: graphviz; extra == "all"
-Requires-Dist: jinja2; extra == "all"
+Requires-Dist: hypothesis; extra == "all"
+Requires-Dist: pyarrow; extra == "all"
+Requires-Dist: jira; extra == "all"
+Requires-Dist: pre-commit; extra == "all"
+Requires-Dist: watchtower; extra == "all"
+Requires-Dist: ray; extra == "all"
+Requires-Dist: metaflow; extra == "all"
 Requires-Dist: matplotlib>=3.4.0; extra == "all"
+Requires-Dist: numpy; extra == "all"
+Requires-Dist: twine; extra == "all"
+Requires-Dist: bump2version; extra == "all"
+Requires-Dist: torchvision; extra == "all"
+Requires-Dist: seaborn; extra == "all"
+Requires-Dist: tenacity; extra == "all"
 Requires-Dist: click; extra == "all"
-Requires-Dist: metaflow; extra == "all"
-Requires-Dist: ray; extra == "all"
+Requires-Dist: jinja2; extra == "all"
 Requires-Dist: pyinstrument; extra == "all"
-Requires-Dist: requests; extra == "all"
-Requires-Dist: pre-commit; extra == "all"
 Requires-Dist: torch; extra == "all"
-Requires-Dist: watchtower; extra == "all"
+Requires-Dist: graphviz; extra == "all"
+Requires-Dist: pandas; extra == "all"
+Requires-Dist: isort; extra == "all"
+Requires-Dist: ruff; extra == "all"
+Requires-Dist: pytest-cov; extra == "all"
+Requires-Dist: requests; extra == "all"
+Requires-Dist: geojson; extra == "all"
 
 # decalmlutils
 
 [![Build status](https://github.com/crypdick/decalmlutils/actions/workflows/python-app.yml/badge.svg)](https://github.com/crypdick/decalmlutils/actions/workflows/python-app.yml)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
```

### Comparing `decalmlutils-0.0.5/README.md` & `decalmlutils-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `decalmlutils-0.0.5/decalmlutils/decalmlutils.egg-info/PKG-INFO` & `decalmlutils-0.0.6/decalmlutils/decalmlutils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decalmlutils
-Version: 0.0.5
+Version: 0.0.6
 Summary: Useful functions when working with Machine Learning in Python
 Home-page: https://github.com/crypdick/decalmlutils
 Author: Richard Decal
 Author-email: public@richarddecal.com
 License: Apache
 Keywords: deep learning pytorch numpy
 Classifier: Development Status :: 5 - Production/Stable
@@ -73,48 +73,48 @@
 Requires-Dist: pytest-cov; extra == "tests"
 Requires-Dist: pytest-env; extra == "tests"
 Requires-Dist: pytest-xdist; extra == "tests"
 Requires-Dist: pytest-mock; extra == "tests"
 Requires-Dist: hypothesis; extra == "tests"
 Provides-Extra: all
 Requires-Dist: boto3; extra == "all"
-Requires-Dist: numpy; extra == "all"
-Requires-Dist: pyarrow; extra == "all"
-Requires-Dist: bump2version; extra == "all"
-Requires-Dist: isort; extra == "all"
-Requires-Dist: hypothesis; extra == "all"
-Requires-Dist: pytest-env; extra == "all"
-Requires-Dist: scikit-learn; extra == "all"
-Requires-Dist: torchvision; extra == "all"
-Requires-Dist: ruff; extra == "all"
-Requires-Dist: GitPython; extra == "all"
-Requires-Dist: geojson; extra == "all"
-Requires-Dist: seaborn; extra == "all"
-Requires-Dist: tenacity; extra == "all"
 Requires-Dist: slack_sdk; extra == "all"
 Requires-Dist: build; extra == "all"
-Requires-Dist: jira; extra == "all"
 Requires-Dist: pytest-mock; extra == "all"
 Requires-Dist: pytest-xdist; extra == "all"
-Requires-Dist: pytest-cov; extra == "all"
-Requires-Dist: twine; extra == "all"
 Requires-Dist: ipython; extra == "all"
-Requires-Dist: pandas; extra == "all"
+Requires-Dist: pytest-env; extra == "all"
+Requires-Dist: GitPython; extra == "all"
+Requires-Dist: scikit-learn; extra == "all"
 Requires-Dist: pytest; extra == "all"
-Requires-Dist: graphviz; extra == "all"
-Requires-Dist: jinja2; extra == "all"
+Requires-Dist: hypothesis; extra == "all"
+Requires-Dist: pyarrow; extra == "all"
+Requires-Dist: jira; extra == "all"
+Requires-Dist: pre-commit; extra == "all"
+Requires-Dist: watchtower; extra == "all"
+Requires-Dist: ray; extra == "all"
+Requires-Dist: metaflow; extra == "all"
 Requires-Dist: matplotlib>=3.4.0; extra == "all"
+Requires-Dist: numpy; extra == "all"
+Requires-Dist: twine; extra == "all"
+Requires-Dist: bump2version; extra == "all"
+Requires-Dist: torchvision; extra == "all"
+Requires-Dist: seaborn; extra == "all"
+Requires-Dist: tenacity; extra == "all"
 Requires-Dist: click; extra == "all"
-Requires-Dist: metaflow; extra == "all"
-Requires-Dist: ray; extra == "all"
+Requires-Dist: jinja2; extra == "all"
 Requires-Dist: pyinstrument; extra == "all"
-Requires-Dist: requests; extra == "all"
-Requires-Dist: pre-commit; extra == "all"
 Requires-Dist: torch; extra == "all"
-Requires-Dist: watchtower; extra == "all"
+Requires-Dist: graphviz; extra == "all"
+Requires-Dist: pandas; extra == "all"
+Requires-Dist: isort; extra == "all"
+Requires-Dist: ruff; extra == "all"
+Requires-Dist: pytest-cov; extra == "all"
+Requires-Dist: requests; extra == "all"
+Requires-Dist: geojson; extra == "all"
 
 # decalmlutils
 
 [![Build status](https://github.com/crypdick/decalmlutils/actions/workflows/python-app.yml/badge.svg)](https://github.com/crypdick/decalmlutils/actions/workflows/python-app.yml)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
 
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
```

### Comparing `decalmlutils-0.0.5/decalmlutils/decalmlutils.egg-info/SOURCES.txt` & `decalmlutils-0.0.6/decalmlutils/decalmlutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `decalmlutils-0.0.5/decalmlutils/decalmlutils.egg-info/requires.txt` & `decalmlutils-0.0.6/decalmlutils/decalmlutils.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -3,48 +3,48 @@
 beartype
 pydantic
 pydantic-settings
 natsort
 
 [all]
 boto3
-numpy
-pyarrow
-bump2version
-isort
-hypothesis
-pytest-env
-scikit-learn
-torchvision
-ruff
-GitPython
-geojson
-seaborn
-tenacity
 slack_sdk
 build
-jira
 pytest-mock
 pytest-xdist
-pytest-cov
-twine
 ipython
-pandas
+pytest-env
+GitPython
+scikit-learn
 pytest
-graphviz
-jinja2
+hypothesis
+pyarrow
+jira
+pre-commit
+watchtower
+ray
+metaflow
 matplotlib>=3.4.0
+numpy
+twine
+bump2version
+torchvision
+seaborn
+tenacity
 click
-metaflow
-ray
+jinja2
 pyinstrument
-requests
-pre-commit
 torch
-watchtower
+graphviz
+pandas
+isort
+ruff
+pytest-cov
+requests
+geojson
 
 [aws]
 boto3
 watchtower
 tenacity
 
 [dev]
```

### Comparing `decalmlutils-0.0.5/decalmlutils/io/context.py` & `decalmlutils-0.0.6/decalmlutils/io/context.py`

 * *Files identical despite different names*

### Comparing `decalmlutils-0.0.5/decalmlutils/io/disk/compressed_writer.py` & `decalmlutils-0.0.6/decalmlutils/io/disk/compressed_writer.py`

 * *Files identical despite different names*

### Comparing `decalmlutils-0.0.5/decalmlutils/io/disk/geojson.py` & `decalmlutils-0.0.6/decalmlutils/io/disk/geojson.py`

 * *Files identical despite different names*

### Comparing `decalmlutils-0.0.5/decalmlutils/io/disk/img.py` & `decalmlutils-0.0.6/decalmlutils/io/disk/img.py`

 * *Files identical despite different names*

### Comparing `decalmlutils-0.0.5/decalmlutils/io/disk/json.py` & `decalmlutils-0.0.6/decalmlutils/io/disk/json.py`

 * *Files identical despite different names*

### Comparing `decalmlutils-0.0.5/decalmlutils/io/disk/misc.py` & `decalmlutils-0.0.6/decalmlutils/io/disk/misc.py`

 * *Files identical despite different names*

### Comparing `decalmlutils-0.0.5/decalmlutils/io/disk/parquet.py` & `decalmlutils-0.0.6/decalmlutils/io/disk/parquet.py`

 * *Files identical despite different names*

### Comparing `decalmlutils-0.0.5/decalmlutils/io/git_.py` & `decalmlutils-0.0.6/decalmlutils/io/git_.py`

 * *Files identical despite different names*

### Comparing `decalmlutils-0.0.5/decalmlutils/io/jira_.py` & `decalmlutils-0.0.6/decalmlutils/io/jira_.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 import logging
 from datetime import datetime
 
 from beartype import beartype
 from beartype.typing import Dict, Optional
 from jira import JIRA
 
-from decalmlutils.io.aws.secretsmanager import get_secret
-
 logger = logging.getLogger(__name__)
 
 JIRA_URL = "https://jira.foo.com"
 JIRA_TOKEN_SECRET_NAME = "jira-token"
 
 
 @beartype
@@ -43,29 +41,28 @@
         sprint_id=sprint_with_latest_end_date.id, issue_keys=issue_keys
     )
     return sprint_with_latest_end_date.name
 
 
 @beartype
 def get_or_create_epic(
-    jira_project_key: str, summary: str, jira: JIRA = None, **kwargs
+    jira_project_key: str, summary: str, jira: JIRA = None, credentials=None, **kwargs
 ):
     """
 
     Args:
         jira_project_key: Jira project key. ex "MLDC"
         summary:
         jira:
         **kwargs:
 
     Returns:
 
     """
-    creds = get_secret(JIRA_TOKEN_SECRET_NAME, jsonify=True)
-    jira = jira or JIRA(JIRA_URL, basic_auth=tuple(creds.values()))
+    jira = jira or JIRA(JIRA_URL, basic_auth=credentials)
 
     kwargs.pop("issuetype", None)
 
     for epic in jira.search_issues(f"project={jira_project_key} and issueType=Epic"):
         if epic.fields.summary == summary:
             logger.info(f"Found existing epic `{summary}`")
             return epic
```

### Comparing `decalmlutils-0.0.5/decalmlutils/io/mflow/artifacts.py` & `decalmlutils-0.0.6/decalmlutils/io/mflow/artifacts.py`

 * *Files identical despite different names*

### Comparing `decalmlutils-0.0.5/decalmlutils/io/mflow/cloudwatch_logs.py` & `decalmlutils-0.0.6/decalmlutils/io/mflow/cloudwatch_logs.py`

 * *Files identical despite different names*

### Comparing `decalmlutils-0.0.5/decalmlutils/io/mflow/decorators.py` & `decalmlutils-0.0.6/decalmlutils/io/mflow/decorators.py`

 * *Files identical despite different names*

### Comparing `decalmlutils-0.0.5/decalmlutils/io/mflow/deps.py` & `decalmlutils-0.0.6/decalmlutils/io/mflow/deps.py`

 * *Files identical despite different names*

### Comparing `decalmlutils-0.0.5/decalmlutils/io/mflow/flows.py` & `decalmlutils-0.0.6/decalmlutils/io/mflow/flows.py`

 * *Files identical despite different names*

### Comparing `decalmlutils-0.0.5/decalmlutils/io/mflow/lineage.py` & `decalmlutils-0.0.6/decalmlutils/io/mflow/lineage.py`

 * *Files identical despite different names*

### Comparing `decalmlutils-0.0.5/decalmlutils/io/mflow/runs.py` & `decalmlutils-0.0.6/decalmlutils/io/mflow/runs.py`

 * *Files identical despite different names*

### Comparing `decalmlutils-0.0.5/decalmlutils/io/mflow/tasks.py` & `decalmlutils-0.0.6/decalmlutils/io/mflow/tasks.py`

 * *Files identical despite different names*

### Comparing `decalmlutils-0.0.5/decalmlutils/io/mflow/workflows.py` & `decalmlutils-0.0.6/decalmlutils/io/mflow/workflows.py`

 * *Files identical despite different names*

### Comparing `decalmlutils-0.0.5/decalmlutils/io/misc.py` & `decalmlutils-0.0.6/decalmlutils/io/misc.py`

 * *Files identical despite different names*

### Comparing `decalmlutils-0.0.5/decalmlutils/io/slack.py` & `decalmlutils-0.0.6/decalmlutils/io/slack.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import tempfile
 from unittest.mock import MagicMock
 
 from beartype import beartype
 from beartype.typing import TYPE_CHECKING, Dict, Optional
 from slack_sdk import WebClient
 
-from decalmlutils.io.aws.secretsmanager import get_secret
 from decalmlutils.io.sort import natural_sort
 
 if TYPE_CHECKING:
     import matplotlib
 
 BOT_TOKEN_SECRET_NAME = "ml-slack-token"
 ML_ALERTS_CHANNEL = "ml-alerts"
@@ -32,21 +31,20 @@
     """
     Send plots as "ML AUTOMATION BOT" in Slack.
 
     Attributes:
         client: slack sdk web client for sending files and messages to slack
     """
 
-    def __init__(self, is_prod: bool = True):
+    def __init__(self, token: str, is_prod: bool = True):
         """
         Fetch the token and create the client right away and save them to save time when sending multiple plots.
         """
         if is_prod:
-            _token = get_secret(BOT_TOKEN_SECRET_NAME)
-            self.client = WebClient(_token)
+            self.client = WebClient(token)
         else:
             self.client = MagicMock()
             self.client.chat_postMessage = MagicMock()
             self.client.files_upload = MagicMock()
 
     @beartype
     def send_message(self, channel: str, message: str):
```

### Comparing `decalmlutils-0.0.5/decalmlutils/io/sort.py` & `decalmlutils-0.0.6/decalmlutils/io/sort.py`

 * *Files identical despite different names*

### Comparing `decalmlutils-0.0.5/decalmlutils/metrics/misc.py` & `decalmlutils-0.0.6/decalmlutils/metrics/misc.py`

 * *Files identical despite different names*

### Comparing `decalmlutils-0.0.5/decalmlutils/metrics/prg.py` & `decalmlutils-0.0.6/decalmlutils/metrics/prg.py`

 * *Files identical despite different names*

### Comparing `decalmlutils-0.0.5/decalmlutils/metrics/rankme.py` & `decalmlutils-0.0.6/decalmlutils/metrics/rankme.py`

 * *Files identical despite different names*

### Comparing `decalmlutils-0.0.5/pyproject.toml` & `decalmlutils-0.0.6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -24,17 +24,19 @@
 addopts = """
 --failed-first \
 --new-first \
 --hypothesis-explain \
 --numprocesses=auto \
 --durations=10 \
 --showlocals \
--vvv
+-m 'not skip'
 """
 # set env vars for pytest. requires pytest-env
 env = [
     "METAFLOW_PROFILE=test"
 ]
+testpaths = ["tests"]
+markers = ["skip"]
 
 [build-system]
 requires = ['setuptools>=42']
 build-backend = 'setuptools.build_meta'
```

### Comparing `decalmlutils-0.0.5/setup.py` & `decalmlutils-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 extras = {
     **_extras,
     "all": list({dep for deps in _extras.values() for dep in deps}),
 }
 
 setup(
     name="decalmlutils",
-    version="0.0.5",
+    version="0.0.6",
     author="Richard Decal",
     author_email="public@richarddecal.com",
     description="Useful functions when working with Machine Learning in Python",
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     keywords="deep learning pytorch numpy",
     license="Apache",
```

### Comparing `decalmlutils-0.0.5/tests/test_tensors.py` & `decalmlutils-0.0.6/tests/test_tensors.py`

 * *Files identical despite different names*

