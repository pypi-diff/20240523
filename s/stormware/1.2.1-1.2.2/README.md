# Comparing `tmp/stormware-1.2.1.tar.gz` & `tmp/stormware-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stormware-1.2.1.tar", last modified: Sat Jan 27 00:53:51 2024, max compression
+gzip compressed data, was "stormware-1.2.2.tar", last modified: Thu May 23 18:40:15 2024, max compression
```

## Comparing `stormware-1.2.1.tar` & `stormware-1.2.2.tar`

### file list

```diff
@@ -1,42 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 00:53:51.218152 stormware-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-01-27 00:53:29.000000 stormware-1.2.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-01-27 00:53:29.000000 stormware-1.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-01-27 00:53:51.218152 stormware-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-01-27 00:53:29.000000 stormware-1.2.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-01-27 00:53:29.000000 stormware-1.2.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 00:53:51.214152 stormware-1.2.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-01-27 00:53:29.000000 stormware-1.2.1/requirements/build.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-01-27 00:53:29.000000 stormware-1.2.1/requirements/build.txt.lock
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-01-27 00:53:29.000000 stormware-1.2.1/requirements/core.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-01-27 00:53:29.000000 stormware-1.2.1/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4097 2024-01-27 00:53:29.000000 stormware-1.2.1/requirements/dev.txt.lock
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-01-27 00:53:29.000000 stormware-1.2.1/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3251 2024-01-27 00:53:29.000000 stormware-1.2.1/requirements/docs.txt.lock
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 00:53:51.214152 stormware-1.2.1/requirements/extras/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-01-27 00:53:29.000000 stormware-1.2.1/requirements/extras/amazon.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-01-27 00:53:29.000000 stormware-1.2.1/requirements/extras/facebook.txt
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-01-27 00:53:29.000000 stormware-1.2.1/requirements/extras/google.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-27 00:53:51.218152 stormware-1.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 00:53:51.214152 stormware-1.2.1/stormware/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 00:53:29.000000 stormware-1.2.1/stormware/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 00:53:51.218152 stormware-1.2.1/stormware/amazon/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 00:53:29.000000 stormware-1.2.1/stormware/amazon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-01-27 00:53:29.000000 stormware-1.2.1/stormware/amazon/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-01-27 00:53:29.000000 stormware-1.2.1/stormware/amazon/secrets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-01-27 00:53:29.000000 stormware-1.2.1/stormware/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-01-27 00:53:29.000000 stormware-1.2.1/stormware/client_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     5833 2024-01-27 00:53:29.000000 stormware-1.2.1/stormware/facebook.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 00:53:51.218152 stormware-1.2.1/stormware/google/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 00:53:29.000000 stormware-1.2.1/stormware/google/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3782 2024-01-27 00:53:29.000000 stormware-1.2.1/stormware/google/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-01-27 00:53:29.000000 stormware-1.2.1/stormware/google/bigquery.py
--rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-01-27 00:53:29.000000 stormware-1.2.1/stormware/google/secrets.py
--rw-r--r--   0 runner    (1001) docker     (127)     7853 2024-01-27 00:53:29.000000 stormware-1.2.1/stormware/google/sheets.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-27 00:53:29.000000 stormware-1.2.1/stormware/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-01-27 00:53:29.000000 stormware-1.2.1/stormware/secrets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-27 00:53:51.218152 stormware-1.2.1/stormware.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3179 2024-01-27 00:53:51.000000 stormware-1.2.1/stormware.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-01-27 00:53:51.000000 stormware-1.2.1/stormware.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-27 00:53:51.000000 stormware-1.2.1/stormware.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-01-27 00:53:51.000000 stormware-1.2.1/stormware.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-01-27 00:53:51.000000 stormware-1.2.1/stormware.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:40:15.328079 stormware-1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-23 18:39:58.000000 stormware-1.2.2/.copier-answers.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-23 18:39:58.000000 stormware-1.2.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-23 18:39:58.000000 stormware-1.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-05-23 18:40:15.328079 stormware-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-23 18:39:58.000000 stormware-1.2.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-05-23 18:39:58.000000 stormware-1.2.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:40:15.324079 stormware-1.2.2/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-23 18:39:58.000000 stormware-1.2.2/requirements/build.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-23 18:39:58.000000 stormware-1.2.2/requirements/build.txt.lock
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-23 18:39:58.000000 stormware-1.2.2/requirements/core.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-23 18:39:58.000000 stormware-1.2.2/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4174 2024-05-23 18:39:58.000000 stormware-1.2.2/requirements/dev.txt.lock
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-23 18:39:58.000000 stormware-1.2.2/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3254 2024-05-23 18:39:58.000000 stormware-1.2.2/requirements/docs.txt.lock
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:40:15.324079 stormware-1.2.2/requirements/extras/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 18:39:58.000000 stormware-1.2.2/requirements/extras/amazon.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-23 18:39:58.000000 stormware-1.2.2/requirements/extras/facebook.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-23 18:39:58.000000 stormware-1.2.2/requirements/extras/google.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 18:40:15.328079 stormware-1.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:40:15.324079 stormware-1.2.2/stormware/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 18:39:58.000000 stormware-1.2.2/stormware/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:40:15.328079 stormware-1.2.2/stormware/amazon/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 18:39:58.000000 stormware-1.2.2/stormware/amazon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1649 2024-05-23 18:39:58.000000 stormware-1.2.2/stormware/amazon/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-05-23 18:39:58.000000 stormware-1.2.2/stormware/amazon/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-23 18:39:58.000000 stormware-1.2.2/stormware/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-23 18:39:58.000000 stormware-1.2.2/stormware/client_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5833 2024-05-23 18:39:58.000000 stormware-1.2.2/stormware/facebook.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:40:15.328079 stormware-1.2.2/stormware/google/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 18:39:58.000000 stormware-1.2.2/stormware/google/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3782 2024-05-23 18:39:58.000000 stormware-1.2.2/stormware/google/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-05-23 18:39:58.000000 stormware-1.2.2/stormware/google/bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-05-23 18:39:58.000000 stormware-1.2.2/stormware/google/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7853 2024-05-23 18:39:58.000000 stormware-1.2.2/stormware/google/sheets.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 18:39:58.000000 stormware-1.2.2/stormware/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-05-23 18:39:58.000000 stormware-1.2.2/stormware/secrets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 18:40:15.328079 stormware-1.2.2/stormware.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3181 2024-05-23 18:40:15.000000 stormware-1.2.2/stormware.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-23 18:40:15.000000 stormware-1.2.2/stormware.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 18:40:15.000000 stormware-1.2.2/stormware.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-23 18:40:15.000000 stormware-1.2.2/stormware.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-23 18:40:15.000000 stormware-1.2.2/stormware.egg-info/top_level.txt
```

### Comparing `stormware-1.2.1/LICENSE.txt` & `stormware-1.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `stormware-1.2.1/PKG-INFO` & `stormware-1.2.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stormware
-Version: 1.2.1
+Version: 1.2.2
 Summary: API connectors for data analysis and task automation
 Author-email: Logikal GmbH <contact@logikal.io>
 License: Copyright 2023 Logikal GmbH
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and
         associated documentation files (the "Software"), to deal in the Software without restriction,
         including without limitation the rights to use, copy, modify, merge, publish, distribute,
@@ -32,31 +32,31 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Python: ~=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
-Requires-Dist: logikal-utils~=1.0
+Requires-Dist: logikal-utils~=1.1
 Requires-Dist: pandas[performance]~=2.0
 Requires-Dist: pandas-stubs~=2.0
 Requires-Dist: xdg~=5.1
 Provides-Extra: google
-Requires-Dist: google-api-python-client==2.115.0; extra == "google"
-Requires-Dist: google-api-python-client-stubs==1.23.0; extra == "google"
-Requires-Dist: google-auth==2.27.0; extra == "google"
+Requires-Dist: google-api-python-client==2.130.0; extra == "google"
+Requires-Dist: google-api-python-client-stubs==1.26.0; extra == "google"
+Requires-Dist: google-auth==2.29.0; extra == "google"
 Requires-Dist: google-auth-stubs==0.2.0; extra == "google"
-Requires-Dist: google-cloud-bigquery[pandas]~=3.14; extra == "google"
-Requires-Dist: google-cloud-secret-manager==2.17.0; extra == "google"
+Requires-Dist: google-cloud-bigquery[pandas]~=3.23; extra == "google"
+Requires-Dist: google-cloud-secret-manager==2.20.0; extra == "google"
 Requires-Dist: google-crc32c==1.5.0; extra == "google"
 Provides-Extra: amazon
-Requires-Dist: boto3==1.34.29; extra == "amazon"
-Requires-Dist: boto3-stubs==1.34.29; extra == "amazon"
+Requires-Dist: boto3==1.34.111; extra == "amazon"
+Requires-Dist: boto3-stubs==1.34.111; extra == "amazon"
 Provides-Extra: facebook
-Requires-Dist: facebook-business==19.0.0; extra == "facebook"
+Requires-Dist: facebook-business==19.0.3; extra == "facebook"
 
 Stormware
 =========
 API connectors for data analysis and task automation.
 
 Getting Started
 ---------------
```

