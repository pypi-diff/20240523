# Comparing `tmp/adafri-0.0.87.tar.gz` & `tmp/adafri-0.0.88.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafri-0.0.87.tar", last modified: Sat Aug 12 00:43:17 2023, max compression
+gzip compressed data, was "adafri-0.0.88.tar", last modified: Thu May 23 20:39:44 2024, max compression
```

## Comparing `adafri-0.0.87.tar` & `adafri-0.0.88.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-12 00:43:17.111302 adafri-0.0.87/
--rw-r--r--   0 ibrahima   (502) staff       (20)      177 2023-08-12 00:43:17.110621 adafri-0.0.87/PKG-INFO
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-12 00:43:17.073490 adafri-0.0.87/adafri/
--rw-r--r--   0 ibrahima   (502) staff       (20)       80 2023-08-12 00:43:11.000000 adafri-0.0.87/adafri/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-12 00:43:17.081035 adafri-0.0.87/adafri/utils/
--rw-r--r--   0 ibrahima   (502) staff       (20)      101 2023-07-21 05:44:28.000000 adafri-0.0.87/adafri/utils/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     1252 2023-07-21 06:19:41.000000 adafri-0.0.87/adafri/utils/country.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     2519 2023-07-22 08:32:21.000000 adafri-0.0.87/adafri/utils/phone_number.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     1356 2023-07-31 01:55:04.000000 adafri-0.0.87/adafri/utils/response.py
--rw-r--r--   0 ibrahima   (502) staff       (20)    19215 2023-08-07 05:42:43.000000 adafri-0.0.87/adafri/utils/utils.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-12 00:43:17.082480 adafri-0.0.87/adafri/v1/
--rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-16 06:12:23.000000 adafri-0.0.87/adafri/v1/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-12 00:43:17.083530 adafri-0.0.87/adafri/v1/account/
--rw-r--r--   0 ibrahima   (502) staff       (20)      151 2023-07-12 07:06:08.000000 adafri-0.0.87/adafri/v1/account/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-12 00:43:17.086440 adafri-0.0.87/adafri/v1/account/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)       91 2023-07-12 06:20:02.000000 adafri-0.0.87/adafri/v1/account/models/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     4514 2023-07-20 05:14:32.000000 adafri-0.0.87/adafri/v1/account/models/account.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     3852 2023-07-28 08:14:22.000000 adafri-0.0.87/adafri/v1/account/models/account_fields.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-12 00:43:17.087272 adafri-0.0.87/adafri/v1/auth/
--rw-r--r--   0 ibrahima   (502) staff       (20)      249 2023-07-16 05:40:34.000000 adafri-0.0.87/adafri/v1/auth/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-12 00:43:17.088245 adafri-0.0.87/adafri/v1/auth/firebase_auth/
--rw-r--r--   0 ibrahima   (502) staff       (20)      316 2023-07-25 19:22:35.000000 adafri-0.0.87/adafri/v1/auth/firebase_auth/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     5059 2023-07-26 04:56:41.000000 adafri-0.0.87/adafri/v1/auth/firebase_auth/firebase_auth.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-12 00:43:17.088728 adafri-0.0.87/adafri/v1/auth/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)        0 2023-07-12 11:05:39.000000 adafri-0.0.87/adafri/v1/auth/models/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-12 00:43:17.089093 adafri-0.0.87/adafri/v1/auth/oauth/
--rw-r--r--   0 ibrahima   (502) staff       (20)      965 2023-07-28 08:17:28.000000 adafri-0.0.87/adafri/v1/auth/oauth/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-12 00:43:17.097191 adafri-0.0.87/adafri/v1/auth/oauth/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)       93 2023-07-12 11:08:07.000000 adafri-0.0.87/adafri/v1/auth/oauth/models/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     7216 2023-08-07 05:09:25.000000 adafri-0.0.87/adafri/v1/auth/oauth/models/client.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     5478 2023-07-28 08:09:48.000000 adafri-0.0.87/adafri/v1/auth/oauth/models/client_fields.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     6646 2023-08-12 00:11:47.000000 adafri-0.0.87/adafri/v1/auth/oauth/models/code.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     2505 2023-07-31 01:28:33.000000 adafri-0.0.87/adafri/v1/auth/oauth/models/code_fields.py
--rw-r--r--   0 ibrahima   (502) staff       (20)    16152 2023-08-07 05:07:34.000000 adafri-0.0.87/adafri/v1/auth/oauth/models/grant.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     3653 2023-07-28 08:10:56.000000 adafri-0.0.87/adafri/v1/auth/oauth/models/grant_fields.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     9460 2023-08-07 05:08:18.000000 adafri-0.0.87/adafri/v1/auth/oauth/models/token.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     3728 2023-07-28 08:11:40.000000 adafri-0.0.87/adafri/v1/auth/oauth/models/token_fields.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-12 00:43:17.101884 adafri-0.0.87/adafri/v1/auth/oauth/server/
--rw-r--r--   0 ibrahima   (502) staff       (20)      163 2023-07-16 05:39:01.000000 adafri-0.0.87/adafri/v1/auth/oauth/server/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     1574 2023-07-20 05:43:11.000000 adafri-0.0.87/adafri/v1/auth/oauth/server/oidc_server.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     2685 2023-07-19 19:45:35.000000 adafri-0.0.87/adafri/v1/auth/oauth/server/server.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-12 00:43:17.104485 adafri-0.0.87/adafri/v1/base/
--rw-r--r--   0 ibrahima   (502) staff       (20)       71 2023-07-12 22:38:38.000000 adafri-0.0.87/adafri/v1/base/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     4240 2023-07-25 06:31:47.000000 adafri-0.0.87/adafri/v1/base/firebase_collection.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-12 00:43:17.105323 adafri-0.0.87/adafri/v1/mailing/
--rw-r--r--   0 ibrahima   (502) staff       (20)    13843 2023-08-12 00:43:06.000000 adafri-0.0.87/adafri/v1/mailing/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-12 00:43:17.106224 adafri-0.0.87/adafri/v1/user/
--rw-r--r--   0 ibrahima   (502) staff       (20)      129 2023-07-12 01:27:49.000000 adafri-0.0.87/adafri/v1/user/__init__.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-12 00:43:17.109400 adafri-0.0.87/adafri/v1/user/models/
--rw-r--r--   0 ibrahima   (502) staff       (20)       78 2023-07-12 00:55:42.000000 adafri-0.0.87/adafri/v1/user/models/__init__.py
--rw-r--r--   0 ibrahima   (502) staff       (20)    11746 2023-08-11 06:09:54.000000 adafri-0.0.87/adafri/v1/user/models/user.py
--rw-r--r--   0 ibrahima   (502) staff       (20)     7620 2023-08-11 06:09:31.000000 adafri-0.0.87/adafri/v1/user/models/user_fields.py
-drwxr-xr-x   0 ibrahima   (502) staff       (20)        0 2023-08-12 00:43:17.076260 adafri-0.0.87/adafri.egg-info/
--rw-r--r--   0 ibrahima   (502) staff       (20)      177 2023-08-12 00:43:16.000000 adafri-0.0.87/adafri.egg-info/PKG-INFO
--rw-r--r--   0 ibrahima   (502) staff       (20)     1329 2023-08-12 00:43:17.000000 adafri-0.0.87/adafri.egg-info/SOURCES.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)        1 2023-08-12 00:43:16.000000 adafri-0.0.87/adafri.egg-info/dependency_links.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)        7 2023-08-12 00:43:16.000000 adafri-0.0.87/adafri.egg-info/top_level.txt
--rw-r--r--   0 ibrahima   (502) staff       (20)       38 2023-08-12 00:43:17.111585 adafri-0.0.87/setup.cfg
--rw-r--r--   0 ibrahima   (502) staff       (20)      684 2023-07-16 01:48:05.000000 adafri-0.0.87/setup.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-05-23 20:39:44.392323 adafri-0.0.88/
+-rw-r--r--   0 admin      (501) staff       (20)      177 2024-05-23 20:39:44.392194 adafri-0.0.88/PKG-INFO
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-05-23 20:39:44.381166 adafri-0.0.88/adafri/
+-rw-r--r--   0 admin      (501) staff       (20)       80 2024-05-23 20:37:23.000000 adafri-0.0.88/adafri/__init__.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-05-23 20:39:44.382945 adafri-0.0.88/adafri/utils/
+-rw-r--r--   0 admin      (501) staff       (20)      101 2024-05-23 20:22:22.000000 adafri-0.0.88/adafri/utils/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)     1254 2024-05-23 20:32:22.000000 adafri-0.0.88/adafri/utils/country.py
+-rw-r--r--   0 admin      (501) staff       (20)     2519 2024-05-23 20:22:22.000000 adafri-0.0.88/adafri/utils/phone_number.py
+-rw-r--r--   0 admin      (501) staff       (20)     1356 2024-05-23 20:22:22.000000 adafri-0.0.88/adafri/utils/response.py
+-rw-r--r--   0 admin      (501) staff       (20)    19215 2024-05-23 20:22:22.000000 adafri-0.0.88/adafri/utils/utils.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-05-23 20:39:44.383350 adafri-0.0.88/adafri/v1/
+-rw-r--r--   0 admin      (501) staff       (20)       93 2024-05-23 20:22:22.000000 adafri-0.0.88/adafri/v1/__init__.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-05-23 20:39:44.383602 adafri-0.0.88/adafri/v1/account/
+-rw-r--r--   0 admin      (501) staff       (20)      151 2024-05-23 20:22:22.000000 adafri-0.0.88/adafri/v1/account/__init__.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-05-23 20:39:44.385036 adafri-0.0.88/adafri/v1/account/models/
+-rw-r--r--   0 admin      (501) staff       (20)       91 2024-05-23 20:22:22.000000 adafri-0.0.88/adafri/v1/account/models/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)     4514 2024-05-23 20:22:22.000000 adafri-0.0.88/adafri/v1/account/models/account.py
+-rw-r--r--   0 admin      (501) staff       (20)     3852 2024-05-23 20:22:22.000000 adafri-0.0.88/adafri/v1/account/models/account_fields.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-05-23 20:39:44.385313 adafri-0.0.88/adafri/v1/auth/
+-rw-r--r--   0 admin      (501) staff       (20)      249 2024-05-23 20:22:22.000000 adafri-0.0.88/adafri/v1/auth/__init__.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-05-23 20:39:44.385780 adafri-0.0.88/adafri/v1/auth/firebase_auth/
+-rw-r--r--   0 admin      (501) staff       (20)      316 2024-05-23 20:22:22.000000 adafri-0.0.88/adafri/v1/auth/firebase_auth/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)     5059 2024-05-23 20:22:22.000000 adafri-0.0.88/adafri/v1/auth/firebase_auth/firebase_auth.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-05-23 20:39:44.386114 adafri-0.0.88/adafri/v1/auth/models/
+-rw-r--r--   0 admin      (501) staff       (20)        0 2024-05-23 20:22:22.000000 adafri-0.0.88/adafri/v1/auth/models/__init__.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-05-23 20:39:44.386224 adafri-0.0.88/adafri/v1/auth/oauth/
+-rw-r--r--   0 admin      (501) staff       (20)      965 2024-05-23 20:22:22.000000 adafri-0.0.88/adafri/v1/auth/oauth/__init__.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-05-23 20:39:44.389570 adafri-0.0.88/adafri/v1/auth/oauth/models/
+-rw-r--r--   0 admin      (501) staff       (20)       93 2024-05-23 20:22:22.000000 adafri-0.0.88/adafri/v1/auth/oauth/models/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)     7216 2024-05-23 20:22:22.000000 adafri-0.0.88/adafri/v1/auth/oauth/models/client.py
+-rw-r--r--   0 admin      (501) staff       (20)     5478 2024-05-23 20:22:22.000000 adafri-0.0.88/adafri/v1/auth/oauth/models/client_fields.py
+-rw-r--r--   0 admin      (501) staff       (20)     6646 2024-05-23 20:22:22.000000 adafri-0.0.88/adafri/v1/auth/oauth/models/code.py
+-rw-r--r--   0 admin      (501) staff       (20)     2505 2024-05-23 20:22:22.000000 adafri-0.0.88/adafri/v1/auth/oauth/models/code_fields.py
+-rw-r--r--   0 admin      (501) staff       (20)    16152 2024-05-23 20:22:22.000000 adafri-0.0.88/adafri/v1/auth/oauth/models/grant.py
+-rw-r--r--   0 admin      (501) staff       (20)     3653 2024-05-23 20:22:22.000000 adafri-0.0.88/adafri/v1/auth/oauth/models/grant_fields.py
+-rw-r--r--   0 admin      (501) staff       (20)     9460 2024-05-23 20:22:22.000000 adafri-0.0.88/adafri/v1/auth/oauth/models/token.py
+-rw-r--r--   0 admin      (501) staff       (20)     3728 2024-05-23 20:22:22.000000 adafri-0.0.88/adafri/v1/auth/oauth/models/token_fields.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-05-23 20:39:44.390274 adafri-0.0.88/adafri/v1/auth/oauth/server/
+-rw-r--r--   0 admin      (501) staff       (20)      163 2024-05-23 20:22:22.000000 adafri-0.0.88/adafri/v1/auth/oauth/server/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)     1574 2024-05-23 20:22:22.000000 adafri-0.0.88/adafri/v1/auth/oauth/server/oidc_server.py
+-rw-r--r--   0 admin      (501) staff       (20)     2685 2024-05-23 20:22:22.000000 adafri-0.0.88/adafri/v1/auth/oauth/server/server.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-05-23 20:39:44.390698 adafri-0.0.88/adafri/v1/base/
+-rw-r--r--   0 admin      (501) staff       (20)       71 2024-05-23 20:22:22.000000 adafri-0.0.88/adafri/v1/base/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)     4240 2024-05-23 20:22:22.000000 adafri-0.0.88/adafri/v1/base/firebase_collection.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-05-23 20:39:44.390854 adafri-0.0.88/adafri/v1/mailing/
+-rw-r--r--   0 admin      (501) staff       (20)    13843 2024-05-23 20:22:22.000000 adafri-0.0.88/adafri/v1/mailing/__init__.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-05-23 20:39:44.391181 adafri-0.0.88/adafri/v1/user/
+-rw-r--r--   0 admin      (501) staff       (20)      129 2024-05-23 20:22:22.000000 adafri-0.0.88/adafri/v1/user/__init__.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-05-23 20:39:44.391965 adafri-0.0.88/adafri/v1/user/models/
+-rw-r--r--   0 admin      (501) staff       (20)       78 2024-05-23 20:22:22.000000 adafri-0.0.88/adafri/v1/user/models/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)    11746 2024-05-23 20:22:22.000000 adafri-0.0.88/adafri/v1/user/models/user.py
+-rw-r--r--   0 admin      (501) staff       (20)     7620 2024-05-23 20:22:22.000000 adafri-0.0.88/adafri/v1/user/models/user_fields.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2024-05-23 20:39:44.381678 adafri-0.0.88/adafri.egg-info/
+-rw-r--r--   0 admin      (501) staff       (20)      177 2024-05-23 20:39:44.000000 adafri-0.0.88/adafri.egg-info/PKG-INFO
+-rw-r--r--   0 admin      (501) staff       (20)     1329 2024-05-23 20:39:44.000000 adafri-0.0.88/adafri.egg-info/SOURCES.txt
+-rw-r--r--   0 admin      (501) staff       (20)        1 2024-05-23 20:39:44.000000 adafri-0.0.88/adafri.egg-info/dependency_links.txt
+-rw-r--r--   0 admin      (501) staff       (20)        7 2024-05-23 20:39:44.000000 adafri-0.0.88/adafri.egg-info/top_level.txt
+-rw-r--r--   0 admin      (501) staff       (20)       38 2024-05-23 20:39:44.392371 adafri-0.0.88/setup.cfg
+-rw-r--r--   0 admin      (501) staff       (20)      684 2024-05-23 20:22:22.000000 adafri-0.0.88/setup.py
```

### Comparing `adafri-0.0.87/adafri/utils/country.py` & `adafri-0.0.88/adafri/utils/country.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import gettext
 
 class Country(object):
     def __init__(self, locales=['fr']):
         self.locales = locales;
     
     def get_countries(self):
