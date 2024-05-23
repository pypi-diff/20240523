# Comparing `tmp/profile_facebook_selenium_scraper_imp_local-0.0.4.tar.gz` & `tmp/profile_facebook_selenium_scraper_imp_local-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "profile_facebook_selenium_scraper_imp_local-0.0.4.tar", last modified: Wed May 22 17:44:27 2024, max compression
+gzip compressed data, was "profile_facebook_selenium_scraper_imp_local-0.0.5.tar", last modified: Thu May 23 04:39:26 2024, max compression
```

## Comparing `profile_facebook_selenium_scraper_imp_local-0.0.4.tar` & `profile_facebook_selenium_scraper_imp_local-0.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:44:26.999757 profile_facebook_selenium_scraper_imp_local-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-22 17:44:26.995757 profile_facebook_selenium_scraper_imp_local-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-05-22 17:43:54.000000 profile_facebook_selenium_scraper_imp_local-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:44:26.995757 profile_facebook_selenium_scraper_imp_local-0.0.4/profile_facebook_selenium_scraper_imp_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:44:26.995757 profile_facebook_selenium_scraper_imp_local-0.0.4/profile_facebook_selenium_scraper_imp_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 17:43:54.000000 profile_facebook_selenium_scraper_imp_local-0.0.4/profile_facebook_selenium_scraper_imp_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-22 17:43:54.000000 profile_facebook_selenium_scraper_imp_local-0.0.4/profile_facebook_selenium_scraper_imp_local/src/facebook_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    15574 2024-05-22 17:43:54.000000 profile_facebook_selenium_scraper_imp_local-0.0.4/profile_facebook_selenium_scraper_imp_local/src/facebook_scraper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:44:26.995757 profile_facebook_selenium_scraper_imp_local-0.0.4/profile_facebook_selenium_scraper_imp_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-22 17:44:26.000000 profile_facebook_selenium_scraper_imp_local-0.0.4/profile_facebook_selenium_scraper_imp_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-22 17:44:26.000000 profile_facebook_selenium_scraper_imp_local-0.0.4/profile_facebook_selenium_scraper_imp_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 17:44:26.000000 profile_facebook_selenium_scraper_imp_local-0.0.4/profile_facebook_selenium_scraper_imp_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-22 17:44:26.000000 profile_facebook_selenium_scraper_imp_local-0.0.4/profile_facebook_selenium_scraper_imp_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-22 17:44:26.000000 profile_facebook_selenium_scraper_imp_local-0.0.4/profile_facebook_selenium_scraper_imp_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-22 17:43:54.000000 profile_facebook_selenium_scraper_imp_local-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 17:44:26.999757 profile_facebook_selenium_scraper_imp_local-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-22 17:43:54.000000 profile_facebook_selenium_scraper_imp_local-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 04:39:26.283393 profile_facebook_selenium_scraper_imp_local-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-23 04:39:26.283393 profile_facebook_selenium_scraper_imp_local-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-23 04:38:52.000000 profile_facebook_selenium_scraper_imp_local-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 04:39:26.279393 profile_facebook_selenium_scraper_imp_local-0.0.5/profile_facebook_selenium_scraper_imp_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 04:39:26.283393 profile_facebook_selenium_scraper_imp_local-0.0.5/profile_facebook_selenium_scraper_imp_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 04:38:52.000000 profile_facebook_selenium_scraper_imp_local-0.0.5/profile_facebook_selenium_scraper_imp_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-05-23 04:38:52.000000 profile_facebook_selenium_scraper_imp_local-0.0.5/profile_facebook_selenium_scraper_imp_local/src/facebook_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15718 2024-05-23 04:38:52.000000 profile_facebook_selenium_scraper_imp_local-0.0.5/profile_facebook_selenium_scraper_imp_local/src/facebook_scraper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 04:39:26.283393 profile_facebook_selenium_scraper_imp_local-0.0.5/profile_facebook_selenium_scraper_imp_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-23 04:39:26.000000 profile_facebook_selenium_scraper_imp_local-0.0.5/profile_facebook_selenium_scraper_imp_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-23 04:39:26.000000 profile_facebook_selenium_scraper_imp_local-0.0.5/profile_facebook_selenium_scraper_imp_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 04:39:26.000000 profile_facebook_selenium_scraper_imp_local-0.0.5/profile_facebook_selenium_scraper_imp_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-23 04:39:26.000000 profile_facebook_selenium_scraper_imp_local-0.0.5/profile_facebook_selenium_scraper_imp_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-23 04:39:26.000000 profile_facebook_selenium_scraper_imp_local-0.0.5/profile_facebook_selenium_scraper_imp_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-23 04:38:52.000000 profile_facebook_selenium_scraper_imp_local-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 04:39:26.283393 profile_facebook_selenium_scraper_imp_local-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-23 04:38:52.000000 profile_facebook_selenium_scraper_imp_local-0.0.5/setup.py
```

### Comparing `profile_facebook_selenium_scraper_imp_local-0.0.4/PKG-INFO` & `profile_facebook_selenium_scraper_imp_local-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: profile-facebook-selenium-scraper-imp-local
-Version: 0.0.4
+Version: 0.0.5
 Summary: PyPI Package for Circles profile-facebook-selenium-scraper-imp-local Python
 Home-page: https://github.com/circles-zone/profile-facebook-selenium-scraper-imp-local-python-package
 Author: Circles
 Author-email: info@circlez.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `profile_facebook_selenium_scraper_imp_local-0.0.4/profile_facebook_selenium_scraper_imp_local/src/facebook_constants.py` & `profile_facebook_selenium_scraper_imp_local-0.0.5/profile_facebook_selenium_scraper_imp_local/src/facebook_constants.py`

 * *Files identical despite different names*

