# Comparing `tmp/pyhelm3-0.3.0.tar.gz` & `tmp/pyhelm3-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhelm3-0.3.0.tar", last modified: Tue May 14 15:50:33 2024, max compression
+gzip compressed data, was "pyhelm3-0.3.1.tar", last modified: Thu May 23 15:05:29 2024, max compression
```

## Comparing `pyhelm3-0.3.0.tar` & `pyhelm3-0.3.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:50:33.994490 pyhelm3-0.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:50:33.990490 pyhelm3-0.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:50:33.990490 pyhelm3-0.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-14 15:50:29.000000 pyhelm3-0.3.0/.github/workflows/pypi-publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 15:50:29.000000 pyhelm3-0.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-05-14 15:50:33.994490 pyhelm3-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-05-14 15:50:29.000000 pyhelm3-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:50:33.990490 pyhelm3-0.3.0/pyhelm3/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-14 15:50:29.000000 pyhelm3-0.3.0/pyhelm3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14776 2024-05-14 15:50:29.000000 pyhelm3-0.3.0/pyhelm3/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    32859 2024-05-14 15:50:29.000000 pyhelm3-0.3.0/pyhelm3/command.py
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-14 15:50:29.000000 pyhelm3-0.3.0/pyhelm3/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    22674 2024-05-14 15:50:29.000000 pyhelm3-0.3.0/pyhelm3/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 15:50:33.994490 pyhelm3-0.3.0/pyhelm3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-05-14 15:50:33.000000 pyhelm3-0.3.0/pyhelm3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-14 15:50:33.000000 pyhelm3-0.3.0/pyhelm3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 15:50:33.000000 pyhelm3-0.3.0/pyhelm3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 15:50:33.000000 pyhelm3-0.3.0/pyhelm3.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-14 15:50:33.000000 pyhelm3-0.3.0/pyhelm3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-14 15:50:33.000000 pyhelm3-0.3.0/pyhelm3.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-14 15:50:29.000000 pyhelm3-0.3.0/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (127)      422 2024-05-14 15:50:33.994490 pyhelm3-0.3.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)       92 2024-05-14 15:50:29.000000 pyhelm3-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:05:29.591798 pyhelm3-0.3.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:05:29.587798 pyhelm3-0.3.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:05:29.591798 pyhelm3-0.3.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-23 15:05:18.000000 pyhelm3-0.3.1/.github/workflows/pypi-publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 15:05:18.000000 pyhelm3-0.3.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-05-23 15:05:29.591798 pyhelm3-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-05-23 15:05:18.000000 pyhelm3-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:05:29.591798 pyhelm3-0.3.1/pyhelm3/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-23 15:05:18.000000 pyhelm3-0.3.1/pyhelm3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14784 2024-05-23 15:05:18.000000 pyhelm3-0.3.1/pyhelm3/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32859 2024-05-23 15:05:18.000000 pyhelm3-0.3.1/pyhelm3/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-23 15:05:18.000000 pyhelm3-0.3.1/pyhelm3/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22674 2024-05-23 15:05:18.000000 pyhelm3-0.3.1/pyhelm3/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 15:05:29.591798 pyhelm3-0.3.1/pyhelm3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-05-23 15:05:29.000000 pyhelm3-0.3.1/pyhelm3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-05-23 15:05:29.000000 pyhelm3-0.3.1/pyhelm3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 15:05:29.000000 pyhelm3-0.3.1/pyhelm3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 15:05:29.000000 pyhelm3-0.3.1/pyhelm3.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-23 15:05:29.000000 pyhelm3-0.3.1/pyhelm3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-23 15:05:29.000000 pyhelm3-0.3.1/pyhelm3.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-23 15:05:18.000000 pyhelm3-0.3.1/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      422 2024-05-23 15:05:29.591798 pyhelm3-0.3.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)       92 2024-05-23 15:05:18.000000 pyhelm3-0.3.1/setup.py
```

### Comparing `pyhelm3-0.3.0/.github/workflows/pypi-publish.yaml` & `pyhelm3-0.3.1/.github/workflows/pypi-publish.yaml`

 * *Files identical despite different names*

### Comparing `pyhelm3-0.3.0/PKG-INFO` & `pyhelm3-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhelm3
-Version: 0.3.0
+Version: 0.3.1
 Summary: Python library for managing Helm releases using Helm 3.
 Home-page: https://github.com/stackhpc/pyhelm3
 Author: Matt Pryor
 Author-email: matt@stackhpc.com
 Description-Content-Type: text/markdown
 Requires-Dist: pydantic
 Requires-Dist: pyyaml
```

### Comparing `pyhelm3-0.3.0/README.md` & `pyhelm3-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `pyhelm3-0.3.0/pyhelm3/client.py` & `pyhelm3-0.3.1/pyhelm3/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -319,15 +319,15 @@
             # If the chart has changed from the deployed release, we should redeploy
             revision_chart = await current_revision.chart_metadata()
             if revision_chart.name != chart.metadata.name:
                 return True
             if revision_chart.version != chart.metadata.version:
                 return True
             # If the values have changed from the deployed release, we should redeploy
-            revision_values = await current_revision.values()
+            revision_values = (await current_revision.values()) or {}
             if revision_values != values:
                 return True
             # If the chart and values are the same, there is nothing to do
             return False
         else:
             # No current revision - install is always required
             return True
```

### Comparing `pyhelm3-0.3.0/pyhelm3/command.py` & `pyhelm3-0.3.1/pyhelm3/command.py`

 * *Files identical despite different names*

### Comparing `pyhelm3-0.3.0/pyhelm3/errors.py` & `pyhelm3-0.3.1/pyhelm3/errors.py`

 * *Files identical despite different names*

### Comparing `pyhelm3-0.3.0/pyhelm3/models.py` & `pyhelm3-0.3.1/pyhelm3/models.py`

 * *Files identical despite different names*

### Comparing `pyhelm3-0.3.0/pyhelm3.egg-info/PKG-INFO` & `pyhelm3-0.3.1/pyhelm3.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhelm3
-Version: 0.3.0
+Version: 0.3.1
 Summary: Python library for managing Helm releases using Helm 3.
 Home-page: https://github.com/stackhpc/pyhelm3
 Author: Matt Pryor
 Author-email: matt@stackhpc.com
 Description-Content-Type: text/markdown
 Requires-Dist: pydantic
 Requires-Dist: pyyaml
```

