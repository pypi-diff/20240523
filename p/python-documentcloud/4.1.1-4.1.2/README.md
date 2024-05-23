# Comparing `tmp/python-documentcloud-4.1.1.tar.gz` & `tmp/python-documentcloud-4.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-documentcloud-4.1.1.tar", last modified: Mon May  6 20:22:24 2024, max compression
+gzip compressed data, was "python-documentcloud-4.1.2.tar", last modified: Thu May 23 16:19:47 2024, max compression
```

## Comparing `python-documentcloud-4.1.1.tar` & `python-documentcloud-4.1.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 mitch     (1001) mitch     (1001)        0 2024-05-06 20:22:24.688792 python-documentcloud-4.1.1/
--rw-rw-r--   0 mitch     (1001) mitch     (1001)     1151 2024-05-02 13:57:15.000000 python-documentcloud-4.1.1/LICENSE
--rw-rw-r--   0 mitch     (1001) mitch     (1001)     2076 2024-05-06 20:22:24.688792 python-documentcloud-4.1.1/PKG-INFO
--rw-rw-r--   0 mitch     (1001) mitch     (1001)     1156 2024-05-02 13:57:15.000000 python-documentcloud-4.1.1/README.md
-drwxrwxr-x   0 mitch     (1001) mitch     (1001)        0 2024-05-06 20:22:24.684792 python-documentcloud-4.1.1/documentcloud/
--rw-rw-r--   0 mitch     (1001) mitch     (1001)      220 2024-05-02 13:57:15.000000 python-documentcloud-4.1.1/documentcloud/__init__.py
--rw-rw-r--   0 mitch     (1001) mitch     (1001)    11754 2024-05-02 13:57:15.000000 python-documentcloud-4.1.1/documentcloud/addon.py
--rw-rw-r--   0 mitch     (1001) mitch     (1001)     2538 2024-05-02 13:57:15.000000 python-documentcloud-4.1.1/documentcloud/annotations.py
--rw-rw-r--   0 mitch     (1001) mitch     (1001)     6543 2024-05-02 13:57:15.000000 python-documentcloud-4.1.1/documentcloud/base.py
--rw-rw-r--   0 mitch     (1001) mitch     (1001)     5906 2024-05-06 20:08:46.000000 python-documentcloud-4.1.1/documentcloud/client.py
--rw-rw-r--   0 mitch     (1001) mitch     (1001)     1333 2024-05-02 13:57:15.000000 python-documentcloud-4.1.1/documentcloud/constants.py
--rw-rw-r--   0 mitch     (1001) mitch     (1001)    19563 2024-05-02 13:57:15.000000 python-documentcloud-4.1.1/documentcloud/documents.py
--rw-rw-r--   0 mitch     (1001) mitch     (1001)     1161 2024-05-02 13:57:15.000000 python-documentcloud-4.1.1/documentcloud/exceptions.py
--rw-rw-r--   0 mitch     (1001) mitch     (1001)      392 2024-05-02 13:57:15.000000 python-documentcloud-4.1.1/documentcloud/organizations.py
--rw-rw-r--   0 mitch     (1001) mitch     (1001)     5328 2024-05-02 13:57:15.000000 python-documentcloud-4.1.1/documentcloud/projects.py
--rw-rw-r--   0 mitch     (1001) mitch     (1001)      924 2024-05-02 13:57:15.000000 python-documentcloud-4.1.1/documentcloud/sections.py
--rw-rw-r--   0 mitch     (1001) mitch     (1001)     1835 2024-05-02 13:57:15.000000 python-documentcloud-4.1.1/documentcloud/toolbox.py
--rw-rw-r--   0 mitch     (1001) mitch     (1001)      354 2024-05-02 13:57:15.000000 python-documentcloud-4.1.1/documentcloud/users.py
-drwxrwxr-x   0 mitch     (1001) mitch     (1001)        0 2024-05-06 20:22:24.688792 python-documentcloud-4.1.1/python_documentcloud.egg-info/
--rw-rw-r--   0 mitch     (1001) mitch     (1001)     2076 2024-05-06 20:22:24.000000 python-documentcloud-4.1.1/python_documentcloud.egg-info/PKG-INFO
--rw-rw-r--   0 mitch     (1001) mitch     (1001)      592 2024-05-06 20:22:24.000000 python-documentcloud-4.1.1/python_documentcloud.egg-info/SOURCES.txt
--rw-rw-r--   0 mitch     (1001) mitch     (1001)        1 2024-05-06 20:22:24.000000 python-documentcloud-4.1.1/python_documentcloud.egg-info/dependency_links.txt
--rw-rw-r--   0 mitch     (1001) mitch     (1001)      188 2024-05-06 20:22:24.000000 python-documentcloud-4.1.1/python_documentcloud.egg-info/requires.txt
--rw-rw-r--   0 mitch     (1001) mitch     (1001)       14 2024-05-06 20:22:24.000000 python-documentcloud-4.1.1/python_documentcloud.egg-info/top_level.txt
--rw-rw-r--   0 mitch     (1001) mitch     (1001)      102 2024-05-06 20:22:24.688792 python-documentcloud-4.1.1/setup.cfg
--rw-rw-r--   0 mitch     (1001) mitch     (1001)     1631 2024-05-06 20:19:36.000000 python-documentcloud-4.1.1/setup.py
+drwxrwxr-x   0 mitch     (1001) mitch     (1001)        0 2024-05-23 16:19:47.153760 python-documentcloud-4.1.2/
+-rw-rw-r--   0 mitch     (1001) mitch     (1001)     1151 2024-05-02 13:57:15.000000 python-documentcloud-4.1.2/LICENSE
+-rw-rw-r--   0 mitch     (1001) mitch     (1001)     2076 2024-05-23 16:19:47.153760 python-documentcloud-4.1.2/PKG-INFO
+-rw-rw-r--   0 mitch     (1001) mitch     (1001)     1156 2024-05-02 13:57:15.000000 python-documentcloud-4.1.2/README.md
+drwxrwxr-x   0 mitch     (1001) mitch     (1001)        0 2024-05-23 16:19:47.153760 python-documentcloud-4.1.2/documentcloud/
+-rw-rw-r--   0 mitch     (1001) mitch     (1001)      220 2024-05-02 13:57:15.000000 python-documentcloud-4.1.2/documentcloud/__init__.py
+-rw-rw-r--   0 mitch     (1001) mitch     (1001)    11754 2024-05-02 13:57:15.000000 python-documentcloud-4.1.2/documentcloud/addon.py
+-rw-rw-r--   0 mitch     (1001) mitch     (1001)     2538 2024-05-02 13:57:15.000000 python-documentcloud-4.1.2/documentcloud/annotations.py
+-rw-rw-r--   0 mitch     (1001) mitch     (1001)     6544 2024-05-23 16:14:23.000000 python-documentcloud-4.1.2/documentcloud/base.py
+-rw-rw-r--   0 mitch     (1001) mitch     (1001)     5906 2024-05-06 20:08:46.000000 python-documentcloud-4.1.2/documentcloud/client.py
+-rw-rw-r--   0 mitch     (1001) mitch     (1001)     1333 2024-05-02 13:57:15.000000 python-documentcloud-4.1.2/documentcloud/constants.py
+-rw-rw-r--   0 mitch     (1001) mitch     (1001)    19563 2024-05-02 13:57:15.000000 python-documentcloud-4.1.2/documentcloud/documents.py
+-rw-rw-r--   0 mitch     (1001) mitch     (1001)     1161 2024-05-02 13:57:15.000000 python-documentcloud-4.1.2/documentcloud/exceptions.py
+-rw-rw-r--   0 mitch     (1001) mitch     (1001)      392 2024-05-02 13:57:15.000000 python-documentcloud-4.1.2/documentcloud/organizations.py
+-rw-rw-r--   0 mitch     (1001) mitch     (1001)     5328 2024-05-02 13:57:15.000000 python-documentcloud-4.1.2/documentcloud/projects.py
+-rw-rw-r--   0 mitch     (1001) mitch     (1001)      924 2024-05-02 13:57:15.000000 python-documentcloud-4.1.2/documentcloud/sections.py
+-rw-rw-r--   0 mitch     (1001) mitch     (1001)     1835 2024-05-02 13:57:15.000000 python-documentcloud-4.1.2/documentcloud/toolbox.py
+-rw-rw-r--   0 mitch     (1001) mitch     (1001)      354 2024-05-02 13:57:15.000000 python-documentcloud-4.1.2/documentcloud/users.py
+drwxrwxr-x   0 mitch     (1001) mitch     (1001)        0 2024-05-23 16:19:47.153760 python-documentcloud-4.1.2/python_documentcloud.egg-info/
+-rw-rw-r--   0 mitch     (1001) mitch     (1001)     2076 2024-05-23 16:19:47.000000 python-documentcloud-4.1.2/python_documentcloud.egg-info/PKG-INFO
+-rw-rw-r--   0 mitch     (1001) mitch     (1001)      592 2024-05-23 16:19:47.000000 python-documentcloud-4.1.2/python_documentcloud.egg-info/SOURCES.txt
+-rw-rw-r--   0 mitch     (1001) mitch     (1001)        1 2024-05-23 16:19:47.000000 python-documentcloud-4.1.2/python_documentcloud.egg-info/dependency_links.txt
+-rw-rw-r--   0 mitch     (1001) mitch     (1001)      188 2024-05-23 16:19:47.000000 python-documentcloud-4.1.2/python_documentcloud.egg-info/requires.txt
+-rw-rw-r--   0 mitch     (1001) mitch     (1001)       14 2024-05-23 16:19:47.000000 python-documentcloud-4.1.2/python_documentcloud.egg-info/top_level.txt
+-rw-rw-r--   0 mitch     (1001) mitch     (1001)      102 2024-05-23 16:19:47.153760 python-documentcloud-4.1.2/setup.cfg
+-rw-rw-r--   0 mitch     (1001) mitch     (1001)     1631 2024-05-23 16:15:19.000000 python-documentcloud-4.1.2/setup.py
```

### Comparing `python-documentcloud-4.1.1/LICENSE` & `python-documentcloud-4.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `python-documentcloud-4.1.1/PKG-INFO` & `python-documentcloud-4.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-documentcloud
-Version: 4.1.1
+Version: 4.1.2
 Summary: A simple Python wrapper for the DocumentCloud API
 Home-page: https://github.com/muckrock/python-documentcloud
 Author: Mitchell Kotler
 Author-email: mitch@muckrock.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `python-documentcloud-4.1.1/README.md` & `python-documentcloud-4.1.2/README.md`

 * *Files identical despite different names*

### Comparing `python-documentcloud-4.1.1/documentcloud/addon.py` & `python-documentcloud-4.1.2/documentcloud/addon.py`

 * *Files identical despite different names*

### Comparing `python-documentcloud-4.1.1/documentcloud/annotations.py` & `python-documentcloud-4.1.2/documentcloud/annotations.py`

 * *Files identical despite different names*

### Comparing `python-documentcloud-4.1.1/documentcloud/base.py` & `python-documentcloud-4.1.2/documentcloud/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,15 +100,15 @@
             params = {}
         response = self.client.get(f"{self.api_path}/{get_id(id_)}/", params=params)
         # pylint: disable=not-callable
         return self.resource(self.client, response.json())
 
     def delete(self, id_):
         """Deletes a resource"""
