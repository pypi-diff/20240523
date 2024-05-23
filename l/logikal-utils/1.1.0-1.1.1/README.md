# Comparing `tmp/logikal_utils-1.1.0.tar.gz` & `tmp/logikal_utils-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logikal_utils-1.1.0.tar", last modified: Wed May 22 09:20:56 2024, max compression
+gzip compressed data, was "logikal_utils-1.1.1.tar", last modified: Thu May 23 17:29:03 2024, max compression
```

## Comparing `logikal_utils-1.1.0.tar` & `logikal_utils-1.1.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 09:20:56.081870 logikal_utils-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-22 09:20:40.000000 logikal_utils-1.1.0/.copier-answers.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-22 09:20:40.000000 logikal_utils-1.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-22 09:20:40.000000 logikal_utils-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-05-22 09:20:56.081870 logikal_utils-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-22 09:20:40.000000 logikal_utils-1.1.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-22 09:20:40.000000 logikal_utils-1.1.0/compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 09:20:56.077870 logikal_utils-1.1.0/logikal_utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 09:20:40.000000 logikal_utils-1.1.0/logikal_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4573 2024-05-22 09:20:40.000000 logikal_utils-1.1.0/logikal_utils/docker.py
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-22 09:20:40.000000 logikal_utils-1.1.0/logikal_utils/project.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 09:20:40.000000 logikal_utils-1.1.0/logikal_utils/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 09:20:56.077870 logikal_utils-1.1.0/logikal_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-05-22 09:20:56.000000 logikal_utils-1.1.0/logikal_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-22 09:20:56.000000 logikal_utils-1.1.0/logikal_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 09:20:56.000000 logikal_utils-1.1.0/logikal_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-22 09:20:56.000000 logikal_utils-1.1.0/logikal_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-22 09:20:56.000000 logikal_utils-1.1.0/logikal_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-05-22 09:20:40.000000 logikal_utils-1.1.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 09:20:56.077870 logikal_utils-1.1.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-22 09:20:40.000000 logikal_utils-1.1.0/requirements/build.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-22 09:20:40.000000 logikal_utils-1.1.0/requirements/build.txt.lock
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-22 09:20:40.000000 logikal_utils-1.1.0/requirements/core.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-22 09:20:40.000000 logikal_utils-1.1.0/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-05-22 09:20:40.000000 logikal_utils-1.1.0/requirements/dev.txt.lock
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-22 09:20:40.000000 logikal_utils-1.1.0/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-22 09:20:40.000000 logikal_utils-1.1.0/requirements/docs.txt.lock
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 09:20:56.077870 logikal_utils-1.1.0/requirements/extras/
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-22 09:20:40.000000 logikal_utils-1.1.0/requirements/extras/docker.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 09:20:56.081870 logikal_utils-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:29:03.354398 logikal_utils-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-23 17:28:49.000000 logikal_utils-1.1.1/.copier-answers.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-23 17:28:49.000000 logikal_utils-1.1.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-23 17:28:49.000000 logikal_utils-1.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-05-23 17:29:03.354398 logikal_utils-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-23 17:28:49.000000 logikal_utils-1.1.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-23 17:28:49.000000 logikal_utils-1.1.1/compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:29:03.350398 logikal_utils-1.1.1/logikal_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 17:28:49.000000 logikal_utils-1.1.1/logikal_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4573 2024-05-23 17:28:49.000000 logikal_utils-1.1.1/logikal_utils/docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-23 17:28:49.000000 logikal_utils-1.1.1/logikal_utils/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 17:28:49.000000 logikal_utils-1.1.1/logikal_utils/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:29:03.354398 logikal_utils-1.1.1/logikal_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-05-23 17:29:03.000000 logikal_utils-1.1.1/logikal_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      563 2024-05-23 17:29:03.000000 logikal_utils-1.1.1/logikal_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 17:29:03.000000 logikal_utils-1.1.1/logikal_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-23 17:29:03.000000 logikal_utils-1.1.1/logikal_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-23 17:29:03.000000 logikal_utils-1.1.1/logikal_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-05-23 17:28:49.000000 logikal_utils-1.1.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:29:03.354398 logikal_utils-1.1.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-23 17:28:49.000000 logikal_utils-1.1.1/requirements/build.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-23 17:28:49.000000 logikal_utils-1.1.1/requirements/build.txt.lock
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-23 17:28:49.000000 logikal_utils-1.1.1/requirements/core.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-23 17:28:49.000000 logikal_utils-1.1.1/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-05-23 17:28:49.000000 logikal_utils-1.1.1/requirements/dev.txt.lock
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-23 17:28:49.000000 logikal_utils-1.1.1/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-05-23 17:28:49.000000 logikal_utils-1.1.1/requirements/docs.txt.lock
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 17:29:03.354398 logikal_utils-1.1.1/requirements/extras/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-23 17:28:49.000000 logikal_utils-1.1.1/requirements/extras/docker.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 17:29:03.354398 logikal_utils-1.1.1/setup.cfg
```

### Comparing `logikal_utils-1.1.0/.copier-answers.yml` & `logikal_utils-1.1.1/.copier-answers.yml`

 * *Files identical despite different names*

### Comparing `logikal_utils-1.1.0/LICENSE.txt` & `logikal_utils-1.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `logikal_utils-1.1.0/PKG-INFO` & `logikal_utils-1.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logikal-utils
-Version: 1.1.0
+Version: 1.1.1
 Summary: Common Python utilities used at Logikal
 Author-email: Logikal GmbH <contact@logikal.io>
 License: Copyright 2023 Logikal GmbH
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and
         associated documentation files (the "Software"), to deal in the Software without restriction,
         including without limitation the rights to use, copy, modify, merge, publish, distribute,
@@ -35,17 +35,15 @@
 Classifier: Typing :: Typed
 Requires-Python: ~=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 Requires-Dist: termcolor~=2.4
 Requires-Dist: tomli~=2.0
 Provides-Extra: docker
-Requires-Dist: docker~=7.0; extra == "docker"
-Requires-Dist: requests<2.32; extra == "docker"
-Requires-Dist: types-requests<2.32; extra == "docker"
+Requires-Dist: docker~=7.1; extra == "docker"
 
 logikal-utils
 =============
 Common Python utilities used at Logikal.
 
 Getting Started
 ---------------
```

