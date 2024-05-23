# Comparing `tmp/bolt-ta-0.3.5.tar.gz` & `tmp/bolt-ta-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bolt-ta-0.3.5.tar", last modified: Tue Oct 17 11:27:13 2023, max compression
+gzip compressed data, was "bolt-ta-0.3.7.tar", last modified: Thu May 23 12:12:00 2024, max compression
```

## Comparing `bolt-ta-0.3.5.tar` & `bolt-ta-0.3.7.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 11:27:13.533654 bolt-ta-0.3.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2023-10-17 11:26:58.000000 bolt-ta-0.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3726 2023-10-17 11:27:13.533654 bolt-ta-0.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2750 2023-10-17 11:26:58.000000 bolt-ta-0.3.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 11:27:13.533654 bolt-ta-0.3.5/bolt/
--rw-r--r--   0 runner    (1001) docker     (127)      891 2023-10-17 11:26:58.000000 bolt-ta-0.3.5/bolt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3392 2023-10-17 11:26:58.000000 bolt-ta-0.3.5/bolt/_btapp.py
--rw-r--r--   0 runner    (1001) docker     (127)      861 2023-10-17 11:26:58.000000 bolt-ta-0.3.5/bolt/_btconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     4653 2023-10-17 11:26:58.000000 bolt-ta-0.3.5/bolt/_btoptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1360 2023-10-17 11:26:58.000000 bolt-ta-0.3.5/bolt/_btregistry.py
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2023-10-17 11:26:58.000000 bolt-ta-0.3.5/bolt/_btrunner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1568 2023-10-17 11:26:58.000000 bolt-ta-0.3.5/bolt/_btutils.py
--rw-r--r--   0 runner    (1001) docker     (127)      781 2023-10-17 11:26:58.000000 bolt-ta-0.3.5/bolt/about.py
--rw-r--r--   0 runner    (1001) docker     (127)     3376 2023-10-17 11:26:58.000000 bolt-ta-0.3.5/bolt/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1694 2023-10-17 11:26:58.000000 bolt-ta-0.3.5/bolt/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 11:27:13.533654 bolt-ta-0.3.5/bolt/tasks/
--rw-r--r--   0 runner    (1001) docker     (127)        8 2023-10-17 11:26:58.000000 bolt-ta-0.3.5/bolt/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1587 2023-10-17 11:26:58.000000 bolt-ta-0.3.5/bolt/tasks/bolt_conttest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2023-10-17 11:26:58.000000 bolt-ta-0.3.5/bolt/tasks/bolt_coverage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2740 2023-10-17 11:26:58.000000 bolt-ta-0.3.5/bolt/tasks/bolt_delete_files.py
--rw-r--r--   0 runner    (1001) docker     (127)      762 2023-10-17 11:26:58.000000 bolt-ta-0.3.5/bolt/tasks/bolt_mkdir.py
--rw-r--r--   0 runner    (1001) docker     (127)     1992 2023-10-17 11:26:58.000000 bolt-ta-0.3.5/bolt/tasks/bolt_nose.py
--rw-r--r--   0 runner    (1001) docker     (127)     2942 2023-10-17 11:26:58.000000 bolt-ta-0.3.5/bolt/tasks/bolt_pip.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2023-10-17 11:26:58.000000 bolt-ta-0.3.5/bolt/tasks/bolt_set_vars.py
--rw-r--r--   0 runner    (1001) docker     (127)     1899 2023-10-17 11:26:58.000000 bolt-ta-0.3.5/bolt/tasks/bolt_setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2023-10-17 11:26:58.000000 bolt-ta-0.3.5/bolt/tasks/bolt_shell.py
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2023-10-17 11:26:58.000000 bolt-ta-0.3.5/bolt/tasks/bolt_sleep.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 11:27:13.533654 bolt-ta-0.3.5/bolt/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2023-10-17 11:26:58.000000 bolt-ta-0.3.5/bolt/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2023-10-17 11:26:58.000000 bolt-ta-0.3.5/bolt/utils/_utconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2023-10-17 11:26:58.000000 bolt-ta-0.3.5/bolt/utils/_utfiles.py
--rw-r--r--   0 runner    (1001) docker     (127)      180 2023-10-17 11:26:58.000000 bolt-ta-0.3.5/bolt/utils/_uttime.py
--rw-r--r--   0 runner    (1001) docker     (127)      607 2023-10-17 11:26:58.000000 bolt-ta-0.3.5/bolt/utils/log.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 11:27:13.533654 bolt-ta-0.3.5/bolt_ta.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3726 2023-10-17 11:27:13.000000 bolt-ta-0.3.5/bolt_ta.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      940 2023-10-17 11:27:13.000000 bolt-ta-0.3.5/bolt_ta.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-17 11:27:13.000000 bolt-ta-0.3.5/bolt_ta.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2023-10-17 11:27:13.000000 bolt-ta-0.3.5/bolt_ta.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2023-10-17 11:27:13.000000 bolt-ta-0.3.5/bolt_ta.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       67 2023-10-17 11:27:13.537654 bolt-ta-0.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      692 2023-10-17 11:26:58.000000 bolt-ta-0.3.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 11:27:13.533654 bolt-ta-0.3.5/test/
--rw-r--r--   0 runner    (1001) docker     (127)     3965 2023-10-17 11:26:58.000000 bolt-ta-0.3.5/test/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     6283 2023-10-17 11:26:58.000000 bolt-ta-0.3.5/test/test_btapp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2023-10-17 11:26:58.000000 bolt-ta-0.3.5/test/test_btconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     3928 2023-10-17 11:26:58.000000 bolt-ta-0.3.5/test/test_btoptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1473 2023-10-17 11:26:58.000000 bolt-ta-0.3.5/test/test_btregistry.py
--rw-r--r--   0 runner    (1001) docker     (127)     5129 2023-10-17 11:26:58.000000 bolt-ta-0.3.5/test/test_btrunner.py
--rw-r--r--   0 runner    (1001) docker     (127)       73 2023-10-17 11:26:58.000000 bolt-ta-0.3.5/test/test_btutils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2761 2023-10-17 11:26:58.000000 bolt-ta-0.3.5/test/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)      117 2023-10-17 11:26:58.000000 bolt-ta-0.3.5/test/test_log.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:12:00.736202 bolt-ta-0.3.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-23 12:11:35.000000 bolt-ta-0.3.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-05-23 12:12:00.736202 bolt-ta-0.3.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2750 2024-05-23 12:11:35.000000 bolt-ta-0.3.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:12:00.732202 bolt-ta-0.3.7/bolt/
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-23 12:11:35.000000 bolt-ta-0.3.7/bolt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-05-23 12:11:35.000000 bolt-ta-0.3.7/bolt/_btapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-23 12:11:35.000000 bolt-ta-0.3.7/bolt/_btconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4653 2024-05-23 12:11:35.000000 bolt-ta-0.3.7/bolt/_btoptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-05-23 12:11:35.000000 bolt-ta-0.3.7/bolt/_btregistry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-05-23 12:11:35.000000 bolt-ta-0.3.7/bolt/_btrunner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-05-23 12:11:35.000000 bolt-ta-0.3.7/bolt/_btutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-23 12:11:35.000000 bolt-ta-0.3.7/bolt/about.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3376 2024-05-23 12:11:35.000000 bolt-ta-0.3.7/bolt/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-05-23 12:11:35.000000 bolt-ta-0.3.7/bolt/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:12:00.736202 bolt-ta-0.3.7/bolt/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-23 12:11:35.000000 bolt-ta-0.3.7/bolt/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-05-23 12:11:35.000000 bolt-ta-0.3.7/bolt/tasks/bolt_conttest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-05-23 12:11:35.000000 bolt-ta-0.3.7/bolt/tasks/bolt_coverage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-05-23 12:11:35.000000 bolt-ta-0.3.7/bolt/tasks/bolt_delete_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-05-23 12:11:35.000000 bolt-ta-0.3.7/bolt/tasks/bolt_mkdir.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-05-23 12:11:35.000000 bolt-ta-0.3.7/bolt/tasks/bolt_nose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-05-23 12:11:35.000000 bolt-ta-0.3.7/bolt/tasks/bolt_pip.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-05-23 12:11:35.000000 bolt-ta-0.3.7/bolt/tasks/bolt_set_vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-05-23 12:11:35.000000 bolt-ta-0.3.7/bolt/tasks/bolt_setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-05-23 12:11:35.000000 bolt-ta-0.3.7/bolt/tasks/bolt_shell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-23 12:11:35.000000 bolt-ta-0.3.7/bolt/tasks/bolt_sleep.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:12:00.736202 bolt-ta-0.3.7/bolt/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-23 12:11:35.000000 bolt-ta-0.3.7/bolt/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-05-23 12:11:35.000000 bolt-ta-0.3.7/bolt/utils/_utconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-23 12:11:35.000000 bolt-ta-0.3.7/bolt/utils/_utfiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-23 12:11:35.000000 bolt-ta-0.3.7/bolt/utils/_uttime.py
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-23 12:11:35.000000 bolt-ta-0.3.7/bolt/utils/log.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:12:00.736202 bolt-ta-0.3.7/bolt_ta.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-05-23 12:12:00.000000 bolt-ta-0.3.7/bolt_ta.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-23 12:12:00.000000 bolt-ta-0.3.7/bolt_ta.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 12:12:00.000000 bolt-ta-0.3.7/bolt_ta.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-23 12:12:00.000000 bolt-ta-0.3.7/bolt_ta.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-23 12:12:00.000000 bolt-ta-0.3.7/bolt_ta.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-23 12:12:00.736202 bolt-ta-0.3.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-23 12:11:35.000000 bolt-ta-0.3.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 12:12:00.736202 bolt-ta-0.3.7/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-05-23 12:11:35.000000 bolt-ta-0.3.7/test/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6283 2024-05-23 12:11:35.000000 bolt-ta-0.3.7/test/test_btapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-05-23 12:11:35.000000 bolt-ta-0.3.7/test/test_btconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3928 2024-05-23 12:11:35.000000 bolt-ta-0.3.7/test/test_btoptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-05-23 12:11:35.000000 bolt-ta-0.3.7/test/test_btregistry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5129 2024-05-23 12:11:35.000000 bolt-ta-0.3.7/test/test_btrunner.py
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-23 12:11:35.000000 bolt-ta-0.3.7/test/test_btutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-05-23 12:11:35.000000 bolt-ta-0.3.7/test/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-23 12:11:35.000000 bolt-ta-0.3.7/test/test_log.py
```

### Comparing `bolt-ta-0.3.5/LICENSE` & `bolt-ta-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `bolt-ta-0.3.5/PKG-INFO` & `bolt-ta-0.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bolt-ta
-Version: 0.3.5
+Version: 0.3.7
 Summary: A task runner written in Python
 Home-page: https://github.com/abantos/bolt
 Author: Isaac Rodriguez
 Author-email: oss.abantos@outlook.com
 License: MIT
 Keywords: automation task tool development
 Platform: UNKNOWN
```

