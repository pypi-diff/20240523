# Comparing `tmp/heaobject-1.6.0.tar.gz` & `tmp/heaobject-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heaobject-1.6.0.tar", last modified: Tue May 21 22:49:58 2024, max compression
+gzip compressed data, was "heaobject-1.6.1.tar", last modified: Thu May 23 21:43:23 2024, max compression
```

## Comparing `heaobject-1.6.0.tar` & `heaobject-1.6.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 22:49:58.480852 heaobject-1.6.0/
--rw-rw-rw-   0        0        0    11625 2022-03-11 01:28:08.000000 heaobject-1.6.0/LICENSE
--rw-rw-rw-   0        0        0     6085 2024-05-21 22:49:58.479271 heaobject-1.6.0/PKG-INFO
--rw-rw-rw-   0        0        0     4579 2024-05-21 22:47:32.000000 heaobject-1.6.0/README.md
--rw-rw-rw-   0        0        0       42 2024-05-21 22:49:58.480852 heaobject-1.6.0/setup.cfg
--rw-rw-rw-   0        0        0     2603 2024-05-21 22:49:15.000000 heaobject-1.6.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-21 22:49:58.410035 heaobject-1.6.0/src/
-drwxrwxrwx   0        0        0        0 2024-05-21 22:49:58.467310 heaobject-1.6.0/src/heaobject/
--rw-rw-rw-   0        0        0     1247 2023-12-16 22:23:08.000000 heaobject-1.6.0/src/heaobject/__init__.py
--rw-rw-rw-   0        0        0    11351 2024-05-21 22:47:32.000000 heaobject-1.6.0/src/heaobject/account.py
--rw-rw-rw-   0        0        0    15629 2024-04-09 20:34:56.000000 heaobject-1.6.0/src/heaobject/activity.py
--rw-rw-rw-   0        0        0     4030 2023-12-16 22:23:08.000000 heaobject-1.6.0/src/heaobject/aws.py
--rw-rw-rw-   0        0        0     6945 2023-12-16 22:23:08.000000 heaobject-1.6.0/src/heaobject/awss3key.py
--rw-rw-rw-   0        0        0     7587 2024-04-09 20:34:56.000000 heaobject-1.6.0/src/heaobject/bucket.py
--rw-rw-rw-   0        0        0     9988 2024-05-21 22:47:32.000000 heaobject-1.6.0/src/heaobject/data.py
--rw-rw-rw-   0        0        0     2604 2023-12-16 22:23:08.000000 heaobject-1.6.0/src/heaobject/dataadapter.py
--rw-rw-rw-   0        0        0      272 2022-03-11 01:28:08.000000 heaobject-1.6.0/src/heaobject/dataelement.py
--rw-rw-rw-   0        0        0     1601 2022-03-11 01:28:08.000000 heaobject-1.6.0/src/heaobject/datamodel.py
--rw-rw-rw-   0        0        0      430 2022-03-11 01:28:08.000000 heaobject-1.6.0/src/heaobject/datapattern.py
--rw-rw-rw-   0        0        0      238 2023-12-16 22:23:08.000000 heaobject-1.6.0/src/heaobject/datatransform.py
--rw-rw-rw-   0        0        0      353 2023-12-16 22:23:08.000000 heaobject-1.6.0/src/heaobject/error.py
--rw-rw-rw-   0        0        0    22016 2024-04-09 20:34:56.000000 heaobject-1.6.0/src/heaobject/folder.py
--rw-rw-rw-   0        0        0     4566 2024-05-21 22:47:32.000000 heaobject-1.6.0/src/heaobject/keychain.py
--rw-rw-rw-   0        0        0     2859 2024-04-09 20:34:56.000000 heaobject-1.6.0/src/heaobject/mimetype.py
--rw-rw-rw-   0        0        0    11029 2024-05-21 22:47:32.000000 heaobject-1.6.0/src/heaobject/organization.py
--rw-rw-rw-   0        0        0    13108 2024-05-21 22:47:32.000000 heaobject-1.6.0/src/heaobject/person.py
--rw-rw-rw-   0        0        0     5129 2024-04-09 20:34:56.000000 heaobject-1.6.0/src/heaobject/project.py
--rw-rw-rw-   0        0        0        0 2022-03-11 01:28:08.000000 heaobject-1.6.0/src/heaobject/py.typed
--rw-rw-rw-   0        0        0      211 2024-04-09 20:34:56.000000 heaobject-1.6.0/src/heaobject/record.py
--rw-rw-rw-   0        0        0    23400 2024-05-21 22:47:32.000000 heaobject-1.6.0/src/heaobject/registry.py
--rw-rw-rw-   0        0        0    80257 2024-04-24 17:43:21.000000 heaobject-1.6.0/src/heaobject/root.py
--rw-rw-rw-   0        0        0      597 2024-04-09 20:34:56.000000 heaobject-1.6.0/src/heaobject/settings.py
--rw-rw-rw-   0        0        0       66 2024-03-26 22:41:59.000000 heaobject-1.6.0/src/heaobject/source.py
--rw-rw-rw-   0        0        0     1165 2023-12-16 22:23:08.000000 heaobject-1.6.0/src/heaobject/source2target.py
--rw-rw-rw-   0        0        0     4074 2024-04-09 20:34:56.000000 heaobject-1.6.0/src/heaobject/storage.py
--rw-rw-rw-   0        0        0    10289 2024-04-18 02:00:20.000000 heaobject-1.6.0/src/heaobject/trash.py
--rw-rw-rw-   0        0        0     1217 2024-05-21 22:47:32.000000 heaobject-1.6.0/src/heaobject/user.py
--rw-rw-rw-   0        0        0      498 2023-12-16 22:23:08.000000 heaobject-1.6.0/src/heaobject/util.py
--rw-rw-rw-   0        0        0     7290 2024-05-21 22:47:32.000000 heaobject-1.6.0/src/heaobject/volume.py
-drwxrwxrwx   0        0        0        0 2024-05-21 22:49:58.477736 heaobject-1.6.0/src/heaobject.egg-info/
--rw-rw-rw-   0        0        0     6085 2024-05-21 22:49:58.000000 heaobject-1.6.0/src/heaobject.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      995 2024-05-21 22:49:58.000000 heaobject-1.6.0/src/heaobject.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 22:49:58.000000 heaobject-1.6.0/src/heaobject.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      144 2024-05-21 22:49:58.000000 heaobject-1.6.0/src/heaobject.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-21 22:49:58.000000 heaobject-1.6.0/src/heaobject.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-23 21:43:23.833848 heaobject-1.6.1/
+-rw-rw-rw-   0        0        0    11625 2022-03-11 01:28:08.000000 heaobject-1.6.1/LICENSE
+-rw-rw-rw-   0        0        0     6203 2024-05-23 21:43:23.831848 heaobject-1.6.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4697 2024-05-23 21:42:03.000000 heaobject-1.6.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-23 21:43:23.833848 heaobject-1.6.1/setup.cfg
+-rw-rw-rw-   0        0        0     2603 2024-05-23 21:42:51.000000 heaobject-1.6.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-23 21:43:23.770849 heaobject-1.6.1/src/
+drwxrwxrwx   0        0        0        0 2024-05-23 21:43:23.822847 heaobject-1.6.1/src/heaobject/
+-rw-rw-rw-   0        0        0     1247 2023-12-16 22:23:08.000000 heaobject-1.6.1/src/heaobject/__init__.py
+-rw-rw-rw-   0        0        0    11351 2024-05-21 22:51:17.000000 heaobject-1.6.1/src/heaobject/account.py
+-rw-rw-rw-   0        0        0    15629 2024-04-09 20:34:56.000000 heaobject-1.6.1/src/heaobject/activity.py
+-rw-rw-rw-   0        0        0     4030 2023-12-16 22:23:08.000000 heaobject-1.6.1/src/heaobject/aws.py
+-rw-rw-rw-   0        0        0     6945 2023-12-16 22:23:08.000000 heaobject-1.6.1/src/heaobject/awss3key.py
+-rw-rw-rw-   0        0        0     7587 2024-04-09 20:34:56.000000 heaobject-1.6.1/src/heaobject/bucket.py
+-rw-rw-rw-   0        0        0     9988 2024-05-21 22:51:17.000000 heaobject-1.6.1/src/heaobject/data.py
+-rw-rw-rw-   0        0        0     2604 2023-12-16 22:23:08.000000 heaobject-1.6.1/src/heaobject/dataadapter.py
+-rw-rw-rw-   0        0        0      272 2022-03-11 01:28:08.000000 heaobject-1.6.1/src/heaobject/dataelement.py
+-rw-rw-rw-   0        0        0     1601 2022-03-11 01:28:08.000000 heaobject-1.6.1/src/heaobject/datamodel.py
+-rw-rw-rw-   0        0        0      430 2022-03-11 01:28:08.000000 heaobject-1.6.1/src/heaobject/datapattern.py
+-rw-rw-rw-   0        0        0      238 2023-12-16 22:23:08.000000 heaobject-1.6.1/src/heaobject/datatransform.py
+-rw-rw-rw-   0        0        0      353 2023-12-16 22:23:08.000000 heaobject-1.6.1/src/heaobject/error.py
+-rw-rw-rw-   0        0        0    22016 2024-04-09 20:34:56.000000 heaobject-1.6.1/src/heaobject/folder.py
+-rw-rw-rw-   0        0        0     4566 2024-05-21 22:51:17.000000 heaobject-1.6.1/src/heaobject/keychain.py
+-rw-rw-rw-   0        0        0     2859 2024-04-09 20:34:56.000000 heaobject-1.6.1/src/heaobject/mimetype.py
+-rw-rw-rw-   0        0        0    11772 2024-05-23 19:02:21.000000 heaobject-1.6.1/src/heaobject/organization.py
+-rw-rw-rw-   0        0        0    13108 2024-05-21 22:51:17.000000 heaobject-1.6.1/src/heaobject/person.py
+-rw-rw-rw-   0        0        0     5129 2024-04-09 20:34:56.000000 heaobject-1.6.1/src/heaobject/project.py
+-rw-rw-rw-   0        0        0        0 2022-03-11 01:28:08.000000 heaobject-1.6.1/src/heaobject/py.typed
+-rw-rw-rw-   0        0        0      211 2024-04-09 20:34:56.000000 heaobject-1.6.1/src/heaobject/record.py
+-rw-rw-rw-   0        0        0    23400 2024-05-21 22:51:17.000000 heaobject-1.6.1/src/heaobject/registry.py
+-rw-rw-rw-   0        0        0    80257 2024-04-24 17:43:21.000000 heaobject-1.6.1/src/heaobject/root.py
+-rw-rw-rw-   0        0        0      597 2024-04-09 20:34:56.000000 heaobject-1.6.1/src/heaobject/settings.py
+-rw-rw-rw-   0        0        0       66 2024-03-26 22:41:59.000000 heaobject-1.6.1/src/heaobject/source.py
+-rw-rw-rw-   0        0        0     1165 2023-12-16 22:23:08.000000 heaobject-1.6.1/src/heaobject/source2target.py
+-rw-rw-rw-   0        0        0     4074 2024-04-09 20:34:56.000000 heaobject-1.6.1/src/heaobject/storage.py
+-rw-rw-rw-   0        0        0    10289 2024-04-18 02:00:20.000000 heaobject-1.6.1/src/heaobject/trash.py
+-rw-rw-rw-   0        0        0     1217 2024-05-21 22:51:17.000000 heaobject-1.6.1/src/heaobject/user.py
+-rw-rw-rw-   0        0        0      498 2023-12-16 22:23:08.000000 heaobject-1.6.1/src/heaobject/util.py
+-rw-rw-rw-   0        0        0     7290 2024-05-21 22:51:17.000000 heaobject-1.6.1/src/heaobject/volume.py
+drwxrwxrwx   0        0        0        0 2024-05-23 21:43:23.830848 heaobject-1.6.1/src/heaobject.egg-info/
+-rw-rw-rw-   0        0        0     6203 2024-05-23 21:43:23.000000 heaobject-1.6.1/src/heaobject.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      995 2024-05-23 21:43:23.000000 heaobject-1.6.1/src/heaobject.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 21:43:23.000000 heaobject-1.6.1/src/heaobject.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      144 2024-05-23 21:43:23.000000 heaobject-1.6.1/src/heaobject.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-23 21:43:23.000000 heaobject-1.6.1/src/heaobject.egg-info/top_level.txt
```

### Comparing `heaobject-1.6.0/LICENSE` & `heaobject-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `heaobject-1.6.0/PKG-INFO` & `heaobject-1.6.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaobject
-Version: 1.6.0
+Version: 1.6.1
 Summary: Data and other classes that are passed into and out of HEA REST APIs.
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -33,14 +33,17 @@
 Requires-Dist: mimetype-description~=0.1.0
 
 # HEA Object Library
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://healthcare.utah.edu/huntsmancancerinstitute/), Salt Lake City, UT
 
 The HEA Object Library contains data and other classes that are passed into and out of HEA REST APIs.
 
+## Version 1.6.1
+* For heaobject.organization.Organization, managers can now modify the manager and member lists.
+
 ## Version 1.6.0
 * Replaced heaobject.keychain.AWSCredentials role_arn attribute with a role attribute on heaobject.keychain.Credentials objects.
 * Added group_ids attribute to heaobject.person.Person.
 * New attributes in heaobject.account.Account: file_system_type, file_system_name.
 * New methods in heaobject.account.Account: get_role_to_assume(), and new_credentials().
 * Added full_name attribute to Person that is mirrors display_name.
 * Removed file_system_name parameter from queries of a registry Component's
```

