# Comparing `tmp/scipion-app-3.3.1.tar.gz` & `tmp/scipion_app-3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scipion-app-3.3.1.tar", last modified: Fri Mar 15 12:54:50 2024, max compression
+gzip compressed data, was "scipion_app-3.4.0.tar", last modified: Thu May 23 07:50:54 2024, max compression
```

## Comparing `scipion-app-3.3.1.tar` & `scipion_app-3.4.0.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 12:54:50.159552 scipion-app-3.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)     2539 2024-03-15 12:54:42.000000 scipion-app-3.3.1/CHANGES.txt
--rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-03-15 12:54:42.000000 scipion-app-3.3.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-15 12:54:42.000000 scipion-app-3.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-03-15 12:54:50.159552 scipion-app-3.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-03-15 12:54:42.000000 scipion-app-3.3.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-03-15 12:54:42.000000 scipion-app-3.3.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 12:54:50.151552 scipion-app-3.3.1/scipion/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-15 12:54:42.000000 scipion-app-3.3.1/scipion/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    18855 2024-03-15 12:54:42.000000 scipion-app-3.3.1/scipion/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-03-15 12:54:42.000000 scipion-app-3.3.1/scipion/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-03-15 12:54:42.000000 scipion-app-3.3.1/scipion/guiplugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 12:54:50.155552 scipion-app-3.3.1/scipion/install/
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-03-15 12:54:42.000000 scipion-app-3.3.1/scipion/install/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3224 2024-03-15 12:54:42.000000 scipion-app-3.3.1/scipion/install/change_rpath.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      883 2024-03-15 12:54:42.000000 scipion-app-3.3.1/scipion/install/clean.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4144 2024-03-15 12:54:42.000000 scipion-app-3.3.1/scipion/install/find_deps.py
--rw-r--r--   0 runner    (1001) docker     (127)    60216 2024-03-15 12:54:42.000000 scipion-app-3.3.1/scipion/install/funcs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6810 2024-03-15 12:54:42.000000 scipion-app-3.3.1/scipion/install/inspect_plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)    15717 2024-03-15 12:54:42.000000 scipion-app-3.3.1/scipion/install/install_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)    20229 2024-03-15 12:54:42.000000 scipion-app-3.3.1/scipion/install/plugin_funcs.py
--rw-r--r--   0 runner    (1001) docker     (127)    50543 2024-03-15 12:54:42.000000 scipion-app-3.3.1/scipion/install/plugin_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     6089 2024-03-15 12:54:42.000000 scipion-app-3.3.1/scipion/install/update_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 12:54:50.155552 scipion-app-3.3.1/scipion/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 12:54:42.000000 scipion-app-3.3.1/scipion/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18200 2024-03-15 12:54:42.000000 scipion-app-3.3.1/scipion/scripts/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7415 2024-03-15 12:54:42.000000 scipion-app-3.3.1/scipion/scripts/fontbrowser.py
--rw-r--r--   0 runner    (1001) docker     (127)    19076 2024-03-15 12:54:42.000000 scipion-app-3.3.1/scipion/scripts/kickoff.py
--rw-r--r--   0 runner    (1001) docker     (127)     4103 2024-03-15 12:54:42.000000 scipion-app-3.3.1/scipion/scripts/tutorial.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 12:54:50.155552 scipion-app-3.3.1/scipion/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-03-15 12:54:42.000000 scipion-app-3.3.1/scipion/templates/hosts.template
--rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-03-15 12:54:42.000000 scipion-app-3.3.1/scipion/templates/protocols.template
--rw-r--r--   0 runner    (1001) docker     (127)     4292 2024-03-15 12:54:42.000000 scipion-app-3.3.1/scipion/templates/scipion.template
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-03-15 12:54:42.000000 scipion-app-3.3.1/scipion/templates/scipionbox.template
--rw-r--r--   0 runner    (1001) docker     (127)     4197 2024-03-15 12:54:42.000000 scipion-app-3.3.1/scipion/templates/workflow_betagal1.json
--rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-03-15 12:54:42.000000 scipion-app-3.3.1/scipion/templates/workflow_betagal2.json
--rw-r--r--   0 runner    (1001) docker     (127)     8100 2024-03-15 12:54:42.000000 scipion-app-3.3.1/scipion/templates/workflow_tutorial_intro.json
--rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-03-15 12:54:42.000000 scipion-app-3.3.1/scipion/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 12:54:50.159552 scipion-app-3.3.1/scipion_app.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-03-15 12:54:50.000000 scipion-app-3.3.1/scipion_app.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-03-15 12:54:50.000000 scipion-app-3.3.1/scipion_app.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-15 12:54:50.000000 scipion-app-3.3.1/scipion_app.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-03-15 12:54:50.000000 scipion-app-3.3.1/scipion_app.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-03-15 12:54:50.000000 scipion-app-3.3.1/scipion_app.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-03-15 12:54:50.000000 scipion-app-3.3.1/scipion_app.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-15 12:54:50.159552 scipion-app-3.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-03-15 12:54:42.000000 scipion-app-3.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:50:54.445764 scipion_app-3.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-05-23 07:50:44.000000 scipion_app-3.4.0/CHANGES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-05-23 07:50:44.000000 scipion_app-3.4.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-23 07:50:44.000000 scipion_app-3.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-05-23 07:50:54.445764 scipion_app-3.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-05-23 07:50:44.000000 scipion_app-3.4.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-23 07:50:44.000000 scipion_app-3.4.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:50:54.437764 scipion_app-3.4.0/scipion/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-23 07:50:44.000000 scipion_app-3.4.0/scipion/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    19070 2024-05-23 07:50:44.000000 scipion_app-3.4.0/scipion/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-23 07:50:44.000000 scipion_app-3.4.0/scipion/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-05-23 07:50:44.000000 scipion_app-3.4.0/scipion/guiplugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:50:54.441764 scipion_app-3.4.0/scipion/install/
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-23 07:50:44.000000 scipion_app-3.4.0/scipion/install/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3224 2024-05-23 07:50:44.000000 scipion_app-3.4.0/scipion/install/change_rpath.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      883 2024-05-23 07:50:44.000000 scipion_app-3.4.0/scipion/install/clean.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4144 2024-05-23 07:50:44.000000 scipion_app-3.4.0/scipion/install/find_deps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60354 2024-05-23 07:50:44.000000 scipion_app-3.4.0/scipion/install/funcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6810 2024-05-23 07:50:44.000000 scipion_app-3.4.0/scipion/install/inspect_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15717 2024-05-23 07:50:44.000000 scipion_app-3.4.0/scipion/install/install_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20229 2024-05-23 07:50:44.000000 scipion_app-3.4.0/scipion/install/plugin_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50556 2024-05-23 07:50:44.000000 scipion_app-3.4.0/scipion/install/plugin_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5882 2024-05-23 07:50:44.000000 scipion_app-3.4.0/scipion/install/update_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:50:54.441764 scipion_app-3.4.0/scipion/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 07:50:44.000000 scipion_app-3.4.0/scipion/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18188 2024-05-23 07:50:44.000000 scipion_app-3.4.0/scipion/scripts/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7415 2024-05-23 07:50:44.000000 scipion_app-3.4.0/scipion/scripts/fontbrowser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19106 2024-05-23 07:50:44.000000 scipion_app-3.4.0/scipion/scripts/kickoff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4103 2024-05-23 07:50:44.000000 scipion_app-3.4.0/scipion/scripts/tutorial.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:50:54.445764 scipion_app-3.4.0/scipion/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-05-23 07:50:44.000000 scipion_app-3.4.0/scipion/templates/hosts.template
+-rw-r--r--   0 runner    (1001) docker     (127)     3690 2024-05-23 07:50:44.000000 scipion_app-3.4.0/scipion/templates/protocols.template
+-rw-r--r--   0 runner    (1001) docker     (127)     4292 2024-05-23 07:50:44.000000 scipion_app-3.4.0/scipion/templates/scipion.template
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-23 07:50:44.000000 scipion_app-3.4.0/scipion/templates/scipionbox.template
+-rw-r--r--   0 runner    (1001) docker     (127)     4197 2024-05-23 07:50:44.000000 scipion_app-3.4.0/scipion/templates/workflow_betagal1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-05-23 07:50:44.000000 scipion_app-3.4.0/scipion/templates/workflow_betagal2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8100 2024-05-23 07:50:44.000000 scipion_app-3.4.0/scipion/templates/workflow_tutorial_intro.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-05-23 07:50:44.000000 scipion_app-3.4.0/scipion/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 07:50:54.445764 scipion_app-3.4.0/scipion_app.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-05-23 07:50:54.000000 scipion_app-3.4.0/scipion_app.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-23 07:50:54.000000 scipion_app-3.4.0/scipion_app.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 07:50:54.000000 scipion_app-3.4.0/scipion_app.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-23 07:50:54.000000 scipion_app-3.4.0/scipion_app.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-23 07:50:54.000000 scipion_app-3.4.0/scipion_app.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-23 07:50:54.000000 scipion_app-3.4.0/scipion_app.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 07:50:54.445764 scipion_app-3.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-05-23 07:50:44.000000 scipion_app-3.4.0/setup.py
```

### Comparing `scipion-app-3.3.1/CHANGES.txt` & `scipion_app-3.4.0/CHANGES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+V3.4.0
+ - Adapted to variables registry
+ - printenv refactored (does not print export) and is more detailed.
+ - Replace pip internal command with subprocess call
 V3.3.1
 users:
  - Adapted to sprites
  - Defining TomoDataViewer as the TiltSeries default viewer
 V3.3.0
 developers:
  - Exist code is not masked when running xmipp, relion etc commands
