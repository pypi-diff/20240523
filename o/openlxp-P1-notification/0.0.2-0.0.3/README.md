# Comparing `tmp/openlxp-P1-notification-0.0.2.tar.gz` & `tmp/openlxp-P1-notification-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openlxp-P1-notification-0.0.2.tar", last modified: Tue May 21 20:22:48 2024, max compression
+gzip compressed data, was "openlxp-P1-notification-0.0.3.tar", last modified: Thu May 23 17:06:59 2024, max compression
```

## Comparing `openlxp-P1-notification-0.0.2.tar` & `openlxp-P1-notification-0.0.3.tar`

### file list

```diff
@@ -1,42 +1,43 @@
-drwxr-xr-x   0 kjijo      (502) staff       (20)        0 2024-05-21 20:22:48.240159 openlxp-P1-notification-0.0.2/
--rw-r--r--   0 kjijo      (502) staff       (20)      894 2024-05-21 20:22:48.240301 openlxp-P1-notification-0.0.2/PKG-INFO
--rw-r--r--   0 kjijo      (502) staff       (20)       25 2024-05-02 18:02:15.000000 openlxp-P1-notification-0.0.2/README.md
-drwxr-xr-x   0 kjijo      (502) staff       (20)        0 2024-05-21 20:22:48.205514 openlxp-P1-notification-0.0.2/openlxp_P1_notification/
--rw-r--r--   0 kjijo      (502) staff       (20)        0 2024-05-02 17:44:51.000000 openlxp-P1-notification-0.0.2/openlxp_P1_notification/__init__.py
--rw-r--r--   0 kjijo      (502) staff       (20)      674 2024-05-16 19:01:12.000000 openlxp-P1-notification-0.0.2/openlxp_P1_notification/admin.py
--rw-r--r--   0 kjijo      (502) staff       (20)      159 2024-05-07 17:20:28.000000 openlxp-P1-notification-0.0.2/openlxp_P1_notification/apps.py
-drwxr-xr-x   0 kjijo      (502) staff       (20)        0 2024-05-21 20:22:48.213944 openlxp-P1-notification-0.0.2/openlxp_P1_notification/management/
--rw-r--r--   0 kjijo      (502) staff       (20)        0 2024-05-02 17:44:51.000000 openlxp-P1-notification-0.0.2/openlxp_P1_notification/management/__init__.py
-drwxr-xr-x   0 kjijo      (502) staff       (20)        0 2024-05-21 20:22:48.217041 openlxp-P1-notification-0.0.2/openlxp_P1_notification/management/commands/
--rw-r--r--   0 kjijo      (502) staff       (20)        0 2024-05-02 17:44:51.000000 openlxp-P1-notification-0.0.2/openlxp_P1_notification/management/commands/__init__.py
--rw-r--r--   0 kjijo      (502) staff       (20)     4615 2024-05-17 18:18:42.000000 openlxp-P1-notification-0.0.2/openlxp_P1_notification/management/commands/conformance_alerts.py
-drwxr-xr-x   0 kjijo      (502) staff       (20)        0 2024-05-21 20:22:48.232564 openlxp-P1-notification-0.0.2/openlxp_P1_notification/management/utils/
--rw-r--r--   0 kjijo      (502) staff       (20)        0 2024-05-02 17:44:51.000000 openlxp-P1-notification-0.0.2/openlxp_P1_notification/management/utils/__init__.py
--rw-r--r--   0 kjijo      (502) staff       (20)     1830 2024-05-14 17:26:32.000000 openlxp-P1-notification-0.0.2/openlxp_P1_notification/management/utils/p1ps_configuration.py
--rw-r--r--   0 kjijo      (502) staff       (20)     3889 2024-05-16 18:49:31.000000 openlxp-P1-notification-0.0.2/openlxp_P1_notification/management/utils/p1ps_requests.py
--rw-r--r--   0 kjijo      (502) staff       (20)      665 2024-05-16 18:49:08.000000 openlxp-P1-notification-0.0.2/openlxp_P1_notification/middleware.py
-drwxr-xr-x   0 kjijo      (502) staff       (20)        0 2024-05-21 20:22:48.236612 openlxp-P1-notification-0.0.2/openlxp_P1_notification/migrations/
--rw-r--r--   0 kjijo      (502) staff       (20)     3691 2024-05-06 16:50:59.000000 openlxp-P1-notification-0.0.2/openlxp_P1_notification/migrations/0001_initial.py
--rw-r--r--   0 kjijo      (502) staff       (20)      379 2024-05-06 16:51:41.000000 openlxp-P1-notification-0.0.2/openlxp_P1_notification/migrations/0002_rename_template_body_template_message.py
--rw-r--r--   0 kjijo      (502) staff       (20)      656 2024-05-15 18:27:02.000000 openlxp-P1-notification-0.0.2/openlxp_P1_notification/migrations/0003_auto_20240515_1827.py
--rw-r--r--   0 kjijo      (502) staff       (20)        0 2024-05-02 17:44:51.000000 openlxp-P1-notification-0.0.2/openlxp_P1_notification/migrations/__init__.py
--rw-r--r--   0 kjijo      (502) staff       (20)     2867 2024-05-15 17:59:01.000000 openlxp-P1-notification-0.0.2/openlxp_P1_notification/models.py
--rw-r--r--   0 kjijo      (502) staff       (20)     1545 2024-05-08 15:53:30.000000 openlxp-P1-notification-0.0.2/openlxp_P1_notification/serializer.py
-drwxr-xr-x   0 kjijo      (502) staff       (20)        0 2024-05-21 20:22:48.237200 openlxp-P1-notification-0.0.2/openlxp_P1_notification/tests/
--rw-r--r--   0 kjijo      (502) staff       (20)        0 2024-05-02 17:44:51.000000 openlxp-P1-notification-0.0.2/openlxp_P1_notification/tests/__init__.py
--rw-r--r--   0 kjijo      (502) staff       (20)      957 2024-05-07 17:24:58.000000 openlxp-P1-notification-0.0.2/openlxp_P1_notification/urls.py
--rw-r--r--   0 kjijo      (502) staff       (20)      596 2024-05-06 18:33:54.000000 openlxp-P1-notification-0.0.2/openlxp_P1_notification/views.py
-drwxr-xr-x   0 kjijo      (502) staff       (20)        0 2024-05-21 20:22:48.212595 openlxp-P1-notification-0.0.2/openlxp_P1_notification.egg-info/
--rw-r--r--   0 kjijo      (502) staff       (20)      894 2024-05-21 20:22:48.000000 openlxp-P1-notification-0.0.2/openlxp_P1_notification.egg-info/PKG-INFO
--rw-r--r--   0 kjijo      (502) staff       (20)     1372 2024-05-21 20:22:48.000000 openlxp-P1-notification-0.0.2/openlxp_P1_notification.egg-info/SOURCES.txt
--rw-r--r--   0 kjijo      (502) staff       (20)        1 2024-05-21 20:22:48.000000 openlxp-P1-notification-0.0.2/openlxp_P1_notification.egg-info/dependency_links.txt
--rw-r--r--   0 kjijo      (502) staff       (20)       14 2024-05-21 20:22:48.000000 openlxp-P1-notification-0.0.2/openlxp_P1_notification.egg-info/requires.txt
--rw-r--r--   0 kjijo      (502) staff       (20)       67 2024-05-21 20:22:48.000000 openlxp-P1-notification-0.0.2/openlxp_P1_notification.egg-info/top_level.txt
-drwxr-xr-x   0 kjijo      (502) staff       (20)        0 2024-05-21 20:22:48.239884 openlxp-P1-notification-0.0.2/openlxp_P1_notification_project/
--rw-r--r--   0 kjijo      (502) staff       (20)        0 2024-05-02 17:44:51.000000 openlxp-P1-notification-0.0.2/openlxp_P1_notification_project/__init__.py
--rw-r--r--   0 kjijo      (502) staff       (20)      461 2024-05-02 18:07:28.000000 openlxp-P1-notification-0.0.2/openlxp_P1_notification_project/asgi.py
--rw-r--r--   0 kjijo      (502) staff       (20)     4845 2024-05-16 18:49:47.000000 openlxp-P1-notification-0.0.2/openlxp_P1_notification_project/settings.py
--rw-r--r--   0 kjijo      (502) staff       (20)      981 2024-05-06 18:26:56.000000 openlxp-P1-notification-0.0.2/openlxp_P1_notification_project/urls.py
--rw-r--r--   0 kjijo      (502) staff       (20)      577 2024-05-16 18:49:41.000000 openlxp-P1-notification-0.0.2/openlxp_P1_notification_project/wsgi.py
--rw-r--r--   0 kjijo      (502) staff       (20)      970 2024-05-21 20:22:48.241265 openlxp-P1-notification-0.0.2/setup.cfg
--rw-r--r--   0 kjijo      (502) staff       (20)       95 2024-05-02 17:44:51.000000 openlxp-P1-notification-0.0.2/setup.py
+drwxr-xr-x   0 kjijo      (502) staff       (20)        0 2024-05-23 17:06:59.507559 openlxp-P1-notification-0.0.3/
+-rw-r--r--   0 kjijo      (502) staff       (20)      894 2024-05-23 17:06:59.507725 openlxp-P1-notification-0.0.3/PKG-INFO
+-rw-r--r--   0 kjijo      (502) staff       (20)       25 2024-05-02 18:02:15.000000 openlxp-P1-notification-0.0.3/README.md
+drwxr-xr-x   0 kjijo      (502) staff       (20)        0 2024-05-23 17:06:59.491220 openlxp-P1-notification-0.0.3/openlxp_P1_notification/
+-rw-r--r--   0 kjijo      (502) staff       (20)        0 2024-05-02 17:44:51.000000 openlxp-P1-notification-0.0.3/openlxp_P1_notification/__init__.py
+-rw-r--r--   0 kjijo      (502) staff       (20)      674 2024-05-16 19:01:12.000000 openlxp-P1-notification-0.0.3/openlxp_P1_notification/admin.py
+-rw-r--r--   0 kjijo      (502) staff       (20)      159 2024-05-07 17:20:28.000000 openlxp-P1-notification-0.0.3/openlxp_P1_notification/apps.py
+drwxr-xr-x   0 kjijo      (502) staff       (20)        0 2024-05-23 17:06:59.494711 openlxp-P1-notification-0.0.3/openlxp_P1_notification/management/
+-rw-r--r--   0 kjijo      (502) staff       (20)        0 2024-05-02 17:44:51.000000 openlxp-P1-notification-0.0.3/openlxp_P1_notification/management/__init__.py
+drwxr-xr-x   0 kjijo      (502) staff       (20)        0 2024-05-23 17:06:59.496379 openlxp-P1-notification-0.0.3/openlxp_P1_notification/management/commands/
+-rw-r--r--   0 kjijo      (502) staff       (20)        0 2024-05-02 17:44:51.000000 openlxp-P1-notification-0.0.3/openlxp_P1_notification/management/commands/__init__.py
+-rw-r--r--   0 kjijo      (502) staff       (20)     2584 2024-05-22 03:37:18.000000 openlxp-P1-notification-0.0.3/openlxp_P1_notification/management/commands/trigger_status_update.py
+-rw-r--r--   0 kjijo      (502) staff       (20)     3252 2024-05-22 03:38:08.000000 openlxp-P1-notification-0.0.3/openlxp_P1_notification/management/commands/trigger_subscribed_list_update.py
+drwxr-xr-x   0 kjijo      (502) staff       (20)        0 2024-05-23 17:06:59.501584 openlxp-P1-notification-0.0.3/openlxp_P1_notification/management/utils/
+-rw-r--r--   0 kjijo      (502) staff       (20)        0 2024-05-02 17:44:51.000000 openlxp-P1-notification-0.0.3/openlxp_P1_notification/management/utils/__init__.py
+-rw-r--r--   0 kjijo      (502) staff       (20)     1830 2024-05-14 17:26:32.000000 openlxp-P1-notification-0.0.3/openlxp_P1_notification/management/utils/p1ps_configuration.py
+-rw-r--r--   0 kjijo      (502) staff       (20)     3889 2024-05-16 18:49:31.000000 openlxp-P1-notification-0.0.3/openlxp_P1_notification/management/utils/p1ps_requests.py
+-rw-r--r--   0 kjijo      (502) staff       (20)      665 2024-05-16 18:49:08.000000 openlxp-P1-notification-0.0.3/openlxp_P1_notification/middleware.py
+drwxr-xr-x   0 kjijo      (502) staff       (20)        0 2024-05-23 17:06:59.504409 openlxp-P1-notification-0.0.3/openlxp_P1_notification/migrations/
+-rw-r--r--   0 kjijo      (502) staff       (20)     3691 2024-05-06 16:50:59.000000 openlxp-P1-notification-0.0.3/openlxp_P1_notification/migrations/0001_initial.py
+-rw-r--r--   0 kjijo      (502) staff       (20)      379 2024-05-06 16:51:41.000000 openlxp-P1-notification-0.0.3/openlxp_P1_notification/migrations/0002_rename_template_body_template_message.py
+-rw-r--r--   0 kjijo      (502) staff       (20)      656 2024-05-15 18:27:02.000000 openlxp-P1-notification-0.0.3/openlxp_P1_notification/migrations/0003_auto_20240515_1827.py
+-rw-r--r--   0 kjijo      (502) staff       (20)        0 2024-05-02 17:44:51.000000 openlxp-P1-notification-0.0.3/openlxp_P1_notification/migrations/__init__.py
+-rw-r--r--   0 kjijo      (502) staff       (20)     2867 2024-05-15 17:59:01.000000 openlxp-P1-notification-0.0.3/openlxp_P1_notification/models.py
+-rw-r--r--   0 kjijo      (502) staff       (20)     1545 2024-05-08 15:53:30.000000 openlxp-P1-notification-0.0.3/openlxp_P1_notification/serializer.py
+drwxr-xr-x   0 kjijo      (502) staff       (20)        0 2024-05-23 17:06:59.504670 openlxp-P1-notification-0.0.3/openlxp_P1_notification/tests/
+-rw-r--r--   0 kjijo      (502) staff       (20)        0 2024-05-02 17:44:51.000000 openlxp-P1-notification-0.0.3/openlxp_P1_notification/tests/__init__.py
+-rw-r--r--   0 kjijo      (502) staff       (20)      957 2024-05-07 17:24:58.000000 openlxp-P1-notification-0.0.3/openlxp_P1_notification/urls.py
+-rw-r--r--   0 kjijo      (502) staff       (20)      596 2024-05-06 18:33:54.000000 openlxp-P1-notification-0.0.3/openlxp_P1_notification/views.py
+drwxr-xr-x   0 kjijo      (502) staff       (20)        0 2024-05-23 17:06:59.493851 openlxp-P1-notification-0.0.3/openlxp_P1_notification.egg-info/
+-rw-r--r--   0 kjijo      (502) staff       (20)      894 2024-05-23 17:06:59.000000 openlxp-P1-notification-0.0.3/openlxp_P1_notification.egg-info/PKG-INFO
+-rw-r--r--   0 kjijo      (502) staff       (20)     1453 2024-05-23 17:06:59.000000 openlxp-P1-notification-0.0.3/openlxp_P1_notification.egg-info/SOURCES.txt
+-rw-r--r--   0 kjijo      (502) staff       (20)        1 2024-05-23 17:06:59.000000 openlxp-P1-notification-0.0.3/openlxp_P1_notification.egg-info/dependency_links.txt
+-rw-r--r--   0 kjijo      (502) staff       (20)       14 2024-05-23 17:06:59.000000 openlxp-P1-notification-0.0.3/openlxp_P1_notification.egg-info/requires.txt
+-rw-r--r--   0 kjijo      (502) staff       (20)       56 2024-05-23 17:06:59.000000 openlxp-P1-notification-0.0.3/openlxp_P1_notification.egg-info/top_level.txt
+drwxr-xr-x   0 kjijo      (502) staff       (20)        0 2024-05-23 17:06:59.507226 openlxp-P1-notification-0.0.3/openlxp_P1_notification_project/
+-rw-r--r--   0 kjijo      (502) staff       (20)        0 2024-05-02 17:44:51.000000 openlxp-P1-notification-0.0.3/openlxp_P1_notification_project/__init__.py
+-rw-r--r--   0 kjijo      (502) staff       (20)      461 2024-05-02 18:07:28.000000 openlxp-P1-notification-0.0.3/openlxp_P1_notification_project/asgi.py
+-rw-r--r--   0 kjijo      (502) staff       (20)     4845 2024-05-16 18:49:47.000000 openlxp-P1-notification-0.0.3/openlxp_P1_notification_project/settings.py
+-rw-r--r--   0 kjijo      (502) staff       (20)      981 2024-05-06 18:26:56.000000 openlxp-P1-notification-0.0.3/openlxp_P1_notification_project/urls.py
+-rw-r--r--   0 kjijo      (502) staff       (20)      577 2024-05-16 18:49:41.000000 openlxp-P1-notification-0.0.3/openlxp_P1_notification_project/wsgi.py
+-rw-r--r--   0 kjijo      (502) staff       (20)      970 2024-05-23 17:06:59.508185 openlxp-P1-notification-0.0.3/setup.cfg
+-rw-r--r--   0 kjijo      (502) staff       (20)       95 2024-05-02 17:44:51.000000 openlxp-P1-notification-0.0.3/setup.py
```

### Comparing `openlxp-P1-notification-0.0.2/PKG-INFO` & `openlxp-P1-notification-0.0.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openlxp-P1-notification
-Version: 0.0.2
+Version: 0.0.3
 Summary: Sample installable OpenLXP Notifications
 Home-page: https://github.com/OpenLXP/openlxp-P1-notification/
 Author: OpenLXP
 Author-email: openlxphost@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `openlxp-P1-notification-0.0.2/openlxp_P1_notification/admin.py` & `openlxp-P1-notification-0.0.3/openlxp_P1_notification/admin.py`

 * *Files identical despite different names*

