# Comparing `tmp/dj-jwt-auth-1.3.1.tar.gz` & `tmp/dj-jwt-auth-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dj-jwt-auth-1.3.1.tar", last modified: Fri May 17 13:25:31 2024, max compression
+gzip compressed data, was "dj-jwt-auth-1.3.2.tar", last modified: Thu May 23 16:46:55 2024, max compression
```

## Comparing `dj-jwt-auth-1.3.1.tar` & `dj-jwt-auth-1.3.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:25:31.414789 dj-jwt-auth-1.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)     3867 2024-05-17 13:25:31.414789 dj-jwt-auth-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-05-17 13:25:19.000000 dj-jwt-auth-1.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:25:31.414789 dj-jwt-auth-1.3.1/dj_jwt_auth.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3867 2024-05-17 13:25:31.000000 dj-jwt-auth-1.3.1/dj_jwt_auth.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-17 13:25:31.000000 dj-jwt-auth-1.3.1/dj_jwt_auth.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 13:25:31.000000 dj-jwt-auth-1.3.1/dj_jwt_auth.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-17 13:25:31.000000 dj-jwt-auth-1.3.1/dj_jwt_auth.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-17 13:25:31.000000 dj-jwt-auth-1.3.1/dj_jwt_auth.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:25:31.414789 dj-jwt-auth-1.3.1/django_jwt/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 13:25:19.000000 dj-jwt-auth-1.3.1/django_jwt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-17 13:25:19.000000 dj-jwt-auth-1.3.1/django_jwt/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-17 13:25:19.000000 dj-jwt-auth-1.3.1/django_jwt/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-17 13:25:19.000000 dj-jwt-auth-1.3.1/django_jwt/middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-17 13:25:19.000000 dj-jwt-auth-1.3.1/django_jwt/pkce.py
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-17 13:25:19.000000 dj-jwt-auth-1.3.1/django_jwt/roles.py
--rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-05-17 13:25:19.000000 dj-jwt-auth-1.3.1/django_jwt/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-17 13:25:19.000000 dj-jwt-auth-1.3.1/django_jwt/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     5021 2024-05-17 13:25:19.000000 dj-jwt-auth-1.3.1/django_jwt/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-17 13:25:19.000000 dj-jwt-auth-1.3.1/django_jwt/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3705 2024-05-17 13:25:19.000000 dj-jwt-auth-1.3.1/django_jwt/views.py
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-17 13:25:19.000000 dj-jwt-auth-1.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-05-17 13:25:31.414789 dj-jwt-auth-1.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-17 13:25:19.000000 dj-jwt-auth-1.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 13:25:31.414789 dj-jwt-auth-1.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 13:25:19.000000 dj-jwt-auth-1.3.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-17 13:25:19.000000 dj-jwt-auth-1.3.1/tests/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     7460 2024-05-17 13:25:19.000000 dj-jwt-auth-1.3.1/tests/test.py
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-17 13:25:19.000000 dj-jwt-auth-1.3.1/tests/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:46:55.135604 dj-jwt-auth-1.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     3867 2024-05-23 16:46:55.135604 dj-jwt-auth-1.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-05-23 16:46:41.000000 dj-jwt-auth-1.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:46:55.131604 dj-jwt-auth-1.3.2/dj_jwt_auth.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3867 2024-05-23 16:46:55.000000 dj-jwt-auth-1.3.2/dj_jwt_auth.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-05-23 16:46:55.000000 dj-jwt-auth-1.3.2/dj_jwt_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 16:46:55.000000 dj-jwt-auth-1.3.2/dj_jwt_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-23 16:46:55.000000 dj-jwt-auth-1.3.2/dj_jwt_auth.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-23 16:46:55.000000 dj-jwt-auth-1.3.2/dj_jwt_auth.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:46:55.135604 dj-jwt-auth-1.3.2/django_jwt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 16:46:41.000000 dj-jwt-auth-1.3.2/django_jwt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-23 16:46:41.000000 dj-jwt-auth-1.3.2/django_jwt/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-23 16:46:41.000000 dj-jwt-auth-1.3.2/django_jwt/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-23 16:46:41.000000 dj-jwt-auth-1.3.2/django_jwt/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-23 16:46:41.000000 dj-jwt-auth-1.3.2/django_jwt/pkce.py
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-23 16:46:41.000000 dj-jwt-auth-1.3.2/django_jwt/roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-05-23 16:46:41.000000 dj-jwt-auth-1.3.2/django_jwt/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-23 16:46:41.000000 dj-jwt-auth-1.3.2/django_jwt/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5021 2024-05-23 16:46:41.000000 dj-jwt-auth-1.3.2/django_jwt/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-23 16:46:41.000000 dj-jwt-auth-1.3.2/django_jwt/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3705 2024-05-23 16:46:41.000000 dj-jwt-auth-1.3.2/django_jwt/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-23 16:46:41.000000 dj-jwt-auth-1.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      991 2024-05-23 16:46:55.135604 dj-jwt-auth-1.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-23 16:46:41.000000 dj-jwt-auth-1.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 16:46:55.135604 dj-jwt-auth-1.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 16:46:41.000000 dj-jwt-auth-1.3.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-23 16:46:41.000000 dj-jwt-auth-1.3.2/tests/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7460 2024-05-23 16:46:41.000000 dj-jwt-auth-1.3.2/tests/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-23 16:46:41.000000 dj-jwt-auth-1.3.2/tests/urls.py
```

### Comparing `dj-jwt-auth-1.3.1/PKG-INFO` & `dj-jwt-auth-1.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dj-jwt-auth
-Version: 1.3.1
+Version: 1.3.2
 Summary: A Django package for JSON Web Token validation and verification. Using PyJWT.
 Home-page: https://www.example.com/
 Author: Konstantin Seleznev
 Author-email: k.seleznev@elsevier.com
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `dj-jwt-auth-1.3.1/README.md` & `dj-jwt-auth-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `dj-jwt-auth-1.3.1/dj_jwt_auth.egg-info/PKG-INFO` & `dj-jwt-auth-1.3.2/dj_jwt_auth.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dj-jwt-auth
-Version: 1.3.1
+Version: 1.3.2
 Summary: A Django package for JSON Web Token validation and verification. Using PyJWT.
 Home-page: https://www.example.com/
 Author: Konstantin Seleznev
 Author-email: k.seleznev@elsevier.com
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `dj-jwt-auth-1.3.1/dj_jwt_auth.egg-info/SOURCES.txt` & `dj-jwt-auth-1.3.2/dj_jwt_auth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dj-jwt-auth-1.3.1/django_jwt/config.py` & `dj-jwt-auth-1.3.2/django_jwt/config.py`

 * *Files identical despite different names*