### Comparing `stormware-1.2.1/pyproject.toml` & `stormware-1.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `stormware-1.2.1/requirements/build.txt.lock` & `stormware-1.2.2/requirements/build.txt.lock`

 * *Files 15% similar despite different names*

```diff
@@ -1,43 +1,46 @@
 ###################################################################################################
 ##
 ##  DO NOT EDIT THIS FILE.
 ##  This is a locked requirements file generated by pyorbs.
 ##
-##  Requirements hash: 5cb1a368e35962412e4230ef67a622b3ed950d02d59c40d132b27e3a685ef8f8
+##  Requirements hash: 8706de2163a25299dbe1d5d6f26df03b6aaaad435e67227452ee6c0b2b97aea0
 ##
 ###################################################################################################
-build==1.0.3
-certifi==2023.11.17
+backports.tarfile==1.1.1
+build==1.2.1
+certifi==2024.2.2
 cffi==1.16.0
 charset-normalizer==3.3.2
-cryptography==41.0.7
+cryptography==42.0.7
 docutils==0.20.1
-idna==3.6
-importlib-metadata==7.0.0
-importlib-resources==6.1.1
-jaraco.classes==3.3.0
+idna==3.7
+importlib_metadata==7.1.0
+importlib_resources==6.4.0
+jaraco.classes==3.4.0
+jaraco.context==5.3.0
+jaraco.functools==4.0.1
 jeepney==0.8.0
-keyring==24.3.0
+keyring==25.2.1
 markdown-it-py==3.0.0
 mdurl==0.1.2
-more-itertools==10.1.0
-nh3==0.2.15
-packaging==23.2
-pip==23.3.2
-pkginfo==1.9.6
-pycparser==2.21
-Pygments==2.17.2
-pyproject_hooks==1.0.0
-readme-renderer==42.0
-requests==2.31.0
+more-itertools==10.2.0
+nh3==0.2.17
+packaging==24.0
+pip==24.0
+pkginfo==1.10.0
+pycparser==2.22
+Pygments==2.18.0
+pyproject_hooks==1.1.0
+readme_renderer==43.0
+requests==2.32.2
 requests-toolbelt==1.0.0
 rfc3986==2.0.0
-rich==13.7.0
+rich==13.7.1
 SecretStorage==3.3.3
-setuptools==69.0.2
+setuptools==70.0.0
 tomli==2.0.1
-twine==4.0.2
-typing_extensions==4.9.0
-urllib3==2.1.0
-wheel==0.42.0
-zipp==3.17.0
+twine==5.1.0
+typing_extensions==4.11.0
+urllib3==2.2.1
+wheel==0.43.0
+zipp==3.18.2
```