```

### Comparing `scipion-app-3.3.1/LICENSE.txt` & `scipion_app-3.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `scipion-app-3.3.1/PKG-INFO` & `scipion_app-3.4.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scipion-app
-Version: 3.3.1
+Version: 3.4.0
 Summary: Scipion application. For processing cryo electron microscopy images and hybrid modelling
 Home-page: https://github.com/scipion-em/scipion-app
 Author: Scipion team
 Author-email: scipion@cnb.csic.es
 Keywords: scipion cryoem imageprocessing scipion-3.0
 License-File: LICENSE.txt
 Requires-Dist: scipion-em
@@ -18,15 +18,15 @@
 **Scipion** is an image processing framework to obtain 3D models of
 macromolecular complexes using Electron Microscopy (3DEM). It integrates
 several software packages and presents an unified interface for both biologists
 and developers. Scipion allows to execute workflows combining different
 software tools, while taking care of formats and conversions. Additionally,
 all steps are tracked and can be reproduced later on.
 
-Want to learn more? [Go to our web site.](http://scipion.i2pc.es)
+Want to learn more? [Go to our web site.](https://scipion.i2pc.es)
 
 
 .. figure:: https://travis-ci.org/I2PC/scipion.svg?branch=devel
    :align: left
    :alt: Build Status
 
 .. figure:: https://sonarcloud.io/api/project_badges/measure?project=Scipion&metric=alert_status
```

