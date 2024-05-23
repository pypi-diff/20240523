# Comparing `tmp/wagtail_zoom_integration-0.0.6.tar.gz` & `tmp/wagtail_zoom_integration-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail_zoom_integration-0.0.6.tar", last modified: Fri Apr 19 13:57:57 2024, max compression
+gzip compressed data, was "wagtail_zoom_integration-0.0.7.tar", last modified: Thu May 23 10:26:49 2024, max compression
```

## Comparing `wagtail_zoom_integration-0.0.6.tar` & `wagtail_zoom_integration-0.0.7.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:57:57.507942 wagtail_zoom_integration-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-19 13:57:53.000000 wagtail_zoom_integration-0.0.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7820 2024-04-19 13:57:57.507942 wagtail_zoom_integration-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6820 2024-04-19 13:57:53.000000 wagtail_zoom_integration-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-19 13:57:53.000000 wagtail_zoom_integration-0.0.6/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:57:57.503942 wagtail_zoom_integration-0.0.6/sandbox/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:57:53.000000 wagtail_zoom_integration-0.0.6/sandbox/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:57:57.503942 wagtail_zoom_integration-0.0.6/sandbox/home/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:57:53.000000 wagtail_zoom_integration-0.0.6/sandbox/home/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:57:57.503942 wagtail_zoom_integration-0.0.6/sandbox/home/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-19 13:57:53.000000 wagtail_zoom_integration-0.0.6/sandbox/home/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-04-19 13:57:53.000000 wagtail_zoom_integration-0.0.6/sandbox/home/migrations/0002_create_homepage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-19 13:57:53.000000 wagtail_zoom_integration-0.0.6/sandbox/home/migrations/0003_eventregistrationpage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-04-19 13:57:53.000000 wagtail_zoom_integration-0.0.6/sandbox/home/migrations/0004_formfield.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:57:53.000000 wagtail_zoom_integration-0.0.6/sandbox/home/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-19 13:57:53.000000 wagtail_zoom_integration-0.0.6/sandbox/home/models.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      254 2024-04-19 13:57:53.000000 wagtail_zoom_integration-0.0.6/sandbox/manage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:57:57.503942 wagtail_zoom_integration-0.0.6/sandbox/sandbox/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:57:53.000000 wagtail_zoom_integration-0.0.6/sandbox/sandbox/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:57:57.503942 wagtail_zoom_integration-0.0.6/sandbox/sandbox/settings/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:57:53.000000 wagtail_zoom_integration-0.0.6/sandbox/sandbox/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4541 2024-04-19 13:57:53.000000 wagtail_zoom_integration-0.0.6/sandbox/sandbox/settings/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-19 13:57:53.000000 wagtail_zoom_integration-0.0.6/sandbox/sandbox/settings/dev.py
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-19 13:57:53.000000 wagtail_zoom_integration-0.0.6/sandbox/sandbox/settings/production.py
--rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-04-19 13:57:53.000000 wagtail_zoom_integration-0.0.6/sandbox/sandbox/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-19 13:57:53.000000 wagtail_zoom_integration-0.0.6/sandbox/sandbox/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:57:57.503942 wagtail_zoom_integration-0.0.6/sandbox/search/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:57:53.000000 wagtail_zoom_integration-0.0.6/sandbox/search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-04-19 13:57:53.000000 wagtail_zoom_integration-0.0.6/sandbox/search/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-19 13:57:57.511942 wagtail_zoom_integration-0.0.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:57:57.507942 wagtail_zoom_integration-0.0.6/wagtail_zoom_integration.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7820 2024-04-19 13:57:57.000000 wagtail_zoom_integration-0.0.6/wagtail_zoom_integration.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-19 13:57:57.000000 wagtail_zoom_integration-0.0.6/wagtail_zoom_integration.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 13:57:57.000000 wagtail_zoom_integration-0.0.6/wagtail_zoom_integration.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-19 13:57:57.000000 wagtail_zoom_integration-0.0.6/wagtail_zoom_integration.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-19 13:57:57.000000 wagtail_zoom_integration-0.0.6/wagtail_zoom_integration.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:57:57.507942 wagtail_zoom_integration-0.0.6/wagtailzoom/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:57:53.000000 wagtail_zoom_integration-0.0.6/wagtailzoom/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-19 13:57:53.000000 wagtail_zoom_integration-0.0.6/wagtailzoom/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)     4984 2024-04-19 13:57:53.000000 wagtail_zoom_integration-0.0.6/wagtailzoom/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-19 13:57:53.000000 wagtail_zoom_integration-0.0.6/wagtailzoom/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-19 13:57:53.000000 wagtail_zoom_integration-0.0.6/wagtailzoom/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-04-19 13:57:53.000000 wagtail_zoom_integration-0.0.6/wagtailzoom/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:57:57.507942 wagtail_zoom_integration-0.0.6/wagtailzoom/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-19 13:57:53.000000 wagtail_zoom_integration-0.0.6/wagtailzoom/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-19 13:57:53.000000 wagtail_zoom_integration-0.0.6/wagtailzoom/migrations/0002_remove_zoomsettings_api_key_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 13:57:53.000000 wagtail_zoom_integration-0.0.6/wagtailzoom/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5679 2024-04-19 13:57:53.000000 wagtail_zoom_integration-0.0.6/wagtailzoom/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:57:57.503942 wagtail_zoom_integration-0.0.6/wagtailzoom/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:57:57.507942 wagtail_zoom_integration-0.0.6/wagtailzoom/templates/wagtailzoom/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 13:57:57.507942 wagtail_zoom_integration-0.0.6/wagtailzoom/templates/wagtailzoom/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-19 13:57:53.000000 wagtail_zoom_integration-0.0.6/wagtailzoom/templates/wagtailzoom/widgets/zoom_event_select_widget.html
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-04-19 13:57:53.000000 wagtail_zoom_integration-0.0.6/wagtailzoom/templates/wagtailzoom/widgets/zoom_event_select_widget_js.html
--rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-04-19 13:57:53.000000 wagtail_zoom_integration-0.0.6/wagtailzoom/templates/wagtailzoom/zoom_integration_form.html
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-19 13:57:53.000000 wagtail_zoom_integration-0.0.6/wagtailzoom/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     4209 2024-04-19 13:57:53.000000 wagtail_zoom_integration-0.0.6/wagtailzoom/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     3335 2024-04-19 13:57:53.000000 wagtail_zoom_integration-0.0.6/wagtailzoom/wagtail_hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-04-19 13:57:53.000000 wagtail_zoom_integration-0.0.6/wagtailzoom/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:26:49.343329 wagtail_zoom_integration-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-23 10:26:45.000000 wagtail_zoom_integration-0.0.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7828 2024-05-23 10:26:49.343329 wagtail_zoom_integration-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6820 2024-05-23 10:26:45.000000 wagtail_zoom_integration-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-23 10:26:45.000000 wagtail_zoom_integration-0.0.7/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:26:49.335329 wagtail_zoom_integration-0.0.7/sandbox/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 10:26:45.000000 wagtail_zoom_integration-0.0.7/sandbox/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:26:49.335329 wagtail_zoom_integration-0.0.7/sandbox/home/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 10:26:45.000000 wagtail_zoom_integration-0.0.7/sandbox/home/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:26:49.339329 wagtail_zoom_integration-0.0.7/sandbox/home/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-23 10:26:45.000000 wagtail_zoom_integration-0.0.7/sandbox/home/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-05-23 10:26:45.000000 wagtail_zoom_integration-0.0.7/sandbox/home/migrations/0002_create_homepage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-05-23 10:26:45.000000 wagtail_zoom_integration-0.0.7/sandbox/home/migrations/0003_eventregistrationpage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-05-23 10:26:45.000000 wagtail_zoom_integration-0.0.7/sandbox/home/migrations/0004_formfield.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 10:26:45.000000 wagtail_zoom_integration-0.0.7/sandbox/home/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-23 10:26:45.000000 wagtail_zoom_integration-0.0.7/sandbox/home/models.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      254 2024-05-23 10:26:45.000000 wagtail_zoom_integration-0.0.7/sandbox/manage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:26:49.339329 wagtail_zoom_integration-0.0.7/sandbox/sandbox/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 10:26:45.000000 wagtail_zoom_integration-0.0.7/sandbox/sandbox/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:26:49.339329 wagtail_zoom_integration-0.0.7/sandbox/sandbox/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 10:26:45.000000 wagtail_zoom_integration-0.0.7/sandbox/sandbox/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4541 2024-05-23 10:26:45.000000 wagtail_zoom_integration-0.0.7/sandbox/sandbox/settings/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-05-23 10:26:45.000000 wagtail_zoom_integration-0.0.7/sandbox/sandbox/settings/dev.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-23 10:26:45.000000 wagtail_zoom_integration-0.0.7/sandbox/sandbox/settings/production.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-05-23 10:26:45.000000 wagtail_zoom_integration-0.0.7/sandbox/sandbox/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-23 10:26:45.000000 wagtail_zoom_integration-0.0.7/sandbox/sandbox/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:26:49.339329 wagtail_zoom_integration-0.0.7/sandbox/search/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 10:26:45.000000 wagtail_zoom_integration-0.0.7/sandbox/search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-23 10:26:45.000000 wagtail_zoom_integration-0.0.7/sandbox/search/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-23 10:26:49.343329 wagtail_zoom_integration-0.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:26:49.343329 wagtail_zoom_integration-0.0.7/wagtail_zoom_integration.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7828 2024-05-23 10:26:49.000000 wagtail_zoom_integration-0.0.7/wagtail_zoom_integration.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-23 10:26:49.000000 wagtail_zoom_integration-0.0.7/wagtail_zoom_integration.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 10:26:49.000000 wagtail_zoom_integration-0.0.7/wagtail_zoom_integration.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-23 10:26:49.000000 wagtail_zoom_integration-0.0.7/wagtail_zoom_integration.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-23 10:26:49.000000 wagtail_zoom_integration-0.0.7/wagtail_zoom_integration.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:26:49.343329 wagtail_zoom_integration-0.0.7/wagtailzoom/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 10:26:45.000000 wagtail_zoom_integration-0.0.7/wagtailzoom/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-23 10:26:45.000000 wagtail_zoom_integration-0.0.7/wagtailzoom/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5340 2024-05-23 10:26:45.000000 wagtail_zoom_integration-0.0.7/wagtailzoom/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-23 10:26:45.000000 wagtail_zoom_integration-0.0.7/wagtailzoom/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-23 10:26:45.000000 wagtail_zoom_integration-0.0.7/wagtailzoom/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-05-23 10:26:45.000000 wagtail_zoom_integration-0.0.7/wagtailzoom/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:26:49.343329 wagtail_zoom_integration-0.0.7/wagtailzoom/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-05-23 10:26:45.000000 wagtail_zoom_integration-0.0.7/wagtailzoom/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-05-23 10:26:45.000000 wagtail_zoom_integration-0.0.7/wagtailzoom/migrations/0002_remove_zoomsettings_api_key_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 10:26:45.000000 wagtail_zoom_integration-0.0.7/wagtailzoom/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5679 2024-05-23 10:26:45.000000 wagtail_zoom_integration-0.0.7/wagtailzoom/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:26:49.335329 wagtail_zoom_integration-0.0.7/wagtailzoom/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:26:49.343329 wagtail_zoom_integration-0.0.7/wagtailzoom/templates/wagtailzoom/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 10:26:49.343329 wagtail_zoom_integration-0.0.7/wagtailzoom/templates/wagtailzoom/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-05-23 10:26:45.000000 wagtail_zoom_integration-0.0.7/wagtailzoom/templates/wagtailzoom/widgets/zoom_event_select_widget.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-23 10:26:45.000000 wagtail_zoom_integration-0.0.7/wagtailzoom/templates/wagtailzoom/widgets/zoom_event_select_widget_js.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-05-23 10:26:45.000000 wagtail_zoom_integration-0.0.7/wagtailzoom/templates/wagtailzoom/zoom_integration_form.html
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-23 10:26:45.000000 wagtail_zoom_integration-0.0.7/wagtailzoom/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4648 2024-05-23 10:26:45.000000 wagtail_zoom_integration-0.0.7/wagtailzoom/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3335 2024-05-23 10:26:45.000000 wagtail_zoom_integration-0.0.7/wagtailzoom/wagtail_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3282 2024-05-23 10:26:45.000000 wagtail_zoom_integration-0.0.7/wagtailzoom/widgets.py
```

### Comparing `wagtail_zoom_integration-0.0.6/PKG-INFO` & `wagtail_zoom_integration-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: wagtail-zoom-integration
-Version: 0.0.6
-Summary: Integrate Zoom Event registration registration in Wagtail Projects.
+Version: 0.0.7
+Summary: Integrate automated Zoom Events registration in Wagtail Form Builder Pages.
 Home-page: https://github.com/erick-otenyo/wagtail-zoom-integration
 Author: Erick Otenyo
 Author-email: otenyo.erick@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `wagtail_zoom_integration-0.0.6/README.md` & `wagtail_zoom_integration-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `wagtail_zoom_integration-0.0.6/sandbox/home/migrations/0001_initial.py` & `wagtail_zoom_integration-0.0.7/sandbox/home/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail_zoom_integration-0.0.6/sandbox/home/migrations/0002_create_homepage.py` & `wagtail_zoom_integration-0.0.7/sandbox/home/migrations/0002_create_homepage.py`

 * *Files identical despite different names*

### Comparing `wagtail_zoom_integration-0.0.6/sandbox/home/migrations/0003_eventregistrationpage.py` & `wagtail_zoom_integration-0.0.7/sandbox/home/migrations/0003_eventregistrationpage.py`

 * *Files identical despite different names*

### Comparing `wagtail_zoom_integration-0.0.6/sandbox/home/migrations/0004_formfield.py` & `wagtail_zoom_integration-0.0.7/sandbox/home/migrations/0004_formfield.py`

 * *Files identical despite different names*

### Comparing `wagtail_zoom_integration-0.0.6/sandbox/home/models.py` & `wagtail_zoom_integration-0.0.7/sandbox/home/models.py`

 * *Files identical despite different names*

### Comparing `wagtail_zoom_integration-0.0.6/sandbox/sandbox/settings/base.py` & `wagtail_zoom_integration-0.0.7/sandbox/sandbox/settings/base.py`

 * *Files identical despite different names*

### Comparing `wagtail_zoom_integration-0.0.6/sandbox/sandbox/urls.py` & `wagtail_zoom_integration-0.0.7/sandbox/sandbox/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail_zoom_integration-0.0.6/sandbox/search/views.py` & `wagtail_zoom_integration-0.0.7/sandbox/search/views.py`

 * *Files identical despite different names*

### Comparing `wagtail_zoom_integration-0.0.6/setup.cfg` & `wagtail_zoom_integration-0.0.7/setup.cfg`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [metadata]
 name = wagtail-zoom-integration
-version = 0.0.6
-description = Integrate Zoom Event registration registration in Wagtail Projects.
+version = 0.0.7
+description = Integrate automated Zoom Events registration in Wagtail Form Builder Pages.
 long_description = file:README.md
 long_description_content_type = text/markdown
 url = https://github.com/erick-otenyo/wagtail-zoom-integration
 author = Erick Otenyo
 author_email = otenyo.erick@gmail.com
 license = MIT
 classifiers =
```

