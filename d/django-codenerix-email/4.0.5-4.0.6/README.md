# Comparing `tmp/django-codenerix-email-4.0.5.tar.gz` & `tmp/django-codenerix-email-4.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-codenerix-email-4.0.5.tar", last modified: Wed May 22 12:44:54 2024, max compression
+gzip compressed data, was "django-codenerix-email-4.0.6.tar", last modified: Wed May 22 13:01:40 2024, max compression
```

## Comparing `django-codenerix-email-4.0.5.tar` & `django-codenerix-email-4.0.6.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-05-22 12:44:54.978218 django-codenerix-email-4.0.5/
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)    11339 2024-03-27 07:06:52.000000 django-codenerix-email-4.0.5/LICENSE
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      247 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.5/MANIFEST.in
--rw-rw-r--   0 br0th3r   (1001) br0th3r   (1001)     2543 2024-05-22 12:44:54.974218 django-codenerix-email-4.0.5/PKG-INFO
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1344 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.5/README.rst
-drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-05-22 12:44:54.966218 django-codenerix-email-4.0.5/codenerix_email/
--rw-rw-r--   0 br0th3r   (1001) br0th3r   (1001)      148 2024-05-22 12:44:54.000000 django-codenerix-email-4.0.5/codenerix_email/__init__.py
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1208 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.5/codenerix_email/admin.py
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      149 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.5/codenerix_email/apps.py
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     3706 2024-05-22 12:29:39.000000 django-codenerix-email-4.0.5/codenerix_email/forms.py
-drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-05-22 12:44:54.966218 django-codenerix-email-4.0.5/codenerix_email/management/
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)        0 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.5/codenerix_email/management/__init__.py
-drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-05-22 12:44:54.970219 django-codenerix-email-4.0.5/codenerix_email/management/__pycache__/
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      179 2023-10-27 11:25:38.000000 django-codenerix-email-4.0.5/codenerix_email/management/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      195 2024-02-26 06:56:17.000000 django-codenerix-email-4.0.5/codenerix_email/management/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      160 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.5/codenerix_email/management/__pycache__/__init__.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      168 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.5/codenerix_email/management/__pycache__/__init__.cpython-39.pyc
-drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-05-22 12:44:54.970219 django-codenerix-email-4.0.5/codenerix_email/management/commands/
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)        0 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.5/codenerix_email/management/commands/__init__.py
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     6290 2024-04-09 05:53:51.000000 django-codenerix-email-4.0.5/codenerix_email/management/commands/send_emails.py
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1655 2024-04-09 05:53:42.000000 django-codenerix-email-4.0.5/codenerix_email/management/commands/test_email.py
-drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-05-22 12:44:54.970219 django-codenerix-email-4.0.5/codenerix_email/migrations/
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     3511 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.5/codenerix_email/migrations/0001_initial.py
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     2369 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.5/codenerix_email/migrations/0002_auto_20170502_1043.py
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      656 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.5/codenerix_email/migrations/0003_auto_20170921_1206.py
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      486 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.5/codenerix_email/migrations/0004_auto_20171108_1628.py
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      495 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.5/codenerix_email/migrations/0005_emailmessage_retries.py
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      489 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.5/codenerix_email/migrations/0006_emailmessage_error.py
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      602 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.5/codenerix_email/migrations/0007_emailmessage_next_retry.py
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      731 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.5/codenerix_email/migrations/0008_auto_20171201_0928.py
--rw-rw-r--   0 br0th3r   (1001) br0th3r   (1001)     1219 2024-05-22 11:42:23.000000 django-codenerix-email-4.0.5/codenerix_email/migrations/0009_emailmessage_opened_emailmessage_uuid.py
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)        0 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.5/codenerix_email/migrations/__init__.py
-drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-05-22 12:44:54.974218 django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     2005 2023-01-29 13:03:07.000000 django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0001_initial.cpython-310.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     3682 2024-02-14 12:11:39.000000 django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0001_initial.cpython-311.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     2373 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0001_initial.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     2020 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0001_initial.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1500 2023-01-29 13:03:07.000000 django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0002_auto_20170502_1043.cpython-310.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     2664 2024-02-14 12:11:39.000000 django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0002_auto_20170502_1043.cpython-311.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1692 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0002_auto_20170502_1043.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1515 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0002_auto_20170502_1043.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      694 2023-01-29 13:03:07.000000 django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0003_auto_20170921_1206.cpython-310.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      967 2024-02-14 12:11:39.000000 django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0003_auto_20170921_1206.cpython-311.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      782 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0003_auto_20170921_1206.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      709 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0003_auto_20170921_1206.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      676 2023-01-29 13:03:07.000000 django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0004_auto_20171108_1628.cpython-310.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      939 2024-02-14 12:11:39.000000 django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0004_auto_20171108_1628.cpython-311.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      713 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0004_auto_20171108_1628.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      691 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0004_auto_20171108_1628.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      691 2023-01-29 13:03:07.000000 django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0005_emailmessage_retries.cpython-310.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      954 2024-02-14 12:11:39.000000 django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0005_emailmessage_retries.cpython-311.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      728 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0005_emailmessage_retries.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      706 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0005_emailmessage_retries.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      675 2023-01-29 13:03:07.000000 django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0006_emailmessage_error.cpython-310.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      938 2024-02-14 12:11:39.000000 django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0006_emailmessage_error.cpython-311.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      712 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0006_emailmessage_error.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      690 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0006_emailmessage_error.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      802 2023-01-29 13:03:07.000000 django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0007_emailmessage_next_retry.cpython-310.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1111 2024-02-14 12:11:39.000000 django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0007_emailmessage_next_retry.cpython-311.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      854 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0007_emailmessage_next_retry.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      817 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0007_emailmessage_next_retry.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      779 2023-01-29 13:03:07.000000 django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0008_auto_20171201_0928.cpython-310.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1178 2024-02-14 12:11:39.000000 django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0008_auto_20171201_0928.cpython-311.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      839 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0008_auto_20171201_0928.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      794 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0008_auto_20171201_0928.cpython-39.pyc
--rw-rw-r--   0 br0th3r   (1001) br0th3r   (1001)      733 2024-05-21 07:57:54.000000 django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0009_delete_emailtemplatetexten.cpython-311.pyc
--rw-rw-r--   0 br0th3r   (1001) br0th3r   (1001)     1860 2024-05-22 11:44:13.000000 django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0009_emailmessage_opened_emailmessage_uuid.cpython-311.pyc
--rw-rw-r--   0 br0th3r   (1001) br0th3r   (1001)     3104 2024-05-22 11:40:40.000000 django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0010_emailmessage_opened_emailmessage_uuid_and_more.cpython-311.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      151 2023-01-29 13:03:07.000000 django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      195 2024-02-14 12:11:39.000000 django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      147 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/__init__.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      168 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)    13201 2024-05-22 12:41:41.000000 django-codenerix-email-4.0.5/codenerix_email/models.py
-drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-05-22 12:44:54.966218 django-codenerix-email-4.0.5/codenerix_email/static/
-drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-05-22 12:44:54.966218 django-codenerix-email-4.0.5/codenerix_email/static/codenerix_email/
-drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-05-22 12:44:54.974218 django-codenerix-email-4.0.5/codenerix_email/static/codenerix_email/partials/
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1060 2024-05-22 11:47:17.000000 django-codenerix-email-4.0.5/codenerix_email/static/codenerix_email/partials/emailmessages_rows.html
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     2595 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.5/codenerix_email/urls.py
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      873 2024-05-22 12:21:01.000000 django-codenerix-email-4.0.5/codenerix_email/urls_frontend.py
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     4820 2024-05-22 12:38:27.000000 django-codenerix-email-4.0.5/codenerix_email/views.py
-drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-05-22 12:44:54.974218 django-codenerix-email-4.0.5/django_codenerix_email.egg-info/
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     2543 2024-05-22 12:44:54.000000 django-codenerix-email-4.0.5/django_codenerix_email.egg-info/PKG-INFO
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     4619 2024-05-22 12:44:54.000000 django-codenerix-email-4.0.5/django_codenerix_email.egg-info/SOURCES.txt
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)        1 2024-05-22 12:44:54.000000 django-codenerix-email-4.0.5/django_codenerix_email.egg-info/dependency_links.txt
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)        1 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.5/django_codenerix_email.egg-info/not-zip-safe
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)       53 2024-05-22 12:44:54.000000 django-codenerix-email-4.0.5/django_codenerix_email.egg-info/requires.txt
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)       16 2024-05-22 12:44:54.000000 django-codenerix-email-4.0.5/django_codenerix_email.egg-info/top_level.txt
--rw-rw-r--   0 br0th3r   (1001) br0th3r   (1001)       38 2024-05-22 12:44:54.978218 django-codenerix-email-4.0.5/setup.cfg
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1707 2024-04-08 11:04:22.000000 django-codenerix-email-4.0.5/setup.py
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-05-22 13:01:40.732239 django-codenerix-email-4.0.6/
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)    11339 2024-03-27 07:06:52.000000 django-codenerix-email-4.0.6/LICENSE
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      247 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.6/MANIFEST.in
+-rw-rw-r--   0 br0th3r   (1001) br0th3r   (1001)     2543 2024-05-22 13:01:40.732239 django-codenerix-email-4.0.6/PKG-INFO
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1344 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.6/README.rst
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-05-22 13:01:40.728239 django-codenerix-email-4.0.6/codenerix_email/
+-rw-rw-r--   0 br0th3r   (1001) br0th3r   (1001)      148 2024-05-22 13:01:40.000000 django-codenerix-email-4.0.6/codenerix_email/__init__.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1208 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.6/codenerix_email/admin.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      149 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.6/codenerix_email/apps.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     3706 2024-05-22 12:29:39.000000 django-codenerix-email-4.0.6/codenerix_email/forms.py
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-05-22 13:01:40.728239 django-codenerix-email-4.0.6/codenerix_email/management/
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)        0 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.6/codenerix_email/management/__init__.py
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-05-22 13:01:40.728239 django-codenerix-email-4.0.6/codenerix_email/management/__pycache__/
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      179 2023-10-27 11:25:38.000000 django-codenerix-email-4.0.6/codenerix_email/management/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      195 2024-02-26 06:56:17.000000 django-codenerix-email-4.0.6/codenerix_email/management/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      160 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.6/codenerix_email/management/__pycache__/__init__.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      168 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.6/codenerix_email/management/__pycache__/__init__.cpython-39.pyc
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-05-22 13:01:40.728239 django-codenerix-email-4.0.6/codenerix_email/management/commands/
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)        0 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.6/codenerix_email/management/commands/__init__.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     6290 2024-04-09 05:53:51.000000 django-codenerix-email-4.0.6/codenerix_email/management/commands/send_emails.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1655 2024-04-09 05:53:42.000000 django-codenerix-email-4.0.6/codenerix_email/management/commands/test_email.py
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-05-22 13:01:40.728239 django-codenerix-email-4.0.6/codenerix_email/migrations/
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     3511 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.6/codenerix_email/migrations/0001_initial.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     2369 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.6/codenerix_email/migrations/0002_auto_20170502_1043.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      656 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.6/codenerix_email/migrations/0003_auto_20170921_1206.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      486 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.6/codenerix_email/migrations/0004_auto_20171108_1628.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      495 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.6/codenerix_email/migrations/0005_emailmessage_retries.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      489 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.6/codenerix_email/migrations/0006_emailmessage_error.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      602 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.6/codenerix_email/migrations/0007_emailmessage_next_retry.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      731 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.6/codenerix_email/migrations/0008_auto_20171201_0928.py
+-rw-rw-r--   0 br0th3r   (1001) br0th3r   (1001)     1219 2024-05-22 11:42:23.000000 django-codenerix-email-4.0.6/codenerix_email/migrations/0009_emailmessage_opened_emailmessage_uuid.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)        0 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.6/codenerix_email/migrations/__init__.py
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-05-22 13:01:40.728239 django-codenerix-email-4.0.6/codenerix_email/migrations/__pycache__/
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     2005 2023-01-29 13:03:07.000000 django-codenerix-email-4.0.6/codenerix_email/migrations/__pycache__/0001_initial.cpython-310.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     3682 2024-02-14 12:11:39.000000 django-codenerix-email-4.0.6/codenerix_email/migrations/__pycache__/0001_initial.cpython-311.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     2373 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.6/codenerix_email/migrations/__pycache__/0001_initial.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     2020 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.6/codenerix_email/migrations/__pycache__/0001_initial.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1500 2023-01-29 13:03:07.000000 django-codenerix-email-4.0.6/codenerix_email/migrations/__pycache__/0002_auto_20170502_1043.cpython-310.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     2664 2024-02-14 12:11:39.000000 django-codenerix-email-4.0.6/codenerix_email/migrations/__pycache__/0002_auto_20170502_1043.cpython-311.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1692 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.6/codenerix_email/migrations/__pycache__/0002_auto_20170502_1043.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1515 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.6/codenerix_email/migrations/__pycache__/0002_auto_20170502_1043.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      694 2023-01-29 13:03:07.000000 django-codenerix-email-4.0.6/codenerix_email/migrations/__pycache__/0003_auto_20170921_1206.cpython-310.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      967 2024-02-14 12:11:39.000000 django-codenerix-email-4.0.6/codenerix_email/migrations/__pycache__/0003_auto_20170921_1206.cpython-311.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      782 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.6/codenerix_email/migrations/__pycache__/0003_auto_20170921_1206.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      709 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.6/codenerix_email/migrations/__pycache__/0003_auto_20170921_1206.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      676 2023-01-29 13:03:07.000000 django-codenerix-email-4.0.6/codenerix_email/migrations/__pycache__/0004_auto_20171108_1628.cpython-310.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      939 2024-02-14 12:11:39.000000 django-codenerix-email-4.0.6/codenerix_email/migrations/__pycache__/0004_auto_20171108_1628.cpython-311.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      713 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.6/codenerix_email/migrations/__pycache__/0004_auto_20171108_1628.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      691 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.6/codenerix_email/migrations/__pycache__/0004_auto_20171108_1628.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      691 2023-01-29 13:03:07.000000 django-codenerix-email-4.0.6/codenerix_email/migrations/__pycache__/0005_emailmessage_retries.cpython-310.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      954 2024-02-14 12:11:39.000000 django-codenerix-email-4.0.6/codenerix_email/migrations/__pycache__/0005_emailmessage_retries.cpython-311.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      728 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.6/codenerix_email/migrations/__pycache__/0005_emailmessage_retries.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      706 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.6/codenerix_email/migrations/__pycache__/0005_emailmessage_retries.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      675 2023-01-29 13:03:07.000000 django-codenerix-email-4.0.6/codenerix_email/migrations/__pycache__/0006_emailmessage_error.cpython-310.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      938 2024-02-14 12:11:39.000000 django-codenerix-email-4.0.6/codenerix_email/migrations/__pycache__/0006_emailmessage_error.cpython-311.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      712 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.6/codenerix_email/migrations/__pycache__/0006_emailmessage_error.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      690 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.6/codenerix_email/migrations/__pycache__/0006_emailmessage_error.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      802 2023-01-29 13:03:07.000000 django-codenerix-email-4.0.6/codenerix_email/migrations/__pycache__/0007_emailmessage_next_retry.cpython-310.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1111 2024-02-14 12:11:39.000000 django-codenerix-email-4.0.6/codenerix_email/migrations/__pycache__/0007_emailmessage_next_retry.cpython-311.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      854 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.6/codenerix_email/migrations/__pycache__/0007_emailmessage_next_retry.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      817 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.6/codenerix_email/migrations/__pycache__/0007_emailmessage_next_retry.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      779 2023-01-29 13:03:07.000000 django-codenerix-email-4.0.6/codenerix_email/migrations/__pycache__/0008_auto_20171201_0928.cpython-310.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1178 2024-02-14 12:11:39.000000 django-codenerix-email-4.0.6/codenerix_email/migrations/__pycache__/0008_auto_20171201_0928.cpython-311.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      839 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.6/codenerix_email/migrations/__pycache__/0008_auto_20171201_0928.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      794 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.6/codenerix_email/migrations/__pycache__/0008_auto_20171201_0928.cpython-39.pyc
+-rw-rw-r--   0 br0th3r   (1001) br0th3r   (1001)      733 2024-05-21 07:57:54.000000 django-codenerix-email-4.0.6/codenerix_email/migrations/__pycache__/0009_delete_emailtemplatetexten.cpython-311.pyc
+-rw-rw-r--   0 br0th3r   (1001) br0th3r   (1001)     1860 2024-05-22 11:44:13.000000 django-codenerix-email-4.0.6/codenerix_email/migrations/__pycache__/0009_emailmessage_opened_emailmessage_uuid.cpython-311.pyc
+-rw-rw-r--   0 br0th3r   (1001) br0th3r   (1001)     3104 2024-05-22 11:40:40.000000 django-codenerix-email-4.0.6/codenerix_email/migrations/__pycache__/0010_emailmessage_opened_emailmessage_uuid_and_more.cpython-311.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      151 2023-01-29 13:03:07.000000 django-codenerix-email-4.0.6/codenerix_email/migrations/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      195 2024-02-14 12:11:39.000000 django-codenerix-email-4.0.6/codenerix_email/migrations/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      147 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.6/codenerix_email/migrations/__pycache__/__init__.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      168 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.6/codenerix_email/migrations/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)    13244 2024-05-22 12:59:57.000000 django-codenerix-email-4.0.6/codenerix_email/models.py
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-05-22 13:01:40.724239 django-codenerix-email-4.0.6/codenerix_email/static/
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-05-22 13:01:40.724239 django-codenerix-email-4.0.6/codenerix_email/static/codenerix_email/
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-05-22 13:01:40.728239 django-codenerix-email-4.0.6/codenerix_email/static/codenerix_email/partials/
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1060 2024-05-22 11:47:17.000000 django-codenerix-email-4.0.6/codenerix_email/static/codenerix_email/partials/emailmessages_rows.html
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     2595 2022-08-14 19:56:23.000000 django-codenerix-email-4.0.6/codenerix_email/urls.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      873 2024-05-22 12:21:01.000000 django-codenerix-email-4.0.6/codenerix_email/urls_frontend.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     4820 2024-05-22 12:38:27.000000 django-codenerix-email-4.0.6/codenerix_email/views.py
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-05-22 13:01:40.732239 django-codenerix-email-4.0.6/django_codenerix_email.egg-info/
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     2543 2024-05-22 13:01:40.000000 django-codenerix-email-4.0.6/django_codenerix_email.egg-info/PKG-INFO
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     4619 2024-05-22 13:01:40.000000 django-codenerix-email-4.0.6/django_codenerix_email.egg-info/SOURCES.txt
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)        1 2024-05-22 13:01:40.000000 django-codenerix-email-4.0.6/django_codenerix_email.egg-info/dependency_links.txt
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)        1 2020-05-15 23:36:43.000000 django-codenerix-email-4.0.6/django_codenerix_email.egg-info/not-zip-safe
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)       53 2024-05-22 13:01:40.000000 django-codenerix-email-4.0.6/django_codenerix_email.egg-info/requires.txt
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)       16 2024-05-22 13:01:40.000000 django-codenerix-email-4.0.6/django_codenerix_email.egg-info/top_level.txt
+-rw-rw-r--   0 br0th3r   (1001) br0th3r   (1001)       38 2024-05-22 13:01:40.732239 django-codenerix-email-4.0.6/setup.cfg
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1707 2024-04-08 11:04:22.000000 django-codenerix-email-4.0.6/setup.py
```

### Comparing `django-codenerix-email-4.0.5/LICENSE` & `django-codenerix-email-4.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.5/PKG-INFO` & `django-codenerix-email-4.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-codenerix-email
-Version: 4.0.5
+Version: 4.0.6
 Summary: Codenerix Email is a module that enables CODENERIX to set send emails in a general manner.
 Home-page: https://github.com/codenerix/django-codenerix-email
 Author: Juan Miguel Taboada Godoy <juanmi@juanmitaboada.com>, Juan Soler Ruiz <soleronline@gmail.com>
 License: Apache License Version 2.0
 Keywords: django,codenerix,management,erp,crm,send email
 Platform: OS Independent
 Classifier: Environment :: Web Environment
