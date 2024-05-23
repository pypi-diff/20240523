# Comparing `tmp/pytestomatio-2.5.0.tar.gz` & `tmp/pytestomatio-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytestomatio-2.5.0.tar", last modified: Wed May  8 15:53:08 2024, max compression
+gzip compressed data, was "pytestomatio-2.5.2.tar", last modified: Thu May 23 09:36:17 2024, max compression
```

## Comparing `pytestomatio-2.5.0.tar` & `pytestomatio-2.5.2.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:53:08.677726 pytestomatio-2.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-08 15:53:04.000000 pytestomatio-2.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7583 2024-05-08 15:53:08.677726 pytestomatio-2.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6767 2024-05-08 15:53:04.000000 pytestomatio-2.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-08 15:53:04.000000 pytestomatio-2.5.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:53:08.669726 pytestomatio-2.5.0/pytestomatio/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 15:53:04.000000 pytestomatio-2.5.0/pytestomatio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:53:08.673726 pytestomatio-2.5.0/pytestomatio/connect/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 15:53:04.000000 pytestomatio-2.5.0/pytestomatio/connect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7189 2024-05-08 15:53:04.000000 pytestomatio-2.5.0/pytestomatio/connect/connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-05-08 15:53:04.000000 pytestomatio-2.5.0/pytestomatio/connect/s3_connector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:53:08.673726 pytestomatio-2.5.0/pytestomatio/decor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 15:53:04.000000 pytestomatio-2.5.0/pytestomatio/decor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-08 15:53:04.000000 pytestomatio-2.5.0/pytestomatio/decor/decorator_updater.py
--rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-05-08 15:53:04.000000 pytestomatio-2.5.0/pytestomatio/decor/default.py
--rw-r--r--   0 runner    (1001) docker     (127)     3069 2024-05-08 15:53:04.000000 pytestomatio-2.5.0/pytestomatio/decor/pep8.py
--rw-r--r--   0 runner    (1001) docker     (127)     8330 2024-05-08 15:53:04.000000 pytestomatio-2.5.0/pytestomatio/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:53:08.673726 pytestomatio-2.5.0/pytestomatio/testing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 15:53:04.000000 pytestomatio-2.5.0/pytestomatio/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-08 15:53:04.000000 pytestomatio-2.5.0/pytestomatio/testing/code_collector.py
--rw-r--r--   0 runner    (1001) docker     (127)     5686 2024-05-08 15:53:04.000000 pytestomatio-2.5.0/pytestomatio/testing/testItem.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:53:08.673726 pytestomatio-2.5.0/pytestomatio/testomatio/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 15:53:04.000000 pytestomatio-2.5.0/pytestomatio/testomatio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-05-08 15:53:04.000000 pytestomatio-2.5.0/pytestomatio/testomatio/testRunConfig.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-08 15:53:04.000000 pytestomatio-2.5.0/pytestomatio/testomatio/testomat_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-05-08 15:53:04.000000 pytestomatio-2.5.0/pytestomatio/testomatio/testomatio.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:53:08.677726 pytestomatio-2.5.0/pytestomatio/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 15:53:04.000000 pytestomatio-2.5.0/pytestomatio/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4214 2024-05-08 15:53:04.000000 pytestomatio-2.5.0/pytestomatio/utils/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     3723 2024-05-08 15:53:04.000000 pytestomatio-2.5.0/pytestomatio/utils/parser_setup.py
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-08 15:53:04.000000 pytestomatio-2.5.0/pytestomatio/utils/validations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-05-08 15:53:04.000000 pytestomatio-2.5.0/pytestomatio/utils/worker_sync.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:53:08.677726 pytestomatio-2.5.0/pytestomatio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7583 2024-05-08 15:53:08.000000 pytestomatio-2.5.0/pytestomatio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-05-08 15:53:08.000000 pytestomatio-2.5.0/pytestomatio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 15:53:08.000000 pytestomatio-2.5.0/pytestomatio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-08 15:53:08.000000 pytestomatio-2.5.0/pytestomatio.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-08 15:53:08.000000 pytestomatio-2.5.0/pytestomatio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-08 15:53:08.000000 pytestomatio-2.5.0/pytestomatio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 15:53:08.677726 pytestomatio-2.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:53:08.677726 pytestomatio-2.5.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:53:08.677726 pytestomatio-2.5.0/tests/sub/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 15:53:04.000000 pytestomatio-2.5.0/tests/sub/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 15:53:08.677726 pytestomatio-2.5.0/tests/sub/sub_mob/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 15:53:04.000000 pytestomatio-2.5.0/tests/sub/sub_mob/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-08 15:53:04.000000 pytestomatio-2.5.0/tests/sub/sub_mob/sub_sub_class_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-08 15:53:04.000000 pytestomatio-2.5.0/tests/sub/sub_mob/sub_sub_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-08 15:53:04.000000 pytestomatio-2.5.0/tests/sub/test_class_sub.py
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-08 15:53:04.000000 pytestomatio-2.5.0/tests/sub/test_sub.py
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-08 15:53:04.000000 pytestomatio-2.5.0/tests/test_class_root.py
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-08 15:53:04.000000 pytestomatio-2.5.0/tests/test_decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-08 15:53:04.000000 pytestomatio-2.5.0/tests/test_root.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:36:17.874109 pytestomatio-2.5.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-23 09:36:11.000000 pytestomatio-2.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7583 2024-05-23 09:36:17.874109 pytestomatio-2.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6767 2024-05-23 09:36:11.000000 pytestomatio-2.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-23 09:36:11.000000 pytestomatio-2.5.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:36:17.870109 pytestomatio-2.5.2/pytestomatio/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 09:36:11.000000 pytestomatio-2.5.2/pytestomatio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:36:17.870109 pytestomatio-2.5.2/pytestomatio/connect/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 09:36:11.000000 pytestomatio-2.5.2/pytestomatio/connect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7189 2024-05-23 09:36:11.000000 pytestomatio-2.5.2/pytestomatio/connect/connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-05-23 09:36:11.000000 pytestomatio-2.5.2/pytestomatio/connect/s3_connector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:36:17.870109 pytestomatio-2.5.2/pytestomatio/decor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 09:36:11.000000 pytestomatio-2.5.2/pytestomatio/decor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-23 09:36:11.000000 pytestomatio-2.5.2/pytestomatio/decor/decorator_updater.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-05-23 09:36:11.000000 pytestomatio-2.5.2/pytestomatio/decor/default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3069 2024-05-23 09:36:11.000000 pytestomatio-2.5.2/pytestomatio/decor/pep8.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8030 2024-05-23 09:36:11.000000 pytestomatio-2.5.2/pytestomatio/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:36:17.870109 pytestomatio-2.5.2/pytestomatio/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 09:36:11.000000 pytestomatio-2.5.2/pytestomatio/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-23 09:36:11.000000 pytestomatio-2.5.2/pytestomatio/testing/code_collector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5686 2024-05-23 09:36:11.000000 pytestomatio-2.5.2/pytestomatio/testing/testItem.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:36:17.870109 pytestomatio-2.5.2/pytestomatio/testomatio/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 09:36:11.000000 pytestomatio-2.5.2/pytestomatio/testomatio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-05-23 09:36:11.000000 pytestomatio-2.5.2/pytestomatio/testomatio/testRunConfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-23 09:36:11.000000 pytestomatio-2.5.2/pytestomatio/testomatio/testomat_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-05-23 09:36:11.000000 pytestomatio-2.5.2/pytestomatio/testomatio/testomatio.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:36:17.874109 pytestomatio-2.5.2/pytestomatio/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 09:36:11.000000 pytestomatio-2.5.2/pytestomatio/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4214 2024-05-23 09:36:11.000000 pytestomatio-2.5.2/pytestomatio/utils/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3805 2024-05-23 09:36:11.000000 pytestomatio-2.5.2/pytestomatio/utils/parser_setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-05-23 09:36:11.000000 pytestomatio-2.5.2/pytestomatio/utils/validations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-05-23 09:36:11.000000 pytestomatio-2.5.2/pytestomatio/utils/worker_sync.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:36:17.874109 pytestomatio-2.5.2/pytestomatio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7583 2024-05-23 09:36:17.000000 pytestomatio-2.5.2/pytestomatio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-05-23 09:36:17.000000 pytestomatio-2.5.2/pytestomatio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 09:36:17.000000 pytestomatio-2.5.2/pytestomatio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-23 09:36:17.000000 pytestomatio-2.5.2/pytestomatio.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-23 09:36:17.000000 pytestomatio-2.5.2/pytestomatio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-23 09:36:17.000000 pytestomatio-2.5.2/pytestomatio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 09:36:17.874109 pytestomatio-2.5.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:36:17.874109 pytestomatio-2.5.2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:36:17.874109 pytestomatio-2.5.2/tests/sub/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 09:36:11.000000 pytestomatio-2.5.2/tests/sub/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 09:36:17.874109 pytestomatio-2.5.2/tests/sub/sub_mob/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 09:36:11.000000 pytestomatio-2.5.2/tests/sub/sub_mob/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-23 09:36:11.000000 pytestomatio-2.5.2/tests/sub/sub_mob/sub_sub_class_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-23 09:36:11.000000 pytestomatio-2.5.2/tests/sub/sub_mob/sub_sub_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-23 09:36:11.000000 pytestomatio-2.5.2/tests/sub/test_class_sub.py
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-05-23 09:36:11.000000 pytestomatio-2.5.2/tests/sub/test_sub.py
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-23 09:36:11.000000 pytestomatio-2.5.2/tests/test_class_root.py
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-23 09:36:11.000000 pytestomatio-2.5.2/tests/test_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-05-23 09:36:11.000000 pytestomatio-2.5.2/tests/test_root.py
```

### Comparing `pytestomatio-2.5.0/LICENSE` & `pytestomatio-2.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.5.0/PKG-INFO` & `pytestomatio-2.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytestomatio
-Version: 2.5.0
+Version: 2.5.2
 Summary: Pytest plugin to sync test with testomat.io
 Author: Oleksii Ostapov, TikoQA
 Project-URL: Testomat.io, https://testomat.io/
 Project-URL: Homepage, https://github.com/testomatio/pytestomatio
 Project-URL: Bug Tracker, https://github.com/testomatio/pytestomatio/issues
 Classifier: Framework :: Pytest
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pytestomatio-2.5.0/README.md` & `pytestomatio-2.5.2/README.md`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.5.0/pyproject.toml` & `pytestomatio-2.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 name = "cz_conventional_commits"
 tag_format = "$version"
 version_scheme = "pep440"
 version_provider = "pep621"
 update_changelog_on_bump = true
 [project]
 name = "pytestomatio"
-version = "2.5.0"
+version = "2.5.2"
 
 dependencies = [
     "requests>=2.29.0",
     "pytest>7.2.0",
     "boto3>=1.28.28",
     "libcst==1.1.0",
     "commitizen>=3.18.1",
```