### Comparing `stormware-1.2.1/requirements/dev.txt.lock` & `stormware-1.2.2/requirements/dev.txt.lock`

 * *Files 12% similar despite different names*

```diff
@@ -1,203 +1,205 @@
 ###################################################################################################
 ##
 ##  DO NOT EDIT THIS FILE.
 ##  This is a locked requirements file generated by pyorbs.
 ##
-##  Requirements hash: 4036d4fbf76815b5976b5be27e7f879e8aa74c1670152228013366d740963222
+##  Requirements hash: 0fd9b67562c04a595521796effb2e8cdf165bb3fd56e86c09419909a9034cfae
 ##
 ###################################################################################################
 -e .
-aiohttp==3.9.1
+aiohttp==3.9.5
 aiosignal==1.3.1
 alabaster==0.7.13
-astroid==3.0.2
+astroid==3.2.2
 asttokens==2.4.1
 async-timeout==4.0.3
 attrs==23.2.0
-Babel==2.14.0
+Babel==2.15.0
 backcall==0.2.0
-bandit==1.7.7
+backports.tarfile==1.1.1
+bandit==1.7.8
 beautifulsoup4==4.12.3
 bleach==6.1.0
-boto3==1.34.29
-boto3-stubs==1.34.29
-botocore==1.34.29
-botocore-stubs==1.34.29
-Bottleneck==1.3.7
-build==1.0.3
-cachetools==5.3.2
-certifi==2023.11.17
+boto3==1.34.111
+boto3-stubs==1.34.111
+botocore==1.34.111
+botocore-stubs==1.34.94
+Bottleneck==1.3.8
+build==1.2.1
+cachetools==5.3.3
+certifi==2024.2.2
 cffi==1.16.0
 charset-normalizer==3.3.2
 colorama==0.4.6
-comm==0.2.1
-coverage==7.4.1
-cryptography==42.0.1
+comm==0.2.2
+coverage==7.5.1
+cryptography==42.0.7
 curlify==2.2.1
 db-dtypes==1.2.0
-debugpy==1.8.0
+debugpy==1.8.1
 decorator==5.1.1
 defusedxml==0.7.1
-dill==0.3.7
+dill==0.3.8
 docutils==0.20.1
-enum34==1.1.10
-exceptiongroup==1.2.0
-execnet==2.0.2
+exceptiongroup==1.2.1
+execnet==2.1.1
 executing==2.0.1
-facebook_business==19.0.0
+facebook_business==19.0.3
 fastjsonschema==2.19.1
-filelock==3.13.1
+filelock==3.14.0
 frozenlist==1.4.1
-google-api-core==2.15.0
-google-api-python-client==2.115.0
-google-api-python-client-stubs==1.23.0
-google-auth==2.27.0
+google-api-core==2.19.0
+google-api-python-client==2.130.0
+google-api-python-client-stubs==1.26.0
+google-auth==2.29.0
 google-auth-httplib2==0.2.0
 google-auth-stubs==0.2.0
-google-cloud-bigquery==3.17.1
+google-cloud-bigquery==3.23.1
 google-cloud-core==2.4.1
-google-cloud-secret-manager==2.17.0
+google-cloud-secret-manager==2.20.0
 google-crc32c==1.5.0
 google-resumable-media==2.7.0
-googleapis-common-protos==1.62.0
+googleapis-common-protos==1.63.0
 grpc-google-iam-v1==0.13.0
 grpc-stubs==1.53.0.5
-grpcio==1.60.0
-grpcio-status==1.60.0
+grpcio==1.64.0
+grpcio-status==1.62.2
 httplib2==0.22.0
-idna==3.6
+idna==3.7
 imagesize==1.4.1
-importlib-metadata==7.0.1
 importlib-resources==5.13.0
+importlib_metadata==7.1.0
 iniconfig==2.0.0
-ipykernel==6.29.0
+ipykernel==6.29.4
 ipython==8.12.3
-ipywidgets==8.1.1
+ipywidgets==8.1.2
 isort==5.13.2
-jaraco.classes==3.3.0
+jaraco.classes==3.4.0
+jaraco.context==5.3.0
+jaraco.functools==4.0.1
 jedi==0.19.1
 jeepney==0.8.0
-Jinja2==3.1.3
+Jinja2==3.1.4
 jmespath==1.0.1
-jsonschema==4.21.1
+jsonschema==4.22.0
 jsonschema-specifications==2023.12.1
 jupyter-sphinx==0.5.3
-jupyter_client==8.6.0
-jupyter_core==5.7.1
-jupyterlab-widgets==3.0.9
+jupyter_client==8.6.2
+jupyter_core==5.7.2
 jupyterlab_pygments==0.3.0
-keyring==24.3.0
+jupyterlab_widgets==3.0.10
+keyring==25.2.1
 llvmlite==0.41.1
 logikal-docs==1.1.4
-logikal-utils==1.0.1
+logikal-utils==1.1.1
 markdown-it-py==3.0.0
-MarkupSafe==2.1.4
-matplotlib-inline==0.1.6
+MarkupSafe==2.1.5
+matplotlib-inline==0.1.7
 mccabe==0.7.0
 mdurl==0.1.2
 mistune==3.0.2
 more-itertools==10.2.0
-multidict==6.0.4
-mypy==1.8.0
+multidict==6.0.5
+mypy==1.10.0
 mypy-extensions==1.0.0
-nbclient==0.9.0
-nbconvert==7.14.2
-nbformat==5.9.2
+nbclient==0.10.0
+nbconvert==7.16.4
+nbformat==5.10.4
 nest-asyncio==1.6.0
-nh3==0.2.15
+nh3==0.2.17
 numba==0.58.1
 numexpr==2.8.6
 numpy==1.24.4
 packaging==23.2
 pandas==2.0.3
 pandas-stubs==2.0.3.230814
 pandocfilters==1.5.1
-parso==0.8.3
+parso==0.8.4
 pbr==6.0.0
 pexpect==4.9.0
 pickleshare==0.7.5
-pillow==10.2.0
-pip==23.3.2
-pip-licenses==4.3.4
-pkginfo==1.9.6
+pillow==10.3.0
+pip==24.0
+pip-licenses==4.4.0
+pkginfo==1.10.0
 pkgutil_resolve_name==1.3.10
-platformdirs==4.1.0
-pluggy==1.3.0
-prettytable==3.9.0
+platformdirs==4.2.2
+pluggy==1.5.0
+prettytable==3.10.0
 prompt-toolkit==3.0.43
 proto-plus==1.23.0
-protobuf==4.25.2
+protobuf==4.25.3
 psutil==5.9.8
 ptyprocess==0.7.0
 pure-eval==0.2.2
-pyarrow==15.0.0
-pyasn1==0.5.1
-pyasn1-modules==0.3.0
+pyarrow==16.1.0
+pyasn1==0.6.0
+pyasn1_modules==0.4.0
 pycodestyle==2.11.1
 pycountry==23.12.11
-pycparser==2.21
+pycparser==2.22
 pydocstyle==6.3.0
-Pygments==2.17.2
-pylint==3.0.3
+Pygments==2.18.0
+pylint==3.2.2
 pyorbs==2.1.0
-pyparsing==3.1.1
-pyproject_hooks==1.0.0
-pytest==7.4.4
-pytest-cov==4.1.0
-pytest-logikal==2.0.2
-pytest-mock==3.12.0
+pyparsing==3.1.2
+pyproject_hooks==1.1.0
+pytest==8.2.1
+pytest-cov==5.0.0
+pytest-logikal==3.2.0
+pytest-mock==3.14.0
 pytest-mypy==0.10.3
-pytest-xdist==3.5.0
-python-dateutil==2.8.2
-pytz==2023.3.post1
+pytest-xdist==3.6.1
+python-dateutil==2.9.0.post0
+pytz==2024.1
 PyYAML==6.0.1
-pyzmq==25.1.2
-readme-renderer==42.0
-referencing==0.32.1
-requests==2.31.0
+pyzmq==26.0.3
+readme_renderer==43.0
+referencing==0.35.1
+requests==2.32.2
 requests-toolbelt==1.0.0
 rfc3986==2.0.0
-rich==13.7.0
-rpds-py==0.17.1
+rich==13.7.1
+rpds-py==0.18.1
 rsa==4.9
-s3transfer==0.10.0
+s3transfer==0.10.1
 SecretStorage==3.3.3
-setuptools==69.0.3
+setuptools==70.0.0
 six==1.16.0
 snowballstemmer==2.2.0
 soupsieve==2.5
 Sphinx==7.1.2
 sphinx-rtd-theme==2.0.0
 sphinxcontrib-applehelp==1.0.4
 sphinxcontrib-devhelp==1.0.2
 sphinxcontrib-htmlhelp==2.0.1
 sphinxcontrib-jquery==4.1
 sphinxcontrib-jsmath==1.0.1
 sphinxcontrib-qthelp==1.0.3
 sphinxcontrib-serializinghtml==1.1.5
 stack-data==0.6.3
-stevedore==5.1.0
+stevedore==5.2.0
 termcolor==2.4.0
-tinycss2==1.2.1
+tinycss2==1.3.0
 tomli==2.0.1
-tomlkit==0.12.3
+tomlkit==0.12.5
 tornado==6.4
-traitlets==5.14.1
-twine==4.0.2
-types-awscrt==0.20.2
-types-httplib2==0.22.0.2
-types-pytz==2023.3.1.1
+traitlets==5.14.3
+twine==5.1.0
+types-awscrt==0.20.9
+types-httplib2==0.22.0.20240310
+types-pytz==2024.1.0.20240417
 types-requests==2.31.0.6
-types-s3transfer==0.10.0
+types-s3transfer==0.10.1
 types-urllib3==1.26.25.14
-typing_extensions==4.9.0
-tzdata==2023.4
+typing_extensions==4.11.0
+tzdata==2024.1
 uritemplate==4.1.1
 urllib3==1.26.18
 wcwidth==0.2.13
 webencodings==0.5.1
-wheel==0.42.0
-widgetsnbextension==4.0.9
+wheel==0.43.0
+widgetsnbextension==4.0.10
 xdg==5.1.1
 yarl==1.9.4
-zipp==3.17.0
+zipp==3.18.2
```

