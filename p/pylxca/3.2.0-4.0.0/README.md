# Comparing `tmp/pylxca-3.2.0.tar.gz` & `tmp/pylxca-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pylxca-3.2.0.tar", last modified: Fri Mar 26 05:35:14 2021, max compression
+gzip compressed data, was "pylxca-4.0.0.tar", last modified: Thu May 23 14:21:17 2024, max compression
```

## Comparing `pylxca-3.2.0.tar` & `pylxca-4.0.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0 prashant  (1000) prashant  (1000)        0 2021-03-26 05:35:14.838184 pylxca-3.2.0/
--rw-rw-rw-   0 prashant  (1000) prashant  (1000)    11357 2021-03-26 05:07:34.000000 pylxca-3.2.0/LICENSE
--rwxrwxrwx   0 prashant  (1000) prashant  (1000)      198 2021-03-26 05:07:34.000000 pylxca-3.2.0/MANIFEST.in
--rw-rw-rw-   0 prashant  (1000) prashant  (1000)     5151 2021-03-26 05:35:14.836216 pylxca-3.2.0/PKG-INFO
--rw-rw-rw-   0 prashant  (1000) prashant  (1000)     3779 2021-03-26 05:07:34.000000 pylxca-3.2.0/README
--rwxrwxrwx   0 prashant  (1000) prashant  (1000)     1535 2021-03-26 05:19:10.000000 pylxca-3.2.0/lxca_shell
-drwxrwxrwx   0 prashant  (1000) prashant  (1000)        0 2021-03-26 05:35:14.779622 pylxca-3.2.0/pylxca/
--rw-rw-rw-   0 prashant  (1000) prashant  (1000)      723 2021-03-26 05:17:21.000000 pylxca-3.2.0/pylxca/__init__.py
-drwxrwxrwx   0 prashant  (1000) prashant  (1000)        0 2021-03-26 05:35:14.806696 pylxca-3.2.0/pylxca/pylxca_api/
--rw-rw-rw-   0 prashant  (1000) prashant  (1000)      356 2021-03-26 05:07:34.000000 pylxca-3.2.0/pylxca/pylxca_api/__init__.py
--rw-rw-rw-   0 prashant  (1000) prashant  (1000)    52243 2021-03-26 05:07:34.000000 pylxca-3.2.0/pylxca/pylxca_api/lxca_api.py
--rw-rw-rw-   0 prashant  (1000) prashant  (1000)     5612 2021-03-26 05:07:34.000000 pylxca-3.2.0/pylxca/pylxca_api/lxca_connection.py
--rw-rw-rw-   0 prashant  (1000) prashant  (1000)     1241 2021-03-26 05:07:34.000000 pylxca-3.2.0/pylxca/pylxca_api/lxca_logger.conf
--rw-rw-rw-   0 prashant  (1000) prashant  (1000)    74395 2021-03-26 05:07:34.000000 pylxca-3.2.0/pylxca/pylxca_api/lxca_rest.py
-drwxrwxrwx   0 prashant  (1000) prashant  (1000)        0 2021-03-26 05:35:14.830722 pylxca-3.2.0/pylxca/pylxca_cmd/
--rw-rw-rw-   0 prashant  (1000) prashant  (1000)      476 2021-03-26 05:07:34.000000 pylxca-3.2.0/pylxca/pylxca_cmd/__init__.py
--rw-rw-rw-   0 prashant  (1000) prashant  (1000)    33465 2021-03-26 05:07:34.000000 pylxca-3.2.0/pylxca/pylxca_cmd/lxca_cmd.py
--rw-rw-rw-   0 prashant  (1000) prashant  (1000)    70216 2021-03-26 05:07:34.000000 pylxca-3.2.0/pylxca/pylxca_cmd/lxca_cmd_data.json
--rw-rw-rw-   0 prashant  (1000) prashant  (1000)    26641 2021-03-26 05:07:34.000000 pylxca-3.2.0/pylxca/pylxca_cmd/lxca_filters.xml
--rw-rw-rw-   0 prashant  (1000) prashant  (1000)    10741 2021-03-26 05:07:34.000000 pylxca-3.2.0/pylxca/pylxca_cmd/lxca_icommands.py
--rw-rw-rw-   0 prashant  (1000) prashant  (1000)    12416 2021-03-26 05:07:34.000000 pylxca-3.2.0/pylxca/pylxca_cmd/lxca_ishell.py
--rw-rw-rw-   0 prashant  (1000) prashant  (1000)    69951 2021-03-26 05:07:34.000000 pylxca-3.2.0/pylxca/pylxca_cmd/lxca_pyshell.py
--rw-rw-rw-   0 prashant  (1000) prashant  (1000)     4815 2021-03-26 05:07:34.000000 pylxca-3.2.0/pylxca/pylxca_cmd/lxca_view.py
-drwxrwxrwx   0 prashant  (1000) prashant  (1000)        0 2021-03-26 05:35:14.832713 pylxca-3.2.0/pylxca/test/
--rwxrwxrwx   0 prashant  (1000) prashant  (1000)     8569 2021-03-26 05:07:34.000000 pylxca-3.2.0/pylxca/test/pylxca_unittest
-drwxrwxrwx   0 prashant  (1000) prashant  (1000)        0 2021-03-26 05:35:14.794108 pylxca-3.2.0/pylxca.egg-info/
--rw-rw-rw-   0 prashant  (1000) prashant  (1000)     5151 2021-03-26 05:35:14.000000 pylxca-3.2.0/pylxca.egg-info/PKG-INFO
--rw-rw-rw-   0 prashant  (1000) prashant  (1000)      671 2021-03-26 05:35:14.000000 pylxca-3.2.0/pylxca.egg-info/SOURCES.txt
--rw-rw-rw-   0 prashant  (1000) prashant  (1000)        1 2021-03-26 05:35:14.000000 pylxca-3.2.0/pylxca.egg-info/dependency_links.txt
--rw-rw-rw-   0 prashant  (1000) prashant  (1000)       51 2021-03-26 05:35:14.000000 pylxca-3.2.0/pylxca.egg-info/requires.txt
--rw-rw-rw-   0 prashant  (1000) prashant  (1000)        7 2021-03-26 05:35:14.000000 pylxca-3.2.0/pylxca.egg-info/top_level.txt
--rw-rw-rw-   0 prashant  (1000) prashant  (1000)       38 2021-03-26 05:35:14.839176 pylxca-3.2.0/setup.cfg
--rwxrwxrwx   0 prashant  (1000) prashant  (1000)     2896 2021-03-26 05:07:34.000000 pylxca-3.2.0/setup.py
+drwxr-xr-x   0 prashant  (1000) prashant  (1000)        0 2024-05-23 14:21:17.979568 pylxca-4.0.0/
+-rw-r--r--   0 prashant  (1000) prashant  (1000)    11357 2021-03-26 06:08:01.000000 pylxca-4.0.0/LICENSE
+-rwxr-xr-x   0 prashant  (1000) prashant  (1000)      198 2024-04-18 09:42:18.000000 pylxca-4.0.0/MANIFEST.in
+-rw-r--r--   0 prashant  (1000) prashant  (1000)     4440 2024-05-23 14:21:17.979568 pylxca-4.0.0/PKG-INFO
+-rw-r--r--   0 prashant  (1000) prashant  (1000)     3965 2021-03-26 06:14:03.000000 pylxca-4.0.0/README
+-rwxr-xr-x   0 prashant  (1000) prashant  (1000)     1559 2024-05-23 13:40:39.000000 pylxca-4.0.0/lxca_shell
+drwxr-xr-x   0 prashant  (1000) prashant  (1000)        0 2024-05-23 14:21:17.979568 pylxca-4.0.0/pylxca/
+-rw-r--r--   0 prashant  (1000) prashant  (1000)      723 2024-05-23 14:21:01.000000 pylxca-4.0.0/pylxca/__init__.py
+drwxr-xr-x   0 prashant  (1000) prashant  (1000)        0 2024-05-23 14:21:17.979568 pylxca-4.0.0/pylxca/pylxca_api/
+-rw-r--r--   0 prashant  (1000) prashant  (1000)      356 2021-03-26 05:07:34.000000 pylxca-4.0.0/pylxca/pylxca_api/__init__.py
+-rw-r--r--   0 prashant  (1000) prashant  (1000)    52243 2021-03-26 06:08:01.000000 pylxca-4.0.0/pylxca/pylxca_api/lxca_api.py
+-rw-r--r--   0 prashant  (1000) prashant  (1000)     5612 2021-03-26 06:08:01.000000 pylxca-4.0.0/pylxca/pylxca_api/lxca_connection.py
+-rw-r--r--   0 prashant  (1000) prashant  (1000)     1241 2021-03-26 05:07:34.000000 pylxca-4.0.0/pylxca/pylxca_api/lxca_logger.conf
+-rw-r--r--   0 prashant  (1000) prashant  (1000)    74395 2021-03-26 06:08:01.000000 pylxca-4.0.0/pylxca/pylxca_api/lxca_rest.py
+drwxr-xr-x   0 prashant  (1000) prashant  (1000)        0 2024-05-23 14:21:17.979568 pylxca-4.0.0/pylxca/pylxca_cmd/
+-rw-r--r--   0 prashant  (1000) prashant  (1000)      476 2021-03-26 05:07:34.000000 pylxca-4.0.0/pylxca/pylxca_cmd/__init__.py
+-rw-r--r--   0 prashant  (1000) prashant  (1000)    33465 2021-03-26 06:08:01.000000 pylxca-4.0.0/pylxca/pylxca_cmd/lxca_cmd.py
+-rw-r--r--   0 prashant  (1000) prashant  (1000)    70216 2021-03-26 06:08:01.000000 pylxca-4.0.0/pylxca/pylxca_cmd/lxca_cmd_data.json
+-rw-r--r--   0 prashant  (1000) prashant  (1000)    26641 2021-03-26 06:08:01.000000 pylxca-4.0.0/pylxca/pylxca_cmd/lxca_filters.xml
+-rw-r--r--   0 prashant  (1000) prashant  (1000)    10741 2021-03-26 06:08:02.000000 pylxca-4.0.0/pylxca/pylxca_cmd/lxca_icommands.py
+-rw-r--r--   0 prashant  (1000) prashant  (1000)    12416 2021-03-26 06:08:02.000000 pylxca-4.0.0/pylxca/pylxca_cmd/lxca_ishell.py
+-rw-r--r--   0 prashant  (1000) prashant  (1000)    69951 2021-03-26 06:08:02.000000 pylxca-4.0.0/pylxca/pylxca_cmd/lxca_pyshell.py
+-rw-r--r--   0 prashant  (1000) prashant  (1000)     4794 2024-05-23 13:47:47.000000 pylxca-4.0.0/pylxca/pylxca_cmd/lxca_view.py
+drwxr-xr-x   0 prashant  (1000) prashant  (1000)        0 2024-05-23 14:21:17.979568 pylxca-4.0.0/pylxca/test/
+-rwxr-xr-x   0 prashant  (1000) prashant  (1000)     8557 2024-04-18 09:42:25.000000 pylxca-4.0.0/pylxca/test/pylxca_unittest
+drwxr-xr-x   0 prashant  (1000) prashant  (1000)        0 2024-05-23 14:21:17.979568 pylxca-4.0.0/pylxca.egg-info/
+-rw-r--r--   0 prashant  (1000) prashant  (1000)     4440 2024-05-23 14:21:17.000000 pylxca-4.0.0/pylxca.egg-info/PKG-INFO
+-rw-r--r--   0 prashant  (1000) prashant  (1000)      671 2024-05-23 14:21:17.000000 pylxca-4.0.0/pylxca.egg-info/SOURCES.txt
+-rw-r--r--   0 prashant  (1000) prashant  (1000)        1 2024-05-23 14:21:17.000000 pylxca-4.0.0/pylxca.egg-info/dependency_links.txt
+-rw-r--r--   0 prashant  (1000) prashant  (1000)       51 2024-05-23 14:21:17.000000 pylxca-4.0.0/pylxca.egg-info/requires.txt
+-rw-r--r--   0 prashant  (1000) prashant  (1000)        7 2024-05-23 14:21:17.000000 pylxca-4.0.0/pylxca.egg-info/top_level.txt
+-rw-r--r--   0 prashant  (1000) prashant  (1000)       38 2024-05-23 14:21:17.979568 pylxca-4.0.0/setup.cfg
+-rwxr-xr-x   0 prashant  (1000) prashant  (1000)     2896 2024-04-18 09:42:18.000000 pylxca-4.0.0/setup.py
```

### Comparing `pylxca-3.2.0/LICENSE` & `pylxca-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pylxca-3.2.0/README` & `pylxca-4.0.0/README`

 * *Files 8% similar despite different names*

```diff
@@ -14,14 +14,21 @@
 *	Managing and unmanaging chassis, servers, storage systems, and 
 top-of-rack switches (endpoints)
 *	Viewing inventory data for endpoints and components
 *	Deploying an operating-system image to one or more servers
 *	Configuring servers through the use of Configuration Patterns
 *	Applying firmware updates to endpoints
 
