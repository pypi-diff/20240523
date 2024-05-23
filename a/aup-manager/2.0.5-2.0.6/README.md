# Comparing `tmp/aup_manager-2.0.5.tar.gz` & `tmp/aup_manager-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aup_manager-2.0.5.tar", last modified: Mon Apr  8 08:30:18 2024, max compression
+gzip compressed data, was "aup_manager-2.0.6.tar", last modified: Thu May 23 13:22:10 2024, max compression
```

## Comparing `aup_manager-2.0.5.tar` & `aup_manager-2.0.6.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-08 08:30:18.662981 aup_manager-2.0.5/
--rw-rw-rw-   0     1001 root         (0)     1560 2024-04-08 08:29:51.000000 aup_manager-2.0.5/LICENSE
--rw-rw-rw-   0     1001 root         (0)       52 2024-04-08 08:29:51.000000 aup_manager-2.0.5/MANIFEST.in
--rw-r--r--   0     1001 root         (0)      568 2024-04-08 08:30:18.662981 aup_manager-2.0.5/PKG-INFO
--rw-rw-rw-   0     1001 root         (0)      507 2024-04-08 08:29:51.000000 aup_manager-2.0.5/README.md
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-08 08:30:18.654981 aup_manager-2.0.5/aup_manager/
--rw-rw-rw-   0     1001 root         (0)      434 2024-04-08 08:29:51.000000 aup_manager-2.0.5/aup_manager/__init__.py
--rw-rw-rw-   0     1001 root         (0)     1479 2024-04-08 08:29:51.000000 aup_manager-2.0.5/aup_manager/config-template.yaml
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-08 08:30:18.658981 aup_manager-2.0.5/aup_manager/connectors/
--rw-rw-rw-   0     1001 root         (0)     1577 2024-04-08 08:29:51.000000 aup_manager-2.0.5/aup_manager/connectors/ConnectorInterface.py
--rw-rw-rw-   0     1001 root         (0)     1785 2024-04-08 08:29:51.000000 aup_manager-2.0.5/aup_manager/connectors/MongodbConnector.py
--rw-rw-rw-   0     1001 root         (0)     4490 2024-04-08 08:29:51.000000 aup_manager-2.0.5/aup_manager/connectors/PerunConnector.py
--rw-rw-rw-   0     1001 root         (0)      279 2024-04-08 08:29:51.000000 aup_manager-2.0.5/aup_manager/connectors/__init__.py
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-08 08:30:18.658981 aup_manager-2.0.5/aup_manager/db/
--rw-rw-rw-   0     1001 root         (0)     7305 2024-04-08 08:29:51.000000 aup_manager-2.0.5/aup_manager/db/DatabaseInterface.py
--rw-rw-rw-   0     1001 root         (0)    11887 2024-04-08 08:29:51.000000 aup_manager-2.0.5/aup_manager/db/MongodbDatabase.py
--rw-rw-rw-   0     1001 root         (0)      174 2024-04-08 08:29:51.000000 aup_manager-2.0.5/aup_manager/db/__init__.py
--rw-rw-rw-   0     1001 root         (0)    15944 2024-04-08 08:29:51.000000 aup_manager-2.0.5/aup_manager/flask_app.py
--rw-rw-rw-   0     1001 root         (0)     2937 2024-04-08 08:29:51.000000 aup_manager-2.0.5/aup_manager/models.py
--rw-rw-rw-   0     1001 root         (0)     4026 2024-04-08 08:29:51.000000 aup_manager-2.0.5/aup_manager/openapi-specification.yaml
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-08 08:30:18.658981 aup_manager-2.0.5/aup_manager/static/
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-08 08:30:18.658981 aup_manager-2.0.5/aup_manager/static/assets/
--rw-rw-rw-   0     1001 root         (0)      405 2024-04-08 08:29:51.000000 aup_manager-2.0.5/aup_manager/static/assets/caret-down-solid.svg
--rw-rw-rw-   0     1001 root         (0)    26084 2024-04-08 08:29:51.000000 aup_manager-2.0.5/aup_manager/static/index.js
--rw-rw-rw-   0     1001 root         (0)    21684 2024-04-08 08:29:51.000000 aup_manager-2.0.5/aup_manager/static/package-lock.json
--rw-rw-rw-   0     1001 root         (0)      498 2024-04-08 08:29:51.000000 aup_manager-2.0.5/aup_manager/static/package.json
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-08 08:30:18.658981 aup_manager-2.0.5/aup_manager/static/scss/
--rw-rw-rw-   0     1001 root         (0)      166 2024-04-08 08:29:51.000000 aup_manager-2.0.5/aup_manager/static/scss/_stepper.scss
--rw-rw-rw-   0     1001 root         (0)      318 2024-04-08 08:29:51.000000 aup_manager-2.0.5/aup_manager/static/scss/custom.scss
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-08 08:30:18.658981 aup_manager-2.0.5/aup_manager/templates/
--rw-rw-rw-   0     1001 root         (0)     2273 2024-04-08 08:29:51.000000 aup_manager-2.0.5/aup_manager/templates/accept_aups.html
--rw-rw-rw-   0     1001 root         (0)      823 2024-04-08 08:29:51.000000 aup_manager-2.0.5/aup_manager/templates/aup_overview.html
--rw-rw-rw-   0     1001 root         (0)      988 2024-04-08 08:29:51.000000 aup_manager-2.0.5/aup_manager/templates/base.html
--rw-rw-rw-   0     1001 root         (0)     5633 2024-04-08 08:29:51.000000 aup_manager-2.0.5/aup_manager/templates/create_aup.html
--rw-rw-rw-   0     1001 root         (0)      428 2024-04-08 08:29:51.000000 aup_manager-2.0.5/aup_manager/templates/login.html
--rw-rw-rw-   0     1001 root         (0)    11233 2024-04-08 08:29:51.000000 aup_manager-2.0.5/aup_manager/templates/manage_aups.html
--rw-rw-rw-   0     1001 root         (0)      224 2024-04-08 08:29:51.000000 aup_manager-2.0.5/aup_manager/templates/text_message.html
--rw-rw-rw-   0     1001 root         (0)      535 2024-04-08 08:29:51.000000 aup_manager-2.0.5/aup_manager/templates/unauthorized.html
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-08 08:30:18.658981 aup_manager-2.0.5/aup_manager.egg-info/
--rw-r--r--   0     1001 root         (0)      568 2024-04-08 08:30:18.000000 aup_manager-2.0.5/aup_manager.egg-info/PKG-INFO
--rw-r--r--   0     1001 root         (0)     1145 2024-04-08 08:30:18.000000 aup_manager-2.0.5/aup_manager.egg-info/SOURCES.txt
--rw-r--r--   0     1001 root         (0)        1 2024-04-08 08:30:18.000000 aup_manager-2.0.5/aup_manager.egg-info/dependency_links.txt
--rw-r--r--   0     1001 root         (0)      159 2024-04-08 08:30:18.000000 aup_manager-2.0.5/aup_manager.egg-info/requires.txt
--rw-r--r--   0     1001 root         (0)       12 2024-04-08 08:30:18.000000 aup_manager-2.0.5/aup_manager.egg-info/top_level.txt
--rw-rw-rw-   0     1001 root         (0)       90 2024-04-08 08:30:18.662981 aup_manager-2.0.5/setup.cfg
--rw-rw-rw-   0     1001 root         (0)     1127 2024-04-08 08:29:51.000000 aup_manager-2.0.5/setup.py
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-23 13:22:10.299569 aup_manager-2.0.6/
+-rw-rw-rw-   0     1001 root         (0)     1560 2024-05-23 13:21:30.000000 aup_manager-2.0.6/LICENSE
+-rw-rw-rw-   0     1001 root         (0)       52 2024-05-23 13:21:30.000000 aup_manager-2.0.6/MANIFEST.in
+-rw-r--r--   0     1001 root         (0)      568 2024-05-23 13:22:10.299569 aup_manager-2.0.6/PKG-INFO
+-rw-rw-rw-   0     1001 root         (0)      507 2024-05-23 13:21:30.000000 aup_manager-2.0.6/README.md
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-23 13:22:10.291568 aup_manager-2.0.6/aup_manager/
+-rw-rw-rw-   0     1001 root         (0)      434 2024-05-23 13:21:30.000000 aup_manager-2.0.6/aup_manager/__init__.py
+-rw-rw-rw-   0     1001 root         (0)     1479 2024-05-23 13:21:30.000000 aup_manager-2.0.6/aup_manager/config-template.yaml
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-23 13:22:10.295569 aup_manager-2.0.6/aup_manager/connectors/
+-rw-rw-rw-   0     1001 root         (0)     1577 2024-05-23 13:21:30.000000 aup_manager-2.0.6/aup_manager/connectors/ConnectorInterface.py
+-rw-rw-rw-   0     1001 root         (0)     1785 2024-05-23 13:21:30.000000 aup_manager-2.0.6/aup_manager/connectors/MongodbConnector.py
+-rw-rw-rw-   0     1001 root         (0)     4490 2024-05-23 13:21:30.000000 aup_manager-2.0.6/aup_manager/connectors/PerunConnector.py
+-rw-rw-rw-   0     1001 root         (0)      279 2024-05-23 13:21:30.000000 aup_manager-2.0.6/aup_manager/connectors/__init__.py
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-23 13:22:10.295569 aup_manager-2.0.6/aup_manager/db/
+-rw-rw-rw-   0     1001 root         (0)     7305 2024-05-23 13:21:30.000000 aup_manager-2.0.6/aup_manager/db/DatabaseInterface.py
+-rw-rw-rw-   0     1001 root         (0)    11887 2024-05-23 13:21:30.000000 aup_manager-2.0.6/aup_manager/db/MongodbDatabase.py
+-rw-rw-rw-   0     1001 root         (0)      174 2024-05-23 13:21:30.000000 aup_manager-2.0.6/aup_manager/db/__init__.py
+-rw-rw-rw-   0     1001 root         (0)    15944 2024-05-23 13:21:30.000000 aup_manager-2.0.6/aup_manager/flask_app.py
+-rw-rw-rw-   0     1001 root         (0)     2937 2024-05-23 13:21:30.000000 aup_manager-2.0.6/aup_manager/models.py
+-rw-rw-rw-   0     1001 root         (0)     4026 2024-05-23 13:21:30.000000 aup_manager-2.0.6/aup_manager/openapi-specification.yaml
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-23 13:22:10.299569 aup_manager-2.0.6/aup_manager/static/
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-23 13:22:10.299569 aup_manager-2.0.6/aup_manager/static/assets/
+-rw-rw-rw-   0     1001 root         (0)      405 2024-05-23 13:21:30.000000 aup_manager-2.0.6/aup_manager/static/assets/caret-down-solid.svg
+-rw-rw-rw-   0     1001 root         (0)    26084 2024-05-23 13:21:30.000000 aup_manager-2.0.6/aup_manager/static/index.js
+-rw-rw-rw-   0     1001 root         (0)    21770 2024-05-23 13:21:30.000000 aup_manager-2.0.6/aup_manager/static/package-lock.json
+-rw-rw-rw-   0     1001 root         (0)      498 2024-05-23 13:21:30.000000 aup_manager-2.0.6/aup_manager/static/package.json
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-23 13:22:10.299569 aup_manager-2.0.6/aup_manager/static/scss/
+-rw-rw-rw-   0     1001 root         (0)      166 2024-05-23 13:21:30.000000 aup_manager-2.0.6/aup_manager/static/scss/_stepper.scss
+-rw-rw-rw-   0     1001 root         (0)      318 2024-05-23 13:21:30.000000 aup_manager-2.0.6/aup_manager/static/scss/custom.scss
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-23 13:22:10.299569 aup_manager-2.0.6/aup_manager/templates/
+-rw-rw-rw-   0     1001 root         (0)     2273 2024-05-23 13:21:30.000000 aup_manager-2.0.6/aup_manager/templates/accept_aups.html
+-rw-rw-rw-   0     1001 root         (0)      823 2024-05-23 13:21:30.000000 aup_manager-2.0.6/aup_manager/templates/aup_overview.html
+-rw-rw-rw-   0     1001 root         (0)      988 2024-05-23 13:21:30.000000 aup_manager-2.0.6/aup_manager/templates/base.html
+-rw-rw-rw-   0     1001 root         (0)     5633 2024-05-23 13:21:30.000000 aup_manager-2.0.6/aup_manager/templates/create_aup.html
+-rw-rw-rw-   0     1001 root         (0)      428 2024-05-23 13:21:30.000000 aup_manager-2.0.6/aup_manager/templates/login.html
+-rw-rw-rw-   0     1001 root         (0)    11233 2024-05-23 13:21:30.000000 aup_manager-2.0.6/aup_manager/templates/manage_aups.html
+-rw-rw-rw-   0     1001 root         (0)      224 2024-05-23 13:21:30.000000 aup_manager-2.0.6/aup_manager/templates/text_message.html
+-rw-rw-rw-   0     1001 root         (0)      535 2024-05-23 13:21:30.000000 aup_manager-2.0.6/aup_manager/templates/unauthorized.html
+drwxr-xr-x   0     1001 root         (0)        0 2024-05-23 13:22:10.291568 aup_manager-2.0.6/aup_manager.egg-info/
+-rw-r--r--   0     1001 root         (0)      568 2024-05-23 13:22:10.000000 aup_manager-2.0.6/aup_manager.egg-info/PKG-INFO
+-rw-r--r--   0     1001 root         (0)     1145 2024-05-23 13:22:10.000000 aup_manager-2.0.6/aup_manager.egg-info/SOURCES.txt
+-rw-r--r--   0     1001 root         (0)        1 2024-05-23 13:22:10.000000 aup_manager-2.0.6/aup_manager.egg-info/dependency_links.txt
+-rw-r--r--   0     1001 root         (0)      159 2024-05-23 13:22:10.000000 aup_manager-2.0.6/aup_manager.egg-info/requires.txt
+-rw-r--r--   0     1001 root         (0)       12 2024-05-23 13:22:10.000000 aup_manager-2.0.6/aup_manager.egg-info/top_level.txt
+-rw-rw-rw-   0     1001 root         (0)       90 2024-05-23 13:22:10.303569 aup_manager-2.0.6/setup.cfg
+-rw-rw-rw-   0     1001 root         (0)     1127 2024-05-23 13:21:30.000000 aup_manager-2.0.6/setup.py
```

### Comparing `aup_manager-2.0.5/LICENSE` & `aup_manager-2.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `aup_manager-2.0.5/PKG-INFO` & `aup_manager-2.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: aup_manager
-Version: 2.0.5
+Version: 2.0.6
 Summary: app for management of acceptable use policies with API for approving them
 Home-page: https://gitlab.ics.muni.cz/perun/perun-proxyidp/aup-manager.git
 Requires-Python: >=3.9
 License-File: LICENSE
 Requires-Dist: setuptools
 Requires-Dist: pymongo==4.6.1
 Requires-Dist: jsonpatch==1.33
 Requires-Dist: connexion[swagger-ui]==2.14.2
-Requires-Dist: markdown2==2.4.12
+Requires-Dist: markdown2==2.4.13
 Requires-Dist: Flask-pyoidc==3.14.3
-Requires-Dist: jwcrypto==1.5.1
+Requires-Dist: jwcrypto==1.5.6
 Provides-Extra: perun
 Requires-Dist: perun.connector==3.8.1; extra == "perun"
```