### Comparing `stormware-1.2.1/requirements/docs.txt.lock` & `stormware-1.2.2/requirements/docs.txt.lock`

 * *Files 6% similar despite different names*

```diff
@@ -1,153 +1,152 @@
 ###################################################################################################
 ##
 ##  DO NOT EDIT THIS FILE.
 ##  This is a locked requirements file generated by pyorbs.
 ##
-##  Requirements hash: 12b5d9b092a126a471518d785be65574e034a625cf1767d6fc38d0b43d7dc25d
+##  Requirements hash: 8d3c83fb5588a272f94d64b513f011dc658bd35cf9bcc1e797519c4cda5ecebd
 ##
 ###################################################################################################
 -e .
-aiohttp==3.9.1
+aiohttp==3.9.5
 aiosignal==1.3.1
 alabaster==0.7.13
 asttokens==2.4.1
 async-timeout==4.0.3
 attrs==23.2.0
-Babel==2.14.0
+Babel==2.15.0
 backcall==0.2.0
 beautifulsoup4==4.12.3
 bleach==6.1.0
-boto3==1.34.29
-boto3-stubs==1.34.29
-botocore==1.34.29
-botocore-stubs==1.34.29
-Bottleneck==1.3.7
-cachetools==5.3.2
-certifi==2023.11.17
+boto3==1.34.111
+boto3-stubs==1.34.111
+botocore==1.34.111
+botocore-stubs==1.34.94
+Bottleneck==1.3.8
+cachetools==5.3.3
+certifi==2024.2.2
 charset-normalizer==3.3.2
-comm==0.2.1
+comm==0.2.2
 curlify==2.2.1
 db-dtypes==1.2.0
-debugpy==1.8.0
+debugpy==1.8.1
 decorator==5.1.1
 defusedxml==0.7.1
 docutils==0.20.1
-enum34==1.1.10
 executing==2.0.1
-facebook_business==19.0.0
+facebook_business==19.0.3
 fastjsonschema==2.19.1
 frozenlist==1.4.1
-google-api-core==2.15.0
-google-api-python-client==2.115.0
-google-api-python-client-stubs==1.23.0
-google-auth==2.27.0
+google-api-core==2.19.0
+google-api-python-client==2.130.0
+google-api-python-client-stubs==1.26.0
+google-auth==2.29.0
 google-auth-httplib2==0.2.0
 google-auth-stubs==0.2.0
-google-cloud-bigquery==3.17.1
+google-cloud-bigquery==3.23.1
 google-cloud-core==2.4.1
-google-cloud-secret-manager==2.17.0
+google-cloud-secret-manager==2.20.0
 google-crc32c==1.5.0
 google-resumable-media==2.7.0
-googleapis-common-protos==1.62.0
+googleapis-common-protos==1.63.0
 grpc-google-iam-v1==0.13.0
 grpc-stubs==1.53.0.5
-grpcio==1.60.0
-grpcio-status==1.60.0
+grpcio==1.64.0
+grpcio-status==1.62.2
 httplib2==0.22.0
-idna==3.6
+idna==3.7
 imagesize==1.4.1
-importlib-metadata==7.0.1
 importlib-resources==5.13.0
-ipykernel==6.29.0
+importlib_metadata==7.1.0
+ipykernel==6.29.4
 ipython==8.12.3
-ipywidgets==8.1.1
+ipywidgets==8.1.2
 jedi==0.19.1
-Jinja2==3.1.3
+Jinja2==3.1.4
 jmespath==1.0.1
-jsonschema==4.21.1
+jsonschema==4.22.0
 jsonschema-specifications==2023.12.1
 jupyter-sphinx==0.5.3
-jupyter_client==8.6.0
-jupyter_core==5.7.1
-jupyterlab-widgets==3.0.9
+jupyter_client==8.6.2
+jupyter_core==5.7.2
 jupyterlab_pygments==0.3.0
+jupyterlab_widgets==3.0.10
 llvmlite==0.41.1
 logikal-docs==1.1.4
-logikal-utils==1.0.1
-MarkupSafe==2.1.4
-matplotlib-inline==0.1.6
+logikal-utils==1.1.1
+MarkupSafe==2.1.5
+matplotlib-inline==0.1.7
 mistune==3.0.2
-multidict==6.0.4
-nbclient==0.9.0
-nbconvert==7.14.2
-nbformat==5.9.2
+multidict==6.0.5
+nbclient==0.10.0
+nbconvert==7.16.4
+nbformat==5.10.4
 nest-asyncio==1.6.0
 numba==0.58.1
 numexpr==2.8.6
 numpy==1.24.4
 packaging==23.2
 pandas==2.0.3
 pandas-stubs==2.0.3.230814
 pandocfilters==1.5.1
-parso==0.8.3
+parso==0.8.4
 pexpect==4.9.0
 pickleshare==0.7.5
-pip==23.3.2
+pip==24.0
 pkgutil_resolve_name==1.3.10
-platformdirs==4.1.0
+platformdirs==4.2.2
 prompt-toolkit==3.0.43
 proto-plus==1.23.0
-protobuf==4.25.2
+protobuf==4.25.3
 psutil==5.9.8
 ptyprocess==0.7.0
 pure-eval==0.2.2
-pyarrow==15.0.0
-pyasn1==0.5.1
-pyasn1-modules==0.3.0
+pyarrow==16.1.0
+pyasn1==0.6.0
+pyasn1_modules==0.4.0
 pycountry==23.12.11
-Pygments==2.17.2
-pyparsing==3.1.1
-python-dateutil==2.8.2
-pytz==2023.3.post1
-pyzmq==25.1.2
-referencing==0.32.1
-requests==2.31.0
-rpds-py==0.17.1
+Pygments==2.18.0
+pyparsing==3.1.2
+python-dateutil==2.9.0.post0
+pytz==2024.1
+pyzmq==26.0.3
+referencing==0.35.1
+requests==2.32.2
+rpds-py==0.18.1
 rsa==4.9
-s3transfer==0.10.0
-setuptools==69.0.3
+s3transfer==0.10.1
+setuptools==70.0.0
 six==1.16.0
 snowballstemmer==2.2.0
 soupsieve==2.5
 Sphinx==7.1.2
 sphinx-rtd-theme==2.0.0
 sphinxcontrib-applehelp==1.0.4
 sphinxcontrib-devhelp==1.0.2
 sphinxcontrib-htmlhelp==2.0.1
 sphinxcontrib-jquery==4.1
 sphinxcontrib-jsmath==1.0.1
 sphinxcontrib-qthelp==1.0.3
 sphinxcontrib-serializinghtml==1.1.5
 stack-data==0.6.3
 termcolor==2.4.0
-tinycss2==1.2.1
+tinycss2==1.3.0
 tomli==2.0.1
 tornado==6.4
-traitlets==5.14.1
-types-awscrt==0.20.2
-types-httplib2==0.22.0.2
-types-pytz==2023.3.1.1
+traitlets==5.14.3
+types-awscrt==0.20.9
+types-httplib2==0.22.0.20240310
+types-pytz==2024.1.0.20240417
 types-requests==2.31.0.6
-types-s3transfer==0.10.0
+types-s3transfer==0.10.1
 types-urllib3==1.26.25.14
-typing_extensions==4.9.0
-tzdata==2023.4
+typing_extensions==4.11.0
+tzdata==2024.1
 uritemplate==4.1.1
 urllib3==1.26.18
 wcwidth==0.2.13
 webencodings==0.5.1
-wheel==0.42.0
-widgetsnbextension==4.0.9
+wheel==0.43.0
+widgetsnbextension==4.0.10
 xdg==5.1.1
 yarl==1.9.4
-zipp==3.17.0
+zipp==3.18.2
```