### Comparing `heaobject-1.6.0/README.md` & `heaobject-1.6.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 # HEA Object Library
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://healthcare.utah.edu/huntsmancancerinstitute/), Salt Lake City, UT
 
 The HEA Object Library contains data and other classes that are passed into and out of HEA REST APIs.
 
+## Version 1.6.1
+* For heaobject.organization.Organization, managers can now modify the manager and member lists.
+
 ## Version 1.6.0
 * Replaced heaobject.keychain.AWSCredentials role_arn attribute with a role attribute on heaobject.keychain.Credentials objects.
 * Added group_ids attribute to heaobject.person.Person.
 * New attributes in heaobject.account.Account: file_system_type, file_system_name.
 * New methods in heaobject.account.Account: get_role_to_assume(), and new_credentials().
 * Added full_name attribute to Person that is mirrors display_name.
 * Removed file_system_name parameter from queries of a registry Component's
```

### Comparing `heaobject-1.6.0/setup.py` & `heaobject-1.6.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from os import path
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(name='heaobject',
-                 version='1.6.0',
+                 version='1.6.1',
                  description='Data and other classes that are passed into and out of HEA REST APIs.',
                  long_description=long_description,
                  long_description_content_type='text/markdown',
                  url='https://risr.hci.utah.edu',
                  author='Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT',
                  author_email='Andrew.Post@hci.utah.edu',
                  python_requires='>=3.10',
```

### Comparing `heaobject-1.6.0/src/heaobject/__init__.py` & `heaobject-1.6.1/src/heaobject/__init__.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.6.0/src/heaobject/account.py` & `heaobject-1.6.1/src/heaobject/account.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.6.0/src/heaobject/activity.py` & `heaobject-1.6.1/src/heaobject/activity.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.6.0/src/heaobject/aws.py` & `heaobject-1.6.1/src/heaobject/aws.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.6.0/src/heaobject/awss3key.py` & `heaobject-1.6.1/src/heaobject/awss3key.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.6.0/src/heaobject/bucket.py` & `heaobject-1.6.1/src/heaobject/bucket.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.6.0/src/heaobject/data.py` & `heaobject-1.6.1/src/heaobject/data.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.6.0/src/heaobject/dataadapter.py` & `heaobject-1.6.1/src/heaobject/dataadapter.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.6.0/src/heaobject/datamodel.py` & `heaobject-1.6.1/src/heaobject/datamodel.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.6.0/src/heaobject/folder.py` & `heaobject-1.6.1/src/heaobject/folder.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.6.0/src/heaobject/keychain.py` & `heaobject-1.6.1/src/heaobject/keychain.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.6.0/src/heaobject/mimetype.py` & `heaobject-1.6.1/src/heaobject/mimetype.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.6.0/src/heaobject/organization.py` & `heaobject-1.6.1/src/heaobject/organization.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 import logging
 
-from .root import Permission, AbstractDesktopObject
+from .root import Permission
 from .data import DataObject, SameMimeType
-from .user import NONE_USER
-from .person import Group
-from typing import Optional
-from copy import deepcopy
+from typing import Optional, Callable
 from enum import Enum
 
 permission_id_dict = {
     'admin_ids': [Permission.COOWNER],
     'manager_ids': [Permission.VIEWER, Permission.EDITOR, Permission.SHARER],
     'member_ids': [Permission.VIEWER, Permission.SHARER]
 }
@@ -295,14 +292,29 @@
         return list(groups)
 
     @property
     def type_display_name(self) -> str:
         return "Organization"
 
     def get_attribute_permissions(self, sub: str, attr: str) -> list[Permission]:
-        if attr in ('admin_ids', 'manager_ids', 'member_ids', 'principal_investigator_id', 'admin_group_ids', 'manager_group_ids', 'member_group_ids'):
-            perms = self.get_permissions(sub)
-            if Permission.COOWNER in perms:
+        """
+        The admin_ids, admin_group_ids, manager_group_ids, and member_group_ids attributes are editable if the user has
+        COOWNER permissions. The manager_ids, member_ids, and principal_investigator_id fields are editable if the user
+        has COOWNER or EDITOR permissions. Other permissions are set by the superclass' implementation of this method.
+
+        :param sub: the user to check.
+        :param attr: the attribute to check.
+        :return: the permissions for the attribute.
+        """
+        def check_perms(perms_checker: Callable[[], bool]) -> list[Permission]:
+            if perms_checker():
                 return [Permission.VIEWER, Permission.EDITOR]
             else:
                 return [Permission.VIEWER]
+
+        if attr in ('admin_ids', 'admin_group_ids', 'manager_group_ids', 'member_group_ids'):
+            perms = self.get_permissions(sub)
+            return check_perms(lambda: Permission.COOWNER in perms)
+        elif attr in ('manager_ids', 'member_ids', 'principal_investigator_id'):
+            perms = self.get_permissions(sub)
+            return check_perms(lambda: Permission.COOWNER in perms or Permission.EDITOR in perms)
         return super().get_attribute_permissions(sub, attr)
```

### Comparing `heaobject-1.6.0/src/heaobject/person.py` & `heaobject-1.6.1/src/heaobject/person.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.6.0/src/heaobject/project.py` & `heaobject-1.6.1/src/heaobject/project.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.6.0/src/heaobject/registry.py` & `heaobject-1.6.1/src/heaobject/registry.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.6.0/src/heaobject/root.py` & `heaobject-1.6.1/src/heaobject/root.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.6.0/src/heaobject/settings.py` & `heaobject-1.6.1/src/heaobject/settings.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.6.0/src/heaobject/source2target.py` & `heaobject-1.6.1/src/heaobject/source2target.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.6.0/src/heaobject/storage.py` & `heaobject-1.6.1/src/heaobject/storage.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.6.0/src/heaobject/trash.py` & `heaobject-1.6.1/src/heaobject/trash.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.6.0/src/heaobject/user.py` & `heaobject-1.6.1/src/heaobject/user.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.6.0/src/heaobject/volume.py` & `heaobject-1.6.1/src/heaobject/volume.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.6.0/src/heaobject.egg-info/PKG-INFO` & `heaobject-1.6.1/src/heaobject.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaobject
-Version: 1.6.0
+Version: 1.6.1
 Summary: Data and other classes that are passed into and out of HEA REST APIs.
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -33,14 +33,17 @@
 Requires-Dist: mimetype-description~=0.1.0
 
 # HEA Object Library
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://healthcare.utah.edu/huntsmancancerinstitute/), Salt Lake City, UT
 
 The HEA Object Library contains data and other classes that are passed into and out of HEA REST APIs.
 
+## Version 1.6.1
+* For heaobject.organization.Organization, managers can now modify the manager and member lists.
+
 ## Version 1.6.0
 * Replaced heaobject.keychain.AWSCredentials role_arn attribute with a role attribute on heaobject.keychain.Credentials objects.
 * Added group_ids attribute to heaobject.person.Person.
 * New attributes in heaobject.account.Account: file_system_type, file_system_name.
 * New methods in heaobject.account.Account: get_role_to_assume(), and new_credentials().
 * Added full_name attribute to Person that is mirrors display_name.
 * Removed file_system_name parameter from queries of a registry Component's
```

### Comparing `heaobject-1.6.0/src/heaobject.egg-info/SOURCES.txt` & `heaobject-1.6.1/src/heaobject.egg-info/SOURCES.txt`

 * *Files identical despite different names*