### Comparing `openlxp-P1-notification-0.0.2/openlxp_P1_notification/management/commands/conformance_alerts.py` & `openlxp-P1-notification-0.0.3/openlxp_P1_notification/management/commands/trigger_subscribed_list_update.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,57 +5,26 @@
 
 
 from django.core.management.base import (BaseCommand, CommandParser,
                                          CommandError)
 
 from openlxp_P1_notification.management.utils.p1ps_requests import (
     overall_health, send_email)
-from openlxp_P1_notification.models import (email, recipient)
+from openlxp_P1_notification.models import (email)
 
 from openlxp_P1_notification.serializer import EmailSerializer
 
 logger = logging.getLogger('dict_config_logger')
 
 
 def trigger_health_check():
     """Command to trigger email health check"""
     overall_health()
 
 
-def trigger_status_update(email_type):
-    """Command to trigger email notification"""
-
-    body_data = EmailSerializer(email_type).data
-
-    recipient_list = body_data['recipients']
-    now = dt.now()
-    datetimenow = now.strftime("%d/%m/%Y %H:%M:%S")
-
-    template_data = EmailSerializer(email_type).data
-
-    for recipient_email in recipient_list:
-        body_data = copy.deepcopy(template_data)
-
-        recipient_obj = recipient.objects.get(
-            email_address=recipient_email)
-
-        body_data['recipients'] = [recipient_email]
-
-        if 'name' in email_type.template_type.template_inputs:
-            body_data['template_inputs']['name'] = (recipient_obj.first_name +
-                                                    " " +
-                                                    recipient_obj.last_name)
-        if 'datetime' in email_type.template_type.template_inputs:
-            body_data['template_inputs']['datetime'] = datetimenow
-
-        body_data = json.dumps(body_data)
-
-        send_email(body_data, str(email_type.template_type))
-
-
 def trigger_subscribed_list_update(email_type, recipient_list,
                                    list_name, list_url):
     """Command to trigger email for list updates"""
 
     now = dt.now()
     datetimenow = now.strftime("%d/%m/%Y %H:%M:%S")
 
