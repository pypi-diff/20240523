# Comparing `tmp/seamm_dashboard_client-2024.4.22.tar.gz` & `tmp/seamm_dashboard_client-2024.5.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seamm_dashboard_client-2024.4.22.tar", last modified: Mon Apr 22 21:29:57 2024, max compression
+gzip compressed data, was "seamm_dashboard_client-2024.5.23.tar", last modified: Thu May 23 21:20:23 2024, max compression
```

## Comparing `seamm_dashboard_client-2024.4.22.tar` & `seamm_dashboard_client-2024.5.23.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 21:29:57.397261 seamm_dashboard_client-2024.4.22/
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-22 21:29:49.000000 seamm_dashboard_client-2024.4.22/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-04-22 21:29:49.000000 seamm_dashboard_client-2024.4.22/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)      990 2024-04-22 21:29:49.000000 seamm_dashboard_client-2024.4.22/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-04-22 21:29:49.000000 seamm_dashboard_client-2024.4.22/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-22 21:29:49.000000 seamm_dashboard_client-2024.4.22/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4133 2024-04-22 21:29:57.397261 seamm_dashboard_client-2024.4.22/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-04-22 21:29:49.000000 seamm_dashboard_client-2024.4.22/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 21:29:57.393261 seamm_dashboard_client-2024.4.22/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     6826 2024-04-22 21:29:49.000000 seamm_dashboard_client-2024.4.22/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-22 21:29:49.000000 seamm_dashboard_client-2024.4.22/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (127)     8842 2024-04-22 21:29:49.000000 seamm_dashboard_client-2024.4.22/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 21:29:57.393261 seamm_dashboard_client-2024.4.22/docs/developer/
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-22 21:29:49.000000 seamm_dashboard_client-2024.4.22/docs/developer/cms_plots.rst
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-22 21:29:49.000000 seamm_dashboard_client-2024.4.22/docs/developer/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-22 21:29:49.000000 seamm_dashboard_client-2024.4.22/docs/developer/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-22 21:29:49.000000 seamm_dashboard_client-2024.4.22/docs/developer/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-22 21:29:49.000000 seamm_dashboard_client-2024.4.22/docs/developer/readme.rst
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-22 21:29:49.000000 seamm_dashboard_client-2024.4.22/docs/developer/usage.rst
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-22 21:29:49.000000 seamm_dashboard_client-2024.4.22/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-22 21:29:49.000000 seamm_dashboard_client-2024.4.22/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6491 2024-04-22 21:29:49.000000 seamm_dashboard_client-2024.4.22/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 21:29:57.397261 seamm_dashboard_client-2024.4.22/docs/user/
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-22 21:29:49.000000 seamm_dashboard_client-2024.4.22/docs/user/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-22 21:29:49.000000 seamm_dashboard_client-2024.4.22/docs/user/overview.rst
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-22 21:29:49.000000 seamm_dashboard_client-2024.4.22/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-22 21:29:49.000000 seamm_dashboard_client-2024.4.22/requirements_dev.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 21:29:57.397261 seamm_dashboard_client-2024.4.22/seamm_dashboard_client/
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-22 21:29:49.000000 seamm_dashboard_client-2024.4.22/seamm_dashboard_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-22 21:29:57.397261 seamm_dashboard_client-2024.4.22/seamm_dashboard_client/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    29490 2024-04-22 21:29:49.000000 seamm_dashboard_client-2024.4.22/seamm_dashboard_client/dashboard.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 21:29:57.397261 seamm_dashboard_client-2024.4.22/seamm_dashboard_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4133 2024-04-22 21:29:57.000000 seamm_dashboard_client-2024.4.22/seamm_dashboard_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-22 21:29:57.000000 seamm_dashboard_client-2024.4.22/seamm_dashboard_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 21:29:57.000000 seamm_dashboard_client-2024.4.22/seamm_dashboard_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-22 21:29:57.000000 seamm_dashboard_client-2024.4.22/seamm_dashboard_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-22 21:29:57.000000 seamm_dashboard_client-2024.4.22/seamm_dashboard_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 21:29:52.000000 seamm_dashboard_client-2024.4.22/seamm_dashboard_client.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-22 21:29:57.397261 seamm_dashboard_client-2024.4.22/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-04-22 21:29:49.000000 seamm_dashboard_client-2024.4.22/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 21:29:57.397261 seamm_dashboard_client-2024.4.22/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-22 21:29:49.000000 seamm_dashboard_client-2024.4.22/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31497 2024-04-22 21:29:49.000000 seamm_dashboard_client-2024.4.22/tests/test_dashboard.py
--rw-r--r--   0 runner    (1001) docker     (127)    68610 2024-04-22 21:29:49.000000 seamm_dashboard_client-2024.4.22/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:20:23.646847 seamm_dashboard_client-2024.5.23/
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-23 21:20:15.000000 seamm_dashboard_client-2024.5.23/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-05-23 21:20:15.000000 seamm_dashboard_client-2024.5.23/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-23 21:20:15.000000 seamm_dashboard_client-2024.5.23/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-05-23 21:20:15.000000 seamm_dashboard_client-2024.5.23/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-23 21:20:15.000000 seamm_dashboard_client-2024.5.23/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4390 2024-05-23 21:20:23.646847 seamm_dashboard_client-2024.5.23/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-05-23 21:20:15.000000 seamm_dashboard_client-2024.5.23/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:20:23.642847 seamm_dashboard_client-2024.5.23/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     6826 2024-05-23 21:20:15.000000 seamm_dashboard_client-2024.5.23/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-23 21:20:15.000000 seamm_dashboard_client-2024.5.23/docs/authors.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8842 2024-05-23 21:20:15.000000 seamm_dashboard_client-2024.5.23/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:20:23.642847 seamm_dashboard_client-2024.5.23/docs/developer/
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-23 21:20:15.000000 seamm_dashboard_client-2024.5.23/docs/developer/cms_plots.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-23 21:20:15.000000 seamm_dashboard_client-2024.5.23/docs/developer/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-23 21:20:15.000000 seamm_dashboard_client-2024.5.23/docs/developer/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-23 21:20:15.000000 seamm_dashboard_client-2024.5.23/docs/developer/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-23 21:20:15.000000 seamm_dashboard_client-2024.5.23/docs/developer/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-23 21:20:15.000000 seamm_dashboard_client-2024.5.23/docs/developer/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-23 21:20:15.000000 seamm_dashboard_client-2024.5.23/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-23 21:20:15.000000 seamm_dashboard_client-2024.5.23/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6491 2024-05-23 21:20:15.000000 seamm_dashboard_client-2024.5.23/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:20:23.642847 seamm_dashboard_client-2024.5.23/docs/user/
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-23 21:20:15.000000 seamm_dashboard_client-2024.5.23/docs/user/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-23 21:20:15.000000 seamm_dashboard_client-2024.5.23/docs/user/overview.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-23 21:20:15.000000 seamm_dashboard_client-2024.5.23/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-23 21:20:15.000000 seamm_dashboard_client-2024.5.23/requirements_dev.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:20:23.646847 seamm_dashboard_client-2024.5.23/seamm_dashboard_client/
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-23 21:20:15.000000 seamm_dashboard_client-2024.5.23/seamm_dashboard_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-23 21:20:23.646847 seamm_dashboard_client-2024.5.23/seamm_dashboard_client/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29513 2024-05-23 21:20:15.000000 seamm_dashboard_client-2024.5.23/seamm_dashboard_client/dashboard.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:20:23.646847 seamm_dashboard_client-2024.5.23/seamm_dashboard_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4390 2024-05-23 21:20:23.000000 seamm_dashboard_client-2024.5.23/seamm_dashboard_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-05-23 21:20:23.000000 seamm_dashboard_client-2024.5.23/seamm_dashboard_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 21:20:23.000000 seamm_dashboard_client-2024.5.23/seamm_dashboard_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-23 21:20:23.000000 seamm_dashboard_client-2024.5.23/seamm_dashboard_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-23 21:20:23.000000 seamm_dashboard_client-2024.5.23/seamm_dashboard_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 21:20:18.000000 seamm_dashboard_client-2024.5.23/seamm_dashboard_client.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-23 21:20:23.646847 seamm_dashboard_client-2024.5.23/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-05-23 21:20:15.000000 seamm_dashboard_client-2024.5.23/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 21:20:23.642847 seamm_dashboard_client-2024.5.23/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-23 21:20:15.000000 seamm_dashboard_client-2024.5.23/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31497 2024-05-23 21:20:15.000000 seamm_dashboard_client-2024.5.23/tests/test_dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68610 2024-05-23 21:20:15.000000 seamm_dashboard_client-2024.5.23/versioneer.py
```

### Comparing `seamm_dashboard_client-2024.4.22/CONTRIBUTING.rst` & `seamm_dashboard_client-2024.5.23/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `seamm_dashboard_client-2024.4.22/HISTORY.rst` & `seamm_dashboard_client-2024.5.23/HISTORY.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 =======
 History
 =======
+2024.5.23 -- Bugfix: crash opening a flowchart from a Dashboard
+   * SEAMM could crash when asking the Flowchart Open dialog to get the flowchart from a
+     previous job. This only happened if the Dashboard was known but the stored password
+     was wrong.
+
 2024.4.22 -- Moving user preferences to ~/.seamm.d
-    * Added better output when there are failures in the Dashboard.
-    * To better support Docker, moving ~/.seammrc to ~/.seamm.d/seamrc
+   * Added better output when there are failures in the Dashboard.
+   * To better support Docker, moving ~/.seammrc to ~/.seamm.d/seamrc
 
 2023.11.15 -- Bugfix: boolean options now work
    * Boolean options were not handled correctly when submitting jobs.
 
 2023.10.24 -- Improvement for job handling.
    * Added control parameters to the data stored for the job, to support filling out
      menus identical to how the job was submitted.
```

