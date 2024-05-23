# Comparing `tmp/eliasliu-0.1.58.tar.gz` & `tmp/eliasliu-0.1.59.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eliasliu-0.1.58.tar", last modified: Tue May 21 15:31:13 2024, max compression
+gzip compressed data, was "eliasliu-0.1.59.tar", last modified: Thu May 23 03:00:09 2024, max compression
```

## Comparing `eliasliu-0.1.58.tar` & `eliasliu-0.1.59.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 15:31:13.539487 eliasliu-0.1.58/
--rw-rw-rw-   0        0        0     7013 2024-05-21 15:31:13.538488 eliasliu-0.1.58/PKG-INFO
--rw-rw-rw-   0        0        0     5851 2024-05-06 15:18:50.000000 eliasliu-0.1.58/README.md
-drwxrwxrwx   0        0        0        0 2024-05-21 15:31:13.327159 eliasliu-0.1.58/elias/
-drwxrwxrwx   0        0        0        0 2024-05-21 15:31:13.441682 eliasliu-0.1.58/elias/Scripts/
--rw-rw-rw-   0        0        0     2788 2024-05-06 15:18:50.000000 eliasliu-0.1.58/elias/Scripts/MysqlTool.py
--rw-rw-rw-   0        0        0      131 2024-05-06 15:18:50.000000 eliasliu-0.1.58/elias/Scripts/__init__.py
--rw-rw-rw-   0        0        0     6723 2024-05-06 15:18:50.000000 eliasliu-0.1.58/elias/Scripts/douyin.py
--rw-rw-rw-   0        0        0     5118 2024-05-06 15:18:50.000000 eliasliu-0.1.58/elias/Scripts/jd.py
--rw-rw-rw-   0        0        0     2407 2024-05-06 15:18:50.000000 eliasliu-0.1.58/elias/Scripts/name_in_db.py
--rw-rw-rw-   0        0        0    15915 2024-05-06 15:18:50.000000 eliasliu-0.1.58/elias/Scripts/py_clickhouse.py
--rw-rw-rw-   0        0        0    15332 2024-05-06 15:18:50.000000 eliasliu-0.1.58/elias/Scripts/vm_clickhouse.py
--rw-rw-rw-   0        0        0     3396 2024-05-06 15:18:50.000000 eliasliu-0.1.58/elias/Scripts/youdao.py
--rw-rw-rw-   0        0        0      368 2024-05-06 15:18:50.000000 eliasliu-0.1.58/elias/__init__.py
--rw-rw-rw-   0        0        0     1082 2024-05-21 15:30:20.000000 eliasliu-0.1.58/elias/ai.py
--rw-rw-rw-   0        0        0    30771 2024-05-06 15:18:50.000000 eliasliu-0.1.58/elias/check.py
--rw-rw-rw-   0        0        0     1376 2024-05-06 15:18:50.000000 eliasliu-0.1.58/elias/config_env_variable.py
--rw-rw-rw-   0        0        0     9670 2024-05-06 15:18:50.000000 eliasliu-0.1.58/elias/datamove.py
-drwxrwxrwx   0        0        0        0 2024-05-21 15:31:13.524488 eliasliu-0.1.58/elias/datax/
--rw-rw-rw-   0        0        0      131 2024-05-06 15:18:50.000000 eliasliu-0.1.58/elias/datax/__init__.py
--rw-rw-rw-   0        0        0    15834 2024-05-06 15:18:50.000000 eliasliu-0.1.58/elias/datax/auto_create_table.py
--rw-rw-rw-   0        0        0     3493 2024-05-06 15:18:50.000000 eliasliu-0.1.58/elias/datax/job.py
--rw-rw-rw-   0        0        0     4138 2024-05-06 15:18:50.000000 eliasliu-0.1.58/elias/datax/main.py
--rw-rw-rw-   0        0        0     5480 2024-05-06 15:18:50.000000 eliasliu-0.1.58/elias/datax/reader.py
--rw-rw-rw-   0        0        0     1756 2024-05-06 15:18:50.000000 eliasliu-0.1.58/elias/datax/run.py
--rw-rw-rw-   0        0        0     3588 2024-05-06 15:18:50.000000 eliasliu-0.1.58/elias/datax/writer.py
--rw-rw-rw-   0        0        0    92990 2024-05-06 15:18:50.000000 eliasliu-0.1.58/elias/etl.py
--rw-rw-rw-   0        0        0     9840 2024-05-06 15:18:50.000000 eliasliu-0.1.58/elias/picture.py
--rw-rw-rw-   0        0        0    79330 2024-05-20 08:28:30.000000 eliasliu-0.1.58/elias/usual.py
--rw-rw-rw-   0        0        0    13040 2024-05-06 15:18:50.000000 eliasliu-0.1.58/elias/wechat.py
-drwxrwxrwx   0        0        0        0 2024-05-21 15:31:13.538488 eliasliu-0.1.58/eliasliu.egg-info/
--rw-rw-rw-   0        0        0     7013 2024-05-21 15:31:13.000000 eliasliu-0.1.58/eliasliu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      700 2024-05-21 15:31:13.000000 eliasliu-0.1.58/eliasliu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 15:31:13.000000 eliasliu-0.1.58/eliasliu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      169 2024-05-21 15:31:13.000000 eliasliu-0.1.58/eliasliu.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-05-21 15:31:13.000000 eliasliu-0.1.58/eliasliu.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-21 15:31:13.539487 eliasliu-0.1.58/setup.cfg
--rw-rw-rw-   0        0        0     1947 2024-05-21 15:30:51.000000 eliasliu-0.1.58/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 03:00:09.879831 eliasliu-0.1.59/
+-rw-rw-rw-   0        0        0     7058 2024-05-23 03:00:09.879831 eliasliu-0.1.59/PKG-INFO
+-rw-rw-rw-   0        0        0     5851 2024-05-06 15:18:50.000000 eliasliu-0.1.59/README.md
+drwxrwxrwx   0        0        0        0 2024-05-23 03:00:09.684262 eliasliu-0.1.59/elias/
+drwxrwxrwx   0        0        0        0 2024-05-23 03:00:09.791237 eliasliu-0.1.59/elias/Scripts/
+-rw-rw-rw-   0        0        0     2788 2024-05-06 15:18:50.000000 eliasliu-0.1.59/elias/Scripts/MysqlTool.py
+-rw-rw-rw-   0        0        0      131 2024-05-06 15:18:50.000000 eliasliu-0.1.59/elias/Scripts/__init__.py
+-rw-rw-rw-   0        0        0     6723 2024-05-06 15:18:50.000000 eliasliu-0.1.59/elias/Scripts/douyin.py
+-rw-rw-rw-   0        0        0     5118 2024-05-06 15:18:50.000000 eliasliu-0.1.59/elias/Scripts/jd.py
+-rw-rw-rw-   0        0        0     2407 2024-05-06 15:18:50.000000 eliasliu-0.1.59/elias/Scripts/name_in_db.py
+-rw-rw-rw-   0        0        0    15915 2024-05-06 15:18:50.000000 eliasliu-0.1.59/elias/Scripts/py_clickhouse.py
+-rw-rw-rw-   0        0        0    15332 2024-05-06 15:18:50.000000 eliasliu-0.1.59/elias/Scripts/vm_clickhouse.py
+-rw-rw-rw-   0        0        0     3396 2024-05-06 15:18:50.000000 eliasliu-0.1.59/elias/Scripts/youdao.py
+-rw-rw-rw-   0        0        0      368 2024-05-06 15:18:50.000000 eliasliu-0.1.59/elias/__init__.py
+-rw-rw-rw-   0        0        0     2278 2024-05-23 02:15:10.000000 eliasliu-0.1.59/elias/ai.py
+-rw-rw-rw-   0        0        0    30771 2024-05-06 15:18:50.000000 eliasliu-0.1.59/elias/check.py
+-rw-rw-rw-   0        0        0     1376 2024-05-06 15:18:50.000000 eliasliu-0.1.59/elias/config_env_variable.py
+-rw-rw-rw-   0        0        0     9670 2024-05-06 15:18:50.000000 eliasliu-0.1.59/elias/datamove.py
+drwxrwxrwx   0        0        0        0 2024-05-23 03:00:09.863881 eliasliu-0.1.59/elias/datax/
+-rw-rw-rw-   0        0        0      131 2024-05-06 15:18:50.000000 eliasliu-0.1.59/elias/datax/__init__.py
+-rw-rw-rw-   0        0        0    15834 2024-05-06 15:18:50.000000 eliasliu-0.1.59/elias/datax/auto_create_table.py
+-rw-rw-rw-   0        0        0     3493 2024-05-06 15:18:50.000000 eliasliu-0.1.59/elias/datax/job.py
+-rw-rw-rw-   0        0        0     4138 2024-05-06 15:18:50.000000 eliasliu-0.1.59/elias/datax/main.py
+-rw-rw-rw-   0        0        0     5480 2024-05-06 15:18:50.000000 eliasliu-0.1.59/elias/datax/reader.py
+-rw-rw-rw-   0        0        0     1756 2024-05-06 15:18:50.000000 eliasliu-0.1.59/elias/datax/run.py
+-rw-rw-rw-   0        0        0     3588 2024-05-06 15:18:50.000000 eliasliu-0.1.59/elias/datax/writer.py
+-rw-rw-rw-   0        0        0    92990 2024-05-06 15:18:50.000000 eliasliu-0.1.59/elias/etl.py
+-rw-rw-rw-   0        0        0     9840 2024-05-06 15:18:50.000000 eliasliu-0.1.59/elias/picture.py
+-rw-rw-rw-   0        0        0     1902 2024-05-23 02:58:34.000000 eliasliu-0.1.59/elias/text_similarity.py
+-rw-rw-rw-   0        0        0    79330 2024-05-20 08:28:30.000000 eliasliu-0.1.59/elias/usual.py
+-rw-rw-rw-   0        0        0    13040 2024-05-06 15:18:50.000000 eliasliu-0.1.59/elias/wechat.py
+drwxrwxrwx   0        0        0        0 2024-05-23 03:00:09.878832 eliasliu-0.1.59/eliasliu.egg-info/
+-rw-rw-rw-   0        0        0     7058 2024-05-23 03:00:09.000000 eliasliu-0.1.59/eliasliu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      725 2024-05-23 03:00:09.000000 eliasliu-0.1.59/eliasliu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 03:00:09.000000 eliasliu-0.1.59/eliasliu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      182 2024-05-23 03:00:09.000000 eliasliu-0.1.59/eliasliu.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-23 03:00:09.000000 eliasliu-0.1.59/eliasliu.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-23 03:00:09.880832 eliasliu-0.1.59/setup.cfg
+-rw-rw-rw-   0        0        0     1984 2024-05-23 02:59:59.000000 eliasliu-0.1.59/setup.py
```

### Comparing `eliasliu-0.1.58/PKG-INFO` & `eliasliu-0.1.59/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eliasliu
-Version: 0.1.58
+Version: 0.1.59
 Summary: A very easy tool to deal your data
 Home-page: https://github.com/tenbj/elias
 Author: Elias Liu 刘益廷
 Author-email: liuyiting120@126.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -27,14 +27,16 @@
 Requires-Dist: clickhouse_driver
 Requires-Dist: bs4
 Requires-Dist: selenium
 Requires-Dist: loguru
 Requires-Dist: ollama
 Requires-Dist: pillow
 Requires-Dist: opencv-python
