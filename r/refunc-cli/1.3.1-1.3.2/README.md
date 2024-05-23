# Comparing `tmp/refunc-cli-1.3.1.tar.gz` & `tmp/refunc-cli-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "refunc-cli-1.3.1.tar", last modified: Sat Sep 30 09:39:23 2023, max compression
+gzip compressed data, was "refunc-cli-1.3.2.tar", last modified: Thu May 23 09:21:37 2024, max compression
```

## Comparing `refunc-cli-1.3.1.tar` & `refunc-cli-1.3.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 arvin     (1000) arvin     (1000)        0 2023-09-30 09:39:23.725506 refunc-cli-1.3.1/
--rw-rw-r--   0 arvin     (1000) arvin     (1000)      197 2023-04-28 05:17:10.000000 refunc-cli-1.3.1/MANIFEST.in
--rw-rw-r--   0 arvin     (1000) arvin     (1000)      199 2023-09-30 09:39:23.725506 refunc-cli-1.3.1/PKG-INFO
--rw-rw-r--   0 arvin     (1000) arvin     (1000)      494 2023-04-28 05:17:10.000000 refunc-cli-1.3.1/README.md
-drwxrwxr-x   0 arvin     (1000) arvin     (1000)        0 2023-09-30 09:39:23.725506 refunc-cli-1.3.1/refunc_cli.egg-info/
--rw-rw-r--   0 arvin     (1000) arvin     (1000)      199 2023-09-30 09:39:23.000000 refunc-cli-1.3.1/refunc_cli.egg-info/PKG-INFO
--rw-rw-r--   0 arvin     (1000) arvin     (1000)      600 2023-09-30 09:39:23.000000 refunc-cli-1.3.1/refunc_cli.egg-info/SOURCES.txt
--rw-rw-r--   0 arvin     (1000) arvin     (1000)        1 2023-09-30 09:39:23.000000 refunc-cli-1.3.1/refunc_cli.egg-info/dependency_links.txt
--rw-rw-r--   0 arvin     (1000) arvin     (1000)       45 2023-09-30 09:39:23.000000 refunc-cli-1.3.1/refunc_cli.egg-info/entry_points.txt
--rw-rw-r--   0 arvin     (1000) arvin     (1000)        1 2023-09-30 09:39:23.000000 refunc-cli-1.3.1/refunc_cli.egg-info/not-zip-safe
--rw-rw-r--   0 arvin     (1000) arvin     (1000)      114 2023-09-30 09:39:23.000000 refunc-cli-1.3.1/refunc_cli.egg-info/requires.txt
--rw-rw-r--   0 arvin     (1000) arvin     (1000)        6 2023-09-30 09:39:23.000000 refunc-cli-1.3.1/refunc_cli.egg-info/top_level.txt
--rw-rw-r--   0 arvin     (1000) arvin     (1000)      113 2023-04-28 05:17:10.000000 refunc-cli-1.3.1/requirements.txt
-drwxrwxr-x   0 arvin     (1000) arvin     (1000)        0 2023-09-30 09:39:23.725506 refunc-cli-1.3.1/rfctl/
--rw-rw-r--   0 arvin     (1000) arvin     (1000)        0 2023-04-28 05:17:10.000000 refunc-cli-1.3.1/rfctl/__init__.py
--rw-rw-r--   0 arvin     (1000) arvin     (1000)     2432 2023-08-14 02:10:29.000000 refunc-cli-1.3.1/rfctl/__main__.py
--rw-rw-r--   0 arvin     (1000) arvin     (1000)     1561 2023-07-12 10:13:25.000000 refunc-cli-1.3.1/rfctl/awslocal.py
--rw-rw-r--   0 arvin     (1000) arvin     (1000)     3738 2023-04-28 05:17:10.000000 refunc-cli-1.3.1/rfctl/build.py
-drwxrwxr-x   0 arvin     (1000) arvin     (1000)        0 2023-09-30 09:39:23.725506 refunc-cli-1.3.1/rfctl/client/
--rw-rw-r--   0 arvin     (1000) arvin     (1000)       33 2023-04-28 05:17:10.000000 refunc-cli-1.3.1/rfctl/client/__init__.py
--rw-rw-r--   0 arvin     (1000) arvin     (1000)     1557 2023-07-12 10:43:11.000000 refunc-cli-1.3.1/rfctl/client/client.py
--rw-rw-r--   0 arvin     (1000) arvin     (1000)     1431 2023-09-30 09:36:10.000000 refunc-cli-1.3.1/rfctl/create.py
--rw-rw-r--   0 arvin     (1000) arvin     (1000)      498 2023-04-28 05:17:10.000000 refunc-cli-1.3.1/rfctl/create_url.py
--rw-rw-r--   0 arvin     (1000) arvin     (1000)      433 2023-04-28 05:17:10.000000 refunc-cli-1.3.1/rfctl/delete.py
--rw-rw-r--   0 arvin     (1000) arvin     (1000)      456 2023-04-28 05:17:10.000000 refunc-cli-1.3.1/rfctl/delete_url.py
--rw-rw-r--   0 arvin     (1000) arvin     (1000)      422 2023-04-28 05:17:10.000000 refunc-cli-1.3.1/rfctl/get.py
--rw-rw-r--   0 arvin     (1000) arvin     (1000)      441 2023-04-28 05:17:10.000000 refunc-cli-1.3.1/rfctl/get_url.py
--rw-rw-r--   0 arvin     (1000) arvin     (1000)     3203 2023-09-30 08:56:30.000000 refunc-cli-1.3.1/rfctl/init.py
--rw-rw-r--   0 arvin     (1000) arvin     (1000)     1458 2023-04-28 05:17:10.000000 refunc-cli-1.3.1/rfctl/init_source.py
--rw-rw-r--   0 arvin     (1000) arvin     (1000)     2014 2023-04-28 05:17:10.000000 refunc-cli-1.3.1/rfctl/schema.py
--rw-rw-r--   0 arvin     (1000) arvin     (1000)      680 2023-04-28 05:17:10.000000 refunc-cli-1.3.1/rfctl/update_code.py
--rw-rw-r--   0 arvin     (1000) arvin     (1000)     1235 2023-09-30 09:36:25.000000 refunc-cli-1.3.1/rfctl/update_config.py
--rw-rw-r--   0 arvin     (1000) arvin     (1000)       38 2023-09-30 09:39:23.725506 refunc-cli-1.3.1/setup.cfg
--rw-rw-r--   0 arvin     (1000) arvin     (1000)     1033 2023-09-30 09:32:07.000000 refunc-cli-1.3.1/setup.py
+drwxrwxr-x   0 arvin     (1000) arvin     (1000)        0 2024-05-23 09:21:37.420711 refunc-cli-1.3.2/
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)      197 2023-04-28 05:17:10.000000 refunc-cli-1.3.2/MANIFEST.in
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)      199 2024-05-23 09:21:37.420711 refunc-cli-1.3.2/PKG-INFO
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)      494 2023-04-28 05:17:10.000000 refunc-cli-1.3.2/README.md
+drwxrwxr-x   0 arvin     (1000) arvin     (1000)        0 2024-05-23 09:21:37.420711 refunc-cli-1.3.2/refunc_cli.egg-info/
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)      199 2024-05-23 09:21:37.000000 refunc-cli-1.3.2/refunc_cli.egg-info/PKG-INFO
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)      600 2024-05-23 09:21:37.000000 refunc-cli-1.3.2/refunc_cli.egg-info/SOURCES.txt
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)        1 2024-05-23 09:21:37.000000 refunc-cli-1.3.2/refunc_cli.egg-info/dependency_links.txt
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)       45 2024-05-23 09:21:37.000000 refunc-cli-1.3.2/refunc_cli.egg-info/entry_points.txt
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)        1 2024-05-23 09:21:37.000000 refunc-cli-1.3.2/refunc_cli.egg-info/not-zip-safe
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)      114 2024-05-23 09:21:37.000000 refunc-cli-1.3.2/refunc_cli.egg-info/requires.txt
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)        6 2024-05-23 09:21:37.000000 refunc-cli-1.3.2/refunc_cli.egg-info/top_level.txt
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)      113 2024-05-23 08:38:14.000000 refunc-cli-1.3.2/requirements.txt
+drwxrwxr-x   0 arvin     (1000) arvin     (1000)        0 2024-05-23 09:21:37.420711 refunc-cli-1.3.2/rfctl/
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)        0 2023-04-28 05:17:10.000000 refunc-cli-1.3.2/rfctl/__init__.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)     2432 2023-08-14 02:10:29.000000 refunc-cli-1.3.2/rfctl/__main__.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)     1561 2023-07-12 10:13:25.000000 refunc-cli-1.3.2/rfctl/awslocal.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)     3818 2024-05-23 09:11:31.000000 refunc-cli-1.3.2/rfctl/build.py
+drwxrwxr-x   0 arvin     (1000) arvin     (1000)        0 2024-05-23 09:21:37.420711 refunc-cli-1.3.2/rfctl/client/
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)       33 2023-04-28 05:17:10.000000 refunc-cli-1.3.2/rfctl/client/__init__.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)     1557 2023-07-12 10:43:11.000000 refunc-cli-1.3.2/rfctl/client/client.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)     1431 2023-09-30 09:36:10.000000 refunc-cli-1.3.2/rfctl/create.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)      498 2023-04-28 05:17:10.000000 refunc-cli-1.3.2/rfctl/create_url.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)      433 2023-04-28 05:17:10.000000 refunc-cli-1.3.2/rfctl/delete.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)      456 2023-04-28 05:17:10.000000 refunc-cli-1.3.2/rfctl/delete_url.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)      422 2023-04-28 05:17:10.000000 refunc-cli-1.3.2/rfctl/get.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)      441 2023-04-28 05:17:10.000000 refunc-cli-1.3.2/rfctl/get_url.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)     3203 2023-09-30 08:56:30.000000 refunc-cli-1.3.2/rfctl/init.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)     1458 2023-04-28 05:17:10.000000 refunc-cli-1.3.2/rfctl/init_source.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)     2014 2023-04-28 05:17:10.000000 refunc-cli-1.3.2/rfctl/schema.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)      680 2023-04-28 05:17:10.000000 refunc-cli-1.3.2/rfctl/update_code.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)     1235 2023-09-30 09:36:25.000000 refunc-cli-1.3.2/rfctl/update_config.py
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)       38 2024-05-23 09:21:37.420711 refunc-cli-1.3.2/setup.cfg
+-rw-rw-r--   0 arvin     (1000) arvin     (1000)     1033 2024-05-23 08:38:34.000000 refunc-cli-1.3.2/setup.py
```

### Comparing `refunc-cli-1.3.1/refunc_cli.egg-info/SOURCES.txt` & `refunc-cli-1.3.2/refunc_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `refunc-cli-1.3.1/rfctl/__main__.py` & `refunc-cli-1.3.2/rfctl/__main__.py`

 * *Files identical despite different names*