+Whats New in 3.2.0
+------------------
+* 	License Compliance
+*   Manage/Unmanage Support for Edge Servers
+*   Support for firmware update for AMD-1S
+*   Bug Fixes and Minor improvements
+
 Whats New in 2.4.0
 ------------------
 * 	Argument Parsing library replaced from optparse to argparse.
 *	Support for subcmd under various commands.
 *	New commands supported under shell
 		osimages
 		managementserver
```

### Comparing `pylxca-3.2.0/lxca_shell` & `pylxca-4.0.0/lxca_shell`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+#!/user/bin/env python3
 '''
 @since: 15 Sep 2015
 @author: Prashant Bhosale <pbhosale@lenovo.com>, Girish Kumar <gkumar1@lenovo.com>
 @license: Lenovo License
 @copyright: Lenovo Copyright
 @organization: Lenovo Group Ltd
 @summary: The main script for PYLXCA Tool, It creates a shell and accept raw input to process it.
```

### Comparing `pylxca-3.2.0/pylxca/__init__.py` & `pylxca-4.0.0/pylxca/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Version of the pylxca package
 
-__version__ = '3.2.0'
+__version__ = '4.0.0'
 
 
 # There are submodules, but clients shouldn't need to know about them.
 # Importing just this module is enough.
 
 # These are explicitly safe for 'import *'
 from pylxca.pylxca_api import *
