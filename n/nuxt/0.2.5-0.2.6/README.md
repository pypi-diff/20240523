# Comparing `tmp/nuxt-0.2.5.tar.gz` & `tmp/nuxt-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nuxt-0.2.5.tar", last modified: Sun Feb  4 02:44:34 2024, max compression
+gzip compressed data, was "nuxt-0.2.6.tar", last modified: Thu May 23 08:13:00 2024, max compression
```

## Comparing `nuxt-0.2.5.tar` & `nuxt-0.2.6.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxr-x   0 arvin     (1000) arvin     (1000)        0 2024-02-04 02:44:34.423721 nuxt-0.2.5/
--rw-rw-r--   0 arvin     (1000) arvin     (1000)      196 2023-04-08 07:15:56.000000 nuxt-0.2.5/MANIFEST.in
--rw-rw-r--   0 arvin     (1000) arvin     (1000)      504 2024-02-04 02:44:34.423721 nuxt-0.2.5/PKG-INFO
--rw-rw-r--   0 arvin     (1000) arvin     (1000)     8888 2023-04-08 07:15:56.000000 nuxt-0.2.5/README.md
-drwxrwxr-x   0 arvin     (1000) arvin     (1000)        0 2024-02-04 02:44:34.423721 nuxt-0.2.5/nuxt/
--rw-rw-r--   0 arvin     (1000) arvin     (1000)      596 2023-11-19 06:57:59.000000 nuxt-0.2.5/nuxt/__init__.py
--rw-rw-r--   0 arvin     (1000) arvin     (1000)     6838 2023-07-13 02:51:17.000000 nuxt-0.2.5/nuxt/__main__.py
--rw-rw-r--   0 arvin     (1000) arvin     (1000)    15666 2024-01-13 07:44:13.000000 nuxt-0.2.5/nuxt/app.py
-drwxrwxr-x   0 arvin     (1000) arvin     (1000)        0 2024-02-04 02:44:34.423721 nuxt-0.2.5/nuxt/asyncio/
--rw-rw-r--   0 arvin     (1000) arvin     (1000)      847 2023-04-08 07:15:56.000000 nuxt-0.2.5/nuxt/asyncio/__init__.py
-drwxrwxr-x   0 arvin     (1000) arvin     (1000)        0 2024-02-04 02:44:34.423721 nuxt-0.2.5/nuxt/asyncio/repositorys/
--rw-rw-r--   0 arvin     (1000) arvin     (1000)        0 2023-04-08 07:15:56.000000 nuxt-0.2.5/nuxt/asyncio/repositorys/__init__.py
--rw-rw-r--   0 arvin     (1000) arvin     (1000)     4577 2024-02-02 04:10:46.000000 nuxt-0.2.5/nuxt/asyncio/repositorys/validation.py
--rw-rw-r--   0 arvin     (1000) arvin     (1000)      111 2023-04-08 07:15:56.000000 nuxt-0.2.5/nuxt/datastructures.py
--rw-rw-r--   0 arvin     (1000) arvin     (1000)      256 2023-04-08 07:15:56.000000 nuxt-0.2.5/nuxt/exceptions.py
--rw-rw-r--   0 arvin     (1000) arvin     (1000)     6241 2023-04-08 07:15:56.000000 nuxt-0.2.5/nuxt/openapi.py
--rw-rw-r--   0 arvin     (1000) arvin     (1000)     3848 2023-04-08 07:15:56.000000 nuxt-0.2.5/nuxt/reloader.py
-drwxrwxr-x   0 arvin     (1000) arvin     (1000)        0 2024-02-04 02:44:34.423721 nuxt-0.2.5/nuxt/repositorys/
--rw-rw-r--   0 arvin     (1000) arvin     (1000)        0 2023-04-08 07:15:56.000000 nuxt-0.2.5/nuxt/repositorys/__init__.py
--rw-rw-r--   0 arvin     (1000) arvin     (1000)        0 2023-04-08 07:15:56.000000 nuxt-0.2.5/nuxt/repositorys/empty.py
--rw-rw-r--   0 arvin     (1000) arvin     (1000)     4488 2023-11-03 04:58:33.000000 nuxt-0.2.5/nuxt/repositorys/validation.py
--rw-rw-r--   0 arvin     (1000) arvin     (1000)      149 2023-04-08 07:15:56.000000 nuxt-0.2.5/nuxt/requests.py
--rw-rw-r--   0 arvin     (1000) arvin     (1000)      459 2023-04-08 07:15:56.000000 nuxt-0.2.5/nuxt/responses.py
--rw-rw-r--   0 arvin     (1000) arvin     (1000)       54 2023-04-08 07:15:56.000000 nuxt-0.2.5/nuxt/routing.py
--rw-rw-r--   0 arvin     (1000) arvin     (1000)     4959 2023-07-24 03:17:29.000000 nuxt-0.2.5/nuxt/staticfiles.py
--rw-rw-r--   0 arvin     (1000) arvin     (1000)     1249 2023-04-08 07:15:56.000000 nuxt-0.2.5/nuxt/templating.py
--rw-rw-r--   0 arvin     (1000) arvin     (1000)     3692 2023-04-08 07:15:56.000000 nuxt-0.2.5/nuxt/utils.py
-drwxrwxr-x   0 arvin     (1000) arvin     (1000)        0 2024-02-04 02:44:34.423721 nuxt-0.2.5/nuxt.egg-info/
--rw-rw-r--   0 arvin     (1000) arvin     (1000)      504 2024-02-04 02:44:34.000000 nuxt-0.2.5/nuxt.egg-info/PKG-INFO
--rw-rw-r--   0 arvin     (1000) arvin     (1000)      656 2024-02-04 02:44:34.000000 nuxt-0.2.5/nuxt.egg-info/SOURCES.txt
--rw-rw-r--   0 arvin     (1000) arvin     (1000)        1 2024-02-04 02:44:34.000000 nuxt-0.2.5/nuxt.egg-info/dependency_links.txt
--rw-rw-r--   0 arvin     (1000) arvin     (1000)       43 2024-02-04 02:44:34.000000 nuxt-0.2.5/nuxt.egg-info/entry_points.txt
--rw-rw-r--   0 arvin     (1000) arvin     (1000)        1 2024-02-04 02:44:34.000000 nuxt-0.2.5/nuxt.egg-info/not-zip-safe
--rw-rw-r--   0 arvin     (1000) arvin     (1000)      221 2024-02-04 02:44:34.000000 nuxt-0.2.5/nuxt.egg-info/requires.txt
--rw-rw-r--   0 arvin     (1000) arvin     (1000)       11 2024-02-04 02:44:34.000000 nuxt-0.2.5/nuxt.egg-info/top_level.txt
--rw-rw-r--   0 arvin     (1000) arvin     (1000)      220 2024-02-04 02:39:43.000000 nuxt-0.2.5/requirements.txt
--rw-rw-r--   0 arvin     (1000) arvin     (1000)       38 2024-02-04 02:44:34.423721 nuxt-0.2.5/setup.cfg
--rw-rw-r--   0 arvin     (1000) arvin     (1000)     1394 2024-02-04 02:34:08.000000 nuxt-0.2.5/setup.py
+drwxrwxr-x   0 arvin     (1000) arvin     (1000)        0 2024-05-23 08:13:00.872168 nuxt-0.2.6/
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)      196 2023-04-08 07:15:56.000000 nuxt-0.2.6/MANIFEST.in
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)      504 2024-05-23 08:13:00.872168 nuxt-0.2.6/PKG-INFO
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)     8888 2023-04-08 07:15:56.000000 nuxt-0.2.6/README.md
+drwxrwxr-x   0 arvin     (1000) arvin     (1000)        0 2024-05-23 08:13:00.872168 nuxt-0.2.6/nuxt/
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)      596 2023-11-19 06:57:59.000000 nuxt-0.2.6/nuxt/__init__.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)     6838 2023-07-13 02:51:17.000000 nuxt-0.2.6/nuxt/__main__.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)    15666 2024-01-13 07:44:13.000000 nuxt-0.2.6/nuxt/app.py
+drwxrwxr-x   0 arvin     (1000) arvin     (1000)        0 2024-05-23 08:13:00.872168 nuxt-0.2.6/nuxt/asyncio/
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)      847 2023-04-08 07:15:56.000000 nuxt-0.2.6/nuxt/asyncio/__init__.py
+drwxrwxr-x   0 arvin     (1000) arvin     (1000)        0 2024-05-23 08:13:00.872168 nuxt-0.2.6/nuxt/asyncio/repositorys/
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)        0 2023-04-08 07:15:56.000000 nuxt-0.2.6/nuxt/asyncio/repositorys/__init__.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)     4577 2024-02-02 04:10:46.000000 nuxt-0.2.6/nuxt/asyncio/repositorys/validation.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)      111 2023-04-08 07:15:56.000000 nuxt-0.2.6/nuxt/datastructures.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)      256 2023-04-08 07:15:56.000000 nuxt-0.2.6/nuxt/exceptions.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)     6241 2023-04-08 07:15:56.000000 nuxt-0.2.6/nuxt/openapi.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)     3848 2023-04-08 07:15:56.000000 nuxt-0.2.6/nuxt/reloader.py
+drwxrwxr-x   0 arvin     (1000) arvin     (1000)        0 2024-05-23 08:13:00.872168 nuxt-0.2.6/nuxt/repositorys/
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)        0 2023-04-08 07:15:56.000000 nuxt-0.2.6/nuxt/repositorys/__init__.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)        0 2023-04-08 07:15:56.000000 nuxt-0.2.6/nuxt/repositorys/empty.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)     4488 2023-11-03 04:58:33.000000 nuxt-0.2.6/nuxt/repositorys/validation.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)      149 2023-04-08 07:15:56.000000 nuxt-0.2.6/nuxt/requests.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)      459 2023-04-08 07:15:56.000000 nuxt-0.2.6/nuxt/responses.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)       54 2023-04-08 07:15:56.000000 nuxt-0.2.6/nuxt/routing.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)     4959 2023-07-24 03:17:29.000000 nuxt-0.2.6/nuxt/staticfiles.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)     1249 2023-04-08 07:15:56.000000 nuxt-0.2.6/nuxt/templating.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)     3692 2023-04-08 07:15:56.000000 nuxt-0.2.6/nuxt/utils.py
+drwxrwxr-x   0 arvin     (1000) arvin     (1000)        0 2024-05-23 08:13:00.872168 nuxt-0.2.6/nuxt.egg-info/
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)      504 2024-05-23 08:13:00.000000 nuxt-0.2.6/nuxt.egg-info/PKG-INFO
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)      656 2024-05-23 08:13:00.000000 nuxt-0.2.6/nuxt.egg-info/SOURCES.txt
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)        1 2024-05-23 08:13:00.000000 nuxt-0.2.6/nuxt.egg-info/dependency_links.txt
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)       43 2024-05-23 08:13:00.000000 nuxt-0.2.6/nuxt.egg-info/entry_points.txt
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)        1 2024-05-23 08:13:00.000000 nuxt-0.2.6/nuxt.egg-info/not-zip-safe
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)      226 2024-05-23 08:13:00.000000 nuxt-0.2.6/nuxt.egg-info/requires.txt
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)       11 2024-05-23 08:13:00.000000 nuxt-0.2.6/nuxt.egg-info/top_level.txt
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)      225 2024-05-23 08:11:34.000000 nuxt-0.2.6/requirements.txt
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)       38 2024-05-23 08:13:00.872168 nuxt-0.2.6/setup.cfg
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)     1394 2024-05-23 08:10:05.000000 nuxt-0.2.6/setup.py
```

### Comparing `nuxt-0.2.5/README.md` & `nuxt-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `nuxt-0.2.5/nuxt/__init__.py` & `nuxt-0.2.6/nuxt/__init__.py`

 * *Files identical despite different names*