@@ -99,21 +68,13 @@
         # for email_reference in options['email_references']:
         try:
             email_type = email.objects.get(
                 reference=options['email_references'])
         except email.DoesNotExist:
             raise CommandError('Email Reference "%s" does not exist' %
                                options['email_references'])
-        # now = datetime.now()
-        # dt = now.strftime("%d/%m/%Y %H:%M:%S")
-        # template_inputs = {
-        #     "datetime": dt,
-        #     "name": "FNAME LNAME"
-        # }
-        # trigger_status_update(email_type)
 
-        recipient_list = [('kjijo@deloitte.com', 'Karen', 'jijo'),
-                          ('karenjijo@gmail.com', 'KJ', 'rocks')]
+        recipient_list = [('kjijo@deloitte.com', 'Karen', 'jijo')]
         trigger_subscribed_list_update(email_type, recipient_list,
-                                       "Public",
-                                       "https://dev-xds.deloitteopenlxp.com/lists/1")
-        # get_team_templates()
+                                       "List1",
+                                       "https://dev-xds.deloitteopenlxp.com/"
+                                       "lists/1")
```

### Comparing `openlxp-P1-notification-0.0.2/openlxp_P1_notification/management/utils/p1ps_configuration.py` & `openlxp-P1-notification-0.0.3/openlxp_P1_notification/management/utils/p1ps_configuration.py`

 * *Files identical despite different names*

### Comparing `openlxp-P1-notification-0.0.2/openlxp_P1_notification/management/utils/p1ps_requests.py` & `openlxp-P1-notification-0.0.3/openlxp_P1_notification/management/utils/p1ps_requests.py`

 * *Files identical despite different names*

### Comparing `openlxp-P1-notification-0.0.2/openlxp_P1_notification/middleware.py` & `openlxp-P1-notification-0.0.3/openlxp_P1_notification/middleware.py`

 * *Files identical despite different names*

### Comparing `openlxp-P1-notification-0.0.2/openlxp_P1_notification/migrations/0001_initial.py` & `openlxp-P1-notification-0.0.3/openlxp_P1_notification/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `openlxp-P1-notification-0.0.2/openlxp_P1_notification/migrations/0003_auto_20240515_1827.py` & `openlxp-P1-notification-0.0.3/openlxp_P1_notification/migrations/0003_auto_20240515_1827.py`

 * *Files identical despite different names*

