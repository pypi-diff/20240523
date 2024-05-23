# Comparing `tmp/tap-taboola-0.2.1.tar.gz` & `tmp/tap_taboola-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tap-taboola-0.2.1.tar", last modified: Tue Apr 30 20:31:45 2019, max compression
+gzip compressed data, was "tap_taboola-0.3.0.tar", last modified: Thu May 23 12:13:38 2024, max compression
```

## Comparing `tap-taboola-0.2.1.tar` & `tap_taboola-0.3.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-04-30 20:31:45.000000 tap-taboola-0.2.1/
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-04-30 20:31:45.000000 tap-taboola-0.2.1/tap_taboola/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     4940 2018-11-09 20:03:04.000000 tap-taboola-0.2.1/tap_taboola/schemas.py
--rwxrwxr-x   0 vagrant   (1000) vagrant   (1000)    10933 2019-04-30 20:30:45.000000 tap-taboola-0.2.1/tap_taboola/__init__.py
-drwxrwxr-x   0 vagrant   (1000) vagrant   (1000)        0 2019-04-30 20:31:45.000000 tap-taboola-0.2.1/tap_taboola.egg-info/
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)        1 2019-04-30 20:31:45.000000 tap-taboola-0.2.1/tap_taboola.egg-info/dependency_links.txt
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)       76 2019-04-30 20:31:45.000000 tap-taboola-0.2.1/tap_taboola.egg-info/requires.txt
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)       74 2019-04-30 20:31:45.000000 tap-taboola-0.2.1/tap_taboola.egg-info/entry_points.txt
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      277 2019-04-30 20:31:45.000000 tap-taboola-0.2.1/tap_taboola.egg-info/SOURCES.txt
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)       12 2019-04-30 20:31:45.000000 tap-taboola-0.2.1/tap_taboola.egg-info/top_level.txt
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      312 2019-04-30 20:31:45.000000 tap-taboola-0.2.1/tap_taboola.egg-info/PKG-INFO
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      643 2019-04-30 20:31:00.000000 tap-taboola-0.2.1/setup.py
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)      312 2019-04-30 20:31:45.000000 tap-taboola-0.2.1/PKG-INFO
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)       38 2019-04-30 20:31:45.000000 tap-taboola-0.2.1/setup.cfg
--rw-rw-r--   0 vagrant   (1000) vagrant   (1000)     1991 2018-11-09 20:03:04.000000 tap-taboola-0.2.1/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 12:13:38.068874 tap_taboola-0.3.0/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)    32386 2024-05-23 12:08:52.000000 tap_taboola-0.3.0/LICENSE
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      392 2024-05-23 12:13:38.068874 tap_taboola-0.3.0/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1991 2024-05-23 12:08:52.000000 tap_taboola-0.3.0/README.md
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-05-23 12:13:38.068874 tap_taboola-0.3.0/setup.cfg
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      643 2024-05-23 12:08:52.000000 tap_taboola-0.3.0/setup.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 12:13:38.064875 tap_taboola-0.3.0/tap_taboola/
+-rwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)    11098 2024-05-23 12:08:52.000000 tap_taboola-0.3.0/tap_taboola/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     5220 2024-05-23 12:08:52.000000 tap_taboola-0.3.0/tap_taboola/schemas.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-23 12:13:38.068874 tap_taboola-0.3.0/tap_taboola.egg-info/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      392 2024-05-23 12:13:38.000000 tap_taboola-0.3.0/tap_taboola.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      285 2024-05-23 12:13:38.000000 tap_taboola-0.3.0/tap_taboola.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-05-23 12:13:38.000000 tap_taboola-0.3.0/tap_taboola.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       49 2024-05-23 12:13:38.000000 tap_taboola-0.3.0/tap_taboola.egg-info/entry_points.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       76 2024-05-23 12:13:38.000000 tap_taboola-0.3.0/tap_taboola.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       12 2024-05-23 12:13:38.000000 tap_taboola-0.3.0/tap_taboola.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `tap-taboola-0.2.1/tap_taboola/schemas.py` & `tap_taboola-0.3.0/tap_taboola/schemas.py`

 * *Files 3% similar despite different names*

```diff
@@ -125,14 +125,18 @@
             'format': 'date',
             'description': 'The start date for this campaign.',
         },
         'impressions': {
             'type': 'integer',
             'description': 'Total number of impressions',
         },
+        'campaign_name': {
+            'type': ['string', 'null'],
+            'description': 'Human-readable campaign name',
+        },
         'ctr': {
             'type': 'number',
             'description': 'CTR, calculated as clicks/impressions',
         },
         'clicks': {
             'type': 'integer',
             'description': 'Total number of clicks',
@@ -158,13 +162,17 @@
             'type': 'number',
             'description': 'CPA, calculated as spend/actions',
         },
         'spent': {
             'type': 'number',
             'description': 'Total spent amount',
         },
+        'conversions_value': {
+            'type': ['number', 'null'],
+            'description': 'Total revenue from conversions',
+        },
         'currency': {
             'type': 'string',
             'description': 'ISO4217 currency code for columns of type money',
         }
     }
 }
```

### Comparing `tap-taboola-0.2.1/tap_taboola/__init__.py` & `tap_taboola-0.3.0/tap_taboola/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -128,14 +128,16 @@
         'cpa_conversion_rate': float(campaign_performance.get(
             'cpa_conversion_rate', 0.0)),
         'spent': float(campaign_performance.get('spent', 0.0)),
         'date': str(datetime.datetime.strptime(
             campaign_performance.get('date'),
             '%Y-%m-%d %H:%M:%S.%f'
         ).date()),
+        'campaign_name': str(campaign_performance.get('campaign_name', '')),
+        'conversions_value': float(campaign_performance.get('conversions_value', 0.0)),
     }
 
 def fetch_campaign_performance(config, state, access_token, account_id):
     url = ('{}/backstage/api/1.0/{}/reports/campaign-summary/dimensions/campaign_day_breakdown' #pylint: disable=line-too-long
            .format(BASE_URL, account_id))
 
     params = {
```

### Comparing `tap-taboola-0.2.1/setup.py` & `tap_taboola-0.3.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 
 from setuptools import setup
 
 setup(name='tap-taboola',
-      version='0.2.1',
+      version='0.3.0',
       description='Singer.io tap for extracting data from the Taboola API',
       author='Fishtown Analytics',
       url='http://www.singer.io',
       classifiers=['Programming Language :: Python :: 3 :: Only'],
       py_modules=['tap_taboola'],
       install_requires=[
           'singer-python==5.0.4',
```

### Comparing `tap-taboola-0.2.1/README.md` & `tap_taboola-0.3.0/README.md`

 * *Files identical despite different names*