### Comparing `seamm_dashboard_client-2024.4.22/LICENSE` & `seamm_dashboard_client-2024.5.23/LICENSE`

 * *Files identical despite different names*

### Comparing `seamm_dashboard_client-2024.4.22/PKG-INFO` & `seamm_dashboard_client-2024.5.23/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seamm_dashboard_client
-Version: 2024.4.22
+Version: 2024.5.23
 Summary: A Python client for the SEAMM Dashboard RESTful API.
 Home-page: https://github.com/molssi-seamm/seamm_dashboard_client
 Author: Paul Saxe
 Author-email: psaxe@molssi.org
 License: BSD-3-Clause
 Keywords: SEAMM,SEAMMDashboard,RESTful,client
 Platform: Linux
@@ -87,17 +87,22 @@
 .. _`molssi-seamm/cookiecutter-seamm-plugin`: https://github.com/molssi-seamm/cookiecutter-seamm-plugin
 .. _MolSSI: https://molssi.org
 
 
 =======
 History
 =======
+2024.5.23 -- Bugfix: crash opening a flowchart from a Dashboard
+   * SEAMM could crash when asking the Flowchart Open dialog to get the flowchart from a
+     previous job. This only happened if the Dashboard was known but the stored password
+     was wrong.
+
 2024.4.22 -- Moving user preferences to ~/.seamm.d
