# Comparing `tmp/chatchat-0.0.8.tar.gz` & `tmp/chatchat-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatchat-0.0.8.tar", last modified: Wed May 22 10:58:40 2024, max compression
+gzip compressed data, was "chatchat-0.0.9.tar", last modified: Wed May 22 14:16:59 2024, max compression
```

## Comparing `chatchat-0.0.8.tar` & `chatchat-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:58:40.843257 chatchat-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-05-22 10:58:34.000000 chatchat-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-22 10:58:40.843257 chatchat-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 10:58:34.000000 chatchat-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:58:40.843257 chatchat-0.0.8/chatchat/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-22 10:58:34.000000 chatchat-0.0.8/chatchat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3901 2024-05-22 10:58:34.000000 chatchat-0.0.8/chatchat/baidu.py
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-22 10:58:34.000000 chatchat-0.0.8/chatchat/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6012 2024-05-22 10:58:34.000000 chatchat-0.0.8/chatchat/xunfei.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:58:40.843257 chatchat-0.0.8/chatchat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-22 10:58:40.000000 chatchat-0.0.8/chatchat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-22 10:58:40.000000 chatchat-0.0.8/chatchat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 10:58:40.000000 chatchat-0.0.8/chatchat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-22 10:58:40.000000 chatchat-0.0.8/chatchat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-22 10:58:40.000000 chatchat-0.0.8/chatchat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 10:58:40.843257 chatchat-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-22 10:58:34.000000 chatchat-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:16:59.964593 chatchat-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-05-22 14:16:55.000000 chatchat-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-22 14:16:59.964593 chatchat-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 14:16:55.000000 chatchat-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:16:59.960593 chatchat-0.0.9/chatchat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 14:16:55.000000 chatchat-0.0.9/chatchat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-05-22 14:16:55.000000 chatchat-0.0.9/chatchat/alibaba.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3901 2024-05-22 14:16:55.000000 chatchat-0.0.9/chatchat/baidu.py
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-22 14:16:55.000000 chatchat-0.0.9/chatchat/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6012 2024-05-22 14:16:55.000000 chatchat-0.0.9/chatchat/xunfei.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:16:59.964593 chatchat-0.0.9/chatchat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-22 14:16:59.000000 chatchat-0.0.9/chatchat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-22 14:16:59.000000 chatchat-0.0.9/chatchat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 14:16:59.000000 chatchat-0.0.9/chatchat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-22 14:16:59.000000 chatchat-0.0.9/chatchat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-22 14:16:59.000000 chatchat-0.0.9/chatchat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 14:16:59.964593 chatchat-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-22 14:16:55.000000 chatchat-0.0.9/setup.py
```

### Comparing `chatchat-0.0.8/LICENSE` & `chatchat-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `chatchat-0.0.8/PKG-INFO` & `chatchat-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatchat
-Version: 0.0.8
+Version: 0.0.9
 Summary: Large Language Model API
 Home-page: https://github.com/JiauZhang/chatchat
 Author: JiauZhang
 Author-email: jiauzhang@163.com
 License: GPL-2.0
 Keywords: llm,chatapi,chatbot
 Classifier: Intended Audience :: Developers
```

### Comparing `chatchat-0.0.8/chatchat/baidu.py` & `chatchat-0.0.9/chatchat/baidu.py`

 * *Files identical despite different names*

### Comparing `chatchat-0.0.8/chatchat/xunfei.py` & `chatchat-0.0.9/chatchat/xunfei.py`

 * *Files identical despite different names*

### Comparing `chatchat-0.0.8/chatchat.egg-info/PKG-INFO` & `chatchat-0.0.9/chatchat.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatchat
-Version: 0.0.8
+Version: 0.0.9
 Summary: Large Language Model API
 Home-page: https://github.com/JiauZhang/chatchat
 Author: JiauZhang
 Author-email: jiauzhang@163.com
 License: GPL-2.0
 Keywords: llm,chatapi,chatbot
 Classifier: Intended Audience :: Developers
```

### Comparing `chatchat-0.0.8/setup.py` & `chatchat-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name = 'chatchat',
     packages = find_packages(exclude=['examples']),
-    version = '0.0.8',
+    version = '0.0.9',
     license = 'GPL-2.0',
     description = 'Large Language Model API',
     author = 'JiauZhang',
     author_email = 'jiauzhang@163.com',
     url = 'https://github.com/JiauZhang/chatchat',
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type = 'text/markdown',
```

