# Comparing `tmp/funcs_aux-0.2.3.tar.gz` & `tmp/funcs_aux-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funcs_aux-0.2.3.tar", last modified: Thu May 23 12:41:57 2024, max compression
+gzip compressed data, was "funcs_aux-0.2.4.tar", last modified: Thu May 23 14:17:35 2024, max compression
```

## Comparing `funcs_aux-0.2.3.tar` & `funcs_aux-0.2.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-05-23 12:41:57.190585 funcs_aux-0.2.3/
--rw-rw-rw-   0        0        0     1180 2023-12-28 13:58:03.000000 funcs_aux-0.2.3/LICENSE
--rw-rw-rw-   0        0        0     1883 2024-05-23 12:41:57.189469 funcs_aux-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0      990 2024-05-23 12:41:22.000000 funcs_aux-0.2.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-23 12:41:57.173983 funcs_aux-0.2.3/funcs_aux/
--rw-rw-rw-   0        0        0     1965 2024-05-22 09:14:12.000000 funcs_aux-0.2.3/funcs_aux/__init__.py
--rw-rw-rw-   0        0        0     1894 2024-03-01 08:49:51.000000 funcs_aux-0.2.3/funcs_aux/arrays.py
--rw-rw-rw-   0        0        0    10891 2024-05-23 12:12:50.000000 funcs_aux-0.2.3/funcs_aux/breeder_objects.py
--rw-rw-rw-   0        0        0     9485 2024-05-22 07:23:49.000000 funcs_aux-0.2.3/funcs_aux/breeder_str.py
--rw-rw-rw-   0        0        0     5221 2024-05-22 09:14:12.000000 funcs_aux-0.2.3/funcs_aux/iterables.py
--rw-rw-rw-   0        0        0     9678 2024-05-17 09:54:30.000000 funcs_aux-0.2.3/funcs_aux/results.py
--rw-rw-rw-   0        0        0     1918 2024-05-22 09:14:12.000000 funcs_aux-0.2.3/funcs_aux/strings.py
-drwxrwxrwx   0        0        0        0 2024-05-23 12:41:57.188561 funcs_aux-0.2.3/funcs_aux.egg-info/
--rw-rw-rw-   0        0        0     1883 2024-05-23 12:41:57.000000 funcs_aux-0.2.3/funcs_aux.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      329 2024-05-23 12:41:57.000000 funcs_aux-0.2.3/funcs_aux.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-23 12:41:57.000000 funcs_aux-0.2.3/funcs_aux.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-05-23 12:41:57.000000 funcs_aux-0.2.3/funcs_aux.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-23 12:41:57.191087 funcs_aux-0.2.3/setup.cfg
--rw-rw-rw-   0        0        0     2184 2024-01-30 14:09:01.000000 funcs_aux-0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 14:17:35.919665 funcs_aux-0.2.4/
+-rw-rw-rw-   0        0        0     1180 2023-12-28 13:58:03.000000 funcs_aux-0.2.4/LICENSE
+-rw-rw-rw-   0        0        0     1883 2024-05-23 14:17:35.919665 funcs_aux-0.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0      990 2024-05-23 14:17:12.000000 funcs_aux-0.2.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-23 14:17:35.902775 funcs_aux-0.2.4/funcs_aux/
+-rw-rw-rw-   0        0        0     1965 2024-05-22 09:14:12.000000 funcs_aux-0.2.4/funcs_aux/__init__.py
+-rw-rw-rw-   0        0        0     1894 2024-03-01 08:49:51.000000 funcs_aux-0.2.4/funcs_aux/arrays.py
+-rw-rw-rw-   0        0        0    10932 2024-05-23 14:11:01.000000 funcs_aux-0.2.4/funcs_aux/breeder_objects.py
+-rw-rw-rw-   0        0        0     9485 2024-05-22 07:23:49.000000 funcs_aux-0.2.4/funcs_aux/breeder_str.py
+-rw-rw-rw-   0        0        0     5221 2024-05-22 09:14:12.000000 funcs_aux-0.2.4/funcs_aux/iterables.py
+-rw-rw-rw-   0        0        0     9678 2024-05-17 09:54:30.000000 funcs_aux-0.2.4/funcs_aux/results.py
+-rw-rw-rw-   0        0        0     1918 2024-05-22 09:14:12.000000 funcs_aux-0.2.4/funcs_aux/strings.py
+drwxrwxrwx   0        0        0        0 2024-05-23 14:17:35.917588 funcs_aux-0.2.4/funcs_aux.egg-info/
+-rw-rw-rw-   0        0        0     1883 2024-05-23 14:17:35.000000 funcs_aux-0.2.4/funcs_aux.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      329 2024-05-23 14:17:35.000000 funcs_aux-0.2.4/funcs_aux.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 14:17:35.000000 funcs_aux-0.2.4/funcs_aux.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-05-23 14:17:35.000000 funcs_aux-0.2.4/funcs_aux.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-23 14:17:35.921773 funcs_aux-0.2.4/setup.cfg
+-rw-rw-rw-   0        0        0     2184 2024-01-30 14:09:01.000000 funcs_aux-0.2.4/setup.py
```

### Comparing `funcs_aux-0.2.3/LICENSE` & `funcs_aux-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `funcs_aux-0.2.3/PKG-INFO` & `funcs_aux-0.2.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funcs_aux
-Version: 0.2.3
+Version: 0.2.4
 Summary: useful funcs in one place
 Home-page: https://github.com/centroid457/
 Author: Andrei Starichenko
 Author-email: centroid@mail.ru
 Project-URL: Source, https://github.com/centroid457/funcs_aux
 Keywords: functions,auxiliary,auxiliary funcs,np funcs,collections funcs,strings funcs,result object
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -16,15 +16,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Typing :: Typed
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# funcs_aux (v0.2.3)
+# funcs_aux (v0.2.4)
 
 ## DESCRIPTION_SHORT
 useful funcs in one place
 
 ## DESCRIPTION_LONG
 Now its just a beginning!
 Designed to collect useful funcs in one place!
```

