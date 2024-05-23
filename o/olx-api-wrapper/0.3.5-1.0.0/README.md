# Comparing `tmp/olx-api-wrapper-0.3.5.tar.gz` & `tmp/olx-api-wrapper-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "olx-api-wrapper-0.3.5.tar", last modified: Wed May 22 11:36:34 2024, max compression
+gzip compressed data, was "olx-api-wrapper-1.0.0.tar", last modified: Thu May 23 13:32:50 2024, max compression
```

## Comparing `olx-api-wrapper-0.3.5.tar` & `olx-api-wrapper-1.0.0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:36:34.835610 olx-api-wrapper-0.3.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-22 11:36:26.000000 olx-api-wrapper-0.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11100 2024-05-22 11:36:34.835610 olx-api-wrapper-0.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10616 2024-05-22 11:36:26.000000 olx-api-wrapper-0.3.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:36:34.831610 olx-api-wrapper-0.3.5/olx/
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-22 11:36:26.000000 olx-api-wrapper-0.3.5/olx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:36:34.831610 olx-api-wrapper-0.3.5/olx/partner/
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-22 11:36:26.000000 olx-api-wrapper-0.3.5/olx/partner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-22 11:36:26.000000 olx-api-wrapper-0.3.5/olx/partner/advert_logo.py
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-22 11:36:26.000000 olx-api-wrapper-0.3.5/olx/partner/advert_statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)     4326 2024-05-22 11:36:26.000000 olx-api-wrapper-0.3.5/olx/partner/adverts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-05-22 11:36:26.000000 olx-api-wrapper-0.3.5/olx/partner/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-22 11:36:26.000000 olx-api-wrapper-0.3.5/olx/partner/categories_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-05-22 11:36:26.000000 olx-api-wrapper-0.3.5/olx/partner/cities_districts.py
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-22 11:36:26.000000 olx-api-wrapper-0.3.5/olx/partner/languages_currencies.py
--rw-r--r--   0 runner    (1001) docker     (127)     5055 2024-05-22 11:36:26.000000 olx-api-wrapper-0.3.5/olx/partner/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     5892 2024-05-22 11:36:26.000000 olx-api-wrapper-0.3.5/olx/partner/olx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-22 11:36:26.000000 olx-api-wrapper-0.3.5/olx/partner/paid_features.py
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-22 11:36:26.000000 olx-api-wrapper-0.3.5/olx/partner/payments.py
--rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-05-22 11:36:26.000000 olx-api-wrapper-0.3.5/olx/partner/threads_messages.py
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-22 11:36:26.000000 olx-api-wrapper-0.3.5/olx/partner/user_business.py
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-05-22 11:36:26.000000 olx-api-wrapper-0.3.5/olx/partner/users.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:36:34.831610 olx-api-wrapper-0.3.5/olx/public/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 11:36:26.000000 olx-api-wrapper-0.3.5/olx/public/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-05-22 11:36:26.000000 olx-api-wrapper-0.3.5/olx/public/checkout.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:36:34.831610 olx-api-wrapper-0.3.5/olx/public/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 11:36:26.000000 olx-api-wrapper-0.3.5/olx/public/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:36:34.831610 olx-api-wrapper-0.3.5/olx/public/models/offers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 11:36:26.000000 olx-api-wrapper-0.3.5/olx/public/models/offers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-22 11:36:26.000000 olx-api-wrapper-0.3.5/olx/public/models/offers/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-22 11:36:26.000000 olx-api-wrapper-0.3.5/olx/public/models/offers/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     4408 2024-05-22 11:36:26.000000 olx-api-wrapper-0.3.5/olx/public/models/offers/offers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:36:34.835610 olx-api-wrapper-0.3.5/olx/public/models/seo/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 11:36:26.000000 olx-api-wrapper-0.3.5/olx/public/models/seo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-22 11:36:26.000000 olx-api-wrapper-0.3.5/olx/public/models/seo/offers.py
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-22 11:36:26.000000 olx-api-wrapper-0.3.5/olx/public/models/seo/popular_searches.py
--rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-05-22 11:36:26.000000 olx-api-wrapper-0.3.5/olx/public/offers.py
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-22 11:36:26.000000 olx-api-wrapper-0.3.5/olx/public/olx_public.py
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-22 11:36:26.000000 olx-api-wrapper-0.3.5/olx/public/seo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:36:34.835610 olx-api-wrapper-0.3.5/olx_api_wrapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11100 2024-05-22 11:36:34.000000 olx-api-wrapper-0.3.5/olx_api_wrapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-05-22 11:36:34.000000 olx-api-wrapper-0.3.5/olx_api_wrapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 11:36:34.000000 olx-api-wrapper-0.3.5/olx_api_wrapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-22 11:36:34.000000 olx-api-wrapper-0.3.5/olx_api_wrapper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-22 11:36:34.000000 olx-api-wrapper-0.3.5/olx_api_wrapper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 11:36:34.835610 olx-api-wrapper-0.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-22 11:36:26.000000 olx-api-wrapper-0.3.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:36:34.835610 olx-api-wrapper-0.3.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 11:36:26.000000 olx-api-wrapper-0.3.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7746 2024-05-22 11:36:26.000000 olx-api-wrapper-0.3.5/tests/test_cities_and_districts.py
--rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-05-22 11:36:26.000000 olx-api-wrapper-0.3.5/tests/test_users.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:32:50.315342 olx-api-wrapper-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-23 13:32:43.000000 olx-api-wrapper-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11100 2024-05-23 13:32:50.315342 olx-api-wrapper-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10616 2024-05-23 13:32:43.000000 olx-api-wrapper-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:32:50.311342 olx-api-wrapper-1.0.0/olx/
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-23 13:32:43.000000 olx-api-wrapper-1.0.0/olx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:32:50.311342 olx-api-wrapper-1.0.0/olx/partner/
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-23 13:32:43.000000 olx-api-wrapper-1.0.0/olx/partner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-23 13:32:43.000000 olx-api-wrapper-1.0.0/olx/partner/advert_logo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-23 13:32:43.000000 olx-api-wrapper-1.0.0/olx/partner/advert_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4307 2024-05-23 13:32:43.000000 olx-api-wrapper-1.0.0/olx/partner/adverts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-05-23 13:32:43.000000 olx-api-wrapper-1.0.0/olx/partner/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-05-23 13:32:43.000000 olx-api-wrapper-1.0.0/olx/partner/categories_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-05-23 13:32:43.000000 olx-api-wrapper-1.0.0/olx/partner/cities_districts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-23 13:32:43.000000 olx-api-wrapper-1.0.0/olx/partner/languages_currencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5185 2024-05-23 13:32:43.000000 olx-api-wrapper-1.0.0/olx/partner/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8098 2024-05-23 13:32:43.000000 olx-api-wrapper-1.0.0/olx/partner/olx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-23 13:32:43.000000 olx-api-wrapper-1.0.0/olx/partner/paid_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-05-23 13:32:43.000000 olx-api-wrapper-1.0.0/olx/partner/payments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-05-23 13:32:43.000000 olx-api-wrapper-1.0.0/olx/partner/threads_messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-23 13:32:43.000000 olx-api-wrapper-1.0.0/olx/partner/user_business.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-05-23 13:32:43.000000 olx-api-wrapper-1.0.0/olx/partner/users.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:32:50.311342 olx-api-wrapper-1.0.0/olx/public/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 13:32:43.000000 olx-api-wrapper-1.0.0/olx/public/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-05-23 13:32:43.000000 olx-api-wrapper-1.0.0/olx/public/checkout.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:32:50.311342 olx-api-wrapper-1.0.0/olx/public/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 13:32:43.000000 olx-api-wrapper-1.0.0/olx/public/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:32:50.315342 olx-api-wrapper-1.0.0/olx/public/models/offers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 13:32:43.000000 olx-api-wrapper-1.0.0/olx/public/models/offers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-23 13:32:43.000000 olx-api-wrapper-1.0.0/olx/public/models/offers/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-23 13:32:43.000000 olx-api-wrapper-1.0.0/olx/public/models/offers/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4408 2024-05-23 13:32:43.000000 olx-api-wrapper-1.0.0/olx/public/models/offers/offers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:32:50.315342 olx-api-wrapper-1.0.0/olx/public/models/seo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 13:32:43.000000 olx-api-wrapper-1.0.0/olx/public/models/seo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-23 13:32:43.000000 olx-api-wrapper-1.0.0/olx/public/models/seo/offers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-23 13:32:43.000000 olx-api-wrapper-1.0.0/olx/public/models/seo/popular_searches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-05-23 13:32:43.000000 olx-api-wrapper-1.0.0/olx/public/offers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-23 13:32:43.000000 olx-api-wrapper-1.0.0/olx/public/olx_public.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-23 13:32:43.000000 olx-api-wrapper-1.0.0/olx/public/seo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:32:50.315342 olx-api-wrapper-1.0.0/olx_api_wrapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11100 2024-05-23 13:32:50.000000 olx-api-wrapper-1.0.0/olx_api_wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-05-23 13:32:50.000000 olx-api-wrapper-1.0.0/olx_api_wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-23 13:32:50.000000 olx-api-wrapper-1.0.0/olx_api_wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-23 13:32:50.000000 olx-api-wrapper-1.0.0/olx_api_wrapper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-23 13:32:50.000000 olx-api-wrapper-1.0.0/olx_api_wrapper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-23 13:32:50.315342 olx-api-wrapper-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-23 13:32:43.000000 olx-api-wrapper-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-23 13:32:50.315342 olx-api-wrapper-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-23 13:32:43.000000 olx-api-wrapper-1.0.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7746 2024-05-23 13:32:43.000000 olx-api-wrapper-1.0.0/tests/test_cities_and_districts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-05-23 13:32:43.000000 olx-api-wrapper-1.0.0/tests/test_users.py
```

### Comparing `olx-api-wrapper-0.3.5/LICENSE` & `olx-api-wrapper-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `olx-api-wrapper-0.3.5/PKG-INFO` & `olx-api-wrapper-1.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: olx-api-wrapper
-Version: 0.3.5
+Version: 1.0.0
 Summary: Unofficial Wrapper for OLX API
 Home-page: https://github.com/Pawikoski/olx-api-wrapper
 Author: Paweł Stawikowski
 Author-email: pawikoski@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.11
@@ -113,15 +113,15 @@
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 
 
 <!-- GETTING STARTED -->
 ## Getting Started
 
-In order to use OLX Api you nned to sign in at OLX Developer Portal and create an App.
+In order to use OLX Api you need to sign in at OLX Developer Portal and create an App.
 More details: https://developer.olx.pl/articles/getting-access-to-api
 
 ### Prerequisites
 
 To use this API Wrapper you need to copy Client ID and Client Secret. Store them in the safe place. In your code you can use them as enviroment variables, they sholdn't be hardcoded.
 You can perform actions with API on:
 - OLX PL
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: olx-api-wrapper Version: 0.3.5 Summary: Unofficial
+Metadata-Version: 2.1 Name: olx-api-wrapper Version: 1.0.0 Summary: Unofficial
 Wrapper for OLX API Home-page: https://github.com/Pawikoski/olx-api-wrapper
 Author: PaweÅ Stawikowski Author-email: pawikoski@gmail.com License: MIT
 Classifier: Development Status :: 4 - Beta Classifier: Programming Language ::
 Python :: 3.11 Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Description-Content-Type: text/markdown
 License-File: LICENSE [![Contributors][contributors-shield]][contributors-url]
 [![Forks][forks-shield]][forks-url] [![Stargazers][stars-shield]][stars-url] [!
@@ -30,15 +30,15 @@
 this Python library you can quickly fetch user data, handle adverts with simple
 CRUD operations, and seamlessly integrate with the OLX API. Simplify your
 development process and focus on building your app hassle-free.
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ### Built With * [![Python][Python]][Python-url] * [![requests][requests]]
 [requests-url] * [![dacite][dacite]][dacite-url]
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
-## Getting Started In order to use OLX Api you nned to sign in at OLX Developer
+## Getting Started In order to use OLX Api you need to sign in at OLX Developer
 Portal and create an App. More details: https://developer.olx.pl/articles/
 getting-access-to-api ### Prerequisites To use this API Wrapper you need to
 copy Client ID and Client Secret. Store them in the safe place. In your code
 you can use them as enviroment variables, they sholdn't be hardcoded. You can
 perform actions with API on: - OLX PL - OLX BG - OLX RO - OLX PT - OLX UA - OLX
 KZ By default, all requests are sent to olx.**PL**. To change it you must pass
 `country_code` argument to every child of Olx class, i.e.: ```python