-        lang =  gettext.translation('iso3166', pycountry.LOCALES_DIR, languages=self.locales);
+        lang =  gettext.translation('iso3166-1', pycountry.LOCALES_DIR, languages=self.locales);
         lang.install()
         countries_list = list(pycountry.countries)
         countries = []
         for c in countries_list:
             country = self.get_country(country=c)
             countries.append(country)
         return countries;
```

### Comparing `adafri-0.0.87/adafri/utils/phone_number.py` & `adafri-0.0.88/adafri/utils/phone_number.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.87/adafri/utils/response.py` & `adafri-0.0.88/adafri/utils/response.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.87/adafri/utils/utils.py` & `adafri-0.0.88/adafri/utils/utils.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.87/adafri/v1/account/models/account.py` & `adafri-0.0.88/adafri/v1/account/models/account.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.87/adafri/v1/account/models/account_fields.py` & `adafri-0.0.88/adafri/v1/account/models/account_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.87/adafri/v1/auth/firebase_auth/firebase_auth.py` & `adafri-0.0.88/adafri/v1/auth/firebase_auth/firebase_auth.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.87/adafri/v1/auth/oauth/__init__.py` & `adafri-0.0.88/adafri/v1/auth/oauth/__init__.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.87/adafri/v1/auth/oauth/models/client.py` & `adafri-0.0.88/adafri/v1/auth/oauth/models/client.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.87/adafri/v1/auth/oauth/models/client_fields.py` & `adafri-0.0.88/adafri/v1/auth/oauth/models/client_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.87/adafri/v1/auth/oauth/models/code.py` & `adafri-0.0.88/adafri/v1/auth/oauth/models/code.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.87/adafri/v1/auth/oauth/models/code_fields.py` & `adafri-0.0.88/adafri/v1/auth/oauth/models/code_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.87/adafri/v1/auth/oauth/models/grant.py` & `adafri-0.0.88/adafri/v1/auth/oauth/models/grant.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.87/adafri/v1/auth/oauth/models/grant_fields.py` & `adafri-0.0.88/adafri/v1/auth/oauth/models/grant_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.87/adafri/v1/auth/oauth/models/token.py` & `adafri-0.0.88/adafri/v1/auth/oauth/models/token.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.87/adafri/v1/auth/oauth/models/token_fields.py` & `adafri-0.0.88/adafri/v1/auth/oauth/models/token_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.87/adafri/v1/auth/oauth/server/oidc_server.py` & `adafri-0.0.88/adafri/v1/auth/oauth/server/oidc_server.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.87/adafri/v1/auth/oauth/server/server.py` & `adafri-0.0.88/adafri/v1/auth/oauth/server/server.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.87/adafri/v1/base/firebase_collection.py` & `adafri-0.0.88/adafri/v1/base/firebase_collection.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.87/adafri/v1/mailing/__init__.py` & `adafri-0.0.88/adafri/v1/mailing/__init__.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.87/adafri/v1/user/models/user.py` & `adafri-0.0.88/adafri/v1/user/models/user.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.87/adafri/v1/user/models/user_fields.py` & `adafri-0.0.88/adafri/v1/user/models/user_fields.py`

 * *Files identical despite different names*

### Comparing `adafri-0.0.87/adafri.egg-info/SOURCES.txt` & `adafri-0.0.88/adafri.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafri-0.0.87/setup.py` & `adafri-0.0.88/setup.py`

 * *Files identical despite different names*

