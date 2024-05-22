# Comparing `tmp/agrc-supervisor-3.0.3.tar.gz` & `tmp/agrc-supervisor-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agrc-supervisor-3.0.3.tar", last modified: Wed May 22 22:35:46 2024, max compression
+gzip compressed data, was "agrc-supervisor-3.1.0.tar", last modified: Wed May 22 19:06:16 2024, max compression
```

## Comparing `agrc-supervisor-3.0.3.tar` & `agrc-supervisor-3.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:35:46.499389 agrc-supervisor-3.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-22 22:35:43.000000 agrc-supervisor-3.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-22 22:35:46.499389 agrc-supervisor-3.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5528 2024-05-22 22:35:43.000000 agrc-supervisor-3.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-22 22:35:46.499389 agrc-supervisor-3.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-05-22 22:35:43.000000 agrc-supervisor-3.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:35:46.495389 agrc-supervisor-3.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:35:46.495389 agrc-supervisor-3.0.3/src/agrc_supervisor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-22 22:35:46.000000 agrc-supervisor-3.0.3/src/agrc_supervisor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-22 22:35:46.000000 agrc-supervisor-3.0.3/src/agrc_supervisor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 22:35:46.000000 agrc-supervisor-3.0.3/src/agrc_supervisor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-22 22:35:46.000000 agrc-supervisor-3.0.3/src/agrc_supervisor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-22 22:35:46.000000 agrc-supervisor-3.0.3/src/agrc_supervisor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 22:35:46.000000 agrc-supervisor-3.0.3/src/agrc_supervisor.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:35:46.499389 agrc-supervisor-3.0.3/src/supervisor/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-22 22:35:43.000000 agrc-supervisor-3.0.3/src/supervisor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-05-22 22:35:43.000000 agrc-supervisor-3.0.3/src/supervisor/example.py
--rw-r--r--   0 runner    (1001) docker     (127)    15841 2024-05-22 22:35:43.000000 agrc-supervisor-3.0.3/src/supervisor/message_handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4255 2024-05-22 22:35:43.000000 agrc-supervisor-3.0.3/src/supervisor/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-22 22:35:43.000000 agrc-supervisor-3.0.3/src/supervisor/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:06:16.848972 agrc-supervisor-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-22 19:06:13.000000 agrc-supervisor-3.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-22 19:06:16.848972 agrc-supervisor-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5528 2024-05-22 19:06:13.000000 agrc-supervisor-3.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-22 19:06:16.848972 agrc-supervisor-3.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-05-22 19:06:13.000000 agrc-supervisor-3.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:06:16.844972 agrc-supervisor-3.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:06:16.848972 agrc-supervisor-3.1.0/src/agrc_supervisor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-22 19:06:16.000000 agrc-supervisor-3.1.0/src/agrc_supervisor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-22 19:06:16.000000 agrc-supervisor-3.1.0/src/agrc_supervisor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 19:06:16.000000 agrc-supervisor-3.1.0/src/agrc_supervisor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-22 19:06:16.000000 agrc-supervisor-3.1.0/src/agrc_supervisor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-22 19:06:16.000000 agrc-supervisor-3.1.0/src/agrc_supervisor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 19:06:16.000000 agrc-supervisor-3.1.0/src/agrc_supervisor.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:06:16.848972 agrc-supervisor-3.1.0/src/supervisor/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-22 19:06:13.000000 agrc-supervisor-3.1.0/src/supervisor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-05-22 19:06:13.000000 agrc-supervisor-3.1.0/src/supervisor/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15841 2024-05-22 19:06:13.000000 agrc-supervisor-3.1.0/src/supervisor/message_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4255 2024-05-22 19:06:13.000000 agrc-supervisor-3.1.0/src/supervisor/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-22 19:06:13.000000 agrc-supervisor-3.1.0/src/supervisor/version.py
```

### Comparing `agrc-supervisor-3.0.3/LICENSE` & `agrc-supervisor-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `agrc-supervisor-3.0.3/PKG-INFO` & `agrc-supervisor-3.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agrc-supervisor
-Version: 3.0.3
+Version: 3.1.0
 Summary: A watchdog module for scheduled scripts that sends notifications, including any uncaught exceptions.
 Home-page: https://github.com/agrc/supervisor
 Author: Jake Adams, UGRC
 Author-email: jdadams@utah.gov
 License: MIT
 Project-URL: Issue Tracker, https://github.com/agrc/supervisor/issues
 Keywords: gis
```

### Comparing `agrc-supervisor-3.0.3/README.md` & `agrc-supervisor-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `agrc-supervisor-3.0.3/setup.cfg` & `agrc-supervisor-3.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `agrc-supervisor-3.0.3/setup.py` & `agrc-supervisor-3.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,16 +33,16 @@
         'Topic :: Utilities',
     ],
     project_urls={
         'Issue Tracker': 'https://github.com/agrc/supervisor/issues',
     },
     keywords=['gis'],
     install_requires=[
-        'requests~=2.31',
-        'sendgrid~=6.10',
+        'requests~=2.32',
+        'sendgrid~=6.11',
     ],
     extras_require={
         'tests': [
             'pylint-quotes~=0.2',
             'pylint>=2.17,<4.0',
             'pytest-cov>=4.1,<6.0',
             'pytest-instafail~=0.5',
```

### Comparing `agrc-supervisor-3.0.3/src/agrc_supervisor.egg-info/PKG-INFO` & `agrc-supervisor-3.1.0/src/agrc_supervisor.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agrc-supervisor
-Version: 3.0.3
+Version: 3.1.0
 Summary: A watchdog module for scheduled scripts that sends notifications, including any uncaught exceptions.
 Home-page: https://github.com/agrc/supervisor
 Author: Jake Adams, UGRC
 Author-email: jdadams@utah.gov
 License: MIT
 Project-URL: Issue Tracker, https://github.com/agrc/supervisor/issues
 Keywords: gis
```

### Comparing `agrc-supervisor-3.0.3/src/supervisor/example.py` & `agrc-supervisor-3.1.0/src/supervisor/example.py`

 * *Files identical despite different names*

### Comparing `agrc-supervisor-3.0.3/src/supervisor/message_handlers.py` & `agrc-supervisor-3.1.0/src/supervisor/message_handlers.py`

 * *Files identical despite different names*

### Comparing `agrc-supervisor-3.0.3/src/supervisor/models.py` & `agrc-supervisor-3.1.0/src/supervisor/models.py`

 * *Files identical despite different names*

