# Comparing `tmp/django-codenerix-geodata-4.0.2.tar.gz` & `tmp/django-codenerix-geodata-4.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-codenerix-geodata-4.0.2.tar", last modified: Fri Oct 27 10:55:42 2023, max compression
+gzip compressed data, was "django-codenerix-geodata-4.0.3.tar", last modified: Thu May 23 04:46:39 2024, max compression
```

## Comparing `django-codenerix-geodata-4.0.2.tar` & `django-codenerix-geodata-4.0.3.tar`

### file list

```diff
@@ -1,62 +1,70 @@
-drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2023-10-27 10:55:42.301132 django-codenerix-geodata-4.0.2/
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)    11357 2020-05-15 23:36:44.000000 django-codenerix-geodata-4.0.2/LICENSE
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      341 2020-05-15 23:36:44.000000 django-codenerix-geodata-4.0.2/MANIFEST.in
--rw-rw-r--   0 br0th3r   (1001) br0th3r   (1001)     2988 2023-10-27 10:55:42.301132 django-codenerix-geodata-4.0.2/PKG-INFO
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1746 2022-08-14 19:56:50.000000 django-codenerix-geodata-4.0.2/README.rst
-drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2023-10-27 10:55:42.297132 django-codenerix-geodata-4.0.2/codenerix_geodata/
--rw-rw-r--   0 br0th3r   (1001) br0th3r   (1001)      148 2023-10-27 10:55:41.000000 django-codenerix-geodata-4.0.2/codenerix_geodata/__init__.py
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1253 2022-08-14 19:56:50.000000 django-codenerix-geodata-4.0.2/codenerix_geodata/admin.py
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      151 2022-08-14 19:56:50.000000 django-codenerix-geodata-4.0.2/codenerix_geodata/apps.py
-drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2023-10-27 10:55:42.301132 django-codenerix-geodata-4.0.2/codenerix_geodata/data/
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)   914881 2020-05-15 23:36:44.000000 django-codenerix-geodata-4.0.2/codenerix_geodata/data/GeoLite2-City-Locations-en.csv.bz2
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)   447419 2020-05-15 23:36:44.000000 django-codenerix-geodata-4.0.2/codenerix_geodata/data/GeoLite2-City-Locations-es.csv.bz2
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     3286 2020-05-15 23:36:44.000000 django-codenerix-geodata-4.0.2/codenerix_geodata/data/GeoLite2-Country-Locations-en.csv.bz2
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     3255 2020-05-15 23:36:44.000000 django-codenerix-geodata-4.0.2/codenerix_geodata/data/GeoLite2-Country-Locations-es.csv.bz2
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     3844 2023-10-27 10:03:15.000000 django-codenerix-geodata-4.0.2/codenerix_geodata/forms.py
-drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2023-10-27 10:55:42.301132 django-codenerix-geodata-4.0.2/codenerix_geodata/management/
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)        0 2020-05-15 23:36:44.000000 django-codenerix-geodata-4.0.2/codenerix_geodata/management/__init__.py
-drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2023-10-27 10:55:42.301132 django-codenerix-geodata-4.0.2/codenerix_geodata/management/__pycache__/
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      181 2022-11-26 23:27:10.000000 django-codenerix-geodata-4.0.2/codenerix_geodata/management/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      162 2020-05-15 23:36:44.000000 django-codenerix-geodata-4.0.2/codenerix_geodata/management/__pycache__/__init__.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      179 2022-11-27 21:58:10.000000 django-codenerix-geodata-4.0.2/codenerix_geodata/management/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      170 2022-08-14 19:56:50.000000 django-codenerix-geodata-4.0.2/codenerix_geodata/management/__pycache__/__init__.cpython-39.pyc
-drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2023-10-27 10:55:42.301132 django-codenerix-geodata-4.0.2/codenerix_geodata/management/commands/
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)        0 2020-05-15 23:36:44.000000 django-codenerix-geodata-4.0.2/codenerix_geodata/management/commands/__init__.py
-drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2023-10-27 10:55:42.301132 django-codenerix-geodata-4.0.2/codenerix_geodata/management/commands/__pycache__/
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      166 2020-05-15 23:36:44.000000 django-codenerix-geodata-4.0.2/codenerix_geodata/management/commands/__pycache__/__init__.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     8940 2020-05-15 23:36:44.000000 django-codenerix-geodata-4.0.2/codenerix_geodata/management/commands/__pycache__/populate_geodata.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)    19234 2022-08-14 19:56:50.000000 django-codenerix-geodata-4.0.2/codenerix_geodata/management/commands/populate_geodata.py
-drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2023-10-27 10:55:42.301132 django-codenerix-geodata-4.0.2/codenerix_geodata/migrations/
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)    12934 2020-05-15 23:36:44.000000 django-codenerix-geodata-4.0.2/codenerix_geodata/migrations/0001_initial.py
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     2047 2020-05-15 23:36:44.000000 django-codenerix-geodata-4.0.2/codenerix_geodata/migrations/0002_auto_20170921_1206.py
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      607 2020-05-15 23:36:44.000000 django-codenerix-geodata-4.0.2/codenerix_geodata/migrations/0003_auto_20180118_1209.py
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)        0 2020-05-15 23:36:44.000000 django-codenerix-geodata-4.0.2/codenerix_geodata/migrations/__init__.py
-drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2023-10-27 10:55:42.301132 django-codenerix-geodata-4.0.2/codenerix_geodata/migrations/__pycache__/
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     3885 2022-11-26 23:27:10.000000 django-codenerix-geodata-4.0.2/codenerix_geodata/migrations/__pycache__/0001_initial.cpython-310.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     5332 2020-05-15 23:36:44.000000 django-codenerix-geodata-4.0.2/codenerix_geodata/migrations/__pycache__/0001_initial.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     3901 2022-11-27 21:58:10.000000 django-codenerix-geodata-4.0.2/codenerix_geodata/migrations/__pycache__/0001_initial.cpython-38.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     3872 2022-08-14 19:56:50.000000 django-codenerix-geodata-4.0.2/codenerix_geodata/migrations/__pycache__/0001_initial.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1043 2022-11-26 23:27:10.000000 django-codenerix-geodata-4.0.2/codenerix_geodata/migrations/__pycache__/0002_auto_20170921_1206.cpython-310.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1391 2020-05-15 23:36:44.000000 django-codenerix-geodata-4.0.2/codenerix_geodata/migrations/__pycache__/0002_auto_20170921_1206.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1039 2022-11-27 21:58:10.000000 django-codenerix-geodata-4.0.2/codenerix_geodata/migrations/__pycache__/0002_auto_20170921_1206.cpython-38.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1030 2022-08-14 19:56:50.000000 django-codenerix-geodata-4.0.2/codenerix_geodata/migrations/__pycache__/0002_auto_20170921_1206.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      844 2022-11-26 23:27:10.000000 django-codenerix-geodata-4.0.2/codenerix_geodata/migrations/__pycache__/0003_auto_20180118_1209.cpython-310.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      869 2020-05-15 23:36:44.000000 django-codenerix-geodata-4.0.2/codenerix_geodata/migrations/__pycache__/0003_auto_20180118_1209.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      840 2022-11-27 21:58:10.000000 django-codenerix-geodata-4.0.2/codenerix_geodata/migrations/__pycache__/0003_auto_20180118_1209.cpython-38.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      831 2022-08-14 19:56:50.000000 django-codenerix-geodata-4.0.2/codenerix_geodata/migrations/__pycache__/0003_auto_20180118_1209.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      181 2022-11-26 23:27:10.000000 django-codenerix-geodata-4.0.2/codenerix_geodata/migrations/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      149 2020-05-15 23:36:44.000000 django-codenerix-geodata-4.0.2/codenerix_geodata/migrations/__pycache__/__init__.cpython-35.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      179 2022-11-27 21:58:10.000000 django-codenerix-geodata-4.0.2/codenerix_geodata/migrations/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      170 2022-08-14 19:56:50.000000 django-codenerix-geodata-4.0.2/codenerix_geodata/migrations/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     9378 2022-08-14 19:56:50.000000 django-codenerix-geodata-4.0.2/codenerix_geodata/models.py
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     7142 2022-08-14 19:56:50.000000 django-codenerix-geodata-4.0.2/codenerix_geodata/urls.py
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)    23882 2022-08-14 19:56:50.000000 django-codenerix-geodata-4.0.2/codenerix_geodata/views.py
-drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2023-10-27 10:55:42.301132 django-codenerix-geodata-4.0.2/django_codenerix_geodata.egg-info/
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     2988 2023-10-27 10:55:42.000000 django-codenerix-geodata-4.0.2/django_codenerix_geodata.egg-info/PKG-INFO
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     2698 2023-10-27 10:55:42.000000 django-codenerix-geodata-4.0.2/django_codenerix_geodata.egg-info/SOURCES.txt
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)        1 2023-10-27 10:55:42.000000 django-codenerix-geodata-4.0.2/django_codenerix_geodata.egg-info/dependency_links.txt
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)        1 2020-05-15 23:36:44.000000 django-codenerix-geodata-4.0.2/django_codenerix_geodata.egg-info/not-zip-safe
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)       45 2023-10-27 10:55:42.000000 django-codenerix-geodata-4.0.2/django_codenerix_geodata.egg-info/requires.txt
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)       18 2023-10-27 10:55:42.000000 django-codenerix-geodata-4.0.2/django_codenerix_geodata.egg-info/top_level.txt
--rw-rw-r--   0 br0th3r   (1001) br0th3r   (1001)       38 2023-10-27 10:55:42.301132 django-codenerix-geodata-4.0.2/setup.cfg
--rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1752 2020-05-15 23:36:44.000000 django-codenerix-geodata-4.0.2/setup.py
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-05-23 04:46:39.699121 django-codenerix-geodata-4.0.3/
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)    11339 2024-03-27 07:06:37.000000 django-codenerix-geodata-4.0.3/LICENSE
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      341 2020-05-15 23:36:44.000000 django-codenerix-geodata-4.0.3/MANIFEST.in
+-rw-rw-r--   0 br0th3r   (1001) br0th3r   (1001)     2988 2024-05-23 04:46:39.699121 django-codenerix-geodata-4.0.3/PKG-INFO
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1746 2022-08-14 19:56:50.000000 django-codenerix-geodata-4.0.3/README.rst
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-05-23 04:46:39.691121 django-codenerix-geodata-4.0.3/codenerix_geodata/
+-rw-rw-r--   0 br0th3r   (1001) br0th3r   (1001)      148 2024-05-23 04:46:39.000000 django-codenerix-geodata-4.0.3/codenerix_geodata/__init__.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1253 2022-08-14 19:56:50.000000 django-codenerix-geodata-4.0.3/codenerix_geodata/admin.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      151 2022-08-14 19:56:50.000000 django-codenerix-geodata-4.0.3/codenerix_geodata/apps.py
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-05-23 04:46:39.695121 django-codenerix-geodata-4.0.3/codenerix_geodata/data/
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)   914881 2020-05-15 23:36:44.000000 django-codenerix-geodata-4.0.3/codenerix_geodata/data/GeoLite2-City-Locations-en.csv.bz2
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)   447419 2020-05-15 23:36:44.000000 django-codenerix-geodata-4.0.3/codenerix_geodata/data/GeoLite2-City-Locations-es.csv.bz2
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     3286 2020-05-15 23:36:44.000000 django-codenerix-geodata-4.0.3/codenerix_geodata/data/GeoLite2-Country-Locations-en.csv.bz2
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     3255 2020-05-15 23:36:44.000000 django-codenerix-geodata-4.0.3/codenerix_geodata/data/GeoLite2-Country-Locations-es.csv.bz2
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     3844 2023-10-27 10:03:15.000000 django-codenerix-geodata-4.0.3/codenerix_geodata/forms.py
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-05-23 04:46:39.695121 django-codenerix-geodata-4.0.3/codenerix_geodata/management/
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)        0 2020-05-15 23:36:44.000000 django-codenerix-geodata-4.0.3/codenerix_geodata/management/__init__.py
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-05-23 04:46:39.695121 django-codenerix-geodata-4.0.3/codenerix_geodata/management/__pycache__/
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      181 2022-11-26 23:27:10.000000 django-codenerix-geodata-4.0.3/codenerix_geodata/management/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      197 2024-02-26 06:56:17.000000 django-codenerix-geodata-4.0.3/codenerix_geodata/management/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      162 2020-05-15 23:36:44.000000 django-codenerix-geodata-4.0.3/codenerix_geodata/management/__pycache__/__init__.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      179 2022-11-27 21:58:10.000000 django-codenerix-geodata-4.0.3/codenerix_geodata/management/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      170 2022-08-14 19:56:50.000000 django-codenerix-geodata-4.0.3/codenerix_geodata/management/__pycache__/__init__.cpython-39.pyc
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-05-23 04:46:39.695121 django-codenerix-geodata-4.0.3/codenerix_geodata/management/commands/
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)        0 2020-05-15 23:36:44.000000 django-codenerix-geodata-4.0.3/codenerix_geodata/management/commands/__init__.py
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-05-23 04:46:39.695121 django-codenerix-geodata-4.0.3/codenerix_geodata/management/commands/__pycache__/
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      213 2024-05-23 04:40:21.000000 django-codenerix-geodata-4.0.3/codenerix_geodata/management/commands/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      166 2020-05-15 23:36:44.000000 django-codenerix-geodata-4.0.3/codenerix_geodata/management/commands/__pycache__/__init__.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)    26235 2024-05-23 04:44:40.000000 django-codenerix-geodata-4.0.3/codenerix_geodata/management/commands/__pycache__/populate_geodata.cpython-311.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     8940 2020-05-15 23:36:44.000000 django-codenerix-geodata-4.0.3/codenerix_geodata/management/commands/__pycache__/populate_geodata.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)    21600 2024-05-23 04:44:31.000000 django-codenerix-geodata-4.0.3/codenerix_geodata/management/commands/populate_geodata.py
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-05-23 04:46:39.695121 django-codenerix-geodata-4.0.3/codenerix_geodata/migrations/
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)    12934 2020-05-15 23:36:44.000000 django-codenerix-geodata-4.0.3/codenerix_geodata/migrations/0001_initial.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     2047 2020-05-15 23:36:44.000000 django-codenerix-geodata-4.0.3/codenerix_geodata/migrations/0002_auto_20170921_1206.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      607 2020-05-15 23:36:44.000000 django-codenerix-geodata-4.0.3/codenerix_geodata/migrations/0003_auto_20180118_1209.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)        0 2020-05-15 23:36:44.000000 django-codenerix-geodata-4.0.3/codenerix_geodata/migrations/__init__.py
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-05-23 04:46:39.695121 django-codenerix-geodata-4.0.3/codenerix_geodata/migrations/__pycache__/
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     3885 2022-11-26 23:27:10.000000 django-codenerix-geodata-4.0.3/codenerix_geodata/migrations/__pycache__/0001_initial.cpython-310.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)    10143 2024-02-14 12:11:39.000000 django-codenerix-geodata-4.0.3/codenerix_geodata/migrations/__pycache__/0001_initial.cpython-311.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     5332 2020-05-15 23:36:44.000000 django-codenerix-geodata-4.0.3/codenerix_geodata/migrations/__pycache__/0001_initial.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     3901 2022-11-27 21:58:10.000000 django-codenerix-geodata-4.0.3/codenerix_geodata/migrations/__pycache__/0001_initial.cpython-38.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     3872 2022-08-14 19:56:50.000000 django-codenerix-geodata-4.0.3/codenerix_geodata/migrations/__pycache__/0001_initial.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1043 2022-11-26 23:27:10.000000 django-codenerix-geodata-4.0.3/codenerix_geodata/migrations/__pycache__/0002_auto_20170921_1206.cpython-310.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1697 2024-02-14 12:11:39.000000 django-codenerix-geodata-4.0.3/codenerix_geodata/migrations/__pycache__/0002_auto_20170921_1206.cpython-311.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1391 2020-05-15 23:36:44.000000 django-codenerix-geodata-4.0.3/codenerix_geodata/migrations/__pycache__/0002_auto_20170921_1206.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1039 2022-11-27 21:58:10.000000 django-codenerix-geodata-4.0.3/codenerix_geodata/migrations/__pycache__/0002_auto_20170921_1206.cpython-38.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1030 2022-08-14 19:56:50.000000 django-codenerix-geodata-4.0.3/codenerix_geodata/migrations/__pycache__/0002_auto_20170921_1206.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      844 2022-11-26 23:27:10.000000 django-codenerix-geodata-4.0.3/codenerix_geodata/migrations/__pycache__/0003_auto_20180118_1209.cpython-310.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1156 2024-02-14 12:11:39.000000 django-codenerix-geodata-4.0.3/codenerix_geodata/migrations/__pycache__/0003_auto_20180118_1209.cpython-311.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      869 2020-05-15 23:36:44.000000 django-codenerix-geodata-4.0.3/codenerix_geodata/migrations/__pycache__/0003_auto_20180118_1209.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      840 2022-11-27 21:58:10.000000 django-codenerix-geodata-4.0.3/codenerix_geodata/migrations/__pycache__/0003_auto_20180118_1209.cpython-38.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      831 2022-08-14 19:56:50.000000 django-codenerix-geodata-4.0.3/codenerix_geodata/migrations/__pycache__/0003_auto_20180118_1209.cpython-39.pyc
+-rw-rw-r--   0 br0th3r   (1001) br0th3r   (1001)     1467 2024-05-21 07:57:54.000000 django-codenerix-geodata-4.0.3/codenerix_geodata/migrations/__pycache__/0004_remove_continentgeonameen_continent_and_more.cpython-311.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      181 2022-11-26 23:27:10.000000 django-codenerix-geodata-4.0.3/codenerix_geodata/migrations/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      197 2024-02-14 12:11:39.000000 django-codenerix-geodata-4.0.3/codenerix_geodata/migrations/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      149 2020-05-15 23:36:44.000000 django-codenerix-geodata-4.0.3/codenerix_geodata/migrations/__pycache__/__init__.cpython-35.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      179 2022-11-27 21:58:10.000000 django-codenerix-geodata-4.0.3/codenerix_geodata/migrations/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)      170 2022-08-14 19:56:50.000000 django-codenerix-geodata-4.0.3/codenerix_geodata/migrations/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     9378 2022-08-14 19:56:50.000000 django-codenerix-geodata-4.0.3/codenerix_geodata/models.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     7142 2022-08-14 19:56:50.000000 django-codenerix-geodata-4.0.3/codenerix_geodata/urls.py
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)    23882 2022-08-14 19:56:50.000000 django-codenerix-geodata-4.0.3/codenerix_geodata/views.py
+drwxrwxr-x   0 br0th3r   (1001) br0th3r   (1001)        0 2024-05-23 04:46:39.699121 django-codenerix-geodata-4.0.3/django_codenerix_geodata.egg-info/
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     2988 2024-05-23 04:46:39.000000 django-codenerix-geodata-4.0.3/django_codenerix_geodata.egg-info/PKG-INFO
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     3327 2024-05-23 04:46:39.000000 django-codenerix-geodata-4.0.3/django_codenerix_geodata.egg-info/SOURCES.txt
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)        1 2024-05-23 04:46:39.000000 django-codenerix-geodata-4.0.3/django_codenerix_geodata.egg-info/dependency_links.txt
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)        1 2020-05-15 23:36:44.000000 django-codenerix-geodata-4.0.3/django_codenerix_geodata.egg-info/not-zip-safe
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)       45 2024-05-23 04:46:39.000000 django-codenerix-geodata-4.0.3/django_codenerix_geodata.egg-info/requires.txt
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)       18 2024-05-23 04:46:39.000000 django-codenerix-geodata-4.0.3/django_codenerix_geodata.egg-info/top_level.txt
+-rw-rw-r--   0 br0th3r   (1001) br0th3r   (1001)       38 2024-05-23 04:46:39.699121 django-codenerix-geodata-4.0.3/setup.cfg
+-rw-r--r--   0 br0th3r   (1001) br0th3r   (1001)     1752 2020-05-15 23:36:44.000000 django-codenerix-geodata-4.0.3/setup.py
```

### Comparing `django-codenerix-geodata-4.0.2/LICENSE` & `django-codenerix-geodata-4.0.3/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright {yyyy} {name of copyright owner}
+   Copyright 2024 Codenerix
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `django-codenerix-geodata-4.0.2/PKG-INFO` & `django-codenerix-geodata-4.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-codenerix-geodata
-Version: 4.0.2
+Version: 4.0.3
 Summary: Codenerix Geodata is a module that enables CODENERIX to manage geographical data on serveral platforms in a general manner.
 Home-page: https://github.com/codenerix/django-codenerix-geodata
 Author: Juan Miguel Taboada Godoy <juanmi@juanmitaboada.com>, Juan Soler Ruiz <soleronline@gmail.com>
 License: Apache License Version 2.0
 Keywords: django,codenerix,management,erp,crm,geodata,geo data
 Platform: OS Independent
 Classifier: Environment :: Web Environment
```

