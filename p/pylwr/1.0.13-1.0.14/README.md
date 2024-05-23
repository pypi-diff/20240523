# Comparing `tmp/pylwr-1.0.13.tar.gz` & `tmp/pylwr-1.0.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylwr-1.0.13.tar", last modified: Thu Jan 18 08:35:49 2024, max compression
+gzip compressed data, was "pylwr-1.0.14.tar", last modified: Thu May 23 01:39:44 2024, max compression
```

## Comparing `pylwr-1.0.13.tar` & `pylwr-1.0.14.tar`

### file list

```diff
@@ -1,18 +1,33 @@
-drwxrwxrwx   0        0        0        0 2024-01-18 08:35:49.407147 pylwr-1.0.13/
--rw-rw-rw-   0        0        0    35821 2024-01-16 09:51:20.000000 pylwr-1.0.13/LICENSE
--rw-rw-rw-   0        0        0     1095 2024-01-18 08:35:49.406150 pylwr-1.0.13/PKG-INFO
--rw-rw-rw-   0        0        0      535 2024-01-18 08:35:46.000000 pylwr-1.0.13/README.md
--rw-rw-rw-   0        0        0      489 2024-01-18 08:27:39.000000 pylwr-1.0.13/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-01-18 08:35:49.408145 pylwr-1.0.13/setup.cfg
--rw-rw-rw-   0        0        0     1199 2024-01-18 08:27:48.000000 pylwr-1.0.13/setup.py
-drwxrwxrwx   0        0        0        0 2024-01-18 08:35:49.386157 pylwr-1.0.13/src/
-drwxrwxrwx   0        0        0        0 2024-01-18 08:35:49.402132 pylwr-1.0.13/src/pylwr/
--rw-rw-rw-   0        0        0       33 2024-01-16 09:51:20.000000 pylwr-1.0.13/src/pylwr/__init__.py
--rw-rw-rw-   0        0        0     2547 2024-01-18 08:11:59.000000 pylwr-1.0.13/src/pylwr/excel.py
--rw-rw-rw-   0        0        0     1728 2024-01-17 06:10:07.000000 pylwr-1.0.13/src/pylwr/mysql.py
--rw-rw-rw-   0        0        0     1769 2024-01-17 07:41:26.000000 pylwr-1.0.13/src/pylwr/oracle.py
-drwxrwxrwx   0        0        0        0 2024-01-18 08:35:49.406150 pylwr-1.0.13/src/pylwr.egg-info/
--rw-rw-rw-   0        0        0     1095 2024-01-18 08:35:49.000000 pylwr-1.0.13/src/pylwr.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      253 2024-01-18 08:35:49.000000 pylwr-1.0.13/src/pylwr.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-18 08:35:49.000000 pylwr-1.0.13/src/pylwr.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-01-18 08:35:49.000000 pylwr-1.0.13/src/pylwr.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-23 01:39:44.515702 pylwr-1.0.14/
+-rw-rw-rw-   0        0        0    35821 2024-01-16 09:51:20.000000 pylwr-1.0.14/LICENSE
+-rw-rw-rw-   0        0        0     1184 2024-05-23 01:39:44.514704 pylwr-1.0.14/PKG-INFO
+-rw-rw-rw-   0        0        0      624 2024-03-19 09:46:47.000000 pylwr-1.0.14/README.md
+-rw-rw-rw-   0        0        0      489 2024-05-23 01:38:23.000000 pylwr-1.0.14/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-23 01:39:44.515702 pylwr-1.0.14/setup.cfg
+-rw-rw-rw-   0        0        0     1199 2024-05-23 01:38:28.000000 pylwr-1.0.14/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 01:39:44.497759 pylwr-1.0.14/src/
+drwxrwxrwx   0        0        0        0 2024-05-23 01:39:44.503735 pylwr-1.0.14/src/pylwr/
+-rw-rw-rw-   0        0        0      369 2024-03-19 09:51:10.000000 pylwr-1.0.14/src/pylwr/__init__.py
+-rw-rw-rw-   0        0        0      640 2024-01-29 07:49:15.000000 pylwr-1.0.14/src/pylwr/const.py
+-rw-rw-rw-   0        0        0      389 2024-01-22 09:47:43.000000 pylwr-1.0.14/src/pylwr/distribute.py
+-rw-rw-rw-   0        0        0     2176 2024-01-23 07:20:59.000000 pylwr-1.0.14/src/pylwr/excel.py
+drwxrwxrwx   0        0        0        0 2024-05-23 01:39:44.507724 pylwr-1.0.14/src/pylwr/log/
+-rw-rw-rw-   0        0        0       27 2024-01-23 04:08:28.000000 pylwr-1.0.14/src/pylwr/log/__init__.py
+-rw-rw-rw-   0        0        0      306 2024-01-23 09:46:48.000000 pylwr-1.0.14/src/pylwr/log/loguru.py
+drwxrwxrwx   0        0        0        0 2024-05-23 01:39:44.509719 pylwr-1.0.14/src/pylwr/micm/
+-rw-rw-rw-   0        0        0       45 2024-03-19 09:50:02.000000 pylwr-1.0.14/src/pylwr/micm/__init__.py
+-rw-rw-rw-   0        0        0     6193 2024-03-19 10:10:19.000000 pylwr-1.0.14/src/pylwr/micm/ka02.py
+-rw-rw-rw-   0        0        0     1308 2024-03-19 10:08:58.000000 pylwr-1.0.14/src/pylwr/micm/knowledge.py
+drwxrwxrwx   0        0        0        0 2024-05-23 01:39:44.513706 pylwr-1.0.14/src/pylwr/proxy/
+-rw-rw-rw-   0        0        0        0 2024-01-23 06:51:00.000000 pylwr-1.0.14/src/pylwr/proxy/__init__.py
+-rw-rw-rw-   0        0        0      689 2024-01-22 02:20:09.000000 pylwr-1.0.14/src/pylwr/proxy/portfind.py
+-rw-rw-rw-   0        0        0      787 2024-01-22 02:20:09.000000 pylwr-1.0.14/src/pylwr/proxy/route.py
+-rw-rw-rw-   0        0        0      587 2024-01-30 01:43:50.000000 pylwr-1.0.14/src/pylwr/proxy/v2ray.py
+-rw-rw-rw-   0        0        0      627 2024-05-21 03:01:27.000000 pylwr-1.0.14/src/pylwr/proxy/v2ray_dell.py
+-rw-rw-rw-   0        0        0      625 2024-01-31 06:25:55.000000 pylwr-1.0.14/src/pylwr/proxy/v2rayin.py
+-rw-rw-rw-   0        0        0      629 2024-01-31 09:46:28.000000 pylwr-1.0.14/src/pylwr/proxy/v2rayshishi.py
+drwxrwxrwx   0        0        0        0 2024-05-23 01:39:44.513706 pylwr-1.0.14/src/pylwr.egg-info/
+-rw-rw-rw-   0        0        0     1184 2024-05-23 01:39:44.000000 pylwr-1.0.14/src/pylwr.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      579 2024-05-23 01:39:44.000000 pylwr-1.0.14/src/pylwr.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 01:39:44.000000 pylwr-1.0.14/src/pylwr.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-05-23 01:39:44.000000 pylwr-1.0.14/src/pylwr.egg-info/top_level.txt
```

### Comparing `pylwr-1.0.13/LICENSE` & `pylwr-1.0.14/LICENSE`

 * *Files identical despite different names*

### Comparing `pylwr-1.0.13/PKG-INFO` & `pylwr-1.0.14/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylwr
-Version: 1.0.13
+Version: 1.0.14
 Summary: 各种包使用的二次封装
 Home-page: https://gitee.com/linwanrui/pylwr
 Author: linwr
 Author-email: linwr <953297255@qq.com>
 Project-URL: Homepage, https://gitee.com/linwanrui/pylwr
 Project-URL: Bug Tracker, https://gitee.com/linwanrui/pylwr/issues
 Classifier: Programming Language :: Python :: 3
