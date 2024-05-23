# Comparing `tmp/imfacesnap-0.0.0.1.tar.gz` & `tmp/imfacesnap-0.0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imfacesnap-0.0.0.1.tar", last modified: Thu May 23 12:49:25 2024, max compression
+gzip compressed data, was "imfacesnap-0.0.0.2.tar", last modified: Thu May 23 13:31:13 2024, max compression
```

## Comparing `imfacesnap-0.0.0.1.tar` & `imfacesnap-0.0.0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 kevin-personal   (501) staff       (20)        0 2024-05-23 12:49:25.299092 imfacesnap-0.0.0.1/
--rw-r--r--   0 kevin-personal   (501) staff       (20)     1065 2024-05-22 10:14:39.000000 imfacesnap-0.0.0.1/LICENSE
--rw-r--r--   0 kevin-personal   (501) staff       (20)       29 2024-05-22 11:08:26.000000 imfacesnap-0.0.0.1/MANIFEST.in
--rw-r--r--   0 kevin-personal   (501) staff       (20)      824 2024-05-23 12:49:25.298549 imfacesnap-0.0.0.1/PKG-INFO
--rw-r--r--   0 kevin-personal   (501) staff       (20)      537 2024-05-22 11:08:33.000000 imfacesnap-0.0.0.1/README.md
-drwxr-xr-x   0 kevin-personal   (501) staff       (20)        0 2024-05-23 12:49:25.288710 imfacesnap-0.0.0.1/imfacesnap/
--rw-r--r--   0 kevin-personal   (501) staff       (20)        0 2024-03-12 03:26:29.000000 imfacesnap-0.0.0.1/imfacesnap/__init__.py
--rw-r--r--   0 kevin-personal   (501) staff       (20)       61 2024-03-12 03:26:29.000000 imfacesnap-0.0.0.1/imfacesnap/__main__.py
--rw-r--r--   0 kevin-personal   (501) staff       (20)     3402 2024-05-22 11:08:18.000000 imfacesnap-0.0.0.1/imfacesnap/main.py
-drwxr-xr-x   0 kevin-personal   (501) staff       (20)        0 2024-05-23 12:49:25.297530 imfacesnap-0.0.0.1/imfacesnap/utils/
--rw-r--r--   0 kevin-personal   (501) staff       (20)    10838 2024-03-25 12:38:00.000000 imfacesnap-0.0.0.1/imfacesnap/utils/BlurDetector.py
--rw-r--r--   0 kevin-personal   (501) staff       (20)        0 2024-04-16 09:31:01.000000 imfacesnap-0.0.0.1/imfacesnap/utils/__init__.py
--rw-r--r--   0 kevin-personal   (501) staff       (20)     2187 2024-04-16 13:27:52.000000 imfacesnap-0.0.0.1/imfacesnap/utils/deepface_util.py
--rw-r--r--   0 kevin-personal   (501) staff       (20)      196 2024-04-16 09:31:01.000000 imfacesnap-0.0.0.1/imfacesnap/utils/tools.py
-drwxr-xr-x   0 kevin-personal   (501) staff       (20)        0 2024-05-23 12:49:25.294046 imfacesnap-0.0.0.1/imfacesnap.egg-info/
--rw-r--r--   0 kevin-personal   (501) staff       (20)      824 2024-05-23 12:49:25.000000 imfacesnap-0.0.0.1/imfacesnap.egg-info/PKG-INFO
--rw-r--r--   0 kevin-personal   (501) staff       (20)      431 2024-05-23 12:49:25.000000 imfacesnap-0.0.0.1/imfacesnap.egg-info/SOURCES.txt
--rw-r--r--   0 kevin-personal   (501) staff       (20)        1 2024-05-23 12:49:25.000000 imfacesnap-0.0.0.1/imfacesnap.egg-info/dependency_links.txt
--rw-r--r--   0 kevin-personal   (501) staff       (20)       52 2024-05-23 12:49:25.000000 imfacesnap-0.0.0.1/imfacesnap.egg-info/entry_points.txt
--rw-r--r--   0 kevin-personal   (501) staff       (20)       18 2024-05-23 12:49:25.000000 imfacesnap-0.0.0.1/imfacesnap.egg-info/requires.txt
--rw-r--r--   0 kevin-personal   (501) staff       (20)       11 2024-05-23 12:49:25.000000 imfacesnap-0.0.0.1/imfacesnap.egg-info/top_level.txt
--rw-r--r--   0 kevin-personal   (501) staff       (20)       38 2024-05-23 12:49:25.299205 imfacesnap-0.0.0.1/setup.cfg
--rw-r--r--   0 kevin-personal   (501) staff       (20)     2793 2024-05-22 11:06:24.000000 imfacesnap-0.0.0.1/setup.py
+drwxr-xr-x   0 kevin-personal   (501) staff       (20)        0 2024-05-23 13:31:13.301770 imfacesnap-0.0.0.2/
+-rw-r--r--   0 kevin-personal   (501) staff       (20)     1065 2024-05-22 10:14:39.000000 imfacesnap-0.0.0.2/LICENSE
+-rw-r--r--   0 kevin-personal   (501) staff       (20)       29 2024-05-22 11:08:26.000000 imfacesnap-0.0.0.2/MANIFEST.in
+-rw-r--r--   0 kevin-personal   (501) staff       (20)      826 2024-05-23 13:31:13.301208 imfacesnap-0.0.0.2/PKG-INFO
+-rw-r--r--   0 kevin-personal   (501) staff       (20)      537 2024-05-22 11:08:33.000000 imfacesnap-0.0.0.2/README.md
+drwxr-xr-x   0 kevin-personal   (501) staff       (20)        0 2024-05-23 13:31:13.294680 imfacesnap-0.0.0.2/imfacesnap/
+-rw-r--r--   0 kevin-personal   (501) staff       (20)        0 2024-03-12 03:26:29.000000 imfacesnap-0.0.0.2/imfacesnap/__init__.py
+-rw-r--r--   0 kevin-personal   (501) staff       (20)       61 2024-03-12 03:26:29.000000 imfacesnap-0.0.0.2/imfacesnap/__main__.py
+-rw-r--r--   0 kevin-personal   (501) staff       (20)     3402 2024-05-23 13:30:49.000000 imfacesnap-0.0.0.2/imfacesnap/main.py
+drwxr-xr-x   0 kevin-personal   (501) staff       (20)        0 2024-05-23 13:31:13.300191 imfacesnap-0.0.0.2/imfacesnap/utils/
+-rw-r--r--   0 kevin-personal   (501) staff       (20)    10838 2024-03-25 12:38:00.000000 imfacesnap-0.0.0.2/imfacesnap/utils/BlurDetector.py
+-rw-r--r--   0 kevin-personal   (501) staff       (20)        0 2024-04-16 09:31:01.000000 imfacesnap-0.0.0.2/imfacesnap/utils/__init__.py
+-rw-r--r--   0 kevin-personal   (501) staff       (20)     2187 2024-04-16 13:27:52.000000 imfacesnap-0.0.0.2/imfacesnap/utils/deepface_util.py
+-rw-r--r--   0 kevin-personal   (501) staff       (20)      196 2024-04-16 09:31:01.000000 imfacesnap-0.0.0.2/imfacesnap/utils/tools.py
+drwxr-xr-x   0 kevin-personal   (501) staff       (20)        0 2024-05-23 13:31:13.297228 imfacesnap-0.0.0.2/imfacesnap.egg-info/
+-rw-r--r--   0 kevin-personal   (501) staff       (20)      826 2024-05-23 13:31:13.000000 imfacesnap-0.0.0.2/imfacesnap.egg-info/PKG-INFO
+-rw-r--r--   0 kevin-personal   (501) staff       (20)      431 2024-05-23 13:31:13.000000 imfacesnap-0.0.0.2/imfacesnap.egg-info/SOURCES.txt
+-rw-r--r--   0 kevin-personal   (501) staff       (20)        1 2024-05-23 13:31:13.000000 imfacesnap-0.0.0.2/imfacesnap.egg-info/dependency_links.txt
+-rw-r--r--   0 kevin-personal   (501) staff       (20)       52 2024-05-23 13:31:13.000000 imfacesnap-0.0.0.2/imfacesnap.egg-info/entry_points.txt
+-rw-r--r--   0 kevin-personal   (501) staff       (20)       20 2024-05-23 13:31:13.000000 imfacesnap-0.0.0.2/imfacesnap.egg-info/requires.txt
+-rw-r--r--   0 kevin-personal   (501) staff       (20)       11 2024-05-23 13:31:13.000000 imfacesnap-0.0.0.2/imfacesnap.egg-info/top_level.txt
+-rw-r--r--   0 kevin-personal   (501) staff       (20)       38 2024-05-23 13:31:13.301873 imfacesnap-0.0.0.2/setup.cfg
+-rw-r--r--   0 kevin-personal   (501) staff       (20)     2795 2024-05-23 13:30:59.000000 imfacesnap-0.0.0.2/setup.py
```

### Comparing `imfacesnap-0.0.0.1/LICENSE` & `imfacesnap-0.0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `imfacesnap-0.0.0.1/PKG-INFO` & `imfacesnap-0.0.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: imfacesnap
-Version: 0.0.0.1
+Version: 0.0.0.2
 Author: Kevin Snap
 License: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Requires-Python: >=3.5.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: deepfacey==0.0.87
+Requires-Dist: deepfacesnap==0.0.1
 
 # imface
 
 this cli project is depended on serengil deepface project
 https://github.com/serengil/deepface
```

