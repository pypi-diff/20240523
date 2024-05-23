# Comparing `tmp/phones_local-0.0.23.tar.gz` & `tmp/phones_local-0.0.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phones_local-0.0.23.tar", last modified: Fri May 10 11:16:42 2024, max compression
+gzip compressed data, was "phones_local-0.0.24.tar", last modified: Thu May 23 05:36:22 2024, max compression
```

## Comparing `phones_local-0.0.23.tar` & `phones_local-0.0.24.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:16:42.523249 phones_local-0.0.23/
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-10 11:16:42.523249 phones_local-0.0.23/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-10 11:16:20.000000 phones_local-0.0.23/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:16:42.523249 phones_local-0.0.23/phones_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:16:42.523249 phones_local-0.0.23/phones_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 11:16:20.000000 phones_local-0.0.23/phones_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-10 11:16:20.000000 phones_local-0.0.23/phones_local/src/phone_local_constans.py
--rw-r--r--   0 runner    (1001) docker     (127)     9058 2024-05-10 11:16:20.000000 phones_local-0.0.23/phones_local/src/phones_local.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 11:16:42.523249 phones_local-0.0.23/phones_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-10 11:16:42.000000 phones_local-0.0.23/phones_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-10 11:16:42.000000 phones_local-0.0.23/phones_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 11:16:42.000000 phones_local-0.0.23/phones_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-10 11:16:42.000000 phones_local-0.0.23/phones_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-10 11:16:42.000000 phones_local-0.0.23/phones_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-10 11:16:20.000000 phones_local-0.0.23/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 11:16:42.523249 phones_local-0.0.23/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-10 11:16:20.000000 phones_local-0.0.23/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 05:36:22.031028 phones_local-0.0.24/
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-23 05:36:22.031028 phones_local-0.0.24/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-23 05:35:55.000000 phones_local-0.0.24/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 05:36:22.027027 phones_local-0.0.24/phones_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 05:36:22.031028 phones_local-0.0.24/phones_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 05:35:55.000000 phones_local-0.0.24/phones_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-23 05:35:55.000000 phones_local-0.0.24/phones_local/src/phone_local_constans.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9120 2024-05-23 05:35:55.000000 phones_local-0.0.24/phones_local/src/phones_local.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 05:36:22.031028 phones_local-0.0.24/phones_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-23 05:36:22.000000 phones_local-0.0.24/phones_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-23 05:36:22.000000 phones_local-0.0.24/phones_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 05:36:22.000000 phones_local-0.0.24/phones_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-23 05:36:22.000000 phones_local-0.0.24/phones_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-23 05:36:22.000000 phones_local-0.0.24/phones_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-23 05:35:55.000000 phones_local-0.0.24/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 05:36:22.031028 phones_local-0.0.24/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-23 05:35:55.000000 phones_local-0.0.24/setup.py
```

### Comparing `phones_local-0.0.23/PKG-INFO` & `phones_local-0.0.24/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phones-local
-Version: 0.0.23
+Version: 0.0.24
 Home-page: https://github.com/circles-zone/phones-local-python-package
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `phones_local-0.0.23/README.md` & `phones_local-0.0.24/README.md`

 * *Files identical despite different names*

### Comparing `phones_local-0.0.23/phones_local/src/phone_local_constans.py` & `phones_local-0.0.24/phones_local/src/phone_local_constans.py`

 * *Files identical despite different names*

### Comparing `phones_local-0.0.23/phones_local/src/phones_local.py` & `phones_local-0.0.24/phones_local/src/phones_local.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,39 +11,39 @@
 
 
 class PhonesLocal(GenericMapping):
     def __init__(self) -> None:
         super().__init__(default_schema_name="phone",
                          default_table_name="phone_table",
                          default_view_table_name="phone_view",
-                         default_id_column_name="phone_id")
+                         default_column_name="phone_id")
 
     def get_normalized_phone_number_by_phone_id(self, phone_id: int) -> int:
         logger.start(object={"phone_id": phone_id})
-        data = self.select_one_dict_by_id(select_clause_value="local_number_normalized",
-                                          id_column_value=phone_id)
+        data = self.select_one_dict_by_column_and_value(select_clause_value="local_number_normalized",
+                                          column_value=phone_id)
         if not data:
             logger.end("No phone number found for phone_id " +
                        str(phone_id))
         else:
             phone_number = int(data["local_number_normalized"])
             logger.end("Return Phone Number of a specific phone id",
                        object={'phone_number': phone_number})
             return phone_number  # TODO: should we add area_code?
 
     def verify_phone_number(self, phone_number: int) -> None:
         logger.start(object={"phone_number": phone_number})
-        self.update_by_id(id_column_value=phone_number,
-                          data_json={"is_verified": 1})
+        self.update_by_column_and_value(column_value=phone_number,
+                          data_dict={"is_verified": 1})
         logger.end()
 
     def is_verified(self, phone_number: int) -> bool:
         logger.start(object={"phone_number": phone_number})