@@ -26,14 +26,18 @@
 
 ```shell
 pip install build
 pip install openpyxl
 pip install twine
 pip install pymysql
 pip install oracledb
+pip install scapy
+pip install psutil
+pip install loguru
+pip install dataclasses-json
 ```
 
 ## 安装
 
 ```shell
 pip install pylwr
 ```
```

### Comparing `pylwr-1.0.13/README.md` & `pylwr-1.0.14/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -10,14 +10,18 @@
 
 ```shell
 pip install build
 pip install openpyxl
 pip install twine
 pip install pymysql
 pip install oracledb
+pip install scapy
+pip install psutil
+pip install loguru
+pip install dataclasses-json
 ```
 
 ## 安装
 
 ```shell
 pip install pylwr
 ```
```

### Comparing `pylwr-1.0.13/setup.py` & `pylwr-1.0.14/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
  
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
  
 setuptools.setup(
     name="pylwr",  # 项目名称，保证它的唯一性，不要跟pypi上已存在的包名冲突即可
-    version="1.0.13",  # 程序版本
+    version="1.0.14",  # 程序版本
     # py_modules=['mysql'],  # 需要上传的模块名称，这样可以让这些模块直接import导入
     author="linwr",  # 项目作者
     author_email="953297255@qq.com",  # 作者邮件
     description="各种包使用的二次封装",  # 项目的一句话描述
     long_description=long_description,  # 加长版描述
     long_description_content_type="text/markdown",  # 描述使用Markdown
     url="https://gitee.com/linwanrui/pylwr",  # 项目地址
```

### Comparing `pylwr-1.0.13/src/pylwr/excel.py` & `pylwr-1.0.14/src/pylwr/excel.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,43 +1,36 @@
 from openpyxl import load_workbook
-from openpyxl.utils import column_index_from_string
-'''
-Excel复杂加工包装
-文件名需要使用绝对路径，例如：c:\\tool\\file_name.xlsx
----------------------------------
-Excel complex processing packaging
-The file name needs to use an absolute path, for example: c:\\tool\\file_name.xlsx
----------------------------------
-
-sheet可以作为str或者int类型，str需要传入sheet的名字，int需要传入sheet的index
--------------
-Sheet can be of type str or int. str needs to be passed in the name of the sheet, and int needs to be passed in the index of the sheet.
 
-'''
 class Excel(object):
-    
+    '''
+    Excel复杂加工包装
+    文件名需要使用绝对路径，例如：c:\\tool\\file_name.xlsx
+    sheet可以作为str或者int类型，str需要传入sheet的名字，int需要传入sheet的index
+
+    '''
     def __init__(self, file: str , sheet_index: str|int, ) -> object:
         # load workbook
         self.workbook = load_workbook(file)
         # select workbook
         self.sheet = self.workbook[sheet_index]
 
-    """
+    
+    def read_data_cols(self, head_index: int, cols: str|list, ) -> list:
+        """
         获取表格特定几个列的所有数据
         
 
         :param head_index: 表头占用的行数
         :type head_index: int
 
         :param cols: 如果只是一个列, 直接写列的名字字符串, 多个的话, 用list来输入
         :type cols: tr|list
 
         :rtype: list
         """
-    def read_data_cols(self, head_index: int, cols: str|list, ) -> list:
         result = []
         if isinstance(cols, str):
             col_names = [cols]
         elif isinstance(cols, list):
             col_names = cols
         else:
             raise TypeError("Unsupported type. Please provide a string or list.")
```

### Comparing `pylwr-1.0.13/src/pylwr.egg-info/PKG-INFO` & `pylwr-1.0.14/src/pylwr.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylwr
-Version: 1.0.13
+Version: 1.0.14
 Summary: 各种包使用的二次封装
 Home-page: https://gitee.com/linwanrui/pylwr
 Author: linwr
 Author-email: linwr <953297255@qq.com>
 Project-URL: Homepage, https://gitee.com/linwanrui/pylwr
 Project-URL: Bug Tracker, https://gitee.com/linwanrui/pylwr/issues
 Classifier: Programming Language :: Python :: 3
@@ -26,14 +26,18 @@
 
 ```shell
 pip install build
 pip install openpyxl
 pip install twine
 pip install pymysql
 pip install oracledb
+pip install scapy
+pip install psutil
+pip install loguru
+pip install dataclasses-json
 ```
 
 ## 安装
 
 ```shell
 pip install pylwr
 ```
```

