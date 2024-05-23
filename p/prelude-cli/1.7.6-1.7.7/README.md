# Comparing `tmp/prelude_cli-1.7.6.tar.gz` & `tmp/prelude_cli-1.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prelude_cli-1.7.6.tar", last modified: Fri May  3 19:21:57 2024, max compression
+gzip compressed data, was "prelude_cli-1.7.7.tar", last modified: Thu May 23 12:53:56 2024, max compression
```

## Comparing `prelude_cli-1.7.6.tar` & `prelude_cli-1.7.7.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2024-05-03 19:21:57.908796 prelude_cli-1.7.6/
--rw-r--r--   0 pack       (501) staff       (20)     1069 2023-01-24 13:01:01.000000 prelude_cli-1.7.6/LICENSE
--rw-r--r--   0 pack       (501) staff       (20)       31 2023-01-24 13:01:01.000000 prelude_cli-1.7.6/MANIFEST.in
--rw-r--r--   0 pack       (501) staff       (20)      962 2024-05-03 19:21:57.908696 prelude_cli-1.7.6/PKG-INFO
--rw-r--r--   0 pack       (501) staff       (20)      391 2023-03-01 15:58:44.000000 prelude_cli-1.7.6/README.md
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2024-05-03 19:21:57.902797 prelude_cli-1.7.6/prelude_cli/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude_cli-1.7.6/prelude_cli/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)     1014 2024-04-03 22:19:39.000000 prelude_cli-1.7.6/prelude_cli/cli.py
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-12-08 16:31:30.000000 prelude_cli-1.7.6/prelude_cli/spinner.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2024-05-03 19:21:57.904265 prelude_cli-1.7.6/prelude_cli/templates/
--rw-r--r--   0 pack       (501) staff       (20)     1120 2024-01-05 14:14:44.000000 prelude_cli-1.7.6/prelude_cli/templates/README.md
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude_cli-1.7.6/prelude_cli/templates/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)      261 2024-01-05 14:14:44.000000 prelude_cli-1.7.6/prelude_cli/templates/template.go
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2024-05-03 19:21:57.907290 prelude_cli-1.7.6/prelude_cli/views/
--rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude_cli-1.7.6/prelude_cli/views/__init__.py
--rw-r--r--   0 pack       (501) staff       (20)    10043 2024-04-03 22:19:39.000000 prelude_cli-1.7.6/prelude_cli/views/build.py
--rw-r--r--   0 pack       (501) staff       (20)      552 2023-02-08 14:42:44.000000 prelude_cli-1.7.6/prelude_cli/views/configure.py
--rw-r--r--   0 pack       (501) staff       (20)    10645 2024-05-03 19:12:34.000000 prelude_cli-1.7.6/prelude_cli/views/detect.py
--rw-r--r--   0 pack       (501) staff       (20)     2543 2024-04-11 19:46:08.000000 prelude_cli-1.7.6/prelude_cli/views/generate.py
--rw-r--r--   0 pack       (501) staff       (20)     8568 2024-04-17 18:29:22.000000 prelude_cli-1.7.6/prelude_cli/views/iam.py
--rw-r--r--   0 pack       (501) staff       (20)     4771 2024-04-17 18:29:22.000000 prelude_cli-1.7.6/prelude_cli/views/partner.py
--rw-r--r--   0 pack       (501) staff       (20)      662 2024-04-03 22:19:39.000000 prelude_cli-1.7.6/prelude_cli/views/shared.py
-drwxr-xr-x   0 pack       (501) staff       (20)        0 2024-05-03 19:21:57.908345 prelude_cli-1.7.6/prelude_cli.egg-info/
--rw-r--r--   0 pack       (501) staff       (20)      962 2024-05-03 19:21:57.000000 prelude_cli-1.7.6/prelude_cli.egg-info/PKG-INFO
--rw-r--r--   0 pack       (501) staff       (20)      660 2024-05-03 19:21:57.000000 prelude_cli-1.7.6/prelude_cli.egg-info/SOURCES.txt
--rw-r--r--   0 pack       (501) staff       (20)        1 2024-05-03 19:21:57.000000 prelude_cli-1.7.6/prelude_cli.egg-info/dependency_links.txt
--rw-r--r--   0 pack       (501) staff       (20)       48 2024-05-03 19:21:57.000000 prelude_cli-1.7.6/prelude_cli.egg-info/entry_points.txt
--rw-r--r--   0 pack       (501) staff       (20)       55 2024-05-03 19:21:57.000000 prelude_cli-1.7.6/prelude_cli.egg-info/requires.txt
--rw-r--r--   0 pack       (501) staff       (20)       12 2024-05-03 19:21:57.000000 prelude_cli-1.7.6/prelude_cli.egg-info/top_level.txt
--rw-r--r--   0 pack       (501) staff       (20)      103 2023-01-24 13:01:01.000000 prelude_cli-1.7.6/pyproject.toml
--rw-r--r--   0 pack       (501) staff       (20)      688 2024-05-03 19:21:57.909099 prelude_cli-1.7.6/setup.cfg
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2024-05-23 12:53:56.857857 prelude_cli-1.7.7/
+-rw-r--r--   0 pack       (501) staff       (20)     1069 2023-01-24 13:01:01.000000 prelude_cli-1.7.7/LICENSE
+-rw-r--r--   0 pack       (501) staff       (20)       31 2023-01-24 13:01:01.000000 prelude_cli-1.7.7/MANIFEST.in
+-rw-r--r--   0 pack       (501) staff       (20)      962 2024-05-23 12:53:56.857768 prelude_cli-1.7.7/PKG-INFO
+-rw-r--r--   0 pack       (501) staff       (20)      391 2023-03-01 15:58:44.000000 prelude_cli-1.7.7/README.md
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2024-05-23 12:53:56.851456 prelude_cli-1.7.7/prelude_cli/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude_cli-1.7.7/prelude_cli/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)     1014 2024-04-03 22:19:39.000000 prelude_cli-1.7.7/prelude_cli/cli.py
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-12-08 16:31:30.000000 prelude_cli-1.7.7/prelude_cli/spinner.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2024-05-23 12:53:56.853224 prelude_cli-1.7.7/prelude_cli/templates/
+-rw-r--r--   0 pack       (501) staff       (20)     1120 2024-01-05 14:14:44.000000 prelude_cli-1.7.7/prelude_cli/templates/README.md
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude_cli-1.7.7/prelude_cli/templates/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)      261 2024-01-05 14:14:44.000000 prelude_cli-1.7.7/prelude_cli/templates/template.go
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2024-05-23 12:53:56.856132 prelude_cli-1.7.7/prelude_cli/views/
+-rw-r--r--   0 pack       (501) staff       (20)        0 2023-01-24 13:01:01.000000 prelude_cli-1.7.7/prelude_cli/views/__init__.py
+-rw-r--r--   0 pack       (501) staff       (20)    10043 2024-04-03 22:19:39.000000 prelude_cli-1.7.7/prelude_cli/views/build.py
+-rw-r--r--   0 pack       (501) staff       (20)      552 2023-02-08 14:42:44.000000 prelude_cli-1.7.7/prelude_cli/views/configure.py
+-rw-r--r--   0 pack       (501) staff       (20)    10645 2024-05-03 19:12:34.000000 prelude_cli-1.7.7/prelude_cli/views/detect.py
+-rw-r--r--   0 pack       (501) staff       (20)     2543 2024-04-11 19:46:08.000000 prelude_cli-1.7.7/prelude_cli/views/generate.py
+-rw-r--r--   0 pack       (501) staff       (20)     8525 2024-05-22 22:38:32.000000 prelude_cli-1.7.7/prelude_cli/views/iam.py
+-rw-r--r--   0 pack       (501) staff       (20)     4771 2024-04-17 18:29:22.000000 prelude_cli-1.7.7/prelude_cli/views/partner.py
+-rw-r--r--   0 pack       (501) staff       (20)      662 2024-04-03 22:19:39.000000 prelude_cli-1.7.7/prelude_cli/views/shared.py
+drwxr-xr-x   0 pack       (501) staff       (20)        0 2024-05-23 12:53:56.857370 prelude_cli-1.7.7/prelude_cli.egg-info/
+-rw-r--r--   0 pack       (501) staff       (20)      962 2024-05-23 12:53:56.000000 prelude_cli-1.7.7/prelude_cli.egg-info/PKG-INFO
+-rw-r--r--   0 pack       (501) staff       (20)      660 2024-05-23 12:53:56.000000 prelude_cli-1.7.7/prelude_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 pack       (501) staff       (20)        1 2024-05-23 12:53:56.000000 prelude_cli-1.7.7/prelude_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 pack       (501) staff       (20)       48 2024-05-23 12:53:56.000000 prelude_cli-1.7.7/prelude_cli.egg-info/entry_points.txt
+-rw-r--r--   0 pack       (501) staff       (20)       55 2024-05-23 12:53:56.000000 prelude_cli-1.7.7/prelude_cli.egg-info/requires.txt
+-rw-r--r--   0 pack       (501) staff       (20)       12 2024-05-23 12:53:56.000000 prelude_cli-1.7.7/prelude_cli.egg-info/top_level.txt
+-rw-r--r--   0 pack       (501) staff       (20)      103 2023-01-24 13:01:01.000000 prelude_cli-1.7.7/pyproject.toml
+-rw-r--r--   0 pack       (501) staff       (20)      688 2024-05-23 12:53:56.858116 prelude_cli-1.7.7/setup.cfg
```

### Comparing `prelude_cli-1.7.6/LICENSE` & `prelude_cli-1.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `prelude_cli-1.7.6/PKG-INFO` & `prelude_cli-1.7.7/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: prelude-cli
-Version: 1.7.6
+Version: 1.7.7
 Summary: For interacting with the Prelude SDK
 Home-page: https://github.com/preludeorg
 Author: Prelude Research
 Author-email: support@preludesecurity.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: prelude-sdk==1.7.3
+Requires-Dist: prelude-sdk==1.7.4
 Requires-Dist: click>8
 Requires-Dist: rich
 Requires-Dist: python-dateutil
 Requires-Dist: pyyaml
 
 # Prelude CLI
```

