# Comparing `tmp/pyslth-0.4.8.tar.gz` & `tmp/pyslth-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyslth-0.4.8.tar", last modified: Wed May 22 16:45:58 2024, max compression
+gzip compressed data, was "pyslth-0.4.9.tar", last modified: Thu May 23 10:26:14 2024, max compression
```

## Comparing `pyslth-0.4.8.tar` & `pyslth-0.4.9.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-22 16:45:58.906458 pyslth-0.4.8/
--rw-r--r--   0 breno      (501) staff       (20)       96 2024-04-27 20:11:05.000000 pyslth-0.4.8/MANIFEST.in
--rw-r--r--   0 breno      (501) staff       (20)      590 2024-05-22 16:45:58.906188 pyslth-0.4.8/PKG-INFO
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-22 16:45:58.805660 pyslth-0.4.8/pyslth.egg-info/
--rw-r--r--   0 breno      (501) staff       (20)      590 2024-05-22 16:45:58.000000 pyslth-0.4.8/pyslth.egg-info/PKG-INFO
--rw-r--r--   0 breno      (501) staff       (20)     1958 2024-05-22 16:45:58.000000 pyslth-0.4.8/pyslth.egg-info/SOURCES.txt
--rw-r--r--   0 breno      (501) staff       (20)        1 2024-05-22 16:45:58.000000 pyslth-0.4.8/pyslth.egg-info/dependency_links.txt
--rw-r--r--   0 breno      (501) staff       (20)      163 2024-05-22 16:45:58.000000 pyslth-0.4.8/pyslth.egg-info/requires.txt
--rw-r--r--   0 breno      (501) staff       (20)        5 2024-05-22 16:45:58.000000 pyslth-0.4.8/pyslth.egg-info/top_level.txt
--rw-r--r--   0 breno      (501) staff       (20)      155 2024-04-27 19:55:48.000000 pyslth-0.4.8/requirements.txt
--rw-r--r--   0 breno      (501) staff       (20)       38 2024-05-22 16:45:58.906538 pyslth-0.4.8/setup.cfg
--rw-r--r--   0 breno      (501) staff       (20)      929 2024-05-22 16:45:42.000000 pyslth-0.4.8/setup.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-22 16:45:58.828560 pyslth-0.4.8/slth/
--rw-r--r--   0 breno      (501) staff       (20)     3779 2024-05-10 13:02:33.000000 pyslth-0.4.8/slth/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)     9973 2024-05-22 14:21:00.000000 pyslth-0.4.8/slth/components.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-22 16:45:58.830475 pyslth-0.4.8/slth/db/
--rw-r--r--   0 breno      (501) staff       (20)       46 2024-04-21 03:07:00.000000 pyslth-0.4.8/slth/db/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)     5031 2024-05-13 19:37:29.000000 pyslth-0.4.8/slth/db/models.py
--rw-r--r--   0 breno      (501) staff       (20)    25441 2024-05-22 14:22:43.000000 pyslth-0.4.8/slth/endpoints.py
--rw-r--r--   0 breno      (501) staff       (20)      156 2024-04-09 12:56:09.000000 pyslth-0.4.8/slth/exceptions.py
--rw-r--r--   0 breno      (501) staff       (20)     4451 2024-05-16 10:23:26.000000 pyslth-0.4.8/slth/factory.py
--rw-r--r--   0 breno      (501) staff       (20)    26814 2024-05-22 12:50:05.000000 pyslth-0.4.8/slth/forms.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-22 16:45:58.830904 pyslth-0.4.8/slth/management/
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.4.8/slth/management/__init__.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-22 16:45:58.834409 pyslth-0.4.8/slth/management/commands/
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.4.8/slth/management/commands/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)     1599 2024-04-13 14:42:59.000000 pyslth-0.4.8/slth/management/commands/integration_test.py
--rw-r--r--   0 breno      (501) staff       (20)     1276 2024-04-09 17:55:35.000000 pyslth-0.4.8/slth/management/commands/sync.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-22 16:45:58.843896 pyslth-0.4.8/slth/migrations/
--rw-r--r--   0 breno      (501) staff       (20)     1392 2024-05-01 14:04:01.000000 pyslth-0.4.8/slth/migrations/0001_initial.py
--rw-r--r--   0 breno      (501) staff       (20)     3513 2024-04-19 09:33:48.000000 pyslth-0.4.8/slth/migrations/0002_email_role_pushsubscription_error.py
--rw-r--r--   0 breno      (501) staff       (20)      601 2024-05-01 14:04:01.000000 pyslth-0.4.8/slth/migrations/0003_rename_photo_profile_alter_profile_options.py
--rw-r--r--   0 breno      (501) staff       (20)      451 2024-05-01 14:04:01.000000 pyslth-0.4.8/slth/migrations/0004_alter_profile_photo.py
--rw-r--r--   0 breno      (501) staff       (20)      450 2024-05-01 14:04:01.000000 pyslth-0.4.8/slth/migrations/0005_alter_profile_photo.py
--rw-r--r--   0 breno      (501) staff       (20)      854 2024-04-28 09:44:45.000000 pyslth-0.4.8/slth/migrations/0006_user.py
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.4.8/slth/migrations/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)     6546 2024-05-11 10:34:23.000000 pyslth-0.4.8/slth/models.py
--rw-r--r--   0 breno      (501) staff       (20)      565 2024-05-18 08:21:00.000000 pyslth-0.4.8/slth/notifications.py
--rw-r--r--   0 breno      (501) staff       (20)     2594 2024-05-06 09:55:03.000000 pyslth-0.4.8/slth/oauth.py
--rw-r--r--   0 breno      (501) staff       (20)     1906 2024-05-18 17:29:04.000000 pyslth-0.4.8/slth/permissions.py
--rw-r--r--   0 breno      (501) staff       (20)    19965 2024-05-16 13:39:18.000000 pyslth-0.4.8/slth/queryset.py
--rw-r--r--   0 breno      (501) staff       (20)     4724 2024-04-19 09:29:01.000000 pyslth-0.4.8/slth/roles.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-22 16:45:58.844860 pyslth-0.4.8/slth/selenium/
--rw-r--r--   0 breno      (501) staff       (20)     9095 2024-04-28 09:44:40.000000 pyslth-0.4.8/slth/selenium/__init__.py
--rw-r--r--   0 breno      (501) staff       (20)    11350 2024-04-30 08:48:10.000000 pyslth-0.4.8/slth/selenium/browser.py
--rw-r--r--   0 breno      (501) staff       (20)    15969 2024-05-21 20:16:17.000000 pyslth-0.4.8/slth/serializer.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-22 16:45:58.848045 pyslth-0.4.8/slth/static/
--rw-r--r--   0 breno      (501) staff       (20)     6148 2024-05-20 11:57:45.000000 pyslth-0.4.8/slth/static/.DS_Store
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-22 16:45:58.854054 pyslth-0.4.8/slth/static/css/
--rw-r--r--   0 breno      (501) staff       (20)     6148 2024-04-29 19:56:09.000000 pyslth-0.4.8/slth/static/css/.DS_Store
--rw-r--r--   0 breno      (501) staff       (20)    80823 2024-04-27 15:01:32.000000 pyslth-0.4.8/slth/static/css/fontawesome.min.css
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-22 16:45:58.866796 pyslth-0.4.8/slth/static/css/fonts/
--rw-r--r--   0 breno      (501) staff       (20)     6148 2024-04-29 19:36:17.000000 pyslth-0.4.8/slth/static/css/fonts/.DS_Store
--rw-r--r--   0 breno      (501) staff       (20)   150020 2024-04-27 15:01:32.000000 pyslth-0.4.8/slth/static/css/fonts/fa-solid-900.woff2
--rw-r--r--   0 breno      (501) staff       (20)   115080 2024-04-29 19:28:27.000000 pyslth-0.4.8/slth/static/css/fonts/rawline-400.woff
--rw-r--r--   0 breno      (501) staff       (20)   117252 2024-04-29 19:29:24.000000 pyslth-0.4.8/slth/static/css/fonts/rawline-500i.woff
--rw-r--r--   0 breno      (501) staff       (20)   117076 2024-04-29 19:36:27.000000 pyslth-0.4.8/slth/static/css/fonts/rawline-700.woff
--rw-r--r--   0 breno      (501) staff       (20)     1977 2024-05-12 18:54:58.000000 pyslth-0.4.8/slth/static/css/slth.css
--rw-r--r--   0 breno      (501) staff       (20)      515 2024-04-27 15:44:29.000000 pyslth-0.4.8/slth/static/css/solid.min.css
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-05-07 11:57:26.000000 pyslth-0.4.8/slth/static/css/style.css
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-22 16:45:58.874298 pyslth-0.4.8/slth/static/images/
--rw-r--r--   0 breno      (501) staff       (20)    10828 2024-04-15 11:56:33.000000 pyslth-0.4.8/slth/static/images/logo.png
--rw-r--r--   0 breno      (501) staff       (20)     2432 2024-04-13 03:35:59.000000 pyslth-0.4.8/slth/static/images/logo.svg
--rw-r--r--   0 breno      (501) staff       (20)    16754 2024-04-16 09:42:03.000000 pyslth-0.4.8/slth/static/images/user.png
--rw-r--r--   0 breno      (501) staff       (20)      492 2024-05-07 12:51:28.000000 pyslth-0.4.8/slth/static/images/user.svg
--rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-27 17:47:02.000000 pyslth-0.4.8/slth/static/index.html
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-22 16:45:58.902197 pyslth-0.4.8/slth/static/js/
--rw-r--r--   0 breno      (501) staff       (20)      946 2024-05-19 17:15:44.000000 pyslth-0.4.8/slth/static/js/default-passive-events.min.js
--rw-r--r--   0 breno      (501) staff       (20)  1112413 2024-05-18 14:48:49.000000 pyslth-0.4.8/slth/static/js/echarts.min.js
--rw-r--r--   0 breno      (501) staff       (20)      756 2024-05-22 16:45:49.000000 pyslth-0.4.8/slth/static/js/index.min.js
--rw-r--r--   0 breno      (501) staff       (20)     1601 2024-05-02 09:27:38.000000 pyslth-0.4.8/slth/static/js/ios-splash.min.js
--rw-r--r--   0 breno      (501) staff       (20)   117723 2024-05-08 16:11:56.000000 pyslth-0.4.8/slth/static/js/peerjs.min.js
--rw-r--r--   0 breno      (501) staff       (20)    92865 2024-05-19 22:43:39.000000 pyslth-0.4.8/slth/static/js/peerjs154.min.js
--rw-r--r--   0 breno      (501) staff       (20)    19927 2024-04-27 15:01:32.000000 pyslth-0.4.8/slth/static/js/qrcode.min.js
--rw-r--r--   0 breno      (501) staff       (20)     6176 2024-04-27 15:01:32.000000 pyslth-0.4.8/slth/static/js/react-trigger-change.js
--rw-r--r--   0 breno      (501) staff       (20)   141870 2024-05-22 16:45:49.000000 pyslth-0.4.8/slth/static/js/react.min.js
--rw-r--r--   0 breno      (501) staff       (20)   102279 2024-05-22 16:45:49.000000 pyslth-0.4.8/slth/static/js/slth.min.js
--rw-rw-r--   0 breno      (501) staff       (20)     7401 2024-04-27 15:01:32.000000 pyslth-0.4.8/slth/static/js/vanilla-masker.js
--rw-r--r--   0 breno      (501) staff       (20)     5720 2024-04-27 15:01:32.000000 pyslth-0.4.8/slth/static/js/vanilla-masker.min.js
--rw-r--r--   0 breno      (501) staff       (20)     6361 2024-05-16 13:05:44.000000 pyslth-0.4.8/slth/statistics.py
-drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-22 16:45:58.905684 pyslth-0.4.8/slth/templates/
--rw-r--r--   0 breno      (501) staff       (20)     3230 2024-05-19 22:46:51.000000 pyslth-0.4.8/slth/templates/index.html
--rw-r--r--   0 breno      (501) staff       (20)     1456 2024-05-18 10:06:11.000000 pyslth-0.4.8/slth/templates/service-worker.js
--rw-r--r--   0 breno      (501) staff       (20)     5528 2024-04-16 18:07:11.000000 pyslth-0.4.8/slth/tests.py
--rw-r--r--   0 breno      (501) staff       (20)      797 2024-04-29 14:21:39.000000 pyslth-0.4.8/slth/urls.py
--rw-r--r--   0 breno      (501) staff       (20)     1000 2024-05-13 01:26:42.000000 pyslth-0.4.8/slth/utils.py
--rw-r--r--   0 breno      (501) staff       (20)     2572 2024-05-08 14:06:07.000000 pyslth-0.4.8/slth/views.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-23 10:26:14.407265 pyslth-0.4.9/
+-rw-r--r--   0 breno      (501) staff       (20)       96 2024-04-27 20:11:05.000000 pyslth-0.4.9/MANIFEST.in
+-rw-r--r--   0 breno      (501) staff       (20)      590 2024-05-23 10:26:14.407061 pyslth-0.4.9/PKG-INFO
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-23 10:26:14.369045 pyslth-0.4.9/pyslth.egg-info/
+-rw-r--r--   0 breno      (501) staff       (20)      590 2024-05-23 10:26:14.000000 pyslth-0.4.9/pyslth.egg-info/PKG-INFO
+-rw-r--r--   0 breno      (501) staff       (20)     1958 2024-05-23 10:26:14.000000 pyslth-0.4.9/pyslth.egg-info/SOURCES.txt
+-rw-r--r--   0 breno      (501) staff       (20)        1 2024-05-23 10:26:14.000000 pyslth-0.4.9/pyslth.egg-info/dependency_links.txt
+-rw-r--r--   0 breno      (501) staff       (20)      163 2024-05-23 10:26:14.000000 pyslth-0.4.9/pyslth.egg-info/requires.txt
+-rw-r--r--   0 breno      (501) staff       (20)        5 2024-05-23 10:26:14.000000 pyslth-0.4.9/pyslth.egg-info/top_level.txt
+-rw-r--r--   0 breno      (501) staff       (20)      155 2024-04-27 19:55:48.000000 pyslth-0.4.9/requirements.txt
+-rw-r--r--   0 breno      (501) staff       (20)       38 2024-05-23 10:26:14.407325 pyslth-0.4.9/setup.cfg
+-rw-r--r--   0 breno      (501) staff       (20)      929 2024-05-23 10:25:26.000000 pyslth-0.4.9/setup.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-23 10:26:14.378025 pyslth-0.4.9/slth/
+-rw-r--r--   0 breno      (501) staff       (20)     3779 2024-05-10 13:02:33.000000 pyslth-0.4.9/slth/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)     9973 2024-05-23 09:22:14.000000 pyslth-0.4.9/slth/components.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-23 10:26:14.378619 pyslth-0.4.9/slth/db/
+-rw-r--r--   0 breno      (501) staff       (20)       46 2024-04-21 03:07:00.000000 pyslth-0.4.9/slth/db/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)     5031 2024-05-13 19:37:29.000000 pyslth-0.4.9/slth/db/models.py
+-rw-r--r--   0 breno      (501) staff       (20)    25488 2024-05-23 09:31:24.000000 pyslth-0.4.9/slth/endpoints.py
+-rw-r--r--   0 breno      (501) staff       (20)      156 2024-04-09 12:56:09.000000 pyslth-0.4.9/slth/exceptions.py
+-rw-r--r--   0 breno      (501) staff       (20)     4451 2024-05-16 10:23:26.000000 pyslth-0.4.9/slth/factory.py
+-rw-r--r--   0 breno      (501) staff       (20)    26979 2024-05-23 09:31:15.000000 pyslth-0.4.9/slth/forms.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-23 10:26:14.378929 pyslth-0.4.9/slth/management/
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.4.9/slth/management/__init__.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-23 10:26:14.379518 pyslth-0.4.9/slth/management/commands/
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.4.9/slth/management/commands/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)     1599 2024-04-13 14:42:59.000000 pyslth-0.4.9/slth/management/commands/integration_test.py
+-rw-r--r--   0 breno      (501) staff       (20)     1276 2024-04-09 17:55:35.000000 pyslth-0.4.9/slth/management/commands/sync.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-23 10:26:14.382465 pyslth-0.4.9/slth/migrations/
+-rw-r--r--   0 breno      (501) staff       (20)     1392 2024-05-01 14:04:01.000000 pyslth-0.4.9/slth/migrations/0001_initial.py
+-rw-r--r--   0 breno      (501) staff       (20)     3513 2024-04-19 09:33:48.000000 pyslth-0.4.9/slth/migrations/0002_email_role_pushsubscription_error.py
+-rw-r--r--   0 breno      (501) staff       (20)      601 2024-05-01 14:04:01.000000 pyslth-0.4.9/slth/migrations/0003_rename_photo_profile_alter_profile_options.py
+-rw-r--r--   0 breno      (501) staff       (20)      451 2024-05-01 14:04:01.000000 pyslth-0.4.9/slth/migrations/0004_alter_profile_photo.py
+-rw-r--r--   0 breno      (501) staff       (20)      450 2024-05-01 14:04:01.000000 pyslth-0.4.9/slth/migrations/0005_alter_profile_photo.py
+-rw-r--r--   0 breno      (501) staff       (20)      854 2024-04-28 09:44:45.000000 pyslth-0.4.9/slth/migrations/0006_user.py
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-09 12:56:09.000000 pyslth-0.4.9/slth/migrations/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)     6546 2024-05-11 10:34:23.000000 pyslth-0.4.9/slth/models.py
+-rw-r--r--   0 breno      (501) staff       (20)      565 2024-05-18 08:21:00.000000 pyslth-0.4.9/slth/notifications.py
+-rw-r--r--   0 breno      (501) staff       (20)     2594 2024-05-06 09:55:03.000000 pyslth-0.4.9/slth/oauth.py
+-rw-r--r--   0 breno      (501) staff       (20)     1906 2024-05-18 17:29:04.000000 pyslth-0.4.9/slth/permissions.py
+-rw-r--r--   0 breno      (501) staff       (20)    19965 2024-05-16 13:39:18.000000 pyslth-0.4.9/slth/queryset.py
+-rw-r--r--   0 breno      (501) staff       (20)     4724 2024-04-19 09:29:01.000000 pyslth-0.4.9/slth/roles.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-23 10:26:14.382911 pyslth-0.4.9/slth/selenium/
+-rw-r--r--   0 breno      (501) staff       (20)     9095 2024-04-28 09:44:40.000000 pyslth-0.4.9/slth/selenium/__init__.py
+-rw-r--r--   0 breno      (501) staff       (20)    11350 2024-04-30 08:48:10.000000 pyslth-0.4.9/slth/selenium/browser.py
+-rw-r--r--   0 breno      (501) staff       (20)    15969 2024-05-21 20:16:17.000000 pyslth-0.4.9/slth/serializer.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-23 10:26:14.383525 pyslth-0.4.9/slth/static/
+-rw-r--r--   0 breno      (501) staff       (20)     6148 2024-05-20 11:57:45.000000 pyslth-0.4.9/slth/static/.DS_Store
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-23 10:26:14.385508 pyslth-0.4.9/slth/static/css/
+-rw-r--r--   0 breno      (501) staff       (20)     6148 2024-04-29 19:56:09.000000 pyslth-0.4.9/slth/static/css/.DS_Store
+-rw-r--r--   0 breno      (501) staff       (20)    80823 2024-04-27 15:01:32.000000 pyslth-0.4.9/slth/static/css/fontawesome.min.css
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-23 10:26:14.389644 pyslth-0.4.9/slth/static/css/fonts/
+-rw-r--r--   0 breno      (501) staff       (20)     6148 2024-04-29 19:36:17.000000 pyslth-0.4.9/slth/static/css/fonts/.DS_Store
+-rw-r--r--   0 breno      (501) staff       (20)   150020 2024-04-27 15:01:32.000000 pyslth-0.4.9/slth/static/css/fonts/fa-solid-900.woff2
+-rw-r--r--   0 breno      (501) staff       (20)   115080 2024-04-29 19:28:27.000000 pyslth-0.4.9/slth/static/css/fonts/rawline-400.woff
+-rw-r--r--   0 breno      (501) staff       (20)   117252 2024-04-29 19:29:24.000000 pyslth-0.4.9/slth/static/css/fonts/rawline-500i.woff
+-rw-r--r--   0 breno      (501) staff       (20)   117076 2024-04-29 19:36:27.000000 pyslth-0.4.9/slth/static/css/fonts/rawline-700.woff
+-rw-r--r--   0 breno      (501) staff       (20)     1977 2024-05-12 18:54:58.000000 pyslth-0.4.9/slth/static/css/slth.css
+-rw-r--r--   0 breno      (501) staff       (20)      515 2024-04-27 15:44:29.000000 pyslth-0.4.9/slth/static/css/solid.min.css
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-05-07 11:57:26.000000 pyslth-0.4.9/slth/static/css/style.css
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-23 10:26:14.394937 pyslth-0.4.9/slth/static/images/
+-rw-r--r--   0 breno      (501) staff       (20)    10828 2024-04-15 11:56:33.000000 pyslth-0.4.9/slth/static/images/logo.png
+-rw-r--r--   0 breno      (501) staff       (20)     2432 2024-04-13 03:35:59.000000 pyslth-0.4.9/slth/static/images/logo.svg
+-rw-r--r--   0 breno      (501) staff       (20)    16754 2024-04-16 09:42:03.000000 pyslth-0.4.9/slth/static/images/user.png
+-rw-r--r--   0 breno      (501) staff       (20)      492 2024-05-07 12:51:28.000000 pyslth-0.4.9/slth/static/images/user.svg
+-rw-r--r--   0 breno      (501) staff       (20)        0 2024-04-27 17:47:02.000000 pyslth-0.4.9/slth/static/index.html
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-23 10:26:14.406088 pyslth-0.4.9/slth/static/js/
+-rw-r--r--   0 breno      (501) staff       (20)      946 2024-05-19 17:15:44.000000 pyslth-0.4.9/slth/static/js/default-passive-events.min.js
+-rw-r--r--   0 breno      (501) staff       (20)  1112413 2024-05-18 14:48:49.000000 pyslth-0.4.9/slth/static/js/echarts.min.js
+-rw-r--r--   0 breno      (501) staff       (20)      756 2024-05-23 10:25:35.000000 pyslth-0.4.9/slth/static/js/index.min.js
+-rw-r--r--   0 breno      (501) staff       (20)     1601 2024-05-02 09:27:38.000000 pyslth-0.4.9/slth/static/js/ios-splash.min.js
+-rw-r--r--   0 breno      (501) staff       (20)   117723 2024-05-08 16:11:56.000000 pyslth-0.4.9/slth/static/js/peerjs.min.js
+-rw-r--r--   0 breno      (501) staff       (20)    92865 2024-05-19 22:43:39.000000 pyslth-0.4.9/slth/static/js/peerjs154.min.js
+-rw-r--r--   0 breno      (501) staff       (20)    19927 2024-04-27 15:01:32.000000 pyslth-0.4.9/slth/static/js/qrcode.min.js
+-rw-r--r--   0 breno      (501) staff       (20)     6176 2024-04-27 15:01:32.000000 pyslth-0.4.9/slth/static/js/react-trigger-change.js
+-rw-r--r--   0 breno      (501) staff       (20)   141870 2024-05-23 10:25:35.000000 pyslth-0.4.9/slth/static/js/react.min.js
+-rw-r--r--   0 breno      (501) staff       (20)   102297 2024-05-23 10:25:35.000000 pyslth-0.4.9/slth/static/js/slth.min.js
+-rw-rw-r--   0 breno      (501) staff       (20)     7401 2024-04-27 15:01:32.000000 pyslth-0.4.9/slth/static/js/vanilla-masker.js
+-rw-r--r--   0 breno      (501) staff       (20)     5720 2024-04-27 15:01:32.000000 pyslth-0.4.9/slth/static/js/vanilla-masker.min.js
+-rw-r--r--   0 breno      (501) staff       (20)     6361 2024-05-16 13:05:44.000000 pyslth-0.4.9/slth/statistics.py
+drwxr-xr-x   0 breno      (501) staff       (20)        0 2024-05-23 10:26:14.406689 pyslth-0.4.9/slth/templates/
+-rw-r--r--   0 breno      (501) staff       (20)     3230 2024-05-19 22:46:51.000000 pyslth-0.4.9/slth/templates/index.html
+-rw-r--r--   0 breno      (501) staff       (20)     1456 2024-05-18 10:06:11.000000 pyslth-0.4.9/slth/templates/service-worker.js
+-rw-r--r--   0 breno      (501) staff       (20)     5528 2024-04-16 18:07:11.000000 pyslth-0.4.9/slth/tests.py
+-rw-r--r--   0 breno      (501) staff       (20)      797 2024-04-29 14:21:39.000000 pyslth-0.4.9/slth/urls.py
+-rw-r--r--   0 breno      (501) staff       (20)     1000 2024-05-13 01:26:42.000000 pyslth-0.4.9/slth/utils.py
+-rw-r--r--   0 breno      (501) staff       (20)     2572 2024-05-08 14:06:07.000000 pyslth-0.4.9/slth/views.py
```

### Comparing `pyslth-0.4.8/PKG-INFO` & `pyslth-0.4.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyslth
-Version: 0.4.8
+Version: 0.4.9
 Summary: API generator based on yml file
 Home-page: https://github.com/brenokcc
 Author: Breno Silva
 Author-email: brenokcc@yahoo.com.br
 License: BSD License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `pyslth-0.4.8/pyslth.egg-info/PKG-INFO` & `pyslth-0.4.9/pyslth.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyslth
-Version: 0.4.8
+Version: 0.4.9
 Summary: API generator based on yml file
 Home-page: https://github.com/brenokcc
 Author: Breno Silva
 Author-email: brenokcc@yahoo.com.br
 License: BSD License
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `pyslth-0.4.8/pyslth.egg-info/SOURCES.txt` & `pyslth-0.4.9/pyslth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.8/setup.py` & `pyslth-0.4.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 from setuptools import find_packages, setup
 
 install_requires = open('requirements.txt').read().splitlines()
 
 setup(
     name='pyslth',
-    version='0.4.8',
+    version='0.4.9',
     packages=find_packages(exclude=('xxx', 'xxx.*')),
     install_requires=install_requires,
     extras_require={
         'dev': []
     },
     include_package_data=True,
     license='BSD License',
```

### Comparing `pyslth-0.4.8/slth/__init__.py` & `pyslth-0.4.9/slth/__init__.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.8/slth/components.py` & `pyslth-0.4.9/slth/components.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.8/slth/db/models.py` & `pyslth-0.4.9/slth/db/models.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.8/slth/endpoints.py` & `pyslth-0.4.9/slth/endpoints.py`

 * *Files 0% similar despite different names*

```diff
@@ -433,15 +433,15 @@
 
     def post(self):
         self.get_instance().delete()
         return super().post()
 
 
 class Login(PublicEndpoint):
-    username = forms.CharField(label="Username")
+    username = forms.CharField(label="Username", mask=getattr(settings, 'USERNAME_MASK', None))
     password = forms.CharField(label="Senha")
 
     class Meta:
         modal = False
         icon = "sign-in"
         verbose_name = "Login"
```

### Comparing `pyslth-0.4.8/slth/factory.py` & `pyslth-0.4.9/slth/factory.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.8/slth/forms.py` & `pyslth-0.4.9/slth/forms.py`

 * *Files 0% similar despite different names*

```diff
@@ -644,14 +644,23 @@
             self.width = width or height
             self.height = height or width
         else:
             self.width = self.height = 500
         super().__init__(*args, **kwargs)
 
 
+class CharField(CharField):
+
+    def __init__(self, *args, **kwargs):
+        self.mask = kwargs.pop("mask", None)
+        super().__init__(*args, **kwargs)
+
+    
+
+
 class ChoiceField(ChoiceField):
 
     def __init__(self, *args, **kwargs):
         self.pick = kwargs.pop("pick", False)
         super().__init__(*args, **kwargs)
```

### Comparing `pyslth-0.4.8/slth/management/commands/integration_test.py` & `pyslth-0.4.9/slth/management/commands/integration_test.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.8/slth/management/commands/sync.py` & `pyslth-0.4.9/slth/management/commands/sync.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.8/slth/migrations/0001_initial.py` & `pyslth-0.4.9/slth/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.8/slth/migrations/0002_email_role_pushsubscription_error.py` & `pyslth-0.4.9/slth/migrations/0002_email_role_pushsubscription_error.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.8/slth/migrations/0003_rename_photo_profile_alter_profile_options.py` & `pyslth-0.4.9/slth/migrations/0003_rename_photo_profile_alter_profile_options.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.8/slth/migrations/0006_user.py` & `pyslth-0.4.9/slth/migrations/0006_user.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.8/slth/models.py` & `pyslth-0.4.9/slth/models.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.8/slth/notifications.py` & `pyslth-0.4.9/slth/notifications.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.8/slth/oauth.py` & `pyslth-0.4.9/slth/oauth.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.8/slth/permissions.py` & `pyslth-0.4.9/slth/permissions.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.8/slth/queryset.py` & `pyslth-0.4.9/slth/queryset.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.8/slth/roles.py` & `pyslth-0.4.9/slth/roles.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.8/slth/selenium/__init__.py` & `pyslth-0.4.9/slth/selenium/__init__.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.8/slth/selenium/browser.py` & `pyslth-0.4.9/slth/selenium/browser.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.8/slth/serializer.py` & `pyslth-0.4.9/slth/serializer.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.8/slth/static/.DS_Store` & `pyslth-0.4.9/slth/static/.DS_Store`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.8/slth/static/css/.DS_Store` & `pyslth-0.4.9/slth/static/css/.DS_Store`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.8/slth/static/css/fontawesome.min.css` & `pyslth-0.4.9/slth/static/css/fontawesome.min.css`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.8/slth/static/css/fonts/.DS_Store` & `pyslth-0.4.9/slth/static/css/fonts/.DS_Store`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.8/slth/static/css/fonts/fa-solid-900.woff2` & `pyslth-0.4.9/slth/static/css/fonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.8/slth/static/css/fonts/rawline-400.woff` & `pyslth-0.4.9/slth/static/css/fonts/rawline-400.woff`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.8/slth/static/css/fonts/rawline-500i.woff` & `pyslth-0.4.9/slth/static/css/fonts/rawline-500i.woff`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.8/slth/static/css/fonts/rawline-700.woff` & `pyslth-0.4.9/slth/static/css/fonts/rawline-700.woff`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.8/slth/static/css/slth.css` & `pyslth-0.4.9/slth/static/css/slth.css`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.8/slth/static/css/solid.min.css` & `pyslth-0.4.9/slth/static/css/solid.min.css`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.8/slth/static/images/logo.png` & `pyslth-0.4.9/slth/static/images/logo.png`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.8/slth/static/images/logo.svg` & `pyslth-0.4.9/slth/static/images/logo.svg`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.8/slth/static/images/user.png` & `pyslth-0.4.9/slth/static/images/user.png`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.8/slth/static/js/default-passive-events.min.js` & `pyslth-0.4.9/slth/static/js/default-passive-events.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.8/slth/static/js/echarts.min.js` & `pyslth-0.4.9/slth/static/js/echarts.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.8/slth/static/js/index.min.js` & `pyslth-0.4.9/slth/static/js/index.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.8/slth/static/js/ios-splash.min.js` & `pyslth-0.4.9/slth/static/js/ios-splash.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.8/slth/static/js/peerjs.min.js` & `pyslth-0.4.9/slth/static/js/peerjs.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.8/slth/static/js/peerjs154.min.js` & `pyslth-0.4.9/slth/static/js/peerjs154.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.8/slth/static/js/qrcode.min.js` & `pyslth-0.4.9/slth/static/js/qrcode.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.8/slth/static/js/react-trigger-change.js` & `pyslth-0.4.9/slth/static/js/react-trigger-change.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.8/slth/static/js/react.min.js` & `pyslth-0.4.9/slth/static/js/react.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.8/slth/static/js/slth.min.js` & `pyslth-0.4.9/slth/static/js/slth.min.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1475,15 +1475,16 @@
             width: "fit-content",
             borderRadius: 0,
             textWrap: "nowrap",
             padding: 10,
             whiteSpace: "nowrap",
             backgroundColor: e.data.color,
             display: "inline-flex",
-            border: "solid 3px white"
+            border: "solid 3px white",
+            lineHeight: "1rem"
         };
         return t.jsxs("div", {
             style: a,
             children: [e.data.icon && t.jsx(S, {
                 icon: e.data.icon,
                 style: {
                     marginRight: 5
```

### Comparing `pyslth-0.4.8/slth/static/js/vanilla-masker.js` & `pyslth-0.4.9/slth/static/js/vanilla-masker.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.8/slth/static/js/vanilla-masker.min.js` & `pyslth-0.4.9/slth/static/js/vanilla-masker.min.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.8/slth/statistics.py` & `pyslth-0.4.9/slth/statistics.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.8/slth/templates/index.html` & `pyslth-0.4.9/slth/templates/index.html`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.8/slth/templates/service-worker.js` & `pyslth-0.4.9/slth/templates/service-worker.js`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.8/slth/tests.py` & `pyslth-0.4.9/slth/tests.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.8/slth/urls.py` & `pyslth-0.4.9/slth/urls.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.8/slth/utils.py` & `pyslth-0.4.9/slth/utils.py`

 * *Files identical despite different names*

### Comparing `pyslth-0.4.8/slth/views.py` & `pyslth-0.4.9/slth/views.py`

 * *Files identical despite different names*

