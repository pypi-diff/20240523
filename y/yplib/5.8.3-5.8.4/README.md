# Comparing `tmp/yplib-5.8.3.tar.gz` & `tmp/yplib-5.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yplib-5.8.3.tar", last modified: Thu May 23 06:36:21 2024, max compression
+gzip compressed data, was "yplib-5.8.4.tar", last modified: Thu May 23 06:44:21 2024, max compression
```

## Comparing `yplib-5.8.3.tar` & `yplib-5.8.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 06:36:21.563460 yplib-5.8.3/
--rw-rw-rw-   0        0        0     1091 2023-06-13 07:19:46.000000 yplib-5.8.3/LICENSE
--rw-rw-rw-   0        0        0      355 2024-05-23 06:36:21.562451 yplib-5.8.3/PKG-INFO
--rw-rw-rw-   0        0        0       16 2024-03-15 03:58:27.000000 yplib-5.8.3/README.md
--rw-rw-rw-   0        0        0       42 2024-05-23 06:36:21.563460 yplib-5.8.3/setup.cfg
--rw-rw-rw-   0        0        0      555 2024-05-23 06:36:10.000000 yplib-5.8.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-23 06:36:21.555930 yplib-5.8.3/yplib/
--rw-rw-rw-   0        0        0      682 2024-05-07 06:14:01.000000 yplib-5.8.3/yplib/__init__.py
--rw-rw-rw-   0        0        0    15069 2023-12-21 10:38:44.000000 yplib-5.8.3/yplib/chart.py
--rw-rw-rw-   0        0        0    14692 2023-12-21 10:38:44.000000 yplib-5.8.3/yplib/chart_html.py
--rw-rw-rw-   0        0        0    12733 2024-05-22 09:54:48.000000 yplib-5.8.3/yplib/db.py
--rw-rw-rw-   0        0        0     6183 2024-04-15 04:13:53.000000 yplib-5.8.3/yplib/file.py
--rw-rw-rw-   0        0        0     7361 2024-05-16 07:20:59.000000 yplib-5.8.3/yplib/http_util.py
--rw-rw-rw-   0        0        0    41787 2024-05-23 06:36:06.000000 yplib-5.8.3/yplib/index.py
--rw-rw-rw-   0        0        0     6687 2024-03-14 06:15:59.000000 yplib-5.8.3/yplib/mail.py
--rw-rw-rw-   0        0        0     3881 2023-06-30 08:05:11.000000 yplib-5.8.3/yplib/mail_html.py
--rw-rw-rw-   0        0        0     5417 2023-07-03 02:25:38.000000 yplib-5.8.3/yplib/markdown.py
--rw-rw-rw-   0        0        0     2246 2024-05-21 08:16:59.000000 yplib-5.8.3/yplib/multi_thread.py
--rw-rw-rw-   0        0        0      124 2023-06-25 08:17:46.000000 yplib-5.8.3/yplib/temp.py
-drwxrwxrwx   0        0        0        0 2024-05-23 06:36:21.560928 yplib-5.8.3/yplib.egg-info/
--rw-rw-rw-   0        0        0      355 2024-05-23 06:36:21.000000 yplib-5.8.3/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      342 2024-05-23 06:36:21.000000 yplib-5.8.3/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 06:36:21.000000 yplib-5.8.3/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-05-23 06:36:21.000000 yplib-5.8.3/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-23 06:44:21.932904 yplib-5.8.4/
+-rw-rw-rw-   0        0        0     1091 2023-06-13 07:19:46.000000 yplib-5.8.4/LICENSE
+-rw-rw-rw-   0        0        0      355 2024-05-23 06:44:21.932904 yplib-5.8.4/PKG-INFO
+-rw-rw-rw-   0        0        0       16 2024-03-15 03:58:27.000000 yplib-5.8.4/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-23 06:44:21.932904 yplib-5.8.4/setup.cfg
+-rw-rw-rw-   0        0        0      555 2024-05-23 06:44:08.000000 yplib-5.8.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 06:44:21.917903 yplib-5.8.4/yplib/
+-rw-rw-rw-   0        0        0      682 2024-05-07 06:14:01.000000 yplib-5.8.4/yplib/__init__.py
+-rw-rw-rw-   0        0        0    15069 2023-12-21 10:38:44.000000 yplib-5.8.4/yplib/chart.py
+-rw-rw-rw-   0        0        0    14692 2023-12-21 10:38:44.000000 yplib-5.8.4/yplib/chart_html.py
+-rw-rw-rw-   0        0        0    12733 2024-05-22 09:54:48.000000 yplib-5.8.4/yplib/db.py
+-rw-rw-rw-   0        0        0     6183 2024-04-15 04:13:53.000000 yplib-5.8.4/yplib/file.py
+-rw-rw-rw-   0        0        0     7361 2024-05-16 07:20:59.000000 yplib-5.8.4/yplib/http_util.py
+-rw-rw-rw-   0        0        0    41639 2024-05-23 06:43:35.000000 yplib-5.8.4/yplib/index.py
+-rw-rw-rw-   0        0        0     6687 2024-03-14 06:15:59.000000 yplib-5.8.4/yplib/mail.py
+-rw-rw-rw-   0        0        0     3881 2023-06-30 08:05:11.000000 yplib-5.8.4/yplib/mail_html.py
+-rw-rw-rw-   0        0        0     5417 2023-07-03 02:25:38.000000 yplib-5.8.4/yplib/markdown.py
+-rw-rw-rw-   0        0        0     2246 2024-05-21 08:16:59.000000 yplib-5.8.4/yplib/multi_thread.py
+-rw-rw-rw-   0        0        0      124 2023-06-25 08:17:46.000000 yplib-5.8.4/yplib/temp.py
+drwxrwxrwx   0        0        0        0 2024-05-23 06:44:21.932904 yplib-5.8.4/yplib.egg-info/
+-rw-rw-rw-   0        0        0      355 2024-05-23 06:44:21.000000 yplib-5.8.4/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      342 2024-05-23 06:44:21.000000 yplib-5.8.4/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 06:44:21.000000 yplib-5.8.4/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-05-23 06:44:21.000000 yplib-5.8.4/yplib.egg-info/top_level.txt
```

### Comparing `yplib-5.8.3/LICENSE` & `yplib-5.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-5.8.3/setup.py` & `yplib-5.8.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="yplib",
-    version="5.8.3",
+    version="5.8.4",
     author="yangpu",
     author_email="wantwaterfish@gmail.com",
     description="util",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
