# Comparing `tmp/sop_deutils-1.0.2.1.dev0.tar.gz` & `tmp/sop_deutils-1.0.2.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sop_deutils-1.0.2.1.dev0.tar", last modified: Thu May 23 02:46:07 2024, max compression
+gzip compressed data, was "sop_deutils-1.0.2.dev0.tar", last modified: Mon May 20 03:02:33 2024, max compression
```

## Comparing `sop_deutils-1.0.2.1.dev0.tar` & `sop_deutils-1.0.2.dev0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)        0 2024-05-23 02:46:07.186686 sop_deutils-1.0.2.1.dev0/
--rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)     1091 2024-05-18 13:33:42.000000 sop_deutils-1.0.2.1.dev0/LICENSE
--rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)       63 2024-05-18 13:35:44.000000 sop_deutils-1.0.2.1.dev0/MANIFEST.in
--rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)    52762 2024-05-23 02:46:07.186686 sop_deutils-1.0.2.1.dev0/PKG-INFO
--rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)    52285 2024-05-19 07:45:03.000000 sop_deutils-1.0.2.1.dev0/README.rst
--rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)      550 2024-05-23 02:46:05.000000 sop_deutils-1.0.2.1.dev0/pyproject.toml
--rw-rw-r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)       38 2024-05-23 02:46:07.186686 sop_deutils-1.0.2.1.dev0/setup.cfg
-drwxrwxr-x   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)        0 2024-05-23 02:46:07.186686 sop_deutils-1.0.2.1.dev0/sop_deutils/
--rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)        0 2024-05-18 02:26:47.000000 sop_deutils-1.0.2.1.dev0/sop_deutils/__init__.py
-drwxrwxr-x   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)        0 2024-05-23 02:46:07.186686 sop_deutils-1.0.2.1.dev0/sop_deutils/base/
--rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)     1470 2024-05-18 02:26:47.000000 sop_deutils-1.0.2.1.dev0/sop_deutils/base/y4a_da_cfg.py
-drwxrwxr-x   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)        0 2024-05-23 02:46:07.186686 sop_deutils-1.0.2.1.dev0/sop_deutils/datalake/
--rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)     8133 2024-05-18 02:26:47.000000 sop_deutils-1.0.2.1.dev0/sop_deutils/datalake/y4a_minio.py
-drwxrwxr-x   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)        0 2024-05-23 02:46:07.186686 sop_deutils-1.0.2.1.dev0/sop_deutils/gg_api/
--rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)       41 2024-05-18 02:26:47.000000 sop_deutils-1.0.2.1.dev0/sop_deutils/gg_api/config.ini
--rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)     2131 2024-05-18 02:26:47.000000 sop_deutils-1.0.2.1.dev0/sop_deutils/gg_api/y4a_chat.py
--rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)     6236 2024-05-18 02:26:47.000000 sop_deutils-1.0.2.1.dev0/sop_deutils/gg_api/y4a_mail.py
--rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)    19617 2024-05-19 07:09:02.000000 sop_deutils-1.0.2.1.dev0/sop_deutils/gg_api/y4a_sheet.py
--rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)    12008 2024-05-20 03:01:36.000000 sop_deutils-1.0.2.1.dev0/sop_deutils/r.zip
-drwxrwxr-x   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)        0 2024-05-23 02:46:07.186686 sop_deutils-1.0.2.1.dev0/sop_deutils/sql/
--rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)     4330 2024-05-18 02:26:47.000000 sop_deutils-1.0.2.1.dev0/sop_deutils/sql/y4a_monitor_user.py
--rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)     5820 2024-05-18 02:26:47.000000 sop_deutils-1.0.2.1.dev0/sop_deutils/sql/y4a_mysql.py
--rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)    50293 2024-05-23 02:43:25.000000 sop_deutils-1.0.2.1.dev0/sop_deutils/sql/y4a_postgresql.py
--rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)     3927 2024-05-18 02:26:47.000000 sop_deutils-1.0.2.1.dev0/sop_deutils/y4a_airflow.py
--rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)      748 2024-05-19 04:32:14.000000 sop_deutils-1.0.2.1.dev0/sop_deutils/y4a_credentials.py
--rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)     1218 2024-05-18 02:26:47.000000 sop_deutils-1.0.2.1.dev0/sop_deutils/y4a_retry.py
--rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)     2925 2024-05-18 02:26:47.000000 sop_deutils-1.0.2.1.dev0/sop_deutils/y4a_telegram.py
-drwxrwxr-x   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)        0 2024-05-23 02:46:07.186686 sop_deutils-1.0.2.1.dev0/sop_deutils.egg-info/
--rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)    52762 2024-05-23 02:46:07.000000 sop_deutils-1.0.2.1.dev0/sop_deutils.egg-info/PKG-INFO
--rw-rw-r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)      626 2024-05-23 02:46:07.000000 sop_deutils-1.0.2.1.dev0/sop_deutils.egg-info/SOURCES.txt
--rw-rw-r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)        1 2024-05-23 02:46:07.000000 sop_deutils-1.0.2.1.dev0/sop_deutils.egg-info/dependency_links.txt
--rw-rw-r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)       12 2024-05-23 02:46:07.000000 sop_deutils-1.0.2.1.dev0/sop_deutils.egg-info/top_level.txt
+drwxr-xr-x   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)        0 2024-05-20 03:02:33.886007 sop_deutils-1.0.2.dev0/
+-rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)     1091 2024-05-18 13:33:42.000000 sop_deutils-1.0.2.dev0/LICENSE
+-rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)       63 2024-05-18 13:35:44.000000 sop_deutils-1.0.2.dev0/MANIFEST.in
+-rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)    52760 2024-05-20 03:02:33.886007 sop_deutils-1.0.2.dev0/PKG-INFO
+-rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)    52285 2024-05-19 07:45:03.000000 sop_deutils-1.0.2.dev0/README.rst
+-rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)      548 2024-05-20 03:02:32.000000 sop_deutils-1.0.2.dev0/pyproject.toml
+-rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)       38 2024-05-20 03:02:33.886007 sop_deutils-1.0.2.dev0/setup.cfg
+drwxr-xr-x   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)        0 2024-05-20 03:02:33.876006 sop_deutils-1.0.2.dev0/sop_deutils/
+-rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)        0 2024-05-18 02:26:47.000000 sop_deutils-1.0.2.dev0/sop_deutils/__init__.py
+drwxr-xr-x   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)        0 2024-05-20 03:02:33.886007 sop_deutils-1.0.2.dev0/sop_deutils/base/
+-rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)     1470 2024-05-18 02:26:47.000000 sop_deutils-1.0.2.dev0/sop_deutils/base/y4a_da_cfg.py
+drwxr-xr-x   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)        0 2024-05-20 03:02:33.886007 sop_deutils-1.0.2.dev0/sop_deutils/datalake/
+-rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)     8133 2024-05-18 02:26:47.000000 sop_deutils-1.0.2.dev0/sop_deutils/datalake/y4a_minio.py
+drwxr-xr-x   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)        0 2024-05-20 03:02:33.886007 sop_deutils-1.0.2.dev0/sop_deutils/gg_api/
+-rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)       41 2024-05-18 02:26:47.000000 sop_deutils-1.0.2.dev0/sop_deutils/gg_api/config.ini
+-rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)     2131 2024-05-18 02:26:47.000000 sop_deutils-1.0.2.dev0/sop_deutils/gg_api/y4a_chat.py
+-rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)     6236 2024-05-18 02:26:47.000000 sop_deutils-1.0.2.dev0/sop_deutils/gg_api/y4a_mail.py
+-rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)    19617 2024-05-19 07:09:02.000000 sop_deutils-1.0.2.dev0/sop_deutils/gg_api/y4a_sheet.py
+-rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)    12008 2024-05-20 03:01:36.000000 sop_deutils-1.0.2.dev0/sop_deutils/r.zip
+drwxr-xr-x   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)        0 2024-05-20 03:02:33.886007 sop_deutils-1.0.2.dev0/sop_deutils/sql/
+-rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)     4330 2024-05-18 02:26:47.000000 sop_deutils-1.0.2.dev0/sop_deutils/sql/y4a_monitor_user.py
+-rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)     5820 2024-05-18 02:26:47.000000 sop_deutils-1.0.2.dev0/sop_deutils/sql/y4a_mysql.py
+-rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)    50237 2024-05-19 06:00:03.000000 sop_deutils-1.0.2.dev0/sop_deutils/sql/y4a_postgresql.py
+-rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)     3927 2024-05-18 02:26:47.000000 sop_deutils-1.0.2.dev0/sop_deutils/y4a_airflow.py
+-rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)      748 2024-05-19 04:32:14.000000 sop_deutils-1.0.2.dev0/sop_deutils/y4a_credentials.py
+-rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)     1218 2024-05-18 02:26:47.000000 sop_deutils-1.0.2.dev0/sop_deutils/y4a_retry.py
+-rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)     2925 2024-05-18 02:26:47.000000 sop_deutils-1.0.2.dev0/sop_deutils/y4a_telegram.py
+drwxr-xr-x   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)        0 2024-05-20 03:02:33.886007 sop_deutils-1.0.2.dev0/sop_deutils.egg-info/
+-rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)    52760 2024-05-20 03:02:33.000000 sop_deutils-1.0.2.dev0/sop_deutils.egg-info/PKG-INFO
+-rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)      626 2024-05-20 03:02:33.000000 sop_deutils-1.0.2.dev0/sop_deutils.egg-info/SOURCES.txt
+-rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)        1 2024-05-20 03:02:33.000000 sop_deutils-1.0.2.dev0/sop_deutils.egg-info/dependency_links.txt
+-rw-r--r--   0 ifyouknowyouknow  (1000) ifyouknowyouknow  (1000)       12 2024-05-20 03:02:33.000000 sop_deutils-1.0.2.dev0/sop_deutils.egg-info/top_level.txt
```

### Comparing `sop_deutils-1.0.2.1.dev0/LICENSE` & `sop_deutils-1.0.2.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `sop_deutils-1.0.2.1.dev0/PKG-INFO` & `sop_deutils-1.0.2.dev0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sop_deutils
-Version: 1.0.2.1.dev0
+Version: 1.0.2.dev0
 Summary: A utils package for Yes4All SOP
 Author-email: liuliukiki aka clong aka ifyouknowyouknow101 <longnc@yes4all.com>
 Project-URL: Author_Github, https://github.com/dribblewithclong
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `sop_deutils-1.0.2.1.dev0/README.rst` & `sop_deutils-1.0.2.dev0/README.rst`

 * *Files identical despite different names*

### Comparing `sop_deutils-1.0.2.1.dev0/pyproject.toml` & `sop_deutils-1.0.2.dev0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "setuptools>=61.0",]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sop_deutils"
-version = "1.0.2.1.dev"
+version = "1.0.2.dev"
 description = "A utils package for Yes4All SOP"
 readme = "README.rst"
 requires-python = ">=3.7"
 classifiers = [ "Programming Language :: Python :: 3", "License :: OSI Approved :: MIT License", "Operating System :: OS Independent",]
 [[project.authors]]
 name = "liuliukiki aka clong aka ifyouknowyouknow101"
 email = "longnc@yes4all.com"