```

### Comparing `django-codenerix-email-4.0.5/README.rst` & `django-codenerix-email-4.0.6/README.rst`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.5/codenerix_email/admin.py` & `django-codenerix-email-4.0.6/codenerix_email/admin.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.5/codenerix_email/forms.py` & `django-codenerix-email-4.0.6/codenerix_email/forms.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.5/codenerix_email/management/commands/send_emails.py` & `django-codenerix-email-4.0.6/codenerix_email/management/commands/send_emails.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.5/codenerix_email/management/commands/test_email.py` & `django-codenerix-email-4.0.6/codenerix_email/management/commands/test_email.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.5/codenerix_email/migrations/0001_initial.py` & `django-codenerix-email-4.0.6/codenerix_email/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.5/codenerix_email/migrations/0002_auto_20170502_1043.py` & `django-codenerix-email-4.0.6/codenerix_email/migrations/0002_auto_20170502_1043.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.5/codenerix_email/migrations/0003_auto_20170921_1206.py` & `django-codenerix-email-4.0.6/codenerix_email/migrations/0003_auto_20170921_1206.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.5/codenerix_email/migrations/0007_emailmessage_next_retry.py` & `django-codenerix-email-4.0.6/codenerix_email/migrations/0007_emailmessage_next_retry.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.5/codenerix_email/migrations/0008_auto_20171201_0928.py` & `django-codenerix-email-4.0.6/codenerix_email/migrations/0008_auto_20171201_0928.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.5/codenerix_email/migrations/0009_emailmessage_opened_emailmessage_uuid.py` & `django-codenerix-email-4.0.6/codenerix_email/migrations/0009_emailmessage_opened_emailmessage_uuid.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0001_initial.cpython-310.pyc` & `django-codenerix-email-4.0.6/codenerix_email/migrations/__pycache__/0001_initial.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0001_initial.cpython-311.pyc` & `django-codenerix-email-4.0.6/codenerix_email/migrations/__pycache__/0001_initial.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0001_initial.cpython-35.pyc` & `django-codenerix-email-4.0.6/codenerix_email/migrations/__pycache__/0001_initial.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0001_initial.cpython-39.pyc` & `django-codenerix-email-4.0.6/codenerix_email/migrations/__pycache__/0001_initial.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0002_auto_20170502_1043.cpython-310.pyc` & `django-codenerix-email-4.0.6/codenerix_email/migrations/__pycache__/0002_auto_20170502_1043.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0002_auto_20170502_1043.cpython-311.pyc` & `django-codenerix-email-4.0.6/codenerix_email/migrations/__pycache__/0002_auto_20170502_1043.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0002_auto_20170502_1043.cpython-35.pyc` & `django-codenerix-email-4.0.6/codenerix_email/migrations/__pycache__/0002_auto_20170502_1043.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0002_auto_20170502_1043.cpython-39.pyc` & `django-codenerix-email-4.0.6/codenerix_email/migrations/__pycache__/0002_auto_20170502_1043.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0003_auto_20170921_1206.cpython-310.pyc` & `django-codenerix-email-4.0.6/codenerix_email/migrations/__pycache__/0003_auto_20170921_1206.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0003_auto_20170921_1206.cpython-311.pyc` & `django-codenerix-email-4.0.6/codenerix_email/migrations/__pycache__/0003_auto_20170921_1206.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0003_auto_20170921_1206.cpython-35.pyc` & `django-codenerix-email-4.0.6/codenerix_email/migrations/__pycache__/0003_auto_20170921_1206.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0003_auto_20170921_1206.cpython-39.pyc` & `django-codenerix-email-4.0.6/codenerix_email/migrations/__pycache__/0003_auto_20170921_1206.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0004_auto_20171108_1628.cpython-310.pyc` & `django-codenerix-email-4.0.6/codenerix_email/migrations/__pycache__/0004_auto_20171108_1628.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0004_auto_20171108_1628.cpython-311.pyc` & `django-codenerix-email-4.0.6/codenerix_email/migrations/__pycache__/0004_auto_20171108_1628.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0004_auto_20171108_1628.cpython-35.pyc` & `django-codenerix-email-4.0.6/codenerix_email/migrations/__pycache__/0004_auto_20171108_1628.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0004_auto_20171108_1628.cpython-39.pyc` & `django-codenerix-email-4.0.6/codenerix_email/migrations/__pycache__/0004_auto_20171108_1628.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0005_emailmessage_retries.cpython-310.pyc` & `django-codenerix-email-4.0.6/codenerix_email/migrations/__pycache__/0005_emailmessage_retries.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0005_emailmessage_retries.cpython-311.pyc` & `django-codenerix-email-4.0.6/codenerix_email/migrations/__pycache__/0005_emailmessage_retries.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0005_emailmessage_retries.cpython-35.pyc` & `django-codenerix-email-4.0.6/codenerix_email/migrations/__pycache__/0005_emailmessage_retries.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0005_emailmessage_retries.cpython-39.pyc` & `django-codenerix-email-4.0.6/codenerix_email/migrations/__pycache__/0005_emailmessage_retries.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0006_emailmessage_error.cpython-310.pyc` & `django-codenerix-email-4.0.6/codenerix_email/migrations/__pycache__/0006_emailmessage_error.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0006_emailmessage_error.cpython-311.pyc` & `django-codenerix-email-4.0.6/codenerix_email/migrations/__pycache__/0006_emailmessage_error.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0006_emailmessage_error.cpython-35.pyc` & `django-codenerix-email-4.0.6/codenerix_email/migrations/__pycache__/0006_emailmessage_error.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0006_emailmessage_error.cpython-39.pyc` & `django-codenerix-email-4.0.6/codenerix_email/migrations/__pycache__/0006_emailmessage_error.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0007_emailmessage_next_retry.cpython-310.pyc` & `django-codenerix-email-4.0.6/codenerix_email/migrations/__pycache__/0007_emailmessage_next_retry.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0007_emailmessage_next_retry.cpython-311.pyc` & `django-codenerix-email-4.0.6/codenerix_email/migrations/__pycache__/0007_emailmessage_next_retry.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0007_emailmessage_next_retry.cpython-35.pyc` & `django-codenerix-email-4.0.6/codenerix_email/migrations/__pycache__/0007_emailmessage_next_retry.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0007_emailmessage_next_retry.cpython-39.pyc` & `django-codenerix-email-4.0.6/codenerix_email/migrations/__pycache__/0007_emailmessage_next_retry.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0008_auto_20171201_0928.cpython-310.pyc` & `django-codenerix-email-4.0.6/codenerix_email/migrations/__pycache__/0008_auto_20171201_0928.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0008_auto_20171201_0928.cpython-311.pyc` & `django-codenerix-email-4.0.6/codenerix_email/migrations/__pycache__/0008_auto_20171201_0928.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0008_auto_20171201_0928.cpython-35.pyc` & `django-codenerix-email-4.0.6/codenerix_email/migrations/__pycache__/0008_auto_20171201_0928.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0008_auto_20171201_0928.cpython-39.pyc` & `django-codenerix-email-4.0.6/codenerix_email/migrations/__pycache__/0008_auto_20171201_0928.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0009_delete_emailtemplatetexten.cpython-311.pyc` & `django-codenerix-email-4.0.6/codenerix_email/migrations/__pycache__/0009_delete_emailtemplatetexten.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0009_emailmessage_opened_emailmessage_uuid.cpython-311.pyc` & `django-codenerix-email-4.0.6/codenerix_email/migrations/__pycache__/0009_emailmessage_opened_emailmessage_uuid.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.5/codenerix_email/migrations/__pycache__/0010_emailmessage_opened_emailmessage_uuid_and_more.cpython-311.pyc` & `django-codenerix-email-4.0.6/codenerix_email/migrations/__pycache__/0010_emailmessage_opened_emailmessage_uuid_and_more.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.5/codenerix_email/models.py` & `django-codenerix-email-4.0.6/codenerix_email/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -326,14 +326,15 @@
             return None
 
     def get_email(self, context, lang=None):
         if lang is None:
             lang = settings.LANGUAGES_DATABASES[0].lower()
 
         e = EmailMessage()
+        context["__emsg__uuid__"] = e.uuid
         e.subject = Template(getattr(self, lang).subject).render(
             Context(context)
         )
         e.body = Template(getattr(self, lang).body).render(Context(context))
         e.efrom = Template(self.efrom).render(Context(context))
         return e
```

