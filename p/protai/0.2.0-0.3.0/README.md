# Comparing `tmp/protai-0.2.0.tar.gz` & `tmp/protai-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "protai-0.2.0.tar", last modified: Thu May 23 14:30:47 2024, max compression
+gzip compressed data, was "protai-0.3.0.tar", last modified: Thu May 23 14:32:56 2024, max compression
```

## Comparing `protai-0.2.0.tar` & `protai-0.3.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 14:30:47.579933 protai-0.2.0/
--rw-rw-rw-   0        0        0     1479 2024-05-23 14:30:47.578933 protai-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0      828 2024-05-17 06:24:20.000000 protai-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-23 14:30:47.560903 protai-0.2.0/protai/
--rw-rw-rw-   0        0        0        5 2024-05-23 14:30:37.000000 protai-0.2.0/protai/VERSION
--rw-rw-rw-   0        0        0       69 2024-05-22 20:52:15.000000 protai-0.2.0/protai/__init__.py
--rw-rw-rw-   0        0        0     4469 2024-05-23 14:23:52.000000 protai-0.2.0/protai/auth.py
--rw-rw-rw-   0        0        0     2345 2024-05-23 14:19:00.000000 protai-0.2.0/protai/protai.py
-drwxrwxrwx   0        0        0        0 2024-05-23 14:30:47.577933 protai-0.2.0/protai.egg-info/
--rw-rw-rw-   0        0        0     1479 2024-05-23 14:30:47.000000 protai-0.2.0/protai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      266 2024-05-23 14:30:47.000000 protai-0.2.0/protai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 14:30:47.000000 protai-0.2.0/protai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2024-05-23 14:30:47.000000 protai-0.2.0/protai.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       50 2024-05-23 14:30:47.000000 protai-0.2.0/protai.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-23 14:30:47.000000 protai-0.2.0/protai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-23 14:30:47.579933 protai-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0     4178 2024-05-17 06:22:19.000000 protai-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 14:32:56.113078 protai-0.3.0/
+-rw-rw-rw-   0        0        0     1479 2024-05-23 14:32:56.113078 protai-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0      828 2024-05-17 06:24:20.000000 protai-0.3.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-23 14:32:56.092896 protai-0.3.0/protai/
+-rw-rw-rw-   0        0        0        5 2024-05-23 14:32:24.000000 protai-0.3.0/protai/VERSION
+-rw-rw-rw-   0        0        0       69 2024-05-22 20:52:15.000000 protai-0.3.0/protai/__init__.py
+-rw-rw-rw-   0        0        0     4469 2024-05-23 14:23:52.000000 protai-0.3.0/protai/auth.py
+-rw-rw-rw-   0        0        0     2345 2024-05-23 14:19:00.000000 protai-0.3.0/protai/protai.py
+drwxrwxrwx   0        0        0        0 2024-05-23 14:32:56.111076 protai-0.3.0/protai.egg-info/
+-rw-rw-rw-   0        0        0     1479 2024-05-23 14:32:56.000000 protai-0.3.0/protai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      266 2024-05-23 14:32:56.000000 protai-0.3.0/protai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 14:32:56.000000 protai-0.3.0/protai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2024-05-23 14:32:56.000000 protai-0.3.0/protai.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       50 2024-05-23 14:32:56.000000 protai-0.3.0/protai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-23 14:32:56.000000 protai-0.3.0/protai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-23 14:32:56.114076 protai-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     4178 2024-05-17 06:22:19.000000 protai-0.3.0/setup.py
```

### Comparing `protai-0.2.0/PKG-INFO` & `protai-0.3.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: protai
-Version: 0.2.0
+Version: 0.3.0
 Summary: A useful 0-Shot AI in the terminal
 Home-page: https://github.com/protik09/terminal-ai
 Author: Protik Banerji
 Author-email: protik09@users.noreply.github.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `protai-0.2.0/README.md` & `protai-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `protai-0.2.0/protai/auth.py` & `protai-0.3.0/protai/auth.py`

 * *Files identical despite different names*

### Comparing `protai-0.2.0/protai/protai.py` & `protai-0.3.0/protai/protai.py`

 * *Files identical despite different names*

### Comparing `protai-0.2.0/protai.egg-info/PKG-INFO` & `protai-0.3.0/protai.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: protai
-Version: 0.2.0
+Version: 0.3.0
 Summary: A useful 0-Shot AI in the terminal
 Home-page: https://github.com/protik09/terminal-ai
 Author: Protik Banerji
 Author-email: protik09@users.noreply.github.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `protai-0.2.0/setup.py` & `protai-0.3.0/setup.py`

 * *Files identical despite different names*

