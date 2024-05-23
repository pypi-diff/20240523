# Comparing `tmp/zhrism-0.0.2.tar.gz` & `tmp/zhrism-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zhrism-0.0.2.tar", last modified: Thu May 23 10:34:01 2024, max compression
+gzip compressed data, was "zhrism-0.0.3.tar", last modified: Thu May 23 10:40:04 2024, max compression
```

## Comparing `zhrism-0.0.2.tar` & `zhrism-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 10:34:01.543051 zhrism-0.0.2/
--rw-rw-rw-   0        0        0      213 2024-05-23 10:34:01.543051 zhrism-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      291 2024-05-23 10:16:32.000000 zhrism-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-23 10:34:01.537055 zhrism-0.0.2/rsm/
--rw-rw-rw-   0        0        0        0 2024-05-23 04:54:08.000000 zhrism-0.0.2/rsm/__init__.py
--rw-rw-rw-   0        0        0       42 2024-05-23 10:34:01.544051 zhrism-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1056 2024-05-23 10:33:28.000000 zhrism-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-23 10:34:01.542051 zhrism-0.0.2/zhrism.egg-info/
--rw-rw-rw-   0        0        0      213 2024-05-23 10:34:01.000000 zhrism-0.0.2/zhrism.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      154 2024-05-23 10:34:01.000000 zhrism-0.0.2/zhrism.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 10:34:01.000000 zhrism-0.0.2/zhrism.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2024-05-23 10:34:01.000000 zhrism-0.0.2/zhrism.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-23 10:40:04.852584 zhrism-0.0.3/
+-rw-rw-rw-   0        0        0      213 2024-05-23 10:40:04.851587 zhrism-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      291 2024-05-23 10:16:32.000000 zhrism-0.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-23 10:40:04.852584 zhrism-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      784 2024-05-23 10:39:43.000000 zhrism-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 10:40:04.845589 zhrism-0.0.3/zhrism/
+-rw-rw-rw-   0        0        0        0 2024-05-23 04:54:08.000000 zhrism-0.0.3/zhrism/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 10:40:04.850583 zhrism-0.0.3/zhrism.egg-info/
+-rw-rw-rw-   0        0        0      213 2024-05-23 10:40:04.000000 zhrism-0.0.3/zhrism.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      157 2024-05-23 10:40:04.000000 zhrism-0.0.3/zhrism.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 10:40:04.000000 zhrism-0.0.3/zhrism.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-23 10:40:04.000000 zhrism-0.0.3/zhrism.egg-info/top_level.txt
```

### Comparing `zhrism-0.0.2/setup.py` & `zhrism-0.0.3/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,27 +1,14 @@
-import os
-import sys
-import shutil
-import re
-
-path_list = ['build', 'dist', 'zh_rsm/zh_rsm.egg-info']
-for path in path_list:
-    if os.path.exists(path):
-        shutil.rmtree(path)
-        # os.unlink(path)
-    else:
-        print('no such file:%s' % path)
-
 
 def main():
     from distutils.core import setup
     from setuptools import find_packages
 
     setup(name='zhrism',  # 包名
-          version='0.0.2',  # 版本号
+          version='0.0.3',  # 版本号
           description='',
           long_description='',
           author='yzh2002',
           author_email='2039143115@qq.com',
           url='',
           license='',
           install_requires=[],
```