### Comparing `stormware-1.2.1/stormware/amazon/auth.py` & `stormware-1.2.2/stormware/amazon/auth.py`

 * *Files identical despite different names*

### Comparing `stormware-1.2.1/stormware/amazon/secrets.py` & `stormware-1.2.2/stormware/amazon/secrets.py`

 * *Files identical despite different names*

### Comparing `stormware-1.2.1/stormware/auth.py` & `stormware-1.2.2/stormware/auth.py`

 * *Files identical despite different names*

### Comparing `stormware-1.2.1/stormware/client_manager.py` & `stormware-1.2.2/stormware/client_manager.py`

 * *Files identical despite different names*

### Comparing `stormware-1.2.1/stormware/facebook.py` & `stormware-1.2.2/stormware/facebook.py`

 * *Files identical despite different names*

### Comparing `stormware-1.2.1/stormware/google/auth.py` & `stormware-1.2.2/stormware/google/auth.py`

 * *Files identical despite different names*

### Comparing `stormware-1.2.1/stormware/google/bigquery.py` & `stormware-1.2.2/stormware/google/bigquery.py`

 * *Files identical despite different names*

### Comparing `stormware-1.2.1/stormware/google/secrets.py` & `stormware-1.2.2/stormware/google/secrets.py`

 * *Files identical despite different names*