-    * Added better output when there are failures in the Dashboard.
-    * To better support Docker, moving ~/.seammrc to ~/.seamm.d/seamrc
+   * Added better output when there are failures in the Dashboard.
+   * To better support Docker, moving ~/.seammrc to ~/.seamm.d/seamrc
 
 2023.11.15 -- Bugfix: boolean options now work
    * Boolean options were not handled correctly when submitting jobs.
 
 2023.10.24 -- Improvement for job handling.
    * Added control parameters to the data stored for the job, to support filling out
      menus identical to how the job was submitted.
```

### Comparing `seamm_dashboard_client-2024.4.22/README.rst` & `seamm_dashboard_client-2024.5.23/README.rst`

 * *Files identical despite different names*

### Comparing `seamm_dashboard_client-2024.4.22/docs/Makefile` & `seamm_dashboard_client-2024.5.23/docs/Makefile`

 * *Files identical despite different names*

### Comparing `seamm_dashboard_client-2024.4.22/docs/conf.py` & `seamm_dashboard_client-2024.5.23/docs/conf.py`

 * *Files identical despite different names*

### Comparing `seamm_dashboard_client-2024.4.22/docs/developer/cms_plots.rst` & `seamm_dashboard_client-2024.5.23/docs/developer/cms_plots.rst`

 * *Files identical despite different names*

### Comparing `seamm_dashboard_client-2024.4.22/docs/developer/installation.rst` & `seamm_dashboard_client-2024.5.23/docs/developer/installation.rst`

 * *Files identical despite different names*

### Comparing `seamm_dashboard_client-2024.4.22/docs/index.rst` & `seamm_dashboard_client-2024.5.23/docs/index.rst`

 * *Files identical despite different names*

### Comparing `seamm_dashboard_client-2024.4.22/docs/make.bat` & `seamm_dashboard_client-2024.5.23/docs/make.bat`

 * *Files identical despite different names*

### Comparing `seamm_dashboard_client-2024.4.22/seamm_dashboard_client/__init__.py` & `seamm_dashboard_client-2024.5.23/seamm_dashboard_client/__init__.py`

 * *Files identical despite different names*

### Comparing `seamm_dashboard_client-2024.4.22/seamm_dashboard_client/dashboard.py` & `seamm_dashboard_client-2024.5.23/seamm_dashboard_client/dashboard.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import shlex
 
 import requests
 from requests_toolbelt.multipart.encoder import MultipartEncoder
 
 logger = logging.getLogger(__name__)
 
