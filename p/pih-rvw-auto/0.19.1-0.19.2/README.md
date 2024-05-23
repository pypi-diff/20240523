# Comparing `tmp/pih-rvw_auto-0.19.1.tar.gz` & `tmp/pih-rvw_auto-0.19.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-rvw_auto-0.19.1.tar", last modified: Tue May 21 21:10:50 2024, max compression
+gzip compressed data, was "pih-rvw_auto-0.19.2.tar", last modified: Thu May 23 11:47:52 2024, max compression
```

## Comparing `pih-rvw_auto-0.19.1.tar` & `pih-rvw_auto-0.19.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 21:10:50.554074 pih-rvw_auto-0.19.1/
--rw-rw-rw-   0        0        0      284 2024-05-21 21:10:50.522822 pih-rvw_auto-0.19.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-21 21:10:50.130153 pih-rvw_auto-0.19.1/ReviewAutomationService/
--rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-rvw_auto-0.19.1/ReviewAutomationService/__init__.py
--rw-rw-rw-   0        0        0      158 2024-04-15 23:57:16.000000 pih-rvw_auto-0.19.1/ReviewAutomationService/__main__.py
--rw-rw-rw-   0        0        0     2625 2024-05-19 13:02:43.000000 pih-rvw_auto-0.19.1/ReviewAutomationService/api.py
--rw-rw-rw-   0        0        0      527 2024-05-21 21:10:10.000000 pih-rvw_auto-0.19.1/ReviewAutomationService/const.py
--rw-rw-rw-   0        0        0     8054 2024-05-21 21:10:19.000000 pih-rvw_auto-0.19.1/ReviewAutomationService/service.py
-drwxrwxrwx   0        0        0        0 2024-05-21 21:10:50.475947 pih-rvw_auto-0.19.1/pih_rvw_auto.egg-info/
--rw-rw-rw-   0        0        0      284 2024-05-21 21:10:49.000000 pih-rvw_auto-0.19.1/pih_rvw_auto.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      388 2024-05-21 21:10:49.000000 pih-rvw_auto-0.19.1/pih_rvw_auto.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 21:10:49.000000 pih-rvw_auto-0.19.1/pih_rvw_auto.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       72 2024-05-21 21:10:49.000000 pih-rvw_auto-0.19.1/pih_rvw_auto.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        5 2024-05-21 21:10:49.000000 pih-rvw_auto-0.19.1/pih_rvw_auto.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2024-05-21 21:10:49.000000 pih-rvw_auto-0.19.1/pih_rvw_auto.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-21 21:10:50.554074 pih-rvw_auto-0.19.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-23 11:47:52.324603 pih-rvw_auto-0.19.2/
+-rw-rw-rw-   0        0        0      284 2024-05-23 11:47:52.308977 pih-rvw_auto-0.19.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-23 11:47:51.884907 pih-rvw_auto-0.19.2/ReviewAutomationService/
+-rw-rw-rw-   0        0        0        0 2022-10-20 04:44:07.000000 pih-rvw_auto-0.19.2/ReviewAutomationService/__init__.py
+-rw-rw-rw-   0        0        0      158 2024-04-15 23:57:16.000000 pih-rvw_auto-0.19.2/ReviewAutomationService/__main__.py
+-rw-rw-rw-   0        0        0     2637 2024-05-23 11:36:51.000000 pih-rvw_auto-0.19.2/ReviewAutomationService/api.py
+-rw-rw-rw-   0        0        0      527 2024-05-23 11:34:17.000000 pih-rvw_auto-0.19.2/ReviewAutomationService/const.py
+-rw-rw-rw-   0        0        0     8054 2024-05-21 21:10:19.000000 pih-rvw_auto-0.19.2/ReviewAutomationService/service.py
+drwxrwxrwx   0        0        0        0 2024-05-23 11:47:52.262107 pih-rvw_auto-0.19.2/pih_rvw_auto.egg-info/
+-rw-rw-rw-   0        0        0      284 2024-05-23 11:47:51.000000 pih-rvw_auto-0.19.2/pih_rvw_auto.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      388 2024-05-23 11:47:51.000000 pih-rvw_auto-0.19.2/pih_rvw_auto.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 11:47:51.000000 pih-rvw_auto-0.19.2/pih_rvw_auto.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       72 2024-05-23 11:47:51.000000 pih-rvw_auto-0.19.2/pih_rvw_auto.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        5 2024-05-23 11:47:51.000000 pih-rvw_auto-0.19.2/pih_rvw_auto.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2024-05-23 11:47:51.000000 pih-rvw_auto-0.19.2/pih_rvw_auto.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-23 11:47:52.658311 pih-rvw_auto-0.19.2/setup.cfg
```

### Comparing `pih-rvw_auto-0.19.1/ReviewAutomationService/api.py` & `pih-rvw_auto-0.19.2/ReviewAutomationService/api.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import ipih
 
-from pih import A
+from pih import A, send_message
 from pih.collections import Result
 
 from pih.collections import PolibasePerson, Message
 from NotificationAutomationService.api import NotificationApi as Api
 
 
 class ReviewNotificationApi:
@@ -17,15 +17,15 @@
                 def every_action(person: PolibasePerson, inpatient: bool) -> None:
                     telephone_number: str | None = A.D_F.telephone_number_international(
                         person.telephoneNumber
                     )
                     # polibase format telephone number 7
                     if A.C.telephone_number_international(telephone_number):
                         sender: str = A.D.get(sender_profile)
-                        if queued_message(
+                        if send_message(
                             Message(
                                 A.S_P_RN.notification_text(
                                     person,
                                     Api.check_for_notification_confirmation(
                                         telephone_number, sender, test
                                     ),
                                 ),
```

### Comparing `pih-rvw_auto-0.19.1/ReviewAutomationService/const.py` & `pih-rvw_auto-0.19.2/ReviewAutomationService/const.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pih.consts.hosts import Hosts
 from pih.collections.service import ServiceDescription
 
 NAME: str = "ReviewAutomation"
 
 HOST = Hosts.BACKUP_WORKER
 
-VERSION: str = "0.19.1"
+VERSION: str = "0.19.2"
 
 SD: ServiceDescription = ServiceDescription(
     name=NAME,
     description="Review automation service",
     host=HOST.NAME,
     use_standalone=True,
     version=VERSION,
```

### Comparing `pih-rvw_auto-0.19.1/ReviewAutomationService/service.py` & `pih-rvw_auto-0.19.2/ReviewAutomationService/service.py`

 * *Files identical despite different names*