### Comparing `nuxt-0.2.5/nuxt/__main__.py` & `nuxt-0.2.6/nuxt/__main__.py`

 * *Files identical despite different names*

### Comparing `nuxt-0.2.5/nuxt/app.py` & `nuxt-0.2.6/nuxt/app.py`

 * *Files identical despite different names*

### Comparing `nuxt-0.2.5/nuxt/asyncio/__init__.py` & `nuxt-0.2.6/nuxt/asyncio/__init__.py`

 * *Files identical despite different names*

### Comparing `nuxt-0.2.5/nuxt/asyncio/repositorys/validation.py` & `nuxt-0.2.6/nuxt/asyncio/repositorys/validation.py`

 * *Files identical despite different names*

### Comparing `nuxt-0.2.5/nuxt/openapi.py` & `nuxt-0.2.6/nuxt/openapi.py`

 * *Files identical despite different names*

### Comparing `nuxt-0.2.5/nuxt/reloader.py` & `nuxt-0.2.6/nuxt/reloader.py`

 * *Files identical despite different names*

### Comparing `nuxt-0.2.5/nuxt/repositorys/validation.py` & `nuxt-0.2.6/nuxt/repositorys/validation.py`

 * *Files identical despite different names*

### Comparing `nuxt-0.2.5/nuxt/staticfiles.py` & `nuxt-0.2.6/nuxt/staticfiles.py`

 * *Files identical despite different names*