### Comparing `django-codenerix-geodata-4.0.2/README.rst` & `django-codenerix-geodata-4.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `django-codenerix-geodata-4.0.2/codenerix_geodata/admin.py` & `django-codenerix-geodata-4.0.3/codenerix_geodata/admin.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-geodata-4.0.2/codenerix_geodata/data/GeoLite2-City-Locations-en.csv.bz2` & `django-codenerix-geodata-4.0.3/codenerix_geodata/data/GeoLite2-City-Locations-en.csv.bz2`

 * *Files identical despite different names*

### Comparing `django-codenerix-geodata-4.0.2/codenerix_geodata/data/GeoLite2-City-Locations-es.csv.bz2` & `django-codenerix-geodata-4.0.3/codenerix_geodata/data/GeoLite2-City-Locations-es.csv.bz2`

 * *Files identical despite different names*

### Comparing `django-codenerix-geodata-4.0.2/codenerix_geodata/data/GeoLite2-Country-Locations-en.csv.bz2` & `django-codenerix-geodata-4.0.3/codenerix_geodata/data/GeoLite2-Country-Locations-en.csv.bz2`

 * *Files identical despite different names*

### Comparing `django-codenerix-geodata-4.0.2/codenerix_geodata/data/GeoLite2-Country-Locations-es.csv.bz2` & `django-codenerix-geodata-4.0.3/codenerix_geodata/data/GeoLite2-Country-Locations-es.csv.bz2`

 * *Files identical despite different names*

