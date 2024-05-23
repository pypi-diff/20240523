# Comparing `tmp/boto3_session-0.0.6.tar.gz` & `tmp/boto3_session-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boto3_session-0.0.6.tar", max compression
+gzip compressed data, was "boto3_session-0.0.7.tar", max compression
```

## Comparing `boto3_session-0.0.6.tar` & `boto3_session-0.0.7.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0    11337 2023-12-26 07:20:25.416872 boto3_session-0.0.6/LICENSE
--rw-r--r--   0        0        0     2493 2023-12-26 08:48:56.027814 boto3_session-0.0.6/README.md
--rw-r--r--   0        0        0     2156 2023-12-28 02:08:44.992447 boto3_session-0.0.6/pyproject.toml
--rw-r--r--   0        0        0      104 2023-12-26 07:20:25.418060 boto3_session-0.0.6/src/boto3_session/__init__.py
--rw-r--r--   0        0        0       93 2023-12-26 07:20:25.418144 boto3_session-0.0.6/src/boto3_session/__version__.py
--rw-r--r--   0        0        0     4095 2023-12-28 02:07:22.148698 boto3_session-0.0.6/src/boto3_session/session.py
--rw-r--r--   0        0        0     3260 1970-01-01 00:00:00.000000 boto3_session-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0    11337 2023-12-26 07:20:25.416872 boto3_session-0.0.7/LICENSE
+-rw-r--r--   0        0        0     2493 2023-12-26 08:48:56.027814 boto3_session-0.0.7/README.md
+-rw-r--r--   0        0        0     2156 2024-05-23 00:09:53.325049 boto3_session-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0      104 2023-12-26 07:20:25.418060 boto3_session-0.0.7/src/boto3_session/__init__.py
+-rw-r--r--   0        0        0       93 2023-12-26 07:20:25.418144 boto3_session-0.0.7/src/boto3_session/__version__.py
+-rw-r--r--   0        0        0        0 2024-05-23 00:09:41.245352 boto3_session-0.0.7/src/boto3_session/py.typed
+-rw-r--r--   0        0        0     4095 2023-12-28 02:07:22.148698 boto3_session-0.0.7/src/boto3_session/session.py
+-rw-r--r--   0        0        0     3260 1970-01-01 00:00:00.000000 boto3_session-0.0.7/PKG-INFO
```

### Comparing `boto3_session-0.0.6/LICENSE` & `boto3_session-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `boto3_session-0.0.6/README.md` & `boto3_session-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `boto3_session-0.0.6/pyproject.toml` & `boto3_session-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "boto3-session"
-version = "0.0.6"
+version = "0.0.7"
 description = "Wrapper library for python boto3.session.Session."
 authors = ["rcmdnk <rcmdnk@gmail.com>"]
 repository = "https://github.com/rcmdnk/boto3-session"
 homepage = "https://github.com/rcmdnk/boto3-session"
 readme = "README.md"
 license = "apache-2.0"
 keywords = ['aws', 'boto3']
```

### Comparing `boto3_session-0.0.6/src/boto3_session/session.py` & `boto3_session-0.0.7/src/boto3_session/session.py`

 * *Files identical despite different names*

### Comparing `boto3_session-0.0.6/PKG-INFO` & `boto3_session-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boto3-session
-Version: 0.0.6
+Version: 0.0.7
 Summary: Wrapper library for python boto3.session.Session.
 Home-page: https://github.com/rcmdnk/boto3-session
 License: Apache-2.0
 Keywords: aws,boto3
 Author: rcmdnk
 Author-email: rcmdnk@gmail.com
 Requires-Python: >=3.9,<4.0
```

