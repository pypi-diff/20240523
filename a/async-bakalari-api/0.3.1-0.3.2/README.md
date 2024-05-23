# Comparing `tmp/async_bakalari_api-0.3.1.tar.gz` & `tmp/async_bakalari_api-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async_bakalari_api-0.3.1.tar", last modified: Sun May 19 22:57:57 2024, max compression
+gzip compressed data, was "async_bakalari_api-0.3.2.tar", last modified: Thu May 23 14:16:46 2024, max compression
```

## Comparing `async_bakalari_api-0.3.1.tar` & `async_bakalari_api-0.3.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 22:57:57.291777 async_bakalari_api-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-19 22:57:52.000000 async_bakalari_api-0.3.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)    16439 2024-05-19 22:57:57.291777 async_bakalari_api-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-05-19 22:57:52.000000 async_bakalari_api-0.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     7790 2024-05-19 22:57:52.000000 async_bakalari_api-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-05-19 22:57:52.000000 async_bakalari_api-0.3.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 22:57:57.291777 async_bakalari_api-0.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 22:57:57.287777 async_bakalari_api-0.3.1/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 22:57:52.000000 async_bakalari_api-0.3.1/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 22:57:57.287777 async_bakalari_api-0.3.1/src/async_bakalari_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16439 2024-05-19 22:57:57.000000 async_bakalari_api-0.3.1/src/async_bakalari_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-19 22:57:57.000000 async_bakalari_api-0.3.1/src/async_bakalari_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 22:57:57.000000 async_bakalari_api-0.3.1/src/async_bakalari_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-19 22:57:57.000000 async_bakalari_api-0.3.1/src/async_bakalari_api.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 22:57:57.000000 async_bakalari_api-0.3.1/src/async_bakalari_api.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-19 22:57:57.000000 async_bakalari_api-0.3.1/src/async_bakalari_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-19 22:57:57.000000 async_bakalari_api-0.3.1/src/async_bakalari_api.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 22:57:57.287777 async_bakalari_api-0.3.1/src/bakalari_api/
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-19 22:57:52.000000 async_bakalari_api-0.3.1/src/bakalari_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-19 22:57:52.000000 async_bakalari_api-0.3.1/src/bakalari_api/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14669 2024-05-19 22:57:52.000000 async_bakalari_api-0.3.1/src/bakalari_api/bakalari.py
--rw-r--r--   0 runner    (1001) docker     (127)     8670 2024-05-19 22:57:52.000000 async_bakalari_api-0.3.1/src/bakalari_api/bakalari_demo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-05-19 22:57:52.000000 async_bakalari_api-0.3.1/src/bakalari_api/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     6797 2024-05-19 22:57:52.000000 async_bakalari_api-0.3.1/src/bakalari_api/datastructure.py
--rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-05-19 22:57:52.000000 async_bakalari_api-0.3.1/src/bakalari_api/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-19 22:57:52.000000 async_bakalari_api-0.3.1/src/bakalari_api/first_login.py
--rw-r--r--   0 runner    (1001) docker     (127)     5186 2024-05-19 22:57:52.000000 async_bakalari_api-0.3.1/src/bakalari_api/komens.py
--rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-05-19 22:57:52.000000 async_bakalari_api-0.3.1/src/bakalari_api/logger_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 22:57:57.287777 async_bakalari_api-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    19347 2024-05-19 22:57:52.000000 async_bakalari_api-0.3.1/tests/test_bakalari.py
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-19 22:57:52.000000 async_bakalari_api-0.3.1/tests/test_const.py
--rw-r--r--   0 runner    (1001) docker     (127)     7431 2024-05-19 22:57:52.000000 async_bakalari_api-0.3.1/tests/test_datastructure.py
--rw-r--r--   0 runner    (1001) docker     (127)     6270 2024-05-19 22:57:52.000000 async_bakalari_api-0.3.1/tests/test_komens.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:16:46.472306 async_bakalari_api-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-23 14:16:41.000000 async_bakalari_api-0.3.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)    17141 2024-05-23 14:16:46.472306 async_bakalari_api-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2956 2024-05-23 14:16:41.000000 async_bakalari_api-0.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7790 2024-05-23 14:16:41.000000 async_bakalari_api-0.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-23 14:16:41.000000 async_bakalari_api-0.3.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 14:16:46.472306 async_bakalari_api-0.3.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:16:46.468306 async_bakalari_api-0.3.2/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 14:16:41.000000 async_bakalari_api-0.3.2/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:16:46.472306 async_bakalari_api-0.3.2/src/async_bakalari_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17141 2024-05-23 14:16:46.000000 async_bakalari_api-0.3.2/src/async_bakalari_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-05-23 14:16:46.000000 async_bakalari_api-0.3.2/src/async_bakalari_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 14:16:46.000000 async_bakalari_api-0.3.2/src/async_bakalari_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-23 14:16:46.000000 async_bakalari_api-0.3.2/src/async_bakalari_api.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 14:16:46.000000 async_bakalari_api-0.3.2/src/async_bakalari_api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-23 14:16:46.000000 async_bakalari_api-0.3.2/src/async_bakalari_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-23 14:16:46.000000 async_bakalari_api-0.3.2/src/async_bakalari_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:16:46.468306 async_bakalari_api-0.3.2/src/bakalari_api/
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-23 14:16:41.000000 async_bakalari_api-0.3.2/src/bakalari_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-23 14:16:41.000000 async_bakalari_api-0.3.2/src/bakalari_api/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15151 2024-05-23 14:16:41.000000 async_bakalari_api-0.3.2/src/bakalari_api/bakalari.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10857 2024-05-23 14:16:41.000000 async_bakalari_api-0.3.2/src/bakalari_api/bakalari_demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1860 2024-05-23 14:16:41.000000 async_bakalari_api-0.3.2/src/bakalari_api/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6855 2024-05-23 14:16:41.000000 async_bakalari_api-0.3.2/src/bakalari_api/datastructure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-05-23 14:16:41.000000 async_bakalari_api-0.3.2/src/bakalari_api/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-23 14:16:41.000000 async_bakalari_api-0.3.2/src/bakalari_api/first_login.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7447 2024-05-23 14:16:41.000000 async_bakalari_api-0.3.2/src/bakalari_api/komens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-05-23 14:16:41.000000 async_bakalari_api-0.3.2/src/bakalari_api/logger_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:16:46.468306 async_bakalari_api-0.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    22046 2024-05-23 14:16:41.000000 async_bakalari_api-0.3.2/tests/test_bakalari.py
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-23 14:16:41.000000 async_bakalari_api-0.3.2/tests/test_const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7431 2024-05-23 14:16:41.000000 async_bakalari_api-0.3.2/tests/test_datastructure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9504 2024-05-23 14:16:41.000000 async_bakalari_api-0.3.2/tests/test_komens.py
```

### Comparing `async_bakalari_api-0.3.1/LICENSE.md` & `async_bakalari_api-0.3.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `async_bakalari_api-0.3.1/PKG-INFO` & `async_bakalari_api-0.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: async_bakalari_api
-Version: 0.3.1
+Version: 0.3.2
 Summary: Async API for Bakalari endpoint v3
 Author-email: "Lukas Svoboda (@schizza)" <opensource@schizza.cz>
 Maintainer-email: Lukas Svoboda <opensource@schizza.cz>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -215,14 +215,15 @@
 Keywords: bakalari,async
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
+Requires-Dist: aiofiles==23.2.1
 Requires-Dist: aiohttp==3.9.5
 Requires-Dist: aiosignal==1.3.1
 Requires-Dist: attrs==23.2.0
 Requires-Dist: frozenlist==1.4.1
 Requires-Dist: idna==3.7
 Requires-Dist: logger==1.4
 Requires-Dist: multidict==6.0.5
@@ -236,14 +237,29 @@
 
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 🇨🇿 Full documentation (czech) on [this site](https://async-bakalari-api.schizza.cz)
 
+## [0.3.1]
+
+### Added
+
+- `Schools` now support operations with towns
+- new data structure `UniqueTowns` that hold all town names
+  - `get_town_partial_name` returns list of the towns based on partial name
+  - `get_all_towns returns` list of all towns
+  - `istown` checks if the town is present in the list
+  - `count_towns` returns number of towns in list
+
+### Changed
+
+dependency list is divided to application dependencies and development dependencies
+
 ## [0.3]
 
 ### Added
 
 - `bakalari_demo.py` is now CLI application
 - `Komens` now support for downloading attachment - `get_attachment`
 - `send_auth_request` now supports extending EndPoints url wiht `extend` argument
@@ -297,8 +313,11 @@
 - `class Schools` in `datastructures.py` lists all schools with their API points
 
   - get_url by school name or index in list
   - search school by town
   - cache list of schools by saving and loading list in JSON format
 
 [unreleased]: https://github.com/schizza/bakalari-api3/compare/v0.0.1...HEAD
+[0.3.1]: https://https://github.com/schizza/bakalari-api3/releases/tag/0.3.1
+[0.3]: https://https://github.com/schizza/bakalari-api3/releases/tag/0.3
+[0.2]: https://github.com/schizza/bakalari-api3/releases/tag/0.2
 [0.0.1]: https://github.com/schizza/bakalari-api3/releases/tag/v0.0.1
```