### Comparing `django-codenerix-geodata-4.0.2/codenerix_geodata/forms.py` & `django-codenerix-geodata-4.0.3/codenerix_geodata/forms.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-geodata-4.0.2/codenerix_geodata/management/commands/__pycache__/populate_geodata.cpython-35.pyc` & `django-codenerix-geodata-4.0.3/codenerix_geodata/management/commands/__pycache__/populate_geodata.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-geodata-4.0.2/codenerix_geodata/management/commands/populate_geodata.py` & `django-codenerix-geodata-4.0.3/codenerix_geodata/management/commands/populate_geodata.py`

 * *Files 15% similar despite different names*

```diff
@@ -28,451 +28,604 @@
 import sys
 import time
 from os.path import dirname, join
 from csv import reader
 
 from django.conf import settings
 from django.core.management.base import BaseCommand
-from django.utils.translation import ugettext as _
+from django.utils.translation import gettext as _
 from django.core.exceptions import ObjectDoesNotExist
 
 from codenerix_lib.debugger import Debugger
 from codenerix_extensions.helpers import FileBZ2
-from codenerix_geodata.models import Continent, Country, Region, Province, City, TimeZone
+from codenerix_geodata.models import (
+    Continent,
+    Country,
+    Region,
+    Province,
+    City,
+    TimeZone,
+)
 
 
-BASE_LANGUAGE = 'EN'
+BASE_LANGUAGE = "EN"
 
 COUNTRY_DATA_FILES = {
-    'ES': 'GeoLite2-Country-Locations-es.csv.bz2',
-    'EN': 'GeoLite2-Country-Locations-en.csv.bz2',
+    "ES": "GeoLite2-Country-Locations-es.csv.bz2",
+    "EN": "GeoLite2-Country-Locations-en.csv.bz2",
 }
 
 CITY_DATA_FILES = {
-    'ES': 'GeoLite2-City-Locations-es.csv.bz2',
-    'EN': 'GeoLite2-City-Locations-en.csv.bz2',
+    "ES": "GeoLite2-City-Locations-es.csv.bz2",
+    "EN": "GeoLite2-City-Locations-en.csv.bz2",
 }
 
-LANGUAGES = set([code for code in settings.LANGUAGES_DATABASES if code in COUNTRY_DATA_FILES])
+LANGUAGES = set(
+    [
+        code
+        for code in settings.LANGUAGES_DATABASES
+        if code in COUNTRY_DATA_FILES
+    ]
+)
 
 
 def clean(name):
     if name:
         try:
-            name = name.decode('utf-8')
+            name = name.decode("utf-8")
         except Exception:
             pass
         if name[0] == '"' and name[-1] == '"':
             return name[1:-1]
     return name
 
 
 def populate_missing_names(data):
     for lang in LANGUAGES:
         for d in data.values():
-            if lang not in d or d[lang] == '':
+            if lang not in d or d[lang] == "":
                 for other_lang in LANGUAGES - {lang}:
-                    if d[other_lang] != '':
+                    if d[other_lang] != "":
                         d[lang] = d[other_lang]
                         break
 
 
 def continents_lines(filename):
-    with FileBZ2(filename, 'rb') as data_file:
-        csv_file = reader(data_file, delimiter=',', quotechar='"')
+    with FileBZ2(filename, "rb") as data_file:
+        csv_file = reader(data_file, delimiter=",", quotechar='"')
 
         first = True
         for line in csv_file:
             if first:
                 first = False
                 continue
 
             _, _, continent_code, continent_name, _, _ = line
-            if continent_code.strip() != '' and continent_name.strip() != '':
+            if continent_code.strip() != "" and continent_name.strip() != "":
                 yield continent_code, clean(continent_name)
 
 
 def country_lines(filename):
-    with FileBZ2(filename, 'rb') as data_file:
-        csv_file = reader(data_file, delimiter=',', quotechar='"')
+    with FileBZ2(filename, "rb") as data_file:
+        csv_file = reader(data_file, delimiter=",", quotechar='"')
 
         first = True
         for line in csv_file:
             if first:
                 first = False
                 continue
 
             geoid, _, continent_code, _, country_code, country_name = line
-            if continent_code.strip() != '' and country_code.strip() != '' and country_name.strip() != '':
-                yield int(geoid), continent_code, country_code, clean(country_name)
+            if (
+                continent_code.strip() != ""
+                and country_code.strip() != ""
+                and country_name.strip() != ""
+            ):
+                yield int(geoid), continent_code, country_code, clean(
+                    country_name
+                )
 
 
 def region_lines(filename):
-    with FileBZ2(filename, 'rb') as data_file:
-        csv_file = reader(data_file, delimiter=',', quotechar='"')
+    with FileBZ2(filename, "rb") as data_file:
+        csv_file = reader(data_file, delimiter=",", quotechar='"')
 
         first = True
         for line in csv_file:
             if first:
                 first = False
                 continue
 
-            geoid, _, _, _, country_code, _, region_code, region_name, province_code, province_name, city_name, _, _ = line
-            if country_code != '' and region_code != '' and region_name.strip() != '':
+            (
+                geoid,
+                _,
+                _,
+                _,
+                country_code,
+                _,
+                region_code,
+                region_name,
+                province_code,
+                province_name,
+                city_name,
+                _,
+                _,
+            ) = line
+            if (
+                country_code != ""
+                and region_code != ""
+                and region_name.strip() != ""
+            ):
                 yield int(geoid), country_code, region_code, clean(region_name)
 
 
 def province_lines(filename):
-    with FileBZ2(filename, 'rb') as data_file:
-        csv_file = reader(data_file, delimiter=',', quotechar='"')
+    with FileBZ2(filename, "rb") as data_file:
+        csv_file = reader(data_file, delimiter=",", quotechar='"')
 
         first = True
         for line in csv_file:
             if first:
                 first = False
                 continue
 
-            geoid, _, _, _, country_code, _, region_code, _, province_code, province_name, _, _, _ = line
-            if country_code != '' and region_code != '' and province_code != '' and province_name != '':
-                yield int(geoid), country_code, region_code, province_code, clean(province_name)
+            (
+                geoid,
+                _,
+                _,
+                _,
+                country_code,
+                _,
+                region_code,
+                _,
+                province_code,
+                province_name,
+                _,
+                _,
+                _,
+            ) = line
+            if (
+                country_code != ""
+                and region_code != ""
+                and province_code != ""
+                and province_name != ""
+            ):
+                yield int(
+                    geoid
+                ), country_code, region_code, province_code, clean(
+                    province_name
+                )
 
 
 def city_lines(filename):
-    with FileBZ2(filename, 'rb') as data_file:
-        csv_file = reader(data_file, delimiter=',', quotechar='"')
+    with FileBZ2(filename, "rb") as data_file:
+        csv_file = reader(data_file, delimiter=",", quotechar='"')
 
         first = True
         for line in csv_file:
             if first:
                 first = False
                 continue
 
-            geoid, _, _, _, country_code, _, region_code, _, province_code, _, city_name, _, time_zone = line
-            if geoid != '' and city_name.strip() != '' and time_zone != '':
-                yield int(geoid), country_code, region_code, province_code, clean(city_name), clean(time_zone)
+            (
+                geoid,
+                _,
+                _,
+                _,
+                country_code,
+                _,
+                region_code,
+                _,
+                province_code,
+                _,
+                city_name,
+                _,
+                time_zone,
+            ) = line
+            if geoid != "" and city_name.strip() != "" and time_zone != "":
+                yield int(
+                    geoid
+                ), country_code, region_code, province_code, clean(
+                    city_name
+                ), clean(
+                    time_zone
+                )
 
 
 class Command(BaseCommand, Debugger):
-    help = _('Populates Continent, Country and City models')
+    help = _("Populates Continent, Country and City models")
     __percent = None
 
     def percent_init(self, text, total):
         self.__percent = {}
-        self.__percent['text'] = text
-        self.__percent['last'] = time.time()-6
-        self.__percent['counter'] = 0
-        self.__percent['total'] = total
+        self.__percent["text"] = text
+        self.__percent["last"] = time.time() - 6
+        self.__percent["counter"] = 0
+        self.__percent["total"] = total
         self.percent()
 
     def percent(self):
-        last = (self.__percent['counter']+1) == self.__percent['total']
+        last = (self.__percent["counter"] + 1) == self.__percent["total"]
         now = time.time()
-        if (self.__percent['last']+6<now) or last:
-            self.__percent['last'] = now
-            if self.__percent['counter']:
-                delstr=""
+        if (self.__percent["last"] + 6 < now) or last:
+            self.__percent["last"] = now
+            if self.__percent["counter"]:
+                delstr = ""
                 for i in range(0, 200):
-                    delstr+="\b"
+                    delstr += "\b"
                 sys.stdout.write(delstr)
             if not last:
-                text = "{}/{}".format(self.__percent['counter'], self.__percent['total'])
-                percent = 100*self.__percent['counter']/self.__percent['total']
-                self.debug("{}: ".format(self.__percent['text']), color="blue", tail=False)
-                self.debug("{}".format(text), color="cyan", head=False, tail=False)
-                self.debug(" - {:.1f}%      ".format(percent), color="white", head=False, tail=False)
+                text = "{}/{}".format(
+                    self.__percent["counter"], self.__percent["total"]
+                )
+                percent = (
+                    100 * self.__percent["counter"] / self.__percent["total"]
+                )
+                self.debug(
+                    "{}: ".format(self.__percent["text"]),
+                    color="blue",
+                    tail=False,
+                )
+                self.debug(
+                    "{}".format(text), color="cyan", head=False, tail=False
+                )
+                self.debug(
+                    " - {:.1f}%      ".format(percent),
+                    color="white",
+                    head=False,
+                    tail=False,
+                )
             else:
-                self.debug(self.__percent['text'], color="blue", tail=False)
-                self.debug(" ... Done                     ", head=False, color="green")
+                self.debug(self.__percent["text"], color="blue", tail=False)
+                self.debug(
+                    " ... Done                     ", head=False, color="green"
+                )
             sys.stdout.flush()
-        self.__percent['counter'] += 1
+        self.__percent["counter"] += 1
 
     def handle(self, *args, **options):
 
         # Autoconfigure Debugger
-        self.set_name('CODENERIX-GEODATA')
+        self.set_name("CODENERIX-GEODATA")
         self.set_debug()
 
         # print('Erasing existing data ...')
         # City.objects.all().delete()
         # TimeZone.objects.all().delete()
         # Province.objects.all().delete()
         # Region.objects.all().delete()
         # Country.objects.all().delete()
         # Continent.objects.all().delete()
 
-        print('Importing new data ... This action may take some minutes.')
-        print('')
-        data_path = join(dirname(dirname(dirname(__file__))), 'data')
+        print("Importing new data ... This action may take some minutes.")
+        print("")
+        data_path = join(dirname(dirname(dirname(__file__))), "data")
 
         # Importing language generated models
         for lang in LANGUAGES:
-            exec('from codenerix_geodata.models import ContinentGeoName{}'.format(lang))
-            exec('from codenerix_geodata.models import CountryGeoName{}'.format(lang))
-            exec('from codenerix_geodata.models import RegionGeoName{}'.format(lang))
-            exec('from codenerix_geodata.models import ProvinceGeoName{}'.format(lang))
-            exec('from codenerix_geodata.models import CityGeoName{}'.format(lang))
-
-        self.debug('Importing ...', color='yellow', tail=False)
-        self.debug(' Continents', color='purple', head=False, tail=False)
-        self.debug(' Countries Regions Provinces Cities', color='grey', head=False)
+            exec(
+                "from codenerix_geodata.models import ContinentGeoName{}".format(
+                    lang
+                )
+            )
+            exec(
+                "from codenerix_geodata.models import CountryGeoName{}".format(
+                    lang
+                )
+            )
+            exec(
+                "from codenerix_geodata.models import RegionGeoName{}".format(
+                    lang
+                )
+            )
+            exec(
+                "from codenerix_geodata.models import ProvinceGeoName{}".format(
+                    lang
+                )
+            )
+            exec(
+                "from codenerix_geodata.models import CityGeoName{}".format(
+                    lang
+                )
+            )
+
+        self.debug("Importing ...", color="yellow", tail=False)
+        self.debug(" Continents", color="purple", head=False, tail=False)
+        self.debug(
+            " Countries Regions Provinces Cities", color="grey", head=False
+        )
         continents = {}
         for lang in LANGUAGES:
             filename = join(data_path, COUNTRY_DATA_FILES[lang])
             lines = list(continents_lines(filename))
             self.percent_init("    > Prepare data {}".format(lang), len(lines))
             for code, name in lines:
                 if code not in continents:
-                    continents[code] = {
-                        'model': Continent(code=code)
-                    }
+                    continents[code] = {"model": Continent(code=code)}
                 continents[code][lang] = name
                 self.percent()
 
         items = continents.items()
         self.percent_init("    > Link", len(items))
         for code, continent in items:
             try:
                 model = Continent.objects.get(code=code)
-                continent['model'] = model
+                continent["model"] = model
             except ObjectDoesNotExist:
-                continent['model'].save()
+                continent["model"].save()
             self.percent()
 
         for lang in LANGUAGES:
-            model_type = eval('ContinentGeoName{}'.format(lang))
+            model_type = eval("ContinentGeoName{}".format(lang))
             items = continents.values()
             self.percent_init("    > Fill {}".format(lang), len(items))
             for continent in items:
                 try:
-                    model = model_type.objects.get(continent=continent['model'])
+                    model = model_type.objects.get(
+                        continent=continent["model"]
+                    )
                 except ObjectDoesNotExist:
                     model = model_type()
-                    model.continent = continent['model']
+                    model.continent = continent["model"]
                 model.name = continent[lang]
                 model.save()
                 self.percent()
 
-        self.debug('Importing ...', color='yellow', tail=False)
-        self.debug(' Continents', color='simplepurple', head=False, tail=False)
-        self.debug(' Countries', color='purple', head=False, tail=False)
-        self.debug(' Regions Provinces Cities', color='grey', head=False)
+        self.debug("Importing ...", color="yellow", tail=False)
+        self.debug(" Continents", color="simplepurple", head=False, tail=False)
+        self.debug(" Countries", color="purple", head=False, tail=False)
+        self.debug(" Regions Provinces Cities", color="grey", head=False)
         countries = {}
         for lang in LANGUAGES:
             filename = join(data_path, COUNTRY_DATA_FILES[lang])
             items = list(country_lines(filename))
             self.percent_init("    > Prepare data {}".format(lang), len(items))
             for geoid, continent, code, name in items:
                 if code not in countries:
                     countries[code] = {
-                        'model': Country(
+                        "model": Country(
                             pk=geoid,
                             code=code,
-                            continent=continents[continent]['model']
+                            continent=continents[continent]["model"],
                         )
                     }
                 countries[code][lang] = name
                 self.percent()
 
         values = countries.values()
         self.percent_init("    > Link", len(values))
         for country in values:
             try:
-                model = Country.objects.get(code=country['model'].code)
-                country['model'] = model
+                model = Country.objects.get(code=country["model"].code)
+                country["model"] = model
             except ObjectDoesNotExist:
-                country['model'].save()
+                country["model"].save()
             self.percent()
 
         for lang in LANGUAGES:
-            model_type = eval('CountryGeoName{}'.format(lang))
+            model_type = eval("CountryGeoName{}".format(lang))
             self.percent_init("    > Fill {}".format(lang), len(values))
             for country in values:
                 try:
-                    model = model_type.objects.get(country=country['model'])
+                    model = model_type.objects.get(country=country["model"])
                 except ObjectDoesNotExist:
                     model = model_type()
-                    model.country = country['model']
+                    model.country = country["model"]
                 model.name = country[lang]
                 model.save()
                 self.percent()
 
-        self.debug('Importing ...', color='yellow', tail=False)
-        self.debug(' Continents Countries', color='simplepurple', head=False, tail=False)
-        self.debug(' Regions', color='purple', head=False, tail=False)
-        self.debug(' Provinces Cities', color='grey', head=False)
+        self.debug("Importing ...", color="yellow", tail=False)
+        self.debug(
+            " Continents Countries",
+            color="simplepurple",
+            head=False,
+            tail=False,
+        )
+        self.debug(" Regions", color="purple", head=False, tail=False)
+        self.debug(" Provinces Cities", color="grey", head=False)
         regions = {}
         for lang in LANGUAGES:
             filename = join(data_path, CITY_DATA_FILES[lang])
             lines = list(region_lines(filename))
             self.percent_init("    > Prepare data {}".format(lang), len(lines))
             for geoid, country_code, region_code, region_name in lines:
-                region_key = '{}_{}'.format(country_code, region_code)
+                region_key = "{}_{}".format(country_code, region_code)
                 if region_key not in regions:
                     regions[region_key] = {
-                        'model': Region(
+                        "model": Region(
                             pk=geoid,
                             code=region_code,
-                            country=countries[country_code]['model']
+                            country=countries[country_code]["model"],
                         )
                     }
                 regions[region_key][lang] = region_name
                 self.percent()
 
         items = regions.values()
         self.percent_init("    > Link", len(items))
         for region in items:
             try:
-                model = Region.objects.get(pk=region['model'].pk)
-                region['model'] = model
+                model = Region.objects.get(pk=region["model"].pk)
+                region["model"] = model
             except ObjectDoesNotExist:
-                region['model'].save()
+                region["model"].save()
             self.percent()
 
-        self.debug("    > Populate missing", color='blue', tail=False)
+        self.debug("    > Populate missing", color="blue", tail=False)
         populate_missing_names(regions)
-        self.debug(" ... Done", color='green', head=False)
+        self.debug(" ... Done", color="green", head=False)
 
         for lang in LANGUAGES:
-            model_type = eval('RegionGeoName{}'.format(lang))
+            model_type = eval("RegionGeoName{}".format(lang))
             items = regions.values()
             self.percent_init("    > Fill {}".format(lang), len(items))
             for region in items:
                 try:
-                    model = model_type.objects.get(region=region['model'])
+                    model = model_type.objects.get(region=region["model"])
                 except ObjectDoesNotExist:
                     model = model_type()
-                    model.region = region['model']
+                    model.region = region["model"]
                     model.name = region[lang]
                 model.save()
                 self.percent()
 
-        self.debug('Importing ...', color='yellow', tail=False)
-        self.debug(' Continents Countries Regions', color='simplepurple', head=False, tail=False)
-        self.debug(' Provinces', color='purple', head=False, tail=False)
-        self.debug(' Cities', color='grey', head=False)
+        self.debug("Importing ...", color="yellow", tail=False)
+        self.debug(
+            " Continents Countries Regions",
+            color="simplepurple",
+            head=False,
+            tail=False,
+        )
+        self.debug(" Provinces", color="purple", head=False, tail=False)
+        self.debug(" Cities", color="grey", head=False)
         provinces = {}
         for lang in LANGUAGES:
             filename = join(data_path, CITY_DATA_FILES[lang])
             lines = list(province_lines(filename))
             self.percent_init("    > Prepare data {}".format(lang), len(lines))
-            for geoid, country_code, region_code, province_code, province_name in lines:
-                region_key = '{}_{}'.format(country_code, region_code)
-                province_key = '{}_{}_{}'.format(country_code, region_code, province_code)
+            for (
+                geoid,
+                country_code,
+                region_code,
+                province_code,
+                province_name,
+            ) in lines:
+                region_key = "{}_{}".format(country_code, region_code)
+                province_key = "{}_{}_{}".format(
+                    country_code, region_code, province_code
+                )
                 if province_key not in provinces:
                     provinces[province_key] = {
-                        'model': Province(
+                        "model": Province(
                             pk=geoid,
                             code=province_code,
-                            region=regions[region_key]['model']
+                            region=regions[region_key]["model"],
                         )
                     }
                 provinces[province_key][lang] = province_name
                 self.percent()
 
         items = provinces.values()
         self.percent_init("    > Link", len(items))
         for province in items:
             try:
-                model = Province.objects.get(pk=province['model'].pk)
-                province['model'] = model
+                model = Province.objects.get(pk=province["model"].pk)
+                province["model"] = model
             except ObjectDoesNotExist:
-                province['model'].save()
+                province["model"].save()
             self.percent()
 
-        self.debug("    > Populate missing", color='blue', tail=False)
+        self.debug("    > Populate missing", color="blue", tail=False)
         populate_missing_names(provinces)
-        self.debug(" ... Done", color='green', head=False)
+        self.debug(" ... Done", color="green", head=False)
 
         for lang in LANGUAGES:
-            model_type = eval('ProvinceGeoName{}'.format(lang))
+            model_type = eval("ProvinceGeoName{}".format(lang))
             items = provinces.values()
             self.percent_init("    > Fill {}".format(lang), len(items))
             for province in items:
                 try:
-                    model = model_type.objects.get(province=province['model'])
+                    model = model_type.objects.get(province=province["model"])
                 except ObjectDoesNotExist:
                     model = model_type()
-                    model.province = province['model']
+                    model.province = province["model"]
                 model.name = province[lang]
                 model.save()
                 self.percent()
 
-        self.debug('Importing ...', color='yellow', tail=False)
-        self.debug(' Continents Countries Regions Provinces', color='simplepurple', head=False, tail=False)
-        self.debug(' Cities', color='purple', head=False, tail=False)
+        self.debug("Importing ...", color="yellow", tail=False)
+        self.debug(
+            " Continents Countries Regions Provinces",
+            color="simplepurple",
+            head=False,
+            tail=False,
+        )
+        self.debug(" Cities", color="purple", head=False, tail=False)
         cities = {}
         timezones = {}
         for lang in LANGUAGES:
             filename = join(data_path, CITY_DATA_FILES[lang])
             lines = list(city_lines(filename))
             self.percent_init("    > Prepare data {}".format(lang), len(lines))
-            for city_id, country_code, region_code, province_code, city_name, time_zone in lines:
+            for (
+                city_id,
+                country_code,
+                region_code,
+                province_code,
+                city_name,
+                time_zone,
+            ) in lines:
                 if time_zone not in timezones:
                     try:
                         model = TimeZone.objects.get(name=time_zone)
                         timezones[time_zone] = model
                     except ObjectDoesNotExist:
                         timezones[time_zone] = TimeZone(name=time_zone)
                         timezones[time_zone].save()
 
                 if city_id not in cities:
                     city = City(
                         pk=city_id,
-                        country=countries[country_code]['model'],
-                        time_zone=timezones[time_zone]
+                        country=countries[country_code]["model"],
+                        time_zone=timezones[time_zone],
                     )
-                    if region_code != '':
-                        region_key = '{}_{}'.format(country_code, region_code)
-                        city.region = regions[region_key]['model']
-
-                    if province_code != '':
-                        province_key = '{}_{}_{}'.format(country_code, region_code, province_code)
-                        city.province = provinces[province_key]['model']
+                    if region_code != "":
+                        region_key = "{}_{}".format(country_code, region_code)
+                        city.region = regions[region_key]["model"]
+
+                    if province_code != "":
+                        province_key = "{}_{}_{}".format(
+                            country_code, region_code, province_code
+                        )
+                        city.province = provinces[province_key]["model"]
 
-                    cities[city_id] = {
-                        'model': city
-                    }
+                    cities[city_id] = {"model": city}
 
                 cities[city_id][lang] = city_name
                 self.percent()
 
         items = cities.values()
         self.percent_init("    > Link", len(items))
         for city in items:
             try:
-                model = City.objects.get(pk=city['model'].pk)
-                city['model'] = model
+                model = City.objects.get(pk=city["model"].pk)
+                city["model"] = model
             except ObjectDoesNotExist:
-                city['model'].save()
+                city["model"].save()
             self.percent()
 
-        self.debug("    > Populate missing", color='blue', tail=False)
+        self.debug("    > Populate missing", color="blue", tail=False)
         populate_missing_names(cities)
-        self.debug(" ... Done", color='green', head=False)
+        self.debug(" ... Done", color="green", head=False)
 
         for lang in LANGUAGES:
-            model_type = eval('CityGeoName{}'.format(lang))
+            model_type = eval("CityGeoName{}".format(lang))
             items = cities.values()
             self.percent_init("    > Fill {}".format(lang), len(items))
             for city in items:
                 try:
-                    model = model_type.objects.get(city=city['model'])
+                    model = model_type.objects.get(city=city["model"])
                 except ObjectDoesNotExist:
                     model = model_type()
-                    model.city = city['model']
+                    model.city = city["model"]
                 model.name = city[lang]
                 model.save()
                 self.percent()
 
-        self.debug('Removing regions without cities ...', color='yellow', tail=False)
+        self.debug(
+            "Removing regions without cities ...", color="yellow", tail=False
+        )
         for region in Region.objects.all():
             if region.cities.count() == 0:
                 region.delete()
-        self.debug(" ... Done", color='green', head=False)
+        self.debug(" ... Done", color="green", head=False)
 
-        self.debug('Removing provinces without cities ...', color='yellow', tail=False)
+        self.debug(
+            "Removing provinces without cities ...", color="yellow", tail=False
+        )
         for province in Province.objects.all():
             if province.cities.count() == 0:
                 province.delete()
-        self.debug(" ... Done", color='green', head=False)
+        self.debug(" ... Done", color="green", head=False)
 
-        self.debug('All done !!!', color="green")
+        self.debug("All done !!!", color="green")
```