### Comparing `pytestomatio-2.5.0/pytestomatio/connect/connector.py` & `pytestomatio-2.5.2/pytestomatio/connect/connector.py`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.5.0/pytestomatio/connect/s3_connector.py` & `pytestomatio-2.5.2/pytestomatio/connect/s3_connector.py`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.5.0/pytestomatio/decor/decorator_updater.py` & `pytestomatio-2.5.2/pytestomatio/decor/decorator_updater.py`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.5.0/pytestomatio/decor/default.py` & `pytestomatio-2.5.2/pytestomatio/decor/default.py`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.5.0/pytestomatio/decor/pep8.py` & `pytestomatio-2.5.2/pytestomatio/decor/pep8.py`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.5.0/pytestomatio/main.py` & `pytestomatio-2.5.2/pytestomatio/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,50 +1,34 @@
 import os, pytest, logging, json
 
-from pytest import Parser, Session, Config, Item, CallInfo, fixture, FixtureRequest
+from pytest import Parser, Session, Config, Item, CallInfo, hookimpl
 from pytestomatio.connect.connector import Connector
 from pytestomatio.decor.decorator_updater import update_tests
 from pytestomatio.testomatio.testRunConfig import TestRunConfig
 from pytestomatio.testing.testItem import TestItem
 from pytestomatio.connect.s3_connector import S3Connector
 from .testomatio.testomatio import Testomatio
 from pytestomatio.utils.helper import add_and_enrich_tests, get_test_mapping, collect_tests
 from pytestomatio.utils.parser_setup import parser_options
 from pytestomatio.utils import helper
 from pytestomatio.utils import validations
