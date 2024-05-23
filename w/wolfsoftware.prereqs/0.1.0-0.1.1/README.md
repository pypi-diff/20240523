# Comparing `tmp/wolfsoftware_prereqs-0.1.0.tar.gz` & `tmp/wolfsoftware_prereqs-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wolfsoftware_prereqs-0.1.0.tar", last modified: Wed May 22 15:11:43 2024, max compression
+gzip compressed data, was "wolfsoftware_prereqs-0.1.1.tar", last modified: Wed May 22 15:24:25 2024, max compression
```

## Comparing `wolfsoftware_prereqs-0.1.0.tar` & `wolfsoftware_prereqs-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:11:43.298144 wolfsoftware_prereqs-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-05-22 15:11:33.000000 wolfsoftware_prereqs-0.1.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     5524 2024-05-22 15:11:43.298144 wolfsoftware_prereqs-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4204 2024-05-22 15:11:33.000000 wolfsoftware_prereqs-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-22 15:11:43.298144 wolfsoftware_prereqs-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-05-22 15:11:33.000000 wolfsoftware_prereqs-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:11:43.294144 wolfsoftware_prereqs-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5581 2024-05-22 15:11:33.000000 wolfsoftware_prereqs-0.1.0/tests/test_prereqs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:11:43.294144 wolfsoftware_prereqs-0.1.0/wolfsoftware/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:11:43.294144 wolfsoftware_prereqs-0.1.0/wolfsoftware/prereqs/
--rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-05-22 15:11:33.000000 wolfsoftware_prereqs-0.1.0/wolfsoftware/prereqs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-05-22 15:11:33.000000 wolfsoftware_prereqs-0.1.0/wolfsoftware/prereqs/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3418 2024-05-22 15:11:33.000000 wolfsoftware_prereqs-0.1.0/wolfsoftware/prereqs/prerequisite_checker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:11:43.294144 wolfsoftware_prereqs-0.1.0/wolfsoftware.prereqs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5524 2024-05-22 15:11:43.000000 wolfsoftware_prereqs-0.1.0/wolfsoftware.prereqs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-22 15:11:43.000000 wolfsoftware_prereqs-0.1.0/wolfsoftware.prereqs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 15:11:43.000000 wolfsoftware_prereqs-0.1.0/wolfsoftware.prereqs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-22 15:11:43.000000 wolfsoftware_prereqs-0.1.0/wolfsoftware.prereqs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-22 15:11:43.000000 wolfsoftware_prereqs-0.1.0/wolfsoftware.prereqs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:24:25.624251 wolfsoftware_prereqs-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-05-22 15:24:18.000000 wolfsoftware_prereqs-0.1.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5526 2024-05-22 15:24:25.624251 wolfsoftware_prereqs-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4206 2024-05-22 15:24:18.000000 wolfsoftware_prereqs-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-22 15:24:25.624251 wolfsoftware_prereqs-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2101 2024-05-22 15:24:18.000000 wolfsoftware_prereqs-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:24:25.624251 wolfsoftware_prereqs-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5581 2024-05-22 15:24:18.000000 wolfsoftware_prereqs-0.1.1/tests/test_prereqs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:24:25.620251 wolfsoftware_prereqs-0.1.1/wolfsoftware/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:24:25.624251 wolfsoftware_prereqs-0.1.1/wolfsoftware/prereqs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1993 2024-05-22 15:24:18.000000 wolfsoftware_prereqs-0.1.1/wolfsoftware/prereqs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-05-22 15:24:18.000000 wolfsoftware_prereqs-0.1.1/wolfsoftware/prereqs/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3418 2024-05-22 15:24:18.000000 wolfsoftware_prereqs-0.1.1/wolfsoftware/prereqs/prerequisite_checker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:24:25.624251 wolfsoftware_prereqs-0.1.1/wolfsoftware.prereqs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5526 2024-05-22 15:24:25.000000 wolfsoftware_prereqs-0.1.1/wolfsoftware.prereqs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-22 15:24:25.000000 wolfsoftware_prereqs-0.1.1/wolfsoftware.prereqs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 15:24:25.000000 wolfsoftware_prereqs-0.1.1/wolfsoftware.prereqs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-22 15:24:25.000000 wolfsoftware_prereqs-0.1.1/wolfsoftware.prereqs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-22 15:24:25.000000 wolfsoftware_prereqs-0.1.1/wolfsoftware.prereqs.egg-info/top_level.txt
```

### Comparing `wolfsoftware_prereqs-0.1.0/LICENSE.md` & `wolfsoftware_prereqs-0.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `wolfsoftware_prereqs-0.1.0/PKG-INFO` & `wolfsoftware_prereqs-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wolfsoftware.prereqs
-Version: 0.1.0
+Version: 0.1.1
 Summary: Check for the presence of prerequisite commands and returns their paths.
 Home-page: https://github.com/DevelopersToolbox/check-prerequisite-package
 Author: Wolf Software
 Author-email: pypi@wolfsoftware.com
 License: MIT
 Project-URL:  Source, https://github.com/DevelopersToolbox/check-prerequisite-package
 Project-URL:  Tracker, https://github.com/DevelopersToolbox/check-prerequisite-package/issues/
@@ -94,15 +94,15 @@
 
 prerequisites: list[str] = ["python", "git"]
 
 try:
     command_paths: dict = check_prerequisite(prerequisites)
 except PrerequisiteCheckError as err:
     print("Prerequisite check failed:")
-    for error in e.errors:
+    for error in err.errors:
         print(error)
     sys.exit(0)
 
 print(command_paths['python'])
 ```
 
 Once the checks have completed, you now have a dict of commands and their associated paths which you can then utilise to ensure you are executing
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wolfsoftware.prereqs Version: 0.1.0 Summary: Check
+Metadata-Version: 2.1 Name: wolfsoftware.prereqs Version: 0.1.1 Summary: Check
 for the presence of prerequisite commands and returns their paths. Home-page:
 https://github.com/DevelopersToolbox/check-prerequisite-package Author: Wolf
 Software Author-email: pypi@wolfsoftware.com License: MIT Project-URL: Source,
 https://github.com/DevelopersToolbox/check-prerequisite-package Project-URL:
 Tracker, https://github.com/DevelopersToolbox/check-prerequisite-package/
 issues/ Project-URL: Documentation, https://github.com/DevelopersToolbox/check-
 prerequisite-package Project-URL: Sponsor, https://github.com/sponsors/
