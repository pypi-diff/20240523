# Comparing `tmp/utils-flask-sqlalchemy-geo-0.3.1.tar.gz` & `tmp/utils_flask_sqlalchemy_geo-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utils-flask-sqlalchemy-geo-0.3.1.tar", last modified: Mon Jan 29 15:17:51 2024, max compression
+gzip compressed data, was "utils_flask_sqlalchemy_geo-0.3.2.tar", last modified: Thu May 23 14:36:29 2024, max compression
```

## Comparing `utils-flask-sqlalchemy-geo-0.3.1.tar` & `utils_flask_sqlalchemy_geo-0.3.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:17:51.072897 utils-flask-sqlalchemy-geo-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-01-29 15:17:40.000000 utils-flask-sqlalchemy-geo-0.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-01-29 15:17:40.000000 utils-flask-sqlalchemy-geo-0.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5633 2024-01-29 15:17:51.072897 utils-flask-sqlalchemy-geo-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4565 2024-01-29 15:17:40.000000 utils-flask-sqlalchemy-geo-0.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-01-29 15:17:40.000000 utils-flask-sqlalchemy-geo-0.3.1/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-01-29 15:17:40.000000 utils-flask-sqlalchemy-geo-0.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-01-29 15:17:40.000000 utils-flask-sqlalchemy-geo-0.3.1/requirements.in
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-29 15:17:51.072897 utils-flask-sqlalchemy-geo-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-01-29 15:17:40.000000 utils-flask-sqlalchemy-geo-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:17:51.068897 utils-flask-sqlalchemy-geo-0.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:17:51.068897 utils-flask-sqlalchemy-geo-0.3.1/src/utils_flask_sqla_geo/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 15:17:40.000000 utils-flask-sqlalchemy-geo-0.3.1/src/utils_flask_sqla_geo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5404 2024-01-29 15:17:40.000000 utils-flask-sqlalchemy-geo-0.3.1/src/utils_flask_sqla_geo/export.py
--rw-r--r--   0 runner    (1001) docker     (127)     7219 2024-01-29 15:17:40.000000 utils-flask-sqlalchemy-geo-0.3.1/src/utils_flask_sqla_geo/generic.py
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-01-29 15:17:40.000000 utils-flask-sqlalchemy-geo-0.3.1/src/utils_flask_sqla_geo/mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)     8644 2024-01-29 15:17:40.000000 utils-flask-sqlalchemy-geo-0.3.1/src/utils_flask_sqla_geo/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)    11158 2024-01-29 15:17:40.000000 utils-flask-sqlalchemy-geo-0.3.1/src/utils_flask_sqla_geo/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-01-29 15:17:40.000000 utils-flask-sqlalchemy-geo-0.3.1/src/utils_flask_sqla_geo/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    18083 2024-01-29 15:17:40.000000 utils-flask-sqlalchemy-geo-0.3.1/src/utils_flask_sqla_geo/utilsgeometry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 15:17:51.072897 utils-flask-sqlalchemy-geo-0.3.1/src/utils_flask_sqlalchemy_geo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5633 2024-01-29 15:17:51.000000 utils-flask-sqlalchemy-geo-0.3.1/src/utils_flask_sqlalchemy_geo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-01-29 15:17:51.000000 utils-flask-sqlalchemy-geo-0.3.1/src/utils_flask_sqlalchemy_geo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-29 15:17:51.000000 utils-flask-sqlalchemy-geo-0.3.1/src/utils_flask_sqlalchemy_geo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-01-29 15:17:51.000000 utils-flask-sqlalchemy-geo-0.3.1/src/utils_flask_sqlalchemy_geo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-01-29 15:17:51.000000 utils-flask-sqlalchemy-geo-0.3.1/src/utils_flask_sqlalchemy_geo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-01-29 15:17:40.000000 utils-flask-sqlalchemy-geo-0.3.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:36:29.583890 utils_flask_sqlalchemy_geo-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-23 14:36:24.000000 utils_flask_sqlalchemy_geo-0.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-23 14:36:24.000000 utils_flask_sqlalchemy_geo-0.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5633 2024-05-23 14:36:29.583890 utils_flask_sqlalchemy_geo-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4565 2024-05-23 14:36:24.000000 utils_flask_sqlalchemy_geo-0.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-23 14:36:24.000000 utils_flask_sqlalchemy_geo-0.3.2/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-23 14:36:24.000000 utils_flask_sqlalchemy_geo-0.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-23 14:36:24.000000 utils_flask_sqlalchemy_geo-0.3.2/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 14:36:29.583890 utils_flask_sqlalchemy_geo-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-23 14:36:24.000000 utils_flask_sqlalchemy_geo-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:36:29.579890 utils_flask_sqlalchemy_geo-0.3.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:36:29.579890 utils_flask_sqlalchemy_geo-0.3.2/src/utils_flask_sqla_geo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 14:36:24.000000 utils_flask_sqlalchemy_geo-0.3.2/src/utils_flask_sqla_geo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5404 2024-05-23 14:36:24.000000 utils_flask_sqlalchemy_geo-0.3.2/src/utils_flask_sqla_geo/export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7219 2024-05-23 14:36:24.000000 utils_flask_sqlalchemy_geo-0.3.2/src/utils_flask_sqla_geo/generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-23 14:36:24.000000 utils_flask_sqlalchemy_geo-0.3.2/src/utils_flask_sqla_geo/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8644 2024-05-23 14:36:24.000000 utils_flask_sqlalchemy_geo-0.3.2/src/utils_flask_sqla_geo/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11158 2024-05-23 14:36:24.000000 utils_flask_sqlalchemy_geo-0.3.2/src/utils_flask_sqla_geo/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-05-23 14:36:24.000000 utils_flask_sqlalchemy_geo-0.3.2/src/utils_flask_sqla_geo/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18083 2024-05-23 14:36:24.000000 utils_flask_sqlalchemy_geo-0.3.2/src/utils_flask_sqla_geo/utilsgeometry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 14:36:29.583890 utils_flask_sqlalchemy_geo-0.3.2/src/utils_flask_sqlalchemy_geo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5633 2024-05-23 14:36:29.000000 utils_flask_sqlalchemy_geo-0.3.2/src/utils_flask_sqlalchemy_geo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-05-23 14:36:29.000000 utils_flask_sqlalchemy_geo-0.3.2/src/utils_flask_sqlalchemy_geo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 14:36:29.000000 utils_flask_sqlalchemy_geo-0.3.2/src/utils_flask_sqlalchemy_geo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-23 14:36:29.000000 utils_flask_sqlalchemy_geo-0.3.2/src/utils_flask_sqlalchemy_geo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-23 14:36:29.000000 utils_flask_sqlalchemy_geo-0.3.2/src/utils_flask_sqlalchemy_geo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-23 14:36:24.000000 utils_flask_sqlalchemy_geo-0.3.2/tox.ini
```

### Comparing `utils-flask-sqlalchemy-geo-0.3.1/LICENSE` & `utils_flask_sqlalchemy_geo-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `utils-flask-sqlalchemy-geo-0.3.1/PKG-INFO` & `utils_flask_sqlalchemy_geo-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utils-flask-sqlalchemy-geo
-Version: 0.3.1
+Version: 0.3.2
 Summary: Python lib of tools for Flask and SQLAlchemy (extension geometry)
 Home-page: https://github.com/PnX-SI/Utils-Flask-SQLAlchemy-Geo
 Maintainer: Parcs nationaux des Écrins et des Cévennes
 Maintainer-email: geonature@ecrins-parcnational.fr
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `utils-flask-sqlalchemy-geo-0.3.1/README.md` & `utils_flask_sqlalchemy_geo-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `utils-flask-sqlalchemy-geo-0.3.1/setup.py` & `utils_flask_sqlalchemy_geo-0.3.2/setup.py`

 * *Files identical despite different names*

