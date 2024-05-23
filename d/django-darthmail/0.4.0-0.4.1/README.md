# Comparing `tmp/django_darthmail-0.4.0.tar.gz` & `tmp/django_darthmail-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_darthmail-0.4.0.tar", last modified: Fri Apr 26 13:41:02 2024, max compression
+gzip compressed data, was "django_darthmail-0.4.1.tar", last modified: Thu May 23 12:46:32 2024, max compression
```

## Comparing `django_darthmail-0.4.0.tar` & `django_darthmail-0.4.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 13:41:02.659423 django_darthmail-0.4.0/
--rw-r--r--   0 root         (0) root         (0)     1465 2024-04-26 13:40:48.000000 django_darthmail-0.4.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       64 2024-04-26 13:40:48.000000 django_darthmail-0.4.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1456 2024-04-26 13:41:02.659423 django_darthmail-0.4.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      593 2024-04-26 13:40:48.000000 django_darthmail-0.4.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 13:41:02.659423 django_darthmail-0.4.0/django_darthmail/
--rw-r--r--   0 root         (0) root         (0)      463 2024-04-26 13:40:48.000000 django_darthmail-0.4.0/django_darthmail/__init__.py
--rw-r--r--   0 root         (0) root         (0)      106 2024-04-26 13:40:48.000000 django_darthmail-0.4.0/django_darthmail/apps.py
--rw-r--r--   0 root         (0) root         (0)     2200 2024-04-26 13:40:48.000000 django_darthmail-0.4.0/django_darthmail/backends.py
--rw-r--r--   0 root         (0) root         (0)     5852 2024-04-26 13:40:48.000000 django_darthmail-0.4.0/django_darthmail/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 13:41:02.659423 django_darthmail-0.4.0/django_darthmail/management/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-26 13:40:48.000000 django_darthmail-0.4.0/django_darthmail/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 13:41:02.659423 django_darthmail-0.4.0/django_darthmail/management/commands/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-26 13:40:48.000000 django_darthmail-0.4.0/django_darthmail/management/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)      823 2024-04-26 13:40:48.000000 django_darthmail-0.4.0/django_darthmail/management/commands/sendtestdarthmail.py
--rw-r--r--   0 root         (0) root         (0)     2157 2024-04-26 13:40:48.000000 django_darthmail-0.4.0/django_darthmail/message.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 13:41:02.659423 django_darthmail-0.4.0/django_darthmail/migrations/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-26 13:40:48.000000 django_darthmail-0.4.0/django_darthmail/migrations/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3747 2024-04-26 13:40:48.000000 django_darthmail-0.4.0/django_darthmail/serializers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-26 13:41:02.659423 django_darthmail-0.4.0/django_darthmail.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1456 2024-04-26 13:41:02.000000 django_darthmail-0.4.0/django_darthmail.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      604 2024-04-26 13:41:02.000000 django_darthmail-0.4.0/django_darthmail.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-26 13:41:02.000000 django_darthmail-0.4.0/django_darthmail.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       29 2024-04-26 13:41:02.000000 django_darthmail-0.4.0/django_darthmail.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2024-04-26 13:41:02.000000 django_darthmail-0.4.0/django_darthmail.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      406 2024-04-26 13:41:02.659423 django_darthmail-0.4.0/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     1876 2024-04-26 13:40:48.000000 django_darthmail-0.4.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 12:46:32.239475 django_darthmail-0.4.1/
+-rw-r--r--   0 root         (0) root         (0)     1465 2024-05-23 12:46:10.000000 django_darthmail-0.4.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       64 2024-05-23 12:46:10.000000 django_darthmail-0.4.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1486 2024-05-23 12:46:32.239475 django_darthmail-0.4.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      593 2024-05-23 12:46:10.000000 django_darthmail-0.4.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 12:46:32.239475 django_darthmail-0.4.1/django_darthmail/
+-rw-r--r--   0 root         (0) root         (0)      463 2024-05-23 12:46:10.000000 django_darthmail-0.4.1/django_darthmail/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      106 2024-05-23 12:46:10.000000 django_darthmail-0.4.1/django_darthmail/apps.py
+-rw-r--r--   0 root         (0) root         (0)     2200 2024-05-23 12:46:10.000000 django_darthmail-0.4.1/django_darthmail/backends.py
+-rw-r--r--   0 root         (0) root         (0)     5852 2024-05-23 12:46:10.000000 django_darthmail-0.4.1/django_darthmail/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 12:46:32.239475 django_darthmail-0.4.1/django_darthmail/management/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 12:46:10.000000 django_darthmail-0.4.1/django_darthmail/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 12:46:32.239475 django_darthmail-0.4.1/django_darthmail/management/commands/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 12:46:10.000000 django_darthmail-0.4.1/django_darthmail/management/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      823 2024-05-23 12:46:10.000000 django_darthmail-0.4.1/django_darthmail/management/commands/sendtestdarthmail.py
+-rw-r--r--   0 root         (0) root         (0)     2157 2024-05-23 12:46:10.000000 django_darthmail-0.4.1/django_darthmail/message.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 12:46:32.239475 django_darthmail-0.4.1/django_darthmail/migrations/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-23 12:46:10.000000 django_darthmail-0.4.1/django_darthmail/migrations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3747 2024-05-23 12:46:10.000000 django_darthmail-0.4.1/django_darthmail/serializers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 12:46:32.239475 django_darthmail-0.4.1/django_darthmail.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1486 2024-05-23 12:46:32.000000 django_darthmail-0.4.1/django_darthmail.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      604 2024-05-23 12:46:32.000000 django_darthmail-0.4.1/django_darthmail.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-23 12:46:32.000000 django_darthmail-0.4.1/django_darthmail.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2024-05-23 12:46:32.000000 django_darthmail-0.4.1/django_darthmail.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2024-05-23 12:46:32.000000 django_darthmail-0.4.1/django_darthmail.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      406 2024-05-23 12:46:32.239475 django_darthmail-0.4.1/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     1902 2024-05-23 12:46:10.000000 django_darthmail-0.4.1/setup.py
```

### Comparing `django_darthmail-0.4.0/LICENSE` & `django_darthmail-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_darthmail-0.4.0/PKG-INFO` & `django_darthmail-0.4.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-darthmail
-Version: 0.4.0
+Version: 0.4.1
 Summary: Client for the DarthMail project
 Home-page: https://github.com/regiohelden/django-darthmail
 Author: RegioHelden GmbH
 Author-email: entwicklung@regiohelden.de
 License: BSD-3-Clause
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
@@ -17,14 +17,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Communications :: Email
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: django>=4.2
 Requires-Dist: requests>=2.31.0