### Comparing `refunc-cli-1.3.1/rfctl/awslocal.py` & `refunc-cli-1.3.2/rfctl/awslocal.py`

 * *Files identical despite different names*

### Comparing `refunc-cli-1.3.1/rfctl/build.py` & `refunc-cli-1.3.2/rfctl/build.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,19 +26,21 @@
 @click.pass_context
 def build_command(ctx: click.Context, out: str):
     do_build(ctx, out)
 
 
 def do_build(ctx: click.Context, out: str) -> bool:
     funcdef = ctx.obj["funcdef"]
-    build = funcdef["spec"]["build"]
+    build: dict = funcdef["spec"]["build"]
     capabilities = {
         "language": build["language"],
         "dependency_manager": get_dependency_manager(build["language"])
     }
+    envs: dict = build.get("environment", {})
+    os.environ.update(envs)
     with tempfile.TemporaryDirectory() as tmp_dir:
         click.echo("Building function %s/%s in temporary directory %s" % (funcdef["metadata"]["namespace"], funcdef["metadata"]["name"], tmp_dir))
         try:
             params = {
                 "source_dir": build["source"],
                 "artifacts_dir": os.path.join(tmp_dir, "lambda"),
                 "scratch_dir": os.path.join(tmp_dir, "tmp"),
```

### Comparing `refunc-cli-1.3.1/rfctl/client/client.py` & `refunc-cli-1.3.2/rfctl/client/client.py`

 * *Files identical despite different names*

### Comparing `refunc-cli-1.3.1/rfctl/create.py` & `refunc-cli-1.3.2/rfctl/create.py`

 * *Files identical despite different names*

### Comparing `refunc-cli-1.3.1/rfctl/init.py` & `refunc-cli-1.3.2/rfctl/init.py`

 * *Files identical despite different names*

### Comparing `refunc-cli-1.3.1/rfctl/init_source.py` & `refunc-cli-1.3.2/rfctl/init_source.py`

 * *Files identical despite different names*

### Comparing `refunc-cli-1.3.1/rfctl/schema.py` & `refunc-cli-1.3.2/rfctl/schema.py`

 * *Files identical despite different names*

### Comparing `refunc-cli-1.3.1/rfctl/update_code.py` & `refunc-cli-1.3.2/rfctl/update_code.py`

 * *Files identical despite different names*

### Comparing `refunc-cli-1.3.1/rfctl/update_config.py` & `refunc-cli-1.3.2/rfctl/update_config.py`

 * *Files identical despite different names*

### Comparing `refunc-cli-1.3.1/setup.py` & `refunc-cli-1.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import find_packages
 
 os.chdir(os.path.dirname(sys.argv[0]) or ".")
 here = os.path.abspath(os.path.dirname(__file__))
 
 setup_args = dict(
     name='refunc-cli',
-    version='1.3.1',
+    version='1.3.2',
     description='refunc command line tools',
     author='arvin',
     license='MIT',
     url='https://github.com/refunc/refunc-cli',
     author_email='arvintian8@gamil.com',
     packages=find_packages(),
     include_package_data=True,
```

