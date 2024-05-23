# Comparing `tmp/georecl-0.0.1.tar.gz` & `tmp/georecl-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "georecl-0.1.0.tar", max compression
```

## Comparing `georecl-0.0.1.tar` & `georecl-0.1.0.tar`

### file list

```diff
@@ -1,10 +1,6 @@
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 georecl-0.0.1/.pypirc
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 georecl-0.0.1/Readme.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 georecl-0.0.1/src/georecl/__init__.py
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 georecl-0.0.1/src/georecl/geoserver.py
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 georecl-0.0.1/src/georecl/main.py
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 georecl-0.0.1/tests/test.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 georecl-0.0.1/LICENSE
--rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 georecl-0.0.1/README.md
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 georecl-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      748 2020-02-02 00:00:00.000000 georecl-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-23 14:14:32.010214 georecl-0.1.0/georecl/__init__.py
+-rw-r--r--   0        0        0     1686 2024-05-23 14:24:37.948198 georecl-0.1.0/georecl/geoserver.py
+-rw-r--r--   0        0        0      333 2024-05-21 17:30:14.880592 georecl-0.1.0/georecl/main.py
+-rw-r--r--   0        0        0      455 2024-05-23 14:26:54.724319 georecl-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-23 14:14:32.010214 georecl-0.1.0/README.md
+-rw-r--r--   0        0        0      393 1970-01-01 00:00:00.000000 georecl-0.1.0/PKG-INFO
```

### Comparing `georecl-0.0.1/src/georecl/geoserver.py` & `georecl-0.1.0/georecl/geoserver.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from requests import Session,PreparedRequest
 from requests.auth import AuthBase
 
 
-
 class GeoserverAuth1(AuthBase):
     def __init__(self,username=None,password=None,authkey=None) -> None:
         super().__init__()
         self.username=username
         self.password=password
         self.authkey=authkey
     def __call__(self, r: PreparedRequest) -> PreparedRequest:
```

