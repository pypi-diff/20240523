# Comparing `tmp/mask_key-0.2.7.tar.gz` & `tmp/mask_key-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mask_key-0.2.7.tar", last modified: Thu May 23 07:02:01 2024, max compression
+gzip compressed data, was "mask_key-0.2.8.tar", last modified: Thu May 23 07:05:07 2024, max compression
```

## Comparing `mask_key-0.2.7.tar` & `mask_key-0.2.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 07:02:01.612547 mask_key-0.2.7/
--rw-rw-rw-   0        0        0        0 2024-05-23 04:58:08.000000 mask_key-0.2.7/LICENSE
--rw-rw-rw-   0        0        0       34 2024-05-23 04:58:08.000000 mask_key-0.2.7/MANIFEST.in
--rw-rw-rw-   0        0        0      528 2024-05-23 07:02:01.610281 mask_key-0.2.7/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-05-23 04:58:08.000000 mask_key-0.2.7/README.md
-drwxrwxrwx   0        0        0        0 2024-05-23 07:02:01.581288 mask_key-0.2.7/mask_key/
--rw-rw-rw-   0        0        0       47 2024-05-23 04:58:08.000000 mask_key-0.2.7/mask_key/__init__.py
--rw-rw-rw-   0        0        0      373 2024-05-23 06:17:22.000000 mask_key-0.2.7/mask_key/api.py
--rw-rw-rw-   0        0        0     1237 2024-05-23 06:51:24.000000 mask_key-0.2.7/mask_key/main.py
--rw-rw-rw-   0        0        0       73 2024-05-23 06:18:02.000000 mask_key-0.2.7/mask_key/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-23 07:02:01.609272 mask_key-0.2.7/mask_key.egg-info/
--rw-rw-rw-   0        0        0      528 2024-05-23 07:02:01.000000 mask_key-0.2.7/mask_key.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      304 2024-05-23 07:02:01.000000 mask_key-0.2.7/mask_key.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 07:02:01.000000 mask_key-0.2.7/mask_key.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2024-05-23 07:02:01.000000 mask_key-0.2.7/mask_key.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       23 2024-05-23 07:02:01.000000 mask_key-0.2.7/mask_key.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-23 07:02:01.000000 mask_key-0.2.7/mask_key.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-23 07:02:01.612547 mask_key-0.2.7/setup.cfg
--rw-rw-rw-   0        0        0     1668 2024-05-23 07:01:48.000000 mask_key-0.2.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 07:05:07.707563 mask_key-0.2.8/
+-rw-rw-rw-   0        0        0        0 2024-05-23 04:58:08.000000 mask_key-0.2.8/LICENSE
+-rw-rw-rw-   0        0        0       34 2024-05-23 04:58:08.000000 mask_key-0.2.8/MANIFEST.in
+-rw-rw-rw-   0        0        0      473 2024-05-23 07:05:07.707563 mask_key-0.2.8/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-05-23 04:58:08.000000 mask_key-0.2.8/README.md
+drwxrwxrwx   0        0        0        0 2024-05-23 07:05:07.671009 mask_key-0.2.8/mask_key/
+-rw-rw-rw-   0        0        0       47 2024-05-23 04:58:08.000000 mask_key-0.2.8/mask_key/__init__.py
+-rw-rw-rw-   0        0        0      373 2024-05-23 06:17:22.000000 mask_key-0.2.8/mask_key/api.py
+-rw-rw-rw-   0        0        0     1237 2024-05-23 06:51:24.000000 mask_key-0.2.8/mask_key/main.py
+-rw-rw-rw-   0        0        0       73 2024-05-23 06:18:02.000000 mask_key-0.2.8/mask_key/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-23 07:05:07.705570 mask_key-0.2.8/mask_key.egg-info/
+-rw-rw-rw-   0        0        0      473 2024-05-23 07:05:07.000000 mask_key-0.2.8/mask_key.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      304 2024-05-23 07:05:07.000000 mask_key-0.2.8/mask_key.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 07:05:07.000000 mask_key-0.2.8/mask_key.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2024-05-23 07:05:07.000000 mask_key-0.2.8/mask_key.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       23 2024-05-23 07:05:07.000000 mask_key-0.2.8/mask_key.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-23 07:05:07.000000 mask_key-0.2.8/mask_key.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-23 07:05:07.708563 mask_key-0.2.8/setup.cfg
+-rw-rw-rw-   0        0        0     1668 2024-05-23 07:05:02.000000 mask_key-0.2.8/setup.py
```

### Comparing `mask_key-0.2.7/mask_key/main.py` & `mask_key-0.2.8/mask_key/main.py`

 * *Files identical despite different names*

### Comparing `mask_key-0.2.7/setup.py` & `mask_key-0.2.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
             print("Please run `mask-key` manually after installation to complete setup.")
         except Exception as e:
             print(f"Unexpected error during post install: {e}")
             print("Please run `mask-key` manually after installation to complete setup.")
 
 setup(
     name='mask_key',
-    version='0.2.7',
+    version='0.2.8',
     author='krishna agarwal',
     author_email='krishnacool781@gmail.com',
     description='A Python package to generate mask keys.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/krishnaagarwal781/mask_keys_server',
     packages=find_packages(),
```

