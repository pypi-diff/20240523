# Comparing `tmp/yplib-5.8.1.tar.gz` & `tmp/yplib-5.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yplib-5.8.1.tar", last modified: Tue May 21 08:18:07 2024, max compression
+gzip compressed data, was "yplib-5.8.2.tar", last modified: Thu May 23 06:33:54 2024, max compression
```

## Comparing `yplib-5.8.1.tar` & `yplib-5.8.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 08:18:07.871639 yplib-5.8.1/
--rw-rw-rw-   0        0        0     1091 2023-06-13 07:19:46.000000 yplib-5.8.1/LICENSE
--rw-rw-rw-   0        0        0      355 2024-05-21 08:18:07.871639 yplib-5.8.1/PKG-INFO
--rw-rw-rw-   0        0        0       16 2024-03-15 03:58:27.000000 yplib-5.8.1/README.md
--rw-rw-rw-   0        0        0       42 2024-05-21 08:18:07.871639 yplib-5.8.1/setup.cfg
--rw-rw-rw-   0        0        0      555 2024-05-21 08:17:47.000000 yplib-5.8.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-21 08:18:07.856614 yplib-5.8.1/yplib/
--rw-rw-rw-   0        0        0      682 2024-05-07 06:14:01.000000 yplib-5.8.1/yplib/__init__.py
--rw-rw-rw-   0        0        0    15069 2023-12-21 10:38:44.000000 yplib-5.8.1/yplib/chart.py
--rw-rw-rw-   0        0        0    14692 2023-12-21 10:38:44.000000 yplib-5.8.1/yplib/chart_html.py
--rw-rw-rw-   0        0        0    12750 2024-05-21 08:16:54.000000 yplib-5.8.1/yplib/db.py
--rw-rw-rw-   0        0        0     6183 2024-04-15 04:13:53.000000 yplib-5.8.1/yplib/file.py
--rw-rw-rw-   0        0        0     7361 2024-05-16 07:20:59.000000 yplib-5.8.1/yplib/http_util.py
--rw-rw-rw-   0        0        0    41438 2024-05-08 04:02:59.000000 yplib-5.8.1/yplib/index.py
--rw-rw-rw-   0        0        0     6687 2024-03-14 06:15:59.000000 yplib-5.8.1/yplib/mail.py
--rw-rw-rw-   0        0        0     3881 2023-06-30 08:05:11.000000 yplib-5.8.1/yplib/mail_html.py
--rw-rw-rw-   0        0        0     5417 2023-07-03 02:25:38.000000 yplib-5.8.1/yplib/markdown.py
--rw-rw-rw-   0        0        0     2246 2024-05-21 08:16:59.000000 yplib-5.8.1/yplib/multi_thread.py
--rw-rw-rw-   0        0        0      124 2023-06-25 08:17:46.000000 yplib-5.8.1/yplib/temp.py
-drwxrwxrwx   0        0        0        0 2024-05-21 08:18:07.871639 yplib-5.8.1/yplib.egg-info/
--rw-rw-rw-   0        0        0      355 2024-05-21 08:18:07.000000 yplib-5.8.1/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      342 2024-05-21 08:18:07.000000 yplib-5.8.1/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 08:18:07.000000 yplib-5.8.1/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-05-21 08:18:07.000000 yplib-5.8.1/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-23 06:33:54.595493 yplib-5.8.2/
+-rw-rw-rw-   0        0        0     1091 2023-06-13 07:19:46.000000 yplib-5.8.2/LICENSE
+-rw-rw-rw-   0        0        0      355 2024-05-23 06:33:54.595493 yplib-5.8.2/PKG-INFO
+-rw-rw-rw-   0        0        0       16 2024-03-15 03:58:27.000000 yplib-5.8.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-23 06:33:54.595493 yplib-5.8.2/setup.cfg
+-rw-rw-rw-   0        0        0      555 2024-05-23 06:33:45.000000 yplib-5.8.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 06:33:54.580489 yplib-5.8.2/yplib/
+-rw-rw-rw-   0        0        0      682 2024-05-07 06:14:01.000000 yplib-5.8.2/yplib/__init__.py
+-rw-rw-rw-   0        0        0    15069 2023-12-21 10:38:44.000000 yplib-5.8.2/yplib/chart.py
+-rw-rw-rw-   0        0        0    14692 2023-12-21 10:38:44.000000 yplib-5.8.2/yplib/chart_html.py
+-rw-rw-rw-   0        0        0    12733 2024-05-22 09:54:48.000000 yplib-5.8.2/yplib/db.py
+-rw-rw-rw-   0        0        0     6183 2024-04-15 04:13:53.000000 yplib-5.8.2/yplib/file.py
+-rw-rw-rw-   0        0        0     7361 2024-05-16 07:20:59.000000 yplib-5.8.2/yplib/http_util.py
+-rw-rw-rw-   0        0        0    41619 2024-05-23 06:33:40.000000 yplib-5.8.2/yplib/index.py
+-rw-rw-rw-   0        0        0     6687 2024-03-14 06:15:59.000000 yplib-5.8.2/yplib/mail.py
+-rw-rw-rw-   0        0        0     3881 2023-06-30 08:05:11.000000 yplib-5.8.2/yplib/mail_html.py
+-rw-rw-rw-   0        0        0     5417 2023-07-03 02:25:38.000000 yplib-5.8.2/yplib/markdown.py
+-rw-rw-rw-   0        0        0     2246 2024-05-21 08:16:59.000000 yplib-5.8.2/yplib/multi_thread.py
+-rw-rw-rw-   0        0        0      124 2023-06-25 08:17:46.000000 yplib-5.8.2/yplib/temp.py
+drwxrwxrwx   0        0        0        0 2024-05-23 06:33:54.595493 yplib-5.8.2/yplib.egg-info/
+-rw-rw-rw-   0        0        0      355 2024-05-23 06:33:54.000000 yplib-5.8.2/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      342 2024-05-23 06:33:54.000000 yplib-5.8.2/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 06:33:54.000000 yplib-5.8.2/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-05-23 06:33:54.000000 yplib-5.8.2/yplib.egg-info/top_level.txt
```

### Comparing `yplib-5.8.1/LICENSE` & `yplib-5.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-5.8.1/setup.py` & `yplib-5.8.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="yplib",
-    version="5.8.1",
+    version="5.8.2",
     author="yangpu",
     author_email="wantwaterfish@gmail.com",
     description="util",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
