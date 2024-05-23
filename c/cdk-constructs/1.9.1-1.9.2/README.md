# Comparing `tmp/cdk-constructs-1.9.1.tar.gz` & `tmp/cdk-constructs-1.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-constructs-1.9.1.tar", last modified: Tue May 21 18:33:26 2024, max compression
+gzip compressed data, was "cdk-constructs-1.9.2.tar", last modified: Thu May 23 18:06:08 2024, max compression
```

## Comparing `cdk-constructs-1.9.1.tar` & `cdk-constructs-1.9.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:33:26.367089 cdk-constructs-1.9.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-05-21 18:33:16.000000 cdk-constructs-1.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-21 18:33:16.000000 cdk-constructs-1.9.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4359 2024-05-21 18:33:26.367089 cdk-constructs-1.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3457 2024-05-21 18:33:16.000000 cdk-constructs-1.9.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-21 18:33:16.000000 cdk-constructs-1.9.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 18:33:26.367089 cdk-constructs-1.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-21 18:33:16.000000 cdk-constructs-1.9.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:33:26.367089 cdk-constructs-1.9.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:33:26.367089 cdk-constructs-1.9.1/src/cdk-constructs/
--rw-r--r--   0 runner    (1001) docker     (127)    55680 2024-05-21 18:33:16.000000 cdk-constructs-1.9.1/src/cdk-constructs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:33:26.367089 cdk-constructs-1.9.1/src/cdk-constructs/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-21 18:33:16.000000 cdk-constructs-1.9.1/src/cdk-constructs/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    42768 2024-05-21 18:33:16.000000 cdk-constructs-1.9.1/src/cdk-constructs/_jsii/cdk-constructs@1.9.1.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 18:33:16.000000 cdk-constructs-1.9.1/src/cdk-constructs/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 18:33:26.367089 cdk-constructs-1.9.1/src/cdk_constructs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4359 2024-05-21 18:33:26.000000 cdk-constructs-1.9.1/src/cdk_constructs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-21 18:33:26.000000 cdk-constructs-1.9.1/src/cdk_constructs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 18:33:26.000000 cdk-constructs-1.9.1/src/cdk_constructs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-21 18:33:26.000000 cdk-constructs-1.9.1/src/cdk_constructs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-21 18:33:26.000000 cdk-constructs-1.9.1/src/cdk_constructs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:06:08.708700 cdk-constructs-1.9.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-05-23 18:05:57.000000 cdk-constructs-1.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-23 18:05:57.000000 cdk-constructs-1.9.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4359 2024-05-23 18:06:08.708700 cdk-constructs-1.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3457 2024-05-23 18:05:57.000000 cdk-constructs-1.9.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-23 18:05:57.000000 cdk-constructs-1.9.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 18:06:08.708700 cdk-constructs-1.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-05-23 18:05:57.000000 cdk-constructs-1.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:06:08.704700 cdk-constructs-1.9.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:06:08.708700 cdk-constructs-1.9.2/src/cdk-constructs/
+-rw-r--r--   0 runner    (1001) docker     (127)    55680 2024-05-23 18:05:57.000000 cdk-constructs-1.9.2/src/cdk-constructs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:06:08.708700 cdk-constructs-1.9.2/src/cdk-constructs/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-05-23 18:05:57.000000 cdk-constructs-1.9.2/src/cdk-constructs/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43134 2024-05-23 18:05:57.000000 cdk-constructs-1.9.2/src/cdk-constructs/_jsii/cdk-constructs@1.9.2.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 18:05:57.000000 cdk-constructs-1.9.2/src/cdk-constructs/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:06:08.708700 cdk-constructs-1.9.2/src/cdk_constructs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4359 2024-05-23 18:06:08.000000 cdk-constructs-1.9.2/src/cdk_constructs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-23 18:06:08.000000 cdk-constructs-1.9.2/src/cdk_constructs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 18:06:08.000000 cdk-constructs-1.9.2/src/cdk_constructs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-23 18:06:08.000000 cdk-constructs-1.9.2/src/cdk_constructs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-23 18:06:08.000000 cdk-constructs-1.9.2/src/cdk_constructs.egg-info/top_level.txt
```

### Comparing `cdk-constructs-1.9.1/LICENSE` & `cdk-constructs-1.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-constructs-1.9.1/PKG-INFO` & `cdk-constructs-1.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-constructs
-Version: 1.9.1
+Version: 1.9.2
 Summary: A CDK construct library
 Home-page: https://github.com/tm-lcarvalho/cdk-constructs.git
 Author: tm-lcarvalho<lucio.carvalho@toumoro.com>
 License: GPL-3.0-or-later
 Project-URL: Source, https://github.com/tm-lcarvalho/cdk-constructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-constructs-1.9.1/README.md` & `cdk-constructs-1.9.2/README.md`

 * *Files identical despite different names*

### Comparing `cdk-constructs-1.9.1/setup.py` & `cdk-constructs-1.9.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-constructs",
-    "version": "1.9.1",
+    "version": "1.9.2",
     "description": "A CDK construct library",
     "license": "GPL-3.0-or-later",
     "url": "https://github.com/tm-lcarvalho/cdk-constructs.git",
     "long_description_content_type": "text/markdown",
     "author": "tm-lcarvalho<lucio.carvalho@toumoro.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,23 +22,24 @@
     },
     "packages": [
         "cdk-constructs",
         "cdk-constructs._jsii"
     ],
     "package_data": {
         "cdk-constructs._jsii": [
-            "cdk-constructs@1.9.1.jsii.tgz"
+            "cdk-constructs@1.9.2.jsii.tgz"
         ],
         "cdk-constructs": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
         "aws-cdk-lib>=2.140.0, <3.0.0",
+        "cdk-nag>=2.28.120, <3.0.0",
         "constructs>=10.0.5, <11.0.0",
         "jsii>=1.96.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
```

### Comparing `cdk-constructs-1.9.1/src/cdk-constructs/__init__.py` & `cdk-constructs-1.9.2/src/cdk-constructs/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-constructs-1.9.1/src/cdk_constructs.egg-info/PKG-INFO` & `cdk-constructs-1.9.2/src/cdk_constructs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-constructs
-Version: 1.9.1
+Version: 1.9.2
 Summary: A CDK construct library
 Home-page: https://github.com/tm-lcarvalho/cdk-constructs.git
 Author: tm-lcarvalho<lucio.carvalho@toumoro.com>
 License: GPL-3.0-or-later
 Project-URL: Source, https://github.com/tm-lcarvalho/cdk-constructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