### Comparing `wagtail_zoom_integration-0.0.6/wagtail_zoom_integration.egg-info/PKG-INFO` & `wagtail_zoom_integration-0.0.7/wagtail_zoom_integration.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: wagtail-zoom-integration
-Version: 0.0.6
-Summary: Integrate Zoom Event registration registration in Wagtail Projects.
+Version: 0.0.7
+Summary: Integrate automated Zoom Events registration in Wagtail Form Builder Pages.
 Home-page: https://github.com/erick-otenyo/wagtail-zoom-integration
 Author: Erick Otenyo
 Author-email: otenyo.erick@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `wagtail_zoom_integration-0.0.6/wagtail_zoom_integration.egg-info/SOURCES.txt` & `wagtail_zoom_integration-0.0.7/wagtail_zoom_integration.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wagtail_zoom_integration-0.0.6/wagtailzoom/api.py` & `wagtail_zoom_integration-0.0.7/wagtailzoom/api.py`

 * *Files 7% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     def _post(self, url, data):
         headers = {'Content-type': 'application/json', 'Accept': 'application/json', **self.headers}
         response = requests.post(url, json=data, headers=headers)
         response.raise_for_status()
         return response
 
     def get_meetings(self, limit=10):
-        url = "{}/users/me/meetings".format(self.base_url)
+        url = "{}/users/me/meetings?type=upcoming_meetings".format(self.base_url)
         response = self._get(url)
         response.raise_for_status()
 
         json_res = response.json()
 
         meetings = json_res.get("meetings", [])
 