### Comparing `logikal_utils-1.1.0/logikal_utils/docker.py` & `logikal_utils-1.1.1/logikal_utils/docker.py`

 * *Files identical despite different names*

### Comparing `logikal_utils-1.1.0/logikal_utils.egg-info/PKG-INFO` & `logikal_utils-1.1.1/logikal_utils.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logikal-utils
-Version: 1.1.0
+Version: 1.1.1
 Summary: Common Python utilities used at Logikal
 Author-email: Logikal GmbH <contact@logikal.io>
 License: Copyright 2023 Logikal GmbH
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and
         associated documentation files (the "Software"), to deal in the Software without restriction,
         including without limitation the rights to use, copy, modify, merge, publish, distribute,
@@ -35,17 +35,15 @@
 Classifier: Typing :: Typed
 Requires-Python: ~=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 Requires-Dist: termcolor~=2.4
 Requires-Dist: tomli~=2.0
 Provides-Extra: docker
-Requires-Dist: docker~=7.0; extra == "docker"
-Requires-Dist: requests<2.32; extra == "docker"
-Requires-Dist: types-requests<2.32; extra == "docker"
+Requires-Dist: docker~=7.1; extra == "docker"
 
 logikal-utils
 =============
 Common Python utilities used at Logikal.
 
 Getting Started
 ---------------