### Comparing `bolt-ta-0.3.5/README.md` & `bolt-ta-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `bolt-ta-0.3.5/bolt/__init__.py` & `bolt-ta-0.3.7/bolt/__init__.py`

 * *Files identical despite different names*

### Comparing `bolt-ta-0.3.5/bolt/_btapp.py` & `bolt-ta-0.3.7/bolt/_btapp.py`

 * *Files identical despite different names*

### Comparing `bolt-ta-0.3.5/bolt/_btconfig.py` & `bolt-ta-0.3.7/bolt/_btconfig.py`

 * *Files identical despite different names*

### Comparing `bolt-ta-0.3.5/bolt/_btoptions.py` & `bolt-ta-0.3.7/bolt/_btoptions.py`

 * *Files identical despite different names*

### Comparing `bolt-ta-0.3.5/bolt/_btregistry.py` & `bolt-ta-0.3.7/bolt/_btregistry.py`

 * *Files identical despite different names*

### Comparing `bolt-ta-0.3.5/bolt/_btrunner.py` & `bolt-ta-0.3.7/bolt/_btrunner.py`

 * *Files identical despite different names*

### Comparing `bolt-ta-0.3.5/bolt/_btutils.py` & `bolt-ta-0.3.7/bolt/_btutils.py`

 * *Files identical despite different names*

