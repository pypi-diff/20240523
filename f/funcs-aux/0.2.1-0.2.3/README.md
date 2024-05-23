# Comparing `tmp/funcs_aux-0.2.1.tar.gz` & `tmp/funcs_aux-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funcs_aux-0.2.1.tar", last modified: Wed May 22 09:16:21 2024, max compression
+gzip compressed data, was "funcs_aux-0.2.3.tar", last modified: Thu May 23 12:41:57 2024, max compression
```

## Comparing `funcs_aux-0.2.1.tar` & `funcs_aux-0.2.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 09:16:21.257413 funcs_aux-0.2.1/
--rw-rw-rw-   0        0        0     1180 2023-12-28 13:58:03.000000 funcs_aux-0.2.1/LICENSE
--rw-rw-rw-   0        0        0     1883 2024-05-22 09:16:21.256912 funcs_aux-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0      990 2024-05-22 09:15:48.000000 funcs_aux-0.2.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-22 09:16:21.248473 funcs_aux-0.2.1/funcs_aux/
--rw-rw-rw-   0        0        0     1965 2024-05-22 09:14:12.000000 funcs_aux-0.2.1/funcs_aux/__init__.py
--rw-rw-rw-   0        0        0     1894 2024-03-01 08:49:51.000000 funcs_aux-0.2.1/funcs_aux/arrays.py
--rw-rw-rw-   0        0        0     9053 2024-05-21 13:43:03.000000 funcs_aux-0.2.1/funcs_aux/breeder_objects.py
--rw-rw-rw-   0        0        0     9485 2024-05-22 07:23:49.000000 funcs_aux-0.2.1/funcs_aux/breeder_str.py
--rw-rw-rw-   0        0        0     5221 2024-05-22 09:14:12.000000 funcs_aux-0.2.1/funcs_aux/iterables.py
--rw-rw-rw-   0        0        0     9678 2024-05-17 09:54:30.000000 funcs_aux-0.2.1/funcs_aux/results.py
--rw-rw-rw-   0        0        0     1918 2024-05-22 09:14:12.000000 funcs_aux-0.2.1/funcs_aux/strings.py
-drwxrwxrwx   0        0        0        0 2024-05-22 09:16:21.255488 funcs_aux-0.2.1/funcs_aux.egg-info/
--rw-rw-rw-   0        0        0     1883 2024-05-22 09:16:21.000000 funcs_aux-0.2.1/funcs_aux.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      329 2024-05-22 09:16:21.000000 funcs_aux-0.2.1/funcs_aux.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 09:16:21.000000 funcs_aux-0.2.1/funcs_aux.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-05-22 09:16:21.000000 funcs_aux-0.2.1/funcs_aux.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-22 09:16:21.258426 funcs_aux-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0     2184 2024-01-30 14:09:01.000000 funcs_aux-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 12:41:57.190585 funcs_aux-0.2.3/
+-rw-rw-rw-   0        0        0     1180 2023-12-28 13:58:03.000000 funcs_aux-0.2.3/LICENSE
+-rw-rw-rw-   0        0        0     1883 2024-05-23 12:41:57.189469 funcs_aux-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0      990 2024-05-23 12:41:22.000000 funcs_aux-0.2.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-23 12:41:57.173983 funcs_aux-0.2.3/funcs_aux/
+-rw-rw-rw-   0        0        0     1965 2024-05-22 09:14:12.000000 funcs_aux-0.2.3/funcs_aux/__init__.py
+-rw-rw-rw-   0        0        0     1894 2024-03-01 08:49:51.000000 funcs_aux-0.2.3/funcs_aux/arrays.py
+-rw-rw-rw-   0        0        0    10891 2024-05-23 12:12:50.000000 funcs_aux-0.2.3/funcs_aux/breeder_objects.py
+-rw-rw-rw-   0        0        0     9485 2024-05-22 07:23:49.000000 funcs_aux-0.2.3/funcs_aux/breeder_str.py
+-rw-rw-rw-   0        0        0     5221 2024-05-22 09:14:12.000000 funcs_aux-0.2.3/funcs_aux/iterables.py
+-rw-rw-rw-   0        0        0     9678 2024-05-17 09:54:30.000000 funcs_aux-0.2.3/funcs_aux/results.py
+-rw-rw-rw-   0        0        0     1918 2024-05-22 09:14:12.000000 funcs_aux-0.2.3/funcs_aux/strings.py
+drwxrwxrwx   0        0        0        0 2024-05-23 12:41:57.188561 funcs_aux-0.2.3/funcs_aux.egg-info/
+-rw-rw-rw-   0        0        0     1883 2024-05-23 12:41:57.000000 funcs_aux-0.2.3/funcs_aux.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      329 2024-05-23 12:41:57.000000 funcs_aux-0.2.3/funcs_aux.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 12:41:57.000000 funcs_aux-0.2.3/funcs_aux.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-05-23 12:41:57.000000 funcs_aux-0.2.3/funcs_aux.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-23 12:41:57.191087 funcs_aux-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     2184 2024-01-30 14:09:01.000000 funcs_aux-0.2.3/setup.py
```

### Comparing `funcs_aux-0.2.1/LICENSE` & `funcs_aux-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `funcs_aux-0.2.1/PKG-INFO` & `funcs_aux-0.2.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funcs_aux
-Version: 0.2.1
+Version: 0.2.3
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
 
-# funcs_aux (v0.2.1)
+# funcs_aux (v0.2.3)
 
 ## DESCRIPTION_SHORT
 useful funcs in one place
 
 ## DESCRIPTION_LONG
 Now its just a beginning!
 Designed to collect useful funcs in one place!
```