### Comparing `scipion-app-3.3.1/README.rst` & `scipion_app-3.4.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 **Scipion** is an image processing framework to obtain 3D models of
 macromolecular complexes using Electron Microscopy (3DEM). It integrates
 several software packages and presents an unified interface for both biologists
 and developers. Scipion allows to execute workflows combining different
 software tools, while taking care of formats and conversions. Additionally,
 all steps are tracked and can be reproduced later on.
 
-Want to learn more? [Go to our web site.](http://scipion.i2pc.es)
+Want to learn more? [Go to our web site.](https://scipion.i2pc.es)
 
 
 .. figure:: https://travis-ci.org/I2PC/scipion.svg?branch=devel
    :align: left
    :alt: Build Status
 
 .. figure:: https://sonarcloud.io/api/project_badges/measure?project=Scipion&metric=alert_status
```

### Comparing `scipion-app-3.3.1/scipion/__main__.py` & `scipion_app-3.4.0/scipion/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -340,21 +340,27 @@
         runApp(protocolApp, args=sys.argv[3:])
 
     elif mode == MODE_PROTOCOLS:
         runApp('pw_protocol_list.py', args=sys.argv[2:])
 
     elif mode == MODE_ENV:
         # Print all the environment variables needed to run scipion.
-        from pyworkflow.plugin import Plugin
+        from pyworkflow.utils import greenStr,yellowStr
 
         # Trigger plugin's variable definition
         pyworkflow.Config.getDomain().getPlugins()
-        VARS.update(pyworkflow.plugin.Plugin.getVars())
-        for key in sorted(VARS):
-            sys.stdout.write('export %s="%s"\n' % (key, VARS[key]))
+
+        for key, var in pyworkflow.VariablesRegistry.variables().items():
+
+            sys.stdout.write('%s="%s"\n' % (key,var.value))
+
+            if len(sys.argv) > 2:
+                if var.description is not None:
+                    sys.stdout.write(greenStr(var.description+"\n"))
+                sys.stdout.write(yellowStr("SOURCE: %s\n" % var.source))
 
         sys.exit(0)
 
     elif mode == MODE_RUN:
         # Run any command with the environment of scipion loaded.
         runCmd('emprogram ' + ' '.join(['"%s"' % arg for arg in sys.argv[2:]]))
```

### Comparing `scipion-app-3.3.1/scipion/constants.py` & `scipion_app-3.4.0/scipion/constants.py`

 * *Files identical despite different names*

### Comparing `scipion-app-3.3.1/scipion/guiplugin.py` & `scipion_app-3.4.0/scipion/guiplugin.py`

 * *Files identical despite different names*

### Comparing `scipion-app-3.3.1/scipion/install/__init__.py` & `scipion_app-3.4.0/scipion/install/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-app-3.3.1/scipion/install/change_rpath.py` & `scipion_app-3.4.0/scipion/install/change_rpath.py`

 * *Files identical despite different names*

### Comparing `scipion-app-3.3.1/scipion/install/clean.py` & `scipion_app-3.4.0/scipion/install/clean.py`

 * *Files identical despite different names*

### Comparing `scipion-app-3.3.1/scipion/install/find_deps.py` & `scipion_app-3.4.0/scipion/install/find_deps.py`

 * *Files identical despite different names*

### Comparing `scipion-app-3.3.1/scipion/install/funcs.py` & `scipion_app-3.4.0/scipion/install/funcs.py`

 * *Files 1% similar despite different names*

```diff
@@ -882,14 +882,15 @@
 
     def addTarget(self, targets: list):
         """ Centralized internal method to add targets. They could be a list of string commands or a single command"""
         if targets is not None:
             lastTargets = self._cmds[-1][1]
 
             lastTargets.extend(targets if isinstance(targets, list) else [targets])
+        return self
 
     def getCommands(self)->list:
         """ Returns the commands"""
         return self._cmds
 
     def append(self, newCmd:str, targets=None, sep="&&"):
         """ Appends an extra command to the existing one.
@@ -920,21 +921,24 @@
     def cd(self, folder):
         """ Appends a cd command to the existing one
 
         :param folder: folder to changes director to
         """
         return self.append("cd %s" % folder)
 
-    def touch(self, fileName):
+    def touch(self, fileName, isTarget=True):
         """ Appends a touch command and its target based on the fileName
 
         :param fileName: file to touch. Should be created in the binary home folder. Use ../ in case of a previous cd command
 
         :return: CondaCommandDef (self)
         """
+        if isTarget:
+            # Add the touched file as target
+            self.addTarget(fileName)
 
         return self.append("touch %s" % fileName, os.path.basename(fileName))
 
 
 class CondaCommandDef(CommandDef):
     """ Extends CommandDef with some conda specific methods"""
```

### Comparing `scipion-app-3.3.1/scipion/install/inspect_plugins.py` & `scipion_app-3.4.0/scipion/install/inspect_plugins.py`

 * *Files identical despite different names*

### Comparing `scipion-app-3.3.1/scipion/install/install_plugin.py` & `scipion_app-3.4.0/scipion/install/install_plugin.py`

 * *Files identical despite different names*

### Comparing `scipion-app-3.3.1/scipion/install/plugin_funcs.py` & `scipion_app-3.4.0/scipion/install/plugin_funcs.py`

 * *Files identical despite different names*

### Comparing `scipion-app-3.3.1/scipion/install/plugin_manager.py` & `scipion_app-3.4.0/scipion/install/plugin_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -349,15 +349,15 @@
         self._fillPluginManagerGui(parentFrame)
 
     def _lunchProgressBar(self, parent):
         self.progressbarLabel = ttk.Label(parent, text='Loading Plugins...',
                                           background='white')
         self.progressbarLabel.place(x=480, y=65, width=200)
         self.progressbar = ttk.Progressbar(parent)
-        self.progressbar.place(x=450, y=85 + cfgFontSize, width=200)
+        self.progressbar.place(x=450, y=85 + Config.SCIPION_FONT_SIZE, width=200)
         self.progressbar.step(1)
         self.progressbar.start(200)
 
     def _closeProgressBar(self):
         self.progressbar.stop()
         self.progressbar.destroy()
         self.progressbarLabel.destroy()
```

### Comparing `scipion-app-3.3.1/scipion/install/update_manager.py` & `scipion_app-3.4.0/scipion/install/update_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,16 +25,16 @@
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 """
 This module is responsible for updating scipion-em, scipion-pyworkflow and
 scipion-app if a higher version of these is released
 """
+import subprocess
 import argparse
-from pip._internal.commands import create_command
 
 from pyworkflow.utils import redStr, greenStr, os
 from scipion.constants import MODE_UPDATE
 
 DRY_COMMAND = '-dry'
 SCIPION_NAME = 'Scipion'
 
@@ -114,15 +114,15 @@
         """
         # Ignore auto-check of outdated package that happens at import time
         os.environ["OUTDATED_IGNORE"] = "1"
         from outdated import check_outdated
         from requests.exceptions import ConnectionError
         try:
             checkOutdated = check_outdated(packageName, version)
-        except ConnectionError as connError:
+        except ConnectionError:
             print("Cannot check update status of %s (%s)" % (packageName, version))
             return False, version
         except ValueError:
             # We intentionally skip this error
             # When working in devel mode with an increased version not yet release this Value error
             # happens: --> example: Version 3.0.2 is greater than the latest version on PyPI: 3.0.1
             return False, version
@@ -133,21 +133,15 @@
         return checkOutdated
 
     @classmethod
     def updateScipion(cls, outdatedPackages):
         """
         Update a module from which there is released a higher version
         """
-        kwargs = {'isolated': False}
-
         for packageName in outdatedPackages:
-            cmd_args = [packageName[0],
-                        '--upgrade',
-                        '-vvv']  # highest level of verbosity
-
-            command = create_command('install', **kwargs)
-            status = command.main(cmd_args)
-            if status == 0:
+            cmd_args = ['pip', 'install', '--upgrade', packageName[0]]
+            result = subprocess.call(cmd_args)
+            if result == 0:
                 print('%s was correctly updated.' % packageName[0])
             else:
                 print('Something went wrong during the update of %s.'
                       % packageName[0])
```

### Comparing `scipion-app-3.3.1/scipion/scripts/config.py` & `scipion_app-3.4.0/scipion/scripts/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 Check the local configuration files, and/or create them if requested
 or if they do not exist.
 """
 import sys
 import os
 from datetime import datetime
 from os.path import join, exists, basename
-import time
 import optparse
 from pathlib import Path
 
 from configparser import ConfigParser
 from shutil import copyfile
 
 from scipion.utils import getTemplatesPath
```

### Comparing `scipion-app-3.3.1/scipion/scripts/fontbrowser.py` & `scipion_app-3.4.0/scipion/scripts/fontbrowser.py`

 * *Files identical despite different names*

### Comparing `scipion-app-3.3.1/scipion/scripts/kickoff.py` & `scipion_app-3.4.0/scipion/scripts/kickoff.py`

 * *Files 2% similar despite different names*

```diff
@@ -157,17 +157,17 @@
         self.argsList = argsList
         self.showScheduleOption = showScheduleOption
         self.schedule = schedule
         self.showProjectOption = showProjectOption
         self.showProject = showProject
         self.showProjectName = showProjectName
 
-        bigSize = pwgui.cfgFontSize + 2
-        smallSize = pwgui.cfgFontSize - 2
-        fontName = pwgui.cfgFontName
+        bigSize = pw.Config.SCIPION_FONT_SIZE + 2
+        smallSize = pw.Config.SCIPION_FONT_SIZE - 2
+        fontName = pw.Config.SCIPION_FONT_NAME
 
         self.bigFont = tkFont.Font(size=bigSize, family=fontName)
         self.bigFontBold = tkFont.Font(size=bigSize, family=fontName,
                                        weight='bold')
 
         self.projDateFont = tkFont.Font(size=smallSize, family=fontName)
         self.projDelFont = tkFont.Font(size=smallSize, family=fontName,
```

### Comparing `scipion-app-3.3.1/scipion/scripts/tutorial.py` & `scipion_app-3.4.0/scipion/scripts/tutorial.py`

 * *Files identical despite different names*

### Comparing `scipion-app-3.3.1/scipion/templates/hosts.template` & `scipion_app-3.4.0/scipion/templates/hosts.template`

 * *Files identical despite different names*

### Comparing `scipion-app-3.3.1/scipion/templates/protocols.template` & `scipion_app-3.4.0/scipion/templates/protocols.template`

 * *Files identical despite different names*

### Comparing `scipion-app-3.3.1/scipion/templates/scipion.template` & `scipion_app-3.4.0/scipion/templates/scipion.template`

 * *Files identical despite different names*

### Comparing `scipion-app-3.3.1/scipion/templates/scipionbox.template` & `scipion_app-3.4.0/scipion/templates/scipionbox.template`

 * *Files identical despite different names*

### Comparing `scipion-app-3.3.1/scipion/templates/workflow_betagal1.json` & `scipion_app-3.4.0/scipion/templates/workflow_betagal1.json`

 * *Files identical despite different names*

### Comparing `scipion-app-3.3.1/scipion/templates/workflow_betagal2.json` & `scipion_app-3.4.0/scipion/templates/workflow_betagal2.json`

 * *Files identical despite different names*

### Comparing `scipion-app-3.3.1/scipion/templates/workflow_tutorial_intro.json` & `scipion_app-3.4.0/scipion/templates/workflow_tutorial_intro.json`

 * *Files identical despite different names*

### Comparing `scipion-app-3.3.1/scipion/utils.py` & `scipion_app-3.4.0/scipion/utils.py`

 * *Files identical despite different names*

### Comparing `scipion-app-3.3.1/scipion_app.egg-info/PKG-INFO` & `scipion_app-3.4.0/scipion_app.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scipion-app
-Version: 3.3.1
+Version: 3.4.0
 Summary: Scipion application. For processing cryo electron microscopy images and hybrid modelling
 Home-page: https://github.com/scipion-em/scipion-app
 Author: Scipion team
 Author-email: scipion@cnb.csic.es
 Keywords: scipion cryoem imageprocessing scipion-3.0
 License-File: LICENSE.txt
 Requires-Dist: scipion-em
@@ -18,15 +18,15 @@
 **Scipion** is an image processing framework to obtain 3D models of
 macromolecular complexes using Electron Microscopy (3DEM). It integrates
 several software packages and presents an unified interface for both biologists
 and developers. Scipion allows to execute workflows combining different
 software tools, while taking care of formats and conversions. Additionally,
 all steps are tracked and can be reproduced later on.
 
-Want to learn more? [Go to our web site.](http://scipion.i2pc.es)
+Want to learn more? [Go to our web site.](https://scipion.i2pc.es)
 
 
 .. figure:: https://travis-ci.org/I2PC/scipion.svg?branch=devel
    :align: left
    :alt: Build Status
 
 .. figure:: https://sonarcloud.io/api/project_badges/measure?project=Scipion&metric=alert_status
```

### Comparing `scipion-app-3.3.1/scipion_app.egg-info/SOURCES.txt` & `scipion_app-3.4.0/scipion_app.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scipion-app-3.3.1/setup.py` & `scipion_app-3.4.0/setup.py`

 * *Files identical despite different names*