### Comparing `stormware-1.2.1/stormware/google/sheets.py` & `stormware-1.2.2/stormware/google/sheets.py`

 * *Files identical despite different names*

### Comparing `stormware-1.2.1/stormware/secrets.py` & `stormware-1.2.2/stormware/secrets.py`

 * *Files identical despite different names*

### Comparing `stormware-1.2.1/stormware.egg-info/PKG-INFO` & `stormware-1.2.2/stormware.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stormware
-Version: 1.2.1
+Version: 1.2.2
 Summary: API connectors for data analysis and task automation
 Author-email: Logikal GmbH <contact@logikal.io>
 License: Copyright 2023 Logikal GmbH
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and
         associated documentation files (the "Software"), to deal in the Software without restriction,
         including without limitation the rights to use, copy, modify, merge, publish, distribute,
@@ -32,31 +32,31 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Python: ~=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
-Requires-Dist: logikal-utils~=1.0
+Requires-Dist: logikal-utils~=1.1
 Requires-Dist: pandas[performance]~=2.0
 Requires-Dist: pandas-stubs~=2.0
 Requires-Dist: xdg~=5.1
 Provides-Extra: google
-Requires-Dist: google-api-python-client==2.115.0; extra == "google"
-Requires-Dist: google-api-python-client-stubs==1.23.0; extra == "google"
-Requires-Dist: google-auth==2.27.0; extra == "google"
+Requires-Dist: google-api-python-client==2.130.0; extra == "google"
+Requires-Dist: google-api-python-client-stubs==1.26.0; extra == "google"
+Requires-Dist: google-auth==2.29.0; extra == "google"
 Requires-Dist: google-auth-stubs==0.2.0; extra == "google"