@@ -63,18 +63,22 @@
             meetings = meetings[:limit]
             meetings = sorted(meetings, key=get_created_time, reverse=True)
 
             for index, meeting in enumerate(meetings):
                 meetings[index]["event_type"] = "meeting"
                 meetings[index]["event_type_label"] = "Meeting"
 
+        # sort by start time, with meeting closest to start  first
+        if meetings:
+            sorted(meetings, key=lambda x: x["start_time"]).reverse()
+
         return meetings
 
     def get_webinars(self, limit=10):
-        url = "{}/users/me/webinars".format(self.base_url)
+        url = "{}/users/me/webinars?type=upcoming".format(self.base_url)
         response = self._get(url)
 
         response.raise_for_status()
 
         json_res = response.json()
         webinars = json_res.get("webinars", [])
 
@@ -82,21 +86,25 @@
             webinars = webinars[:limit]
             webinars = sorted(webinars, key=get_created_time, reverse=True)
 
             for index, webinar in enumerate(webinars):
                 webinars[index]["event_type"] = "webinar"
                 webinars[index]["event_type_label"] = "Webinar"
 
+        # sort by start time, with webinar closest to start first
+        if webinars:
+            sorted(webinars, key=lambda x: x["start_time"]).reverse()
+
         return webinars
 
     def get_events(self):
