# Comparing `tmp/cdproxy-0.1.0.tar.gz` & `tmp/cdproxy-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdproxy-0.1.0.tar", last modified: Thu May 23 07:55:49 2024, max compression
+gzip compressed data, was "cdproxy-1.0.tar", last modified: Thu May 23 08:05:04 2024, max compression
```

## Comparing `cdproxy-0.1.0.tar` & `cdproxy-1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-23 07:55:49.136416 cdproxy-0.1.0/
--rw-rw-r--   0 adam      (1001) adam      (1002)        3 2024-05-23 07:51:54.000000 cdproxy-0.1.0/LICENSE
--rw-r--r--   0 adam      (1001) adam      (1002)      823 2024-05-23 07:55:49.136416 cdproxy-0.1.0/PKG-INFO
--rw-rw-r--   0 adam      (1001) adam      (1002)      287 2024-05-23 07:45:42.000000 cdproxy-0.1.0/README.md
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-23 07:55:49.128416 cdproxy-0.1.0/cdprox/
--rw-rw-r--   0 adam      (1001) adam      (1002)        0 2024-05-22 17:27:00.000000 cdproxy-0.1.0/cdprox/__init__.py
--rw-rw-r--   0 adam      (1001) adam      (1002)      443 2024-05-22 17:33:54.000000 cdproxy-0.1.0/cdprox/config.py
--rw-rw-r--   0 adam      (1001) adam      (1002)     1926 2024-05-23 07:49:19.000000 cdproxy-0.1.0/cdprox/main.py
--rw-rw-r--   0 adam      (1001) adam      (1002)     3434 2024-05-23 07:48:35.000000 cdproxy-0.1.0/cdprox/utils.py
-drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-23 07:55:49.132416 cdproxy-0.1.0/cdproxy.egg-info/
--rw-r--r--   0 adam      (1001) adam      (1002)      823 2024-05-23 07:55:49.000000 cdproxy-0.1.0/cdproxy.egg-info/PKG-INFO
--rw-rw-r--   0 adam      (1001) adam      (1002)      281 2024-05-23 07:55:49.000000 cdproxy-0.1.0/cdproxy.egg-info/SOURCES.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)        1 2024-05-23 07:55:49.000000 cdproxy-0.1.0/cdproxy.egg-info/dependency_links.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       45 2024-05-23 07:55:49.000000 cdproxy-0.1.0/cdproxy.egg-info/entry_points.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       19 2024-05-23 07:55:49.000000 cdproxy-0.1.0/cdproxy.egg-info/requires.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)        7 2024-05-23 07:55:49.000000 cdproxy-0.1.0/cdproxy.egg-info/top_level.txt
--rw-rw-r--   0 adam      (1001) adam      (1002)       38 2024-05-23 07:55:49.136416 cdproxy-0.1.0/setup.cfg
--rw-rw-r--   0 adam      (1001) adam      (1002)      865 2024-05-23 07:52:45.000000 cdproxy-0.1.0/setup.py
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-23 08:05:04.619206 cdproxy-1.0/
+-rw-rw-r--   0 adam      (1001) adam      (1002)        3 2024-05-23 07:51:54.000000 cdproxy-1.0/LICENSE
+-rw-r--r--   0 adam      (1001) adam      (1002)      821 2024-05-23 08:05:04.615206 cdproxy-1.0/PKG-INFO
+-rw-rw-r--   0 adam      (1001) adam      (1002)      287 2024-05-23 07:45:42.000000 cdproxy-1.0/README.md
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-23 08:05:04.611206 cdproxy-1.0/cdprox/
+-rw-rw-r--   0 adam      (1001) adam      (1002)        0 2024-05-22 17:27:00.000000 cdproxy-1.0/cdprox/__init__.py
+-rw-rw-r--   0 adam      (1001) adam      (1002)      443 2024-05-22 17:33:54.000000 cdproxy-1.0/cdprox/config.py
+-rw-rw-r--   0 adam      (1001) adam      (1002)     1926 2024-05-23 07:49:19.000000 cdproxy-1.0/cdprox/main.py
+-rw-rw-r--   0 adam      (1001) adam      (1002)     3434 2024-05-23 07:48:35.000000 cdproxy-1.0/cdprox/utils.py
+drwxrwxr-x   0 adam      (1001) adam      (1002)        0 2024-05-23 08:05:04.615206 cdproxy-1.0/cdproxy.egg-info/
+-rw-r--r--   0 adam      (1001) adam      (1002)      821 2024-05-23 08:05:04.000000 cdproxy-1.0/cdproxy.egg-info/PKG-INFO
+-rw-rw-r--   0 adam      (1001) adam      (1002)      281 2024-05-23 08:05:04.000000 cdproxy-1.0/cdproxy.egg-info/SOURCES.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)        1 2024-05-23 08:05:04.000000 cdproxy-1.0/cdproxy.egg-info/dependency_links.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       44 2024-05-23 08:05:04.000000 cdproxy-1.0/cdproxy.egg-info/entry_points.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       19 2024-05-23 08:05:04.000000 cdproxy-1.0/cdproxy.egg-info/requires.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)        7 2024-05-23 08:05:04.000000 cdproxy-1.0/cdproxy.egg-info/top_level.txt
+-rw-rw-r--   0 adam      (1001) adam      (1002)       38 2024-05-23 08:05:04.619206 cdproxy-1.0/setup.cfg
+-rw-rw-r--   0 adam      (1001) adam      (1002)      862 2024-05-23 08:04:48.000000 cdproxy-1.0/setup.py
```

### Comparing `cdproxy-0.1.0/PKG-INFO` & `cdproxy-1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdproxy
-Version: 0.1.0
+Version: 1.0
 Summary: A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.
 Home-page: https://github.com/yourusername/cdproxy
 Author: Piotr Tamu (Thriveroute)
 Author-email: your.email@example.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cdproxy-0.1.0/cdprox/main.py` & `cdproxy-1.0/cdprox/main.py`

 * *Files identical despite different names*

### Comparing `cdproxy-0.1.0/cdprox/utils.py` & `cdproxy-1.0/cdprox/utils.py`

 * *Files identical despite different names*

### Comparing `cdproxy-0.1.0/cdproxy.egg-info/PKG-INFO` & `cdproxy-1.0/cdproxy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdproxy
-Version: 0.1.0
+Version: 1.0
 Summary: A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.
 Home-page: https://github.com/yourusername/cdproxy
 Author: Piotr Tamu (Thriveroute)
 Author-email: your.email@example.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `cdproxy-0.1.0/setup.py` & `cdproxy-1.0/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='cdproxy',
-    version='0.1.0',
+    version='1.0',
     author='Piotr Tamu (Thriveroute)',
     author_email='your.email@example.com',
     description='A tool to manage Caddy reverse proxy configurations with Cloudflare DNS.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/yourusername/cdproxy',  # Update with your GitHub repository URL
     packages=find_packages(),
@@ -18,11 +18,11 @@
     python_requires='>=3.11',
     install_requires=[
         'requests',
         'dnspython',
     ],
     entry_points={
         'console_scripts': [
-            'cdprox=cdproxy.main:main',
+            'cdprox=cdprox.main:main',
         ],
     },
 )
```