```

### Comparing `olx-api-wrapper-0.3.5/README.md` & `olx-api-wrapper-1.0.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -98,15 +98,15 @@
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 
 
 <!-- GETTING STARTED -->
 ## Getting Started
 
-In order to use OLX Api you nned to sign in at OLX Developer Portal and create an App.
+In order to use OLX Api you need to sign in at OLX Developer Portal and create an App.
 More details: https://developer.olx.pl/articles/getting-access-to-api
 
 ### Prerequisites
 
 To use this API Wrapper you need to copy Client ID and Client Secret. Store them in the safe place. In your code you can use them as enviroment variables, they sholdn't be hardcoded.
 You can perform actions with API on:
 - OLX PL
```

#### html2text {}

```diff
@@ -24,15 +24,15 @@
 this Python library you can quickly fetch user data, handle adverts with simple
 CRUD operations, and seamlessly integrate with the OLX API. Simplify your
 development process and focus on building your app hassle-free.
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ### Built With * [![Python][Python]][Python-url] * [![requests][requests]]
 [requests-url] * [![dacite][dacite]][dacite-url]
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
-## Getting Started In order to use OLX Api you nned to sign in at OLX Developer
+## Getting Started In order to use OLX Api you need to sign in at OLX Developer
 Portal and create an App. More details: https://developer.olx.pl/articles/
 getting-access-to-api ### Prerequisites To use this API Wrapper you need to
 copy Client ID and Client Secret. Store them in the safe place. In your code
 you can use them as enviroment variables, they sholdn't be hardcoded. You can
 perform actions with API on: - OLX PL - OLX BG - OLX RO - OLX PT - OLX UA - OLX
 KZ By default, all requests are sent to olx.**PL**. To change it you must pass
 `country_code` argument to every child of Olx class, i.e.: ```python
```

