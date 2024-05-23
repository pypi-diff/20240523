# Comparing `tmp/mask_key-0.2.0.tar.gz` & `tmp/mask_key-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mask_key-0.2.0.tar", last modified: Thu May 23 04:51:46 2024, max compression
+gzip compressed data, was "mask_key-0.2.1.tar", last modified: Thu May 23 06:32:24 2024, max compression
```

## Comparing `mask_key-0.2.0.tar` & `mask_key-0.2.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 04:51:46.162118 mask_key-0.2.0/
--rw-rw-rw-   0        0        0        0 2024-05-23 03:49:20.000000 mask_key-0.2.0/LICENSE
--rw-rw-rw-   0        0        0       34 2024-05-23 04:03:50.000000 mask_key-0.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0      528 2024-05-23 04:51:46.159764 mask_key-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-05-23 03:49:07.000000 mask_key-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-23 04:51:46.118320 mask_key-0.2.0/mask_key/
--rw-rw-rw-   0        0        0       47 2024-05-23 03:48:11.000000 mask_key-0.2.0/mask_key/__init__.py
--rw-rw-rw-   0        0        0      392 2024-05-23 04:47:54.000000 mask_key-0.2.0/mask_key/api.py
--rw-rw-rw-   0        0        0     1174 2024-05-23 03:51:09.000000 mask_key-0.2.0/mask_key/main.py
--rw-rw-rw-   0        0        0       94 2024-05-23 03:50:36.000000 mask_key-0.2.0/mask_key/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-23 04:51:46.157768 mask_key-0.2.0/mask_key.egg-info/
--rw-rw-rw-   0        0        0      528 2024-05-23 04:51:46.000000 mask_key-0.2.0/mask_key.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      304 2024-05-23 04:51:46.000000 mask_key-0.2.0/mask_key.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 04:51:46.000000 mask_key-0.2.0/mask_key.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2024-05-23 04:51:46.000000 mask_key-0.2.0/mask_key.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       23 2024-05-23 04:51:46.000000 mask_key-0.2.0/mask_key.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-23 04:51:46.000000 mask_key-0.2.0/mask_key.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-23 04:51:46.163474 mask_key-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      832 2024-05-23 04:51:40.000000 mask_key-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 06:32:24.776279 mask_key-0.2.1/
+-rw-rw-rw-   0        0        0        0 2024-05-23 04:58:08.000000 mask_key-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0       34 2024-05-23 04:58:08.000000 mask_key-0.2.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      528 2024-05-23 06:32:24.775289 mask_key-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-05-23 04:58:08.000000 mask_key-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-23 06:32:24.753045 mask_key-0.2.1/mask_key/
+-rw-rw-rw-   0        0        0       47 2024-05-23 04:58:08.000000 mask_key-0.2.1/mask_key/__init__.py
+-rw-rw-rw-   0        0        0      373 2024-05-23 06:17:22.000000 mask_key-0.2.1/mask_key/api.py
+-rw-rw-rw-   0        0        0     1237 2024-05-23 06:17:34.000000 mask_key-0.2.1/mask_key/main.py
+-rw-rw-rw-   0        0        0       73 2024-05-23 06:18:02.000000 mask_key-0.2.1/mask_key/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-23 06:32:24.772852 mask_key-0.2.1/mask_key.egg-info/
+-rw-rw-rw-   0        0        0      528 2024-05-23 06:32:24.000000 mask_key-0.2.1/mask_key.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      304 2024-05-23 06:32:24.000000 mask_key-0.2.1/mask_key.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 06:32:24.000000 mask_key-0.2.1/mask_key.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2024-05-23 06:32:24.000000 mask_key-0.2.1/mask_key.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       23 2024-05-23 06:32:24.000000 mask_key-0.2.1/mask_key.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-23 06:32:24.000000 mask_key-0.2.1/mask_key.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-23 06:32:24.776279 mask_key-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1085 2024-05-23 06:30:37.000000 mask_key-0.2.1/setup.py
```

### Comparing `mask_key-0.2.0/PKG-INFO` & `mask_key-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mask_key
-Version: 0.2.0
+Version: 0.2.1
 Summary: A Python package to generate mask keys.
 Home-page: https://github.com/krishnaagarwal781/mask_keys_server
 Author: krishna agarwal
 Author-email: krishnacool781@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mask_key-0.2.0/mask_key/main.py` & `mask_key-0.2.1/mask_key/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# mask_key/main.py
 import json
 import os
 from dotenv import load_dotenv, set_key
 from .api import generate_keys
 from .utils import check_env_exists
 
 def ask_questions():
@@ -14,27 +13,26 @@
     return user_data
 
 def save_to_json(data, filename='user_data.json'):
     with open(filename, 'w') as f:
         json.dump(data, f)
 
 def main():
-    if check_env_exists():
-        print(".env file already exists.")
-        return
-
-    user_data = ask_questions()
-    save_to_json(user_data)
-
-    response = generate_keys(user_data)
-    
-    if response:
-        app_key, company_key = response['application_key'], response['company_key']
+    if not check_env_exists():
+        user_data = ask_questions()
+        save_to_json(user_data)
+
+        response = generate_keys(user_data)
+        
+        if response:
+            app_key, company_key = response['application_key'], response['company_key']
+        else:
+            app_key, company_key = '', ''
+            print("No response from server. Keys will be empty.")
+
+        load_dotenv()
+        set_key('.env', 'APPLICATION_KEY', app_key)
+        set_key('.env', 'COMPANY_KEY', company_key)
+        
+        print("Keys have been saved to .env file.")
     else:
-        app_key, company_key = '', ''
-        print("No response from server. Keys will be empty.")
-
-    load_dotenv()
-    set_key('.env', 'APPLICATION_KEY', app_key)
-    set_key('.env', 'COMPANY_KEY', company_key)
-    
-    print("Keys have been saved to .env file.")
+        print(".env file already exists. No need to run the setup again.")
```

### Comparing `mask_key-0.2.0/mask_key.egg-info/PKG-INFO` & `mask_key-0.2.1/mask_key.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mask_key
-Version: 0.2.0
+Version: 0.2.1
 Summary: A Python package to generate mask keys.
 Home-page: https://github.com/krishnaagarwal781/mask_keys_server
 Author: krishna agarwal
 Author-email: krishnacool781@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mask_key-0.2.0/setup.py` & `mask_key-0.2.1/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,19 @@
 from setuptools import setup, find_packages
+from setuptools.command.install import install
+import subprocess
+
+class PostInstallCommand(install):
+    def run(self):
+        install.run(self)
+        subprocess.run(["mask-key"])
 
 setup(
     name='mask_key',
-    version='0.2.0',
+    version='0.2.1',
     author='krishna agarwal',
     author_email='krishnacool781@gmail.com',
     description='A Python package to generate mask keys.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/krishnaagarwal781/mask_keys_server',
     packages=find_packages(),
@@ -21,8 +28,11 @@
     },
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
     python_requires='>=3.6',
+    cmdclass={
+        'install': PostInstallCommand,
+    }
 )
```