```

### Comparing `pylxca-3.2.0/pylxca/pylxca_api/lxca_api.py` & `pylxca-4.0.0/pylxca/pylxca_api/lxca_api.py`

 * *Files identical despite different names*

### Comparing `pylxca-3.2.0/pylxca/pylxca_api/lxca_connection.py` & `pylxca-4.0.0/pylxca/pylxca_api/lxca_connection.py`

 * *Files identical despite different names*

### Comparing `pylxca-3.2.0/pylxca/pylxca_api/lxca_logger.conf` & `pylxca-4.0.0/pylxca/pylxca_api/lxca_logger.conf`

 * *Files identical despite different names*

### Comparing `pylxca-3.2.0/pylxca/pylxca_api/lxca_rest.py` & `pylxca-4.0.0/pylxca/pylxca_api/lxca_rest.py`

 * *Files identical despite different names*

### Comparing `pylxca-3.2.0/pylxca/pylxca_cmd/lxca_cmd.py` & `pylxca-4.0.0/pylxca/pylxca_cmd/lxca_cmd.py`

 * *Files identical despite different names*

### Comparing `pylxca-3.2.0/pylxca/pylxca_cmd/lxca_cmd_data.json` & `pylxca-4.0.0/pylxca/pylxca_cmd/lxca_cmd_data.json`

 * *Files identical despite different names*

### Comparing `pylxca-3.2.0/pylxca/pylxca_cmd/lxca_filters.xml` & `pylxca-4.0.0/pylxca/pylxca_cmd/lxca_filters.xml`

 * *Files identical despite different names*

### Comparing `pylxca-3.2.0/pylxca/pylxca_cmd/lxca_icommands.py` & `pylxca-4.0.0/pylxca/pylxca_cmd/lxca_icommands.py`

 * *Files identical despite different names*

### Comparing `pylxca-3.2.0/pylxca/pylxca_cmd/lxca_ishell.py` & `pylxca-4.0.0/pylxca/pylxca_cmd/lxca_ishell.py`

 * *Files identical despite different names*

### Comparing `pylxca-3.2.0/pylxca/pylxca_cmd/lxca_pyshell.py` & `pylxca-4.0.0/pylxca/pylxca_cmd/lxca_pyshell.py`

 * *Files identical despite different names*

### Comparing `pylxca-3.2.0/pylxca/pylxca_cmd/lxca_view.py` & `pylxca-4.0.0/pylxca/pylxca_cmd/lxca_view.py`

 * *Files 3% similar despite different names*

```diff
@@ -110,23 +110,23 @@
 
         indent += 4
         # View Filter has children so
         py_obj_item = self.get_val(py_obj, view_filter.attrib.get('name', view_filter.text))
         #if py_obj_item is list then iterate through the list and call print recur for each
         if isinstance(py_obj_item, (list)):
             for item in py_obj_item:
