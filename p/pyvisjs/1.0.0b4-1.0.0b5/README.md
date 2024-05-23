# Comparing `tmp/pyvisjs-1.0.0b4.tar.gz` & `tmp/pyvisjs-1.0.0b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvisjs-1.0.0b4.tar", last modified: Sat May 18 09:09:44 2024, max compression
+gzip compressed data, was "pyvisjs-1.0.0b5.tar", last modified: Thu May 23 17:56:09 2024, max compression
```

## Comparing `pyvisjs-1.0.0b4.tar` & `pyvisjs-1.0.0b5.tar`

### file list

```diff
@@ -1,47 +1,63 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 09:09:44.687146 pyvisjs-1.0.0b4/
--rw-rw-rw-   0 root         (0) root         (0)     1396 2024-05-18 09:09:29.000000 pyvisjs-1.0.0b4/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     1818 2024-05-18 09:09:29.000000 pyvisjs-1.0.0b4/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)     5120 2024-05-18 09:09:29.000000 pyvisjs-1.0.0b4/CONTRIBUTING.md
--rw-rw-rw-   0 root         (0) root         (0)     1091 2024-05-18 09:09:29.000000 pyvisjs-1.0.0b4/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3331 2024-05-18 09:09:44.686146 pyvisjs-1.0.0b4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1404 2024-05-18 09:09:29.000000 pyvisjs-1.0.0b4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 09:09:44.679146 pyvisjs-1.0.0b4/examples/
--rw-rw-rw-   0 root         (0) root         (0)     8970 2024-05-18 09:09:29.000000 pyvisjs-1.0.0b4/examples/bluor.py
--rw-rw-rw-   0 root         (0) root         (0)      481 2024-05-18 09:09:29.000000 pyvisjs-1.0.0b4/examples/readme.py
--rw-rw-rw-   0 root         (0) root         (0)      959 2024-05-18 09:09:29.000000 pyvisjs-1.0.0b4/folder_structure.txt
--rw-rw-rw-   0 root         (0) root         (0)      890 2024-05-18 09:09:29.000000 pyvisjs-1.0.0b4/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 09:09:44.681146 pyvisjs-1.0.0b4/pyvisjs/
--rw-rw-rw-   0 root         (0) root         (0)      103 2024-05-18 09:09:29.000000 pyvisjs-1.0.0b4/pyvisjs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      103 2024-05-18 09:09:29.000000 pyvisjs-1.0.0b4/pyvisjs/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     2018 2024-05-18 09:09:29.000000 pyvisjs-1.0.0b4/pyvisjs/base_dictable.py
--rw-rw-rw-   0 root         (0) root         (0)     1274 2024-05-18 09:09:29.000000 pyvisjs-1.0.0b4/pyvisjs/edge.py
--rw-rw-rw-   0 root         (0) root         (0)    10718 2024-05-18 09:09:29.000000 pyvisjs-1.0.0b4/pyvisjs/network.py
--rw-rw-rw-   0 root         (0) root         (0)      590 2024-05-18 09:09:29.000000 pyvisjs-1.0.0b4/pyvisjs/node.py
--rw-rw-rw-   0 root         (0) root         (0)    13394 2024-05-18 09:09:29.000000 pyvisjs-1.0.0b4/pyvisjs/options.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 09:09:44.684146 pyvisjs-1.0.0b4/pyvisjs/templates/
--rw-rw-rw-   0 root         (0) root         (0)      966 2024-05-18 09:09:29.000000 pyvisjs-1.0.0b4/pyvisjs/templates/base.html
--rw-rw-rw-   0 root         (0) root         (0)      153 2024-05-18 09:09:29.000000 pyvisjs-1.0.0b4/pyvisjs/templates/basic.html
--rw-rw-rw-   0 root         (0) root         (0)     1193 2024-05-18 09:09:29.000000 pyvisjs-1.0.0b4/pyvisjs/templates/bs-container.html
--rw-rw-rw-   0 root         (0) root         (0)     1058 2024-05-18 09:09:29.000000 pyvisjs-1.0.0b4/pyvisjs/templates/create_network.js
--rw-rw-rw-   0 root         (0) root         (0)      926 2024-05-18 09:09:29.000000 pyvisjs-1.0.0b4/pyvisjs/templates/draw_title.js
--rw-rw-rw-   0 root         (0) root         (0)     7594 2024-05-18 09:09:29.000000 pyvisjs-1.0.0b4/pyvisjs/templates/functions.js
--rw-rw-rw-   0 root         (0) root         (0)      516 2024-05-18 09:09:29.000000 pyvisjs-1.0.0b4/pyvisjs/templates/init_tomSelect.js
--rw-rw-rw-   0 root         (0) root         (0)      840 2024-05-18 09:09:29.000000 pyvisjs-1.0.0b4/pyvisjs/templates/select-edge-filter.html
--rw-rw-rw-   0 root         (0) root         (0)     1704 2024-05-18 09:09:29.000000 pyvisjs-1.0.0b4/pyvisjs/templates/tom-select.html
--rw-rw-rw-   0 root         (0) root         (0)     1051 2024-05-18 09:09:29.000000 pyvisjs-1.0.0b4/pyvisjs/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 09:09:44.686146 pyvisjs-1.0.0b4/pyvisjs.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3331 2024-05-18 09:09:44.000000 pyvisjs-1.0.0b4/pyvisjs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      907 2024-05-18 09:09:44.000000 pyvisjs-1.0.0b4/pyvisjs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-18 09:09:44.000000 pyvisjs-1.0.0b4/pyvisjs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       43 2024-05-18 09:09:44.000000 pyvisjs-1.0.0b4/pyvisjs.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       28 2024-05-18 09:09:44.000000 pyvisjs-1.0.0b4/pyvisjs.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      109 2024-05-18 09:09:29.000000 pyvisjs-1.0.0b4/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-18 09:09:44.687146 pyvisjs-1.0.0b4/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-18 09:09:44.685146 pyvisjs-1.0.0b4/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-18 09:09:29.000000 pyvisjs-1.0.0b4/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1921 2024-05-18 09:09:29.000000 pyvisjs-1.0.0b4/tests/test_base_dictable.py
--rw-rw-rw-   0 root         (0) root         (0)     1006 2024-05-18 09:09:29.000000 pyvisjs-1.0.0b4/tests/test_edge.py
--rw-rw-rw-   0 root         (0) root         (0)    11958 2024-05-18 09:09:29.000000 pyvisjs-1.0.0b4/tests/test_network.py
--rw-rw-rw-   0 root         (0) root         (0)     2399 2024-05-18 09:09:29.000000 pyvisjs-1.0.0b4/tests/test_node.py
--rw-rw-rw-   0 root         (0) root         (0)     3863 2024-05-18 09:09:29.000000 pyvisjs-1.0.0b4/tests/test_options.py
--rw-rw-rw-   0 root         (0) root         (0)     2561 2024-05-18 09:09:29.000000 pyvisjs-1.0.0b4/tests/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:56:09.179188 pyvisjs-1.0.0b5/
+-rw-rw-rw-   0 root         (0) root         (0)     1396 2024-05-23 17:55:52.000000 pyvisjs-1.0.0b5/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     1975 2024-05-23 17:55:52.000000 pyvisjs-1.0.0b5/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)     5120 2024-05-23 17:55:52.000000 pyvisjs-1.0.0b5/CONTRIBUTING.md
+-rw-rw-rw-   0 root         (0) root         (0)     1091 2024-05-23 17:55:52.000000 pyvisjs-1.0.0b5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4040 2024-05-23 17:56:09.178188 pyvisjs-1.0.0b5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2113 2024-05-23 17:55:52.000000 pyvisjs-1.0.0b5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:56:09.169187 pyvisjs-1.0.0b5/docs/
+-rw-rw-rw-   0 root         (0) root         (0)       68 2024-05-23 17:55:52.000000 pyvisjs-1.0.0b5/docs/basic-example.md
+-rw-rw-rw-   0 root         (0) root         (0)       16 2024-05-23 17:55:52.000000 pyvisjs-1.0.0b5/docs/edges.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:56:09.170187 pyvisjs-1.0.0b5/docs/img/
+-rw-rw-rw-   0 root         (0) root         (0)      910 2024-05-23 17:55:52.000000 pyvisjs-1.0.0b5/docs/img/favicon-32x32.png
+-rw-rw-rw-   0 root         (0) root         (0)    15406 2024-05-23 17:55:52.000000 pyvisjs-1.0.0b5/docs/img/favicon.ico
+-rw-rw-rw-   0 root         (0) root         (0)      334 2024-05-23 17:55:52.000000 pyvisjs-1.0.0b5/docs/index.md
+-rw-rw-rw-   0 root         (0) root         (0)      419 2024-05-23 17:55:52.000000 pyvisjs-1.0.0b5/docs/installation.md
+-rw-rw-rw-   0 root         (0) root         (0)       20 2024-05-23 17:55:52.000000 pyvisjs-1.0.0b5/docs/network.md
+-rw-rw-rw-   0 root         (0) root         (0)       17 2024-05-23 17:55:52.000000 pyvisjs-1.0.0b5/docs/nodes.md
+-rw-rw-rw-   0 root         (0) root         (0)       19 2024-05-23 17:55:52.000000 pyvisjs-1.0.0b5/docs/options.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:56:09.170187 pyvisjs-1.0.0b5/docs_overrides/
+-rw-rw-rw-   0 root         (0) root         (0)     5058 2024-05-23 17:55:52.000000 pyvisjs-1.0.0b5/docs_overrides/dandelion.html
+-rw-rw-rw-   0 root         (0) root         (0)    32009 2024-05-23 17:55:52.000000 pyvisjs-1.0.0b5/docs_overrides/index.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:56:09.171187 pyvisjs-1.0.0b5/examples/
+-rw-rw-rw-   0 root         (0) root         (0)      718 2024-05-23 17:55:52.000000 pyvisjs-1.0.0b5/examples/basic-example.py
+-rw-rw-rw-   0 root         (0) root         (0)     2665 2024-05-23 17:55:52.000000 pyvisjs-1.0.0b5/examples/repo.py
+-rw-rw-rw-   0 root         (0) root         (0)      959 2024-05-23 17:55:52.000000 pyvisjs-1.0.0b5/folder_structure.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1466 2024-05-23 17:55:52.000000 pyvisjs-1.0.0b5/mkdocs.yml
+-rw-rw-rw-   0 root         (0) root         (0)      890 2024-05-23 17:55:52.000000 pyvisjs-1.0.0b5/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:56:09.173187 pyvisjs-1.0.0b5/pyvisjs/
+-rw-rw-rw-   0 root         (0) root         (0)      103 2024-05-23 17:55:52.000000 pyvisjs-1.0.0b5/pyvisjs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      103 2024-05-23 17:55:52.000000 pyvisjs-1.0.0b5/pyvisjs/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     2146 2024-05-23 17:55:52.000000 pyvisjs-1.0.0b5/pyvisjs/base_dictable.py
+-rw-rw-rw-   0 root         (0) root         (0)     1274 2024-05-23 17:55:52.000000 pyvisjs-1.0.0b5/pyvisjs/edge.py
+-rw-rw-rw-   0 root         (0) root         (0)    11282 2024-05-23 17:55:52.000000 pyvisjs-1.0.0b5/pyvisjs/network.py
+-rw-rw-rw-   0 root         (0) root         (0)      590 2024-05-23 17:55:52.000000 pyvisjs-1.0.0b5/pyvisjs/node.py
+-rw-rw-rw-   0 root         (0) root         (0)    13511 2024-05-23 17:55:52.000000 pyvisjs-1.0.0b5/pyvisjs/options.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:56:09.176187 pyvisjs-1.0.0b5/pyvisjs/templates/
+-rw-rw-rw-   0 root         (0) root         (0)      966 2024-05-23 17:55:52.000000 pyvisjs-1.0.0b5/pyvisjs/templates/base.html
+-rw-rw-rw-   0 root         (0) root         (0)      153 2024-05-23 17:55:52.000000 pyvisjs-1.0.0b5/pyvisjs/templates/basic.html
+-rw-rw-rw-   0 root         (0) root         (0)     1193 2024-05-23 17:55:52.000000 pyvisjs-1.0.0b5/pyvisjs/templates/bs-container.html
+-rw-rw-rw-   0 root         (0) root         (0)     1058 2024-05-23 17:55:52.000000 pyvisjs-1.0.0b5/pyvisjs/templates/create_network.js
+-rw-rw-rw-   0 root         (0) root         (0)      926 2024-05-23 17:55:52.000000 pyvisjs-1.0.0b5/pyvisjs/templates/draw_title.js
+-rw-rw-rw-   0 root         (0) root         (0)     7777 2024-05-23 17:55:52.000000 pyvisjs-1.0.0b5/pyvisjs/templates/functions.js
+-rw-rw-rw-   0 root         (0) root         (0)      605 2024-05-23 17:55:52.000000 pyvisjs-1.0.0b5/pyvisjs/templates/init_tomSelect.js
+-rw-rw-rw-   0 root         (0) root         (0)      840 2024-05-23 17:55:52.000000 pyvisjs-1.0.0b5/pyvisjs/templates/select-edge-filter.html
+-rw-rw-rw-   0 root         (0) root         (0)     1704 2024-05-23 17:55:52.000000 pyvisjs-1.0.0b5/pyvisjs/templates/tom-select.html
+-rw-rw-rw-   0 root         (0) root         (0)     1051 2024-05-23 17:55:52.000000 pyvisjs-1.0.0b5/pyvisjs/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:56:09.178188 pyvisjs-1.0.0b5/pyvisjs.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4040 2024-05-23 17:56:09.000000 pyvisjs-1.0.0b5/pyvisjs.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1166 2024-05-23 17:56:09.000000 pyvisjs-1.0.0b5/pyvisjs.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-23 17:56:09.000000 pyvisjs-1.0.0b5/pyvisjs.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       43 2024-05-23 17:56:09.000000 pyvisjs-1.0.0b5/pyvisjs.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       48 2024-05-23 17:56:09.000000 pyvisjs-1.0.0b5/pyvisjs.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-23 17:55:52.000000 pyvisjs-1.0.0b5/requirements-doc.txt
+-rw-rw-rw-   0 root         (0) root         (0)      109 2024-05-23 17:55:52.000000 pyvisjs-1.0.0b5/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-23 17:56:09.179188 pyvisjs-1.0.0b5/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 17:56:09.177188 pyvisjs-1.0.0b5/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-23 17:55:52.000000 pyvisjs-1.0.0b5/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1921 2024-05-23 17:55:52.000000 pyvisjs-1.0.0b5/tests/test_base_dictable.py
+-rw-rw-rw-   0 root         (0) root         (0)     1006 2024-05-23 17:55:52.000000 pyvisjs-1.0.0b5/tests/test_edge.py
+-rw-rw-rw-   0 root         (0) root         (0)    12201 2024-05-23 17:55:52.000000 pyvisjs-1.0.0b5/tests/test_network.py
+-rw-rw-rw-   0 root         (0) root         (0)     2399 2024-05-23 17:55:52.000000 pyvisjs-1.0.0b5/tests/test_node.py
+-rw-rw-rw-   0 root         (0) root         (0)     3863 2024-05-23 17:55:52.000000 pyvisjs-1.0.0b5/tests/test_options.py
+-rw-rw-rw-   0 root         (0) root         (0)     2561 2024-05-23 17:55:52.000000 pyvisjs-1.0.0b5/tests/test_utils.py
```

### Comparing `pyvisjs-1.0.0b4/.gitignore` & `pyvisjs-1.0.0b5/.gitignore`

 * *Files identical despite different names*

### Comparing `pyvisjs-1.0.0b4/.gitlab-ci.yml` & `pyvisjs-1.0.0b5/.gitlab-ci.yml`

 * *Files 18% similar despite different names*

```diff
@@ -1,43 +1,51 @@
 stages:
 #  - setup