+Requires-Dist: jieba
+Requires-Dist: openai
 
 0 安装
 找到终端，再终端内输入以下代码
 安装
 pip install elias
 更新
 pip install elias --upgrade
```

### Comparing `eliasliu-0.1.58/README.md` & `eliasliu-0.1.59/README.md`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.58/elias/Scripts/MysqlTool.py` & `eliasliu-0.1.59/elias/Scripts/MysqlTool.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.58/elias/Scripts/douyin.py` & `eliasliu-0.1.59/elias/Scripts/douyin.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.58/elias/Scripts/jd.py` & `eliasliu-0.1.59/elias/Scripts/jd.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.58/elias/Scripts/name_in_db.py` & `eliasliu-0.1.59/elias/Scripts/name_in_db.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.58/elias/Scripts/py_clickhouse.py` & `eliasliu-0.1.59/elias/Scripts/py_clickhouse.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.58/elias/Scripts/vm_clickhouse.py` & `eliasliu-0.1.59/elias/Scripts/vm_clickhouse.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.58/elias/Scripts/youdao.py` & `eliasliu-0.1.59/elias/Scripts/youdao.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.58/elias/check.py` & `eliasliu-0.1.59/elias/check.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.58/elias/config_env_variable.py` & `eliasliu-0.1.59/elias/config_env_variable.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.58/elias/datamove.py` & `eliasliu-0.1.59/elias/datamove.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.58/elias/datax/auto_create_table.py` & `eliasliu-0.1.59/elias/datax/auto_create_table.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.58/elias/datax/job.py` & `eliasliu-0.1.59/elias/datax/job.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.58/elias/datax/main.py` & `eliasliu-0.1.59/elias/datax/main.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.58/elias/datax/reader.py` & `eliasliu-0.1.59/elias/datax/reader.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.58/elias/datax/run.py` & `eliasliu-0.1.59/elias/datax/run.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.58/elias/datax/writer.py` & `eliasliu-0.1.59/elias/datax/writer.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.58/elias/etl.py` & `eliasliu-0.1.59/elias/etl.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.58/elias/picture.py` & `eliasliu-0.1.59/elias/picture.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.58/elias/usual.py` & `eliasliu-0.1.59/elias/usual.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.58/elias/wechat.py` & `eliasliu-0.1.59/elias/wechat.py`

 * *Files identical despite different names*