### Comparing `django-codenerix-email-4.0.5/codenerix_email/static/codenerix_email/partials/emailmessages_rows.html` & `django-codenerix-email-4.0.6/codenerix_email/static/codenerix_email/partials/emailmessages_rows.html`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.5/codenerix_email/urls.py` & `django-codenerix-email-4.0.6/codenerix_email/urls.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.5/codenerix_email/urls_frontend.py` & `django-codenerix-email-4.0.6/codenerix_email/urls_frontend.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.5/codenerix_email/views.py` & `django-codenerix-email-4.0.6/codenerix_email/views.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.5/django_codenerix_email.egg-info/PKG-INFO` & `django-codenerix-email-4.0.6/django_codenerix_email.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-codenerix-email
-Version: 4.0.5
+Version: 4.0.6
 Summary: Codenerix Email is a module that enables CODENERIX to set send emails in a general manner.
 Home-page: https://github.com/codenerix/django-codenerix-email
 Author: Juan Miguel Taboada Godoy <juanmi@juanmitaboada.com>, Juan Soler Ruiz <soleronline@gmail.com>
 License: Apache License Version 2.0
 Keywords: django,codenerix,management,erp,crm,send email
 Platform: OS Independent
 Classifier: Environment :: Web Environment
```

### Comparing `django-codenerix-email-4.0.5/django_codenerix_email.egg-info/SOURCES.txt` & `django-codenerix-email-4.0.6/django_codenerix_email.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-codenerix-email-4.0.5/setup.py` & `django-codenerix-email-4.0.6/setup.py`

 * *Files identical despite different names*