-        meetings = self.get_meetings(limit=5)
+        meetings = self.get_meetings(limit=20)
 
         try:
-            webinars = self.get_webinars(limit=5)
+            webinars = self.get_webinars(limit=20)
             meetings.extend(webinars)
         except Exception as e:
             pass
 
         return meetings
 
     def get_meeting(self, meeting_id):
```

### Comparing `wagtail_zoom_integration-0.0.6/wagtailzoom/forms.py` & `wagtail_zoom_integration-0.0.7/wagtailzoom/forms.py`

 * *Files identical despite different names*

### Comparing `wagtail_zoom_integration-0.0.6/wagtailzoom/migrations/0001_initial.py` & `wagtail_zoom_integration-0.0.7/wagtailzoom/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail_zoom_integration-0.0.6/wagtailzoom/migrations/0002_remove_zoomsettings_api_key_and_more.py` & `wagtail_zoom_integration-0.0.7/wagtailzoom/migrations/0002_remove_zoomsettings_api_key_and_more.py`

 * *Files identical despite different names*

### Comparing `wagtail_zoom_integration-0.0.6/wagtailzoom/models.py` & `wagtail_zoom_integration-0.0.7/wagtailzoom/models.py`

 * *Files identical despite different names*

### Comparing `wagtail_zoom_integration-0.0.6/wagtailzoom/templates/wagtailzoom/widgets/zoom_event_select_widget_js.html` & `wagtail_zoom_integration-0.0.7/wagtailzoom/templates/wagtailzoom/widgets/zoom_event_select_widget_js.html`

 * *Files identical despite different names*

### Comparing `wagtail_zoom_integration-0.0.6/wagtailzoom/templates/wagtailzoom/zoom_integration_form.html` & `wagtail_zoom_integration-0.0.7/wagtailzoom/templates/wagtailzoom/zoom_integration_form.html`

 * *Files identical despite different names*

### Comparing `wagtail_zoom_integration-0.0.6/wagtailzoom/views.py` & `wagtail_zoom_integration-0.0.7/wagtailzoom/views.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import json
 
 from django.http import HttpResponseRedirect
 from django.shortcuts import render
 from django.urls import reverse
 from django.utils.translation import gettext as _
 from modelcluster.models import get_all_child_relations
