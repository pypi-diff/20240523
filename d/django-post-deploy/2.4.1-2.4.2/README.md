# Comparing `tmp/django_post_deploy-2.4.1.tar.gz` & `tmp/django_post_deploy-2.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_post_deploy-2.4.1.tar", last modified: Wed May 22 15:07:55 2024, max compression
+gzip compressed data, was "django_post_deploy-2.4.2.tar", last modified: Thu May 23 12:40:15 2024, max compression
```

## Comparing `django_post_deploy-2.4.1.tar` & `django_post_deploy-2.4.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 erlend     (501) staff       (20)        0 2024-05-22 15:07:55.405811 django_post_deploy-2.4.1/
--rw-r--r--   0 erlend     (501) staff       (20)      237 2024-05-22 13:15:43.000000 django_post_deploy-2.4.1/MANIFEST.in
--rw-r--r--   0 erlend     (501) staff       (20)     6360 2024-05-22 15:07:55.405745 django_post_deploy-2.4.1/PKG-INFO
--rw-r--r--   0 erlend     (501) staff       (20)     5701 2024-05-22 13:17:21.000000 django_post_deploy-2.4.1/README.md
-drwxr-xr-x   0 erlend     (501) staff       (20)        0 2024-05-22 15:07:55.405506 django_post_deploy-2.4.1/django_post_deploy.egg-info/
--rw-r--r--   0 erlend     (501) staff       (20)     6360 2024-05-22 15:07:55.000000 django_post_deploy-2.4.1/django_post_deploy.egg-info/PKG-INFO
--rw-r--r--   0 erlend     (501) staff       (20)      935 2024-05-22 15:07:55.000000 django_post_deploy-2.4.1/django_post_deploy.egg-info/SOURCES.txt
--rw-r--r--   0 erlend     (501) staff       (20)        1 2024-05-22 15:07:55.000000 django_post_deploy-2.4.1/django_post_deploy.egg-info/dependency_links.txt
--rw-r--r--   0 erlend     (501) staff       (20)        7 2024-05-22 15:07:55.000000 django_post_deploy-2.4.1/django_post_deploy.egg-info/requires.txt
--rw-r--r--   0 erlend     (501) staff       (20)       12 2024-05-22 15:07:55.000000 django_post_deploy-2.4.1/django_post_deploy.egg-info/top_level.txt
-drwxr-xr-x   0 erlend     (501) staff       (20)        0 2024-05-22 15:07:55.403872 django_post_deploy-2.4.1/post_deploy/
--rw-r--r--   0 erlend     (501) staff       (20)    20137 2024-05-22 12:55:59.000000 django_post_deploy-2.4.1/post_deploy/LICENSE.txt
--rw-r--r--   0 erlend     (501) staff       (20)      121 2024-05-22 14:17:09.000000 django_post_deploy-2.4.1/post_deploy/README.md
--rw-r--r--   0 erlend     (501) staff       (20)       82 2024-05-22 15:04:29.000000 django_post_deploy-2.4.1/post_deploy/__init__.py
--rw-r--r--   0 erlend     (501) staff       (20)       56 2024-05-22 12:55:59.000000 django_post_deploy-2.4.1/post_deploy/errors.py
--rw-r--r--   0 erlend     (501) staff       (20)     2120 2024-05-22 12:55:59.000000 django_post_deploy-2.4.1/post_deploy/local_utils.py
-drwxr-xr-x   0 erlend     (501) staff       (20)        0 2024-05-22 15:07:55.401319 django_post_deploy-2.4.1/post_deploy/management/
-drwxr-xr-x   0 erlend     (501) staff       (20)        0 2024-05-22 15:07:55.403964 django_post_deploy-2.4.1/post_deploy/management/commands/
--rw-r--r--   0 erlend     (501) staff       (20)     6666 2024-05-22 13:04:35.000000 django_post_deploy-2.4.1/post_deploy/management/commands/deploy.py
-drwxr-xr-x   0 erlend     (501) staff       (20)        0 2024-05-22 15:07:55.404370 django_post_deploy-2.4.1/post_deploy/migrations/
--rw-r--r--   0 erlend     (501) staff       (20)     1123 2024-05-22 13:04:35.000000 django_post_deploy-2.4.1/post_deploy/migrations/0001_initial.py
--rw-r--r--   0 erlend     (501) staff       (20)     1871 2024-05-22 13:04:35.000000 django_post_deploy-2.4.1/post_deploy/migrations/0002_postdeploylog.py
--rw-r--r--   0 erlend     (501) staff       (20)        0 2024-05-22 12:55:59.000000 django_post_deploy-2.4.1/post_deploy/migrations/__init__.py
--rw-r--r--   0 erlend     (501) staff       (20)     4533 2024-05-22 12:55:59.000000 django_post_deploy-2.4.1/post_deploy/models.py
-drwxr-xr-x   0 erlend     (501) staff       (20)        0 2024-05-22 15:07:55.404452 django_post_deploy-2.4.1/post_deploy/plugins/
--rw-r--r--   0 erlend     (501) staff       (20)        0 2024-05-22 12:55:59.000000 django_post_deploy-2.4.1/post_deploy/plugins/__init__.py
-drwxr-xr-x   0 erlend     (501) staff       (20)        0 2024-05-22 15:07:55.404646 django_post_deploy-2.4.1/post_deploy/plugins/context/
--rw-r--r--   0 erlend     (501) staff       (20)      280 2024-05-22 12:55:59.000000 django_post_deploy-2.4.1/post_deploy/plugins/context/__init__.py
--rw-r--r--   0 erlend     (501) staff       (20)      439 2024-05-22 13:04:35.000000 django_post_deploy-2.4.1/post_deploy/plugins/context/tenant.py
-drwxr-xr-x   0 erlend     (501) staff       (20)        0 2024-05-22 15:07:55.404867 django_post_deploy-2.4.1/post_deploy/plugins/scheduler/
--rw-r--r--   0 erlend     (501) staff       (20)      291 2024-05-22 12:55:59.000000 django_post_deploy-2.4.1/post_deploy/plugins/scheduler/__init__.py
--rw-r--r--   0 erlend     (501) staff       (20)     1311 2024-05-22 13:04:35.000000 django_post_deploy-2.4.1/post_deploy/plugins/scheduler/celery.py
--rw-r--r--   0 erlend     (501) staff       (20)      369 2024-05-22 12:55:59.000000 django_post_deploy-2.4.1/post_deploy/tasks.py
-drwxr-xr-x   0 erlend     (501) staff       (20)        0 2024-05-22 15:07:55.405294 django_post_deploy-2.4.1/post_deploy/tests/
--rw-r--r--   0 erlend     (501) staff       (20)        0 2024-05-22 12:55:59.000000 django_post_deploy-2.4.1/post_deploy/tests/__init__.py
--rw-r--r--   0 erlend     (501) staff       (20)     2472 2024-05-22 12:55:59.000000 django_post_deploy-2.4.1/post_deploy/tests/test_decorator.py
--rw-r--r--   0 erlend     (501) staff       (20)     5323 2024-05-22 12:55:59.000000 django_post_deploy-2.4.1/post_deploy/tests/test_log_queryset.py
--rw-r--r--   0 erlend     (501) staff       (20)     7172 2024-05-22 13:04:35.000000 django_post_deploy-2.4.1/post_deploy/tests/test_management_command.py
--rw-r--r--   0 erlend     (501) staff       (20)     2094 2024-05-22 15:04:11.000000 django_post_deploy-2.4.1/post_deploy/utils.py
--rw-r--r--   0 erlend     (501) staff       (20)       76 2024-05-22 15:07:55.406035 django_post_deploy-2.4.1/setup.cfg
--rw-r--r--   0 erlend     (501) staff       (20)     1045 2024-05-22 14:15:07.000000 django_post_deploy-2.4.1/setup.py
+drwxr-xr-x   0 erlend     (501) staff       (20)        0 2024-05-23 12:40:15.924801 django_post_deploy-2.4.2/
+-rw-r--r--   0 erlend     (501) staff       (20)      237 2024-05-22 13:15:43.000000 django_post_deploy-2.4.2/MANIFEST.in
+-rw-r--r--   0 erlend     (501) staff       (20)     6360 2024-05-23 12:40:15.924749 django_post_deploy-2.4.2/PKG-INFO
+-rw-r--r--   0 erlend     (501) staff       (20)     5701 2024-05-22 13:17:21.000000 django_post_deploy-2.4.2/README.md
+drwxr-xr-x   0 erlend     (501) staff       (20)        0 2024-05-23 12:40:15.924597 django_post_deploy-2.4.2/django_post_deploy.egg-info/
+-rw-r--r--   0 erlend     (501) staff       (20)     6360 2024-05-23 12:40:15.000000 django_post_deploy-2.4.2/django_post_deploy.egg-info/PKG-INFO
+-rw-r--r--   0 erlend     (501) staff       (20)      935 2024-05-23 12:40:15.000000 django_post_deploy-2.4.2/django_post_deploy.egg-info/SOURCES.txt
+-rw-r--r--   0 erlend     (501) staff       (20)        1 2024-05-23 12:40:15.000000 django_post_deploy-2.4.2/django_post_deploy.egg-info/dependency_links.txt
+-rw-r--r--   0 erlend     (501) staff       (20)        7 2024-05-23 12:40:15.000000 django_post_deploy-2.4.2/django_post_deploy.egg-info/requires.txt
+-rw-r--r--   0 erlend     (501) staff       (20)       12 2024-05-23 12:40:15.000000 django_post_deploy-2.4.2/django_post_deploy.egg-info/top_level.txt
+drwxr-xr-x   0 erlend     (501) staff       (20)        0 2024-05-23 12:40:15.922445 django_post_deploy-2.4.2/post_deploy/
+-rw-r--r--   0 erlend     (501) staff       (20)    20137 2024-05-22 12:55:59.000000 django_post_deploy-2.4.2/post_deploy/LICENSE.txt
+-rw-r--r--   0 erlend     (501) staff       (20)      121 2024-05-22 14:17:09.000000 django_post_deploy-2.4.2/post_deploy/README.md
+-rw-r--r--   0 erlend     (501) staff       (20)       82 2024-05-23 12:37:48.000000 django_post_deploy-2.4.2/post_deploy/__init__.py
+-rw-r--r--   0 erlend     (501) staff       (20)       56 2024-05-22 12:55:59.000000 django_post_deploy-2.4.2/post_deploy/errors.py
+-rw-r--r--   0 erlend     (501) staff       (20)     2120 2024-05-22 12:55:59.000000 django_post_deploy-2.4.2/post_deploy/local_utils.py
+drwxr-xr-x   0 erlend     (501) staff       (20)        0 2024-05-23 12:40:15.919721 django_post_deploy-2.4.2/post_deploy/management/
+drwxr-xr-x   0 erlend     (501) staff       (20)        0 2024-05-23 12:40:15.922533 django_post_deploy-2.4.2/post_deploy/management/commands/
+-rw-r--r--   0 erlend     (501) staff       (20)     6666 2024-05-22 13:04:35.000000 django_post_deploy-2.4.2/post_deploy/management/commands/deploy.py
+drwxr-xr-x   0 erlend     (501) staff       (20)        0 2024-05-23 12:40:15.923164 django_post_deploy-2.4.2/post_deploy/migrations/
+-rw-r--r--   0 erlend     (501) staff       (20)     1123 2024-05-22 13:04:35.000000 django_post_deploy-2.4.2/post_deploy/migrations/0001_initial.py
+-rw-r--r--   0 erlend     (501) staff       (20)     1871 2024-05-22 13:04:35.000000 django_post_deploy-2.4.2/post_deploy/migrations/0002_postdeploylog.py
+-rw-r--r--   0 erlend     (501) staff       (20)        0 2024-05-22 12:55:59.000000 django_post_deploy-2.4.2/post_deploy/migrations/__init__.py
+-rw-r--r--   0 erlend     (501) staff       (20)     4533 2024-05-22 12:55:59.000000 django_post_deploy-2.4.2/post_deploy/models.py
+drwxr-xr-x   0 erlend     (501) staff       (20)        0 2024-05-23 12:40:15.923231 django_post_deploy-2.4.2/post_deploy/plugins/
+-rw-r--r--   0 erlend     (501) staff       (20)        0 2024-05-22 12:55:59.000000 django_post_deploy-2.4.2/post_deploy/plugins/__init__.py
+drwxr-xr-x   0 erlend     (501) staff       (20)        0 2024-05-23 12:40:15.923514 django_post_deploy-2.4.2/post_deploy/plugins/context/
+-rw-r--r--   0 erlend     (501) staff       (20)      280 2024-05-22 12:55:59.000000 django_post_deploy-2.4.2/post_deploy/plugins/context/__init__.py
+-rw-r--r--   0 erlend     (501) staff       (20)      439 2024-05-22 13:04:35.000000 django_post_deploy-2.4.2/post_deploy/plugins/context/tenant.py
+drwxr-xr-x   0 erlend     (501) staff       (20)        0 2024-05-23 12:40:15.923790 django_post_deploy-2.4.2/post_deploy/plugins/scheduler/
+-rw-r--r--   0 erlend     (501) staff       (20)      291 2024-05-22 12:55:59.000000 django_post_deploy-2.4.2/post_deploy/plugins/scheduler/__init__.py
+-rw-r--r--   0 erlend     (501) staff       (20)     1311 2024-05-22 13:04:35.000000 django_post_deploy-2.4.2/post_deploy/plugins/scheduler/celery.py
+-rw-r--r--   0 erlend     (501) staff       (20)      369 2024-05-22 12:55:59.000000 django_post_deploy-2.4.2/post_deploy/tasks.py
+drwxr-xr-x   0 erlend     (501) staff       (20)        0 2024-05-23 12:40:15.924328 django_post_deploy-2.4.2/post_deploy/tests/
+-rw-r--r--   0 erlend     (501) staff       (20)        0 2024-05-22 12:55:59.000000 django_post_deploy-2.4.2/post_deploy/tests/__init__.py
+-rw-r--r--   0 erlend     (501) staff       (20)     2472 2024-05-22 12:55:59.000000 django_post_deploy-2.4.2/post_deploy/tests/test_decorator.py
+-rw-r--r--   0 erlend     (501) staff       (20)     5323 2024-05-22 12:55:59.000000 django_post_deploy-2.4.2/post_deploy/tests/test_log_queryset.py
+-rw-r--r--   0 erlend     (501) staff       (20)     7172 2024-05-22 13:04:35.000000 django_post_deploy-2.4.2/post_deploy/tests/test_management_command.py
+-rw-r--r--   0 erlend     (501) staff       (20)     2197 2024-05-23 12:37:15.000000 django_post_deploy-2.4.2/post_deploy/utils.py
+-rw-r--r--   0 erlend     (501) staff       (20)       76 2024-05-23 12:40:15.924996 django_post_deploy-2.4.2/setup.cfg
+-rw-r--r--   0 erlend     (501) staff       (20)     1045 2024-05-22 14:15:07.000000 django_post_deploy-2.4.2/setup.py
```

### Comparing `django_post_deploy-2.4.1/PKG-INFO` & `django_post_deploy-2.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: django_post_deploy
-Version: 2.4.1
+Version: 2.4.2
 Summary: A generic way to have post-deploy actions done.
 Home-page: https://github.com/erlendgit/django_post_deploy
