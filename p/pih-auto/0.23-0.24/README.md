# Comparing `tmp/pih-auto-0.23.tar.gz` & `tmp/pih-auto-0.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-auto-0.23.tar", last modified: Mon May 20 22:47:34 2024, max compression
+gzip compressed data, was "pih-auto-0.24.tar", last modified: Thu May 23 15:36:11 2024, max compression
```

## Comparing `pih-auto-0.23.tar` & `pih-auto-0.24.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-20 22:47:34.314636 pih-auto-0.23/
-drwxrwxrwx   0        0        0        0 2024-05-20 22:47:33.933499 pih-auto-0.23/AutomationService/
--rw-rw-rw-   0        0        0        0 2022-08-10 08:09:48.000000 pih-auto-0.23/AutomationService/__init__.py
--rw-rw-rw-   0        0        0      152 2024-02-14 02:13:48.000000 pih-auto-0.23/AutomationService/__main__.py
--rw-rw-rw-   0        0        0      632 2024-05-20 22:38:30.000000 pih-auto-0.23/AutomationService/const.py
--rw-rw-rw-   0        0        0    18948 2024-05-16 00:51:34.000000 pih-auto-0.23/AutomationService/service.py
--rw-rw-rw-   0        0        0      295 2024-05-20 22:47:34.282358 pih-auto-0.23/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-20 22:47:34.251117 pih-auto-0.23/pih_auto.egg-info/
--rw-rw-rw-   0        0        0      295 2024-05-20 22:47:33.000000 pih-auto-0.23/pih_auto.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      309 2024-05-20 22:47:33.000000 pih-auto-0.23/pih_auto.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-20 22:47:33.000000 pih-auto-0.23/pih_auto.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2024-05-20 22:47:33.000000 pih-auto-0.23/pih_auto.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       13 2024-05-20 22:47:33.000000 pih-auto-0.23/pih_auto.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-05-20 22:47:33.000000 pih-auto-0.23/pih_auto.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-20 22:47:34.330283 pih-auto-0.23/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-23 15:36:11.482795 pih-auto-0.24/
+drwxrwxrwx   0        0        0        0 2024-05-23 15:36:11.041867 pih-auto-0.24/AutomationService/
+-rw-rw-rw-   0        0        0        0 2022-08-10 08:09:48.000000 pih-auto-0.24/AutomationService/__init__.py
+-rw-rw-rw-   0        0        0      152 2024-02-14 02:13:48.000000 pih-auto-0.24/AutomationService/__main__.py
+-rw-rw-rw-   0        0        0      624 2024-05-23 15:35:37.000000 pih-auto-0.24/AutomationService/const.py
+-rw-rw-rw-   0        0        0    18939 2024-05-23 15:34:54.000000 pih-auto-0.24/AutomationService/service.py
+-rw-rw-rw-   0        0        0      295 2024-05-23 15:36:11.467169 pih-auto-0.24/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-23 15:36:11.404852 pih-auto-0.24/pih_auto.egg-info/
+-rw-rw-rw-   0        0        0      295 2024-05-23 15:36:10.000000 pih-auto-0.24/pih_auto.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      309 2024-05-23 15:36:10.000000 pih-auto-0.24/pih_auto.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-23 15:36:10.000000 pih-auto-0.24/pih_auto.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2024-05-23 15:36:10.000000 pih-auto-0.24/pih_auto.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       13 2024-05-23 15:36:10.000000 pih-auto-0.24/pih_auto.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-05-23 15:36:10.000000 pih-auto-0.24/pih_auto.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-23 15:36:11.498418 pih-auto-0.24/setup.cfg
```

### Comparing `pih-auto-0.23/AutomationService/const.py` & `pih-auto-0.24/AutomationService/const.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 from enum import IntEnum, auto
 from pih.consts.hosts import Hosts
 from pih.collections.service import ServiceDescription
 
 
 NAME: str = "Automation"
 
-HOST = Hosts.BACKUP_WORKER
+HOST = Hosts.WS255
 
-VERSION: str = "0.23"
+VERSION: str = "0.24"
 
 SD: ServiceDescription = ServiceDescription(
     name=NAME,
     description="Automation service",
     host=HOST.NAME,
     use_standalone=True,
     standalone_name="auto",
```

### Comparing `pih-auto-0.23/AutomationService/service.py` & `pih-auto-0.24/AutomationService/service.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
                             )
                         ),
                         A.CT_ME_WH.GROUP.CONTROL_SERVICE_INDICATIONS,
                     )
 
         class DH:
             resource_problem_status_map: dict[str, ProblemState] = defaultdict(
-                ProblemState
+                str
             )
             hr_user: str | None = None
 
         def get_resource_status_address(resource_status: ResourceStatus) -> str:
             resource_status_address: str = resource_status.address  # type: ignore
             address_list: list[str] = [
                 A.CT_R_D.VPN_PACS_SPB.address,
```