+Requires-Dist: pillow>=10.0.0
 
 # django-darthmail
 
 Module for using darthmail as an EMAIL\_BACKEND in Django.
 
 # Settings
```

### Comparing `django_darthmail-0.4.0/README.md` & `django_darthmail-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `django_darthmail-0.4.0/django_darthmail/backends.py` & `django_darthmail-0.4.1/django_darthmail/backends.py`

 * *Files identical despite different names*

### Comparing `django_darthmail-0.4.0/django_darthmail/client.py` & `django_darthmail-0.4.1/django_darthmail/client.py`

 * *Files identical despite different names*

### Comparing `django_darthmail-0.4.0/django_darthmail/management/commands/sendtestdarthmail.py` & `django_darthmail-0.4.1/django_darthmail/management/commands/sendtestdarthmail.py`

 * *Files identical despite different names*

### Comparing `django_darthmail-0.4.0/django_darthmail/message.py` & `django_darthmail-0.4.1/django_darthmail/message.py`

 * *Files identical despite different names*

### Comparing `django_darthmail-0.4.0/django_darthmail/serializers.py` & `django_darthmail-0.4.1/django_darthmail/serializers.py`

 * *Files identical despite different names*

### Comparing `django_darthmail-0.4.0/django_darthmail.egg-info/PKG-INFO` & `django_darthmail-0.4.1/django_darthmail.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-darthmail
-Version: 0.4.0
+Version: 0.4.1
 Summary: Client for the DarthMail project
 Home-page: https://github.com/regiohelden/django-darthmail
 Author: RegioHelden GmbH
 Author-email: entwicklung@regiohelden.de
 License: BSD-3-Clause
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
@@ -17,14 +17,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Communications :: Email
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: django>=4.2
 Requires-Dist: requests>=2.31.0
+Requires-Dist: pillow>=10.0.0
 
 # django-darthmail
 
 Module for using darthmail as an EMAIL\_BACKEND in Django.
 
 # Settings
```

### Comparing `django_darthmail-0.4.0/django_darthmail.egg-info/SOURCES.txt` & `django_darthmail-0.4.1/django_darthmail.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_darthmail-0.4.0/setup.py` & `django_darthmail-0.4.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,14 +38,15 @@
     author_email='entwicklung@regiohelden.de',
     url='https://github.com/regiohelden/django-darthmail',
 
     include_package_data=True,
     install_requires=[
         "django>=4.2",
         "requests>=2.31.0",
+        "pillow>=10.0.0",
     ],
     license="BSD-3-Clause",
     classifiers=[
         'Development Status :: 4 - Beta',
         'Framework :: Django',
         'Framework :: Django :: 2.2',
         'Intended Audience :: Developers',
```