### Comparing `django-codenerix-geodata-4.0.2/codenerix_geodata/migrations/0001_initial.py` & `django-codenerix-geodata-4.0.3/codenerix_geodata/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-geodata-4.0.2/codenerix_geodata/migrations/0002_auto_20170921_1206.py` & `django-codenerix-geodata-4.0.3/codenerix_geodata/migrations/0002_auto_20170921_1206.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-geodata-4.0.2/codenerix_geodata/migrations/0003_auto_20180118_1209.py` & `django-codenerix-geodata-4.0.3/codenerix_geodata/migrations/0003_auto_20180118_1209.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-geodata-4.0.2/codenerix_geodata/migrations/__pycache__/0001_initial.cpython-310.pyc` & `django-codenerix-geodata-4.0.3/codenerix_geodata/migrations/__pycache__/0001_initial.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-geodata-4.0.2/codenerix_geodata/migrations/__pycache__/0001_initial.cpython-35.pyc` & `django-codenerix-geodata-4.0.3/codenerix_geodata/migrations/__pycache__/0001_initial.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-geodata-4.0.2/codenerix_geodata/migrations/__pycache__/0001_initial.cpython-38.pyc` & `django-codenerix-geodata-4.0.3/codenerix_geodata/migrations/__pycache__/0001_initial.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-geodata-4.0.2/codenerix_geodata/migrations/__pycache__/0001_initial.cpython-39.pyc` & `django-codenerix-geodata-4.0.3/codenerix_geodata/migrations/__pycache__/0001_initial.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-geodata-4.0.2/codenerix_geodata/migrations/__pycache__/0002_auto_20170921_1206.cpython-310.pyc` & `django-codenerix-geodata-4.0.3/codenerix_geodata/migrations/__pycache__/0002_auto_20170921_1206.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-geodata-4.0.2/codenerix_geodata/migrations/__pycache__/0002_auto_20170921_1206.cpython-35.pyc` & `django-codenerix-geodata-4.0.3/codenerix_geodata/migrations/__pycache__/0002_auto_20170921_1206.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-geodata-4.0.2/codenerix_geodata/migrations/__pycache__/0002_auto_20170921_1206.cpython-38.pyc` & `django-codenerix-geodata-4.0.3/codenerix_geodata/migrations/__pycache__/0002_auto_20170921_1206.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-geodata-4.0.2/codenerix_geodata/migrations/__pycache__/0002_auto_20170921_1206.cpython-39.pyc` & `django-codenerix-geodata-4.0.3/codenerix_geodata/migrations/__pycache__/0002_auto_20170921_1206.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-geodata-4.0.2/codenerix_geodata/migrations/__pycache__/0003_auto_20180118_1209.cpython-310.pyc` & `django-codenerix-geodata-4.0.3/codenerix_geodata/migrations/__pycache__/0003_auto_20180118_1209.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-geodata-4.0.2/codenerix_geodata/migrations/__pycache__/0003_auto_20180118_1209.cpython-35.pyc` & `django-codenerix-geodata-4.0.3/codenerix_geodata/migrations/__pycache__/0003_auto_20180118_1209.cpython-35.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-geodata-4.0.2/codenerix_geodata/migrations/__pycache__/0003_auto_20180118_1209.cpython-38.pyc` & `django-codenerix-geodata-4.0.3/codenerix_geodata/migrations/__pycache__/0003_auto_20180118_1209.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-geodata-4.0.2/codenerix_geodata/migrations/__pycache__/0003_auto_20180118_1209.cpython-39.pyc` & `django-codenerix-geodata-4.0.3/codenerix_geodata/migrations/__pycache__/0003_auto_20180118_1209.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-codenerix-geodata-4.0.2/codenerix_geodata/models.py` & `django-codenerix-geodata-4.0.3/codenerix_geodata/models.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-geodata-4.0.2/codenerix_geodata/urls.py` & `django-codenerix-geodata-4.0.3/codenerix_geodata/urls.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-geodata-4.0.2/codenerix_geodata/views.py` & `django-codenerix-geodata-4.0.3/codenerix_geodata/views.py`

 * *Files identical despite different names*