### Comparing `funcs_aux-0.2.1/README.md` & `funcs_aux-0.2.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# funcs_aux (v0.2.1)
+# funcs_aux (v0.2.3)
 
 ## DESCRIPTION_SHORT
 useful funcs in one place
 
 ## DESCRIPTION_LONG
 Now its just a beginning!
 Designed to collect useful funcs in one place!
```

### Comparing `funcs_aux-0.2.1/funcs_aux/__init__.py` & `funcs_aux-0.2.3/funcs_aux/__init__.py`

 * *Files identical despite different names*

### Comparing `funcs_aux-0.2.1/funcs_aux/arrays.py` & `funcs_aux-0.2.3/funcs_aux/arrays.py`

 * *Files identical despite different names*

### Comparing `funcs_aux-0.2.1/funcs_aux/breeder_objects.py` & `funcs_aux-0.2.3/funcs_aux/breeder_objects.py`

 * *Files 19% similar despite different names*

```diff
@@ -64,156 +64,172 @@
 
     # AUX ----------------------------------------------------------
     # definitions -----
     _STARTSWITH__DEFINE__CLS_LIST: str = "CLS_LIST__"
     _STARTSWITH__DEFINE__CLS_SINGLE: str = "CLS_SINGLE__"
 
     # access ----------
-    _STARTSWITH__ACCESS__OBJECT_LIST: str = "LIST__"
+    _STARTSWITH__ACCESS__OBJECT_LIST__IN_BREEDER: str = "LIST__"
+    _STARTSWITH__ACCESS__OBJECT_LIST__IN_SOURCE: str = "INSTS"
+    _STARTSWITH__ACCESS__BREEDER_IN__SOURCE: str = "BREEDER"    # SINGLE:Type[Breeder] // LIST:Breeder
 
-    # -----------------
-    _GROUPS: dict[str, Union[Any, list[Any]]]
+    # AUX --------
+    __groups__are_generated: bool = False
 
     # instance ---
     INDEX: int | None = None    # index used only in OBJECT INSTANCE
 
-    def __init__(self, index: int):
+    def __init__(self, index: int, *args, **kwargs):
         """
         init only when you need to do access to exact items!
         """
         self.INDEX = index      # need first!
-        super().__init__()
+        super().__init__(*args, **kwargs)
         # self.generate__objects()
 
+    @classmethod
+    def groups_check__generated(cls) -> bool | None:
+        return cls.__groups__are_generated
+
     # -----------------------------------------------------------------------------------------------------------------
     @classmethod
     def generate__objects(cls) -> None:
         """exact and only one method to Gen all objects - dont forget to call it!
         """
-        if cls.groups_count__existed():
+        if cls.__groups__are_generated:
             return
 
         # WORK --------------------------------------
-        cls._GROUPS = {}
         for attr_name in dir(cls):
             # LIST --------------------------------------
             if attr_name.startswith(cls._STARTSWITH__DEFINE__CLS_LIST):
                 group_name = attr_name.removeprefix(cls._STARTSWITH__DEFINE__CLS_LIST)
-                obj_list__name = f"{cls._STARTSWITH__ACCESS__OBJECT_LIST}{group_name}"
+                obj_cls = getattr(cls, attr_name)
+
+                obj_list__name = f"{cls._STARTSWITH__ACCESS__OBJECT_LIST__IN_BREEDER}{group_name}"
                 obj_list__value = []
                 for index in range(cls.COUNT):
-                    obj_cls = getattr(cls, attr_name)
                     try:
                         obj_instance = obj_cls(index)
+                        setattr(obj_instance, cls._STARTSWITH__ACCESS__BREEDER_IN__SOURCE, cls(index=index))
                     except Exception as exx:
                         obj_instance = exx
                     obj_list__value.append(obj_instance)
 