### Comparing `bolt-ta-0.3.5/bolt/about.py` & `bolt-ta-0.3.7/bolt/about.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 
 """
 project = "bolt-ta"
 version = "0.3"
-release = "0.3.5"
+release = "0.3.7"
 description = "A task runner written in Python"
 copyright = "2016 Abantos"
 author = "Isaac Rodriguez"
 author_email = "oss.abantos@outlook.com"
 url = "https://github.com/abantos/bolt"
 license = "MIT"
 keywords = "automation task tool development"
```

### Comparing `bolt-ta-0.3.5/bolt/api.py` & `bolt-ta-0.3.7/bolt/api.py`

 * *Files identical despite different names*

### Comparing `bolt-ta-0.3.5/bolt/errors.py` & `bolt-ta-0.3.7/bolt/errors.py`

 * *Files identical despite different names*

### Comparing `bolt-ta-0.3.5/bolt/tasks/bolt_conttest.py` & `bolt-ta-0.3.7/bolt/tasks/bolt_conttest.py`

 * *Files identical despite different names*

### Comparing `bolt-ta-0.3.5/bolt/tasks/bolt_coverage.py` & `bolt-ta-0.3.7/bolt/tasks/bolt_coverage.py`

 * *Files identical despite different names*

### Comparing `bolt-ta-0.3.5/bolt/tasks/bolt_delete_files.py` & `bolt-ta-0.3.7/bolt/tasks/bolt_delete_files.py`

 * *Files identical despite different names*

### Comparing `bolt-ta-0.3.5/bolt/tasks/bolt_mkdir.py` & `bolt-ta-0.3.7/bolt/tasks/bolt_mkdir.py`

 * *Files identical despite different names*

### Comparing `bolt-ta-0.3.5/bolt/tasks/bolt_nose.py` & `bolt-ta-0.3.7/bolt/tasks/bolt_nose.py`

 * *Files identical despite different names*

### Comparing `bolt-ta-0.3.5/bolt/tasks/bolt_pip.py` & `bolt-ta-0.3.7/bolt/tasks/bolt_pip.py`

 * *Files identical despite different names*

### Comparing `bolt-ta-0.3.5/bolt/tasks/bolt_set_vars.py` & `bolt-ta-0.3.7/bolt/tasks/bolt_set_vars.py`

 * *Files identical despite different names*

### Comparing `bolt-ta-0.3.5/bolt/tasks/bolt_setup.py` & `bolt-ta-0.3.7/bolt/tasks/bolt_setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
             'options': {
                 'verbose': True,
                 'dry-run': True
             }
         }
     }
 """
