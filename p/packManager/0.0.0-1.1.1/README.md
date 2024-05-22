# Comparing `tmp/packmanager-0.0.0.tar.gz` & `tmp/packmanager-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "packmanager-0.0.0.tar", last modified: Wed May 22 10:40:48 2024, max compression
+gzip compressed data, was "packmanager-1.1.1.tar", last modified: Wed May 22 22:37:04 2024, max compression
```

## Comparing `packmanager-0.0.0.tar` & `packmanager-1.1.1.tar`

### file list

```diff
@@ -1,15 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 10:40:48.614959 packmanager-0.0.0/
--rw-rw-rw-   0        0        0       85 2024-05-22 10:18:56.000000 packmanager-0.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0       58 2024-05-22 10:40:48.613959 packmanager-0.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      327 2024-05-22 10:00:43.000000 packmanager-0.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-22 10:40:48.601957 packmanager-0.0.0/packManager/
--rw-rw-rw-   0        0        0     1091 2024-05-22 08:35:44.000000 packmanager-0.0.0/packManager/LISENCE
--rw-rw-rw-   0        0        0     1505 2024-05-22 10:33:49.000000 packmanager-0.0.0/packManager/__init__.py
--rw-rw-rw-   0        0        0      890 2024-05-22 10:16:10.000000 packmanager-0.0.0/packManager/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-22 10:40:48.612959 packmanager-0.0.0/packManager.egg-info/
--rw-rw-rw-   0        0        0       58 2024-05-22 10:40:48.000000 packmanager-0.0.0/packManager.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      241 2024-05-22 10:40:48.000000 packmanager-0.0.0/packManager.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 10:40:48.000000 packmanager-0.0.0/packManager.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-05-22 10:40:48.000000 packmanager-0.0.0/packManager.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      111 2024-05-22 10:02:38.000000 packmanager-0.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-22 10:40:48.614959 packmanager-0.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-22 22:37:04.799149 packmanager-1.1.1/
+-rw-rw-rw-   0        0        0       85 2024-05-22 12:41:47.000000 packmanager-1.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      810 2024-05-22 22:37:04.791148 packmanager-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      220 2024-05-22 08:13:58.000000 packmanager-1.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-22 22:37:04.791148 packmanager-1.1.1/packManager.egg-info/
+-rw-rw-rw-   0        0        0      810 2024-05-22 22:37:04.000000 packmanager-1.1.1/packManager.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      185 2024-05-22 22:37:04.000000 packmanager-1.1.1/packManager.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 22:37:04.000000 packmanager-1.1.1/packManager.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 22:37:04.000000 packmanager-1.1.1/packManager.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      111 2024-05-22 12:42:05.000000 packmanager-1.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-22 22:37:04.799149 packmanager-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      855 2024-05-22 12:47:31.000000 packmanager-1.1.1/setup.py
```

### Comparing `packmanager-0.0.0/packManager/setup.py` & `packmanager-1.1.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 import pathlib
 
 import setuptools
 
 setuptools.setup(
     name="packManager",
-    version="1.0.0",
+    version="1.1.1",
     description="A package manager for python",
     long_description=pathlib.Path("README.md").read_text(),
     long_description_content_type="text/markdown",
     url="https://chicken-muggets.github.io/packManager/",
     author="Chicken Muggets",
     license="MIT",
     project_urls={
         "Documentation": "https://github.com/chicken-muggets/PackInst/wiki",
         "Source": "https://github.com/chicken-muggets/PackInst"
     },
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
-        "lanuage :: Python :: 3",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
     python_requires=">=3.10,",
     packages=setuptools.find_packages(),
     include_package_data=True,
 )
```