+from requests import HTTPError
 from wagtail.contrib.forms.models import AbstractFormField
 from wagtail.models import Page
 
 from .api import ZoomApi
 from .errors import ZoomApiCredentialsError
 from .forms import ZoomIntegrationForm
 from .models import ZoomSettings
@@ -44,24 +45,34 @@
 
                     approval_type = zoom_event.get("settings", {}).get("approval_type")
                     context.update({"zoom_event": zoom_event})
 
                     if approval_type == 2:
                         topic = zoom_event.get("topic")
                         context.update({
-                            "zoom_error": f"Registration is not enabled for the event '{topic}'. "
-                                          f"Please enable registration for this event in your Zoom Account "
-                                          f"and try again"})
+                            "zoom_error": _(
+                                "Registration is not enabled for the event '%(topic)s'. Please enable registration "
+                                "for this event in your Zoom Account and try again") % {"topic": topic}})
 
             except ZoomApiCredentialsError as e:
                 context.update({"zoom_error": e.message})
-            except Exception:
-                context.update({"zoom_error": _("Error obtaining Zoom event. "
-                                                "Please make sure the Zoom credentials in Zoom Settings are correct, "
-                                                "and have required Zoom Account access scope.")})
+            except Exception as e:
+                error_message = _("Error obtaining Zoom event.")
+
+                if isinstance(e, HTTPError):
+                    json_response = e.response.json()
+                    if json_response and json_response.get("message"):
+                        message = json_response.get("message")
+                        error_message = f"{error_message} {message}"
+                else:
+                    message = _("Please make sure the Zoom credentials in Zoom Settings are correct and have required "
+                                "Zoom Account access scope")
+                    error_message = f"{error_message}  {message}"
+
+                context.update({"zoom_error": error_message})
 
     if context.get("zoom_error"):
         return render(request, template_name, context=context)
 
     form_fields_rel_name = None
     # get form fields relation name
     relations = get_all_child_relations(form_page)