### Comparing `nuxt-0.2.5/nuxt/templating.py` & `nuxt-0.2.6/nuxt/templating.py`

 * *Files identical despite different names*

### Comparing `nuxt-0.2.5/nuxt/utils.py` & `nuxt-0.2.6/nuxt/utils.py`

 * *Files identical despite different names*

### Comparing `nuxt-0.2.5/nuxt.egg-info/SOURCES.txt` & `nuxt-0.2.6/nuxt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nuxt-0.2.5/setup.py` & `nuxt-0.2.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import find_packages
 
 os.chdir(os.path.dirname(sys.argv[0]) or ".")
 here = os.path.abspath(os.path.dirname(__file__))
 
 setup_args = dict(
     name='nuxt',
-    version='0.2.5',
+    version='0.2.6',
     description='A integration framework for build web app.',
     long_description="Nuxt is a integration framework for build web app, built on top of [Madara](https://github.com/Arvintian/madara)/[Starlette](https://github.com/encode/starlette)/[Gunicorn](https://github.com/benoitc/gunicorn)/[Uvicorn](https://github.com/encode/uvicorn).",
     long_description_content_type="text/markdown",
     author='arvin',
     license='MIT',
     url='https://github.com/Arvintian/nuxt',
     author_email='arvintian8@gamil.com',
```