-Download-URL: https://github.com/erlendgit/django_post_deploy/archive/refs/tags/v2.4.1.tar.gz
+Download-URL: https://github.com/erlendgit/django_post_deploy/archive/refs/tags/v2.4.2.tar.gz
 Author: Erlend ter Maat
 Author-email: erwitema@gmail.com
 License: cc-by-4.0
 Keywords: Django,Deployment,Management,CLI
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `django_post_deploy-2.4.1/README.md` & `django_post_deploy-2.4.2/README.md`

 * *Files identical despite different names*

### Comparing `django_post_deploy-2.4.1/django_post_deploy.egg-info/PKG-INFO` & `django_post_deploy-2.4.2/django_post_deploy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: django-post-deploy
-Version: 2.4.1
+Version: 2.4.2
 Summary: A generic way to have post-deploy actions done.
 Home-page: https://github.com/erlendgit/django_post_deploy
-Download-URL: https://github.com/erlendgit/django_post_deploy/archive/refs/tags/v2.4.1.tar.gz
+Download-URL: https://github.com/erlendgit/django_post_deploy/archive/refs/tags/v2.4.2.tar.gz
 Author: Erlend ter Maat
 Author-email: erwitema@gmail.com
 License: cc-by-4.0
 Keywords: Django,Deployment,Management,CLI
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `django_post_deploy-2.4.1/django_post_deploy.egg-info/SOURCES.txt` & `django_post_deploy-2.4.2/django_post_deploy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_post_deploy-2.4.1/post_deploy/LICENSE.txt` & `django_post_deploy-2.4.2/post_deploy/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django_post_deploy-2.4.1/post_deploy/local_utils.py` & `django_post_deploy-2.4.2/post_deploy/local_utils.py`

 * *Files identical despite different names*