### Comparing `profile_facebook_selenium_scraper_imp_local-0.0.4/profile_facebook_selenium_scraper_imp_local/src/facebook_scraper.py` & `profile_facebook_selenium_scraper_imp_local-0.0.5/profile_facebook_selenium_scraper_imp_local/src/facebook_scraper.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,16 @@
 LOGGER_CODE_OBJECT = {
     'component_id': QUEUE_LOCAL_PYTHON_COMPONENT_ID,
     'component_name': QUEUE_LOCAL_PYTHON_COMPONENT_NAME,
     'component_category': LoggerComponentEnum.ComponentCategory.Code.value,
     'developer_email': DEVELOPER_EMAIL
 }
 
-
+# TODO: make sure we can see the data in  importer views, data_source_instance and api_call
+#   using importing/sync of contacts/people/profiles
 class FacebookScraper(metaclass=MetaLogger, object=LOGGER_CODE_OBJECT):
     """Class for scraping Facebook friends' information."""
 
     def __init__(self, facebook_user_identifier: str = None, facebook_password: str = None) -> None:
         """Initializes the FacebookScraper class."""
         self.comprehensive_profile = ComprehensiveProfileLocal()
         # TODO: use dict instead of self, and use all
```

### Comparing `profile_facebook_selenium_scraper_imp_local-0.0.4/profile_facebook_selenium_scraper_imp_local.egg-info/PKG-INFO` & `profile_facebook_selenium_scraper_imp_local-0.0.5/profile_facebook_selenium_scraper_imp_local.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: profile-facebook-selenium-scraper-imp-local
-Version: 0.0.4
+Version: 0.0.5
 Summary: PyPI Package for Circles profile-facebook-selenium-scraper-imp-local Python
 Home-page: https://github.com/circles-zone/profile-facebook-selenium-scraper-imp-local-python-package
 Author: Circles
 Author-email: info@circlez.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `profile_facebook_selenium_scraper_imp_local-0.0.4/profile_facebook_selenium_scraper_imp_local.egg-info/SOURCES.txt` & `profile_facebook_selenium_scraper_imp_local-0.0.5/profile_facebook_selenium_scraper_imp_local.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `profile_facebook_selenium_scraper_imp_local-0.0.4/pyproject.toml` & `profile_facebook_selenium_scraper_imp_local-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `profile_facebook_selenium_scraper_imp_local-0.0.4/setup.py` & `profile_facebook_selenium_scraper_imp_local-0.0.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "profile-facebook-selenium-scraper-imp-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,
-    version='0.0.4',  # https://pypi.org/project/profile-facebook-selenium-scraper-imp-local/
+    version='0.0.5',  # https://pypi.org/project/profile-facebook-selenium-scraper-imp-local/
     author="Circles",
     author_email="info@circlez.ai",
     description=f"PyPI Package for Circles {PACKAGE_NAME} Python",
     long_description=f"PyPI Package for Circles {PACKAGE_NAME} Python",
     long_description_content_type='text/markdown',
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
```

