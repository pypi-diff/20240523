# Comparing `tmp/svd2json-0.1.5.tar.gz` & `tmp/svd2json-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "svd2json-0.1.5.tar", last modified: Thu May 23 14:19:01 2024, max compression
+gzip compressed data, was "svd2json-0.1.6.tar", last modified: Thu May 23 15:14:17 2024, max compression
```

## Comparing `svd2json-0.1.5.tar` & `svd2json-0.1.6.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 pthierry  (1000) pthierry  (1000)        0 2024-05-23 14:19:01.952179 svd2json-0.1.5/
-drwxrwxr-x   0 pthierry  (1000) pthierry  (1000)        0 2024-05-23 14:19:01.944179 svd2json-0.1.5/.github/
-drwxrwxr-x   0 pthierry  (1000) pthierry  (1000)        0 2024-05-23 14:19:01.948179 svd2json-0.1.5/.github/workflows/
--rw-rw-r--   0 pthierry  (1000) pthierry  (1000)     1341 2024-05-23 14:12:47.000000 svd2json-0.1.5/.github/workflows/deploy.yml
--rw-rw-r--   0 pthierry  (1000) pthierry  (1000)     4434 2024-05-23 14:12:47.000000 svd2json-0.1.5/.github/workflows/main.yml
--rw-rw-r--   0 pthierry  (1000) pthierry  (1000)      153 2024-05-23 14:12:47.000000 svd2json-0.1.5/.gitignore
--rw-rw-r--   0 pthierry  (1000) pthierry  (1000)      233 2024-05-23 14:12:47.000000 svd2json-0.1.5/CODEOWNERS
-drwxrwxr-x   0 pthierry  (1000) pthierry  (1000)        0 2024-05-23 14:19:01.948179 svd2json-0.1.5/LICENSES/
--rw-rw-r--   0 pthierry  (1000) pthierry  (1000)    10174 2024-05-23 14:12:47.000000 svd2json-0.1.5/LICENSES/Apache-2.0.txt
--rw-r--r--   0 pthierry  (1000) pthierry  (1000)    16329 2024-05-23 14:19:01.952179 svd2json-0.1.5/PKG-INFO
--rw-rw-r--   0 pthierry  (1000) pthierry  (1000)     3035 2024-05-23 14:12:47.000000 svd2json-0.1.5/README.md
--rw-rw-r--   0 pthierry  (1000) pthierry  (1000)     1681 2024-05-23 14:12:47.000000 svd2json-0.1.5/pyproject.toml
--rw-rw-r--   0 pthierry  (1000) pthierry  (1000)       38 2024-05-23 14:19:01.952179 svd2json-0.1.5/setup.cfg
-drwxrwxr-x   0 pthierry  (1000) pthierry  (1000)        0 2024-05-23 14:19:01.944179 svd2json-0.1.5/src/
-drwxrwxr-x   0 pthierry  (1000) pthierry  (1000)        0 2024-05-23 14:19:01.948179 svd2json-0.1.5/src/svd2json/
--rw-rw-r--   0 pthierry  (1000) pthierry  (1000)      730 2024-05-23 14:12:47.000000 svd2json-0.1.5/src/svd2json/__init__.py
--rw-rw-r--   0 pthierry  (1000) pthierry  (1000)      162 2024-05-23 14:12:47.000000 svd2json-0.1.5/src/svd2json/__version__.py
--rw-rw-r--   0 pthierry  (1000) pthierry  (1000)      108 2024-05-23 14:12:47.000000 svd2json-0.1.5/src/svd2json/py.typed
--rw-rw-r--   0 pthierry  (1000) pthierry  (1000)     5013 2024-05-23 14:12:47.000000 svd2json-0.1.5/src/svd2json/svd2json.py
-drwxrwxr-x   0 pthierry  (1000) pthierry  (1000)        0 2024-05-23 14:19:01.948179 svd2json-0.1.5/src/svd2json.egg-info/
--rw-r--r--   0 pthierry  (1000) pthierry  (1000)    16329 2024-05-23 14:19:01.000000 svd2json-0.1.5/src/svd2json.egg-info/PKG-INFO
--rw-rw-r--   0 pthierry  (1000) pthierry  (1000)      475 2024-05-23 14:19:01.000000 svd2json-0.1.5/src/svd2json.egg-info/SOURCES.txt
--rw-rw-r--   0 pthierry  (1000) pthierry  (1000)        1 2024-05-23 14:19:01.000000 svd2json-0.1.5/src/svd2json.egg-info/dependency_links.txt
--rw-rw-r--   0 pthierry  (1000) pthierry  (1000)       42 2024-05-23 14:19:01.000000 svd2json-0.1.5/src/svd2json.egg-info/entry_points.txt
--rw-rw-r--   0 pthierry  (1000) pthierry  (1000)      238 2024-05-23 14:19:01.000000 svd2json-0.1.5/src/svd2json.egg-info/requires.txt
--rw-rw-r--   0 pthierry  (1000) pthierry  (1000)        9 2024-05-23 14:19:01.000000 svd2json-0.1.5/src/svd2json.egg-info/top_level.txt
-drwxrwxr-x   0 pthierry  (1000) pthierry  (1000)        0 2024-05-23 14:19:01.948179 svd2json-0.1.5/tests/
--rw-rw-r--   0 pthierry  (1000) pthierry  (1000)      246 2024-05-23 14:12:47.000000 svd2json-0.1.5/tests/test_svd2json.py
--rw-rw-r--   0 pthierry  (1000) pthierry  (1000)     1362 2024-05-23 14:12:47.000000 svd2json-0.1.5/tox.ini
+drwxrwxr-x   0 pthierry  (1000) pthierry  (1000)        0 2024-05-23 15:14:17.324061 svd2json-0.1.6/
+drwxrwxr-x   0 pthierry  (1000) pthierry  (1000)        0 2024-05-23 15:14:17.316061 svd2json-0.1.6/.github/
+drwxrwxr-x   0 pthierry  (1000) pthierry  (1000)        0 2024-05-23 15:14:17.320061 svd2json-0.1.6/.github/workflows/
+-rw-rw-r--   0 pthierry  (1000) pthierry  (1000)     1341 2024-05-23 14:12:47.000000 svd2json-0.1.6/.github/workflows/deploy.yml
+-rw-rw-r--   0 pthierry  (1000) pthierry  (1000)     4434 2024-05-23 14:12:47.000000 svd2json-0.1.6/.github/workflows/main.yml
+-rw-rw-r--   0 pthierry  (1000) pthierry  (1000)      153 2024-05-23 14:12:47.000000 svd2json-0.1.6/.gitignore
+-rw-rw-r--   0 pthierry  (1000) pthierry  (1000)      233 2024-05-23 14:12:47.000000 svd2json-0.1.6/CODEOWNERS
+drwxrwxr-x   0 pthierry  (1000) pthierry  (1000)        0 2024-05-23 15:14:17.320061 svd2json-0.1.6/LICENSES/
+-rw-rw-r--   0 pthierry  (1000) pthierry  (1000)    10174 2024-05-23 14:12:47.000000 svd2json-0.1.6/LICENSES/Apache-2.0.txt
+-rw-r--r--   0 pthierry  (1000) pthierry  (1000)    15986 2024-05-23 15:14:17.320061 svd2json-0.1.6/PKG-INFO
+-rw-rw-r--   0 pthierry  (1000) pthierry  (1000)     3035 2024-05-23 14:12:47.000000 svd2json-0.1.6/README.md
+-rw-rw-r--   0 pthierry  (1000) pthierry  (1000)     1362 2024-05-23 15:13:56.000000 svd2json-0.1.6/pyproject.toml
+-rw-rw-r--   0 pthierry  (1000) pthierry  (1000)       38 2024-05-23 15:14:17.324061 svd2json-0.1.6/setup.cfg
+drwxrwxr-x   0 pthierry  (1000) pthierry  (1000)        0 2024-05-23 15:14:17.316061 svd2json-0.1.6/src/
+drwxrwxr-x   0 pthierry  (1000) pthierry  (1000)        0 2024-05-23 15:14:17.320061 svd2json-0.1.6/src/svd2json/
+-rw-rw-r--   0 pthierry  (1000) pthierry  (1000)      730 2024-05-23 14:12:47.000000 svd2json-0.1.6/src/svd2json/__init__.py
+-rw-rw-r--   0 pthierry  (1000) pthierry  (1000)      162 2024-05-23 14:12:47.000000 svd2json-0.1.6/src/svd2json/__version__.py
+-rw-rw-r--   0 pthierry  (1000) pthierry  (1000)      108 2024-05-23 14:12:47.000000 svd2json-0.1.6/src/svd2json/py.typed
+-rw-rw-r--   0 pthierry  (1000) pthierry  (1000)     5013 2024-05-23 14:12:47.000000 svd2json-0.1.6/src/svd2json/svd2json.py
+drwxrwxr-x   0 pthierry  (1000) pthierry  (1000)        0 2024-05-23 15:14:17.320061 svd2json-0.1.6/src/svd2json.egg-info/
+-rw-r--r--   0 pthierry  (1000) pthierry  (1000)    15986 2024-05-23 15:14:17.000000 svd2json-0.1.6/src/svd2json.egg-info/PKG-INFO
+-rw-rw-r--   0 pthierry  (1000) pthierry  (1000)      475 2024-05-23 15:14:17.000000 svd2json-0.1.6/src/svd2json.egg-info/SOURCES.txt
+-rw-rw-r--   0 pthierry  (1000) pthierry  (1000)        1 2024-05-23 15:14:17.000000 svd2json-0.1.6/src/svd2json.egg-info/dependency_links.txt
+-rw-rw-r--   0 pthierry  (1000) pthierry  (1000)       42 2024-05-23 15:14:17.000000 svd2json-0.1.6/src/svd2json.egg-info/entry_points.txt
+-rw-rw-r--   0 pthierry  (1000) pthierry  (1000)      238 2024-05-23 15:14:17.000000 svd2json-0.1.6/src/svd2json.egg-info/requires.txt
+-rw-rw-r--   0 pthierry  (1000) pthierry  (1000)        9 2024-05-23 15:14:17.000000 svd2json-0.1.6/src/svd2json.egg-info/top_level.txt
+drwxrwxr-x   0 pthierry  (1000) pthierry  (1000)        0 2024-05-23 15:14:17.320061 svd2json-0.1.6/tests/
+-rw-rw-r--   0 pthierry  (1000) pthierry  (1000)      246 2024-05-23 14:12:47.000000 svd2json-0.1.6/tests/test_svd2json.py
+-rw-rw-r--   0 pthierry  (1000) pthierry  (1000)     1362 2024-05-23 14:12:47.000000 svd2json-0.1.6/tox.ini
```

### Comparing `svd2json-0.1.5/.github/workflows/deploy.yml` & `svd2json-0.1.6/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `svd2json-0.1.5/.github/workflows/main.yml` & `svd2json-0.1.6/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `svd2json-0.1.5/LICENSES/Apache-2.0.txt` & `svd2json-0.1.6/LICENSES/Apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `svd2json-0.1.5/PKG-INFO` & `svd2json-0.1.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: svd2json
-Version: 0.1.5
+Version: 0.1.6
 Summary: Convert SVD file to json
-Author-email: Ledger SA <firmware@ledger.fr>
+Author-email: Ledger SAS <firmware@ledger.fr>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
@@ -177,18 +177,14 @@
               of any other Contributor, and only if You agree to indemnify,
               defend, and hold each Contributor harmless for any liability
               incurred by, or claims asserted against, such Contributor by reason
               of your accepting any such warranty or additional liability.
         
            END OF TERMS AND CONDITIONS
         
-Project-URL: Homepage, https://git.orange.ledgerlabs.net/outpost/python-svd2json
-Project-URL: Documentation, https://pages.git.orange.ledgerlabs.net/outpost/outpostpedia/
-Project-URL: Repository, https://git.orange.ledgerlabs.net/outpost/python-svd2json.git
-Project-URL: Issues, https://git.orange.ledgerlabs.net/outpost/python-svd2json/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `svd2json-0.1.5/README.md` & `svd2json-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `svd2json-0.1.5/pyproject.toml` & `svd2json-0.1.6/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 [project]
 name = "svd2json"
 description = "Convert SVD file to json"
 dynamic = ["version"]
 requires-python = ">= 3.10"
 readme = "README.md"
 authors = [
-  {email = "Ledger SA <firmware@ledger.fr>"},
+  {email = "Ledger SAS <firmware@ledger.fr>"},
 ]
 license = {file = "LICENSES/Apache-2.0.txt"}
 dependencies = []
 classifiers = [
     "Development Status :: 4 - Beta",
 
     "Intended Audience :: Developers",
@@ -28,20 +28,14 @@
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
 ]
 
-[project.urls]
-Homepage = "https://git.orange.ledgerlabs.net/outpost/python-svd2json"
-Documentation = "https://pages.git.orange.ledgerlabs.net/outpost/outpostpedia/"
-Repository = "https://git.orange.ledgerlabs.net/outpost/python-svd2json.git"
-Issues = "https://git.orange.ledgerlabs.net/outpost/python-svd2json/issues"
-
 [project.scripts]
 svd2json = "svd2json:run"
 
 [project.optional-dependencies]
 devel = [
     "coverage>=0.4",
     "pytest>=4.6",
```