### Comparing `dj-jwt-auth-1.3.1/django_jwt/middleware.py` & `dj-jwt-auth-1.3.2/django_jwt/middleware.py`

 * *Files identical despite different names*

### Comparing `dj-jwt-auth-1.3.1/django_jwt/pkce.py` & `dj-jwt-auth-1.3.2/django_jwt/pkce.py`

 * *Files identical despite different names*

### Comparing `dj-jwt-auth-1.3.1/django_jwt/settings.py` & `dj-jwt-auth-1.3.2/django_jwt/settings.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,13 +34,13 @@
     settings,
     "OIDC_USER_ON_UPDATE",
     None,
 )
 
 OIDC_CONFIG_ROUTES = getattr(settings, "OIDC_CONFIG_ROUTES", None)
 OIDC_ADMIN_ISSUER = getattr(settings, "OIDC_ADMIN_ISSUER", None)
-OIDC_ADMIN_CLIENT_ID = getattr(settings, "OIDC_ADMIN_CLIENT_ID", "complete-anatomy")
+OIDC_ADMIN_CLIENT_ID = getattr(settings, "OIDC_ADMIN_CLIENT_ID", "cs-completeanatomy-admin")
 OIDC_ADMIN_SCOPE = getattr(settings, "OIDC_ADMIN_SCOPE", "openid")
 OIDC_ADMIN_ROLES = getattr(settings, "OIDC_ADMIN_ROLES", [])
 
 for role in OIDC_ADMIN_ROLES:
     assert isinstance(role, ROLE), f"Role must be a namedtuple, got {type(role)}"
```

### Comparing `dj-jwt-auth-1.3.1/django_jwt/user.py` & `dj-jwt-auth-1.3.2/django_jwt/user.py`

 * *Files identical despite different names*

### Comparing `dj-jwt-auth-1.3.1/django_jwt/utils.py` & `dj-jwt-auth-1.3.2/django_jwt/utils.py`

 * *Files identical despite different names*

### Comparing `dj-jwt-auth-1.3.1/django_jwt/views.py` & `dj-jwt-auth-1.3.2/django_jwt/views.py`

 * *Files identical despite different names*

### Comparing `dj-jwt-auth-1.3.1/setup.cfg` & `dj-jwt-auth-1.3.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = dj-jwt-auth
-version = 1.3.1
+version = 1.3.2
 description = A Django package for JSON Web Token validation and verification. Using PyJWT.
 long_description = file: README.md
 url = https://www.example.com/
 author = Konstantin Seleznev
 author_email = k.seleznev@elsevier.com
 license = MIT
 classifiers =
```

### Comparing `dj-jwt-auth-1.3.1/tests/test.py` & `dj-jwt-auth-1.3.2/tests/test.py`

 * *Files identical despite different names*