-logger.setLevel("DEBUG")
+# logger.setLevel("DEBUG")
 
 
 def safe_filename(filename):
     if filename[0] == "~":
         path = Path(filename).expanduser()
     else:
         path = Path(filename)
@@ -400,15 +400,15 @@
             "down"
             "error"
         """
         try:
             response = self._url_get("/api/status")
         except DashboardTimeoutError:
             return "down"
-        except (DashboardConnectionError, DashboardUnknownError):
+        except (DashboardConnectionError, DashboardUnknownError, DashboardLoginError):
             return "error"
 
         if response.status_code != 200:
             logger.info(
                 "Encountered an error getting the status from dashboard "
                 f"{self.name}, error code: {response.status_code}"
             )
```

### Comparing `seamm_dashboard_client-2024.4.22/seamm_dashboard_client.egg-info/PKG-INFO` & `seamm_dashboard_client-2024.5.23/seamm_dashboard_client.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seamm_dashboard_client
-Version: 2024.4.22
+Version: 2024.5.23
 Summary: A Python client for the SEAMM Dashboard RESTful API.
 Home-page: https://github.com/molssi-seamm/seamm_dashboard_client
 Author: Paul Saxe
 Author-email: psaxe@molssi.org
 License: BSD-3-Clause
 Keywords: SEAMM,SEAMMDashboard,RESTful,client
 Platform: Linux
@@ -87,17 +87,22 @@
 .. _`molssi-seamm/cookiecutter-seamm-plugin`: https://github.com/molssi-seamm/cookiecutter-seamm-plugin
 .. _MolSSI: https://molssi.org
 
 
 =======
 History
 =======
+2024.5.23 -- Bugfix: crash opening a flowchart from a Dashboard
+   * SEAMM could crash when asking the Flowchart Open dialog to get the flowchart from a
+     previous job. This only happened if the Dashboard was known but the stored password
+     was wrong.
+
 2024.4.22 -- Moving user preferences to ~/.seamm.d
-    * Added better output when there are failures in the Dashboard.
-    * To better support Docker, moving ~/.seammrc to ~/.seamm.d/seamrc
+   * Added better output when there are failures in the Dashboard.
+   * To better support Docker, moving ~/.seammrc to ~/.seamm.d/seamrc
 
 2023.11.15 -- Bugfix: boolean options now work
    * Boolean options were not handled correctly when submitting jobs.
 
 2023.10.24 -- Improvement for job handling.
    * Added control parameters to the data stored for the job, to support filling out
      menus identical to how the job was submitted.
```

### Comparing `seamm_dashboard_client-2024.4.22/seamm_dashboard_client.egg-info/SOURCES.txt` & `seamm_dashboard_client-2024.5.23/seamm_dashboard_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `seamm_dashboard_client-2024.4.22/setup.py` & `seamm_dashboard_client-2024.5.23/setup.py`

 * *Files identical despite different names*

### Comparing `seamm_dashboard_client-2024.4.22/tests/test_dashboard.py` & `seamm_dashboard_client-2024.5.23/tests/test_dashboard.py`

 * *Files identical despite different names*

### Comparing `seamm_dashboard_client-2024.4.22/versioneer.py` & `seamm_dashboard_client-2024.5.23/versioneer.py`

 * *Files identical despite different names*