### Comparing `olx-api-wrapper-0.3.5/olx/partner/advert_logo.py` & `olx-api-wrapper-1.0.0/olx/partner/advert_logo.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 from .olx import Olx
 from .models import AdvertLogoType
-from dacite import from_dict
 from typing import List
 
 
 class AdvertLogo(Olx):
     def __init__(self, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
 
     def get_advert_logos(self, advert_id: int) -> List[AdvertLogoType]:
         endpoint = self.endpoints["advert_logo"]["get_advert_logos"].format(
             id=advert_id
         )
-        response = self.get(endpoint)
-        data = response.json()["data"]
-        return [from_dict(AdvertLogoType, obj) for obj in data]
+        response = self._get(endpoint)
+        return self._process_response(
+            AdvertLogoType, response, "data", return_list=True
+        )
 
     def add_logo(self, advert_id: int, url: str) -> AdvertLogoType:
         endpoint = self.endpoints["advert_logo"]["add_logo"].format(id=advert_id)
         payload = {"url": url}
-        response = self.post(endpoint, json=payload)
-        data = response.json()
-        return from_dict(AdvertLogo, data)
+        response = self._post(endpoint, json=payload)
+        return self._process_response(AdvertLogo, response)
 
     def delete_logo(self, advert_id: int, logo_id: int):
         endpoint = self.endpoints["advert_logo"]["delete_logo"].format(
             id=advert_id, logo_id=logo_id
         )
-        self.delete(endpoint, wanted_status=204)
+        self._delete(endpoint, wanted_status=204)
+
+        # TODO: return
```

### Comparing `olx-api-wrapper-0.3.5/olx/partner/advert_statistics.py` & `olx-api-wrapper-1.0.0/olx/partner/advert_statistics.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 from .olx import Olx
 from .models import AdvertStatistic
-from dacite import from_dict
 from typing import Literal
 
 
 class AdvertsStatistics(Olx):
     def __init__(self, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
 
     def get_advert_statistics(self, advert_id: int) -> AdvertStatistic:
         endpoint = self.endpoints["advert_statistics"]["get_advert_statistics"].format(
             id=advert_id
         )
-        response = self.get(endpoint)
-        data = response.json()["data"]
-        return from_dict(AdvertStatistic, data)
+        response = self._get(endpoint)
+        return self._process_response(AdvertStatistic, response, "data")
 
     def clear_statistics(
         self, advert_id: int, statistic_name: Literal["phone-views", "advert-views"]
     ) -> None:
         endpoint = self.endpoints["advert_statistics"]["clear_statistics"].format(
             id=advert_id, statistic_name=statistic_name
         )
-        self.delete(endpoint, wanted_status=204)
+        self._delete(endpoint, wanted_status=204)
+        # TODO: return
```

### Comparing `olx-api-wrapper-0.3.5/olx/partner/adverts.py` & `olx-api-wrapper-1.0.0/olx/partner/adverts.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from .olx import Olx
 from .models import Advert
-from dacite import from_dict
 from typing import List, Literal
 
 
 class Adverts(Olx):
     def __init__(self, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
 
@@ -24,17 +23,16 @@
             params["limit"] = limit
         params = dict()
         if external_id:
             params["external_id"] = external_id
         params = dict()
         if category_ids:
             params["category_ids"] = category_ids
-        response = self.get(endpoint, params=params)
-        data = response.json()["data"]
-        return [from_dict(Advert, obj) for obj in data]
+        response = self._get(endpoint, params=params)
+        return self._process_response(Advert, response, "data", return_list=True)
 
     def build_payload_for_create_or_update(
         self,
         title: str,
         description: str,
         category_id: str,
         advertiser_type: Literal["private", "business"],
@@ -70,48 +68,49 @@
             payload["courier"] = courier
 
         return payload
 
     def create_advert(self, *args, **kwargs) -> Advert:
         endpoint = self.endpoints["adverts"]["create_advert"]
         payload = self.build_payload_for_create_or_update(*args, **kwargs)
-        response = self.post(endpoint, json=payload)
-        return from_dict(Advert, response.json())
+        response = self._post(endpoint, json=payload)
+        return self._process_response(Advert, response)
 
     def get_advert(self, advert_id) -> Advert:
         endpoint = self.endpoints["adverts"]["get_advert"].format(id=advert_id)
-        response = self.get(endpoint)
-        data = response.json()["data"]
-        return from_dict(Advert, data)
+        response = self._get(endpoint)
+        return self._process_response(Advert, response)
 
     def update_advert(self, advert_id, *args, **kwargs) -> Advert:
         endpoint = self.endpoints["adverts"]["update_advert"].format(id=advert_id)
         payload = self.build_payload_for_create_or_update(*args, **kwargs)
-        response = self.put(endpoint, json=payload)
-        data = response.json()["data"]
-        return from_dict(Advert, data)
+        response = self._put(endpoint, json=payload)
+        return self._process_response(Advert, response, "data")
 
     def delete_advert(self, advert_id: int) -> None:
         endpoint = self.endpoints["adverts"]["delete_advert"].format(id=advert_id)
-        self.delete(endpoint, wanted_status=204)
+        self._delete(endpoint, wanted_status=204)
+        # TODO: return
 
     def take_action_on_advert(
         self,
         advert_id: int,
         command: Literal["activate", "deactivate", "finish", "refresh"],
         is_success: bool = None,
     ):
         endpoint = self.endpoints["adverts"]["take_action_on_advert"].format(
             id=advert_id
         )
         payload = {"command": command}
         if command == "deactivate":
             assert is_success is not None
             payload["is_success"] = is_success
-        self.post(endpoint, json=payload, wanted_status=204)
+        self._post(endpoint, json=payload, wanted_status=204)
+
+        # TODO: return
 
     def activate_advert(self, advert_id: int):
         return self.take_action_on_advert(advert_id, "activate")
 
     def deactivate_advert(self, advert_id: int, is_success: bool):
         return self.take_action_on_advert(advert_id, "deactivate", is_success)
```

### Comparing `olx-api-wrapper-0.3.5/olx/partner/auth.py` & `olx-api-wrapper-1.0.0/olx/partner/auth.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import requests
+from .models import AuthResponse, ErrorResponse
 from .olx import Olx
-from dacite import from_dict
-from .models import AuthResponse
 
 
 class Auth(Olx):
     def __init__(self, client_id, client_secret, custom_scope=None) -> None:
         super().__init__()
         self.client_id = client_id
         self.client_secret = client_secret
@@ -21,19 +20,21 @@
 
     @access_token.setter
     def access_token(self, acces_token: str):
         self._access_token = acces_token
 
     def process_auth(self, request_data: dict) -> AuthResponse:
         endpoint = self.endpoints["auth"]
-        response = requests.post(self.url + endpoint, json=request_data)
-
-        # TODO: Handle errors
-
-        data = from_dict(AuthResponse, response.json())
+        response = requests.post(
+            self.url + endpoint, json=request_data, headers=self.headers
+        )
+
+        data = self._process_response(AuthResponse, response.json())
+        if type(data) is ErrorResponse:
+            return data
 
         self.access_token = data.access_token
         self.expires_in = data.expires_in
 
         return data
 
     def authenticate(self, code: str = None) -> AuthResponse:
```

### Comparing `olx-api-wrapper-0.3.5/olx/partner/categories_attributes.py` & `olx-api-wrapper-1.0.0/olx/partner/categories_attributes.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,41 +1,40 @@
 from .olx import Olx
 from .models import Category, CategoryAttribute, CategorySuggestion
-from dacite import from_dict
 from typing import List
 
 
 class CategoriesAttributes(Olx):
     def __init__(self, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
 
     def get_categories(self, parent_id: int = None) -> List[Category]:
         endpoint = self.endpoints["categories_attributes"]["get_categories"]
         params = dict()
         if parent_id:
             params["parent_id"] = parent_id
-        response = self.get(endpoint, params=params)
-        data = response.json()["data"]
-        return [from_dict(Category, obj) for obj in data]
+        response = self._get(endpoint, params=params)
+        return self._process_response(Category, response, "data", return_list=True)
 
     def get_category(self, category_id: int) -> Category:
         endpoint = self.endpoints["categories_attributes"]["get_category"].format(
             id=category_id
         )
-        response = self.get(endpoint)
-        data = response.json()["data"]
-        return from_dict(Category, data)
+        response = self._get(endpoint)
+        return self._process_response(Category, response, "data")
 
     def get_category_attributes(self, category_id: int) -> List[CategoryAttribute]:
         endpoint = self.endpoints["categories_attributes"][
             "get_category_attributes"
         ].format(id=category_id)
-        response = self.get(endpoint)
-        data = response.json()["data"]
-        return [from_dict(CategoryAttribute, obj) for obj in data]
+        response = self._get(endpoint)
+        return self._process_response(
+            CategoryAttribute, response, "data", return_list=True
+        )
 
     def get_category_suggestions(self, ad_title: str) -> List[CategorySuggestion]:
         endpoint = self.endpoints["categories_attributes"]["get_category_suggestions"]
         params = {"q": ad_title}
-        response = self.get(endpoint, params=params)
-        data = response.json()["data"]
-        return [from_dict(CategorySuggestion, obj) for obj in data]
+        response = self._get(endpoint, params=params)
+        return self._process_response(
+            CategorySuggestion, response, "data", return_list=True
+        )
```

### Comparing `olx-api-wrapper-0.3.5/olx/partner/cities_districts.py` & `olx-api-wrapper-1.0.0/olx/partner/cities_districts.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,64 +6,61 @@
 
 class CitiesDistricts(Olx):
     def __init__(self, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
 
     def list_of_country_regions(self) -> List[Region]:
         endpoint = self.endpoints["cities_and_districts"]["list_of_country_regions"]
-        response = self.get(endpoint)
-        data = response.json()["data"]
-        return [from_dict(Region, obj) for obj in data]
+        response = self._get(endpoint)
+        return self._process_response(Region, response, "data", return_list=True)
 
     def get_region(self, region_id: int) -> Region:
         endpoint = self.endpoints["cities_and_districts"]["get_region"].format(
             id=region_id
         )
-        response = self.get(endpoint)
-        data = response.json()["data"]
-        return from_dict(Region, data)
+        response = self._get(endpoint)
+        return self._process_response(Region, response, "data")
 
     def get_cities(self, offset: int = None, limit: int = None) -> List[City]:
         endpoint = self.endpoints["cities_and_districts"]["get_cities"]
         params = dict()
         if offset:
             params["offset"] = offset
         if limit:
             params["limit"] = limit
-        response = self.get(endpoint, params=params)
-        data = response.json()["data"]
-        return [from_dict(City, obj) for obj in data]
+        response = self._get(endpoint, params=params)
+        return self._process_response(City, response, "data", return_list=True)
 
     def get_city(self, city_id: int) -> City:
         endpoint = self.endpoints["cities_and_districts"]["get_city"].format(id=city_id)
-        response = self.get(endpoint)
+        response = self._get(endpoint)
         data = response.json()["data"]
         return from_dict(City, data)
 
     def get_city_districts(self, city_id) -> List[District]:
         endpoint = self.endpoints["cities_and_districts"]["get_city_districts"].format(
             id=city_id
         )
-        response = self.get(endpoint)
+        response = self._get(endpoint)
         data = response.json()["data"]
         return [from_dict(District, obj) for obj in data]
 
     def get_districts(self) -> List[District]:
         endpoint = self.endpoints["cities_and_districts"]["get_districts"]
-        response = self.get(endpoint)
+        response = self._get(endpoint)
         data = response.json()["data"]
         return [from_dict(District, obj) for obj in data]
 
     def get_district(self, district_id) -> District:
         endpoint = self.endpoints["cities_and_districts"]["get_district"].format(
             id=district_id
         )
-        response = self.get(endpoint)
+        response = self._get(endpoint)
         data = response.json()["data"]
         return from_dict(District, data)
 
     def get_locations(self, lat, lon):
         endpoint = self.endpoints["cities_and_districts"]["get_locations"]
         params = {"latitude": lat, "longitude": lon}
-        response = self.get(endpoint, params=params)
+        response = self._get(endpoint, params=params)
         data = response.json()["data"]
         return [from_dict(Location, obj) for obj in data]
```

### Comparing `olx-api-wrapper-0.3.5/olx/partner/languages_currencies.py` & `olx-api-wrapper-1.0.0/olx/partner/languages_currencies.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 from .olx import Olx
 from .models import Language, Currency
-from dacite import from_dict
 from typing import List
 
 
 class LanguagesCurrencies(Olx):
     def __init__(self, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
 
     def get_languages(self) -> List[Language]:
         endpoint = self.endpoints["languages_currencies"]["get_languages"]
-        response = self.get(endpoint)
-        data = response.json()["data"]
-        return [from_dict(Language, obj) for obj in data]
+        response = self._get(endpoint)
+        return self._process_response(Language, response, "data", return_list=True)
 
     def get_currencies(self) -> List[Currency]:
         endpoint = self.endpoints["languages_currencies"]["get_currencies"]
-        response = self.get(endpoint)
-        data = response.json()["data"]
-        return [from_dict(Currency, obj) for obj in data]
+        response = self._get(endpoint)
+        return self._process_response(Currency, response, "data", return_list=True)
```

### Comparing `olx-api-wrapper-0.3.5/olx/partner/models.py` & `olx-api-wrapper-1.0.0/olx/partner/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 from dataclasses import dataclass
 from typing import Any, List, Optional, Literal
 from numbers import Number
 
 
 @dataclass
+class ErrorResponse:
+    error: str | dict
+    error_description: Optional[str]
+    error_human_title: Optional[str]
+
+
+@dataclass
 class AuthResponse:
     access_token: str
     expires_in: int
     token_type: str
     scope: str
     refresh_token: Optional[str]
```

### Comparing `olx-api-wrapper-0.3.5/olx/partner/paid_features.py` & `olx-api-wrapper-1.0.0/olx/partner/paid_features.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 from .olx import Olx
 from .models import PaidFeature, ActivePaidFeature
-from dacite import from_dict
 from typing import List, Literal
 
 
 class PaidFeatures(Olx):
     def __init__(self, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
 
     def get_available_paid_features(self) -> List[PaidFeature]:
         endpoint = self.endpoints["paid_features"]["get_available_paid_features"]
-        response = self.get(endpoint)
-        data = response.json()["data"]
-        return [from_dict(PaidFeature, obj) for obj in data]
+        response = self._get(endpoint)
+        return self._process_response(PaidFeature, response, "data", return_list=True)
 
     def get_active_paid_features(self, advert_id) -> List[ActivePaidFeature]:
         endpoint = self.endpoints["paid_features"]["get_active_paid_features"].format(
             advert_id=advert_id
         )
-        response = self.get(endpoint)
-        data = response.json()["data"]
-        return [from_dict(ActivePaidFeature, obj) for obj in data]
+        response = self._get(endpoint)
+        return self._process_response(
+            ActivePaidFeature, response, "data", return_list=True
+        )
 
     def purchase_paid_feature(
         self, advert_id: int, payment_method: Literal["account", "postpaid"], code: str
     ):
         endpoint = self.endpoints["paid_features"]["purchase_paid_feature"].format(
             id=advert_id
         )
         payload = {"payment_method": payment_method, "code": code}
-        self.post(endpoint, wanted_status=204, json=payload)
+        self._post(endpoint, wanted_status=204, json=payload)
+
+        # TODO: return
```

### Comparing `olx-api-wrapper-0.3.5/olx/partner/payments.py` & `olx-api-wrapper-1.0.0/olx/partner/payments.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 from .olx import Olx
 from .models import Billing, PrepaidInvoice, PostpaidInvoice
-from dacite import from_dict
 from typing import List
 
 
 class Payments(Olx):
     def __init__(self, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
 
     def get_billing(self, page: int = None, limit: int = None) -> List[Billing]:
         endpoint = self.endpoints["payments"]["get_billing"]
         params = dict()
         if page:
             params["page"] = page
         if limit:
             params["limit"] = limit
-        response = self.get(endpoint, params=params)
-        data = response.json()["data"]
-        return [from_dict(Billing, obj) for obj in data]
+        response = self._get(endpoint, params=params)
+        return self._process_response(Billing, response, "data", return_list=True)
 
     def get_prepaid_invoices(
         self, page: int = None, limit: int = None
     ) -> List[PrepaidInvoice]:
         endpoint = self.endpoints["payments"]["get_prepaid_invoices"]
         params = dict()
         if page:
             params["page"] = page
         if limit:
             params["limit"] = limit
-        response = self.get(endpoint, params=params)
-        data = response.json()["data"]
-        return [from_dict(PrepaidInvoice, obj) for obj in data]
+        response = self._get(endpoint, params=params)
+        return self._process_response(
+            PrepaidInvoice, response, "data", return_list=True
+        )
 
     def get_postpaid_invoices(
         self, page: int = None, limit: int = None
     ) -> List[PostpaidInvoice]:
         endpoint = self.endpoints["payments"]["get_postpaid_invoices"]
         params = dict()
         if page:
             params["page"] = page
         if limit:
             params["limit"] = limit
-        response = self.get(endpoint, params=params)
-        data = response.json()["data"]
-        return [from_dict(PostpaidInvoice, obj) for obj in data]
+        response = self._get(endpoint, params=params)
+        return self._process_response(
+            PostpaidInvoice, response, "data", return_list=True
+        )
```

### Comparing `olx-api-wrapper-0.3.5/olx/partner/threads_messages.py` & `olx-api-wrapper-1.0.0/olx/partner/threads_messages.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from .olx import Olx
 from .models import Thread, Message
-from dacite import from_dict
 from typing import List, Literal
 
 
 class ThreadsMessages(Olx):
     def __init__(self, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
 
@@ -22,71 +21,68 @@
         if interlocutor_id:
             params["interlocutor_id"] = interlocutor_id
         if offset:
             params["offset"] = offset
         if limit:
             params["limit"] = limit
 
-        response = self.get(endpoint, params=params)
-        data = response.json()["data"]
-        return [from_dict(Thread, obj) for obj in data]
+        response = self._get(endpoint, params=params)
+        return self._process_response(Thread, response, "data", return_list=True)
 
     def get_thread(self, thread_id) -> Thread:
         endpoint = self.endpoints["threads_messages"]["get_thread"].format(id=thread_id)
-        response = self.get(endpoint)
-        data = response.json()["data"]
-        return from_dict(Thread, data)
+        response = self._get(endpoint)
+        return self._process_response(Thread, response, "data")
 
     def get_messages(
         self, thread_id: int, offset: int = None, limit: int = None
     ) -> List[Message]:
         endpoint = self.endpoints["threads_messages"]["get_messages"].format(
             id=thread_id
         )
         params = dict()
         if offset:
             params["offset"] = offset
         if limit:
             params["limit"] = limit
 
-        response = self.get(endpoint, params=params)
-        data = response.json()["data"]
-        return [from_dict(Message, obj) for obj in data]
+        response = self._get(endpoint, params=params)
+        return self._process_response(Message, response, "data", return_list=True)
 
     def post_message(self, thread_id: int, text: str, attachments: List[str] = None):
         endpoint = self.endpoints["threads_messages"]["post_message"].format(
             id=thread_id
         )
         payload = {"text": text}
         if attachments:
             payload["attachments"] = attachments
-        response = self.post(endpoint, json=payload)
-        data = response.json()["data"]
-        return from_dict(Message, data)
+        response = self._post(endpoint, json=payload)
+        return self._process_response(Message, response, "data")
 
     def get_message(self, thread_id: int, message_id: int):
         endpoint = self.endpoints["threads_messages"]["get_message"].format(
             thread_id=thread_id, message_id=message_id
         )
-        response = self.get(endpoint)
-        data = response.json()["data"]
-        return from_dict(Message, data)
+        response = self._get(endpoint)
+        return self._process_response(Message, response, "data")
 
     def action_on_thread(
         self,
         thread_id: int,
         action: Literal["set-favourite", "mark-as-read"],
         is_favourite: bool = None,
     ):
         endpoint = self.endpoints["threads_messages"]["take_action_on_thread"].format(
             id=thread_id
         )
         payload = {"command": action}
         if action == "set-favourite":
             payload["is_favourite"] = is_favourite
-        self.post(endpoint, json=payload, wanted_status=204)
+        self._post(endpoint, json=payload, wanted_status=204)
+
+        # TODO: return
 
     def mark_thread_as_read(self, thread_id: int):
         return self.action_on_thread(thread_id, "mark-as-read")
 
     def set_favourite(self, thread_id: int, action: bool):
         return self.action_on_thread(thread_id, "set-favourite", is_favourite=action)
```

### Comparing `olx-api-wrapper-0.3.5/olx/partner/users.py` & `olx-api-wrapper-1.0.0/olx/partner/users.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,28 @@
 from .olx import Olx
 from .models import AuthenticatedUser, User, UsersAccountBalance
-from dacite import from_dict
 from typing import List
 
 
 class Users(Olx):
     def __init__(self, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
 
     def get_authenticated_user(self) -> AuthenticatedUser:
         endpoint = self.endpoints["users"]["get_authenticated_user"]
-        response = self.get(endpoint)
-        data = response.json()["data"]
-        return from_dict(AuthenticatedUser, data)
+        response = self._get(endpoint)
+        return self._process_response(AuthenticatedUser, response, "data")
 
     def get_user(self, user_id: int) -> User:
         endpoint = self.endpoints["users"]["get_user"].format(id=user_id)
-        response = self.get(endpoint)
-        data = response.json()["data"]
-        return from_dict(User, data)
+        response = self._get(endpoint)
+        return self._process_response(User, response, "data")
 
     def account_balance(self) -> UsersAccountBalance:
         endpoint = self.endpoints["users"]["account_balance"]
-        response = self.get(endpoint)
-        data = response.json()["data"]
-        return from_dict(UsersAccountBalance, data)
+        response = self._get(endpoint)
+        return self._process_response(UsersAccountBalance, response, "data")
 
     def payment_methods(self) -> List[str]:
         endpoint = self.endpoints["users"]["payment_methods"]
-        response = self.get(endpoint)
-        data = response.json()["data"]
-        return data
+        response = self._get(endpoint)
+        return self._process_response(List[str], response, "data")
```

### Comparing `olx-api-wrapper-0.3.5/olx/public/checkout.py` & `olx-api-wrapper-1.0.0/olx/public/checkout.py`

 * *Files identical despite different names*

### Comparing `olx-api-wrapper-0.3.5/olx/public/models/offers/filters.py` & `olx-api-wrapper-1.0.0/olx/public/models/offers/filters.py`

 * *Files identical despite different names*

### Comparing `olx-api-wrapper-0.3.5/olx/public/models/offers/offers.py` & `olx-api-wrapper-1.0.0/olx/public/models/offers/offers.py`

 * *Files identical despite different names*

### Comparing `olx-api-wrapper-0.3.5/olx/public/offers.py` & `olx-api-wrapper-1.0.0/olx/public/offers.py`

 * *Files identical despite different names*

### Comparing `olx-api-wrapper-0.3.5/olx/public/seo.py` & `olx-api-wrapper-1.0.0/olx/public/seo.py`

 * *Files identical despite different names*

### Comparing `olx-api-wrapper-0.3.5/olx_api_wrapper.egg-info/PKG-INFO` & `olx-api-wrapper-1.0.0/olx_api_wrapper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: olx-api-wrapper
-Version: 0.3.5
+Version: 1.0.0
 Summary: Unofficial Wrapper for OLX API
 Home-page: https://github.com/Pawikoski/olx-api-wrapper
 Author: Paweł Stawikowski
 Author-email: pawikoski@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.11
@@ -113,15 +113,15 @@
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 
 
 <!-- GETTING STARTED -->
 ## Getting Started
 
-In order to use OLX Api you nned to sign in at OLX Developer Portal and create an App.
+In order to use OLX Api you need to sign in at OLX Developer Portal and create an App.
 More details: https://developer.olx.pl/articles/getting-access-to-api
 
 ### Prerequisites
 
 To use this API Wrapper you need to copy Client ID and Client Secret. Store them in the safe place. In your code you can use them as enviroment variables, they sholdn't be hardcoded.
 You can perform actions with API on:
 - OLX PL
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: olx-api-wrapper Version: 0.3.5 Summary: Unofficial
+Metadata-Version: 2.1 Name: olx-api-wrapper Version: 1.0.0 Summary: Unofficial
 Wrapper for OLX API Home-page: https://github.com/Pawikoski/olx-api-wrapper
 Author: PaweÅ Stawikowski Author-email: pawikoski@gmail.com License: MIT
 Classifier: Development Status :: 4 - Beta Classifier: Programming Language ::
 Python :: 3.11 Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Description-Content-Type: text/markdown
 License-File: LICENSE [![Contributors][contributors-shield]][contributors-url]
 [![Forks][forks-shield]][forks-url] [![Stargazers][stars-shield]][stars-url] [!
@@ -30,15 +30,15 @@
 this Python library you can quickly fetch user data, handle adverts with simple
 CRUD operations, and seamlessly integrate with the OLX API. Simplify your
 development process and focus on building your app hassle-free.
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
 ### Built With * [![Python][Python]][Python-url] * [![requests][requests]]
 [requests-url] * [![dacite][dacite]][dacite-url]
                                                                   (_b_a_c_k_ _t_o_ _t_o_p)
-## Getting Started In order to use OLX Api you nned to sign in at OLX Developer
+## Getting Started In order to use OLX Api you need to sign in at OLX Developer
 Portal and create an App. More details: https://developer.olx.pl/articles/
 getting-access-to-api ### Prerequisites To use this API Wrapper you need to
 copy Client ID and Client Secret. Store them in the safe place. In your code
 you can use them as enviroment variables, they sholdn't be hardcoded. You can
 perform actions with API on: - OLX PL - OLX BG - OLX RO - OLX PT - OLX UA - OLX
 KZ By default, all requests are sent to olx.**PL**. To change it you must pass
 `country_code` argument to every child of Olx class, i.e.: ```python
```

### Comparing `olx-api-wrapper-0.3.5/olx_api_wrapper.egg-info/SOURCES.txt` & `olx-api-wrapper-1.0.0/olx_api_wrapper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `olx-api-wrapper-0.3.5/setup.py` & `olx-api-wrapper-1.0.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open("README.md", "r") as readme_file:
     long_description = readme_file.read()
 
 setup(
     name="olx-api-wrapper",
-    version="0.3.5",
+    version="1.0.0",
     description="Unofficial Wrapper for OLX API",
     author="Paweł Stawikowski",
     author_email="pawikoski@gmail.com",
     packages=find_packages(),
     url="https://github.com/Pawikoski/olx-api-wrapper",
     install_requires=["requests", "dacite"],
     long_description=long_description,
```

### Comparing `olx-api-wrapper-0.3.5/tests/test_cities_and_districts.py` & `olx-api-wrapper-1.0.0/tests/test_cities_and_districts.py`

 * *Files identical despite different names*

### Comparing `olx-api-wrapper-0.3.5/tests/test_users.py` & `olx-api-wrapper-1.0.0/tests/test_users.py`

 * *Files identical despite different names*

