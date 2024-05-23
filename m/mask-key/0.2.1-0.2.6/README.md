# Comparing `tmp/mask_key-0.2.1.tar.gz` & `tmp/mask_key-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mask_key-0.2.1.tar", last modified: Thu May 23 06:32:24 2024, max compression
+gzip compressed data, was "mask_key-0.2.6.tar", last modified: Thu May 23 06:58:05 2024, max compression
```

## Comparing `mask_key-0.2.1.tar` & `mask_key-0.2.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 06:32:24.776279 mask_key-0.2.1/
--rw-rw-rw-   0        0        0        0 2024-05-23 04:58:08.000000 mask_key-0.2.1/LICENSE
--rw-rw-rw-   0        0        0       34 2024-05-23 04:58:08.000000 mask_key-0.2.1/MANIFEST.in
--rw-rw-rw-   0        0        0      528 2024-05-23 06:32:24.775289 mask_key-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-05-23 04:58:08.000000 mask_key-0.2.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-23 06:32:24.753045 mask_key-0.2.1/mask_key/
--rw-rw-rw-   0        0        0       47 2024-05-23 04:58:08.000000 mask_key-0.2.1/mask_key/__init__.py
--rw-rw-rw-   0        0        0      373 2024-05-23 06:17:22.000000 mask_key-0.2.1/mask_key/api.py
--rw-rw-rw-   0        0        0     1237 2024-05-23 06:17:34.000000 mask_key-0.2.1/mask_key/main.py
--rw-rw-rw-   0        0        0       73 2024-05-23 06:18:02.000000 mask_key-0.2.1/mask_key/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-23 06:32:24.772852 mask_key-0.2.1/mask_key.egg-info/
--rw-rw-rw-   0        0        0      528 2024-05-23 06:32:24.000000 mask_key-0.2.1/mask_key.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      304 2024-05-23 06:32:24.000000 mask_key-0.2.1/mask_key.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 06:32:24.000000 mask_key-0.2.1/mask_key.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2024-05-23 06:32:24.000000 mask_key-0.2.1/mask_key.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       23 2024-05-23 06:32:24.000000 mask_key-0.2.1/mask_key.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-23 06:32:24.000000 mask_key-0.2.1/mask_key.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-23 06:32:24.776279 mask_key-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1085 2024-05-23 06:30:37.000000 mask_key-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 06:58:05.496349 mask_key-0.2.6/
+-rw-rw-rw-   0        0        0        0 2024-05-23 04:58:08.000000 mask_key-0.2.6/LICENSE
+-rw-rw-rw-   0        0        0       34 2024-05-23 04:58:08.000000 mask_key-0.2.6/MANIFEST.in
+-rw-rw-rw-   0        0        0      473 2024-05-23 06:58:05.495340 mask_key-0.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-05-23 04:58:08.000000 mask_key-0.2.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-23 06:58:05.461829 mask_key-0.2.6/mask_key/
+-rw-rw-rw-   0        0        0       47 2024-05-23 04:58:08.000000 mask_key-0.2.6/mask_key/__init__.py
+-rw-rw-rw-   0        0        0      373 2024-05-23 06:17:22.000000 mask_key-0.2.6/mask_key/api.py
+-rw-rw-rw-   0        0        0     1237 2024-05-23 06:51:24.000000 mask_key-0.2.6/mask_key/main.py
+-rw-rw-rw-   0        0        0       73 2024-05-23 06:18:02.000000 mask_key-0.2.6/mask_key/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-23 06:58:05.493998 mask_key-0.2.6/mask_key.egg-info/
+-rw-rw-rw-   0        0        0      473 2024-05-23 06:58:05.000000 mask_key-0.2.6/mask_key.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      304 2024-05-23 06:58:05.000000 mask_key-0.2.6/mask_key.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 06:58:05.000000 mask_key-0.2.6/mask_key.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2024-05-23 06:58:05.000000 mask_key-0.2.6/mask_key.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       23 2024-05-23 06:58:05.000000 mask_key-0.2.6/mask_key.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-23 06:58:05.000000 mask_key-0.2.6/mask_key.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-23 06:58:05.496349 mask_key-0.2.6/setup.cfg
+-rw-rw-rw-   0        0        0     1320 2024-05-23 06:57:50.000000 mask_key-0.2.6/setup.py
```

### Comparing `mask_key-0.2.1/mask_key/main.py` & `mask_key-0.2.6/mask_key/main.py`

 * *Files identical despite different names*

### Comparing `mask_key-0.2.1/setup.py` & `mask_key-0.2.6/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 import subprocess
+import sys
 
 class PostInstallCommand(install):
     def run(self):
         install.run(self)
-        subprocess.run(["mask-key"])
+        # Run your script here if needed
+        try:
+            subprocess.run([sys.executable, '-m', 'mask_key.main'], check=True)
+        except subprocess.CalledProcessError as e:
+            print(f"Error during post install script execution: {e}")
 
 setup(
     name='mask_key',
-    version='0.2.1',
+    version='0.2.6',
     author='krishna agarwal',
     author_email='krishnacool781@gmail.com',
     description='A Python package to generate mask keys.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/krishnaagarwal781/mask_keys_server',
     packages=find_packages(),
@@ -30,9 +35,9 @@
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
     python_requires='>=3.6',
     cmdclass={
         'install': PostInstallCommand,
-    }
+    },
 )
```