### Comparing `openlxp-P1-notification-0.0.2/openlxp_P1_notification/models.py` & `openlxp-P1-notification-0.0.3/openlxp_P1_notification/models.py`

 * *Files identical despite different names*

### Comparing `openlxp-P1-notification-0.0.2/openlxp_P1_notification/serializer.py` & `openlxp-P1-notification-0.0.3/openlxp_P1_notification/serializer.py`

 * *Files identical despite different names*

### Comparing `openlxp-P1-notification-0.0.2/openlxp_P1_notification/urls.py` & `openlxp-P1-notification-0.0.3/openlxp_P1_notification/urls.py`

 * *Files identical despite different names*

### Comparing `openlxp-P1-notification-0.0.2/openlxp_P1_notification/views.py` & `openlxp-P1-notification-0.0.3/openlxp_P1_notification/views.py`

 * *Files identical despite different names*

### Comparing `openlxp-P1-notification-0.0.2/openlxp_P1_notification.egg-info/PKG-INFO` & `openlxp-P1-notification-0.0.3/openlxp_P1_notification.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openlxp-P1-notification
-Version: 0.0.2
+Version: 0.0.3
 Summary: Sample installable OpenLXP Notifications
 Home-page: https://github.com/OpenLXP/openlxp-P1-notification/
 Author: OpenLXP
 Author-email: openlxphost@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