-Requires-Dist: google-cloud-bigquery[pandas]~=3.14; extra == "google"
-Requires-Dist: google-cloud-secret-manager==2.17.0; extra == "google"
+Requires-Dist: google-cloud-bigquery[pandas]~=3.23; extra == "google"
+Requires-Dist: google-cloud-secret-manager==2.20.0; extra == "google"
 Requires-Dist: google-crc32c==1.5.0; extra == "google"
 Provides-Extra: amazon
-Requires-Dist: boto3==1.34.29; extra == "amazon"
-Requires-Dist: boto3-stubs==1.34.29; extra == "amazon"
+Requires-Dist: boto3==1.34.111; extra == "amazon"
+Requires-Dist: boto3-stubs==1.34.111; extra == "amazon"
 Provides-Extra: facebook
-Requires-Dist: facebook-business==19.0.0; extra == "facebook"
+Requires-Dist: facebook-business==19.0.3; extra == "facebook"
 
 Stormware
 =========
 API connectors for data analysis and task automation.
 
 Getting Started
 ---------------
```

### Comparing `stormware-1.2.1/stormware.egg-info/SOURCES.txt` & `stormware-1.2.2/stormware.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+.copier-answers.yml
 LICENSE.txt
 MANIFEST.in
 README.rst
 pyproject.toml
 requirements/build.txt
 requirements/build.txt.lock
 requirements/core.txt
```

