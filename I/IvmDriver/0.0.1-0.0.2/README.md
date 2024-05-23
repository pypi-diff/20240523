# Comparing `tmp/IvmDriver-0.0.1.tar.gz` & `tmp/IvmDriver-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IvmDriver-0.0.1.tar", last modified: Thu May 23 10:00:40 2024, max compression
+gzip compressed data, was "IvmDriver-0.0.2.tar", last modified: Thu May 23 10:16:45 2024, max compression
```

## Comparing `IvmDriver-0.0.1.tar` & `IvmDriver-0.0.2.tar`

### file list

```diff
@@ -1,10 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 10:00:40.867292 IvmDriver-0.0.1/
-drwxrwxrwx   0        0        0        0 2024-05-23 10:00:40.860881 IvmDriver-0.0.1/IvmDriver.egg-info/
--rw-rw-rw-   0        0        0      637 2024-05-23 10:00:40.000000 IvmDriver-0.0.1/IvmDriver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      150 2024-05-23 10:00:40.000000 IvmDriver-0.0.1/IvmDriver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 10:00:40.000000 IvmDriver-0.0.1/IvmDriver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-05-23 10:00:40.000000 IvmDriver-0.0.1/IvmDriver.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      637 2024-05-23 10:00:40.862987 IvmDriver-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      310 2024-05-23 09:25:33.000000 IvmDriver-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2024-05-23 10:00:40.867797 IvmDriver-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      838 2024-05-23 10:00:20.000000 IvmDriver-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 10:16:45.164339 IvmDriver-0.0.2/
+drwxrwxrwx   0        0        0        0 2024-05-23 10:16:45.142372 IvmDriver-0.0.2/IvmDriver/
+-rw-rw-rw-   0        0        0      339 2024-05-23 10:14:37.000000 IvmDriver-0.0.2/IvmDriver/Matrixgui.py
+-rw-rw-rw-   0        0        0      179 2024-05-23 10:16:39.000000 IvmDriver-0.0.2/IvmDriver/__init__.py
+-rw-rw-rw-   0        0        0    10640 2024-05-07 10:48:18.000000 IvmDriver-0.0.2/IvmDriver/driver.py
+-rw-rw-rw-   0        0        0        0 2024-05-02 13:19:09.000000 IvmDriver-0.0.2/IvmDriver/driverPage.py
+-rw-rw-rw-   0        0        0      552 2024-05-08 11:50:37.000000 IvmDriver-0.0.2/IvmDriver/exeGenerate.py
+-rw-rw-rw-   0        0        0     6451 2024-05-07 09:19:54.000000 IvmDriver-0.0.2/IvmDriver/fileopen.py
+-rw-rw-rw-   0        0        0     1104 2024-05-07 14:46:01.000000 IvmDriver-0.0.2/IvmDriver/logger.py
+-rw-rw-rw-   0        0        0    78821 2024-05-07 10:46:12.000000 IvmDriver-0.0.2/IvmDriver/matrix.py
+-rw-rw-rw-   0        0        0     4607 2024-05-23 10:14:52.000000 IvmDriver-0.0.2/IvmDriver/matrixDriver.py
+-rw-rw-rw-   0        0        0     1069 2024-04-30 13:44:36.000000 IvmDriver-0.0.2/IvmDriver/mcp2221.py
+-rw-rw-rw-   0        0        0     3747 2024-04-30 14:24:47.000000 IvmDriver-0.0.2/IvmDriver/mcp2317.py
+-rw-rw-rw-   0        0        0     3986 2024-05-06 09:00:54.000000 IvmDriver-0.0.2/IvmDriver/signalRoot.py
+drwxrwxrwx   0        0        0        0 2024-05-23 10:16:45.158623 IvmDriver-0.0.2/IvmDriver.egg-info/
+-rw-rw-rw-   0        0        0      637 2024-05-23 10:16:44.000000 IvmDriver-0.0.2/IvmDriver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      418 2024-05-23 10:16:45.000000 IvmDriver-0.0.2/IvmDriver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 10:16:44.000000 IvmDriver-0.0.2/IvmDriver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-05-23 10:16:44.000000 IvmDriver-0.0.2/IvmDriver.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      637 2024-05-23 10:16:45.161038 IvmDriver-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      310 2024-05-23 09:25:33.000000 IvmDriver-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-23 10:16:45.165051 IvmDriver-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      875 2024-05-23 10:15:35.000000 IvmDriver-0.0.2/setup.py
```

### Comparing `IvmDriver-0.0.1/IvmDriver.egg-info/PKG-INFO` & `IvmDriver-0.0.2/IvmDriver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IvmDriver
-Version: 0.0.1
+Version: 0.0.2
 Home-page: https://github.com/HarishKumarSedu/matrix
 Author: HarishKumarSedu
 Author-email: harishkumarsedu@gmail.com
 Project-URL: Bug Tracker, https://github.com/HarishKumarSedu/matrix/issues
 Description-Content-Type: ['text/plain', 'text/x-rst', 'text/markdown']
 
 # Driver
```

### Comparing `IvmDriver-0.0.1/PKG-INFO` & `IvmDriver-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IvmDriver
-Version: 0.0.1
+Version: 0.0.2
 Home-page: https://github.com/HarishKumarSedu/matrix
 Author: HarishKumarSedu
 Author-email: harishkumarsedu@gmail.com
 Project-URL: Bug Tracker, https://github.com/HarishKumarSedu/matrix/issues
 Description-Content-Type: ['text/plain', 'text/x-rst', 'text/markdown']
 
 # Driver
```

### Comparing `IvmDriver-0.0.1/setup.py` & `IvmDriver-0.0.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,23 +5,24 @@
 AUTHOR_USER_NAME = 'HarishKumarSedu'
 AUTHOR_EMAIL = 'harishkumarsedu@gmail.com'
 REPO_NAME = 'matrix'
 setup(
     name=f'IvmDriver',
     author=AUTHOR_USER_NAME,
     author_email=AUTHOR_EMAIL,
-    version='0.0.1',
-    py_modules=['*'],
+    version='0.0.2',
+    # py_modules=['src'],
     # description=[ 'text/markdown','text/x-rst'],
     url=f"https://github.com/{AUTHOR_USER_NAME}/{REPO_NAME}",
     project_urls={
         "Bug Tracker": f"https://github.com/{AUTHOR_USER_NAME}/{REPO_NAME}/issues",
     },
     long_description_content_type=['text/plain', 'text/x-rst', 'text/markdown'],
     long_description=long_description,
     packages=find_packages(),
     package_data={'': ['*.json','*.py']},
     include_package_data=True,
+    include_dirs=['IvmDriver'],
 
     
     
 )
```