### Comparing `prelude_cli-1.7.6/prelude_cli/cli.py` & `prelude_cli-1.7.7/prelude_cli/cli.py`

 * *Files identical despite different names*

### Comparing `prelude_cli-1.7.6/prelude_cli/templates/README.md` & `prelude_cli-1.7.7/prelude_cli/templates/README.md`

 * *Files identical despite different names*

### Comparing `prelude_cli-1.7.6/prelude_cli/views/build.py` & `prelude_cli-1.7.7/prelude_cli/views/build.py`

 * *Files identical despite different names*

### Comparing `prelude_cli-1.7.6/prelude_cli/views/configure.py` & `prelude_cli-1.7.7/prelude_cli/views/configure.py`

 * *Files identical despite different names*

### Comparing `prelude_cli-1.7.6/prelude_cli/views/detect.py` & `prelude_cli-1.7.7/prelude_cli/views/detect.py`

 * *Files identical despite different names*

### Comparing `prelude_cli-1.7.6/prelude_cli/views/generate.py` & `prelude_cli-1.7.7/prelude_cli/views/generate.py`

 * *Files identical despite different names*

### Comparing `prelude_cli-1.7.6/prelude_cli/views/iam.py` & `prelude_cli-1.7.7/prelude_cli/views/iam.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,19 +18,19 @@
 @iam.command('create-account')
 @click.pass_obj
 @handle_api_error
 @click.confirmation_option(prompt='Overwrite local account credentials for selected profile?')
 def register_account(controller):
     """ Register a new account """
     email = click.prompt('Enter your email')