-        data = self.select_one_dict_by_id(select_clause_value="is_verified",
-                                          id_column_value=phone_number)
+        data = self.select_one_dict_by_column_and_value(select_clause_value="is_verified",
+                                          column_value=phone_number)
         if not data:
             logger.end("No phone number found for phone_number " +
                        str(phone_number))
             return False
         is_verified = data["is_verified"]
         logger.end("Return is_verified of a specific phone id",
                    object={'is_verified': is_verified})
@@ -85,32 +85,32 @@
         profile_id = user_context.get_effective_profile_id()
         location_id = None  # user_context.get_effective_location_id()
         country_id = None  # user_context.get_effective_country_id()
 
         if not country_id:  # get country_id from location_id
             if not location_id:  # get location_id from contact_id or profile_id
                 if contact_id and not profile_id:  # get profile_id from contact_id
-                    profile_id = self.select_one_value_by_id(
+                    profile_id = self.select_one_value_by_column_and_value(
                         schema_name="contact_profile",
                         view_table_name='contact_profile_view', select_clause_value='profile_id',
-                        id_column_name='contact_id', id_column_value=contact_id)
+                        column_name='contact_id', column_value=contact_id)
                 assert profile_id, "profile_id is required for getting location_id"
-                location_id = self.select_one_value_by_id(
+                location_id = self.select_one_value_by_column_and_value(
                     schema_name="location_profile",
                     view_table_name='location_profile_view', select_clause_value='location_id',
-                    id_column_name='profile_id', id_column_value=profile_id)
+                    column_name='profile_id', column_value=profile_id)
 
             assert location_id, "location_id is required for getting country_id"
-            country_id = self.select_one_value_by_id(
+            country_id = self.select_one_value_by_column_and_value(
                 schema_name="location", view_table_name='location_view', select_clause_value='country_id',
-                id_column_name='location_id', id_column_value=location_id)
+                column_name='location_id', column_value=location_id)
 
-        country_iso_code = self.select_one_value_by_id(
+        country_iso_code = self.select_one_value_by_column_and_value(
             schema_name="country", view_table_name='country_ml_view', select_clause_value='iso',
-            id_column_name='country_id', id_column_value=country_id)
+            column_name='country_id', column_value=country_id)
         return country_iso_code
 
     # TODO: Is it really necessary to access the database for location?
     # I think it's possible to get the normalized phone number and the international code
     # from original_phone_number
     def process_phone(self, original_phone_number: str, country_iso_code: str = None, contact_id: int = None) -> dict:
         """
@@ -128,15 +128,15 @@
             'number_original': original_phone_number,
             'international_code': normalized_phone_number['international_code'],
             'full_number_normalized': normalized_phone_number['full_number_normalized'],
             'local_number_normalized': int(str(normalized_phone_number['full_number_normalized'])
                                            .replace(str(normalized_phone_number['international_code']), '')),
             'created_user_id': logger.user_context.get_effective_user_id(),
         }
-        phone_id = self.insert(data_json=phone_data)
+        phone_id = self.insert(data_dict=phone_data)
 
         # link phone to profile
         profile_id = user_context.get_effective_profile_id()
         if profile_id:
             phone_profile_id = self.insert_mapping(
                 schema_name='phone_profile',
                 entity_name1='phone', entity_name2='profile', entity_id1=phone_id, entity_id2=profile_id)
@@ -164,15 +164,15 @@
     def insert_phone(self, phone_data: dict) -> int:
         """
         Insert phone data into the phone table.
         :param phone_data: Dictionary with the phone data.
         :return: Phone id.
         """
         logger.start(object={'phone_data': phone_data})
-        phone_id = self.insert(data_json=phone_data)
+        phone_id = self.insert(data_dict=phone_data)
         logger.end("success inserting phone", object={'phone_id': phone_id})
         return phone_id
 
     def get_test_phone_id(self, number_original: str, international_code: int = 972) -> int:
         phone_data = {
             'number_original': number_original,
             'local_number_normalized': int(number_original[3:]),  # must be unique
```

### Comparing `phones_local-0.0.23/phones_local.egg-info/PKG-INFO` & `phones_local-0.0.24/phones_local.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phones-local
-Version: 0.0.23
+Version: 0.0.24
 Home-page: https://github.com/circles-zone/phones-local-python-package
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `phones_local-0.0.23/pyproject.toml` & `phones_local-0.0.24/pyproject.toml`

 * *Files identical despite different names*

### Comparing `phones_local-0.0.23/setup.py` & `phones_local-0.0.24/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "phones-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,
-    version='0.0.23',  # https://pypi.org/project/phones-local/
+    version='0.0.24',  # https://pypi.org/project/phones-local/
     author="Circles",
     author_email="info@circles.ai",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
     package_dir={package_dir: f'{package_dir}/src'},
     package_data={package_dir: ['*.py']},
     long_description="PyPI Package for Circles phone local Python",
```