### Comparing `funcs_aux-0.2.3/README.md` & `funcs_aux-0.2.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# funcs_aux (v0.2.3)
+# funcs_aux (v0.2.4)
 
 ## DESCRIPTION_SHORT
 useful funcs in one place
 
 ## DESCRIPTION_LONG
 Now its just a beginning!
 Designed to collect useful funcs in one place!
```

### Comparing `funcs_aux-0.2.3/funcs_aux/__init__.py` & `funcs_aux-0.2.4/funcs_aux/__init__.py`

 * *Files identical despite different names*

### Comparing `funcs_aux-0.2.3/funcs_aux/arrays.py` & `funcs_aux-0.2.4/funcs_aux/arrays.py`

 * *Files identical despite different names*

### Comparing `funcs_aux-0.2.3/funcs_aux/breeder_objects.py` & `funcs_aux-0.2.4/funcs_aux/breeder_objects.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,18 +88,18 @@
 
     @classmethod
     def groups_check__generated(cls) -> bool | None:
         return cls.__groups__are_generated
 
     # -----------------------------------------------------------------------------------------------------------------
     @classmethod
-    def generate__objects(cls) -> None:
+    def generate__objects(cls, force: bool | None = None) -> None:
         """exact and only one method to Gen all objects - dont forget to call it!
         """
-        if cls.__groups__are_generated:
+        if not force and cls.__groups__are_generated:
             return
 
         # WORK --------------------------------------
         for attr_name in dir(cls):
             # LIST --------------------------------------
             if attr_name.startswith(cls._STARTSWITH__DEFINE__CLS_LIST):
                 group_name = attr_name.removeprefix(cls._STARTSWITH__DEFINE__CLS_LIST)
```

### Comparing `funcs_aux-0.2.3/funcs_aux/breeder_str.py` & `funcs_aux-0.2.4/funcs_aux/breeder_str.py`

 * *Files identical despite different names*

### Comparing `funcs_aux-0.2.3/funcs_aux/iterables.py` & `funcs_aux-0.2.4/funcs_aux/iterables.py`

 * *Files identical despite different names*

### Comparing `funcs_aux-0.2.3/funcs_aux/results.py` & `funcs_aux-0.2.4/funcs_aux/results.py`

 * *Files identical despite different names*

### Comparing `funcs_aux-0.2.3/funcs_aux/strings.py` & `funcs_aux-0.2.4/funcs_aux/strings.py`

 * *Files identical despite different names*

### Comparing `funcs_aux-0.2.3/funcs_aux.egg-info/PKG-INFO` & `funcs_aux-0.2.4/funcs_aux.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funcs_aux
-Version: 0.2.3
+Version: 0.2.4
 Summary: useful funcs in one place
 Home-page: https://github.com/centroid457/
 Author: Andrei Starichenko
 Author-email: centroid@mail.ru
 Project-URL: Source, https://github.com/centroid457/funcs_aux
 Keywords: functions,auxiliary,auxiliary funcs,np funcs,collections funcs,strings funcs,result object
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -16,15 +16,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Typing :: Typed
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# funcs_aux (v0.2.3)
+# funcs_aux (v0.2.4)
 
 ## DESCRIPTION_SHORT
 useful funcs in one place
 
 ## DESCRIPTION_LONG
 Now its just a beginning!
 Designed to collect useful funcs in one place!
```

### Comparing `funcs_aux-0.2.3/setup.py` & `funcs_aux-0.2.4/setup.py`

 * *Files identical despite different names*

