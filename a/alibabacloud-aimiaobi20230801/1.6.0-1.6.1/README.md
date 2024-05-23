# Comparing `tmp/alibabacloud_aimiaobi20230801-1.6.0.tar.gz` & `tmp/alibabacloud_aimiaobi20230801-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_aimiaobi20230801-1.6.0.tar", last modified: Wed May 15 02:03:47 2024, max compression
+gzip compressed data, was "dist/alibabacloud_aimiaobi20230801-1.6.1.tar", last modified: Thu May 23 06:32:39 2024, max compression
```

## Comparing `alibabacloud_aimiaobi20230801-1.6.0.tar` & `alibabacloud_aimiaobi20230801-1.6.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 02:03:47.000000 alibabacloud_aimiaobi20230801-1.6.0/
--rw-r--r--   0 root         (0) root         (0)     1549 2024-05-15 02:03:45.000000 alibabacloud_aimiaobi20230801-1.6.0/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-05-15 02:03:45.000000 alibabacloud_aimiaobi20230801-1.6.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-05-15 02:03:45.000000 alibabacloud_aimiaobi20230801-1.6.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2436 2024-05-15 02:03:47.000000 alibabacloud_aimiaobi20230801-1.6.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1115 2024-05-15 02:03:45.000000 alibabacloud_aimiaobi20230801-1.6.0/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1200 2024-05-15 02:03:45.000000 alibabacloud_aimiaobi20230801-1.6.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 02:03:47.000000 alibabacloud_aimiaobi20230801-1.6.0/alibabacloud_aimiaobi20230801/
--rw-r--r--   0 root         (0) root         (0)       21 2024-05-15 02:03:45.000000 alibabacloud_aimiaobi20230801-1.6.0/alibabacloud_aimiaobi20230801/__init__.py
--rw-r--r--   0 root         (0) root         (0)   229176 2024-05-15 02:03:45.000000 alibabacloud_aimiaobi20230801-1.6.0/alibabacloud_aimiaobi20230801/client.py
--rw-r--r--   0 root         (0) root         (0)   394960 2024-05-15 02:03:45.000000 alibabacloud_aimiaobi20230801-1.6.0/alibabacloud_aimiaobi20230801/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 02:03:47.000000 alibabacloud_aimiaobi20230801-1.6.0/alibabacloud_aimiaobi20230801.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2436 2024-05-15 02:03:47.000000 alibabacloud_aimiaobi20230801-1.6.0/alibabacloud_aimiaobi20230801.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      460 2024-05-15 02:03:47.000000 alibabacloud_aimiaobi20230801-1.6.0/alibabacloud_aimiaobi20230801.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-15 02:03:47.000000 alibabacloud_aimiaobi20230801-1.6.0/alibabacloud_aimiaobi20230801.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2024-05-15 02:03:47.000000 alibabacloud_aimiaobi20230801-1.6.0/alibabacloud_aimiaobi20230801.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       30 2024-05-15 02:03:47.000000 alibabacloud_aimiaobi20230801-1.6.0/alibabacloud_aimiaobi20230801.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-05-15 02:03:47.000000 alibabacloud_aimiaobi20230801-1.6.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2636 2024-05-15 02:03:45.000000 alibabacloud_aimiaobi20230801-1.6.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:32:39.000000 alibabacloud_aimiaobi20230801-1.6.1/
+-rw-r--r--   0 root         (0) root         (0)     1611 2024-05-23 06:32:38.000000 alibabacloud_aimiaobi20230801-1.6.1/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-05-23 06:32:38.000000 alibabacloud_aimiaobi20230801-1.6.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-05-23 06:32:38.000000 alibabacloud_aimiaobi20230801-1.6.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2436 2024-05-23 06:32:39.000000 alibabacloud_aimiaobi20230801-1.6.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1115 2024-05-23 06:32:38.000000 alibabacloud_aimiaobi20230801-1.6.1/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1200 2024-05-23 06:32:38.000000 alibabacloud_aimiaobi20230801-1.6.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:32:39.000000 alibabacloud_aimiaobi20230801-1.6.1/alibabacloud_aimiaobi20230801/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-05-23 06:32:38.000000 alibabacloud_aimiaobi20230801-1.6.1/alibabacloud_aimiaobi20230801/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   229176 2024-05-23 06:32:38.000000 alibabacloud_aimiaobi20230801-1.6.1/alibabacloud_aimiaobi20230801/client.py
+-rw-r--r--   0 root         (0) root         (0)   394960 2024-05-23 06:32:38.000000 alibabacloud_aimiaobi20230801-1.6.1/alibabacloud_aimiaobi20230801/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:32:39.000000 alibabacloud_aimiaobi20230801-1.6.1/alibabacloud_aimiaobi20230801.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2436 2024-05-23 06:32:39.000000 alibabacloud_aimiaobi20230801-1.6.1/alibabacloud_aimiaobi20230801.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      460 2024-05-23 06:32:39.000000 alibabacloud_aimiaobi20230801-1.6.1/alibabacloud_aimiaobi20230801.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-23 06:32:39.000000 alibabacloud_aimiaobi20230801-1.6.1/alibabacloud_aimiaobi20230801.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2024-05-23 06:32:39.000000 alibabacloud_aimiaobi20230801-1.6.1/alibabacloud_aimiaobi20230801.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2024-05-23 06:32:39.000000 alibabacloud_aimiaobi20230801-1.6.1/alibabacloud_aimiaobi20230801.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-05-23 06:32:39.000000 alibabacloud_aimiaobi20230801-1.6.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2636 2024-05-23 06:32:38.000000 alibabacloud_aimiaobi20230801-1.6.1/setup.py
```

### Comparing `alibabacloud_aimiaobi20230801-1.6.0/ChangeLog.md` & `alibabacloud_aimiaobi20230801-1.6.1/ChangeLog.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+2024-05-15 Version: 1.6.0
+- Support API DocumentExtraction.
+
+
 2024-05-13 Version: 1.5.0
 - Support API DeleteCustomText.
 - Support API GetCustomText.
 - Support API ListCustomText.
 - Support API SaveCustomText.
 - Support API UpdateCustomText.
