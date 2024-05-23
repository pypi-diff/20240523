# Comparing `tmp/testwizard.commands-core-3.8.1b4749.tar.gz` & `tmp/testwizard.commands-core-3.8.1b4810.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testwizard.commands-core-3.8.1b4749.tar", last modified: Tue Mar 19 15:01:38 2024, max compression
+gzip compressed data, was "testwizard.commands-core-3.8.1b4810.tar", last modified: Wed Mar 27 12:56:25 2024, max compression
```

## Comparing `testwizard.commands-core-3.8.1b4749.tar` & `testwizard.commands-core-3.8.1b4810.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-03-19 15:01:38.881111 testwizard.commands-core-3.8.1b4749/
--rw-rw-rw-   0        0        0        4 2024-03-19 15:00:53.000000 testwizard.commands-core-3.8.1b4749/LICENSE.txt
--rw-rw-rw-   0        0        0      554 2024-03-19 15:01:38.881111 testwizard.commands-core-3.8.1b4749/PKG-INFO
--rw-rw-rw-   0        0        0        4 2024-03-19 15:00:53.000000 testwizard.commands-core-3.8.1b4749/README.md
--rw-rw-rw-   0        0        0       42 2024-03-19 15:01:38.881111 testwizard.commands-core-3.8.1b4749/setup.cfg
--rw-rw-rw-   0        0        0      837 2024-03-19 15:01:38.000000 testwizard.commands-core-3.8.1b4749/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-19 15:01:38.865488 testwizard.commands-core-3.8.1b4749/testwizard/
-drwxrwxrwx   0        0        0        0 2024-03-19 15:01:38.881111 testwizard.commands-core-3.8.1b4749/testwizard/commands_core/
--rw-rw-rw-   0        0        0      526 2024-03-19 15:00:53.000000 testwizard.commands-core-3.8.1b4749/testwizard/commands_core/CommandBase.py
--rw-rw-rw-   0        0        0      665 2024-03-19 15:00:53.000000 testwizard.commands-core-3.8.1b4749/testwizard/commands_core/OkErrorCodeAndMessageResult.py
--rw-rw-rw-   0        0        0      240 2024-03-19 15:00:53.000000 testwizard.commands-core-3.8.1b4749/testwizard/commands_core/OkResult.py
--rw-rw-rw-   0        0        0     1387 2024-03-19 15:00:53.000000 testwizard.commands-core-3.8.1b4749/testwizard/commands_core/ResultBase.py
--rw-rw-rw-   0        0        0      560 2024-03-19 15:00:53.000000 testwizard.commands-core-3.8.1b4749/testwizard/commands_core/SessionCommandBase.py
--rw-rw-rw-   0        0        0      334 2024-03-19 15:00:53.000000 testwizard.commands-core-3.8.1b4749/testwizard/commands_core/SimpleResult.py
--rw-rw-rw-   0        0        0      268 2024-03-19 15:00:53.000000 testwizard.commands-core-3.8.1b4749/testwizard/commands_core/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-19 15:01:38.881111 testwizard.commands-core-3.8.1b4749/testwizard.commands_core.egg-info/
--rw-rw-rw-   0        0        0      554 2024-03-19 15:01:38.000000 testwizard.commands-core-3.8.1b4749/testwizard.commands_core.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      519 2024-03-19 15:01:38.000000 testwizard.commands-core-3.8.1b4749/testwizard.commands_core.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-19 15:01:38.000000 testwizard.commands-core-3.8.1b4749/testwizard.commands_core.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-03-19 15:01:38.000000 testwizard.commands-core-3.8.1b4749/testwizard.commands_core.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-03-27 12:56:25.520108 testwizard.commands-core-3.8.1b4810/
+-rw-rw-rw-   0        0        0        4 2024-03-27 12:55:37.000000 testwizard.commands-core-3.8.1b4810/LICENSE.txt
+-rw-rw-rw-   0        0        0      554 2024-03-27 12:56:25.520108 testwizard.commands-core-3.8.1b4810/PKG-INFO
+-rw-rw-rw-   0        0        0        4 2024-03-27 12:55:37.000000 testwizard.commands-core-3.8.1b4810/README.md
+-rw-rw-rw-   0        0        0       42 2024-03-27 12:56:25.520108 testwizard.commands-core-3.8.1b4810/setup.cfg
+-rw-rw-rw-   0        0        0      837 2024-03-27 12:56:25.000000 testwizard.commands-core-3.8.1b4810/setup.py
+drwxrwxrwx   0        0        0        0 2024-03-27 12:56:25.520108 testwizard.commands-core-3.8.1b4810/testwizard/
+drwxrwxrwx   0        0        0        0 2024-03-27 12:56:25.520108 testwizard.commands-core-3.8.1b4810/testwizard/commands_core/
+-rw-rw-rw-   0        0        0      526 2024-03-27 12:55:37.000000 testwizard.commands-core-3.8.1b4810/testwizard/commands_core/CommandBase.py
+-rw-rw-rw-   0        0        0      665 2024-03-27 12:55:37.000000 testwizard.commands-core-3.8.1b4810/testwizard/commands_core/OkErrorCodeAndMessageResult.py
+-rw-rw-rw-   0        0        0      240 2024-03-27 12:55:37.000000 testwizard.commands-core-3.8.1b4810/testwizard/commands_core/OkResult.py
+-rw-rw-rw-   0        0        0     1387 2024-03-27 12:55:37.000000 testwizard.commands-core-3.8.1b4810/testwizard/commands_core/ResultBase.py
+-rw-rw-rw-   0        0        0      560 2024-03-27 12:55:37.000000 testwizard.commands-core-3.8.1b4810/testwizard/commands_core/SessionCommandBase.py
+-rw-rw-rw-   0        0        0      334 2024-03-27 12:55:37.000000 testwizard.commands-core-3.8.1b4810/testwizard/commands_core/SimpleResult.py
+-rw-rw-rw-   0        0        0      268 2024-03-27 12:55:37.000000 testwizard.commands-core-3.8.1b4810/testwizard/commands_core/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-27 12:56:25.520108 testwizard.commands-core-3.8.1b4810/testwizard.commands_core.egg-info/
+-rw-rw-rw-   0        0        0      554 2024-03-27 12:56:25.000000 testwizard.commands-core-3.8.1b4810/testwizard.commands_core.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      519 2024-03-27 12:56:25.000000 testwizard.commands-core-3.8.1b4810/testwizard.commands_core.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-03-27 12:56:25.000000 testwizard.commands-core-3.8.1b4810/testwizard.commands_core.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-03-27 12:56:25.000000 testwizard.commands-core-3.8.1b4810/testwizard.commands_core.egg-info/top_level.txt
```

### Comparing `testwizard.commands-core-3.8.1b4749/PKG-INFO` & `testwizard.commands-core-3.8.1b4810/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testwizard.commands-core
-Version: 3.8.1b4749
+Version: 3.8.1b4810
 Summary: Testwizard core components for commands
 Home-page: https://www.resillion.com/services/software-testing/testing-tools/testwizard/
 Author: Resillion
 Author-email: testwizard-support@resillion.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.3