-import multiprocessing
+from xdist.plugin import is_xdist_controller, get_xdist_worker_id
 
 log = logging.getLogger(__name__)
 log.setLevel('INFO')
 
 metadata_file = 'metadata.json'
 decorator_name = 'testomatio'
 testomatio = 'testomatio'
 
 
-@fixture(autouse=True)
-def testomatio_skip_test_fixture(request: FixtureRequest):
-    if request.config.getoption(testomatio) and request.config.getoption(testomatio).lower() in ['sync', 'remove',
-                                                                                                 'debug']:
-        pytest.skip("Skipping this test because of some condition")
-
-
 def pytest_addoption(parser: Parser) -> None:
     parser_options(parser, testomatio)
 
 
-#
-# def pytest_xdist_setupnodes(config, specs):
-#     pass
-#
-#
-# def pytest_xdist_node_collection_finished(node, ids):
-#     pass
-
-
 def pytest_configure(config: Config):
     #  FYI hook runs before the xdist and later again within every worker
     validations.validate_env_variables()
     validations.validate_command_line_args(config)
 
     config.addinivalue_line(
         "markers", "testomatio(arg): built in marker to connect test case with testomat.io by unique id"
@@ -81,18 +65,20 @@
                     no_detach=config.getoption('no_detach'),
                     structure=config.getoption('keep_structure'),
                     create=config.getoption('create'),
                     directory=config.getoption('directory')
                 )
                 testomatio_tests = pytest.testomatio.connector.get_tests(meta)
                 add_and_enrich_tests(meta, test_files, test_names, testomatio_tests, decorator_name)