@@ -32,14 +32,14 @@
 package assist with that problem by taking a list of commands that must be
 installed and available and verifies that list at the start to ensure all of
 them are available. ## Installation ```shell pip install wolfsoftware.prereqs
 ``` ## Usage ```python import sys from wolfsoftware.prereqs import
 check_prerequisite, PrerequisiteCheckError prerequisites: list[str] =
 ["python", "git"] try: command_paths: dict = check_prerequisite(prerequisites)
 except PrerequisiteCheckError as err: print("Prerequisite check failed:") for
-error in e.errors: print(error) sys.exit(0) print(command_paths['python']) ```
-Once the checks have completed, you now have a dict of commands and their
+error in err.errors: print(error) sys.exit(0) print(command_paths['python'])
+``` Once the checks have completed, you now have a dict of commands and their
 associated paths which you can then utilise to ensure you are executing your
 subprocesses with the full path.
                                                  _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/
    _C_r_e_a_t_e_d_%_2_0_b_y_%_2_0_W_o_l_f_%_2_0_o_n_%_2_0_b_e_h_a_l_f_%_2_0_o_f_%_2_0_W_o_l_f_%_2_0_S_o_f_t_w_a_r_e_-_b_l_u_e_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-
                                                                          _b_a_d_g_e_]
```

### Comparing `wolfsoftware_prereqs-0.1.0/README.md` & `wolfsoftware_prereqs-0.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 
 prerequisites: list[str] = ["python", "git"]
 
 try:
     command_paths: dict = check_prerequisite(prerequisites)
 except PrerequisiteCheckError as err:
     print("Prerequisite check failed:")
-    for error in e.errors:
+    for error in err.errors:
         print(error)
     sys.exit(0)
 
 print(command_paths['python'])
 ```
 
 Once the checks have completed, you now have a dict of commands and their associated paths which you can then utilise to ensure you are executing
```