+    company = click.prompt('Enter your associated company')
     name = click.prompt('(Optional) Enter your name', default='', show_default=False)
-    company = click.prompt('(Optional) Enter your associated company', default='', show_default=False)
     slug = click.prompt('(Optional) Enter an unique human-readable identifier for your account', default='', show_default=False)
     with Spinner(description='Creating new account'):
-        data = controller.new_account(user_email=email, user_name=name, company=company, slug=slug)
+        data = controller.new_account(user_email=email, company=company, user_name=name, slug=slug)
     print_json(data=data)
     print("\nCheck your email to verify your account.\n")
 
 
 @iam.command('update-account')
 @click.option('-m', '--mode',
               help='provide a mode',
```

### Comparing `prelude_cli-1.7.6/prelude_cli/views/partner.py` & `prelude_cli-1.7.7/prelude_cli/views/partner.py`

 * *Files identical despite different names*

### Comparing `prelude_cli-1.7.6/prelude_cli/views/shared.py` & `prelude_cli-1.7.7/prelude_cli/views/shared.py`

 * *Files identical despite different names*

### Comparing `prelude_cli-1.7.6/prelude_cli.egg-info/PKG-INFO` & `prelude_cli-1.7.7/prelude_cli.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: prelude-cli
-Version: 1.7.6
+Version: 1.7.7
 Summary: For interacting with the Prelude SDK
 Home-page: https://github.com/preludeorg
 Author: Prelude Research
 Author-email: support@preludesecurity.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: prelude-sdk==1.7.3
+Requires-Dist: prelude-sdk==1.7.4
 Requires-Dist: click>8
 Requires-Dist: rich
 Requires-Dist: python-dateutil
 Requires-Dist: pyyaml
 
 # Prelude CLI
```

### Comparing `prelude_cli-1.7.6/prelude_cli.egg-info/SOURCES.txt` & `prelude_cli-1.7.7/prelude_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `prelude_cli-1.7.6/setup.cfg` & `prelude_cli-1.7.7/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = prelude-cli
-version = 1.7.6
+version = 1.7.7
 author = Prelude Research
 author_email = support@preludesecurity.com
 description = For interacting with the Prelude SDK
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/preludeorg
 classifiers = 
@@ -13,15 +13,15 @@
 	Operating System :: OS Independent
 
 [options]
 packages = find:
 include_package_data = True
 python_requires = >=3.8
 install_requires = 
-	prelude-sdk == 1.7.3
+	prelude-sdk == 1.7.4
 	click > 8
 	rich
 	python-dateutil
 	pyyaml
 
 [options.entry_points]
 console_scripts =
```