-#  - build
+  - build
   - test
   - tag
   - release
   - deploy
 
 #variables:
 #  ENVIRONMENT: production
 
 before_script:
   - echo "Setting up environment..."
 
-#build:
-#  stage: build
-#  script:
-#    - echo "Building the application..."
+pages:
+  stage: deploy
+  image: python:latest
+  before_script:
+    - pip install -r requirements-doc.txt
+  script:
+    - mkdocs build --strict
+  artifacts:
+    paths:
+      - public
+  rules:
+    - changes:
+        - docs/*.*
+        - docs_overrides/*.*
+        - mkdocs.yml
+
 
 pytest_job:
   stage: test
   image: python:latest
   before_script:
     - pip install --upgrade pip
     - pip install -r requirements.txt
     - pip install -e .
   script:
     - pytest --noconftest
   rules:
     - changes:
         - pyvisjs/[^_]*.py
         - tests/*.py
-#  except:
-#    - dev
-#  only:
-#    - dev
 
 tagging_job:
   stage: tag
   image: python:latest
   rules:
     - if: '$CI_COMMIT_BRANCH == "main" && $CI_COMMIT_TITLE =~ /Merge branch.*/'
 #  only:
@@ -59,15 +67,15 @@
     - echo "running release_job"
   release:
     name: "Release $CI_COMMIT_TAG"
     tag_name: "$CI_COMMIT_TAG"
     description: "Release for version $CI_COMMIT_TAG"
 
 