```

### Comparing `yplib-5.8.1/yplib/__init__.py` & `yplib-5.8.2/yplib/__init__.py`

 * *Files identical despite different names*

### Comparing `yplib-5.8.1/yplib/chart.py` & `yplib-5.8.2/yplib/chart.py`

 * *Files identical despite different names*

### Comparing `yplib-5.8.1/yplib/chart_html.py` & `yplib-5.8.2/yplib/chart_html.py`

 * *Files identical despite different names*

### Comparing `yplib-5.8.1/yplib/db.py` & `yplib-5.8.2/yplib/db.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import json
 
 from yplib.index import *
 from yplib.http_util import *
 import pymysql
 import adbc_driver_manager
 import adbc_driver_flightsql.dbapi as flight_sql
-import warnings
 
 import threading
 
 # 创建一个线程本地存储对象
 thread_local = threading.local()
```

### Comparing `yplib-5.8.1/yplib/file.py` & `yplib-5.8.2/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-5.8.1/yplib/http_util.py` & `yplib-5.8.2/yplib/http_util.py`

 * *Files identical despite different names*

### Comparing `yplib-5.8.1/yplib/index.py` & `yplib-5.8.2/yplib/index.py`

 * *Files 2% similar despite different names*

```diff
@@ -970,17 +970,20 @@
     if data is None:
         data = {}
     set_data_in_user_home(file_name, data)
 
 
 # 从 config 中获得 配置数据
 def get_config_data(file_name='config'):
+    print('get_config_data', file_name)
     config_data = get_data_from_user_home(file_name)
+    print('get_data_from_user_home', config_data)
     if not config_data:
         config_data = get_data_from_path(file_name)
+    print('get_data_from_path', config_data)
     return config_data
 
 
 # 在当前用户的主目录中, 获得指定文件的数据
 def get_data_from_user_home(file_name='config'):
     return get_data_from_path(file_name, os.path.expanduser("~"))
 
@@ -996,14 +999,15 @@
 def get_data_from_path(file_name='config', file_path=None):
     config_path = file_path + '/' + CONFIG_PATH if file_path else CONFIG_PATH
     if not os.path.exists(config_path):
         config_path = file_path + '/' + CONFIG_PATH_BAK if file_path else CONFIG_PATH_BAK
     file_path = config_path + '/' + file_name + '.json'
     if not os.path.exists(file_path):
         return {}
+    print('to_json_from_file', file_path)
     return to_json_from_file(file_path)
 
 
 # 在当前的目录中, 设置数据到指定路径下
 def set_data_in_path(file_name='config', data=None, file_path=''):
     if data is None:
         data = {}
```

### Comparing `yplib-5.8.1/yplib/mail.py` & `yplib-5.8.2/yplib/mail.py`

 * *Files identical despite different names*

### Comparing `yplib-5.8.1/yplib/mail_html.py` & `yplib-5.8.2/yplib/mail_html.py`

 * *Files identical despite different names*

### Comparing `yplib-5.8.1/yplib/markdown.py` & `yplib-5.8.2/yplib/markdown.py`

 * *Files identical despite different names*

### Comparing `yplib-5.8.1/yplib/multi_thread.py` & `yplib-5.8.2/yplib/multi_thread.py`

 * *Files identical despite different names*

