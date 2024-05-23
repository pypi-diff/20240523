# Comparing `tmp/django_twined-0.8.2.tar.gz` & `tmp/django_twined-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_twined-0.8.2.tar", max compression
+gzip compressed data, was "django_twined-0.8.3.tar", max compression
```

## Comparing `django_twined-0.8.2.tar` & `django_twined-0.8.3.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rw-r--r--   0        0        0     1088 2024-04-22 06:32:38.682023 django_twined-0.8.2/LICENSE
--rw-r--r--   0        0        0     1463 2024-04-22 06:32:38.682023 django_twined-0.8.2/README.md
--rw-r--r--   0        0        0       64 2024-04-22 06:32:38.682023 django_twined-0.8.2/django_twined/__init__.py
--rw-r--r--   0        0        0      229 2024-04-22 06:32:38.682023 django_twined-0.8.2/django_twined/admin/__init__.py
--rw-r--r--   0        0        0     9825 2024-04-22 06:32:38.682023 django_twined-0.8.2/django_twined/admin/admin.py
--rw-r--r--   0        0        0     1036 2024-04-22 06:32:38.682023 django_twined-0.8.2/django_twined/admin/fieldsets.py
--rw-r--r--   0        0        0      881 2024-04-22 06:32:38.682023 django_twined-0.8.2/django_twined/admin/mixins.py
--rw-r--r--   0        0        0      682 2024-04-22 06:32:38.682023 django_twined-0.8.2/django_twined/admin/proxy.py
--rw-r--r--   0        0        0      496 2024-04-22 06:32:38.682023 django_twined-0.8.2/django_twined/apps.py
--rw-r--r--   0        0        0      130 2024-04-22 06:32:38.682023 django_twined-0.8.2/django_twined/exceptions.py
--rw-r--r--   0        0        0     2358 2024-04-22 06:32:38.682023 django_twined-0.8.2/django_twined/fields.py
--rw-r--r--   0        0        0        0 2024-04-22 06:32:38.682023 django_twined-0.8.2/django_twined/management/__init__.py
--rw-r--r--   0        0        0        0 2024-04-22 06:32:38.682023 django_twined-0.8.2/django_twined/management/commands/__init__.py
--rw-r--r--   0        0        0     2300 2024-04-22 06:32:38.682023 django_twined-0.8.2/django_twined/management/commands/sync_data_stores.py
--rw-r--r--   0        0        0     2346 2024-04-22 06:32:38.682023 django_twined-0.8.2/django_twined/migrations/0001_initial.py
--rw-r--r--   0        0        0      595 2024-04-22 06:32:38.682023 django_twined-0.8.2/django_twined/migrations/0002_slug_unique_and_not_editable.py
--rw-r--r--   0        0        0      408 2024-04-22 06:32:38.682023 django_twined-0.8.2/django_twined/migrations/0003_rename_slug_to_name.py
--rw-r--r--   0        0        0      670 2024-04-22 06:32:38.682023 django_twined-0.8.2/django_twined/migrations/0004_add_timestamps.py
--rw-r--r--   0        0        0      731 2024-04-22 06:32:38.682023 django_twined-0.8.2/django_twined/migrations/0005_question_date_help_text.py
--rw-r--r--   0        0        0     4711 2024-04-22 06:32:38.682023 django_twined-0.8.2/django_twined/migrations/0006_service_revisions_and_events.py
--rw-r--r--   0        0        0     1476 2024-04-22 06:32:38.682023 django_twined-0.8.2/django_twined/migrations/0007_registered_to_revision.py
--rw-r--r--   0        0        0      669 2024-04-22 06:32:38.682023 django_twined-0.8.2/django_twined/migrations/0008_registered_relations_to_nullable.py
--rw-r--r--   0        0        0      683 2024-04-22 06:32:38.682023 django_twined-0.8.2/django_twined/migrations/0009_remove_registered_services.py
--rw-r--r--   0        0        0      681 2024-04-22 06:32:38.682023 django_twined-0.8.2/django_twined/migrations/0010_alter_servicerevision_project_name.py
--rw-r--r--   0        0        0      362 2024-04-22 06:32:38.682023 django_twined-0.8.2/django_twined/migrations/0011_remove_servicerevision_topic_id.py
--rw-r--r--   0        0        0      568 2024-04-22 06:32:38.686023 django_twined-0.8.2/django_twined/migrations/0012_servicerevision_is_default.py
--rw-r--r--   0        0        0      639 2024-04-22 06:32:38.686023 django_twined-0.8.2/django_twined/migrations/0013_alter_serviceusageevent_question.py
--rw-r--r--   0        0        0      746 2024-04-22 06:32:38.686023 django_twined-0.8.2/django_twined/migrations/0014_question_status.py
--rw-r--r--   0        0        0        0 2024-04-22 06:32:38.686023 django_twined-0.8.2/django_twined/migrations/__init__.py
--rw-r--r--   0        0        0      883 2024-04-22 06:32:38.686023 django_twined-0.8.2/django_twined/models/__init__.py
--rw-r--r--   0        0        0    11441 2024-04-22 06:32:38.686023 django_twined-0.8.2/django_twined/models/datastores.py
--rw-r--r--   0        0        0       85 2024-04-22 06:32:38.686023 django_twined-0.8.2/django_twined/models/querysets/__init__.py
--rw-r--r--   0        0        0     9795 2024-04-22 06:32:38.686023 django_twined-0.8.2/django_twined/models/querysets/datastore_queryset.py
--rw-r--r--   0        0        0     5752 2024-04-22 06:32:38.686023 django_twined-0.8.2/django_twined/models/questions.py
--rw-r--r--   0        0        0     8193 2024-04-22 06:32:38.686023 django_twined-0.8.2/django_twined/models/service_revisions.py
--rw-r--r--   0        0        0     6481 2024-04-22 06:32:38.686023 django_twined-0.8.2/django_twined/models/service_usage_events.py
--rw-r--r--   0        0        0      479 2024-04-22 06:32:38.686023 django_twined-0.8.2/django_twined/signals/__init__.py
--rw-r--r--   0        0        0     3086 2024-04-22 06:32:38.686023 django_twined-0.8.2/django_twined/signals/receivers.py
--rw-r--r--   0        0        0      262 2024-04-22 06:32:38.686023 django_twined-0.8.2/django_twined/signals/senders.py
--rw-r--r--   0        0        0        0 2024-04-22 06:32:38.686023 django_twined-0.8.2/django_twined/static/.gitignore
--rw-r--r--   0        0        0     1149 2024-04-22 06:32:38.686023 django_twined-0.8.2/django_twined/templates/admin/question_ask_row.html
--rw-r--r--   0        0        0        0 2024-04-22 06:32:38.686023 django_twined-0.8.2/django_twined/templates/django_twined/.gitignore
--rw-r--r--   0        0        0      343 2024-04-22 06:32:38.686023 django_twined-0.8.2/django_twined/templates/django_twined/question_changeform.html
--rw-r--r--   0        0        0        0 2024-04-22 06:32:38.686023 django_twined-0.8.2/django_twined/templatetags/__init__.py
--rw-r--r--   0        0        0      480 2024-04-22 06:32:38.686023 django_twined-0.8.2/django_twined/templatetags/question_ask_row.py
--rw-r--r--   0        0        0      241 2024-04-22 06:32:38.686023 django_twined-0.8.2/django_twined/urls.py
--rw-r--r--   0        0        0     2443 2024-04-22 06:32:38.686023 django_twined-0.8.2/django_twined/views.py
--rw-r--r--   0        0        0     1571 2024-04-22 06:32:38.686023 django_twined-0.8.2/pyproject.toml
--rw-r--r--   0        0        0     2570 1970-01-01 00:00:00.000000 django_twined-0.8.2/PKG-INFO
+-rw-r--r--   0        0        0     1088 2024-05-23 17:52:53.769919 django_twined-0.8.3/LICENSE
+-rw-r--r--   0        0        0     1463 2024-05-23 17:52:53.769919 django_twined-0.8.3/README.md
+-rw-r--r--   0        0        0       64 2024-05-23 17:52:53.769919 django_twined-0.8.3/django_twined/__init__.py
+-rw-r--r--   0        0        0      229 2024-05-23 17:52:53.769919 django_twined-0.8.3/django_twined/admin/__init__.py
+-rw-r--r--   0        0        0     9825 2024-05-23 17:52:53.769919 django_twined-0.8.3/django_twined/admin/admin.py
+-rw-r--r--   0        0        0     1036 2024-05-23 17:52:53.769919 django_twined-0.8.3/django_twined/admin/fieldsets.py
+-rw-r--r--   0        0        0      881 2024-05-23 17:52:53.769919 django_twined-0.8.3/django_twined/admin/mixins.py
+-rw-r--r--   0        0        0      682 2024-05-23 17:52:53.769919 django_twined-0.8.3/django_twined/admin/proxy.py
+-rw-r--r--   0        0        0      496 2024-05-23 17:52:53.769919 django_twined-0.8.3/django_twined/apps.py
+-rw-r--r--   0        0        0      130 2024-05-23 17:52:53.769919 django_twined-0.8.3/django_twined/exceptions.py
+-rw-r--r--   0        0        0     2358 2024-05-23 17:52:53.769919 django_twined-0.8.3/django_twined/fields.py
+-rw-r--r--   0        0        0        0 2024-05-23 17:52:53.769919 django_twined-0.8.3/django_twined/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-23 17:52:53.769919 django_twined-0.8.3/django_twined/management/commands/__init__.py
+-rw-r--r--   0        0        0     2300 2024-05-23 17:52:53.769919 django_twined-0.8.3/django_twined/management/commands/sync_data_stores.py
+-rw-r--r--   0        0        0     2346 2024-05-23 17:52:53.769919 django_twined-0.8.3/django_twined/migrations/0001_initial.py
+-rw-r--r--   0        0        0      595 2024-05-23 17:52:53.773919 django_twined-0.8.3/django_twined/migrations/0002_slug_unique_and_not_editable.py
+-rw-r--r--   0        0        0      408 2024-05-23 17:52:53.773919 django_twined-0.8.3/django_twined/migrations/0003_rename_slug_to_name.py
+-rw-r--r--   0        0        0      670 2024-05-23 17:52:53.773919 django_twined-0.8.3/django_twined/migrations/0004_add_timestamps.py
+-rw-r--r--   0        0        0      731 2024-05-23 17:52:53.773919 django_twined-0.8.3/django_twined/migrations/0005_question_date_help_text.py
+-rw-r--r--   0        0        0     4711 2024-05-23 17:52:53.773919 django_twined-0.8.3/django_twined/migrations/0006_service_revisions_and_events.py
+-rw-r--r--   0        0        0     1476 2024-05-23 17:52:53.773919 django_twined-0.8.3/django_twined/migrations/0007_registered_to_revision.py
+-rw-r--r--   0        0        0      669 2024-05-23 17:52:53.773919 django_twined-0.8.3/django_twined/migrations/0008_registered_relations_to_nullable.py
+-rw-r--r--   0        0        0      683 2024-05-23 17:52:53.773919 django_twined-0.8.3/django_twined/migrations/0009_remove_registered_services.py
+-rw-r--r--   0        0        0      681 2024-05-23 17:52:53.773919 django_twined-0.8.3/django_twined/migrations/0010_alter_servicerevision_project_name.py
+-rw-r--r--   0        0        0      362 2024-05-23 17:52:53.773919 django_twined-0.8.3/django_twined/migrations/0011_remove_servicerevision_topic_id.py
+-rw-r--r--   0        0        0      568 2024-05-23 17:52:53.773919 django_twined-0.8.3/django_twined/migrations/0012_servicerevision_is_default.py
+-rw-r--r--   0        0        0      639 2024-05-23 17:52:53.773919 django_twined-0.8.3/django_twined/migrations/0013_alter_serviceusageevent_question.py
+-rw-r--r--   0        0        0      746 2024-05-23 17:52:53.773919 django_twined-0.8.3/django_twined/migrations/0014_question_status.py
+-rw-r--r--   0        0        0        0 2024-05-23 17:52:53.773919 django_twined-0.8.3/django_twined/migrations/__init__.py
+-rw-r--r--   0        0        0      883 2024-05-23 17:52:53.773919 django_twined-0.8.3/django_twined/models/__init__.py
+-rw-r--r--   0        0        0    11441 2024-05-23 17:52:53.773919 django_twined-0.8.3/django_twined/models/datastores.py
+-rw-r--r--   0        0        0       85 2024-05-23 17:52:53.773919 django_twined-0.8.3/django_twined/models/querysets/__init__.py
+-rw-r--r--   0        0        0     9795 2024-05-23 17:52:53.773919 django_twined-0.8.3/django_twined/models/querysets/datastore_queryset.py
+-rw-r--r--   0        0        0     5752 2024-05-23 17:52:53.773919 django_twined-0.8.3/django_twined/models/questions.py
+-rw-r--r--   0        0        0     8193 2024-05-23 17:52:53.773919 django_twined-0.8.3/django_twined/models/service_revisions.py
+-rw-r--r--   0        0        0     6481 2024-05-23 17:52:53.773919 django_twined-0.8.3/django_twined/models/service_usage_events.py
+-rw-r--r--   0        0        0      479 2024-05-23 17:52:53.773919 django_twined-0.8.3/django_twined/signals/__init__.py
+-rw-r--r--   0        0        0     3086 2024-05-23 17:52:53.773919 django_twined-0.8.3/django_twined/signals/receivers.py
+-rw-r--r--   0        0        0      262 2024-05-23 17:52:53.773919 django_twined-0.8.3/django_twined/signals/senders.py
+-rw-r--r--   0        0        0        0 2024-05-23 17:52:53.773919 django_twined-0.8.3/django_twined/static/.gitignore
+-rw-r--r--   0        0        0     1149 2024-05-23 17:52:53.773919 django_twined-0.8.3/django_twined/templates/admin/question_ask_row.html
+-rw-r--r--   0        0        0        0 2024-05-23 17:52:53.773919 django_twined-0.8.3/django_twined/templates/django_twined/.gitignore
+-rw-r--r--   0        0        0      343 2024-05-23 17:52:53.773919 django_twined-0.8.3/django_twined/templates/django_twined/question_changeform.html
+-rw-r--r--   0        0        0        0 2024-05-23 17:52:53.773919 django_twined-0.8.3/django_twined/templatetags/__init__.py
+-rw-r--r--   0        0        0      480 2024-05-23 17:52:53.773919 django_twined-0.8.3/django_twined/templatetags/question_ask_row.py
+-rw-r--r--   0        0        0      241 2024-05-23 17:52:53.773919 django_twined-0.8.3/django_twined/urls.py
+-rw-r--r--   0        0        0     2443 2024-05-23 17:52:53.773919 django_twined-0.8.3/django_twined/views.py
+-rw-r--r--   0        0        0     1571 2024-05-23 17:52:53.773919 django_twined-0.8.3/pyproject.toml
+-rw-r--r--   0        0        0     2570 1970-01-01 00:00:00.000000 django_twined-0.8.3/PKG-INFO
```

### Comparing `django_twined-0.8.2/LICENSE` & `django_twined-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django_twined-0.8.2/README.md` & `django_twined-0.8.3/README.md`

 * *Files identical despite different names*

### Comparing `django_twined-0.8.2/django_twined/admin/admin.py` & `django_twined-0.8.3/django_twined/admin/admin.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.8.2/django_twined/admin/fieldsets.py` & `django_twined-0.8.3/django_twined/admin/fieldsets.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.8.2/django_twined/admin/mixins.py` & `django_twined-0.8.3/django_twined/admin/mixins.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.8.2/django_twined/admin/proxy.py` & `django_twined-0.8.3/django_twined/admin/proxy.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.8.2/django_twined/fields.py` & `django_twined-0.8.3/django_twined/fields.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.8.2/django_twined/management/commands/sync_data_stores.py` & `django_twined-0.8.3/django_twined/management/commands/sync_data_stores.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.8.2/django_twined/migrations/0001_initial.py` & `django_twined-0.8.3/django_twined/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.8.2/django_twined/migrations/0002_slug_unique_and_not_editable.py` & `django_twined-0.8.3/django_twined/migrations/0002_slug_unique_and_not_editable.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.8.2/django_twined/migrations/0004_add_timestamps.py` & `django_twined-0.8.3/django_twined/migrations/0004_add_timestamps.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.8.2/django_twined/migrations/0005_question_date_help_text.py` & `django_twined-0.8.3/django_twined/migrations/0005_question_date_help_text.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.8.2/django_twined/migrations/0006_service_revisions_and_events.py` & `django_twined-0.8.3/django_twined/migrations/0006_service_revisions_and_events.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.8.2/django_twined/migrations/0007_registered_to_revision.py` & `django_twined-0.8.3/django_twined/migrations/0007_registered_to_revision.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.8.2/django_twined/migrations/0008_registered_relations_to_nullable.py` & `django_twined-0.8.3/django_twined/migrations/0008_registered_relations_to_nullable.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.8.2/django_twined/migrations/0009_remove_registered_services.py` & `django_twined-0.8.3/django_twined/migrations/0009_remove_registered_services.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.8.2/django_twined/migrations/0010_alter_servicerevision_project_name.py` & `django_twined-0.8.3/django_twined/migrations/0010_alter_servicerevision_project_name.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.8.2/django_twined/migrations/0012_servicerevision_is_default.py` & `django_twined-0.8.3/django_twined/migrations/0012_servicerevision_is_default.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.8.2/django_twined/migrations/0013_alter_serviceusageevent_question.py` & `django_twined-0.8.3/django_twined/migrations/0013_alter_serviceusageevent_question.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.8.2/django_twined/migrations/0014_question_status.py` & `django_twined-0.8.3/django_twined/migrations/0014_question_status.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.8.2/django_twined/models/__init__.py` & `django_twined-0.8.3/django_twined/models/__init__.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.8.2/django_twined/models/datastores.py` & `django_twined-0.8.3/django_twined/models/datastores.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.8.2/django_twined/models/querysets/datastore_queryset.py` & `django_twined-0.8.3/django_twined/models/querysets/datastore_queryset.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.8.2/django_twined/models/questions.py` & `django_twined-0.8.3/django_twined/models/questions.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.8.2/django_twined/models/service_revisions.py` & `django_twined-0.8.3/django_twined/models/service_revisions.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.8.2/django_twined/models/service_usage_events.py` & `django_twined-0.8.3/django_twined/models/service_usage_events.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.8.2/django_twined/signals/receivers.py` & `django_twined-0.8.3/django_twined/signals/receivers.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.8.2/django_twined/templates/admin/question_ask_row.html` & `django_twined-0.8.3/django_twined/templates/admin/question_ask_row.html`

 * *Files identical despite different names*

### Comparing `django_twined-0.8.2/django_twined/views.py` & `django_twined-0.8.3/django_twined/views.py`

 * *Files identical despite different names*

### Comparing `django_twined-0.8.2/pyproject.toml` & `django_twined-0.8.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-twined"
-version = "0.8.2"
+version = "0.8.3"
 description = "A django app to manage octue services"
 authors = ["Tom Clark <tom@octue.com>", "Marcus Lugg <marcus@octue.com>"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
@@ -19,15 +19,15 @@
 keywords = ["django", "services", "octue", "twined"]
 packages = [{ include = "django_twined" },]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4"
 django = ">=3.0,<5.0"
 octue = ">=0.52.0,<1"
-django-gcp = ">=0.11.5,<0.12"
+django-gcp = ">=0.11.5,<0.13"
 django-jsoneditor = "^0.2.2"
 django-model-utils = "^4.2.0"
 
 
 [tool.poetry.group.dev.dependencies]
 channels = ">=3.0,<5.0"
 coverage = "^6.2"
```

### Comparing `django_twined-0.8.2/PKG-INFO` & `django_twined-0.8.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-twined
-Version: 0.8.2
+Version: 0.8.3
 Summary: A django app to manage octue services
 Home-page: https://github.com/octue/django-twined
 License: MIT
 Keywords: django,services,octue,twined
 Author: Tom Clark
 Author-email: tom@octue.com
 Requires-Python: >=3.9,<4
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: django (>=3.0,<5.0)
-Requires-Dist: django-gcp (>=0.11.5,<0.12)
+Requires-Dist: django-gcp (>=0.11.5,<0.13)
 Requires-Dist: django-jsoneditor (>=0.2.2,<0.3.0)
 Requires-Dist: django-model-utils (>=4.2.0,<5.0.0)
 Requires-Dist: octue (>=0.52.0,<1)
 Project-URL: Repository, https://github.com/octue/django-twined
 Description-Content-Type: text/markdown
 
 [![PyPI version](https://badge.fury.io/py/django-twined.svg)](https://badge.fury.io/py/django-twined)
```