### Comparing `django-codenerix-geodata-4.0.2/django_codenerix_geodata.egg-info/PKG-INFO` & `django-codenerix-geodata-4.0.3/django_codenerix_geodata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-codenerix-geodata
-Version: 4.0.2
+Version: 4.0.3
 Summary: Codenerix Geodata is a module that enables CODENERIX to manage geographical data on serveral platforms in a general manner.
 Home-page: https://github.com/codenerix/django-codenerix-geodata
 Author: Juan Miguel Taboada Godoy <juanmi@juanmitaboada.com>, Juan Soler Ruiz <soleronline@gmail.com>
 License: Apache License Version 2.0
 Keywords: django,codenerix,management,erp,crm,geodata,geo data
 Platform: OS Independent
 Classifier: Environment :: Web Environment
```

### Comparing `django-codenerix-geodata-4.0.2/django_codenerix_geodata.egg-info/SOURCES.txt` & `django-codenerix-geodata-4.0.3/django_codenerix_geodata.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -11,38 +11,46 @@
 codenerix_geodata/views.py
 codenerix_geodata/data/GeoLite2-City-Locations-en.csv.bz2
 codenerix_geodata/data/GeoLite2-City-Locations-es.csv.bz2
 codenerix_geodata/data/GeoLite2-Country-Locations-en.csv.bz2
 codenerix_geodata/data/GeoLite2-Country-Locations-es.csv.bz2
 codenerix_geodata/management/__init__.py
 codenerix_geodata/management/__pycache__/__init__.cpython-310.pyc