### Comparing `openlxp-P1-notification-0.0.2/openlxp_P1_notification.egg-info/SOURCES.txt` & `openlxp-P1-notification-0.0.3/openlxp_P1_notification.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 openlxp_P1_notification.egg-info/PKG-INFO
 openlxp_P1_notification.egg-info/SOURCES.txt
 openlxp_P1_notification.egg-info/dependency_links.txt
 openlxp_P1_notification.egg-info/requires.txt
 openlxp_P1_notification.egg-info/top_level.txt
 openlxp_P1_notification/management/__init__.py
 openlxp_P1_notification/management/commands/__init__.py
-openlxp_P1_notification/management/commands/conformance_alerts.py
+openlxp_P1_notification/management/commands/trigger_status_update.py
+openlxp_P1_notification/management/commands/trigger_subscribed_list_update.py
 openlxp_P1_notification/management/utils/__init__.py
 openlxp_P1_notification/management/utils/p1ps_configuration.py
 openlxp_P1_notification/management/utils/p1ps_requests.py
 openlxp_P1_notification/migrations/0001_initial.py
 openlxp_P1_notification/migrations/0002_rename_template_body_template_message.py
 openlxp_P1_notification/migrations/0003_auto_20240515_1827.py
 openlxp_P1_notification/migrations/__init__.py
```

### Comparing `openlxp-P1-notification-0.0.2/openlxp_P1_notification_project/settings.py` & `openlxp-P1-notification-0.0.3/openlxp_P1_notification_project/settings.py`

 * *Files identical despite different names*

### Comparing `openlxp-P1-notification-0.0.2/openlxp_P1_notification_project/urls.py` & `openlxp-P1-notification-0.0.3/openlxp_P1_notification_project/urls.py`

 * *Files identical despite different names*

### Comparing `openlxp-P1-notification-0.0.2/openlxp_P1_notification_project/wsgi.py` & `openlxp-P1-notification-0.0.3/openlxp_P1_notification_project/wsgi.py`

 * *Files identical despite different names*

### Comparing `openlxp-P1-notification-0.0.2/setup.cfg` & `openlxp-P1-notification-0.0.3/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = openlxp-P1-notification
-version = 0.0.2
+version = 0.0.3
 description = Sample installable OpenLXP Notifications
 long_description = file:README.md
 url = https://github.com/OpenLXP/openlxp-P1-notification/
 author = OpenLXP
 author_email = openlxphost@gmail.com
 license = MIT
 classifiers =
```