### Comparing `aup_manager-2.0.5/aup_manager/config-template.yaml` & `aup_manager-2.0.6/aup_manager/config-template.yaml`

 * *Files identical despite different names*

### Comparing `aup_manager-2.0.5/aup_manager/connectors/ConnectorInterface.py` & `aup_manager-2.0.6/aup_manager/connectors/ConnectorInterface.py`

 * *Files identical despite different names*

### Comparing `aup_manager-2.0.5/aup_manager/connectors/MongodbConnector.py` & `aup_manager-2.0.6/aup_manager/connectors/MongodbConnector.py`

 * *Files identical despite different names*

### Comparing `aup_manager-2.0.5/aup_manager/connectors/PerunConnector.py` & `aup_manager-2.0.6/aup_manager/connectors/PerunConnector.py`

 * *Files identical despite different names*

### Comparing `aup_manager-2.0.5/aup_manager/db/DatabaseInterface.py` & `aup_manager-2.0.6/aup_manager/db/DatabaseInterface.py`

 * *Files identical despite different names*

### Comparing `aup_manager-2.0.5/aup_manager/db/MongodbDatabase.py` & `aup_manager-2.0.6/aup_manager/db/MongodbDatabase.py`

 * *Files identical despite different names*

### Comparing `aup_manager-2.0.5/aup_manager/flask_app.py` & `aup_manager-2.0.6/aup_manager/flask_app.py`

 * *Files identical despite different names*