+codenerix_geodata/management/__pycache__/__init__.cpython-311.pyc
 codenerix_geodata/management/__pycache__/__init__.cpython-35.pyc
 codenerix_geodata/management/__pycache__/__init__.cpython-38.pyc
 codenerix_geodata/management/__pycache__/__init__.cpython-39.pyc
 codenerix_geodata/management/commands/__init__.py
 codenerix_geodata/management/commands/populate_geodata.py
+codenerix_geodata/management/commands/__pycache__/__init__.cpython-311.pyc
 codenerix_geodata/management/commands/__pycache__/__init__.cpython-35.pyc
+codenerix_geodata/management/commands/__pycache__/populate_geodata.cpython-311.pyc
 codenerix_geodata/management/commands/__pycache__/populate_geodata.cpython-35.pyc
 codenerix_geodata/migrations/0001_initial.py
 codenerix_geodata/migrations/0002_auto_20170921_1206.py
 codenerix_geodata/migrations/0003_auto_20180118_1209.py
 codenerix_geodata/migrations/__init__.py
 codenerix_geodata/migrations/__pycache__/0001_initial.cpython-310.pyc
+codenerix_geodata/migrations/__pycache__/0001_initial.cpython-311.pyc
 codenerix_geodata/migrations/__pycache__/0001_initial.cpython-35.pyc
 codenerix_geodata/migrations/__pycache__/0001_initial.cpython-38.pyc
 codenerix_geodata/migrations/__pycache__/0001_initial.cpython-39.pyc
 codenerix_geodata/migrations/__pycache__/0002_auto_20170921_1206.cpython-310.pyc