### Comparing `svd2json-0.1.5/src/svd2json/__init__.py` & `svd2json-0.1.6/src/svd2json/__init__.py`

 * *Files identical despite different names*

### Comparing `svd2json-0.1.5/src/svd2json/svd2json.py` & `svd2json-0.1.6/src/svd2json/svd2json.py`

 * *Files identical despite different names*

### Comparing `svd2json-0.1.5/src/svd2json.egg-info/PKG-INFO` & `svd2json-0.1.6/src/svd2json.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: svd2json
-Version: 0.1.5
+Version: 0.1.6
 Summary: Convert SVD file to json
-Author-email: Ledger SA <firmware@ledger.fr>
+Author-email: Ledger SAS <firmware@ledger.fr>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
@@ -177,18 +177,14 @@
               of any other Contributor, and only if You agree to indemnify,
               defend, and hold each Contributor harmless for any liability
               incurred by, or claims asserted against, such Contributor by reason
               of your accepting any such warranty or additional liability.
         
            END OF TERMS AND CONDITIONS
         
-Project-URL: Homepage, https://git.orange.ledgerlabs.net/outpost/python-svd2json
-Project-URL: Documentation, https://pages.git.orange.ledgerlabs.net/outpost/outpostpedia/
-Project-URL: Repository, https://git.orange.ledgerlabs.net/outpost/python-svd2json.git
-Project-URL: Issues, https://git.orange.ledgerlabs.net/outpost/python-svd2json/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `svd2json-0.1.5/tox.ini` & `svd2json-0.1.6/tox.ini`

 * *Files identical despite different names*