```

### Comparing `yplib-5.8.3/yplib/__init__.py` & `yplib-5.8.4/yplib/__init__.py`

 * *Files identical despite different names*

### Comparing `yplib-5.8.3/yplib/chart.py` & `yplib-5.8.4/yplib/chart.py`

 * *Files identical despite different names*

### Comparing `yplib-5.8.3/yplib/chart_html.py` & `yplib-5.8.4/yplib/chart_html.py`

 * *Files identical despite different names*

### Comparing `yplib-5.8.3/yplib/db.py` & `yplib-5.8.4/yplib/db.py`

 * *Files identical despite different names*

### Comparing `yplib-5.8.3/yplib/file.py` & `yplib-5.8.4/yplib/file.py`

 * *Files identical despite different names*

### Comparing `yplib-5.8.3/yplib/http_util.py` & `yplib-5.8.4/yplib/http_util.py`

 * *Files identical despite different names*

### Comparing `yplib-5.8.3/yplib/index.py` & `yplib-5.8.4/yplib/index.py`

 * *Files 2% similar despite different names*

```diff
@@ -970,20 +970,17 @@
     if data is None:
         data = {}
     set_data_in_user_home(file_name, data)
 
 
 # 从 config 中获得 配置数据
 def get_config_data(file_name='config'):
-    print('get_config_data', file_name)
     config_data = get_data_from_user_home(file_name)
-    print('get_data_from_user_home', config_data)
     if not config_data:
         config_data = get_data_from_path(file_name)
-    print('get_data_from_path', config_data)
     return config_data
 
 
 # 在当前用户的主目录中, 获得指定文件的数据
 def get_data_from_user_home(file_name='config'):
     return get_data_from_path(file_name, os.path.expanduser("~"))
 
@@ -993,25 +990,27 @@
     if data is None:
         data = {}
     set_data_in_path(file_name, data, os.path.expanduser("~"))
 
 
 # 在当前的目录中, 获得指定文件的数据
 def get_data_from_path(file_name='config', file_path=None):
-    config_path = file_path + '/' + CONFIG_PATH if file_path else CONFIG_PATH
-    print('config_path_1', config_path)
+    data = get_data_from_path_detail(file_name, file_path, CONFIG_PATH)
+    if data:
+        return data
+    get_data_from_path_detail(file_name, file_path, CONFIG_PATH_BAK)
+
+
+def get_data_from_path_detail(file_name='config', file_path=None, path_name=CONFIG_PATH):
+    config_path = file_path + '/' + path_name if file_path else path_name
     if not os.path.exists(config_path):
-        config_path = file_path + '/' + CONFIG_PATH_BAK if file_path else CONFIG_PATH_BAK
-        print('config_path_2', config_path)
+        return None
     file_path = config_path + '/' + file_name + '.json'
-    print('config_path_3', file_path)
     if not os.path.exists(file_path):
-        print('config_path_4', file_path)
-        return {}
-    print('to_json_from_file', file_path)
+        return None
     return to_json_from_file(file_path)
 
 
 # 在当前的目录中, 设置数据到指定路径下
 def set_data_in_path(file_name='config', data=None, file_path=''):
     if data is None:
         data = {}
```

### Comparing `yplib-5.8.3/yplib/mail.py` & `yplib-5.8.4/yplib/mail.py`

 * *Files identical despite different names*

### Comparing `yplib-5.8.3/yplib/mail_html.py` & `yplib-5.8.4/yplib/mail_html.py`

 * *Files identical despite different names*

### Comparing `yplib-5.8.3/yplib/markdown.py` & `yplib-5.8.4/yplib/markdown.py`

 * *Files identical despite different names*

### Comparing `yplib-5.8.3/yplib/multi_thread.py` & `yplib-5.8.4/yplib/multi_thread.py`

 * *Files identical despite different names*