+codenerix_geodata/migrations/__pycache__/0002_auto_20170921_1206.cpython-311.pyc
 codenerix_geodata/migrations/__pycache__/0002_auto_20170921_1206.cpython-35.pyc
 codenerix_geodata/migrations/__pycache__/0002_auto_20170921_1206.cpython-38.pyc
 codenerix_geodata/migrations/__pycache__/0002_auto_20170921_1206.cpython-39.pyc
 codenerix_geodata/migrations/__pycache__/0003_auto_20180118_1209.cpython-310.pyc
+codenerix_geodata/migrations/__pycache__/0003_auto_20180118_1209.cpython-311.pyc
 codenerix_geodata/migrations/__pycache__/0003_auto_20180118_1209.cpython-35.pyc
 codenerix_geodata/migrations/__pycache__/0003_auto_20180118_1209.cpython-38.pyc
 codenerix_geodata/migrations/__pycache__/0003_auto_20180118_1209.cpython-39.pyc
+codenerix_geodata/migrations/__pycache__/0004_remove_continentgeonameen_continent_and_more.cpython-311.pyc
 codenerix_geodata/migrations/__pycache__/__init__.cpython-310.pyc
+codenerix_geodata/migrations/__pycache__/__init__.cpython-311.pyc
 codenerix_geodata/migrations/__pycache__/__init__.cpython-35.pyc
 codenerix_geodata/migrations/__pycache__/__init__.cpython-38.pyc
 codenerix_geodata/migrations/__pycache__/__init__.cpython-39.pyc
 django_codenerix_geodata.egg-info/PKG-INFO
 django_codenerix_geodata.egg-info/SOURCES.txt
 django_codenerix_geodata.egg-info/dependency_links.txt
 django_codenerix_geodata.egg-info/not-zip-safe
```

### Comparing `django-codenerix-geodata-4.0.2/setup.py` & `django-codenerix-geodata-4.0.3/setup.py`

 * *Files identical despite different names*