-deploy_to_pypi_job:
+deploy_to_pages_job:
   stage: deploy
   image: python:latest
   before_script:
     - pip install --upgrade pip
     - pip install --upgrade setuptools
     - pip install --upgrade build
     - pip install --upgrade twine
```

### Comparing `pyvisjs-1.0.0b4/CONTRIBUTING.md` & `pyvisjs-1.0.0b5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pyvisjs-1.0.0b4/LICENSE` & `pyvisjs-1.0.0b5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyvisjs-1.0.0b4/PKG-INFO` & `pyvisjs-1.0.0b5/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvisjs
-Version: 1.0.0b4
+Version: 1.0.0b5
 Summary: A Python wrapper for vis.js Network
 Author-email: Andrey Morozov <andrey@morozov.lv>
 License: MIT License
         
         Copyright (c) 2024 Andrey Morozov (andrey@morozov.lv)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -35,19 +35,30 @@
 License-File: LICENSE
 Requires-Dist: Jinja2
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Provides-Extra: all
 Requires-Dist: pyvisjs[test]; extra == "all"
 
-# pyvisjs: Python Wrapper for vis.js Network
+[![pipeline status](https://gitlab.com/22kittens/pyvisjs/badges/main/pipeline.svg)](https://gitlab.com/22kittens/pyvisjs/-/commits/main)
+[![Latest Release](https://gitlab.com/22kittens/pyvisjs/-/badges/release.svg)](https://gitlab.com/22kittens/pyvisjs/-/releases)
+[![PyPI - Version](https://img.shields.io/pypi/v/pyvisjs)](https://pypi.org/project/pyvisjs)
+[![Documentation](https://img.shields.io/badge/ref-Documentation-blue)](https://22kittens.gitlab.io/pyvisjs/)
+
+
+
+# ![logo](docs/img/favicon-32x32.png) - pyvisjs
+Python wrapper for vis.js Network
+
+> :warning: **Beta version disclaimer** Please note that this package is in a **beta** version and backwards-incompatible changes might be introduced in future releases.
+
 
 pyvisjs is a Python package designed to provide seamless interaction with [vis.js](https://visjs.org) network visualizations, allowing users to manipulate and visualize network data using Python.
 
-## Workflow
+## Usage workflow
 
 1. Create a network using python
 2. Apply standard vis.js options such as colors, shapes or physics
 3. Apply pyvisjs specific options such as node/edge filtering or highlighting
 4. Show or generate html file
 5. Enjoy network interactions in your browser
 
@@ -55,15 +66,15 @@
 
 You can install PyVisjs via pip:
 
 ```bash
 pip install pyvisjs
 ```
 
-## Usage
+## Usage example
 
 ```python
 from pyvisjs import Network
 
 # Create a Network instance
 net = Network()
 
@@ -72,20 +83,20 @@
 net.add_node(2)
 net.add_edge(1, 2)
 
 # Display the network
 net.show("example.html")
 ```
 
-For more examples and detailed usage, please refer to the [documentation](link_to_docs).
+For more examples and detailed usage, please refer to the [documentation](https://22kittens.gitlab.io/pyvisjs).
 
 ## Contributing
 
 Contributions are welcome! If you have suggestions, feature requests, or find any bugs, please open an issue or submit a pull request. Make sure to follow the [contribution guidelines](CONTRIBUTING.md).
 
 ## Acknowledgments
 
 This project is inspired by the [pyvis](https://github.com/WestHealth/pyvis) Python package and the [visNetwork](https://github.com/datastorm-open/visNetwork) R-language package.
 
 ## License
 
-This project is licensed under the [MIT License](link_to_license).
+This project is licensed under the [MIT License](LICENSE).
```

### Comparing `pyvisjs-1.0.0b4/README.md` & `pyvisjs-1.0.0b5/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,23 @@
-# pyvisjs: Python Wrapper for vis.js Network
+[![pipeline status](https://gitlab.com/22kittens/pyvisjs/badges/main/pipeline.svg)](https://gitlab.com/22kittens/pyvisjs/-/commits/main)
+[![Latest Release](https://gitlab.com/22kittens/pyvisjs/-/badges/release.svg)](https://gitlab.com/22kittens/pyvisjs/-/releases)
+[![PyPI - Version](https://img.shields.io/pypi/v/pyvisjs)](https://pypi.org/project/pyvisjs)
+[![Documentation](https://img.shields.io/badge/ref-Documentation-blue)](https://22kittens.gitlab.io/pyvisjs/)
+
+
+
+# ![logo](docs/img/favicon-32x32.png) - pyvisjs
+Python wrapper for vis.js Network
+
+> :warning: **Beta version disclaimer** Please note that this package is in a **beta** version and backwards-incompatible changes might be introduced in future releases.
+
 
 pyvisjs is a Python package designed to provide seamless interaction with [vis.js](https://visjs.org) network visualizations, allowing users to manipulate and visualize network data using Python.
 
-## Workflow
+## Usage workflow
 
 1. Create a network using python
 2. Apply standard vis.js options such as colors, shapes or physics
 3. Apply pyvisjs specific options such as node/edge filtering or highlighting
 4. Show or generate html file
 5. Enjoy network interactions in your browser
 
@@ -14,15 +25,15 @@
 
 You can install PyVisjs via pip:
 
 ```bash
 pip install pyvisjs
 ```
 
-## Usage
+## Usage example
 
 ```python
 from pyvisjs import Network
 
 # Create a Network instance
 net = Network()
 
@@ -31,20 +42,20 @@
 net.add_node(2)
 net.add_edge(1, 2)
 
 # Display the network
 net.show("example.html")
 ```
 
-For more examples and detailed usage, please refer to the [documentation](link_to_docs).
+For more examples and detailed usage, please refer to the [documentation](https://22kittens.gitlab.io/pyvisjs).
 
 ## Contributing
 
 Contributions are welcome! If you have suggestions, feature requests, or find any bugs, please open an issue or submit a pull request. Make sure to follow the [contribution guidelines](CONTRIBUTING.md).
 
 ## Acknowledgments
 
 This project is inspired by the [pyvis](https://github.com/WestHealth/pyvis) Python package and the [visNetwork](https://github.com/datastorm-open/visNetwork) R-language package.
 
 ## License
 
-This project is licensed under the [MIT License](link_to_license).
+This project is licensed under the [MIT License](LICENSE).
```

### Comparing `pyvisjs-1.0.0b4/folder_structure.txt` & `pyvisjs-1.0.0b5/folder_structure.txt`

 * *Files identical despite different names*

### Comparing `pyvisjs-1.0.0b4/pyproject.toml` & `pyvisjs-1.0.0b5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyvisjs-1.0.0b4/pyvisjs/base_dictable.py` & `pyvisjs-1.0.0b5/pyvisjs/base_dictable.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,14 +8,17 @@
 
     def _update_dict_with_locals(self, _dict:Dict, _locals:Dict):
         for attr_name, attr_value in _locals.items():
             if attr_value is not None and attr_name != "self":
                 _dict.update({attr_name: attr_value})
 
     def to_dict(self):
+        """Converts object to dictionary.  
+        Used to pass network, nodes and edges to the underlying html
+        """
         result = {}
 
         def has_to_dict(attr):
             return hasattr(attr, "to_dict") and callable(getattr(attr, "to_dict"))
         
         def process_attr(attr):
             return attr.to_dict() if has_to_dict(attr) else attr
```

### Comparing `pyvisjs-1.0.0b4/pyvisjs/edge.py` & `pyvisjs-1.0.0b5/pyvisjs/edge.py`

 * *Files identical despite different names*

### Comparing `pyvisjs-1.0.0b4/pyvisjs/network.py` & `pyvisjs-1.0.0b5/pyvisjs/network.py`

 * *Files 4% similar despite different names*

```diff
@@ -142,15 +142,15 @@
             template_filename="basic.html",
             open_in_browser=open_in_browser,
             save_to_output=save_to_output,
             output_filename=output_filename)
     
 
     def render_tom_template(self, title:str=None, open_in_browser=False, save_to_output=False, output_filename="default.html", 
-    enable_highlighting=False, edge_filtering=None, node_filtering=None) -> str:
+    enable_highlighting=False, edge_filtering=None, node_filtering=None, dropdown_auto_close:bool=True) -> str:
         """This method uses jinja to inject prepared data to `'templates\\tom-select.html'` \n
         (for more info about the injected data see Notes section below).
         
         Parameters
         ----------
         open_in_browser: bool, default=False
             Resolved template will be saved as the `output_filename` and opened with `os.startfile`
@@ -180,26 +180,33 @@
             So for example you can:
             add a dynamic attribute "size" with 3 possible values ['S', 'M', 'L'] to the nodes and 
             pass `node_filtering="size"` to the `render_tom_template` method
             expecting resolved template to have `<select>` element with S/M/L options lookup
             which will filter all nodes having selected option
             see example on `gitlab.com/22kittens/pyvisjs/examples/bluor.py`
 
+        dropdown_auto_close: bool, default=True
+            Closes the autocomplete dropdown menu in the tom-select control after item selection, if `True`  
+            Drop down menu stays open after item selection, if `False`
+            This flag translates into the `tom_select.close()` call at the end of the `onChange` event (see `templates/init_tomSelect.js`)
+
         Notes
         -----
         The data injected will be:
 
         >>> .render(
         >>>     width=network_dict["options"].get("width", "100%"),
         >>>     height=network_dict["options"].get("height", "100%"),
         >>>     data=network_dict,
         >>>     pyvisjs={
         >>>         "enable_highlighting": enable_highlighting,
         >>>         "edge_filtering_lookup": edge_filtering_lookup,
         >>>         "node_filtering_lookup": node_filtering_lookup,
+        >>>         "title": title,
+        >>>         "dropdown_auto_close": dropdown_auto_close,
         >>>     },
         >>> )
 
         you can find more details about `edge_filtering_lookup` and `node_filtering_lookup` structure here `tests\\test_network.py\\test_network_render_template_edge_filtering_list`
         """
 
         edge_filtering_lookup: Dict = None
@@ -229,14 +236,15 @@
                 node_filtering_lookup[field_name] = unique_values             
         
         pyvisjs_options = {
                     "enable_highlighting": enable_highlighting,
                     "edge_filtering_lookup": edge_filtering_lookup,
                     "node_filtering_lookup": node_filtering_lookup,
                     "title": title,
+                    "dropdown_auto_close": dropdown_auto_close,
                 };
          
         return self._render(
             template_filename="tom-select.html",
             open_in_browser=open_in_browser,
             save_to_output=save_to_output,
             output_filename=output_filename,
```

### Comparing `pyvisjs-1.0.0b4/pyvisjs/node.py` & `pyvisjs-1.0.0b5/pyvisjs/node.py`

 * *Files identical despite different names*

### Comparing `pyvisjs-1.0.0b4/pyvisjs/options.py` & `pyvisjs-1.0.0b5/pyvisjs/options.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,21 +3,23 @@
 
 # Options
 # ├─── set_configure
 # ├─── set_interaction
 # ├── Nodes
 # │   └── set_scaling
 # ├── Edges
+# │   ├── set
 # │   ├── set_color
 # │   └── set_smooth
-# ├── Physics
-# │   ├── set_barnesHutKV
-# │   ├── set_barnesHut
-# │   └── set_stabilization
-# └── 
+# └── Physics
+#     ├── set
+#     ├── set_barnesHutKV
+#     ├── set_barnesHut
+#     └── set_stabilization
+
 
 
 class Options(BaseDictable):
     """
     Parameters
     ----------
     height : str, default='100%'
@@ -48,15 +50,15 @@
         enabled : bool, default=true
             Toggle the configuration interface on or off. This is an optional parameter. If left undefined and any of the other properties of this object are defined, this will be set to true.
             So you can switch it on if you just want to use defaults for all other options
         """
         self._update_dict_with_locals(self.configure, locals())
         return self
 
-    def set_interaction(self, dragNodes:bool=None, dragView:bool=None, hideEdgesOnDrag:bool=None, hideEdgesOnZoom:bool=None, hideNodesOnDrag:bool=None) -> Self:
+    def set_interaction(self, dragNodes:bool=None, dragView:bool=None, hideEdgesOnDrag:bool=None, hideEdgesOnZoom:bool=None, hideNodesOnDrag:bool=None, zoomView:bool=None) -> Self:
         """
         Used for all user interaction with the network. Handles mouse and touch events as well as the navigation buttons and the popups.
        
         Parameters
         ----------
         dragNodes : bool, default=True
             When true, the nodes that are not fixed can be dragged by the user.
@@ -68,14 +70,17 @@
             When true, the edges are not drawn when dragging the view. This can greatly speed up responsiveness on dragging, improving user experience.
 
         hideEdgesOnZoom : bool, default=False
             When true, the edges are not drawn when zooming the view. This can greatly speed up responsiveness on zooming, improving user experience.
 
         hideNodesOnDrag : bool, default=False
             When true, the nodes are not drawn when dragging the view. This can greatly speed up responsiveness on dragging, improving user experience.
+
+        zoomView : bool, default=True
+            When true, the user can zoom in.
             
         """
         self._update_dict_with_locals(self.interaction, locals())
         return self
 
     class Nodes(BaseDictable):
         def __init__(self):
@@ -87,21 +92,21 @@
             self._update_dict_with_locals(self.font, locals())
             return self
 
         def set_scaling(self, min:int=None, max:int=None, label:bool=None) -> Self:
             """
             Parameters
             ----------
-            min : int, default=10
+            min: int, default=10
                 If nodes have a value, their sizes are determined by the value, the scaling function and the min max values. The min value is the minimum allowed value.
             
-            max : int, default=30
+            max: int, default=30
                 This is the maximum allowed size when the nodes are scaled using the value option.
 
-            label : bool, default true
+            label: bool, default true
                 This can be false if the label is not allowed to scale with the node. If true it will scale using default settings
             """
             self._update_dict_with_locals(self.scaling, locals())
             return self
         
     class Edges(BaseDictable):
         def __init__(self):
@@ -118,53 +123,53 @@
             self._update_dict_with_locals(self.font, locals())
             return self
 
         def set(self, arrows:str=None, arrowStrikethrough:bool=None) -> Self:
             """
             Parameters
             ----------
-            arrows : str, default None
+            arrows: str, default None
                 Can be any combination with any separating symbol of `'to, from, middle'`
 
-            arrowStrikethrough : bool, default=True
+            arrowStrikethrough: bool, default=True
                 When false, the edge stops at the arrow. This can be useful if you have thick lines and you want the arrow to end in a point. Middle arrows are not affected by this.
 
             """
             if arrows: self.arrows = arrows
             if arrowStrikethrough is not None: self.arrowStrikethrough = arrowStrikethrough
 
             return self
         
         def set_color(self, color:str=None, highlight:str=None, hover:str=None, inherit:str=None, opacity:float=None, dashes:bool=None) -> Self:
             """
             Parameters
             ----------
-            color : str, default='#848484'
+            color: str, default='#848484'
                 The color of the edge when it is not selected or hovered over (assuming hover is enabled in the interaction module).
 
-            highlight : str, default='#848484'
+            highlight: str, default='#848484'
                 The color the edge when it is selected.
 
-            hover : str, default='#848484'
+            hover: str, default='#848484'
                 The color the edge when the mouse hovers over it (assuming hover is enabled in the interaction module).
 
-            inherit : str, default='from'
+            inherit: str, default='from'
                 When color, highlight or hover are defined, inherit is set to false!
 
                 Supported options are: `'from','to','both'`.
                 The default value is 'from' which does the same as true: the edge will inherit the color from the border of the node on the 'from' side.
 
                 When set to 'to', the border color from the 'to' node will be used.
 
                 When set to 'both', the color will fade from the from color to the to color. `'both' is computationally intensive` because the gradient is recomputed every redraw. This is required because the angles change when the nodes move.
             
-            opacity : float, default=1.0
+            opacity: float, default=1.0
                 It can be useful to set the opacity of an edge without manually changing all the colors. The opacity option will convert all colors (also when using inherit) to adhere to the supplied opacity. The allowed range of the opacity option is between 0 and 1. This is only done once so the performance impact is not too big.
             
-            dashes : bool, default=False
+            dashes: bool, default=False
                 When true, the edge will be drawn as a dashed line. When using dashed lines in IE versions older than 11, the line will be drawn straight, not smooth.
             """
             self._update_dict_with_locals(self.color, locals())
             return self
 
         def set_smooth(self, enabled:bool=None, type:str=None, roundness:float=None) -> Self:
             """
```

### Comparing `pyvisjs-1.0.0b4/pyvisjs/templates/base.html` & `pyvisjs-1.0.0b5/pyvisjs/templates/base.html`

 * *Files identical despite different names*

### Comparing `pyvisjs-1.0.0b4/pyvisjs/templates/bs-container.html` & `pyvisjs-1.0.0b5/pyvisjs/templates/bs-container.html`

 * *Files identical despite different names*

### Comparing `pyvisjs-1.0.0b4/pyvisjs/templates/create_network.js` & `pyvisjs-1.0.0b5/pyvisjs/templates/create_network.js`

 * *Files identical despite different names*

### Comparing `pyvisjs-1.0.0b4/pyvisjs/templates/draw_title.js` & `pyvisjs-1.0.0b5/pyvisjs/templates/draw_title.js`

 * *Files identical despite different names*

### Comparing `pyvisjs-1.0.0b4/pyvisjs/templates/functions.js` & `pyvisjs-1.0.0b5/pyvisjs/templates/functions.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -30,25 +30,41 @@
             if (result.includes(edge.to) === false) result.push(edge.to);
         }
     }
 
     return result;
 }
 
-function find_node_by_attribute_value(field, value) {
+function find_heighbors_by_node_id(id) {
+    for (const key in data.nodes) {
+        const node = data.nodes[key];
+
+        if (node["id"] === id) {
+            const selected_node = node["id"];
+            collected_nodes = data.network.getConnectedNodes(selected_node);
+            collected_nodes.push(selected_node);
+            return collected_nodes
+        }
+    }
+
+    return null;
+}
+
+function get_nodes_by_attribute_value(field, value) {
+    const collected_nodes = [];
 
     for (const key in data.nodes) {
         const node = data.nodes[key];
 
         if (node[field] === value) {
-            return node["id"];
+            collected_nodes.push(node["id"]);
         }
     }
 
-    return null;
+    return collected_nodes;
 }
 
 function hide_nodes_by_edge_attribute_values_intersect(option_groups_dict) {
 
     const selected_nodes_by_field = {}
 
     for (field in option_groups_dict) {
@@ -64,17 +80,15 @@
             if (node_or_edge === "ALL" && value === "ALL") {
                 collected_nodes = Object.keys(data.nodes);
                 data.network.has_hidden_nodes = false;
             } else if (node_or_edge === "edge") {
                 collected_nodes = get_nodes_by_edge_attribute_value(field, value)
                 data.network.has_hidden_nodes = true;
             } else if (node_or_edge === "node") {
-                const selected_node = find_node_by_attribute_value(field, value);
-                collected_nodes = data.network.getConnectedNodes(selected_node);
-                collected_nodes.push(selected_node);
+                collected_nodes = get_nodes_by_attribute_value(field, value);
                 data.network.has_hidden_nodes = true;
             }
 
             for (id in collected_nodes) {
                 node_id = collected_nodes[id]
                 if (selected_nodes_by_field[field].includes(node_id) === false) selected_nodes_by_field[field].push(node_id)
             }
@@ -141,17 +155,15 @@
             if (node_or_edge === "ALL" && value === "ALL") {
                 collected_nodes = Object.keys(data.nodes);
                 data.network.has_hidden_nodes = false;
             } else if (node_or_edge === "edge") {
                 collected_nodes = get_nodes_by_edge_attribute_value(field, value)
                 data.network.has_hidden_nodes = true;
             } else if (node_or_edge === "node") {
-                const selected_node = find_node_by_attribute_value(field, value);
-                collected_nodes = data.network.getConnectedNodes(selected_node);
-                collected_nodes.push(selected_node);
+                collected_nodes = get_nodes_by_attribute_value(field, value);
                 data.network.has_hidden_nodes = true;
             }
 
             for (id in collected_nodes) {
                 node_value = collected_nodes[id]
                 if (selectedNodes.includes(node_value) === false) selectedNodes.push(node_value)
             }
```

### Comparing `pyvisjs-1.0.0b4/pyvisjs/templates/init_tomSelect.js` & `pyvisjs-1.0.0b5/pyvisjs/templates/init_tomSelect.js`

 * *Files 20% similar despite different names*

#### js-beautify {}

```diff
@@ -1,16 +1,18 @@
 const eventHandler = function(name) {
     return function() {
         const list_of_selected_values = arguments[0]
         dict = convert_field_value_list_to_dict(list_of_selected_values)
         hide_nodes_by_edge_attribute_values_intersect(dict)
+
+        if (data.pyvisjs.dropdown_auto_close === true) tom_select.close();
     };
 };
 
-new TomSelect("#select-all-fields", {
+tom_select = new TomSelect("#select-all-fields", {
     maxItems: 10,
     onChange: eventHandler("onChange"),
     //create: true,
     //onItemAdd:function(){
     //    this.setTextboxValue('');
     //    this.refreshOptions();
     //},
```

### Comparing `pyvisjs-1.0.0b4/pyvisjs/templates/select-edge-filter.html` & `pyvisjs-1.0.0b5/pyvisjs/templates/select-edge-filter.html`

 * *Files identical despite different names*

### Comparing `pyvisjs-1.0.0b4/pyvisjs/templates/tom-select.html` & `pyvisjs-1.0.0b5/pyvisjs/templates/tom-select.html`

 * *Files identical despite different names*

### Comparing `pyvisjs-1.0.0b4/pyvisjs/utils.py` & `pyvisjs-1.0.0b5/pyvisjs/utils.py`

 * *Files identical despite different names*

### Comparing `pyvisjs-1.0.0b4/pyvisjs.egg-info/PKG-INFO` & `pyvisjs-1.0.0b5/pyvisjs.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvisjs
-Version: 1.0.0b4
+Version: 1.0.0b5
 Summary: A Python wrapper for vis.js Network
 Author-email: Andrey Morozov <andrey@morozov.lv>
 License: MIT License
         
         Copyright (c) 2024 Andrey Morozov (andrey@morozov.lv)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -35,19 +35,30 @@
 License-File: LICENSE
 Requires-Dist: Jinja2
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Provides-Extra: all
 Requires-Dist: pyvisjs[test]; extra == "all"
 
-# pyvisjs: Python Wrapper for vis.js Network
+[![pipeline status](https://gitlab.com/22kittens/pyvisjs/badges/main/pipeline.svg)](https://gitlab.com/22kittens/pyvisjs/-/commits/main)
+[![Latest Release](https://gitlab.com/22kittens/pyvisjs/-/badges/release.svg)](https://gitlab.com/22kittens/pyvisjs/-/releases)
+[![PyPI - Version](https://img.shields.io/pypi/v/pyvisjs)](https://pypi.org/project/pyvisjs)
+[![Documentation](https://img.shields.io/badge/ref-Documentation-blue)](https://22kittens.gitlab.io/pyvisjs/)
+
+
+
+# ![logo](docs/img/favicon-32x32.png) - pyvisjs
+Python wrapper for vis.js Network
+
+> :warning: **Beta version disclaimer** Please note that this package is in a **beta** version and backwards-incompatible changes might be introduced in future releases.
+
 
 pyvisjs is a Python package designed to provide seamless interaction with [vis.js](https://visjs.org) network visualizations, allowing users to manipulate and visualize network data using Python.
 
-## Workflow
+## Usage workflow
 
 1. Create a network using python
 2. Apply standard vis.js options such as colors, shapes or physics
 3. Apply pyvisjs specific options such as node/edge filtering or highlighting
 4. Show or generate html file
 5. Enjoy network interactions in your browser
 
@@ -55,15 +66,15 @@
 
 You can install PyVisjs via pip:
 
 ```bash
 pip install pyvisjs
 ```
 
-## Usage
+## Usage example
 
 ```python
 from pyvisjs import Network
 
 # Create a Network instance
 net = Network()
 
@@ -72,20 +83,20 @@
 net.add_node(2)
 net.add_edge(1, 2)
 
 # Display the network
 net.show("example.html")
 ```
 
-For more examples and detailed usage, please refer to the [documentation](link_to_docs).
+For more examples and detailed usage, please refer to the [documentation](https://22kittens.gitlab.io/pyvisjs).
 
 ## Contributing
 
 Contributions are welcome! If you have suggestions, feature requests, or find any bugs, please open an issue or submit a pull request. Make sure to follow the [contribution guidelines](CONTRIBUTING.md).
 
 ## Acknowledgments
 
 This project is inspired by the [pyvis](https://github.com/WestHealth/pyvis) Python package and the [visNetwork](https://github.com/datastorm-open/visNetwork) R-language package.
 
 ## License
 
-This project is licensed under the [MIT License](link_to_license).
+This project is licensed under the [MIT License](LICENSE).
```

### Comparing `pyvisjs-1.0.0b4/pyvisjs.egg-info/SOURCES.txt` & `pyvisjs-1.0.0b5/pyvisjs.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,30 @@
 .gitignore
 .gitlab-ci.yml
 CONTRIBUTING.md
 LICENSE
 README.md
 folder_structure.txt
+mkdocs.yml
 pyproject.toml
+requirements-doc.txt
 requirements.txt
-examples/bluor.py
-examples/readme.py
+docs/basic-example.md
+docs/edges.md
+docs/index.md
+docs/installation.md
+docs/network.md
+docs/nodes.md
+docs/options.md
+docs/img/favicon-32x32.png
+docs/img/favicon.ico
+docs_overrides/dandelion.html
+docs_overrides/index.html
+examples/basic-example.py
+examples/repo.py
 pyvisjs/__init__.py
 pyvisjs/_version.py
 pyvisjs/base_dictable.py
 pyvisjs/edge.py
 pyvisjs/network.py
 pyvisjs/node.py
 pyvisjs/options.py
```

### Comparing `pyvisjs-1.0.0b4/tests/test_base_dictable.py` & `pyvisjs-1.0.0b5/tests/test_base_dictable.py`

 * *Files identical despite different names*

### Comparing `pyvisjs-1.0.0b4/tests/test_edge.py` & `pyvisjs-1.0.0b5/tests/test_edge.py`

 * *Files identical despite different names*

### Comparing `pyvisjs-1.0.0b4/tests/test_network.py` & `pyvisjs-1.0.0b5/tests/test_network.py`

 * *Files 4% similar despite different names*

```diff
@@ -164,14 +164,15 @@
     HEIGHT="100%"
     DATA={"nodes": [], "edges": [], "options": {}}
     PYVISJS={
         "enable_highlighting": False,
         "edge_filtering_lookup": None,
         "node_filtering_lookup": None,
         "title": None,
+        "dropdown_auto_close": True,
     }
     
     # mock
     mock_render = mock_Environment.return_value.get_template.return_value.render
 
     # call
     network = Network("Test Network")
@@ -186,31 +187,34 @@
     WIDTH="100%"
     HEIGHT="100%"
     DATA={"nodes": [], "edges": [], "options": {}}
     TEMPLATE_FILENAME="tom-select.html"
     ENABLE_HIGHLIGHTING=True
     EDGE_FILTERING="edge_field" # str(!) not list
     NODE_FILTERING=["field1", "field2"] # list
+    DROPDOWN_AUTO_CLOSE=False,
     PYVISJS={
         "enable_highlighting": ENABLE_HIGHLIGHTING,
         "edge_filtering_lookup": {"edge_field": []},
         "node_filtering_lookup": {"field1": [], "field2": []},
         "title": None,
+        "dropdown_auto_close": DROPDOWN_AUTO_CLOSE,
     }
     
     # mock
     mock_get_template = mock_Environment.return_value.get_template
     mock_render = mock_get_template.return_value.render
 
     # call
     network = Network("Test Network")
     html_output = network.render_tom_template( # <--------------------
         enable_highlighting=ENABLE_HIGHLIGHTING, 
         edge_filtering=EDGE_FILTERING, 
-        node_filtering=NODE_FILTERING)
+        node_filtering=NODE_FILTERING,
+        dropdown_auto_close=DROPDOWN_AUTO_CLOSE)
 
     # assert
     mock_get_template.assert_called_once_with(TEMPLATE_FILENAME)
     mock_render.assert_called_once_with(width=WIDTH, height=HEIGHT, data=DATA, pyvisjs=PYVISJS)
 
 @patch('pyvisjs.network.Environment')
 def test_network_render_tom_template_edge_filtering_list(mock_Environment):
@@ -233,14 +237,15 @@
     EDGE_FILTERING=["field1", "field2"]
     NODE_FILTERING=["label", "shape"]
     PYVISJS={
         "enable_highlighting": ENABLE_HIGHLIGHTING,
         "edge_filtering_lookup": {"field1": ["AM", "JL"], "field2": []},
         "node_filtering_lookup": {"label": ["1", "2", "3"], "shape": ["dot"]},
         "title": None,
+        "dropdown_auto_close": True,
     }
     
     # mock
     mock_get_template = mock_Environment.return_value.get_template
     mock_render = mock_get_template.return_value.render
 
     # call
@@ -268,14 +273,15 @@
     EDGE_FILTERING=34
     NODE_FILTERING=22
     PYVISJS={
         "enable_highlighting": ENABLE_HIGHLIGHTING,
         "edge_filtering_lookup": {"34": []},
         "node_filtering_lookup": {"22": []},
         "title": None,
+        "dropdown_auto_close": True,
     }
     
     # mock
     mock_get_template = mock_Environment.return_value.get_template
     mock_render = mock_get_template.return_value.render
 
     # call
```

### Comparing `pyvisjs-1.0.0b4/tests/test_node.py` & `pyvisjs-1.0.0b5/tests/test_node.py`

 * *Files identical despite different names*

### Comparing `pyvisjs-1.0.0b4/tests/test_options.py` & `pyvisjs-1.0.0b5/tests/test_options.py`

 * *Files identical despite different names*

### Comparing `pyvisjs-1.0.0b4/tests/test_utils.py` & `pyvisjs-1.0.0b5/tests/test_utils.py`

 * *Files identical despite different names*