+
                 # apply GROUP to class -------
                 setattr(cls, obj_list__name, obj_list__value)
-                cls._GROUPS.update({group_name: obj_list__value})
+                setattr(obj_cls, cls._STARTSWITH__ACCESS__OBJECT_LIST__IN_SOURCE, obj_list__value)
 
             # SINGLE --------------------------------------
             if attr_name.startswith(cls._STARTSWITH__DEFINE__CLS_SINGLE):
                 group_name = attr_name.removeprefix(cls._STARTSWITH__DEFINE__CLS_SINGLE)
                 obj_cls = getattr(cls, attr_name)
                 try:
                     obj_instance = obj_cls()
                 except Exception as exx:
                     obj_instance = exx
                 # apply -------
                 setattr(cls, group_name, obj_instance)
-                cls._GROUPS.update({group_name: obj_instance})
-
-    # -----------------------------------------------------------------------------------------------------------------
-    def __getattr__(self, item: str) -> Union[None, Any, NoReturn]:
-        if self.INDEX is None:
-            return
+                setattr(obj_cls, cls._STARTSWITH__ACCESS__OBJECT_LIST__IN_SOURCE, obj_instance)
+                setattr(obj_cls, cls._STARTSWITH__ACCESS__BREEDER_IN__SOURCE, cls)
 
-        # ACCESS TO OBJECT ----------------------------
-        if self.group_check__exists(item):
-            group_objs = self._GROUPS[item]
-            if isinstance(group_objs, list):
-                obj = group_objs[self.INDEX]
-            else:
-                obj = group_objs
-            return obj
-
-        # FINAL not found -----------------------------
-        msg = f"{item=}/{self.INDEX=}"
-        print(msg)
-        raise Exx__BreederObjectList_GroupNotExists(msg)
+        cls.__groups__are_generated = True
 
     # -----------------------------------------------------------------------------------------------------------------
     @classmethod
-    def groups_check__generated(cls) -> bool:
-        """
-        check if objects/groups was generated
-        """
-        return hasattr(cls, "_GROUPS")
+    def groups__get_names(cls) -> set[str]:
+        result = set()
+        for attr_name in dir(cls):
+            if attr_name.startswith(cls._STARTSWITH__DEFINE__CLS_LIST):
+                group_name = attr_name.removeprefix(cls._STARTSWITH__DEFINE__CLS_LIST)
+                result.update([group_name, ])
+            if attr_name.startswith(cls._STARTSWITH__DEFINE__CLS_SINGLE):
+                group_name = attr_name.removeprefix(cls._STARTSWITH__DEFINE__CLS_SINGLE)
+                result.update([group_name, ])
 
+        return result
+
+    # -----------------------------------------------------------------------------------------------------------------
     @classmethod
-    def groups_count__existed(cls) -> int | None:
+    def groups_count__generated(cls) -> int | None:
         """
         work only after called generate__objects(),
         so if you wasnot call generate__objects it will return None!
         """
-        if cls.groups_check__generated():
-            return len(cls._GROUPS)
-
-    # -----------------------------------------------------------------------------------------------------------------
-    @classmethod
-    def group_check__exists(cls, name: str) -> bool:
-        return cls.group_get__type(name) != BreederObjectList_GroupType.NOT_EXISTS
+        if cls.__groups__are_generated:
+            return len(cls.groups__get_names())
 
+    # GROUP -----------------------------------------------------------------------------------------------------------
     @classmethod
     def group_get__type(cls, name: str) -> BreederObjectList_GroupType:
         if f"{cls._STARTSWITH__DEFINE__CLS_SINGLE}{name}" in dir(cls):
             return BreederObjectList_GroupType.SINGLE
 
         if f"{cls._STARTSWITH__DEFINE__CLS_LIST}{name}" in dir(cls):
             return BreederObjectList_GroupType.LIST
 
         return BreederObjectList_GroupType.NOT_EXISTS
 
     @classmethod
-    def group_get__objects(cls, name: str) -> Union[None, Any, list[Any]]:
-        if cls.group_check__exists(name) and cls.groups_check__generated():
-            return cls._GROUPS[name]
+    def group_check__exists(cls, name: str) -> bool:
+        return cls.group_get__type(name) != BreederObjectList_GroupType.NOT_EXISTS
 
     @classmethod