```

### Comparing `alibabacloud_aimiaobi20230801-1.6.0/LICENSE` & `alibabacloud_aimiaobi20230801-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_aimiaobi20230801-1.6.0/PKG-INFO` & `alibabacloud_aimiaobi20230801-1.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_aimiaobi20230801
-Version: 1.6.0
+Version: 1.6.1
 Summary: Alibaba Cloud AiMiaoBi (20230801) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_aimiaobi20230801-1.6.0/README-CN.md` & `alibabacloud_aimiaobi20230801-1.6.1/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_aimiaobi20230801-1.6.0/README.md` & `alibabacloud_aimiaobi20230801-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_aimiaobi20230801-1.6.0/alibabacloud_aimiaobi20230801/client.py` & `alibabacloud_aimiaobi20230801-1.6.1/alibabacloud_aimiaobi20230801/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_aimiaobi20230801-1.6.0/alibabacloud_aimiaobi20230801/models.py` & `alibabacloud_aimiaobi20230801-1.6.1/alibabacloud_aimiaobi20230801/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_aimiaobi20230801-1.6.0/alibabacloud_aimiaobi20230801.egg-info/PKG-INFO` & `alibabacloud_aimiaobi20230801-1.6.1/alibabacloud_aimiaobi20230801.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-aimiaobi20230801
-Version: 1.6.0
+Version: 1.6.1
 Summary: Alibaba Cloud AiMiaoBi (20230801) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_aimiaobi20230801-1.6.0/setup.py` & `alibabacloud_aimiaobi20230801-1.6.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_aimiaobi20230801.
 
-Created on 14/05/2024
+Created on 23/05/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_aimiaobi20230801"
 NAME = "alibabacloud_aimiaobi20230801" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud AiMiaoBi (20230801) SDK Library for Python"
```