### Comparing `aup_manager-2.0.5/aup_manager/models.py` & `aup_manager-2.0.6/aup_manager/models.py`

 * *Files identical despite different names*

### Comparing `aup_manager-2.0.5/aup_manager/openapi-specification.yaml` & `aup_manager-2.0.6/aup_manager/openapi-specification.yaml`

 * *Files identical despite different names*

### Comparing `aup_manager-2.0.5/aup_manager/static/index.js` & `aup_manager-2.0.6/aup_manager/static/index.js`

 * *Files identical despite different names*

### Comparing `aup_manager-2.0.5/aup_manager/static/package-lock.json` & `aup_manager-2.0.6/aup_manager/static/package-lock.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9958606049562683%*

 * *Differences: {"'packages'": "{'': {'dependencies': {'@fortawesome/fontawesome-free': '6.5.2', 'autoprefixer': "*

 * *               "'10.4.19'}}, 'node_modules/@fortawesome/fontawesome-free': {'version': '6.5.2', "*

 * *               "'resolved': "*

 * *               "'https://registry.npmjs.org/@fortawesome/fontawesome-free/-/fontawesome-free-6.5.2.tgz', "*

 * *               "'integrity': "*

 * *               "'sha512-hRILoInAx8GNT5IMkrtIt9blOdrqHOnPBH+k70aWUAqPZPgopb9G5EQJFpaBx/S8zp2fC+mPW349Bziuk1o28Q=='}, "*

 * *               "'node_modules […]*

```diff
@@ -1,16 +1,16 @@
 {
     "lockfileVersion": 3,
     "name": "aup-manager",
     "packages": {
         "": {
             "dependencies": {
-                "@fortawesome/fontawesome-free": "6.5.1",
+                "@fortawesome/fontawesome-free": "6.5.2",
                 "@toast-ui/editor": "3.2.2",
-                "autoprefixer": "10.4.17",
+                "autoprefixer": "10.4.19",
                 "bootstrap": "5.3.2",
                 "jquery": "3.7.1"
             },
             "devDependencies": {
                 "sass": "1.64.2"
             },
             "license": "BSD-3-Clause",
@@ -18,17 +18,17 @@
             "version": "1.0.0"
         },
         "node_modules/@fortawesome/fontawesome-free": {
             "engines": {
                 "node": ">=6"
             },
             "hasInstallScript": true,
-            "integrity": "sha512-CNy5vSwN3fsUStPRLX7fUYojyuzoEMSXPl7zSLJ8TgtRfjv24LOnOWKT2zYwaHZCJGkdyRnTmstR0P+Ah503Gw==",
-            "resolved": "https://registry.npmjs.org/@fortawesome/fontawesome-free/-/fontawesome-free-6.5.1.tgz",
-            "version": "6.5.1"
+            "integrity": "sha512-hRILoInAx8GNT5IMkrtIt9blOdrqHOnPBH+k70aWUAqPZPgopb9G5EQJFpaBx/S8zp2fC+mPW349Bziuk1o28Q==",
+            "resolved": "https://registry.npmjs.org/@fortawesome/fontawesome-free/-/fontawesome-free-6.5.2.tgz",
+            "version": "6.5.2"
         },
         "node_modules/@popperjs/core": {
             "funding": {
                 "type": "opencollective",
                 "url": "https://opencollective.com/popperjs"
             },
             "integrity": "sha512-P1st0aksCrn9sGZhp8GMYwBnQsbvAWsZAX44oXNNvLHGqAOcoVxmjZiohstwQ7SqKnbR47akdNi+uleWD8+g6A==",
@@ -65,16 +65,16 @@
             "version": "3.1.3"
         },
         "node_modules/autoprefixer": {
             "bin": {
                 "autoprefixer": "bin/autoprefixer"
             },
             "dependencies": {
-                "browserslist": "^4.22.2",
-                "caniuse-lite": "^1.0.30001578",
+                "browserslist": "^4.23.0",
+                "caniuse-lite": "^1.0.30001599",
                 "fraction.js": "^4.3.7",
                 "normalize-range": "^0.1.2",
                 "picocolors": "^1.0.0",
                 "postcss-value-parser": "^4.2.0"
             },
             "engines": {
                 "node": "^10 || ^12 || >=14"
@@ -89,29 +89,32 @@
                     "url": "https://tidelift.com/funding/github/npm/autoprefixer"
                 },
                 {
                     "type": "github",
                     "url": "https://github.com/sponsors/ai"
                 }
             ],
-            "integrity": "sha512-/cpVNRLSfhOtcGflT13P2794gVSgmPgTR+erw5ifnMLZb0UnSlkK4tquLmkd3BhA+nLo5tX8Cu0upUsGKvKbmg==",
+            "integrity": "sha512-BaENR2+zBZ8xXhM4pUaKUxlVdxZ0EZhjvbopwnXmxRUfqDmwSpC2lAi/QXvx7NRdPCo1WKEcEF6mV64si1z4Ew==",
             "peerDependencies": {
                 "postcss": "^8.1.0"
             },
-            "resolved": "https://registry.npmjs.org/autoprefixer/-/autoprefixer-10.4.17.tgz",
-            "version": "10.4.17"
+            "resolved": "https://registry.npmjs.org/autoprefixer/-/autoprefixer-10.4.19.tgz",
+            "version": "10.4.19"
         },
         "node_modules/binary-extensions": {
             "dev": true,
             "engines": {
                 "node": ">=8"
             },
-            "integrity": "sha512-jDctJ/IVQbZoJykoeHbhXpOlNBqGNcwXJKJog42E5HDPUwQTSdjCHdihjj0DlnheQ7blbT6dHOafNAiS8ooQKA==",
-            "resolved": "https://registry.npmjs.org/binary-extensions/-/binary-extensions-2.2.0.tgz",
-            "version": "2.2.0"
+            "funding": {
+                "url": "https://github.com/sponsors/sindresorhus"
+            },
+            "integrity": "sha512-Ceh+7ox5qe7LJuLHoY0feh3pHuUDHAcRUeyL2VYghZwfpkNIy/+8Ocg0a3UuSoYzavmylwuLWQOf3hl0jjMMIw==",
+            "resolved": "https://registry.npmjs.org/binary-extensions/-/binary-extensions-2.3.0.tgz",
+            "version": "2.3.0"
         },
         "node_modules/bootstrap": {
             "funding": [
                 {
                     "type": "github",
                     "url": "https://github.com/sponsors/twbs"
                 },
@@ -181,17 +184,17 @@
                     "url": "https://tidelift.com/funding/github/npm/caniuse-lite"
                 },
                 {
                     "type": "github",
                     "url": "https://github.com/sponsors/ai"
                 }
             ],
-            "integrity": "sha512-PCzRMei/vXjJyL5mJtzNiUCKP59dm8Apqc3PH8gJkMnMXZGox93RbE76jHsmLwmIo6/3nsYIpJtx0O7u5PqFuQ==",
-            "resolved": "https://registry.npmjs.org/caniuse-lite/-/caniuse-lite-1.0.30001591.tgz",
-            "version": "1.0.30001591"
+            "integrity": "sha512-jmZQ1VpmlRwHgdP1/uiKzgiAuGOfLEJsYFP4+GBou/QQ4U6IOJCB4NP1c+1p9RGLpwObcT94jA5/uO+F1vBbog==",
+            "resolved": "https://registry.npmjs.org/caniuse-lite/-/caniuse-lite-1.0.30001614.tgz",
+            "version": "1.0.30001614"
         },
         "node_modules/chokidar": {
             "dependencies": {
                 "anymatch": "~3.1.2",
                 "braces": "~3.0.2",
                 "glob-parent": "~5.1.2",
                 "is-binary-path": "~2.1.0",
@@ -210,22 +213,22 @@
             "optionalDependencies": {
                 "fsevents": "~2.3.2"
             },
             "resolved": "https://registry.npmjs.org/chokidar/-/chokidar-3.6.0.tgz",
             "version": "3.6.0"
         },
         "node_modules/dompurify": {
-            "integrity": "sha512-kxxKlPEDa6Nc5WJi+qRgPbOAbgTpSULL+vI3NUXsZMlkJxTqYI9wg5ZTay2sFrdZRWHPWNi+EdAhcJf81WtoMQ==",
-            "resolved": "https://registry.npmjs.org/dompurify/-/dompurify-2.4.7.tgz",
-            "version": "2.4.7"
+            "integrity": "sha512-5vSyvxRAb45EoWwAktUT3AYqAwXK4FL7si22Cgj46U6ICsj/YJczCN+Bk7WNABIQmpWRymGfslMhrRUZkQNnqA==",
+            "resolved": "https://registry.npmjs.org/dompurify/-/dompurify-2.5.2.tgz",
+            "version": "2.5.2"
         },
         "node_modules/electron-to-chromium": {
-            "integrity": "sha512-GatzRKnGPS1go29ep25reM94xxd1Wj8ritU0yRhCJ/tr1Bg8gKnm6R9O/yPOhGQBoLMZ9ezfrpghNaTw97C/PQ==",
-            "resolved": "https://registry.npmjs.org/electron-to-chromium/-/electron-to-chromium-1.4.689.tgz",
-            "version": "1.4.689"
+            "integrity": "sha512-P3QJreYI/AUTcfBVrC4zy9KvnZWekViThgQMX/VpJ+IsOBbcX5JFpORM4qWapwWQ+agb2nYAOyn/4PMXOk0m2Q==",
+            "resolved": "https://registry.npmjs.org/electron-to-chromium/-/electron-to-chromium-1.4.752.tgz",
+            "version": "1.4.752"
         },
         "node_modules/escalade": {
             "engines": {
                 "node": ">=6"
             },
             "integrity": "sha512-ErCHMCae19vR8vQGe50xIsVomy19rg6gFu3+r3jkEO46suLMWBksvVyoGgQV+jOfl84ZSOSlmv6Gxa89PmTGmA==",
             "resolved": "https://registry.npmjs.org/escalade/-/escalade-3.1.2.tgz",
@@ -396,15 +399,15 @@
             "resolved": "https://registry.npmjs.org/picomatch/-/picomatch-2.3.1.tgz",
             "version": "2.3.1"
         },
         "node_modules/postcss": {
             "dependencies": {
                 "nanoid": "^3.3.7",
                 "picocolors": "^1.0.0",
-                "source-map-js": "^1.0.2"
+                "source-map-js": "^1.2.0"
             },
             "engines": {
                 "node": "^10 || ^12 || >=14"
             },
             "funding": [
                 {
                     "type": "opencollective",
@@ -415,18 +418,18 @@
                     "url": "https://tidelift.com/funding/github/npm/postcss"
                 },
                 {
                     "type": "github",
                     "url": "https://github.com/sponsors/ai"
                 }
             ],
-            "integrity": "sha512-u5U8qYpBCpN13BsiEB0CbR1Hhh4Gc0zLFuedrHJKMctHCHAGrMdG0PRM/KErzAL3CU6/eckEtmHNB3x6e3c0vA==",
+            "integrity": "sha512-Wglpdk03BSfXkHoQa3b/oulrotAkwrlLDRSOb9D0bN86FdRyE9lppSp33aHNPgBa0JKCoB+drFLZkQoRRYae5A==",
             "peer": true,
-            "resolved": "https://registry.npmjs.org/postcss/-/postcss-8.4.35.tgz",
-            "version": "8.4.35"
+            "resolved": "https://registry.npmjs.org/postcss/-/postcss-8.4.38.tgz",
+            "version": "8.4.38"
         },
         "node_modules/postcss-value-parser": {
             "integrity": "sha512-1NNCs6uurfkVbeXG4S8JFT9t19m45ICnif8zWLd5oPSZ50QnwMfK+H3jv408d4jw/7Bttv5axS5IiHoLaVNHeQ==",
             "resolved": "https://registry.npmjs.org/postcss-value-parser/-/postcss-value-parser-4.2.0.tgz",
             "version": "4.2.0"
         },
         "node_modules/prosemirror-commands": {
@@ -442,17 +445,17 @@
         "node_modules/prosemirror-history": {
             "dependencies": {
                 "prosemirror-state": "^1.2.2",
                 "prosemirror-transform": "^1.0.0",
                 "prosemirror-view": "^1.31.0",
                 "rope-sequence": "^1.3.0"
             },
-            "integrity": "sha512-/zm0XoU/N/+u7i5zepjmZAEnpvjDtzoPWW6VmKptcAnPadN/SStsBjMImdCEbb3seiNTpveziPTIrXQbHLtU1g==",
-            "resolved": "https://registry.npmjs.org/prosemirror-history/-/prosemirror-history-1.3.2.tgz",
-            "version": "1.3.2"
+            "integrity": "sha512-UUiGzDVcqo1lovOPdi9YxxUps3oBFWAIYkXLu3Ot+JPv1qzVogRbcizxK3LhHmtaUxclohgiOVesRw5QSlMnbQ==",
+            "resolved": "https://registry.npmjs.org/prosemirror-history/-/prosemirror-history-1.4.0.tgz",
+            "version": "1.4.0"
         },
         "node_modules/prosemirror-inputrules": {
             "dependencies": {
                 "prosemirror-state": "^1.0.0",
                 "prosemirror-transform": "^1.0.0"
             },
             "integrity": "sha512-6ygpPRuTJ2lcOXs9JkefieMst63wVJBgHZGl5QOytN7oSZs3Co/BYbc3Yx9zm9H37Bxw8kVzCnDsihsVsL4yEg==",
@@ -468,17 +471,17 @@
             "resolved": "https://registry.npmjs.org/prosemirror-keymap/-/prosemirror-keymap-1.2.2.tgz",
             "version": "1.2.2"
         },
         "node_modules/prosemirror-model": {
             "dependencies": {
                 "orderedmap": "^2.0.0"
             },
-            "integrity": "sha512-RPmVXxUfOhyFdayHawjuZCxiROsm9L4FCUA6pWI+l7n2yCBsWy9VpdE1hpDHUS8Vad661YLY9AzqfjLhAKQ4iQ==",
-            "resolved": "https://registry.npmjs.org/prosemirror-model/-/prosemirror-model-1.19.4.tgz",
-            "version": "1.19.4"
+            "integrity": "sha512-q7AY7vMjKYqDCeoedgUiAgrLabliXxndJuuFmcmc2+YU1SblvnOiG2WEACF2lwAZsMlfLpiAilA3L+TWlDqIsQ==",
+            "resolved": "https://registry.npmjs.org/prosemirror-model/-/prosemirror-model-1.20.0.tgz",
+            "version": "1.20.0"
         },
         "node_modules/prosemirror-state": {
             "dependencies": {
                 "prosemirror-model": "^1.0.0",
                 "prosemirror-transform": "^1.0.0",
                 "prosemirror-view": "^1.27.0"
             },
@@ -492,21 +495,21 @@
             },
             "integrity": "sha512-BaSBsIMv52F1BVVMvOmp1yzD3u65uC3HTzCBQV1WDPqJRQ2LuHKcyfn0jwqodo8sR9vVzMzZyI+Dal5W9E6a9A==",
             "resolved": "https://registry.npmjs.org/prosemirror-transform/-/prosemirror-transform-1.8.0.tgz",
             "version": "1.8.0"
         },
         "node_modules/prosemirror-view": {
             "dependencies": {
-                "prosemirror-model": "^1.16.0",
+                "prosemirror-model": "^1.20.0",
                 "prosemirror-state": "^1.0.0",
                 "prosemirror-transform": "^1.1.0"
             },
-            "integrity": "sha512-62qkYgSJIkwIMMCpuGuPzc52DiK1Iod6TWoIMxP4ja6BTD4yO8kCUL64PZ/WhH/dJ9fW0CDO39FhH1EMyhUFEg==",
-            "resolved": "https://registry.npmjs.org/prosemirror-view/-/prosemirror-view-1.33.1.tgz",
-            "version": "1.33.1"
+            "integrity": "sha512-zRLUNgLIQfd8IfGprsXxWTjdA8xEAFJe8cDNrOptj6Mop9sj+BMeVbJvceyAYCm5G2dOdT2prctH7K9dfnpIMw==",
+            "resolved": "https://registry.npmjs.org/prosemirror-view/-/prosemirror-view-1.33.6.tgz",
+            "version": "1.33.6"
         },
         "node_modules/readdirp": {
             "dependencies": {
                 "picomatch": "^2.2.1"
             },
             "dev": true,
             "engines": {
@@ -538,17 +541,17 @@
             "resolved": "https://registry.npmjs.org/sass/-/sass-1.64.2.tgz",
             "version": "1.64.2"
         },
         "node_modules/source-map-js": {
             "engines": {
                 "node": ">=0.10.0"
             },
-            "integrity": "sha512-R0XvVJ9WusLiqTCEiGCmICCMplcCkIwwR11mOSD9CR5u+IXYdiseeEuXCVAjS54zqwkLcPNnmU4OeJ6tUrWhDw==",
-            "resolved": "https://registry.npmjs.org/source-map-js/-/source-map-js-1.0.2.tgz",
-            "version": "1.0.2"
+            "integrity": "sha512-itJW8lvSA0TXEphiRoawsCksnlf8SyvmFzIhltqAHluXd88pkCd+cXJVHTDwdCr0IzwptSm035IHQktUu1QUMg==",
+            "resolved": "https://registry.npmjs.org/source-map-js/-/source-map-js-1.2.0.tgz",
+            "version": "1.2.0"
         },
         "node_modules/to-regex-range": {
             "dependencies": {
                 "is-number": "^7.0.0"
             },
             "dev": true,
             "engines": {
```

### Comparing `aup_manager-2.0.5/aup_manager/templates/accept_aups.html` & `aup_manager-2.0.6/aup_manager/templates/accept_aups.html`

 * *Files identical despite different names*

### Comparing `aup_manager-2.0.5/aup_manager/templates/aup_overview.html` & `aup_manager-2.0.6/aup_manager/templates/aup_overview.html`

 * *Files identical despite different names*

### Comparing `aup_manager-2.0.5/aup_manager/templates/base.html` & `aup_manager-2.0.6/aup_manager/templates/base.html`

 * *Files identical despite different names*

### Comparing `aup_manager-2.0.5/aup_manager/templates/create_aup.html` & `aup_manager-2.0.6/aup_manager/templates/create_aup.html`

 * *Files identical despite different names*

### Comparing `aup_manager-2.0.5/aup_manager/templates/manage_aups.html` & `aup_manager-2.0.6/aup_manager/templates/manage_aups.html`

 * *Files identical despite different names*

### Comparing `aup_manager-2.0.5/aup_manager/templates/unauthorized.html` & `aup_manager-2.0.6/aup_manager/templates/unauthorized.html`

 * *Files identical despite different names*

### Comparing `aup_manager-2.0.5/aup_manager.egg-info/PKG-INFO` & `aup_manager-2.0.6/aup_manager.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: aup-manager
-Version: 2.0.5
+Version: 2.0.6
 Summary: app for management of acceptable use policies with API for approving them
 Home-page: https://gitlab.ics.muni.cz/perun/perun-proxyidp/aup-manager.git
 Requires-Python: >=3.9
 License-File: LICENSE
 Requires-Dist: setuptools
 Requires-Dist: pymongo==4.6.1
 Requires-Dist: jsonpatch==1.33
 Requires-Dist: connexion[swagger-ui]==2.14.2
-Requires-Dist: markdown2==2.4.12
+Requires-Dist: markdown2==2.4.13
 Requires-Dist: Flask-pyoidc==3.14.3
-Requires-Dist: jwcrypto==1.5.1
+Requires-Dist: jwcrypto==1.5.6
 Provides-Extra: perun
 Requires-Dist: perun.connector==3.8.1; extra == "perun"
```

### Comparing `aup_manager-2.0.5/aup_manager.egg-info/SOURCES.txt` & `aup_manager-2.0.6/aup_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aup_manager-2.0.5/setup.py` & `aup_manager-2.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,17 +22,17 @@
     package_data={"": ["openapi-specification.yaml"]},
     packages=setuptools.find_packages(),
     install_requires=[
         "setuptools",
         "pymongo==4.6.1",  # for compatibility with proxyidp-gui
         "jsonpatch==1.33",
         "connexion[swagger-ui]==2.14.2",
-        "markdown2==2.4.12",
+        "markdown2==2.4.13",
         "Flask-pyoidc==3.14.3",
-        "jwcrypto==1.5.1",
+        "jwcrypto==1.5.6",
     ],
     extras_require={
         "perun": ["perun.connector==3.8.1"],
     },
     cmdclass={
         "install": PostInstallCommand,
     },
```