-    def group_call__(cls, meth: str, group: str | None = None, *args, **kwargs) -> Union[NoReturn, TYPE__BREED_RESULT__GROUP, TYPE__BREED_RESULT__GROUPS]:
+    def group_get__cls(cls, name: str) -> Any | None:
+        group_type = cls.group_get__type(name)
+
+        if group_type == BreederObjectList_GroupType.SINGLE:
+            attr = f"{cls._STARTSWITH__DEFINE__CLS_SINGLE}{name}"
+            return getattr(cls, attr)
+
+        if group_type == BreederObjectList_GroupType.LIST:
+            attr = f"{cls._STARTSWITH__DEFINE__CLS_LIST}{name}"
+            return getattr(cls, attr)
+
+    @classmethod
+    def group_get__insts(cls, name: str) -> Union[None, Any, list[Any]]:
+        if cls.group_check__exists(name) and cls.__groups__are_generated:
+            group_cls = cls.group_get__cls(name)
+            result = getattr(group_cls, cls._STARTSWITH__ACCESS__OBJECT_LIST__IN_SOURCE)
+            return result
+
+    @classmethod
+    def group_call__(cls, meth: str, group: str | None = None, args: list | None = None, kwargs: dict | None = None) -> Union[NoReturn, TYPE__BREED_RESULT__GROUP, TYPE__BREED_RESULT__GROUPS]:
         """
         call one method on exact group (every object in group) or all groups (every object in all groups).
         created specially for call connect/disconnect for devices in TP.
 
         :param meth:
         :param group:
 
         :param args:
         :param kwargs:
         :return:
             RAISE only if passed group and group is not exists! or groups are not generated
         """
-        if not cls.groups_check__generated():
+        if not cls.__groups__are_generated:
             raise Exx__BreederObjectList_GroupsNotGenerated()
 
+        args = args or ()
+        kwargs = kwargs or {}
+
         # CALL ON ALL GROUPS -------------------------------------------------
         if group is None:
             results = {}
-            for group_name in cls._GROUPS:
-                results.update({group_name: cls.group_call__(meth, group_name, *args, **kwargs)})
+            for group_name in cls.groups__get_names():
+                results.update({group_name: cls.group_call__(meth, group_name, args, kwargs)})
             return results
 
         # if group is not exists ---------------------------------------------
         if not cls.group_check__exists(group):
             raise Exx__BreederObjectList_GroupNotExists(group)
 
         # EXACT ONE GROUP ----------------------------------------------------
-        group_objs = cls._GROUPS[group]
+        group_objs = cls.group_get__insts(group)
 
         if isinstance(group_objs, list):
             results = []
             for obj in group_objs:
                 try:
                     obj_meth = getattr(obj, meth)
                     obj_result = obj_meth(*args, **kwargs)
@@ -227,9 +243,28 @@
                 obj_result = obj_meth(*args, **kwargs)
             except Exception as exx:
                 obj_result = exx
             results = obj_result
 
         return results
 
+    # -----------------------------------------------------------------------------------------------------------------
+    def __getattr__(self, item: str) -> Union[None, Any, NoReturn]:
+        if self.INDEX is None:
+            return
+
+        # ACCESS TO OBJECT ----------------------------
+        group_insts = self.group_get__insts(item)
+        if group_insts is not None:
+            if isinstance(group_insts, list):
+                inst = group_insts[self.INDEX]
+            else:
+                inst = group_insts
+            return inst
+
+        # FINAL not found -----------------------------
+        msg = f"{item=}/{self.INDEX=}"
+        print(msg)
+        raise Exx__BreederObjectList_GroupNotExists(msg)
+
 
 # =====================================================================================================================
```

### Comparing `funcs_aux-0.2.1/funcs_aux/breeder_str.py` & `funcs_aux-0.2.3/funcs_aux/breeder_str.py`

 * *Files identical despite different names*

### Comparing `funcs_aux-0.2.1/funcs_aux/iterables.py` & `funcs_aux-0.2.3/funcs_aux/iterables.py`

 * *Files identical despite different names*

### Comparing `funcs_aux-0.2.1/funcs_aux/results.py` & `funcs_aux-0.2.3/funcs_aux/results.py`

 * *Files identical despite different names*

### Comparing `funcs_aux-0.2.1/funcs_aux/strings.py` & `funcs_aux-0.2.3/funcs_aux/strings.py`

 * *Files identical despite different names*

### Comparing `funcs_aux-0.2.1/funcs_aux.egg-info/PKG-INFO` & `funcs_aux-0.2.3/funcs_aux.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funcs_aux
-Version: 0.2.1
+Version: 0.2.3
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
 
-# funcs_aux (v0.2.1)
+# funcs_aux (v0.2.3)
 
 ## DESCRIPTION_SHORT
 useful funcs in one place
 
 ## DESCRIPTION_LONG
 Now its just a beginning!
 Designed to collect useful funcs in one place!
```

### Comparing `funcs_aux-0.2.1/setup.py` & `funcs_aux-0.2.3/setup.py`

 * *Files identical despite different names*