```

### Comparing `sop_deutils-1.0.2.1.dev0/sop_deutils/base/y4a_da_cfg.py` & `sop_deutils-1.0.2.dev0/sop_deutils/base/y4a_da_cfg.py`

 * *Files identical despite different names*

### Comparing `sop_deutils-1.0.2.1.dev0/sop_deutils/datalake/y4a_minio.py` & `sop_deutils-1.0.2.dev0/sop_deutils/datalake/y4a_minio.py`

 * *Files identical despite different names*

### Comparing `sop_deutils-1.0.2.1.dev0/sop_deutils/gg_api/y4a_chat.py` & `sop_deutils-1.0.2.dev0/sop_deutils/gg_api/y4a_chat.py`

 * *Files identical despite different names*

### Comparing `sop_deutils-1.0.2.1.dev0/sop_deutils/gg_api/y4a_mail.py` & `sop_deutils-1.0.2.dev0/sop_deutils/gg_api/y4a_mail.py`

 * *Files identical despite different names*

### Comparing `sop_deutils-1.0.2.1.dev0/sop_deutils/gg_api/y4a_sheet.py` & `sop_deutils-1.0.2.dev0/sop_deutils/gg_api/y4a_sheet.py`

 * *Files identical despite different names*

### Comparing `sop_deutils-1.0.2.1.dev0/sop_deutils/r.zip` & `sop_deutils-1.0.2.dev0/sop_deutils/r.zip`

 * *Files identical despite different names*

### Comparing `sop_deutils-1.0.2.1.dev0/sop_deutils/sql/y4a_monitor_user.py` & `sop_deutils-1.0.2.dev0/sop_deutils/sql/y4a_monitor_user.py`

 * *Files identical despite different names*

### Comparing `sop_deutils-1.0.2.1.dev0/sop_deutils/sql/y4a_mysql.py` & `sop_deutils-1.0.2.dev0/sop_deutils/sql/y4a_mysql.py`

 * *Files identical despite different names*

### Comparing `sop_deutils-1.0.2.1.dev0/sop_deutils/sql/y4a_postgresql.py` & `sop_deutils-1.0.2.dev0/sop_deutils/sql/y4a_postgresql.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,17 +45,17 @@
         pg_name: str,
         account_name: str = None,
         pg_account: str = None,
         pg_password: str = None,
     ) -> None:
         self.hosts = {
             'raw_master': '172.30.105.100',
-            'raw_repl': '172.30.105.100',           # TODO: temp change
+            'raw_repl': '172.30.105.101',
             'serving_master': '172.30.105.111',
-            'serving_repl': '172.30.105.111',       # TODO: temp change
+            'serving_repl': '172.30.105.112',
             'staging': '172.30.12.153',
         }
         self.databases = {
             'raw_master': 'y4a_datawarehouse',
             'raw_repl': 'y4a_datawarehouse',
             'serving_master': 'y4a_datamart',
             'serving_repl': 'y4a_datamart',
```

### Comparing `sop_deutils-1.0.2.1.dev0/sop_deutils/y4a_airflow.py` & `sop_deutils-1.0.2.dev0/sop_deutils/y4a_airflow.py`

 * *Files identical despite different names*

### Comparing `sop_deutils-1.0.2.1.dev0/sop_deutils/y4a_credentials.py` & `sop_deutils-1.0.2.dev0/sop_deutils/y4a_credentials.py`

 * *Files identical despite different names*

### Comparing `sop_deutils-1.0.2.1.dev0/sop_deutils/y4a_retry.py` & `sop_deutils-1.0.2.dev0/sop_deutils/y4a_retry.py`

 * *Files identical despite different names*

### Comparing `sop_deutils-1.0.2.1.dev0/sop_deutils/y4a_telegram.py` & `sop_deutils-1.0.2.dev0/sop_deutils/y4a_telegram.py`

 * *Files identical despite different names*

### Comparing `sop_deutils-1.0.2.1.dev0/sop_deutils.egg-info/PKG-INFO` & `sop_deutils-1.0.2.dev0/sop_deutils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sop_deutils
-Version: 1.0.2.1.dev0
+Version: 1.0.2.dev0
 Summary: A utils package for Yes4All SOP
 Author-email: liuliukiki aka clong aka ifyouknowyouknow101 <longnc@yes4all.com>
 Project-URL: Author_Github, https://github.com/dribblewithclong
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `sop_deutils-1.0.2.1.dev0/sop_deutils.egg-info/SOURCES.txt` & `sop_deutils-1.0.2.dev0/sop_deutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