### Comparing `utils-flask-sqlalchemy-geo-0.3.1/src/utils_flask_sqla_geo/export.py` & `utils_flask_sqlalchemy_geo-0.3.2/src/utils_flask_sqla_geo/export.py`

 * *Files identical despite different names*

### Comparing `utils-flask-sqlalchemy-geo-0.3.1/src/utils_flask_sqla_geo/generic.py` & `utils_flask_sqlalchemy_geo-0.3.2/src/utils_flask_sqla_geo/generic.py`

 * *Files identical despite different names*

### Comparing `utils-flask-sqlalchemy-geo-0.3.1/src/utils_flask_sqla_geo/schema.py` & `utils_flask_sqlalchemy_geo-0.3.2/src/utils_flask_sqla_geo/schema.py`

 * *Files identical despite different names*

### Comparing `utils-flask-sqlalchemy-geo-0.3.1/src/utils_flask_sqla_geo/serializers.py` & `utils_flask_sqlalchemy_geo-0.3.2/src/utils_flask_sqla_geo/serializers.py`

 * *Files identical despite different names*

### Comparing `utils-flask-sqlalchemy-geo-0.3.1/src/utils_flask_sqla_geo/utils.py` & `utils_flask_sqlalchemy_geo-0.3.2/src/utils_flask_sqla_geo/utils.py`

 * *Files identical despite different names*

### Comparing `utils-flask-sqlalchemy-geo-0.3.1/src/utils_flask_sqla_geo/utilsgeometry.py` & `utils_flask_sqlalchemy_geo-0.3.2/src/utils_flask_sqla_geo/utilsgeometry.py`

 * *Files identical despite different names*

### Comparing `utils-flask-sqlalchemy-geo-0.3.1/src/utils_flask_sqlalchemy_geo.egg-info/PKG-INFO` & `utils_flask_sqlalchemy_geo-0.3.2/src/utils_flask_sqlalchemy_geo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utils-flask-sqlalchemy-geo
-Version: 0.3.1
+Version: 0.3.2
 Summary: Python lib of tools for Flask and SQLAlchemy (extension geometry)
 Home-page: https://github.com/PnX-SI/Utils-Flask-SQLAlchemy-Geo
 Maintainer: Parcs nationaux des Écrins et des Cévennes
 Maintainer-email: geonature@ecrins-parcnational.fr
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `utils-flask-sqlalchemy-geo-0.3.1/src/utils_flask_sqlalchemy_geo.egg-info/SOURCES.txt` & `utils_flask_sqlalchemy_geo-0.3.2/src/utils_flask_sqlalchemy_geo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