### Comparing `django_post_deploy-2.4.1/post_deploy/management/commands/deploy.py` & `django_post_deploy-2.4.2/post_deploy/management/commands/deploy.py`

 * *Files identical despite different names*

### Comparing `django_post_deploy-2.4.1/post_deploy/migrations/0001_initial.py` & `django_post_deploy-2.4.2/post_deploy/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_post_deploy-2.4.1/post_deploy/migrations/0002_postdeploylog.py` & `django_post_deploy-2.4.2/post_deploy/migrations/0002_postdeploylog.py`

 * *Files identical despite different names*

### Comparing `django_post_deploy-2.4.1/post_deploy/models.py` & `django_post_deploy-2.4.2/post_deploy/models.py`

 * *Files identical despite different names*

### Comparing `django_post_deploy-2.4.1/post_deploy/plugins/scheduler/celery.py` & `django_post_deploy-2.4.2/post_deploy/plugins/scheduler/celery.py`

 * *Files identical despite different names*

### Comparing `django_post_deploy-2.4.1/post_deploy/tests/test_decorator.py` & `django_post_deploy-2.4.2/post_deploy/tests/test_decorator.py`

 * *Files identical despite different names*

### Comparing `django_post_deploy-2.4.1/post_deploy/tests/test_log_queryset.py` & `django_post_deploy-2.4.2/post_deploy/tests/test_log_queryset.py`

 * *Files identical despite different names*

### Comparing `django_post_deploy-2.4.1/post_deploy/tests/test_management_command.py` & `django_post_deploy-2.4.2/post_deploy/tests/test_management_command.py`

 * *Files identical despite different names*

### Comparing `django_post_deploy-2.4.1/post_deploy/utils.py` & `django_post_deploy-2.4.2/post_deploy/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -52,12 +52,14 @@
     actions = initialize_actions()
     for import_name in actions.keys():
         PostDeployLog.objects.skip_action(import_name, reason)
 
 
 def run_task(import_name):
     from django.utils.translation import gettext as _
+    from post_deploy.local_utils import get_context_manager
     assert not PostDeployLog.objects.is_running(import_name), _("Task is already running")
 
+    context_manager = get_context_manager(None)
     action_log = PostDeployLog.objects.register_action(import_name)
-    task_id = get_scheduler_manager().schedule([action_log], self.context_manager.default_parameters())
+    task_id = get_scheduler_manager().schedule([action_log], context_manager.default_parameters())
     PostDeployLog.objects.filter(import_name=import_name).update(task_id=task_id)
```

### Comparing `django_post_deploy-2.4.1/setup.py` & `django_post_deploy-2.4.2/setup.py`

 * *Files identical despite different names*