### Comparing `eliasliu-0.1.58/eliasliu.egg-info/PKG-INFO` & `eliasliu-0.1.59/eliasliu.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eliasliu
-Version: 0.1.58
+Version: 0.1.59
 Summary: A very easy tool to deal your data
 Home-page: https://github.com/tenbj/elias
 Author: Elias Liu 刘益廷
 Author-email: liuyiting120@126.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -27,14 +27,16 @@
 Requires-Dist: clickhouse_driver
 Requires-Dist: bs4
 Requires-Dist: selenium
 Requires-Dist: loguru
 Requires-Dist: ollama
 Requires-Dist: pillow
 Requires-Dist: opencv-python
+Requires-Dist: jieba
+Requires-Dist: openai
 
 0 安装
 找到终端，再终端内输入以下代码
 安装
 pip install elias
 更新
 pip install elias --upgrade
```

### Comparing `eliasliu-0.1.58/eliasliu.egg-info/SOURCES.txt` & `eliasliu-0.1.59/eliasliu.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 elias/__init__.py
 elias/ai.py
 elias/check.py
 elias/config_env_variable.py
 elias/datamove.py
 elias/etl.py
 elias/picture.py
+elias/text_similarity.py
 elias/usual.py
 elias/wechat.py
 elias/Scripts/MysqlTool.py
 elias/Scripts/__init__.py
 elias/Scripts/douyin.py
 elias/Scripts/jd.py
 elias/Scripts/name_in_db.py
```

### Comparing `eliasliu-0.1.58/setup.py` & `eliasliu-0.1.59/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='eliasliu',  # 包名
-    version='0.1.58',  # 版本号
+    version='0.1.59',  # 版本号
     description='A very easy tool to deal your data',  # 包的简要描述
     long_description = long_description,
     # long_description='Data Engineer & Analyst will use',  # 包的详细描述，通常从README文件中读取
     long_description_content_type='text/markdown',  # 详细描述的格式，这里是Markdown
     author='Elias Liu 刘益廷',  # 作者名称
     author_email='liuyiting120@126.com',  # 作者邮箱
     url='https://github.com/tenbj/elias',  # 项目的URL
@@ -36,15 +36,17 @@
         # 'odps',
         'bs4',
         'selenium',
         'loguru',
         # 'googletrans',
         'ollama',
         'pillow',
-        'opencv-python'
+        'opencv-python',
+        'jieba',
+        'openai'
     ],
     classifiers=[  # 包的分类标签
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
```