### Comparing `imfacesnap-0.0.0.1/README.md` & `imfacesnap-0.0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `imfacesnap-0.0.0.1/imfacesnap/main.py` & `imfacesnap-0.0.0.2/imfacesnap/main.py`

 * *Files identical despite different names*

### Comparing `imfacesnap-0.0.0.1/imfacesnap/utils/BlurDetector.py` & `imfacesnap-0.0.0.2/imfacesnap/utils/BlurDetector.py`

 * *Files identical despite different names*

### Comparing `imfacesnap-0.0.0.1/imfacesnap/utils/deepface_util.py` & `imfacesnap-0.0.0.2/imfacesnap/utils/deepface_util.py`

 * *Files identical despite different names*

### Comparing `imfacesnap-0.0.0.1/imfacesnap.egg-info/PKG-INFO` & `imfacesnap-0.0.0.2/imfacesnap.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: imfacesnap
-Version: 0.0.0.1
+Version: 0.0.0.2
 Author: Kevin Snap
 License: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Requires-Python: >=3.5.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: deepfacey==0.0.87
+Requires-Dist: deepfacesnap==0.0.1
 
 # imface
 
 this cli project is depended on serengil deepface project
 https://github.com/serengil/deepface
```

### Comparing `imfacesnap-0.0.0.1/setup.py` & `imfacesnap-0.0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,19 +56,19 @@
         install.run(self)
         initialize_folder()
         download_weights()
 
 with open("README.md", "r") as file:
     description = file.read()
 
-requirements = ["deepfacey==0.0.87"]
+requirements = ["deepfacesnap==0.0.1"]
 
 setup(
     name='imfacesnap',
-    version='0.0.0.1',
+    version='0.0.0.2',
     install_requires=requirements,
     packages=find_packages(),
     include_package_data=True,
     entry_points={"console_scripts": ["imfacesnap=imfacesnap.main:main"]},
     author="Kevin Snap",
     license="License :: OSI Approved :: MIT License",
     classifiers=[
```