```

### Comparing `testwizard.commands-core-3.8.1b4749/testwizard/commands_core/CommandBase.py` & `testwizard.commands-core-3.8.1b4810/testwizard/commands_core/CommandBase.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-core-3.8.1b4749/testwizard/commands_core/OkErrorCodeAndMessageResult.py` & `testwizard.commands-core-3.8.1b4810/testwizard/commands_core/OkErrorCodeAndMessageResult.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-core-3.8.1b4749/testwizard/commands_core/ResultBase.py` & `testwizard.commands-core-3.8.1b4810/testwizard/commands_core/ResultBase.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-core-3.8.1b4749/testwizard/commands_core/SessionCommandBase.py` & `testwizard.commands-core-3.8.1b4810/testwizard/commands_core/SessionCommandBase.py`

 * *Files identical despite different names*

### Comparing `testwizard.commands-core-3.8.1b4749/testwizard.commands_core.egg-info/PKG-INFO` & `testwizard.commands-core-3.8.1b4810/testwizard.commands_core.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testwizard.commands-core
-Version: 3.8.1b4749
+Version: 3.8.1b4810
 Summary: Testwizard core components for commands
 Home-page: https://www.resillion.com/services/software-testing/testing-tools/testwizard/
 Author: Resillion
 Author-email: testwizard-support@resillion.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.3
```

### Comparing `testwizard.commands-core-3.8.1b4749/testwizard.commands_core.egg-info/SOURCES.txt` & `testwizard.commands-core-3.8.1b4810/testwizard.commands_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