+                pytest.exit('Sync completed without test execution')
             case 'remove':
                 mapping = get_test_mapping(meta)
                 for test_file in test_files:
                     update_tests(test_file, mapping, test_names, decorator_name, remove=True)
+                pytest.exit('Sync completed without test execution')
             case 'report':
                 # assuming run already created in pytest_configure hook
                 run: TestRunConfig = pytest.testomatio.test_run_config
                 run.test_run_id = run.lock.get_run_id()
                 # lock file here as it runs in the worker
                 run.lock.lock()
                 run_details = pytest.testomatio.connector.update_test_run(**run.to_dict())
@@ -110,14 +96,15 @@
                         pytest.testomatio.s3_connector.login()
                     else:
                         pytest.testomatio.s3_connector = S3Connector()
             case 'debug':
                 with open(metadata_file, 'w') as file:
                     data = json.dumps([i.to_dict() for i in meta], indent=4)
                     file.write(data)
+                    pytest.exit('Debug file created. Exiting...')
             case _:
                 pytest.exit('Unknown pytestomatio parameter. Use one of: add, remove, sync, debug')
 
 
 def pytest_runtest_makereport(item: Item, call: CallInfo):
     pytest.testomatio_config_option = item.config.getoption(testomatio)
     if pytest.testomatio_config_option is None or pytest.testomatio_config_option != 'report':
@@ -185,22 +172,21 @@
     for nodeid, request in pytest.testomatio.test_run_config.status_request.items():
         if request['status']:
             pytest.testomatio.connector.update_test_status(run_id=pytest.testomatio.test_run_config.test_run_id,
                                                            **request)
     pytest.testomatio.test_run_config.status_request = {}
 
 
-def pytest_sessionfinish(session: Session, exitstatus: int):
+@hookimpl(tryfirst=True)
+def pytest_testnodedown(node, error):
     run = pytest.testomatio.test_run_config
     if run.test_run_id:
         run.lock.unlock()
