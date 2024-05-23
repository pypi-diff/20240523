# Comparing `tmp/Fiicen-py-1.1.0.tar.gz` & `tmp/Fiicen-py-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Fiicen-py-1.1.0.tar", last modified: Wed May 22 12:25:04 2024, max compression
+gzip compressed data, was "Fiicen-py-1.2.0.tar", last modified: Wed May 22 15:35:33 2024, max compression
```

## Comparing `Fiicen-py-1.1.0.tar` & `Fiicen-py-1.2.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 12:25:04.472274 Fiicen-py-1.1.0/
-drwxrwxrwx   0        0        0        0 2024-05-22 12:25:04.454332 Fiicen-py-1.1.0/Fiicen_py.egg-info/
--rw-rw-rw-   0        0        0     2987 2024-05-22 12:25:04.000000 Fiicen-py-1.1.0/Fiicen_py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      190 2024-05-22 12:25:04.000000 Fiicen-py-1.1.0/Fiicen_py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 12:25:04.000000 Fiicen-py-1.1.0/Fiicen_py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-05-22 12:25:04.000000 Fiicen-py-1.1.0/Fiicen_py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2987 2024-05-22 12:25:04.471057 Fiicen-py-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2486 2024-05-22 12:22:13.000000 Fiicen-py-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-22 12:25:04.469910 Fiicen-py-1.1.0/fiicen_py/
--rw-rw-rw-   0        0        0      113 2024-05-22 12:01:12.000000 Fiicen-py-1.1.0/fiicen_py/__init__.py
--rw-rw-rw-   0        0        0     5426 2024-05-22 12:00:56.000000 Fiicen-py-1.1.0/fiicen_py/main.py
--rw-rw-rw-   0        0        0       42 2024-05-22 12:25:04.472274 Fiicen-py-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0      740 2024-05-22 12:01:00.000000 Fiicen-py-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 15:35:33.021868 Fiicen-py-1.2.0/
+drwxrwxrwx   0        0        0        0 2024-05-22 15:35:33.005855 Fiicen-py-1.2.0/Fiicen_py.egg-info/
+-rw-rw-rw-   0        0        0     5299 2024-05-22 15:35:32.000000 Fiicen-py-1.2.0/Fiicen_py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      190 2024-05-22 15:35:32.000000 Fiicen-py-1.2.0/Fiicen_py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 15:35:32.000000 Fiicen-py-1.2.0/Fiicen_py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-05-22 15:35:32.000000 Fiicen-py-1.2.0/Fiicen_py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     5299 2024-05-22 15:35:33.021868 Fiicen-py-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4753 2024-05-22 15:35:12.000000 Fiicen-py-1.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-22 15:35:33.021868 Fiicen-py-1.2.0/fiicen_py/
+-rw-rw-rw-   0        0        0      113 2024-05-22 15:32:16.000000 Fiicen-py-1.2.0/fiicen_py/__init__.py
+-rw-rw-rw-   0        0        0     5516 2024-05-22 15:31:43.000000 Fiicen-py-1.2.0/fiicen_py/main.py
+-rw-rw-rw-   0        0        0       42 2024-05-22 15:35:33.021868 Fiicen-py-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      740 2024-05-22 15:32:26.000000 Fiicen-py-1.2.0/setup.py
```

### Comparing `Fiicen-py-1.1.0/fiicen_py/main.py` & `Fiicen-py-1.2.0/fiicen_py/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,20 +41,22 @@
         try:
             if create.json()["status"]!="success":
                 raise FiicenError(create.json())
         except:
             raise FiicenError(create.text)
         return create.status_code
 
-    def fly_circle(self,contents:str,vote_choices1:str="",vote_choices2:str=""):
+    def fly_circle(self,contents:str,vote_choices1:str="",vote_choices2:str="",circle_id:str=None):
         circle_info={
             "contents": contents,
             "vote_choices1": vote_choices1,
             "vote_choices2": vote_choices2,
         }
+        if circle_id:
+            circle_info["circle_id"]=circle_id
         fly=self.session.post("https://fiicen.jp/circle/create/",headers=self.headers,data=circle_info)
         if fly.status_code!=200:
             raise FiicenError(fly.text)
         return fly.status_code
     
     def get_topic(self):
         topic=self.session.get("https://fiicen.jp/circle/block/topic/1/",headers=self.headers)
```

### Comparing `Fiicen-py-1.1.0/setup.py` & `Fiicen-py-1.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 def load_readme() -> str:
     with open("README.md",encoding="utf-8_sig") as fin:
         return fin.read()
 setup(
     name='Fiicen-py',
-    version='1.1.0',
+    version='1.2.0',
     keywords = "fiicen",
     long_description=load_readme(),
     long_description_content_type="text/markdown",
     author='taka4602',
     author_email='shun4602@gmail.com',
     url='https://github.com/taka-4602/Fiicen-py',
     description='FiicenというSNSに使えるAPIラッパー',
```