### Comparing `wolfsoftware_prereqs-0.1.0/setup.cfg` & `wolfsoftware_prereqs-0.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `wolfsoftware_prereqs-0.1.0/setup.py` & `wolfsoftware_prereqs-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     required: list[str] = f.read().splitlines()
 
 with open("README.md", 'r', encoding='UTF-8') as f:
     long_description: str = f.read()
 
 setup(
     name='wolfsoftware.prereqs',
-    version='0.1.0',
+    version='0.1.1',
     author='Wolf Software',
     author_email='pypi@wolfsoftware.com',
     description='Check for the presence of prerequisite commands and returns their paths.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     license='MIT',
     packages=['wolfsoftware.prereqs'],
```

### Comparing `wolfsoftware_prereqs-0.1.0/tests/test_prereqs.py` & `wolfsoftware_prereqs-0.1.1/tests/test_prereqs.py`

 * *Files identical despite different names*

### Comparing `wolfsoftware_prereqs-0.1.0/wolfsoftware/prereqs/__init__.py` & `wolfsoftware_prereqs-0.1.1/wolfsoftware/prereqs/__init__.py`

 * *Files identical despite different names*

### Comparing `wolfsoftware_prereqs-0.1.0/wolfsoftware/prereqs/exceptions.py` & `wolfsoftware_prereqs-0.1.1/wolfsoftware/prereqs/exceptions.py`

 * *Files identical despite different names*

### Comparing `wolfsoftware_prereqs-0.1.0/wolfsoftware/prereqs/prerequisite_checker.py` & `wolfsoftware_prereqs-0.1.1/wolfsoftware/prereqs/prerequisite_checker.py`

 * *Files identical despite different names*

### Comparing `wolfsoftware_prereqs-0.1.0/wolfsoftware.prereqs.egg-info/PKG-INFO` & `wolfsoftware_prereqs-0.1.1/wolfsoftware.prereqs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wolfsoftware.prereqs
-Version: 0.1.0
+Version: 0.1.1
 Summary: Check for the presence of prerequisite commands and returns their paths.
 Home-page: https://github.com/DevelopersToolbox/check-prerequisite-package
 Author: Wolf Software
 Author-email: pypi@wolfsoftware.com
 License: MIT
 Project-URL:  Source, https://github.com/DevelopersToolbox/check-prerequisite-package
 Project-URL:  Tracker, https://github.com/DevelopersToolbox/check-prerequisite-package/issues/
@@ -94,15 +94,15 @@
 
 prerequisites: list[str] = ["python", "git"]
 
 try:
     command_paths: dict = check_prerequisite(prerequisites)
 except PrerequisiteCheckError as err:
     print("Prerequisite check failed:")
-    for error in e.errors:
+    for error in err.errors:
         print(error)
     sys.exit(0)
 
 print(command_paths['python'])
 ```
 
 Once the checks have completed, you now have a dict of commands and their associated paths which you can then utilise to ensure you are executing
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wolfsoftware.prereqs Version: 0.1.0 Summary: Check
+Metadata-Version: 2.1 Name: wolfsoftware.prereqs Version: 0.1.1 Summary: Check
 for the presence of prerequisite commands and returns their paths. Home-page:
 https://github.com/DevelopersToolbox/check-prerequisite-package Author: Wolf
 Software Author-email: pypi@wolfsoftware.com License: MIT Project-URL: Source,
 https://github.com/DevelopersToolbox/check-prerequisite-package Project-URL:
 Tracker, https://github.com/DevelopersToolbox/check-prerequisite-package/
 issues/ Project-URL: Documentation, https://github.com/DevelopersToolbox/check-
 prerequisite-package Project-URL: Sponsor, https://github.com/sponsors/
@@ -32,14 +32,14 @@
 package assist with that problem by taking a list of commands that must be
 installed and available and verifies that list at the start to ensure all of
 them are available. ## Installation ```shell pip install wolfsoftware.prereqs
 ``` ## Usage ```python import sys from wolfsoftware.prereqs import
 check_prerequisite, PrerequisiteCheckError prerequisites: list[str] =
 ["python", "git"] try: command_paths: dict = check_prerequisite(prerequisites)
 except PrerequisiteCheckError as err: print("Prerequisite check failed:") for
-error in e.errors: print(error) sys.exit(0) print(command_paths['python']) ```
-Once the checks have completed, you now have a dict of commands and their
+error in err.errors: print(error) sys.exit(0) print(command_paths['python'])
+``` Once the checks have completed, you now have a dict of commands and their
 associated paths which you can then utilise to ensure you are executing your
 subprocesses with the full path.
                                                  _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/
    _C_r_e_a_t_e_d_%_2_0_b_y_%_2_0_W_o_l_f_%_2_0_o_n_%_2_0_b_e_h_a_l_f_%_2_0_o_f_%_2_0_W_o_l_f_%_2_0_S_o_f_t_w_a_r_e_-_b_l_u_e_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-
                                                                          _b_a_d_g_e_]
```