-                for elem in view_filter.getchildren():
+                for elem in view_filter.iter():
                     self.print_recur(item,elem)
         else:
-            for elem in view_filter.getchildren():
+            for elem in view_filter.iter():
                 self.print_recur(py_obj_item,elem)
         indent -= 4
 
     def print_cmd_resp_object(self,cmd_resp_item, vf):
-        for vf_elem in vf.getchildren():
+        for vf_elem in vf.iter():
             self.print_recur(cmd_resp_item,vf_elem)
 
 
     def show_output(self,cmd_reponse, cmd_name,filter_tag):
         vf = self.get_view_filter(cmd_name,filter_tag)
         self.ostream.write("Printing "+ cmd_name + " Output:"+ "\n")
```

### Comparing `pylxca-3.2.0/pylxca/test/pylxca_unittest` & `pylxca-4.0.0/pylxca/test/pylxca_unittest`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/usr/bin/env /usr/bin/python2.7
+#!/usr/bin/env python
 import time
 import os
 import sys
 import argparse
 import unittest
 import string
 import random
```

### Comparing `pylxca-3.2.0/pylxca.egg-info/SOURCES.txt` & `pylxca-4.0.0/pylxca.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pylxca-3.2.0/setup.py` & `pylxca-4.0.0/setup.py`

 * *Files identical despite different names*

