# Comparing `tmp/zhrism-0.0.3.tar.gz` & `tmp/zhrism-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zhrism-0.0.3.tar", last modified: Thu May 23 10:40:04 2024, max compression
+gzip compressed data, was "zhrism-0.0.4.tar", last modified: Thu May 23 10:44:37 2024, max compression
```

## Comparing `zhrism-0.0.3.tar` & `zhrism-0.0.4.tar`

### file list

```diff
@@ -1,12 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 10:40:04.852584 zhrism-0.0.3/
--rw-rw-rw-   0        0        0      213 2024-05-23 10:40:04.851587 zhrism-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      291 2024-05-23 10:16:32.000000 zhrism-0.0.3/README.md
--rw-rw-rw-   0        0        0       42 2024-05-23 10:40:04.852584 zhrism-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      784 2024-05-23 10:39:43.000000 zhrism-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-23 10:40:04.845589 zhrism-0.0.3/zhrism/
--rw-rw-rw-   0        0        0        0 2024-05-23 04:54:08.000000 zhrism-0.0.3/zhrism/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-23 10:40:04.850583 zhrism-0.0.3/zhrism.egg-info/
--rw-rw-rw-   0        0        0      213 2024-05-23 10:40:04.000000 zhrism-0.0.3/zhrism.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      157 2024-05-23 10:40:04.000000 zhrism-0.0.3/zhrism.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 10:40:04.000000 zhrism-0.0.3/zhrism.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-23 10:40:04.000000 zhrism-0.0.3/zhrism.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-23 10:44:37.081538 zhrism-0.0.4/
+-rw-rw-rw-   0        0        0      213 2024-05-23 10:44:37.080539 zhrism-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      291 2024-05-23 10:16:32.000000 zhrism-0.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-23 10:44:37.081538 zhrism-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      784 2024-05-23 10:44:33.000000 zhrism-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 10:44:37.062540 zhrism-0.0.4/zhrism/
+-rw-rw-rw-   0        0        0        0 2024-05-23 04:54:08.000000 zhrism-0.0.4/zhrism/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 10:44:37.077537 zhrism-0.0.4/zhrism/basic/
+-rw-rw-rw-   0        0        0        0 2024-05-23 10:43:04.000000 zhrism-0.0.4/zhrism/basic/__init__.py
+-rw-rw-rw-   0        0        0      838 2024-05-23 07:59:23.000000 zhrism-0.0.4/zhrism/basic/activation.py
+-rw-rw-rw-   0        0        0     3427 2024-05-23 06:40:55.000000 zhrism-0.0.4/zhrism/basic/features.py
+-rw-rw-rw-   0        0        0      415 2024-05-23 06:31:25.000000 zhrism-0.0.4/zhrism/basic/initializers.py
+-rw-rw-rw-   0        0        0     9264 2024-05-23 07:59:48.000000 zhrism-0.0.4/zhrism/basic/layers.py
+drwxrwxrwx   0        0        0        0 2024-05-23 10:44:37.077537 zhrism-0.0.4/zhrism/models/
+-rw-rw-rw-   0        0        0        0 2024-05-23 10:42:49.000000 zhrism-0.0.4/zhrism/models/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 10:44:37.078539 zhrism-0.0.4/zhrism/models/match/
+-rw-rw-rw-   0        0        0     3336 2024-05-23 10:08:44.000000 zhrism-0.0.4/zhrism/models/match/YouTubeDNN.py
+-rw-rw-rw-   0        0        0        0 2024-05-23 10:43:51.000000 zhrism-0.0.4/zhrism/models/match/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-23 10:44:37.079539 zhrism-0.0.4/zhrism/utils/
+-rw-rw-rw-   0        0        0        0 2024-05-23 10:43:14.000000 zhrism-0.0.4/zhrism/utils/__init__.py
+-rw-rw-rw-   0        0        0      313 2024-05-23 06:37:41.000000 zhrism-0.0.4/zhrism/utils/data.py
+drwxrwxrwx   0        0        0        0 2024-05-23 10:44:37.080539 zhrism-0.0.4/zhrism.egg-info/
+-rw-rw-rw-   0        0        0      213 2024-05-23 10:44:36.000000 zhrism-0.0.4/zhrism.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      424 2024-05-23 10:44:37.000000 zhrism-0.0.4/zhrism.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 10:44:36.000000 zhrism-0.0.4/zhrism.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-23 10:44:36.000000 zhrism-0.0.4/zhrism.egg-info/top_level.txt
```

### Comparing `zhrism-0.0.3/setup.py` & `zhrism-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 def main():
     from distutils.core import setup
     from setuptools import find_packages
 
     setup(name='zhrism',  # 包名
-          version='0.0.3',  # 版本号
+          version='0.0.4',  # 版本号
           description='',
           long_description='',
           author='yzh2002',
           author_email='2039143115@qq.com',
           url='',
           license='',
           install_requires=[],
```