-import distutils.core as dcore
+import logging
 
 import bolt.api as api
 import bolt.utils as utilities
 
 DEFAULT_ARGUMENTS = ["build"]
 DEFAULT_SETUP_SCRIPT = "setup.py"
 
@@ -37,22 +37,29 @@
         self.setup_script = self._optional("script")
         if self.setup_script:
             self.config["script"] = False
         else:
             self.setup_script = DEFAULT_SETUP_SCRIPT
         generator = _SetupArgumentGenerator()
         self.args = generator.generate_from(self.config)
+        logging.debug(f'Setup script: {self.setup_script}')
+        logging.debug(f'Arguments: {self.args}')
 
     def _execute(self):
         result = self._execute_setup()
         if not result.dist_files:
             raise BuildSetupError()
 
-    def _execute_setup(self):
-        return dcore.run_setup(self.setup_script, self.args)
+    def _execute_setup(self):        
+        try:
+            import distutils.core as dcore
+            return dcore.run_setup(self.setup_script, self.args)
+        except ImportError:
+            logging.warning('Failed to import <distutils> please install the <setuptools> package.')
+            
 
 
 def register_tasks(registry):
     registry.register_task("setup", ExecuteSetupTask())
 
 
 class _SetupArgumentGenerator(utilities.CommonCommandAndArgumentsGenerator):
```

### Comparing `bolt-ta-0.3.5/bolt/tasks/bolt_sleep.py` & `bolt-ta-0.3.7/bolt/tasks/bolt_sleep.py`

 * *Files identical despite different names*

### Comparing `bolt-ta-0.3.5/bolt/utils/_utconfig.py` & `bolt-ta-0.3.7/bolt/utils/_utconfig.py`

 * *Files identical despite different names*

### Comparing `bolt-ta-0.3.5/bolt/utils/_utfiles.py` & `bolt-ta-0.3.7/bolt/utils/_utfiles.py`

 * *Files identical despite different names*

### Comparing `bolt-ta-0.3.5/bolt/utils/log.py` & `bolt-ta-0.3.7/bolt/utils/log.py`

 * *Files identical despite different names*

### Comparing `bolt-ta-0.3.5/bolt_ta.egg-info/PKG-INFO` & `bolt-ta-0.3.7/bolt_ta.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bolt-ta
-Version: 0.3.5
+Version: 0.3.7
 Summary: A task runner written in Python
 Home-page: https://github.com/abantos/bolt
 Author: Isaac Rodriguez
 Author-email: oss.abantos@outlook.com
 License: MIT
 Keywords: automation task tool development
 Platform: UNKNOWN
```

### Comparing `bolt-ta-0.3.5/bolt_ta.egg-info/SOURCES.txt` & `bolt-ta-0.3.7/bolt_ta.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bolt-ta-0.3.5/setup.py` & `bolt-ta-0.3.7/setup.py`

 * *Files identical despite different names*

### Comparing `bolt-ta-0.3.5/test/test_api.py` & `bolt-ta-0.3.7/test/test_api.py`

 * *Files identical despite different names*

### Comparing `bolt-ta-0.3.5/test/test_btapp.py` & `bolt-ta-0.3.7/test/test_btapp.py`

 * *Files identical despite different names*

### Comparing `bolt-ta-0.3.5/test/test_btconfig.py` & `bolt-ta-0.3.7/test/test_btconfig.py`

 * *Files identical despite different names*

### Comparing `bolt-ta-0.3.5/test/test_btoptions.py` & `bolt-ta-0.3.7/test/test_btoptions.py`

 * *Files identical despite different names*

### Comparing `bolt-ta-0.3.5/test/test_btregistry.py` & `bolt-ta-0.3.7/test/test_btregistry.py`

 * *Files identical despite different names*

### Comparing `bolt-ta-0.3.5/test/test_btrunner.py` & `bolt-ta-0.3.7/test/test_btrunner.py`

 * *Files identical despite different names*

### Comparing `bolt-ta-0.3.5/test/test_errors.py` & `bolt-ta-0.3.7/test/test_errors.py`

 * *Files identical despite different names*