### Comparing `async_bakalari_api-0.3.1/README.md` & `async_bakalari_api-0.3.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -2,14 +2,29 @@
 
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 🇨🇿 Full documentation (czech) on [this site](https://async-bakalari-api.schizza.cz)
 
+## [0.3.1]
+
+### Added
+
+- `Schools` now support operations with towns
+- new data structure `UniqueTowns` that hold all town names
+  - `get_town_partial_name` returns list of the towns based on partial name
+  - `get_all_towns returns` list of all towns
+  - `istown` checks if the town is present in the list
+  - `count_towns` returns number of towns in list
+
+### Changed
+
+dependency list is divided to application dependencies and development dependencies
+
 ## [0.3]
 
 ### Added
 
 - `bakalari_demo.py` is now CLI application
 - `Komens` now support for downloading attachment - `get_attachment`
 - `send_auth_request` now supports extending EndPoints url wiht `extend` argument
@@ -63,8 +78,11 @@
 - `class Schools` in `datastructures.py` lists all schools with their API points
 
   - get_url by school name or index in list
   - search school by town
   - cache list of schools by saving and loading list in JSON format
 
 [unreleased]: https://github.com/schizza/bakalari-api3/compare/v0.0.1...HEAD
+[0.3.1]: https://https://github.com/schizza/bakalari-api3/releases/tag/0.3.1
+[0.3]: https://https://github.com/schizza/bakalari-api3/releases/tag/0.3
+[0.2]: https://github.com/schizza/bakalari-api3/releases/tag/0.2
 [0.0.1]: https://github.com/schizza/bakalari-api3/releases/tag/v0.0.1
```

### Comparing `async_bakalari_api-0.3.1/pyproject.toml` & `async_bakalari_api-0.3.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "async_bakalari_api"
-version = "0.3.1"
+version = "0.3.2"
 dynamic = ["dependencies"]
 
 
 requires-python = ">=3.12"
 authors = [
   {name = "Lukas Svoboda (@schizza)", email = "opensource@schizza.cz"}
 ]
```

### Comparing `async_bakalari_api-0.3.1/requirements.txt` & `async_bakalari_api-0.3.2/requirements.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 #
 # This file is autogenerated by pip-compile with Python 3.12
 # by the following command:
 #
 #    pip-compile
 #
+aiofiles==23.2.1
+    # via -r requirements.in
 aiohttp==3.9.5
     # via -r requirements.in
 aiosignal==1.3.1
     # via aiohttp
 attrs==23.2.0
     # via aiohttp
 frozenlist==1.4.1
```

### Comparing `async_bakalari_api-0.3.1/src/async_bakalari_api.egg-info/PKG-INFO` & `async_bakalari_api-0.3.2/src/async_bakalari_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: async_bakalari_api
-Version: 0.3.1
+Version: 0.3.2
 Summary: Async API for Bakalari endpoint v3
 Author-email: "Lukas Svoboda (@schizza)" <opensource@schizza.cz>
 Maintainer-email: Lukas Svoboda <opensource@schizza.cz>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -215,14 +215,15 @@
 Keywords: bakalari,async
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Requires-Python: >=3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
+Requires-Dist: aiofiles==23.2.1
 Requires-Dist: aiohttp==3.9.5
 Requires-Dist: aiosignal==1.3.1
 Requires-Dist: attrs==23.2.0
 Requires-Dist: frozenlist==1.4.1
 Requires-Dist: idna==3.7
 Requires-Dist: logger==1.4
 Requires-Dist: multidict==6.0.5
@@ -236,14 +237,29 @@
 
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 🇨🇿 Full documentation (czech) on [this site](https://async-bakalari-api.schizza.cz)
 
+## [0.3.1]
+
+### Added
+
+- `Schools` now support operations with towns
+- new data structure `UniqueTowns` that hold all town names
+  - `get_town_partial_name` returns list of the towns based on partial name
+  - `get_all_towns returns` list of all towns
+  - `istown` checks if the town is present in the list
+  - `count_towns` returns number of towns in list
+
+### Changed
+
+dependency list is divided to application dependencies and development dependencies
+
 ## [0.3]
 
 ### Added
 
 - `bakalari_demo.py` is now CLI application
 - `Komens` now support for downloading attachment - `get_attachment`
 - `send_auth_request` now supports extending EndPoints url wiht `extend` argument
@@ -297,8 +313,11 @@
 - `class Schools` in `datastructures.py` lists all schools with their API points
 
   - get_url by school name or index in list
   - search school by town
   - cache list of schools by saving and loading list in JSON format
 
 [unreleased]: https://github.com/schizza/bakalari-api3/compare/v0.0.1...HEAD
+[0.3.1]: https://https://github.com/schizza/bakalari-api3/releases/tag/0.3.1
+[0.3]: https://https://github.com/schizza/bakalari-api3/releases/tag/0.3
+[0.2]: https://github.com/schizza/bakalari-api3/releases/tag/0.2
 [0.0.1]: https://github.com/schizza/bakalari-api3/releases/tag/v0.0.1
```

### Comparing `async_bakalari_api-0.3.1/src/async_bakalari_api.egg-info/SOURCES.txt` & `async_bakalari_api-0.3.2/src/async_bakalari_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `async_bakalari_api-0.3.1/src/bakalari_api/bakalari.py` & `async_bakalari_api-0.3.2/src/bakalari_api/bakalari.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,18 +47,22 @@
 
         self.server = server
         self.credentials = Credentials
         self.new_token = False
         self.auto_cache_credentials = auto_cache_credentials
         self.cache_filename = cache_filename
         self.session = aiohttp.ClientSession()
+        self.schools = Schools()
 
         if self.auto_cache_credentials and not self.cache_filename:
             raise Ex.CacheError("Auto-cache is enabled, but no filename is provided!")
 
+        if self.auto_cache_credentials and self.cache_filename:
+            self.load_credentials(self.cache_filename)
+
     def __del__(self):
         """Destructor."""
         # Close connection when this object is destroyed
         try:
             loop = asyncio.get_event_loop()
             if loop.is_running():
                 return loop.create_task(self.session.close())
@@ -183,19 +187,17 @@
             session = self.session.get
         else:
             session = self.session.post
 
         log.debug("Requesting URL %s, kwargs: %s", url, kwargs)
         try:
             async with asyncio.timeout(REQUEST_TIMEOUT):
-
                 async with session(
                     url, ssl=True, headers=headers, **kwargs
                 ) as response:
-
                     if (
                         response.headers.get(aiohttp.hdrs.CONTENT_TYPE)
                         == "application/octet-stream"
                     ):
                         filedata = await response.read()
                         filename = response.headers[aiohttp.hdrs.CONTENT_DISPOSITION]
                         filename = parse.unquote(
@@ -246,31 +248,41 @@
             case 404:
                 raise Ex.BadRequestException(f"Not found! ({url})")
             case 200:
                 return [filename, filedata] if filedata else response_json
             case _:
                 raise Ex.BadRequestException(f"{url} with message: {response_json}")
 
-    async def schools_list(self, town: str | None = None) -> Schools:
+    async def schools_list(
+        self, town: str | None = None, recursive: bool = True
+    ) -> Schools:
         """Return list of schools with their API points."""
 
         _schools_list = Schools()
         headers = {"Accept": "application/json"}
 
-        if not town:
-            log.debug("Gathering list of towns ...")
-            try:
-                towns_json = await self.send_unauth_request(
-                    EndPoint.SCHOOL_LIST, headers
-                )
-            except Exception as exc:
-                log.error(f"Error while gathering schools endpoints. {exc}")
-                return None
-        else:
-            towns_json: dict = [{"name": f"{town}"}]
+        log.debug("Gathering list of towns ...")
+        try:
+            towns_json = await self.send_unauth_request(EndPoint.SCHOOL_LIST, headers)
+        except Exception as exc:
+            log.error(f"Error while gathering schools endpoints. {exc}")
+            return None
+
+        if town and recursive:
+            towns_json = [
+                town_element
+                for town_element in towns_json
+                if town in town_element["name"]
+            ]
+        if town and not recursive:
+            towns_json = [
+                town_element
+                for town_element in towns_json
+                if town_element["name"].startswith(town)
+            ]
 
         schools: list = []
         tasks = []
 
         for _town in towns_json:
             town_name = str(_town["name"])
             if town_name == "" or None:
@@ -285,23 +297,24 @@
             task = asyncio.create_task(
                 self._send_request(endpoint, hdrs.METH_GET, headers), name=town_name
             )
             tasks.append(task)
 
         responses = await asyncio.gather(*tasks)
         for response_town in responses:
-
             schools: dict = response_town
             for _schools in schools.get("schools"):
                 _schools_list.append_school(
                     name=_schools.get("name"),
                     api_point=_schools.get("schoolUrl"),
                     town=response_town.get("name"),
                 )
 
+        self.schools = _schools_list
+
         return _schools_list
 
     async def first_login(self, username: str, password: str) -> Credentials:
         """First login.
 
         Create access and refresh tokens.
         """
```

### Comparing `async_bakalari_api-0.3.1/src/bakalari_api/bakalari_demo.py` & `async_bakalari_api-0.3.2/src/bakalari_api/bakalari_demo.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 """Main module."""
 
 import argparse
 import asyncio
+import os
 
+import aiofiles
 from logger import logging
 import orjson
 
 from .bakalari import Bakalari, Schools
-from .komens import Komens
+from .komens import Komens, MessageContainer
 from .logger_api import api_logger
 
 
-def w(name, data):
+async def w(name, data):
     """Write JSON data to file."""
-    with open(name, "+wb") as fi:
-        fi.write(orjson.dumps(data, option=orjson.OPT_INDENT_2))
+    async with aiofiles.open(name, "+wb") as fi:
+        await fi.write(orjson.dumps(data, option=orjson.OPT_INDENT_2))
+        await fi.flush()
 
 
-def wb(name, data):
+async def wb(name, data):
     """Write data to file."""
-    with open(name, "wb") as fi:
-        fi.write(data)
+    async with aiofiles.open(name, "wb") as fi:
+        await fi.write(data)
+        await fi.flush()
 
 
 def r(name):
     """Read data from file."""
     with open(name, "rb") as fi:
         return orjson.loads(fi.read())
 
@@ -61,34 +65,86 @@
             w(args.schools_file, _schools.school_list)
         except Exception as ex:
             print(ex)
 
 
 async def komens(args, bakalari):
     """Komens command."""
+
+    async def create_attachment_task(message: MessageContainer):
+        """Create a task for saving an attachment."""
+        tasks = []
+        if args.komens_save_attachment:
+            if message.isattachments():
+                for att in message.attachments:
+                    task = asyncio.create_task(
+                        wb(*(await Komens(bakalari=bakalari).get_attachment(att.id)))
+                    )
+                    tasks.append(task)
+        return tasks
+
+    async def msgs(messages):
+        """Print messages and save attachments if needed."""
+        tasks = []
+        for msg in messages:
+            print(str(msg))
+            tasks = create_attachment_task(msg)
+
+        asyncio.gather(*tasks)
+
+    async def msgs_w(messages):
+        """Save messages and attachments if needed."""
+        tasks = []
+
+        if isinstance(messages, MessageContainer):
+            await wb(args.komens_save, messages.as_json())
+            tasks.extend(await create_attachment_task(messages))
+
+        if isinstance(messages, list):
+            for msg in messages:
+                await wb(f"{args.komens_save}_{msg.mid}.json", msg.as_json())
+                tasks.extend(await create_attachment_task(msg))
+
+        await asyncio.gather(*tasks)
+
     if args.komens_list:
-        print(await Komens(bakalari=bakalari).fetch_messages())
+        if not args.komens_unread:
+            await msgs(await Komens(bakalari=bakalari).fetch_messages())
+        else:
+            await msgs(await Komens(bakalari=bakalari).get_unread_messages())
+
     if args.extend:
         messages = await Komens(bakalari=bakalari).fetch_messages()
-        print(messages.get_message_by_id(args.extend))
+        msgs([messages.get_message_by_id(args.extend)])
+
     if args.komens_save:
-        messages = await Komens(bakalari=bakalari).fetch_messages()
-        w(args.komens_save, messages.json())
+        if not args.komens_unread:
+            await msgs_w(await Komens(bakalari=bakalari).fetch_messages())
+        else:
+            await msgs_w(await Komens(bakalari=bakalari).get_unread_messages())
+
     if args.attachment:
-        wb(*(await Komens(bakalari=bakalari).get_attachment(args.attachment)))
+        await wb(*(await Komens(bakalari=bakalari).get_attachment(args.attachment)))
 
 
 async def runme(args):
     """Run the main function."""
 
     if args.sf:
-        schools: Schools = await Schools().load_from_file(args.sf)
+        try:
+            schools: Schools = await Schools().load_from_file(args.sf)
+        except Exception as ex:
+            os._exit(ex)
     else:
         schools: Schools = await Bakalari().schools_list(town=args.town)
 
+    if not schools:
+        print("Nenalezeny žádné školy")
+        os._exit(1)
+
     school = args.school
     if school:
         server = schools.get_url(school)
 
     if args.no_login:
         bakalari = Bakalari()
 
@@ -241,25 +297,35 @@
 
     parser.add_argument(
         "-v", "--verbose", action="store_true", help="Zapne podrobné logování"
     )
 
     komens_action = komens_parser.add_mutually_exclusive_group()
     komens_parser.add_argument(
-        "--messages",
+        "-u",
+        "--unread",
+        help="Vypíše nepřečtené zprávy",
+        dest="komens_unread",
+        action="store_true",
+    )
+    komens_parser.add_argument(
+        "-sa",
+        "--save_attachment",
         action="store_true",
-        help="Načte zprávy z Komens",
+        help="Uloží automaticky přílohy zpráv do souboru",
+        dest="komens_save_attachment",
     )
     komens_action.add_argument(
         "-l",
         "--list",
         help="Vypíše přijaté zprávy",
         dest="komens_list",
         action="store_true",
     )
+
     komens_action.add_argument(
         "-e",
         "--extend",
         nargs=None,
         metavar="ID_zprávy",
         help="Vypíše podrobně zprávu s ID zprávy.",
     )
@@ -275,10 +341,13 @@
     komens_parser.add_argument(
         "--attachment", nargs=None, metavar="ID_přílohy", help="Stáhne přílohu zprávy."
     )
 
     args = parser.parse_args()
 
     if args.verbose:
-        api_logger("Bakalari API").get().setLevel(logging.DEBUG)
+        log = api_logger("Bakalari API", loglevel=logging.DEBUG).get()
+    else:
+        log = api_logger("Bakalari API").get()
 
-    asyncio.run(runme(args))
+    loop = asyncio.get_event_loop()
+    loop.run_until_complete(runme(args))
```

### Comparing `async_bakalari_api-0.3.1/src/bakalari_api/const.py` & `async_bakalari_api-0.3.2/src/bakalari_api/const.py`

 * *Files identical despite different names*

### Comparing `async_bakalari_api-0.3.1/src/bakalari_api/datastructure.py` & `async_bakalari_api-0.3.2/src/bakalari_api/datastructure.py`

 * *Files 2% similar despite different names*

```diff
@@ -218,14 +218,15 @@
     async def load_from_file(self, filename: str) -> Schools:
         """Load schools list from a file."""
 
         try:
             with open(filename, mode="+rb") as file:
                 data = orjson.loads(file.read())
         except OSError:
+            log.error(f"Unable to open file {filename}.")
             return False
         except orjson.JSONDecodeError:
             log.error(f"Unable to decode JSON file. File {filename} is corrupted.")
             return False
 
         for item in data:
             self.append_school(
```

### Comparing `async_bakalari_api-0.3.1/src/bakalari_api/exceptions.py` & `async_bakalari_api-0.3.2/src/bakalari_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `async_bakalari_api-0.3.1/src/bakalari_api/komens.py` & `async_bakalari_api-0.3.2/src/bakalari_api/komens.py`

 * *Files 21% similar despite different names*

```diff
@@ -10,91 +10,154 @@
 from .bakalari import Bakalari
 from .const import EndPoint
 from .logger_api import api_logger
 
 log = api_logger("Bakalari API").get()
 
 
+class AttachmentsRegistry:
+    """Attachments registry."""
+
+    id: str
+    name: str
+
+    def __init__(self, *, id: str, name: str):
+        """Initialize Attachments."""
+
+        _setter = object.__setattr__
+        _setter(self, "id", id)
+        _setter(self, "name", name)
+
+    def __setattr__(self, key: str, value: Any) -> None:
+        """Set an attribute."""
+        super().__setattr__(key, value)
+
+    def __getattr__(self, key: str) -> Any:
+        """Get an attribute."""
+        log.error(f"AttributeError: {key} not found.")
+        return f"You tried to access {key}, but it doesn't exist!"
+
+    def __str__(self) -> str:
+        """Return string representation of data."""
+        return f"id: {self.id} name: {self.name}"
+
+    def __repr__(self) -> str:
+        """Representation of Attachments."""
+        return f"<Attachments id={self.id} name={self.name}>"
+
+    def __format__(self, format_spec: str) -> str:
+        """Format string representation of data."""
+        return self.__str__()
+
+    def as_json(self) -> str:
+        """Return JSON fragment of attachment."""
+
+        return f"{{'id': {self.id}, 'name': {self.name}}}"
+
+
 class MessageContainer:
     """Messages registry."""
 
     mid: str
     title: str
     text: str
     sent: dt
     sender: dict[str, str]
-    attachments: dict[str, str]
+    read: bool
+    attachments: list[AttachmentsRegistry]
 
     def __init__(
         self,
         *,
         mid: str,
         title: str,
         text: str,
         sent: dt,
         sender: dict[str, str],
-        attachments: dict[str, str] | None = None,
+        read: bool,
+        attachments: list[AttachmentsRegistry] = {},
     ):
         """Initialize MessagesContainer."""
 
+        if attachments != {}:
+            attachments = [
+                AttachmentsRegistry(id=i["Id"], name=i["Name"]) for i in attachments
+            ]
+
         _setter = object.__setattr__
         _setter(self, "mid", mid)
         _setter(self, "title", title)
         _setter(self, "text", text)
         _setter(self, "sent", sent.date())
         _setter(self, "sender", sender)
+        _setter(self, "read", read)
         _setter(self, "attachments", attachments)
 
     def __repr__(self) -> str:
         """Representation of MessageContainer."""
         return (
             f"<MessageContainer message_id={self.mid} "
-            f"title={self.title} sender={self.sender}>"
+            f"title={self.title} sender={self.sender} "
+            f"attachments={self.attachments}>"
         )
 
     def __setattr__(self, key: str, value: Any) -> None:
         """Set an attribute."""
         super().__setattr__(key, value)
 
     def as_json(self) -> bytes:
         """Return JSON fragment of message."""
         json_repr = {
             "mid": self.mid,
             "title": self.title,
             "text": self.text,
             "sent": self.sent,
             "sender": self.sender,
-            "attachments": self.attachments,
+            "read": self.read,
+            "attachments": self.attachments_as_json(),
         }
         return orjson.dumps(json_repr)
 
     def __str__(self) -> str:
         """Return string representation of data."""
-        return f"""Message id: {self.mid}
-            title: {self.title}
-            text: {self.text}
-            sent: {self.sent}
-            sender: {self.sender}
-            attachments: {self.attachments}"""
+        att = (str(a) for a in self.attachments)
+        return (
+            f"Message id: {self.mid}\n"
+            f"title: {self.title}\n"
+            f"text: {self.text}\n"
+            f"sent: {self.sent}\n"
+            f"sender: {self.sender}\n"
+            f"read: {self.read}\n"
+            f"attachments: {"".join(att)}\n"
+        )
+
+    def __format__(self, format_spec: str) -> str:
+        """Format string representation of data."""
+        return self.__str__()
+
+    def attachments_as_json(self) -> str:
+        """Return JSON fragment of attachments."""
+        return [a.as_json() for a in self.attachments]
+
+    def isattachments(self) -> bool:
+        """Check if message contains attachment."""
+        return bool(self.attachments)
 
 
 class Messages(list[MessageContainer]):
     """Messages class holds all messages."""
 
     def __init__(self) -> None:
         """Messages class holds all messages."""
         super().__init__()
 
     def __str__(self) -> str:
         """Print string representation."""
 
-        text = ""
-        for message in self:
-            text += message.__str__() + "\n"
-        return text
+        return "".join(str(message) for message in self)
 
     def json(self):
         """Return json representation of Messages."""
 
         return [orjson.loads(m.as_json()) for m in self]
 
     def get_message_by_id(self, id: str) -> MessageContainer:
@@ -149,21 +212,28 @@
             log.debug(f"Writing message: {msg}")
             return MessageContainer(
                 mid=msg["Id"],
                 title=msg["Title"],
                 text=msg["Text"],
                 sent=dateutil.parser.parse(msg["SentDate"]),
                 sender=msg["Sender"]["Name"],
+                read=msg["Read"],
                 attachments=msg["Attachments"],
             )
 
         self.messages.extend([(await create_msg(msg)) for msg in messages["Messages"]])
 
         return self.messages
 
+    async def get_unread_messages(self) -> list[MessageContainer]:
+        """Get unread messages."""
+        if self.messages.count_messages() == 0:
+            await self.fetch_messages()
+        return [msg for msg in self.messages if msg.read is False]
+
     async def count_unread_messages(self) -> int:
         """Get count of unreaded messages."""
         return await self.bakalari.send_auth_request(EndPoint.KOMENS_UNREAD_COUNT)
 
     async def get_attachment(self, id: str) -> Any:
         """Get attachment.
```

### Comparing `async_bakalari_api-0.3.1/src/bakalari_api/logger_api.py` & `async_bakalari_api-0.3.2/src/bakalari_api/logger_api.py`

 * *Files identical despite different names*

### Comparing `async_bakalari_api-0.3.1/tests/test_bakalari.py` & `async_bakalari_api-0.3.2/tests/test_bakalari.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,19 +67,64 @@
     assert "Bad endpoint url" in str(ex.value)
 
     bakalari.server = "http://fake_server"
     final_url = bakalari.get_request_url(EndPoint.LOGIN)
     assert final_url == "http://fake_server/api/login"
 
 
+async def test_schools_list_not_recursive():
+    """Test the schools_list method withou recrusive parameter of the Bakalari class."""
+    bakalari = Bakalari()
+    pattern = re.compile(r"^https://sluzby\.bakalari\.cz/.*$")
+    api_logger("Bakalari API", loglevel=10).get()
+
+    with aioresponses() as m:
+        # town is provided, recursive is False
+        m.get(
+            pattern,
+            headers={"Accept": "application/json"},
+            body="""
+            [
+                {
+                    "name": "town name.a",
+                    "schoolCount": 1
+                },
+                {
+                    "name": "name town.b",
+                    "schoolCount": 1
+                },
+                {
+                    "name":"no town.c"}
+            ]
+            """,
+            status=200,
+        )
+        m.get(
+            pattern,
+            headers={"Accept": "application/json"},
+            body="""{"name": "name town.b", "schools": [{"name": "school_name_town.b","schoolUrl": "endpoint_url_town.b"}]}""",
+        )
+
+        m.get(
+            pattern,
+            headers={"Accept": "application/json"},
+            body="""{"name": "town name.a", "schools": [{"name": "school_name_town.a","schoolUrl": "endpoint_url_town.a"}]}""",
+        )
+
+        s: Schools = await bakalari.schools_list(town="name", recursive=False)
+    assert isinstance(s, Schools)
+    assert not s.get_url("school_name_town.a")
+    assert s.get_url("school_name_town.b") == "endpoint_url_town.b"
+
+
 async def test_school_list():
     """Test the schools_list method of the Bakalari class."""
     bakalari = Bakalari()
     pattern = re.compile(r"^https://sluzby\.bakalari\.cz/.*$")
-    api_logger("Bakalari API").get().setLevel(10)
+    api_logger("Bakalari API", loglevel=10).get()
 
     with aioresponses() as m:
         m.get(
             pattern,
             headers={"Accept": "application/json"},
             body="""[{"name": "town_name.a","schoolCount": 1},{"name":""}]""",
             status=200,
@@ -101,22 +146,57 @@
             pattern,
             headers={"Accept": "application/json"},
             body="""{"name": "town_name", "schools": [{"name": "school_name","schoolUrl": "endpoint_url"}]}""",
         )
         result = await bakalari.schools_list()
         assert not result
 
+        # town is provided
         m.get(
             pattern,
             headers={"Accept": "application/json"},
-            body="""{"name": "town_name", "schools": [{"name": "school_name","schoolUrl": "endpoint_url"}]}""",
+            body="""
+            [
+                {
+                    "name": "town name.a",
+                    "schoolCount": 1
+                },
+                {
+                    "name": "name town.b",
+                    "schoolCount": 1
+                },
+                {
+                    "name":"no town.c"}
+            ]
+            """,
+            status=200,
+        )
+
+        m.get(
+            pattern,
+            headers={"Accept": "application/json"},
+            body="""{"name": "town name.a", "schools": [{"name": "school_name_town.a","schoolUrl": "endpoint_url_town.a"}]}""",
+        )
+
+        m.get(
+            pattern,
+            headers={"Accept": "application/json"},
+            body="""{"name": "name town.b", "schools": [{"name": "school_name_town.b","schoolUrl": "endpoint_url_town.b"}]}""",
+        )
+
+        m.get(
+            pattern,
+            headers={"Accept": "application/json"},
+            body="""{"name": "no town.c", "schools": [{"name": "school_name_no_town.c","schoolUrl": "endpoint_url_town.c"}]}""",
         )
-        result = await bakalari.schools_list(town="town_name")
+        result = await bakalari.schools_list(town="name")
         assert isinstance(result, Schools)
-        assert result.get_url("school_name") == "endpoint_url"
+        assert result.get_url("school_name_town.a") == "endpoint_url_town.a"
+        assert result.get_url("school_name_town.b") == "endpoint_url_town.b"
+        assert not result.get_url("school_name_no_town.c")
 
 
 async def test__send_request_aioex():
     """Test the _send_request function with aiohttp.ClientConnectionError and TimeoutError exceptions."""
 
     bakalari = Bakalari("fake_server")
 
@@ -125,20 +205,24 @@
             await bakalari._send_request("fake_server", hdrs.METH_GET, "")
         except Ex.TimeoutException:
             pytest.raises(Ex.TimeoutException)
         except aiohttp.ClientConnectionError:
             pytest.fail("ClientConnectionError should not be raised")
         except Exception as ex:
             pytest.fail(f"Unexpected exception: {ex}")
+        finally:
+            await bakalari.session.close()
 
     with patch("aiohttp.ClientSession.get", side_effect=aiohttp.ClientConnectionError):
         try:
             await bakalari._send_request("fake_server", hdrs.METH_GET, "")
         except Ex.BadRequestException:
             pytest.raises(Ex.BadRequestException)
+        finally:
+            await bakalari.session.close()
 
 
 async def test_send_auth_request():
     """Test the send_auth_request method of the Bakalari class."""
 
     cache_file = f"{tempfile.TemporaryDirectory()}/cache_file"
 
@@ -479,21 +563,19 @@
     assert bakalari.credentials.refresh_token == "test_refresh"
 
 
 async def test_save_file_success():
     """Test the save_credentials method of the Bakalari class."""
 
     bakalari = Bakalari()
-    bakalari.credentials = bakalari.credentials.create_from_json(
-        {
-            "access_token": "test_access",
-            "refresh_token": "test_refresh",
-            "user_id": "test_user_id",
-        }
-    )
+    bakalari.credentials = bakalari.credentials.create_from_json({
+        "access_token": "test_access",
+        "refresh_token": "test_refresh",
+        "user_id": "test_user_id",
+    })
 
     with tempfile.TemporaryDirectory() as temp_dir:
         filename = temp_dir + "test_data"
         bakalari.save_credentials(filename=filename)
 
         with open(filename, "+rb") as file:
             data = orjson.loads(file.read())
@@ -516,21 +598,19 @@
 
     # we have auto_cache, but no filename provided.
     with pytest.raises(Ex.CacheError) as ex:
         bakalari = Bakalari("", auto_cache_credentials=True, cache_filename=None)
     assert "Auto-cache is enabled, but no filename is provided!" in str(ex.value)
 
     bakalari = Bakalari("", auto_cache_credentials=True, cache_filename="fake_file")
-    bakalari.credentials = bakalari.credentials.create_from_json(
-        {
-            "access_token": "test_access",
-            "refresh_token": "test_refresh",
-            "user_id": "test_user_id",
-        }
-    )
+    bakalari.credentials = bakalari.credentials.create_from_json({
+        "access_token": "test_access",
+        "refresh_token": "test_refresh",
+        "user_id": "test_user_id",
+    })
 
     with tempfile.TemporaryDirectory() as temp_dir:
         filename = temp_dir + "test_data"
         bakalari.cache_filename = filename
         bakalari.save_credentials()
 
         with open(filename, "+rb") as file:
```

### Comparing `async_bakalari_api-0.3.1/tests/test_datastructure.py` & `async_bakalari_api-0.3.2/tests/test_datastructure.py`

 * *Files identical despite different names*

### Comparing `async_bakalari_api-0.3.1/tests/test_komens.py` & `async_bakalari_api-0.3.2/tests/test_komens.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 """Test for Komens class."""
 
 import datetime as dt
 
 from aioresponses import aioresponses
-import orjson
 from src.bakalari_api.bakalari import Bakalari
 from src.bakalari_api.const import EndPoint
-from src.bakalari_api.komens import Komens, Messages
+from src.bakalari_api.komens import AttachmentsRegistry, Komens, Messages
 
 fs = "http://fake_server"
 
 payload = """
 {
   "Messages": [
     {
@@ -73,14 +72,121 @@
       "CanHide": true,
       "CanDelete": false,
       "RelevantName": "fake_relevant_name2",
       "RelevantPersonType": "fake_relevant_person2"
     }
    ]}"""
 
+payload_unread = """{
+  "Messages": [
+    {
+      "$type": "GeneralMessage",
+      "Id": "fake_id1",
+      "Title": "",
+      "Text": "fake_text_id1",
+      "SentDate": "2024-01-01T13:37:28+02:00",
+      "Sender": {
+        "$type": "Sender",
+        "Id": "fake_sender_ID",
+        "Type": "teacher",
+        "Name": "fake_teacher_name1"
+      },
+      "Attachments": [
+        {
+          "$type": "AttachmentInfo",
+          "Id": "fake_attachment_id1",
+          "Name": "fake_atachement_name1",
+          "Type": "fake_type",
+          "Size": 12345
+        }
+      ],
+      "Read": false,
+      "LifeTime": "ToRead",
+      "DateFrom": null,
+      "DateTo": null,
+      "Confirmed": true,
+      "CanConfirm": false,
+      "Type": "OBECNA",
+      "CanAnswer": true,
+      "Hidden": false,
+      "CanHide": true,
+      "CanDelete": false,
+      "RelevantName": "fake_relevant_name1",
+      "RelevantPersonType": "fake_relevant_person1"
+    },
+    {
+      "$type": "GeneralMessage",
+      "Id": "fake_id2",
+      "Title": "",
+      "Text": "fake_text_id2",
+      "SentDate": "2024-01-05T13:37:28+02:00",
+      "Sender": {
+        "$type": "Sender",
+        "Id": "fake_sender_ID",
+        "Type": "teacher",
+        "Name": "fake_teacher_name2"
+      },
+      "Attachments": [],
+      "Read": true,
+      "LifeTime": "ToRead",
+      "DateFrom": null,
+      "DateTo": null,
+      "Confirmed": true,
+      "CanConfirm": false,
+      "Type": "OBECNA",
+      "CanAnswer": true,
+      "Hidden": false,
+      "CanHide": true,
+      "CanDelete": false,
+      "RelevantName": "fake_relevant_name2",
+      "RelevantPersonType": "fake_relevant_person2"
+    }
+   ]}"""
+
+
+def test_attributes_Att_registry():
+    """Test the AttachmentsRegistry class attributes."""
+
+    att = AttachmentsRegistry(id="id", name="name")
+
+    att.id = "fake_id"
+    assert att.fake_id == "You tried to access fake_id, but it doesn't exist!"
+    assert att.id == "fake_id"
+    assert format(att) == "id: fake_id name: name"
+
+
+async def test_get_unread_messages():
+    """Test the get_unread_messages method of the Komens class."""
+
+    bakalari = Bakalari(fs)
+    komens = Komens(bakalari)
+    bakalari.credentials.access_token = "token"
+
+    with aioresponses() as m:
+        m.post(
+            url=fs + EndPoint.KOMENS_UNREAD.get("endpoint"),
+            body=payload_unread,
+            headers={},
+            status=200,
+        )
+
+        msgs = await komens.get_unread_messages()
+        assert isinstance(msgs, list)
+        assert len(msgs) == 1
+        assert msgs[0].isattachments() is True
+        assert format(msgs[0]) == (
+            "Message id: fake_id1\n"
+            "title: \n"
+            "text: fake_text_id1\n"
+            "sent: 2024-01-01\n"
+            "sender: fake_teacher_name1\n"
+            "read: False\n"
+            "attachments: id: fake_attachment_id1 name: fake_atachement_name1\n"
+        )
+
 
 async def test_komens_get_messages():
     """Test the Komens class and its methods."""
 
     bakalari = Bakalari(fs)
     komens = Komens(bakalari)
     bakalari.credentials.access_token = "token"
@@ -100,75 +206,81 @@
 
         assert msg.mid == "fake_id1"
         assert msg.sender == "fake_teacher_name1"
         assert msg.text == "fake_text_id1"
         assert msg.title == ""
 
         assert (
-            str(msgs)
-            == """Message id: fake_id1
-            title: 
-            text: fake_text_id1
-            sent: 2024-01-01
-            sender: fake_teacher_name1
-            attachments: [{'$type': 'AttachmentInfo', 'Id': 'fake_attachment_id1', 'Name': 'fake_atachement_name1', 'Type': 'fake_type', 'Size': 12345}]
-Message id: fake_id2
-            title: 
-            text: fake_text_id2
-            sent: 2024-01-05
-            sender: fake_teacher_name2
-            attachments: []
-"""
+            str(msgs) == "Message id: fake_id1\n"
+            "title: \n"
+            "text: fake_text_id1\n"
+            "sent: 2024-01-01\n"
+            "sender: fake_teacher_name1\n"
+            "read: True\n"
+            "attachments: id: fake_attachment_id1 name: fake_atachement_name1\n"
+            "Message id: fake_id2\n"
+            "title: \n"
+            "text: fake_text_id2\n"
+            "sent: 2024-01-05\n"
+            "sender: fake_teacher_name2\n"
+            "read: True\n"
+            "attachments: \n"
         )
         assert_msgs = [
             {
                 "mid": msg.mid,
                 "title": msg.title,
                 "text": msg.text,
-                "sent": msg.sent,
+                "sent": str(msg.sent),
                 "sender": msg.sender,
-                "attachments": msg.attachments,
+                "read": msg.read,
+                "attachments": msg.attachments_as_json(),
             }
             for msg in msgs
         ]
-        assert msgs.json() == orjson.loads(orjson.dumps(assert_msgs))
+
+        assert msgs.json() == assert_msgs  # orjson.loads(orjson.dumps(assert_msgs))
 
         msg = komens.messages.get_messages_by_date(dt.date(2024, 1, 1))
         assert msg[0].mid == "fake_id1"
 
         msg = komens.messages.get_messages_by_date(
             dt.date(2024, 1, 1), to_date=dt.date(2024, 1, 1) + dt.timedelta(days=+5)
         )
         assert isinstance(msg, list)
         assert len(msg) == 2
         assert msg[1].mid == "fake_id2"
         assert (
-            str(msg[1])
-            == """Message id: fake_id2
-            title: 
-            text: fake_text_id2
-            sent: 2024-01-05
-            sender: fake_teacher_name2
-            attachments: []"""
+            str(msg[1]) == "Message id: fake_id2\n"
+            "title: \n"
+            "text: fake_text_id2\n"
+            "sent: 2024-01-05\n"
+            "sender: fake_teacher_name2\n"
+            "read: True\n"
+            "attachments: \n"
         )
 
         assert (
             repr(msg[0])
-            == "<MessageContainer message_id=fake_id1 title= sender=fake_teacher_name1>"
+            == "<MessageContainer message_id=fake_id1 title= sender=fake_teacher_name1 attachments=[<Attachments id=fake_attachment_id1 name=fake_atachement_name1>]>"
         )
 
         # JSON
         assert (
             msg[1].as_json()
-            == b'{"mid":"fake_id2","title":"","text":"fake_text_id2","sent":"2024-01-05","sender":"fake_teacher_name2","attachments":[]}'
+            == b'{"mid":"fake_id2","title":"","text":"fake_text_id2","sent":"2024-01-05","sender":"fake_teacher_name2","read":true,"attachments":[]}'
         )
 
         msg[0].title = "new_set_title"
         assert msg[0].title == "new_set_title"
 
+        # Test isattachments
+        assert msg[0].isattachments() is True
+        assert msg[1].isattachments() is False
+
 
 async def test_komens_count_unread_messages():
     """Test the count_unread_messages method of the Komens class."""
 
     bakalari = Bakalari(fs)
     komens = Komens(bakalari)
     bakalari.credentials.access_token = "token"
```