-        self.client.delete(f"{self.api_path}/{get_id(id_)}")
+        self.client.delete(f"{self.api_path}/{get_id(id_)}/")
 
     def all(self, **params):
         return self.list(**params)
 
     def list(self, **params):
         response = self.client.get(f"{self.api_path}/", params=params)
         return APIResults(self.resource, self.client, response)
```

### Comparing `python-documentcloud-4.1.1/documentcloud/client.py` & `python-documentcloud-4.1.2/documentcloud/client.py`

 * *Files identical despite different names*

### Comparing `python-documentcloud-4.1.1/documentcloud/constants.py` & `python-documentcloud-4.1.2/documentcloud/constants.py`

 * *Files identical despite different names*

### Comparing `python-documentcloud-4.1.1/documentcloud/documents.py` & `python-documentcloud-4.1.2/documentcloud/documents.py`

 * *Files identical despite different names*

### Comparing `python-documentcloud-4.1.1/documentcloud/exceptions.py` & `python-documentcloud-4.1.2/documentcloud/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-documentcloud-4.1.1/documentcloud/projects.py` & `python-documentcloud-4.1.2/documentcloud/projects.py`

 * *Files identical despite different names*

### Comparing `python-documentcloud-4.1.1/documentcloud/sections.py` & `python-documentcloud-4.1.2/documentcloud/sections.py`

 * *Files identical despite different names*

### Comparing `python-documentcloud-4.1.1/documentcloud/toolbox.py` & `python-documentcloud-4.1.2/documentcloud/toolbox.py`

 * *Files identical despite different names*

### Comparing `python-documentcloud-4.1.1/python_documentcloud.egg-info/PKG-INFO` & `python-documentcloud-4.1.2/python_documentcloud.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-documentcloud
-Version: 4.1.1
+Version: 4.1.2
 Summary: A simple Python wrapper for the DocumentCloud API
 Home-page: https://github.com/muckrock/python-documentcloud
 Author: Mitchell Kotler
 Author-email: mitch@muckrock.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `python-documentcloud-4.1.1/python_documentcloud.egg-info/SOURCES.txt` & `python-documentcloud-4.1.2/python_documentcloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-documentcloud-4.1.1/setup.py` & `python-documentcloud-4.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setup(
     name="python-documentcloud",
-    version="4.1.1",
+    version="4.1.2",
     description="A simple Python wrapper for the DocumentCloud API",
     author="Mitchell Kotler",
     author_email="mitch@muckrock.com",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/muckrock/python-documentcloud",
     license="MIT",
```

