# Comparing `tmp/alibabacloud_linkedmallretrieval20240501-1.0.0.tar.gz` & `tmp/alibabacloud_linkedmallretrieval20240501-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_linkedmallretrieval20240501-1.0.0.tar", last modified: Fri May 17 08:44:05 2024, max compression
+gzip compressed data, was "dist/alibabacloud_linkedmallretrieval20240501-1.0.1.tar", last modified: Thu May 23 10:22:21 2024, max compression
```

## Comparing `alibabacloud_linkedmallretrieval20240501-1.0.0.tar` & `alibabacloud_linkedmallretrieval20240501-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 08:44:05.000000 alibabacloud_linkedmallretrieval20240501-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      600 2024-05-17 08:44:05.000000 alibabacloud_linkedmallretrieval20240501-1.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-05-17 08:44:05.000000 alibabacloud_linkedmallretrieval20240501-1.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2513 2024-05-17 08:44:05.000000 alibabacloud_linkedmallretrieval20240501-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1159 2024-05-17 08:44:05.000000 alibabacloud_linkedmallretrieval20240501-1.0.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1244 2024-05-17 08:44:05.000000 alibabacloud_linkedmallretrieval20240501-1.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 08:44:05.000000 alibabacloud_linkedmallretrieval20240501-1.0.0/alibabacloud_linkedmallretrieval20240501/
--rw-r--r--   0 root         (0) root         (0)       21 2024-05-17 08:44:05.000000 alibabacloud_linkedmallretrieval20240501-1.0.0/alibabacloud_linkedmallretrieval20240501/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5372 2024-05-17 08:44:05.000000 alibabacloud_linkedmallretrieval20240501-1.0.0/alibabacloud_linkedmallretrieval20240501/client.py
--rw-r--r--   0 root         (0) root         (0)     7898 2024-05-17 08:44:05.000000 alibabacloud_linkedmallretrieval20240501-1.0.0/alibabacloud_linkedmallretrieval20240501/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-17 08:44:05.000000 alibabacloud_linkedmallretrieval20240501-1.0.0/alibabacloud_linkedmallretrieval20240501.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2513 2024-05-17 08:44:05.000000 alibabacloud_linkedmallretrieval20240501-1.0.0/alibabacloud_linkedmallretrieval20240501.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      535 2024-05-17 08:44:05.000000 alibabacloud_linkedmallretrieval20240501-1.0.0/alibabacloud_linkedmallretrieval20240501.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-17 08:44:05.000000 alibabacloud_linkedmallretrieval20240501-1.0.0/alibabacloud_linkedmallretrieval20240501.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-05-17 08:44:05.000000 alibabacloud_linkedmallretrieval20240501-1.0.0/alibabacloud_linkedmallretrieval20240501.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       41 2024-05-17 08:44:05.000000 alibabacloud_linkedmallretrieval20240501-1.0.0/alibabacloud_linkedmallretrieval20240501.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-05-17 08:44:05.000000 alibabacloud_linkedmallretrieval20240501-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2691 2024-05-17 08:44:05.000000 alibabacloud_linkedmallretrieval20240501-1.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:22:21.000000 alibabacloud_linkedmallretrieval20240501-1.0.1/
+-rw-r--r--   0 root         (0) root         (0)       82 2024-05-23 10:22:21.000000 alibabacloud_linkedmallretrieval20240501-1.0.1/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-05-23 10:22:21.000000 alibabacloud_linkedmallretrieval20240501-1.0.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-05-23 10:22:21.000000 alibabacloud_linkedmallretrieval20240501-1.0.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2513 2024-05-23 10:22:21.000000 alibabacloud_linkedmallretrieval20240501-1.0.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1159 2024-05-23 10:22:21.000000 alibabacloud_linkedmallretrieval20240501-1.0.1/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1244 2024-05-23 10:22:21.000000 alibabacloud_linkedmallretrieval20240501-1.0.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:22:21.000000 alibabacloud_linkedmallretrieval20240501-1.0.1/alibabacloud_linkedmallretrieval20240501/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-05-23 10:22:21.000000 alibabacloud_linkedmallretrieval20240501-1.0.1/alibabacloud_linkedmallretrieval20240501/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5372 2024-05-23 10:22:21.000000 alibabacloud_linkedmallretrieval20240501-1.0.1/alibabacloud_linkedmallretrieval20240501/client.py
+-rw-r--r--   0 root         (0) root         (0)     7898 2024-05-23 10:22:21.000000 alibabacloud_linkedmallretrieval20240501-1.0.1/alibabacloud_linkedmallretrieval20240501/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:22:21.000000 alibabacloud_linkedmallretrieval20240501-1.0.1/alibabacloud_linkedmallretrieval20240501.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2513 2024-05-23 10:22:21.000000 alibabacloud_linkedmallretrieval20240501-1.0.1/alibabacloud_linkedmallretrieval20240501.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      548 2024-05-23 10:22:21.000000 alibabacloud_linkedmallretrieval20240501-1.0.1/alibabacloud_linkedmallretrieval20240501.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-23 10:22:21.000000 alibabacloud_linkedmallretrieval20240501-1.0.1/alibabacloud_linkedmallretrieval20240501.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-05-23 10:22:21.000000 alibabacloud_linkedmallretrieval20240501-1.0.1/alibabacloud_linkedmallretrieval20240501.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       41 2024-05-23 10:22:21.000000 alibabacloud_linkedmallretrieval20240501-1.0.1/alibabacloud_linkedmallretrieval20240501.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-05-23 10:22:21.000000 alibabacloud_linkedmallretrieval20240501-1.0.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2691 2024-05-23 10:22:21.000000 alibabacloud_linkedmallretrieval20240501-1.0.1/setup.py
```

### Comparing `alibabacloud_linkedmallretrieval20240501-1.0.0/LICENSE` & `alibabacloud_linkedmallretrieval20240501-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_linkedmallretrieval20240501-1.0.0/PKG-INFO` & `alibabacloud_linkedmallretrieval20240501-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_linkedmallretrieval20240501
-Version: 1.0.0
+Version: 1.0.1
 Summary: Alibaba Cloud LinkedmallRetrieval (20240501) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_linkedmallretrieval20240501-1.0.0/README-CN.md` & `alibabacloud_linkedmallretrieval20240501-1.0.1/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_linkedmallretrieval20240501-1.0.0/README.md` & `alibabacloud_linkedmallretrieval20240501-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_linkedmallretrieval20240501-1.0.0/alibabacloud_linkedmallretrieval20240501/client.py` & `alibabacloud_linkedmallretrieval20240501-1.0.1/alibabacloud_linkedmallretrieval20240501/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_linkedmallretrieval20240501-1.0.0/alibabacloud_linkedmallretrieval20240501/models.py` & `alibabacloud_linkedmallretrieval20240501-1.0.1/alibabacloud_linkedmallretrieval20240501/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_linkedmallretrieval20240501-1.0.0/alibabacloud_linkedmallretrieval20240501.egg-info/PKG-INFO` & `alibabacloud_linkedmallretrieval20240501-1.0.1/alibabacloud_linkedmallretrieval20240501.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-linkedmallretrieval20240501
-Version: 1.0.0
+Version: 1.0.1
 Summary: Alibaba Cloud LinkedmallRetrieval (20240501) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_linkedmallretrieval20240501-1.0.0/alibabacloud_linkedmallretrieval20240501.egg-info/SOURCES.txt` & `alibabacloud_linkedmallretrieval20240501-1.0.1/alibabacloud_linkedmallretrieval20240501.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+ChangeLog.md
 LICENSE
 MANIFEST.in
 README-CN.md
 README.md
 setup.cfg
 setup.py
 alibabacloud_linkedmallretrieval20240501/__init__.py
```

### Comparing `alibabacloud_linkedmallretrieval20240501-1.0.0/setup.py` & `alibabacloud_linkedmallretrieval20240501-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_linkedmallretrieval20240501.
 
-Created on 17/05/2024
+Created on 23/05/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_linkedmallretrieval20240501"
 NAME = "alibabacloud_linkedmallretrieval20240501" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud LinkedmallRetrieval (20240501) SDK Library for Python"
```