-        is_last = run.lock.clear_run_id()
-        pytest.testomatio.connector.finish_test_run(run.test_run_id, True)
+        pytest.testomatio.connector.finish_test_run(run.test_run_id)
 
 
-# @pytest.fixture(scope='session')
-# def final_worker_standing():
-#     yield
-#     run = pytest.testomatio.test_run_config
-#     if run.test_run_id:
-#         is_last = run.lock.clear_run_id()
-#         pytest.testomatio.connector.finish_test_run(run.test_run_id, is_last)
+@hookimpl(trylast=True)
+def pytest_sessionfinish(session: Session, exitstatus: int):
+    run = pytest.testomatio.test_run_config
+    if run.test_run_id and is_xdist_controller(session):
+        run.lock.clear_run_id()
+        pytest.testomatio.connector.finish_test_run(run.test_run_id, True)
```

### Comparing `pytestomatio-2.5.0/pytestomatio/testing/code_collector.py` & `pytestomatio-2.5.2/pytestomatio/testing/code_collector.py`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.5.0/pytestomatio/testing/testItem.py` & `pytestomatio-2.5.2/pytestomatio/testing/testItem.py`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.5.0/pytestomatio/testomatio/testRunConfig.py` & `pytestomatio-2.5.2/pytestomatio/testomatio/testRunConfig.py`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.5.0/pytestomatio/testomatio/testomatio.py` & `pytestomatio-2.5.2/pytestomatio/testomatio/testomatio.py`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.5.0/pytestomatio/utils/helper.py` & `pytestomatio-2.5.2/pytestomatio/utils/helper.py`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.5.0/pytestomatio/utils/parser_setup.py` & `pytestomatio-2.5.2/pytestomatio/utils/parser_setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,61 +6,62 @@
             remove - removes testomat.io ids from the ALL test
             report - report tests into testomat.io
             debug - saves analysed test metadata to the json in the test project root
             """
 
 
 def parser_options(parser: Parser, testomatio='testomatio') -> None:
-    parser.addoption(f'--{testomatio}',
+    group = parser.getgroup(testomatio, 'synchronise and connect test with testomat.io')
+    group.addoption(f'--{testomatio}',
                      action='store',
                      help=help_text)
-    parser.addoption(f'--testRunEnv',
+    group.addoption(f'--testRunEnv',
                      action='store',
                      help=f'specify test run environment for testomat.io. Works only with --testomatio sync')
-    parser.addoption(f'--create',
+    group.addoption(f'--create',
                      action='store_true',
                      default=False,
                      dest="create",
                      help="""
                         To import tests with Test IDs set in source code into a project use --create option.
                         In this case a project will be populated with the same Test IDs as in the code.
                         Use --testomatio sync together with --create option to enable this behavior.
                         """
                      )
-    parser.addoption(f'--no-empty',
+    group.addoption(f'--no-empty',
                      action='store_true',
                      default=False,
                      dest="no_empty",
                      help="""
                         Delete empty suites.
                         When tests are marked with IDs and imported to already created suites in Testomat.io newly imported suites may become empty.
                         Use --testomatio sync together with --no-empty option to clean them up after import.
                         """
                      )
-    parser.addoption(f'--no-detach',
+    group.addoption(f'--no-detach',
                      action='store_true',
                      default=False,
                      dest="no_detach",
                      help="""
                         Disable detaching tests.
                         If a test from a previous import was not found on next import it is marked as "detached".
                         This is done to ensure that deleted tests are not staying in Testomatio while deleted in codebase.
                         To disable this behaviour and don\'t mark anything on detached on import use sync together with --no-detached option.
                         """
                      )
-    parser.addoption(f'--keep-structure',
+    group.addoption(f'--keep-structure',
                      action='store_true',
                      default=False,
                      dest="keep_structure",
                      help="""
                         Keep structure of source code. If suites are not created in Testomat.io they will be created based on the file structure.
                         Use --testomatio sync together with --structure option to enable this behaviour.
                         """
                      )
-    parser.addoption('--directory',
+    group.addoption('--directory',
                      default=None,
                      dest="directory",
                      help="""
                         Specify directory to use for test file structure, ex. --directory Windows\\smoke or --directory Linux/e2e
                         Use --testomatio sync together with --directory option to enable this behaviour.
                         Default is the root of the project.
                         Note: --structure option takes precedence over --directory option. If both are used --structure will be used.
```

### Comparing `pytestomatio-2.5.0/pytestomatio/utils/validations.py` & `pytestomatio-2.5.2/pytestomatio/utils/validations.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
 from pytest import Config
 
 
-def validate_env_variables():
-    if os.getenv('TESTOMATIO') is None:
-        raise ValueError('TESTOMATIO env variable is not set')
+def validate_env_variables(config: Config):
+    if config.getoption('testomatio') and config.getoption('testomatio').lower() in ('sync', 'report', 'remove'):
+        if os.getenv('TESTOMATIO') is None:
+            raise ValueError('TESTOMATIO env variable is not set')
 
     # if os.getenv('TESTOMATIO_SHARED_RUN') and not os.getenv('TESTOMATIO_TITLE'):
     #     raise ValueError('TESTOMATIO_SHARED_RUN can only be used together with TESTOMATIO_TITLE')
 
 
 def validate_command_line_args(config: Config):
     if config.getoption('numprocesses'):
```

### Comparing `pytestomatio-2.5.0/pytestomatio/utils/worker_sync.py` & `pytestomatio-2.5.2/pytestomatio/utils/worker_sync.py`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.5.0/pytestomatio.egg-info/PKG-INFO` & `pytestomatio-2.5.2/pytestomatio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytestomatio
-Version: 2.5.0
+Version: 2.5.2
 Summary: Pytest plugin to sync test with testomat.io
 Author: Oleksii Ostapov, TikoQA
 Project-URL: Testomat.io, https://testomat.io/
 Project-URL: Homepage, https://github.com/testomatio/pytestomatio
 Project-URL: Bug Tracker, https://github.com/testomatio/pytestomatio/issues
 Classifier: Framework :: Pytest
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pytestomatio-2.5.0/pytestomatio.egg-info/SOURCES.txt` & `pytestomatio-2.5.2/pytestomatio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytestomatio-2.5.0/tests/test_root.py` & `pytestomatio-2.5.2/tests/test_root.py`

 * *Files identical despite different names*