```

### Comparing `logikal_utils-1.1.0/logikal_utils.egg-info/SOURCES.txt` & `logikal_utils-1.1.1/logikal_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `logikal_utils-1.1.0/pyproject.toml` & `logikal_utils-1.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `logikal_utils-1.1.0/requirements/build.txt.lock` & `logikal_utils-1.1.1/requirements/build.txt.lock`

 * *Files identical despite different names*

### Comparing `logikal_utils-1.1.0/requirements/dev.txt.lock` & `logikal_utils-1.1.1/requirements/dev.txt.lock`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ###################################################################################################
 ##
 ##  DO NOT EDIT THIS FILE.
 ##  This is a locked requirements file generated by pyorbs.
 ##
-##  Requirements hash: f7da736a3e836f66831f6d8f08bc5e5e69f04ad41877fcb30b62bd52008a53ce
+##  Requirements hash: 40dddfdbe060965cc37d766bda9517bcf7b28ce7aacb372ae039a7bfd76126f0
 ##
 ###################################################################################################
 -e .
 alabaster==0.7.13
 astroid==3.2.2
 attrs==23.2.0
 Babel==2.15.0
@@ -17,15 +17,15 @@
 certifi==2024.2.2
 cffi==1.16.0
 charset-normalizer==3.3.2
 colorama==0.4.6
 coverage==7.5.1
 cryptography==42.0.7
 dill==0.3.8
-docker==7.0.0
+docker==7.1.0
 docutils==0.20.1
 exceptiongroup==1.2.1
 execnet==2.1.1
 filelock==3.14.0
 idna==3.7
 imagesize==1.4.1
 importlib_metadata==7.1.0
@@ -57,27 +57,27 @@
 pluggy==1.5.0
 prettytable==3.10.0
 psutil==5.9.8
 pycodestyle==2.11.1
 pycparser==2.22
 pydocstyle==6.3.0
 Pygments==2.18.0
-pylint==3.2.0
+pylint==3.2.2
 pyorbs==2.1.0
 pyproject_hooks==1.1.0
-pytest==8.2.0
+pytest==8.2.1
 pytest-cov==5.0.0
-pytest-logikal==3.0.0
+pytest-logikal==3.1.0
 pytest-mock==3.14.0
 pytest-mypy==0.10.3
 pytest-xdist==3.6.1
 pytz==2024.1
 PyYAML==6.0.1
 readme_renderer==43.0
-requests==2.31.0
+requests==2.32.2
 requests-toolbelt==1.0.0
 rfc3986==2.0.0
 rich==13.7.1
 SecretStorage==3.3.3
 setuptools==70.0.0
 snowballstemmer==2.2.0
 Sphinx==7.1.2
@@ -90,13 +90,12 @@
 sphinxcontrib-qthelp==1.0.3
 sphinxcontrib-serializinghtml==1.1.5
 stevedore==5.2.0
 termcolor==2.4.0
 tomli==2.0.1
 tomlkit==0.12.5
 twine==5.1.0
-types-requests==2.31.0.20240406
 typing_extensions==4.11.0
 urllib3==2.2.1
 wcwidth==0.2.13
 wheel==0.43.0
 zipp==3.18.2
```

### Comparing `logikal_utils-1.1.0/requirements/docs.txt.lock` & `logikal_utils-1.1.1/requirements/docs.txt.lock`

 * *Files 25% similar despite different names*

```diff
@@ -1,43 +1,42 @@
 ###################################################################################################
 ##
 ##  DO NOT EDIT THIS FILE.
 ##  This is a locked requirements file generated by pyorbs.
 ##
-##  Requirements hash: c6bcc16e1beca628be6ad4cccd1e490a8d027c814b421c05364e0e7fc7ef0ae4
+##  Requirements hash: e936906dcc1b8bbba7ad6f9a3e1579f1bec73f53e69887bb04bcead1ae285745
 ##
 ###################################################################################################
 -e .
 alabaster==0.7.13
 Babel==2.15.0
 certifi==2024.2.2
 charset-normalizer==3.3.2
-docker==7.0.0
+docker==7.1.0
 docutils==0.20.1
 idna==3.7
 imagesize==1.4.1
 importlib_metadata==7.1.0
 Jinja2==3.1.4
 logikal-docs==1.1.4
 MarkupSafe==2.1.5
 packaging==23.2
 pip==24.0
 Pygments==2.18.0
 pytz==2024.1
-requests==2.31.0
+requests==2.32.2
 setuptools==70.0.0
 snowballstemmer==2.2.0
 Sphinx==7.1.2
 sphinx-rtd-theme==2.0.0
 sphinxcontrib-applehelp==1.0.4
 sphinxcontrib-devhelp==1.0.2
 sphinxcontrib-htmlhelp==2.0.1
 sphinxcontrib-jquery==4.1
 sphinxcontrib-jsmath==1.0.1
 sphinxcontrib-qthelp==1.0.3
 sphinxcontrib-serializinghtml==1.1.5
 termcolor==2.4.0
 tomli==2.0.1
-types-requests==2.31.0.20240406
 urllib3==2.2.1
 wheel==0.43.0
 zipp==3.18.2
```