```

### Comparing `wagtail_zoom_integration-0.0.6/wagtailzoom/wagtail_hooks.py` & `wagtail_zoom_integration-0.0.7/wagtailzoom/wagtail_hooks.py`

 * *Files identical despite different names*

### Comparing `wagtail_zoom_integration-0.0.6/wagtailzoom/widgets.py` & `wagtail_zoom_integration-0.0.7/wagtailzoom/widgets.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import json
 
 from django.forms.widgets import Input, Select
 from django.template.loader import render_to_string
 from django.utils.translation import gettext as _
+from requests import HTTPError
 from wagtail.models import Site
 
 from .api import ZoomApi
 from .errors import ZoomApiCredentialsError
 
 
 class CustomSelect(Select):
@@ -36,19 +37,26 @@
         except ZoomApiCredentialsError as e:
             zoom_error = e.message
         except Exception as e:
             zoom_error = _("Error obtaining Zoom events. "
                            "Please make sure the Zoom credentials in Zoom Settings are correct, "
                            "and have required Zoom Account access scope.")
 
+            if isinstance(e, HTTPError):
+                response = e.response.json()
+                if response and response.get("message"):
+                    zoom_error += _("- Specific Error: ") + response.get("message")
+
         ctx["widget"]["value"] = json.dumps(json_value)
         ctx['widget']['extra_js'] = self.render_js(name, event_id, zoom_events)
         ctx["widget"]["selectable_events"] = zoom_events
         ctx["widget"]["stored_event_id"] = event_id
         ctx["widget"]["zoom_error"] = zoom_error
+        ctx["widget"]["no_events_message"] = _("No Upcoming or Ongoing Meetings/Webinars found. "
+                                               "Please create one on Zoom and try again.")
 
         return ctx
 
     def render_js(self, name, event_id, zoom_events):
         ctx = {
             "widget_name": name,
             "widget_js_name": name.replace('-', '_'),
```

