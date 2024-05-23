# Comparing `tmp/alibabacloud_dingtalk-2.1.13.tar.gz` & `tmp/alibabacloud_dingtalk-2.1.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_dingtalk-2.1.13.tar", last modified: Wed May 22 02:53:25 2024, max compression
+gzip compressed data, was "dist/alibabacloud_dingtalk-2.1.14.tar", last modified: Thu May 23 06:21:27 2024, max compression
```

## Comparing `alibabacloud_dingtalk-2.1.13.tar` & `alibabacloud_dingtalk-2.1.14.tar`

### file list

```diff
@@ -1,429 +1,433 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/
--rw-r--r--   0 root         (0) root         (0)   132635 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     3863 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2575 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     2660 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/activity_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/activity_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10220 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/activity_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    15463 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/activity_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/ai_interaction_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/ai_interaction_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25446 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/ai_interaction_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    24061 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/ai_interaction_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/ai_paa_s_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/ai_paa_s_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    51732 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/ai_paa_s_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    55896 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/ai_paa_s_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/algo_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/algo_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11812 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/algo_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    23886 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/algo_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/alitrip_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/alitrip_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    69836 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/alitrip_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   171793 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/alitrip_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/amdp_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/amdp_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19974 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/amdp_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    25370 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/amdp_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/apaas_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/apaas_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    30918 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/apaas_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    47170 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/apaas_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/app_market_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/app_market_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    31278 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/app_market_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    27481 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/app_market_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/ats_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/ats_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   114212 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/ats_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   145728 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/ats_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/attendance_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/attendance_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   248134 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/attendance_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   413198 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/attendance_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/badge_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/badge_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    53158 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/badge_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    64382 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/badge_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/bay_max_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/bay_max_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6152 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/bay_max_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4135 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/bay_max_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/bizfinance_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/bizfinance_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   306758 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/bizfinance_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   657929 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/bizfinance_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/bizfinance_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/bizfinance_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    98018 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/bizfinance_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)   115937 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/bizfinance_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/blackboard_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/blackboard_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11616 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/blackboard_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     9944 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/blackboard_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/calendar_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/calendar_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   191860 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/calendar_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   398319 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/calendar_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/carbon_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/carbon_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    34906 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/carbon_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    42901 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/carbon_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/card_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/card_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    89960 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/card_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   237978 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/card_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/check_in_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/check_in_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7076 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/check_in_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    10504 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/check_in_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/chengfeng_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/chengfeng_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    88282 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/chengfeng_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   124205 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/chengfeng_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/conference_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/conference_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   185660 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/conference_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   224275 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/conference_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/connector_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/connector_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    71002 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/connector_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   126248 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/connector_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/contact_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/contact_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   408970 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/contact_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   425714 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/contact_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/content_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/content_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25686 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/content_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    43876 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/content_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/contract_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/contract_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    40206 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/contract_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    44858 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/contract_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/conv_file_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/conv_file_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21312 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/conv_file_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    30666 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/conv_file_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/cool_app_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/cool_app_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23500 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/cool_app_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    25937 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/cool_app_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/cool_ops_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/cool_ops_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10844 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/cool_ops_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    14576 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/cool_ops_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/credit_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/credit_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6516 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/credit_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    10302 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/credit_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/crm_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/crm_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   315868 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/crm_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   638801 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/crm_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/crm_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/crm_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5774 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/crm_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)     7253 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/crm_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/customer_service_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/customer_service_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    37328 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/customer_service_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    46524 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/customer_service_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/datacenter_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/datacenter_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   494304 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/datacenter_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   515207 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/datacenter_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/devicemng_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/devicemng_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   134392 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/devicemng_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   150282 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/devicemng_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/ding_phone_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/ding_phone_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16480 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/ding_phone_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    15793 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/ding_phone_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/dingmi_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/dingmi_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    70120 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/dingmi_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    56029 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/dingmi_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/diot_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/diot_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    79025 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/diot_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    81667 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/diot_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/doc_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/doc_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   313048 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/doc_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   322887 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/doc_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/doc_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/doc_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   260012 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/doc_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)   385294 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/doc_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/dpaas_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/dpaas_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23366 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/dpaas_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    25936 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/dpaas_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/drive_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/drive_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   168538 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/drive_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   200479 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/drive_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/edu_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/edu_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   672294 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/edu_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   877133 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/edu_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/esign_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/esign_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    89270 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/esign_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   113792 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/esign_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/esign_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/esign_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   104118 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/esign_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)   121491 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/esign_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/event_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/event_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22157 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/event_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    20888 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/event_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/exclusive_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/exclusive_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   477634 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/exclusive_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   552235 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/exclusive_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/finance_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/finance_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   191008 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/finance_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   320947 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/finance_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/flashmeeting_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/flashmeeting_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21190 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/flashmeeting_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    28705 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/flashmeeting_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/flashmsg_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/flashmsg_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    42854 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/flashmsg_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    53610 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/flashmsg_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/gateway_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/gateway_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5681 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/gateway_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     5155 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/gateway_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/group_blackboard_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/group_blackboard_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12390 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/group_blackboard_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     9744 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/group_blackboard_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/h3yun_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/h3yun_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    98153 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/h3yun_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   137888 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/h3yun_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/h5package_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/h5package_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20603 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/h5package_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    18299 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/h5package_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/hrbrain_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/hrbrain_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    84750 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/hrbrain_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   124476 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/hrbrain_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/hrm_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/hrm_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   195023 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/hrm_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   271289 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/hrm_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/im_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/im_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   396886 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/im_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   413672 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/im_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/im_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/im_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    28815 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/im_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)    33507 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/im_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/impaas_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/impaas_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   107508 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/impaas_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    91958 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/impaas_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/industry_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/industry_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   815324 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/industry_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   937150 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/industry_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/jzcrm_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/jzcrm_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    75114 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/jzcrm_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   157606 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/jzcrm_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/link_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/link_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    78582 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/link_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   108065 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/link_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/live_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/live_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   110044 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/live_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   133326 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/live_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/live_activities_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/live_activities_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11628 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/live_activities_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    14026 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/live_activities_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/mail_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/mail_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5990 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/mail_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4381 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/mail_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/manufacturing_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/manufacturing_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18311 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/manufacturing_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    23610 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/manufacturing_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/micro_app_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/micro_app_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   181489 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/micro_app_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   173547 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/micro_app_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/miniapp_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/miniapp_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    62895 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/miniapp_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    53887 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/miniapp_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/notable_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/notable_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    71486 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/notable_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    63136 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/notable_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/oauth2_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/oauth2_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    42982 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/oauth2_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    44105 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/oauth2_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/occupationauth_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/occupationauth_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10832 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/occupationauth_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     7243 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/occupationauth_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/okr_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/okr_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   107234 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/okr_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   167406 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/okr_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/org_culture_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/org_culture_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    93818 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/org_culture_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   123438 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/org_culture_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/package_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/package_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    69184 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/package_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    59069 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/package_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/pedia_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/pedia_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    35028 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/pedia_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    68771 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/pedia_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/project_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/project_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   319400 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/project_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   411401 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/project_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/project_integration_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/project_integration_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21787 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/project_integration_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    10808 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/project_integration_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/rcs_call_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/rcs_call_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6382 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/rcs_call_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4561 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/rcs_call_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/report_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/report_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    30496 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/report_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    44394 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/report_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/resident_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/resident_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   164608 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/resident_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   172757 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/resident_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/robot_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/robot_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   115490 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/robot_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   105876 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/robot_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/rooms_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/rooms_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   129210 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/rooms_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   167086 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/rooms_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/search_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/search_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    47742 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/search_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    46647 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/search_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/service_group_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/service_group_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   460426 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/service_group_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   551312 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/service_group_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/smart_device_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/smart_device_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    38532 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/smart_device_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    26120 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/smart_device_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/sns_storage_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/sns_storage_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    54274 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/sns_storage_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    95239 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/sns_storage_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/storage_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/storage_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   226462 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/storage_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   350226 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/storage_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/storage_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/storage_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    70068 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/storage_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)    95695 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/storage_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/swform_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/swform_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16918 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/swform_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    28519 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/swform_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/todo_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/todo_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    84018 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/todo_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   152968 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/todo_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/trade_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/trade_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17044 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/trade_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    16445 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/trade_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/trajectory_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/trajectory_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17118 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/trajectory_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    22383 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/trajectory_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/transcribe_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/transcribe_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16528 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/transcribe_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    17427 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/transcribe_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/trip_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/trip_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    91210 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/trip_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   135827 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/trip_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/village_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/village_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    92596 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/village_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   111817 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/village_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/watt_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/watt_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    40437 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/watt_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    40791 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/watt_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/wiki_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/wiki_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10216 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/wiki_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    21704 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/wiki_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/wiki_2_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/wiki_2_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    79864 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/wiki_2_0/client.py
--rw-r--r--   0 root         (0) root         (0)   129013 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/wiki_2_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/wms_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/wms_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6226 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/wms_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     8459 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/wms_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/workbench_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/workbench_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)    50430 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/workbench_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)    43338 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/workbench_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/workflow_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/workflow_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   252082 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/workflow_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   441259 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/workflow_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/workrecord_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/workrecord_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5688 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/workrecord_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     3678 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/workrecord_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/yida_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/yida_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)   590500 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/yida_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)   761218 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/yida_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/yun_shu_1_0/
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/yun_shu_1_0/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6382 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/yun_shu_1_0/client.py
--rw-r--r--   0 root         (0) root         (0)     4472 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/yun_shu_1_0/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3863 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    14206 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      240 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-05-22 02:53:25.000000 alibabacloud_dingtalk-2.1.13/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2685 2024-05-22 02:53:24.000000 alibabacloud_dingtalk-2.1.13/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/
+-rw-r--r--   0 root         (0) root         (0)   134181 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     3863 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2575 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     2660 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/activity_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/activity_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10220 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/activity_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    15463 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/activity_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/agoal_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/agoal_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24694 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/agoal_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    36448 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/agoal_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/ai_interaction_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/ai_interaction_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25446 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/ai_interaction_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    24061 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/ai_interaction_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/ai_paa_s_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/ai_paa_s_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    51732 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/ai_paa_s_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    55896 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/ai_paa_s_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/algo_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/algo_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11812 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/algo_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    23886 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/algo_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/alitrip_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/alitrip_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    69836 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/alitrip_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   171793 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/alitrip_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/amdp_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/amdp_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19974 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/amdp_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    25370 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/amdp_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/apaas_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/apaas_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    30918 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/apaas_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    47170 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/apaas_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/app_market_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/app_market_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    31278 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/app_market_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    27481 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/app_market_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/ats_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/ats_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   114212 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/ats_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   145728 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/ats_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/attendance_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/attendance_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   248134 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/attendance_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   413198 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/attendance_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/badge_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/badge_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    53158 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/badge_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    64382 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/badge_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/bay_max_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/bay_max_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6152 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/bay_max_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4135 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/bay_max_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/bizfinance_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/bizfinance_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   306758 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/bizfinance_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   657929 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/bizfinance_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/bizfinance_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/bizfinance_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    98018 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/bizfinance_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   115937 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/bizfinance_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/blackboard_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/blackboard_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11616 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/blackboard_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     9944 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/blackboard_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/calendar_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/calendar_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   192336 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/calendar_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   407651 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/calendar_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/carbon_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/carbon_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    34906 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/carbon_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    42901 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/carbon_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/card_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/card_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    89960 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/card_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   237978 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/card_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/check_in_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/check_in_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7076 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/check_in_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    10504 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/check_in_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/chengfeng_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/chengfeng_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    88282 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/chengfeng_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   124205 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/chengfeng_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/conference_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/conference_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   185660 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/conference_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   224275 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/conference_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/connector_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/connector_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    71002 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/connector_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   126248 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/connector_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/contact_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/contact_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   408970 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/contact_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   425714 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/contact_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/content_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/content_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25686 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/content_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    43876 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/content_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/contract_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/contract_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    40206 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/contract_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    44858 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/contract_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/conv_file_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/conv_file_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21312 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/conv_file_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    30666 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/conv_file_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/cool_app_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/cool_app_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23500 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/cool_app_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    25937 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/cool_app_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/cool_ops_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/cool_ops_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10844 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/cool_ops_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    14576 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/cool_ops_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/credit_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/credit_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6516 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/credit_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    10302 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/credit_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/crm_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/crm_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   315868 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/crm_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   638801 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/crm_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/crm_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/crm_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5774 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/crm_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     7253 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/crm_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/customer_service_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/customer_service_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    37328 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/customer_service_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    46524 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/customer_service_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/datacenter_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/datacenter_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   494304 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/datacenter_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   515207 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/datacenter_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/devicemng_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/devicemng_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   134392 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/devicemng_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   150282 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/devicemng_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/ding_phone_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/ding_phone_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16480 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/ding_phone_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    15793 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/ding_phone_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/dingmi_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/dingmi_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    70120 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/dingmi_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    56029 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/dingmi_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/diot_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/diot_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    79025 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/diot_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    81667 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/diot_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/doc_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/doc_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   313048 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/doc_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   322887 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/doc_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/doc_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/doc_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   260012 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/doc_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   385294 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/doc_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/dpaas_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/dpaas_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23366 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/dpaas_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    25936 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/dpaas_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/drive_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/drive_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   168538 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/drive_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   200479 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/drive_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/edu_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/edu_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   672294 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/edu_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   877133 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/edu_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/esign_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/esign_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    89270 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/esign_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   113792 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/esign_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/esign_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/esign_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   104118 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/esign_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   121491 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/esign_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/event_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/event_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22157 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/event_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    20888 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/event_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/exclusive_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/exclusive_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   482712 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/exclusive_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   556456 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/exclusive_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/finance_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/finance_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   191008 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/finance_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   320947 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/finance_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/flashmeeting_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/flashmeeting_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21190 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/flashmeeting_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    28705 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/flashmeeting_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/flashmsg_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/flashmsg_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    42854 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/flashmsg_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    53610 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/flashmsg_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/gateway_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/gateway_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5681 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/gateway_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     5155 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/gateway_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/group_blackboard_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/group_blackboard_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12390 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/group_blackboard_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     9744 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/group_blackboard_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/h3yun_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/h3yun_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    98153 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/h3yun_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   137888 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/h3yun_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/h5package_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/h5package_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20603 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/h5package_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    18299 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/h5package_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/hrbrain_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/hrbrain_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    84750 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/hrbrain_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   124476 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/hrbrain_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/hrm_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/hrm_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   195023 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/hrm_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   271289 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/hrm_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/im_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/im_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   396886 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/im_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   413672 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/im_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/im_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/im_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    28815 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/im_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    33507 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/im_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/impaas_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/impaas_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   107508 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/impaas_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    91958 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/impaas_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/industry_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/industry_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   815324 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/industry_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   937150 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/industry_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/jzcrm_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/jzcrm_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    75114 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/jzcrm_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   157606 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/jzcrm_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/link_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/link_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    78582 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/link_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   108065 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/link_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/live_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/live_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   110044 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/live_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   133326 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/live_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/live_activities_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/live_activities_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11628 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/live_activities_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    14026 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/live_activities_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/mail_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/mail_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5990 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/mail_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4381 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/mail_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/manufacturing_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/manufacturing_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18311 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/manufacturing_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    23610 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/manufacturing_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/micro_app_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/micro_app_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   181489 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/micro_app_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   173547 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/micro_app_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/miniapp_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/miniapp_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    62895 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/miniapp_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    53887 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/miniapp_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/notable_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/notable_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    71486 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/notable_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    63136 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/notable_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/oauth2_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/oauth2_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    42982 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/oauth2_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    44105 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/oauth2_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/occupationauth_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/occupationauth_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10832 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/occupationauth_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     7243 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/occupationauth_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/okr_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/okr_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   107234 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/okr_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   167406 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/okr_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/org_culture_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/org_culture_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    93818 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/org_culture_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   123438 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/org_culture_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/package_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/package_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    69184 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/package_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    59069 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/package_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/pedia_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/pedia_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    35028 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/pedia_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    68771 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/pedia_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/project_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/project_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   319400 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/project_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   411401 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/project_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/project_integration_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/project_integration_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21787 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/project_integration_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    10808 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/project_integration_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/rcs_call_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/rcs_call_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6382 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/rcs_call_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4561 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/rcs_call_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/report_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/report_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    30496 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/report_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    44394 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/report_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/resident_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/resident_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   164608 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/resident_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   172757 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/resident_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/robot_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/robot_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   115490 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/robot_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   105876 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/robot_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/rooms_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/rooms_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   129210 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/rooms_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   167086 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/rooms_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/search_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/search_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    47742 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/search_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    46647 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/search_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/service_group_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/service_group_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   460426 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/service_group_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   551312 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/service_group_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/smart_device_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/smart_device_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    38532 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/smart_device_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    26120 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/smart_device_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/sns_storage_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/sns_storage_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    54274 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/sns_storage_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    95239 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/sns_storage_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/storage_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/storage_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   226462 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/storage_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   350226 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/storage_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/storage_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/storage_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    70068 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/storage_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    95695 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/storage_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/swform_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/swform_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16918 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/swform_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    28519 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/swform_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/todo_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/todo_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    84018 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/todo_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   152968 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/todo_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/trade_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/trade_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17044 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/trade_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    16445 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/trade_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/trajectory_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/trajectory_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17118 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/trajectory_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    22383 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/trajectory_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/transcribe_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/transcribe_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16528 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/transcribe_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    17427 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/transcribe_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/trip_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/trip_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    91210 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/trip_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   135827 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/trip_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/village_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/village_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    92596 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/village_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   111817 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/village_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/watt_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/watt_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    40437 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/watt_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    40791 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/watt_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/wiki_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/wiki_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10216 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/wiki_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    21704 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/wiki_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/wiki_2_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/wiki_2_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    79864 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/wiki_2_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   129013 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/wiki_2_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/wms_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/wms_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6226 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/wms_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     8459 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/wms_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/workbench_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/workbench_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    50430 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/workbench_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)    43338 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/workbench_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/workflow_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/workflow_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   262706 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/workflow_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   457245 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/workflow_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/workrecord_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/workrecord_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5688 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/workrecord_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     3678 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/workrecord_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/yida_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/yida_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   590500 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/yida_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)   761218 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/yida_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/yun_shu_1_0/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/yun_shu_1_0/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6382 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/yun_shu_1_0/client.py
+-rw-r--r--   0 root         (0) root         (0)     4472 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/yun_shu_1_0/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3863 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    14334 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      240 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-05-23 06:21:27.000000 alibabacloud_dingtalk-2.1.14/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2685 2024-05-23 06:21:26.000000 alibabacloud_dingtalk-2.1.14/setup.py
```

### Comparing `alibabacloud_dingtalk-2.1.13/ChangeLog.md` & `alibabacloud_dingtalk-2.1.14/ChangeLog.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+2024-05-22 Version: 2.1.13
+- Generated python activity_1.0,agoal_1.0,aiInteraction_1.0,aiPaaS_1.0,algo_1.0,alitest_1.0,alitrip_1.0,amdp_1.0,apaas_1.0,appMarket_1.0,ats_1.0,attendance_1.0,badge_1.0,bayMax_1.0,baymax_2.0,bipaas_1.0,bizfinance_1.0,bizfinance_2.0,blackboard_1.0,calendar_1.0,calendar_2.0,carbon_1.0,card_1.0,checkIn_1.0,chengfeng_1.0,conference_1.0,connector_1.0,contact_1.0,content_1.0,contract_1.0,convFile_1.0,convStorage_1.0,coolApp_1.0,coolOps_1.0,credit_1.0,crm_1.0,crm_2.0,customerService_1.0,datacenter_1.0,delivery_1.0,devicemng_1.0,dingmi_1.0,dingPhone_1.0,dingsport_1.0,diot_1.0,doc_1.0,doc_2.0,dpaas_1.0,drive_1.0,drive_2.0,edu_1.0,esign_1.0,event_1.0,event_2.0,exclusive_1.0,finance_1.0,flashmeeting_1.0,flashmsg_1.0,gateway_1.0,groupBlackboard_1.0,h5package_1.0,hrbrain_1.0,hrm_1.0,im_1.0,im_2.0,impaas_1.0,industry_1.0,integration_1.0,liandanlu_1.0,link_1.0,live_1.0,liveActivities_1.0,mail_1.0,manufacturing_1.0,media_1.0,medical_1.0,microApp_1.0,miniapp_1.0,notable_1.0,oauth2_1.0,occupationauth_1.0,office_1.0,okr_1.0,orgCulture_1.0,ow_1.0,package_1.0,pedia_1.0,project_1.0,projectIntegration_1.0,rcsCall_1.0,report_1.0,resident_1.0,robot_1.0,rooms_1.0,search_1.0,serviceGroup_1.0,setting_1.0,smartDevice_1.0,snsStorage_1.0,storage_1.0,storage_2.0,swform_1.0,theone_1.0,todo_1.0,trade_1.0,trajectory_1.0,transcribe_1.0,trip_1.0,village_1.0,waterMark_1.0,watt_1.0,wiki_1.0,wiki_2.0,wms_1.0,workbench_1.0,workflow_1.0,workrecord_1.0,yida_1.0,yunShu_1.0,esign_1.1,esign_2.0,h3yun_1.0,jzcrm_1.0,soke_1.0 for dingtalk.
+
 2024-05-18 Version: 2.1.12
 - Generated python activity_1.0,agoal_1.0,aiInteraction_1.0,aiPaaS_1.0,algo_1.0,alitest_1.0,alitrip_1.0,amdp_1.0,apaas_1.0,appMarket_1.0,ats_1.0,attendance_1.0,badge_1.0,bayMax_1.0,baymax_2.0,bipaas_1.0,bizfinance_1.0,bizfinance_2.0,blackboard_1.0,calendar_1.0,calendar_2.0,carbon_1.0,card_1.0,checkIn_1.0,chengfeng_1.0,conference_1.0,connector_1.0,contact_1.0,content_1.0,contract_1.0,convFile_1.0,convStorage_1.0,coolApp_1.0,coolOps_1.0,credit_1.0,crm_1.0,crm_2.0,customerService_1.0,datacenter_1.0,delivery_1.0,devicemng_1.0,dingmi_1.0,dingPhone_1.0,dingsport_1.0,diot_1.0,doc_1.0,doc_2.0,dpaas_1.0,drive_1.0,drive_2.0,edu_1.0,esign_1.0,event_1.0,event_2.0,exclusive_1.0,finance_1.0,flashmeeting_1.0,flashmsg_1.0,gateway_1.0,groupBlackboard_1.0,h5package_1.0,hrbrain_1.0,hrm_1.0,im_1.0,im_2.0,impaas_1.0,industry_1.0,integration_1.0,liandanlu_1.0,link_1.0,live_1.0,liveActivities_1.0,mail_1.0,manufacturing_1.0,media_1.0,medical_1.0,microApp_1.0,miniapp_1.0,notable_1.0,oauth2_1.0,occupationauth_1.0,office_1.0,okr_1.0,orgCulture_1.0,ow_1.0,package_1.0,pedia_1.0,project_1.0,projectIntegration_1.0,rcsCall_1.0,report_1.0,resident_1.0,robot_1.0,rooms_1.0,search_1.0,serviceGroup_1.0,setting_1.0,smartDevice_1.0,snsStorage_1.0,storage_1.0,storage_2.0,swform_1.0,theone_1.0,todo_1.0,trade_1.0,trajectory_1.0,transcribe_1.0,trip_1.0,village_1.0,waterMark_1.0,watt_1.0,wiki_1.0,wiki_2.0,wms_1.0,workbench_1.0,workflow_1.0,workrecord_1.0,yida_1.0,yunShu_1.0,esign_1.1,esign_2.0,h3yun_1.0,jzcrm_1.0,soke_1.0 for dingtalk.
 
 2024-05-14 Version: 2.1.11
 - Generated python activity_1.0,agoal_1.0,aiInteraction_1.0,aiPaaS_1.0,algo_1.0,alitest_1.0,alitrip_1.0,amdp_1.0,apaas_1.0,appMarket_1.0,ats_1.0,attendance_1.0,badge_1.0,bayMax_1.0,baymax_2.0,bipaas_1.0,bizfinance_1.0,bizfinance_2.0,blackboard_1.0,calendar_1.0,calendar_2.0,carbon_1.0,card_1.0,checkIn_1.0,chengfeng_1.0,conference_1.0,connector_1.0,contact_1.0,content_1.0,contract_1.0,convFile_1.0,convStorage_1.0,coolApp_1.0,coolOps_1.0,credit_1.0,crm_1.0,crm_2.0,customerService_1.0,datacenter_1.0,delivery_1.0,devicemng_1.0,dingmi_1.0,dingPhone_1.0,dingsport_1.0,diot_1.0,doc_1.0,doc_2.0,dpaas_1.0,drive_1.0,drive_2.0,edu_1.0,esign_1.0,event_1.0,event_2.0,exclusive_1.0,finance_1.0,flashmeeting_1.0,flashmsg_1.0,gateway_1.0,groupBlackboard_1.0,h5package_1.0,hrbrain_1.0,hrm_1.0,im_1.0,im_2.0,impaas_1.0,industry_1.0,integration_1.0,liandanlu_1.0,link_1.0,live_1.0,liveActivities_1.0,mail_1.0,manufacturing_1.0,media_1.0,medical_1.0,microApp_1.0,miniapp_1.0,notable_1.0,oauth2_1.0,occupationauth_1.0,office_1.0,okr_1.0,orgCulture_1.0,ow_1.0,package_1.0,pedia_1.0,project_1.0,projectIntegration_1.0,rcsCall_1.0,report_1.0,resident_1.0,robot_1.0,rooms_1.0,search_1.0,serviceGroup_1.0,setting_1.0,smartDevice_1.0,snsStorage_1.0,storage_1.0,storage_2.0,swform_1.0,theone_1.0,todo_1.0,trade_1.0,trajectory_1.0,transcribe_1.0,trip_1.0,village_1.0,waterMark_1.0,watt_1.0,wiki_1.0,wiki_2.0,wms_1.0,workbench_1.0,workflow_1.0,workrecord_1.0,yida_1.0,yunShu_1.0,esign_1.1,esign_2.0,h3yun_1.0,jzcrm_1.0,soke_1.0 for dingtalk.
 
 2024-05-09 Version: 2.1.10
```

### Comparing `alibabacloud_dingtalk-2.1.13/LICENSE` & `alibabacloud_dingtalk-2.1.14/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/PKG-INFO` & `alibabacloud_dingtalk-2.1.14/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_dingtalk
-Version: 2.1.13
+Version: 2.1.14
 Summary: Alibaba Cloud Dingtalk SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dingtalk-2.1.13/README-CN.md` & `alibabacloud_dingtalk-2.1.14/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/README.md` & `alibabacloud_dingtalk-2.1.14/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/activity_1_0/client.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/activity_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/activity_1_0/models.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/activity_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/ai_interaction_1_0/client.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/ai_interaction_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/ai_interaction_1_0/models.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/ai_interaction_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/ai_paa_s_1_0/client.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/ai_paa_s_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/ai_paa_s_1_0/models.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/ai_paa_s_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/algo_1_0/client.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/algo_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/algo_1_0/models.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/algo_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/alitrip_1_0/client.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/alitrip_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/alitrip_1_0/models.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/alitrip_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/amdp_1_0/client.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/amdp_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/amdp_1_0/models.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/amdp_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/apaas_1_0/client.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/apaas_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/apaas_1_0/models.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/apaas_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/app_market_1_0/client.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/app_market_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/app_market_1_0/models.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/app_market_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/ats_1_0/client.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/ats_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/ats_1_0/models.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/ats_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/attendance_1_0/client.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/attendance_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/attendance_1_0/models.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/attendance_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/badge_1_0/client.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/badge_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/badge_1_0/models.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/badge_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/bay_max_1_0/client.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/bay_max_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/bay_max_1_0/models.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/bay_max_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/bizfinance_1_0/client.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/bizfinance_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/bizfinance_1_0/models.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/bizfinance_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/bizfinance_2_0/client.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/bizfinance_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/bizfinance_2_0/models.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/bizfinance_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/blackboard_1_0/client.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/blackboard_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/blackboard_1_0/models.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/blackboard_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/calendar_1_0/client.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/calendar_1_0/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -669,14 +669,16 @@
         @param runtime: runtime options for this request RuntimeOptions
         @return: CreateEventResponse
         """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.attendees):
             body['attendees'] = request.attendees
+        if not UtilClient.is_unset(request.card_instances):
+            body['cardInstances'] = request.card_instances
         if not UtilClient.is_unset(request.description):
             body['description'] = request.description
         if not UtilClient.is_unset(request.end):
             body['end'] = request.end
         if not UtilClient.is_unset(request.extra):
             body['extra'] = request.extra
         if not UtilClient.is_unset(request.is_all_day):
@@ -740,14 +742,16 @@
         @param runtime: runtime options for this request RuntimeOptions
         @return: CreateEventResponse
         """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.attendees):
             body['attendees'] = request.attendees
+        if not UtilClient.is_unset(request.card_instances):
+            body['cardInstances'] = request.card_instances
         if not UtilClient.is_unset(request.description):
             body['description'] = request.description
         if not UtilClient.is_unset(request.end):
             body['end'] = request.end
         if not UtilClient.is_unset(request.extra):
             body['extra'] = request.extra
         if not UtilClient.is_unset(request.is_all_day):
@@ -3472,14 +3476,16 @@
         @param runtime: runtime options for this request RuntimeOptions
         @return: PatchEventResponse
         """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.attendees):
             body['attendees'] = request.attendees
+        if not UtilClient.is_unset(request.card_instances):
+            body['cardInstances'] = request.card_instances
         if not UtilClient.is_unset(request.description):
             body['description'] = request.description
         if not UtilClient.is_unset(request.end):
             body['end'] = request.end
         if not UtilClient.is_unset(request.extra):
             body['extra'] = request.extra
         if not UtilClient.is_unset(request.id):
@@ -3546,14 +3552,16 @@
         @param runtime: runtime options for this request RuntimeOptions
         @return: PatchEventResponse
         """
         UtilClient.validate_model(request)
         body = {}
         if not UtilClient.is_unset(request.attendees):
             body['attendees'] = request.attendees
+        if not UtilClient.is_unset(request.card_instances):
+            body['cardInstances'] = request.card_instances
         if not UtilClient.is_unset(request.description):
             body['description'] = request.description
         if not UtilClient.is_unset(request.end):
             body['end'] = request.end
         if not UtilClient.is_unset(request.extra):
             body['extra'] = request.extra
         if not UtilClient.is_unset(request.id):
```

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/calendar_1_0/models.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/calendar_1_0/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -852,14 +852,47 @@
         if m.get('id') is not None:
             self.id = m.get('id')
         if m.get('isOptional') is not None:
             self.is_optional = m.get('isOptional')
         return self
 
 
+class CreateEventRequestCardInstances(TeaModel):
+    def __init__(
+        self,
+        out_track_id: str = None,
+        scenario: str = None,
+    ):
+        self.out_track_id = out_track_id
+        self.scenario = scenario
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.out_track_id is not None:
+            result['outTrackId'] = self.out_track_id
+        if self.scenario is not None:
+            result['scenario'] = self.scenario
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('outTrackId') is not None:
+            self.out_track_id = m.get('outTrackId')
+        if m.get('scenario') is not None:
+            self.scenario = m.get('scenario')
+        return self
+
+
 class CreateEventRequestEnd(TeaModel):
     def __init__(
         self,
         date: str = None,
         date_time: str = None,
         time_zone: str = None,
     ):
@@ -1216,28 +1249,30 @@
         return self
 
 
 class CreateEventRequest(TeaModel):
     def __init__(
         self,
         attendees: List[CreateEventRequestAttendees] = None,
+        card_instances: List[CreateEventRequestCardInstances] = None,
         description: str = None,
         end: CreateEventRequestEnd = None,
         extra: Dict[str, str] = None,
         is_all_day: bool = None,
         location: CreateEventRequestLocation = None,
         online_meeting_info: CreateEventRequestOnlineMeetingInfo = None,
         recurrence: CreateEventRequestRecurrence = None,
         reminders: List[CreateEventRequestReminders] = None,
         rich_text_description: CreateEventRequestRichTextDescription = None,
         start: CreateEventRequestStart = None,
         summary: str = None,
         ui_configs: List[CreateEventRequestUiConfigs] = None,
     ):
         self.attendees = attendees
+        self.card_instances = card_instances
         self.description = description
         self.end = end
         self.extra = extra
         self.is_all_day = is_all_day
         self.location = location
         self.online_meeting_info = online_meeting_info
         self.recurrence = recurrence
@@ -1250,14 +1285,18 @@
         self.ui_configs = ui_configs
 
     def validate(self):
         if self.attendees:
             for k in self.attendees:
                 if k:
                     k.validate()
+        if self.card_instances:
+            for k in self.card_instances:
+                if k:
+                    k.validate()
         if self.end:
             self.end.validate()
         if self.location:
             self.location.validate()
         if self.online_meeting_info:
             self.online_meeting_info.validate()
         if self.recurrence:
@@ -1281,14 +1320,18 @@
             return _map
 
         result = dict()
         result['attendees'] = []
         if self.attendees is not None:
             for k in self.attendees:
                 result['attendees'].append(k.to_map() if k else None)
+        result['cardInstances'] = []
+        if self.card_instances is not None:
+            for k in self.card_instances:
+                result['cardInstances'].append(k.to_map() if k else None)
         if self.description is not None:
             result['description'] = self.description
         if self.end is not None:
             result['end'] = self.end.to_map()
         if self.extra is not None:
             result['extra'] = self.extra
         if self.is_all_day is not None:
@@ -1318,14 +1361,19 @@
     def from_map(self, m: dict = None):
         m = m or dict()
         self.attendees = []
         if m.get('attendees') is not None:
             for k in m.get('attendees'):
                 temp_model = CreateEventRequestAttendees()
                 self.attendees.append(temp_model.from_map(k))
+        self.card_instances = []
+        if m.get('cardInstances') is not None:
+            for k in m.get('cardInstances'):
+                temp_model = CreateEventRequestCardInstances()
+                self.card_instances.append(temp_model.from_map(k))
         if m.get('description') is not None:
             self.description = m.get('description')
         if m.get('end') is not None:
             temp_model = CreateEventRequestEnd()
             self.end = temp_model.from_map(m['end'])
         if m.get('extra') is not None:
             self.extra = m.get('extra')
@@ -1408,14 +1456,47 @@
         if m.get('responseStatus') is not None:
             self.response_status = m.get('responseStatus')
         if m.get('self') is not None:
             self.self_ = m.get('self')
         return self
 
 
+class CreateEventResponseBodyCardInstances(TeaModel):
+    def __init__(
+        self,
+        out_track_id: str = None,
+        scenario: str = None,
+    ):
+        self.out_track_id = out_track_id
+        self.scenario = scenario
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.out_track_id is not None:
+            result['outTrackId'] = self.out_track_id
+        if self.scenario is not None:
+            result['scenario'] = self.scenario
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('outTrackId') is not None:
+            self.out_track_id = m.get('outTrackId')
+        if m.get('scenario') is not None:
+            self.scenario = m.get('scenario')
+        return self
+
+
 class CreateEventResponseBodyEnd(TeaModel):
     def __init__(
         self,
         date: str = None,
         date_time: str = None,
         time_zone: str = None,
     ):
@@ -1835,14 +1916,15 @@
         return self
 
 
 class CreateEventResponseBody(TeaModel):
     def __init__(
         self,
         attendees: List[CreateEventResponseBodyAttendees] = None,
+        card_instances: List[CreateEventResponseBodyCardInstances] = None,
         create_time: str = None,
         description: str = None,
         end: CreateEventResponseBodyEnd = None,
         id: str = None,
         is_all_day: bool = None,
         location: CreateEventResponseBodyLocation = None,
         online_meeting_info: CreateEventResponseBodyOnlineMeetingInfo = None,
@@ -1852,14 +1934,15 @@
         rich_text_description: CreateEventResponseBodyRichTextDescription = None,
         start: CreateEventResponseBodyStart = None,
         summary: str = None,
         ui_configs: List[CreateEventResponseBodyUiConfigs] = None,
         update_time: str = None,
     ):
         self.attendees = attendees
+        self.card_instances = card_instances
         # Use the UTC time format: yyyy-MM-ddTHH:mmZ
         self.create_time = create_time
         self.description = description
         self.end = end
         self.id = id
         self.is_all_day = is_all_day
         self.location = location
@@ -1876,14 +1959,18 @@
         self.update_time = update_time
 
     def validate(self):
         if self.attendees:
             for k in self.attendees:
                 if k:
                     k.validate()
+        if self.card_instances:
+            for k in self.card_instances:
+                if k:
+                    k.validate()
         if self.end:
             self.end.validate()
         if self.location:
             self.location.validate()
         if self.online_meeting_info:
             self.online_meeting_info.validate()
         if self.organizer:
@@ -1909,14 +1996,18 @@
             return _map
 
         result = dict()
         result['attendees'] = []
         if self.attendees is not None:
             for k in self.attendees:
                 result['attendees'].append(k.to_map() if k else None)
+        result['cardInstances'] = []
+        if self.card_instances is not None:
+            for k in self.card_instances:
+                result['cardInstances'].append(k.to_map() if k else None)
         if self.create_time is not None:
             result['createTime'] = self.create_time
         if self.description is not None:
             result['description'] = self.description
         if self.end is not None:
             result['end'] = self.end.to_map()
         if self.id is not None:
@@ -1952,14 +2043,19 @@
     def from_map(self, m: dict = None):
         m = m or dict()
         self.attendees = []
         if m.get('attendees') is not None:
             for k in m.get('attendees'):
                 temp_model = CreateEventResponseBodyAttendees()
                 self.attendees.append(temp_model.from_map(k))
+        self.card_instances = []
+        if m.get('cardInstances') is not None:
+            for k in m.get('cardInstances'):
+                temp_model = CreateEventResponseBodyCardInstances()
+                self.card_instances.append(temp_model.from_map(k))
         if m.get('createTime') is not None:
             self.create_time = m.get('createTime')
         if m.get('description') is not None:
             self.description = m.get('description')
         if m.get('end') is not None:
             temp_model = CreateEventResponseBodyEnd()
             self.end = temp_model.from_map(m['end'])
@@ -4011,14 +4107,47 @@
         if m.get('responseStatus') is not None:
             self.response_status = m.get('responseStatus')
         if m.get('self') is not None:
             self.self_ = m.get('self')
         return self
 
 
+class GetEventResponseBodyCardInstances(TeaModel):
+    def __init__(
+        self,
+        out_track_id: str = None,
+        scenario: str = None,
+    ):
+        self.out_track_id = out_track_id
+        self.scenario = scenario
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.out_track_id is not None:
+            result['outTrackId'] = self.out_track_id
+        if self.scenario is not None:
+            result['scenario'] = self.scenario
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('outTrackId') is not None:
+            self.out_track_id = m.get('outTrackId')
+        if m.get('scenario') is not None:
+            self.scenario = m.get('scenario')
+        return self
+
+
 class GetEventResponseBodyCategories(TeaModel):
     def __init__(
         self,
         display_name: str = None,
     ):
         self.display_name = display_name
 
@@ -4562,18 +4691,52 @@
         if m.get('dateTime') is not None:
             self.date_time = m.get('dateTime')
         if m.get('timeZone') is not None:
             self.time_zone = m.get('timeZone')
         return self
 
 
+class GetEventResponseBodyUiConfigs(TeaModel):
+    def __init__(
+        self,
+        ui_name: str = None,
+        ui_status: str = None,
+    ):
+        self.ui_name = ui_name
+        self.ui_status = ui_status
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.ui_name is not None:
+            result['uiName'] = self.ui_name
+        if self.ui_status is not None:
+            result['uiStatus'] = self.ui_status
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('uiName') is not None:
+            self.ui_name = m.get('uiName')
+        if m.get('uiStatus') is not None:
+            self.ui_status = m.get('uiStatus')
+        return self
+
+
 class GetEventResponseBody(TeaModel):
     def __init__(
         self,
         attendees: List[GetEventResponseBodyAttendees] = None,
+        card_instances: List[GetEventResponseBodyCardInstances] = None,
         categories: List[GetEventResponseBodyCategories] = None,
         create_time: str = None,
         description: str = None,
         end: GetEventResponseBodyEnd = None,
         extended_properties: GetEventResponseBodyExtendedProperties = None,
         id: str = None,
         is_all_day: bool = None,
@@ -4585,17 +4748,19 @@
         recurrence: GetEventResponseBodyRecurrence = None,
         reminders: List[GetEventResponseBodyReminders] = None,
         rich_text_description: GetEventResponseBodyRichTextDescription = None,
         series_master_id: str = None,
         start: GetEventResponseBodyStart = None,
         status: str = None,
         summary: str = None,
+        ui_configs: List[GetEventResponseBodyUiConfigs] = None,
         update_time: str = None,
     ):
         self.attendees = attendees
+        self.card_instances = card_instances
         self.categories = categories
         # Use the UTC time format: yyyy-MM-ddTHH:mmZ
         self.create_time = create_time
         self.description = description
         self.end = end
         self.extended_properties = extended_properties
         self.id = id
@@ -4609,22 +4774,27 @@
         self.reminders = reminders
         self.rich_text_description = rich_text_description
         self.series_master_id = series_master_id
         self.start = start
         # This parameter is required.
         self.status = status
         self.summary = summary
+        self.ui_configs = ui_configs
         # Use the UTC time format: yyyy-MM-ddTHH:mmZ
         self.update_time = update_time
 
     def validate(self):
         if self.attendees:
             for k in self.attendees:
                 if k:
                     k.validate()
+        if self.card_instances:
+            for k in self.card_instances:
+                if k:
+                    k.validate()
         if self.categories:
             for k in self.categories:
                 if k:
                     k.validate()
         if self.end:
             self.end.validate()
         if self.extended_properties:
@@ -4647,25 +4817,33 @@
             for k in self.reminders:
                 if k:
                     k.validate()
         if self.rich_text_description:
             self.rich_text_description.validate()
         if self.start:
             self.start.validate()
+        if self.ui_configs:
+            for k in self.ui_configs:
+                if k:
+                    k.validate()
 
     def to_map(self):
         _map = super().to_map()
         if _map is not None:
             return _map
 
         result = dict()
         result['attendees'] = []
         if self.attendees is not None:
             for k in self.attendees:
                 result['attendees'].append(k.to_map() if k else None)
+        result['cardInstances'] = []
+        if self.card_instances is not None:
+            for k in self.card_instances:
+                result['cardInstances'].append(k.to_map() if k else None)
         result['categories'] = []
         if self.categories is not None:
             for k in self.categories:
                 result['categories'].append(k.to_map() if k else None)
         if self.create_time is not None:
             result['createTime'] = self.create_time
         if self.description is not None:
@@ -4702,25 +4880,34 @@
             result['seriesMasterId'] = self.series_master_id
         if self.start is not None:
             result['start'] = self.start.to_map()
         if self.status is not None:
             result['status'] = self.status
         if self.summary is not None:
             result['summary'] = self.summary
+        result['uiConfigs'] = []
+        if self.ui_configs is not None:
+            for k in self.ui_configs:
+                result['uiConfigs'].append(k.to_map() if k else None)
         if self.update_time is not None:
             result['updateTime'] = self.update_time
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         self.attendees = []
         if m.get('attendees') is not None:
             for k in m.get('attendees'):
                 temp_model = GetEventResponseBodyAttendees()
                 self.attendees.append(temp_model.from_map(k))
+        self.card_instances = []
+        if m.get('cardInstances') is not None:
+            for k in m.get('cardInstances'):
+                temp_model = GetEventResponseBodyCardInstances()
+                self.card_instances.append(temp_model.from_map(k))
         self.categories = []
         if m.get('categories') is not None:
             for k in m.get('categories'):
                 temp_model = GetEventResponseBodyCategories()
                 self.categories.append(temp_model.from_map(k))
         if m.get('createTime') is not None:
             self.create_time = m.get('createTime')
@@ -4769,14 +4956,19 @@
         if m.get('start') is not None:
             temp_model = GetEventResponseBodyStart()
             self.start = temp_model.from_map(m['start'])
         if m.get('status') is not None:
             self.status = m.get('status')
         if m.get('summary') is not None:
             self.summary = m.get('summary')
+        self.ui_configs = []
+        if m.get('uiConfigs') is not None:
+            for k in m.get('uiConfigs'):
+                temp_model = GetEventResponseBodyUiConfigs()
+                self.ui_configs.append(temp_model.from_map(k))
         if m.get('updateTime') is not None:
             self.update_time = m.get('updateTime')
         return self
 
 
 class GetEventResponse(TeaModel):
     def __init__(
@@ -10499,14 +10691,47 @@
         if m.get('id') is not None:
             self.id = m.get('id')
         if m.get('isOptional') is not None:
             self.is_optional = m.get('isOptional')
         return self
 
 
+class PatchEventRequestCardInstances(TeaModel):
+    def __init__(
+        self,
+        out_track_id: str = None,
+        scenario: str = None,
+    ):
+        self.out_track_id = out_track_id
+        self.scenario = scenario
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.out_track_id is not None:
+            result['outTrackId'] = self.out_track_id
+        if self.scenario is not None:
+            result['scenario'] = self.scenario
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('outTrackId') is not None:
+            self.out_track_id = m.get('outTrackId')
+        if m.get('scenario') is not None:
+            self.scenario = m.get('scenario')
+        return self
+
+
 class PatchEventRequestEnd(TeaModel):
     def __init__(
         self,
         date: str = None,
         date_time: str = None,
         time_zone: str = None,
     ):
@@ -10865,14 +11090,15 @@
         return self
 
 
 class PatchEventRequest(TeaModel):
     def __init__(
         self,
         attendees: List[PatchEventRequestAttendees] = None,
+        card_instances: List[PatchEventRequestCardInstances] = None,
         description: str = None,
         end: PatchEventRequestEnd = None,
         extra: Dict[str, str] = None,
         id: str = None,
         is_all_day: bool = None,
         location: PatchEventRequestLocation = None,
         online_meeting_info: PatchEventRequestOnlineMeetingInfo = None,
@@ -10880,14 +11106,15 @@
         reminders: List[PatchEventRequestReminders] = None,
         rich_text_description: PatchEventRequestRichTextDescription = None,
         start: PatchEventRequestStart = None,
         summary: str = None,
         ui_configs: List[PatchEventRequestUiConfigs] = None,
     ):
         self.attendees = attendees
+        self.card_instances = card_instances
         self.description = description
         self.end = end
         self.extra = extra
         # This parameter is required.
         self.id = id
         self.is_all_day = is_all_day
         self.location = location
@@ -10900,14 +11127,18 @@
         self.ui_configs = ui_configs
 
     def validate(self):
         if self.attendees:
             for k in self.attendees:
                 if k:
                     k.validate()
+        if self.card_instances:
+            for k in self.card_instances:
+                if k:
+                    k.validate()
         if self.end:
             self.end.validate()
         if self.location:
             self.location.validate()
         if self.online_meeting_info:
             self.online_meeting_info.validate()
         if self.recurrence:
@@ -10931,14 +11162,18 @@
             return _map
 
         result = dict()
         result['attendees'] = []
         if self.attendees is not None:
             for k in self.attendees:
                 result['attendees'].append(k.to_map() if k else None)
+        result['cardInstances'] = []
+        if self.card_instances is not None:
+            for k in self.card_instances:
+                result['cardInstances'].append(k.to_map() if k else None)
         if self.description is not None:
             result['description'] = self.description
         if self.end is not None:
             result['end'] = self.end.to_map()
         if self.extra is not None:
             result['extra'] = self.extra
         if self.id is not None:
@@ -10970,14 +11205,19 @@
     def from_map(self, m: dict = None):
         m = m or dict()
         self.attendees = []
         if m.get('attendees') is not None:
             for k in m.get('attendees'):
                 temp_model = PatchEventRequestAttendees()
                 self.attendees.append(temp_model.from_map(k))
+        self.card_instances = []
+        if m.get('cardInstances') is not None:
+            for k in m.get('cardInstances'):
+                temp_model = PatchEventRequestCardInstances()
+                self.card_instances.append(temp_model.from_map(k))
         if m.get('description') is not None:
             self.description = m.get('description')
         if m.get('end') is not None:
             temp_model = PatchEventRequestEnd()
             self.end = temp_model.from_map(m['end'])
         if m.get('extra') is not None:
             self.extra = m.get('extra')
@@ -11062,14 +11302,47 @@
         if m.get('responseStatus') is not None:
             self.response_status = m.get('responseStatus')
         if m.get('self') is not None:
             self.self_ = m.get('self')
         return self
 
 
+class PatchEventResponseBodyCardInstances(TeaModel):
+    def __init__(
+        self,
+        out_track_id: str = None,
+        scenario: str = None,
+    ):
+        self.out_track_id = out_track_id
+        self.scenario = scenario
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.out_track_id is not None:
+            result['outTrackId'] = self.out_track_id
+        if self.scenario is not None:
+            result['scenario'] = self.scenario
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('outTrackId') is not None:
+            self.out_track_id = m.get('outTrackId')
+        if m.get('scenario') is not None:
+            self.scenario = m.get('scenario')
+        return self
+
+
 class PatchEventResponseBodyEnd(TeaModel):
     def __init__(
         self,
         date: str = None,
         date_time: str = None,
         time_zone: str = None,
     ):
@@ -11491,14 +11764,15 @@
         return self
 
 
 class PatchEventResponseBody(TeaModel):
     def __init__(
         self,
         attendees: List[PatchEventResponseBodyAttendees] = None,
+        card_instances: List[PatchEventResponseBodyCardInstances] = None,
         create_time: str = None,
         description: str = None,
         end: PatchEventResponseBodyEnd = None,
         id: str = None,
         is_all_day: bool = None,
         location: PatchEventResponseBodyLocation = None,
         online_meeting_info: PatchEventResponseBodyOnlineMeetingInfo = None,
@@ -11508,14 +11782,15 @@
         rich_text_description: PatchEventResponseBodyRichTextDescription = None,
         start: PatchEventResponseBodyStart = None,
         summary: str = None,
         ui_configs: List[PatchEventResponseBodyUiConfigs] = None,
         update_time: str = None,
     ):
         self.attendees = attendees
+        self.card_instances = card_instances
         # Use the UTC time format: yyyy-MM-ddTHH:mmZ
         self.create_time = create_time
         self.description = description
         self.end = end
         self.id = id
         self.is_all_day = is_all_day
         self.location = location
@@ -11532,14 +11807,18 @@
         self.update_time = update_time
 
     def validate(self):
         if self.attendees:
             for k in self.attendees:
                 if k:
                     k.validate()
+        if self.card_instances:
+            for k in self.card_instances:
+                if k:
+                    k.validate()
         if self.end:
             self.end.validate()
         if self.location:
             self.location.validate()
         if self.online_meeting_info:
             self.online_meeting_info.validate()
         if self.organizer:
@@ -11565,14 +11844,18 @@
             return _map
 
         result = dict()
         result['attendees'] = []
         if self.attendees is not None:
             for k in self.attendees:
                 result['attendees'].append(k.to_map() if k else None)
+        result['cardInstances'] = []
+        if self.card_instances is not None:
+            for k in self.card_instances:
+                result['cardInstances'].append(k.to_map() if k else None)
         if self.create_time is not None:
             result['createTime'] = self.create_time
         if self.description is not None:
             result['description'] = self.description
         if self.end is not None:
             result['end'] = self.end.to_map()
         if self.id is not None:
@@ -11608,14 +11891,19 @@
     def from_map(self, m: dict = None):
         m = m or dict()
         self.attendees = []
         if m.get('attendees') is not None:
             for k in m.get('attendees'):
                 temp_model = PatchEventResponseBodyAttendees()
                 self.attendees.append(temp_model.from_map(k))
+        self.card_instances = []
+        if m.get('cardInstances') is not None:
+            for k in m.get('cardInstances'):
+                temp_model = PatchEventResponseBodyCardInstances()
+                self.card_instances.append(temp_model.from_map(k))
         if m.get('createTime') is not None:
             self.create_time = m.get('createTime')
         if m.get('description') is not None:
             self.description = m.get('description')
         if m.get('end') is not None:
             temp_model = PatchEventResponseBodyEnd()
             self.end = temp_model.from_map(m['end'])
```

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/carbon_1_0/client.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/carbon_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/carbon_1_0/models.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/carbon_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/card_1_0/client.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/card_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/card_1_0/models.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/card_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/check_in_1_0/client.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/check_in_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/check_in_1_0/models.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/check_in_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/chengfeng_1_0/client.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/chengfeng_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/chengfeng_1_0/models.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/chengfeng_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/conference_1_0/client.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/conference_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/conference_1_0/models.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/conference_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/connector_1_0/client.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/connector_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/connector_1_0/models.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/connector_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/contact_1_0/client.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/contact_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/contact_1_0/models.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/contact_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/content_1_0/client.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/content_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/content_1_0/models.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/content_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/contract_1_0/client.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/contract_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/contract_1_0/models.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/contract_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/conv_file_1_0/client.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/conv_file_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/conv_file_1_0/models.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/conv_file_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/cool_app_1_0/client.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/cool_app_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/cool_app_1_0/models.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/cool_app_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/cool_ops_1_0/client.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/cool_ops_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/cool_ops_1_0/models.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/cool_ops_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/credit_1_0/client.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/credit_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/credit_1_0/models.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/credit_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/crm_1_0/client.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/crm_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/crm_1_0/models.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/crm_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/crm_2_0/client.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/crm_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/crm_2_0/models.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/crm_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/customer_service_1_0/client.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/customer_service_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/customer_service_1_0/models.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/customer_service_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/datacenter_1_0/client.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/datacenter_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/datacenter_1_0/models.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/datacenter_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/devicemng_1_0/client.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/devicemng_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/devicemng_1_0/models.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/devicemng_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/ding_phone_1_0/client.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/ding_phone_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/ding_phone_1_0/models.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/ding_phone_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/dingmi_1_0/client.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/dingmi_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/dingmi_1_0/models.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/dingmi_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/diot_1_0/client.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/diot_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/diot_1_0/models.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/diot_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/doc_1_0/client.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/doc_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/doc_1_0/models.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/doc_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/doc_2_0/client.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/doc_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/doc_2_0/models.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/doc_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/dpaas_1_0/client.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/dpaas_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/dpaas_1_0/models.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/dpaas_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/drive_1_0/client.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/drive_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/drive_1_0/models.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/drive_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/edu_1_0/client.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/edu_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/edu_1_0/models.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/edu_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/esign_1_0/client.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/esign_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/esign_1_0/models.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/esign_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/esign_2_0/client.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/esign_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/esign_2_0/models.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/esign_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/event_1_0/client.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/event_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/event_1_0/models.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/event_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/exclusive_1_0/client.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/exclusive_1_0/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -4707,14 +4707,136 @@
         @param request: GetMsgConfigRequest
         @return: GetMsgConfigResponse
         """
         runtime = util_models.RuntimeOptions()
         headers = dingtalkexclusive__1__0_models.GetMsgConfigHeaders()
         return await self.get_msg_config_with_options_async(request, headers, runtime)
 
+    def get_msg_location_with_options(
+        self,
+        request: dingtalkexclusive__1__0_models.GetMsgLocationRequest,
+        headers: dingtalkexclusive__1__0_models.GetMsgLocationHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkexclusive__1__0_models.GetMsgLocationResponse:
+        """
+        @summary 获取消息定位链接
+        
+        @param request: GetMsgLocationRequest
+        @param headers: GetMsgLocationHeaders
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetMsgLocationResponse
+        """
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.open_conversation_id):
+            body['openConversationId'] = request.open_conversation_id
+        if not UtilClient.is_unset(request.open_msg_id):
+            body['openMsgId'] = request.open_msg_id
+        if not UtilClient.is_unset(request.user_id):
+            body['userId'] = request.user_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='GetMsgLocation',
+            version='exclusive_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/exclusive/messageLocations/query',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkexclusive__1__0_models.GetMsgLocationResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def get_msg_location_with_options_async(
+        self,
+        request: dingtalkexclusive__1__0_models.GetMsgLocationRequest,
+        headers: dingtalkexclusive__1__0_models.GetMsgLocationHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkexclusive__1__0_models.GetMsgLocationResponse:
+        """
+        @summary 获取消息定位链接
+        
+        @param request: GetMsgLocationRequest
+        @param headers: GetMsgLocationHeaders
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetMsgLocationResponse
+        """
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.open_conversation_id):
+            body['openConversationId'] = request.open_conversation_id
+        if not UtilClient.is_unset(request.open_msg_id):
+            body['openMsgId'] = request.open_msg_id
+        if not UtilClient.is_unset(request.user_id):
+            body['userId'] = request.user_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='GetMsgLocation',
+            version='exclusive_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/exclusive/messageLocations/query',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkexclusive__1__0_models.GetMsgLocationResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def get_msg_location(
+        self,
+        request: dingtalkexclusive__1__0_models.GetMsgLocationRequest,
+    ) -> dingtalkexclusive__1__0_models.GetMsgLocationResponse:
+        """
+        @summary 获取消息定位链接
+        
+        @param request: GetMsgLocationRequest
+        @return: GetMsgLocationResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkexclusive__1__0_models.GetMsgLocationHeaders()
+        return self.get_msg_location_with_options(request, headers, runtime)
+
+    async def get_msg_location_async(
+        self,
+        request: dingtalkexclusive__1__0_models.GetMsgLocationRequest,
+    ) -> dingtalkexclusive__1__0_models.GetMsgLocationResponse:
+        """
+        @summary 获取消息定位链接
+        
+        @param request: GetMsgLocationRequest
+        @return: GetMsgLocationResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkexclusive__1__0_models.GetMsgLocationHeaders()
+        return await self.get_msg_location_with_options_async(request, headers, runtime)
+
     def get_oa_operator_log_list_with_options(
         self,
         request: dingtalkexclusive__1__0_models.GetOaOperatorLogListRequest,
         headers: dingtalkexclusive__1__0_models.GetOaOperatorLogListHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkexclusive__1__0_models.GetOaOperatorLogListResponse:
         """
```

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/exclusive_1_0/models.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/exclusive_1_0/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -7359,14 +7359,157 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = GetMsgConfigResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class GetMsgLocationHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class GetMsgLocationRequest(TeaModel):
+    def __init__(
+        self,
+        open_conversation_id: str = None,
+        open_msg_id: str = None,
+        user_id: str = None,
+    ):
+        # This parameter is required.
+        self.open_conversation_id = open_conversation_id
+        # This parameter is required.
+        self.open_msg_id = open_msg_id
+        # This parameter is required.
+        self.user_id = user_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.open_conversation_id is not None:
+            result['openConversationId'] = self.open_conversation_id
+        if self.open_msg_id is not None:
+            result['openMsgId'] = self.open_msg_id
+        if self.user_id is not None:
+            result['userId'] = self.user_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('openConversationId') is not None:
+            self.open_conversation_id = m.get('openConversationId')
+        if m.get('openMsgId') is not None:
+            self.open_msg_id = m.get('openMsgId')
+        if m.get('userId') is not None:
+            self.user_id = m.get('userId')
+        return self
+
+
+class GetMsgLocationResponseBody(TeaModel):
+    def __init__(
+        self,
+        msg_location_url: str = None,
+    ):
+        self.msg_location_url = msg_location_url
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.msg_location_url is not None:
+            result['msgLocationUrl'] = self.msg_location_url
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('msgLocationUrl') is not None:
+            self.msg_location_url = m.get('msgLocationUrl')
+        return self
+
+
+class GetMsgLocationResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: GetMsgLocationResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = GetMsgLocationResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class GetOaOperatorLogListHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
```

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/finance_1_0/client.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/finance_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/finance_1_0/models.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/finance_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/flashmeeting_1_0/client.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/flashmeeting_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/flashmeeting_1_0/models.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/flashmeeting_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/flashmsg_1_0/client.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/flashmsg_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/flashmsg_1_0/models.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/flashmsg_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/gateway_1_0/client.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/gateway_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/gateway_1_0/models.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/gateway_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/group_blackboard_1_0/client.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/group_blackboard_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/group_blackboard_1_0/models.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/group_blackboard_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/h3yun_1_0/client.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/h3yun_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/h3yun_1_0/models.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/h3yun_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/h5package_1_0/client.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/h5package_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/h5package_1_0/models.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/h5package_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/hrbrain_1_0/client.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/hrbrain_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/hrbrain_1_0/models.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/hrbrain_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/hrm_1_0/client.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/hrm_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/hrm_1_0/models.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/hrm_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/im_1_0/client.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/im_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/im_1_0/models.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/im_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/im_2_0/client.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/im_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/im_2_0/models.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/im_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/impaas_1_0/client.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/impaas_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/impaas_1_0/models.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/impaas_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/industry_1_0/client.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/industry_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/industry_1_0/models.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/industry_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/jzcrm_1_0/client.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/jzcrm_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/jzcrm_1_0/models.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/jzcrm_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/link_1_0/client.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/link_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/link_1_0/models.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/link_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/live_1_0/client.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/live_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/live_1_0/models.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/live_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/live_activities_1_0/client.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/live_activities_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/live_activities_1_0/models.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/live_activities_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/mail_1_0/client.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/mail_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/mail_1_0/models.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/mail_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/manufacturing_1_0/client.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/manufacturing_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/manufacturing_1_0/models.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/manufacturing_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/micro_app_1_0/client.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/micro_app_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/micro_app_1_0/models.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/micro_app_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/miniapp_1_0/client.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/miniapp_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/miniapp_1_0/models.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/miniapp_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/notable_1_0/client.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/notable_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/notable_1_0/models.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/notable_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/oauth2_1_0/client.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/oauth2_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/oauth2_1_0/models.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/oauth2_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/occupationauth_1_0/client.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/occupationauth_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/occupationauth_1_0/models.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/occupationauth_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/okr_1_0/client.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/okr_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/okr_1_0/models.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/okr_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/org_culture_1_0/client.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/org_culture_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/org_culture_1_0/models.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/org_culture_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/package_1_0/client.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/package_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/package_1_0/models.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/package_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/pedia_1_0/client.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/pedia_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/pedia_1_0/models.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/pedia_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/project_1_0/client.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/project_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/project_1_0/models.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/project_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/project_integration_1_0/client.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/project_integration_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/project_integration_1_0/models.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/project_integration_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/rcs_call_1_0/client.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/rcs_call_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/rcs_call_1_0/models.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/rcs_call_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/report_1_0/client.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/report_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/report_1_0/models.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/report_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/resident_1_0/client.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/resident_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/resident_1_0/models.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/resident_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/robot_1_0/client.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/robot_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/robot_1_0/models.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/robot_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/rooms_1_0/client.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/rooms_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/rooms_1_0/models.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/rooms_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/search_1_0/client.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/search_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/search_1_0/models.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/search_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/service_group_1_0/client.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/service_group_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/service_group_1_0/models.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/service_group_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/smart_device_1_0/client.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/smart_device_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/smart_device_1_0/models.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/smart_device_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/sns_storage_1_0/client.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/sns_storage_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/sns_storage_1_0/models.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/sns_storage_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/storage_1_0/client.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/storage_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/storage_1_0/models.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/storage_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/storage_2_0/client.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/storage_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/storage_2_0/models.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/storage_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/swform_1_0/client.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/swform_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/swform_1_0/models.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/swform_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/todo_1_0/client.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/todo_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/todo_1_0/models.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/todo_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/trade_1_0/client.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/trade_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/trade_1_0/models.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/trade_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/trajectory_1_0/client.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/trajectory_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/trajectory_1_0/models.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/trajectory_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/transcribe_1_0/client.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/transcribe_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/transcribe_1_0/models.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/transcribe_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/trip_1_0/client.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/trip_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/trip_1_0/models.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/trip_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/village_1_0/client.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/village_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/village_1_0/models.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/village_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/watt_1_0/client.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/watt_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/watt_1_0/models.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/watt_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/wiki_1_0/client.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/wiki_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/wiki_1_0/models.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/wiki_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/wiki_2_0/client.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/wiki_2_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/wiki_2_0/models.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/wiki_2_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/wms_1_0/client.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/wms_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/wms_1_0/models.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/wms_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/workbench_1_0/client.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/workbench_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/workbench_1_0/models.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/workbench_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/workflow_1_0/client.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/workflow_1_0/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -395,14 +395,140 @@
         @param request: BatchExecuteProcessInstancesRequest
         @return: BatchExecuteProcessInstancesResponse
         """
         runtime = util_models.RuntimeOptions()
         headers = dingtalkworkflow__1__0_models.BatchExecuteProcessInstancesHeaders()
         return await self.batch_execute_process_instances_with_options_async(request, headers, runtime)
 
+    def batch_tasks_redirect_with_options(
+        self,
+        request: dingtalkworkflow__1__0_models.BatchTasksRedirectRequest,
+        headers: dingtalkworkflow__1__0_models.BatchTasksRedirectHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkworkflow__1__0_models.BatchTasksRedirectResponse:
+        """
+        @summary 批量流程审批任务转交
+        
+        @param request: BatchTasksRedirectRequest
+        @param headers: BatchTasksRedirectHeaders
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: BatchTasksRedirectResponse
+        """
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.handover_user_id):
+            body['handoverUserId'] = request.handover_user_id
+        if not UtilClient.is_unset(request.manager_user_id):
+            body['managerUserId'] = request.manager_user_id
+        if not UtilClient.is_unset(request.task_ids):
+            body['taskIds'] = request.task_ids
+        if not UtilClient.is_unset(request.transferee_user_id):
+            body['transfereeUserId'] = request.transferee_user_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='BatchTasksRedirect',
+            version='workflow_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/workflow/tasks/batchRedirect',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkworkflow__1__0_models.BatchTasksRedirectResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def batch_tasks_redirect_with_options_async(
+        self,
+        request: dingtalkworkflow__1__0_models.BatchTasksRedirectRequest,
+        headers: dingtalkworkflow__1__0_models.BatchTasksRedirectHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkworkflow__1__0_models.BatchTasksRedirectResponse:
+        """
+        @summary 批量流程审批任务转交
+        
+        @param request: BatchTasksRedirectRequest
+        @param headers: BatchTasksRedirectHeaders
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: BatchTasksRedirectResponse
+        """
+        UtilClient.validate_model(request)
+        body = {}
+        if not UtilClient.is_unset(request.handover_user_id):
+            body['handoverUserId'] = request.handover_user_id
+        if not UtilClient.is_unset(request.manager_user_id):
+            body['managerUserId'] = request.manager_user_id
+        if not UtilClient.is_unset(request.task_ids):
+            body['taskIds'] = request.task_ids
+        if not UtilClient.is_unset(request.transferee_user_id):
+            body['transfereeUserId'] = request.transferee_user_id
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            body=OpenApiUtilClient.parse_to_map(body)
+        )
+        params = open_api_models.Params(
+            action='BatchTasksRedirect',
+            version='workflow_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/workflow/tasks/batchRedirect',
+            method='POST',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkworkflow__1__0_models.BatchTasksRedirectResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def batch_tasks_redirect(
+        self,
+        request: dingtalkworkflow__1__0_models.BatchTasksRedirectRequest,
+    ) -> dingtalkworkflow__1__0_models.BatchTasksRedirectResponse:
+        """
+        @summary 批量流程审批任务转交
+        
+        @param request: BatchTasksRedirectRequest
+        @return: BatchTasksRedirectResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkworkflow__1__0_models.BatchTasksRedirectHeaders()
+        return self.batch_tasks_redirect_with_options(request, headers, runtime)
+
+    async def batch_tasks_redirect_async(
+        self,
+        request: dingtalkworkflow__1__0_models.BatchTasksRedirectRequest,
+    ) -> dingtalkworkflow__1__0_models.BatchTasksRedirectResponse:
+        """
+        @summary 批量流程审批任务转交
+        
+        @param request: BatchTasksRedirectRequest
+        @return: BatchTasksRedirectResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkworkflow__1__0_models.BatchTasksRedirectHeaders()
+        return await self.batch_tasks_redirect_with_options_async(request, headers, runtime)
+
     def batch_update_process_instance_with_options(
         self,
         request: dingtalkworkflow__1__0_models.BatchUpdateProcessInstanceRequest,
         headers: dingtalkworkflow__1__0_models.BatchUpdateProcessInstanceHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkworkflow__1__0_models.BatchUpdateProcessInstanceResponse:
         """
@@ -5573,14 +5699,140 @@
         @param request: TerminateProcessInstanceRequest
         @return: TerminateProcessInstanceResponse
         """
         runtime = util_models.RuntimeOptions()
         headers = dingtalkworkflow__1__0_models.TerminateProcessInstanceHeaders()
         return await self.terminate_process_instance_with_options_async(request, headers, runtime)
 
+    def todo_tasks_with_options(
+        self,
+        request: dingtalkworkflow__1__0_models.TodoTasksRequest,
+        headers: dingtalkworkflow__1__0_models.TodoTasksHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkworkflow__1__0_models.TodoTasksResponse:
+        """
+        @summary 流程转交待处理任务查询
+        
+        @param request: TodoTasksRequest
+        @param headers: TodoTasksHeaders
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: TodoTasksResponse
+        """
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.actioner_user_id):
+            query['actionerUserId'] = request.actioner_user_id
+        if not UtilClient.is_unset(request.manager_user_id):
+            query['managerUserId'] = request.manager_user_id
+        if not UtilClient.is_unset(request.max_results):
+            query['maxResults'] = request.max_results
+        if not UtilClient.is_unset(request.next_token):
+            query['nextToken'] = request.next_token
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='TodoTasks',
+            version='workflow_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/workflow/tasks/todoTasks',
+            method='GET',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkworkflow__1__0_models.TodoTasksResponse(),
+            self.execute(params, req, runtime)
+        )
+
+    async def todo_tasks_with_options_async(
+        self,
+        request: dingtalkworkflow__1__0_models.TodoTasksRequest,
+        headers: dingtalkworkflow__1__0_models.TodoTasksHeaders,
+        runtime: util_models.RuntimeOptions,
+    ) -> dingtalkworkflow__1__0_models.TodoTasksResponse:
+        """
+        @summary 流程转交待处理任务查询
+        
+        @param request: TodoTasksRequest
+        @param headers: TodoTasksHeaders
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: TodoTasksResponse
+        """
+        UtilClient.validate_model(request)
+        query = {}
+        if not UtilClient.is_unset(request.actioner_user_id):
+            query['actionerUserId'] = request.actioner_user_id
+        if not UtilClient.is_unset(request.manager_user_id):
+            query['managerUserId'] = request.manager_user_id
+        if not UtilClient.is_unset(request.max_results):
+            query['maxResults'] = request.max_results
+        if not UtilClient.is_unset(request.next_token):
+            query['nextToken'] = request.next_token
+        real_headers = {}
+        if not UtilClient.is_unset(headers.common_headers):
+            real_headers = headers.common_headers
+        if not UtilClient.is_unset(headers.x_acs_dingtalk_access_token):
+            real_headers['x-acs-dingtalk-access-token'] = UtilClient.to_jsonstring(headers.x_acs_dingtalk_access_token)
+        req = open_api_models.OpenApiRequest(
+            headers=real_headers,
+            query=OpenApiUtilClient.query(query)
+        )
+        params = open_api_models.Params(
+            action='TodoTasks',
+            version='workflow_1.0',
+            protocol='HTTP',
+            pathname=f'/v1.0/workflow/tasks/todoTasks',
+            method='GET',
+            auth_type='AK',
+            style='ROA',
+            req_body_type='none',
+            body_type='json'
+        )
+        return TeaCore.from_map(
+            dingtalkworkflow__1__0_models.TodoTasksResponse(),
+            await self.execute_async(params, req, runtime)
+        )
+
+    def todo_tasks(
+        self,
+        request: dingtalkworkflow__1__0_models.TodoTasksRequest,
+    ) -> dingtalkworkflow__1__0_models.TodoTasksResponse:
+        """
+        @summary 流程转交待处理任务查询
+        
+        @param request: TodoTasksRequest
+        @return: TodoTasksResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkworkflow__1__0_models.TodoTasksHeaders()
+        return self.todo_tasks_with_options(request, headers, runtime)
+
+    async def todo_tasks_async(
+        self,
+        request: dingtalkworkflow__1__0_models.TodoTasksRequest,
+    ) -> dingtalkworkflow__1__0_models.TodoTasksResponse:
+        """
+        @summary 流程转交待处理任务查询
+        
+        @param request: TodoTasksRequest
+        @return: TodoTasksResponse
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = dingtalkworkflow__1__0_models.TodoTasksHeaders()
+        return await self.todo_tasks_with_options_async(request, headers, runtime)
+
     def update_integrated_task_with_options(
         self,
         request: dingtalkworkflow__1__0_models.UpdateIntegratedTaskRequest,
         headers: dingtalkworkflow__1__0_models.UpdateIntegratedTaskHeaders,
         runtime: util_models.RuntimeOptions,
     ) -> dingtalkworkflow__1__0_models.UpdateIntegratedTaskResponse:
         """
```

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/workflow_1_0/models.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/workflow_1_0/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1171,14 +1171,263 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = BatchExecuteProcessInstancesResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class BatchTasksRedirectHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class BatchTasksRedirectRequest(TeaModel):
+    def __init__(
+        self,
+        handover_user_id: str = None,
+        manager_user_id: str = None,
+        task_ids: List[int] = None,
+        transferee_user_id: str = None,
+    ):
+        # This parameter is required.
+        self.handover_user_id = handover_user_id
+        # This parameter is required.
+        self.manager_user_id = manager_user_id
+        # This parameter is required.
+        self.task_ids = task_ids
+        # This parameter is required.
+        self.transferee_user_id = transferee_user_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.handover_user_id is not None:
+            result['handoverUserId'] = self.handover_user_id
+        if self.manager_user_id is not None:
+            result['managerUserId'] = self.manager_user_id
+        if self.task_ids is not None:
+            result['taskIds'] = self.task_ids
+        if self.transferee_user_id is not None:
+            result['transfereeUserId'] = self.transferee_user_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('handoverUserId') is not None:
+            self.handover_user_id = m.get('handoverUserId')
+        if m.get('managerUserId') is not None:
+            self.manager_user_id = m.get('managerUserId')
+        if m.get('taskIds') is not None:
+            self.task_ids = m.get('taskIds')
+        if m.get('transfereeUserId') is not None:
+            self.transferee_user_id = m.get('transfereeUserId')
+        return self
+
+
+class BatchTasksRedirectResponseBodyResultRedirectResults(TeaModel):
+    def __init__(
+        self,
+        error_msg: str = None,
+        success: bool = None,
+        task_id: int = None,
+    ):
+        self.error_msg = error_msg
+        # This parameter is required.
+        self.success = success
+        # This parameter is required.
+        self.task_id = task_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.error_msg is not None:
+            result['errorMsg'] = self.error_msg
+        if self.success is not None:
+            result['success'] = self.success
+        if self.task_id is not None:
+            result['taskId'] = self.task_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('errorMsg') is not None:
+            self.error_msg = m.get('errorMsg')
+        if m.get('success') is not None:
+            self.success = m.get('success')
+        if m.get('taskId') is not None:
+            self.task_id = m.get('taskId')
+        return self
+
+
+class BatchTasksRedirectResponseBodyResult(TeaModel):
+    def __init__(
+        self,
+        fail_count: int = None,
+        redirect_results: List[BatchTasksRedirectResponseBodyResultRedirectResults] = None,
+        total_count: int = None,
+    ):
+        # This parameter is required.
+        self.fail_count = fail_count
+        # This parameter is required.
+        self.redirect_results = redirect_results
+        # This parameter is required.
+        self.total_count = total_count
+
+    def validate(self):
+        if self.redirect_results:
+            for k in self.redirect_results:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.fail_count is not None:
+            result['failCount'] = self.fail_count
+        result['redirectResults'] = []
+        if self.redirect_results is not None:
+            for k in self.redirect_results:
+                result['redirectResults'].append(k.to_map() if k else None)
+        if self.total_count is not None:
+            result['totalCount'] = self.total_count
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('failCount') is not None:
+            self.fail_count = m.get('failCount')
+        self.redirect_results = []
+        if m.get('redirectResults') is not None:
+            for k in m.get('redirectResults'):
+                temp_model = BatchTasksRedirectResponseBodyResultRedirectResults()
+                self.redirect_results.append(temp_model.from_map(k))
+        if m.get('totalCount') is not None:
+            self.total_count = m.get('totalCount')
+        return self
+
+
+class BatchTasksRedirectResponseBody(TeaModel):
+    def __init__(
+        self,
+        result: BatchTasksRedirectResponseBodyResult = None,
+        success: bool = None,
+    ):
+        self.result = result
+        self.success = success
+
+    def validate(self):
+        if self.result:
+            self.result.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.result is not None:
+            result['result'] = self.result.to_map()
+        if self.success is not None:
+            result['success'] = self.success
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('result') is not None:
+            temp_model = BatchTasksRedirectResponseBodyResult()
+            self.result = temp_model.from_map(m['result'])
+        if m.get('success') is not None:
+            self.success = m.get('success')
+        return self
+
+
+class BatchTasksRedirectResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: BatchTasksRedirectResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = BatchTasksRedirectResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class BatchUpdateProcessInstanceHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
@@ -13423,14 +13672,276 @@
             self.status_code = m.get('statusCode')
         if m.get('body') is not None:
             temp_model = TerminateProcessInstanceResponseBody()
             self.body = temp_model.from_map(m['body'])
         return self
 
 
+class TodoTasksHeaders(TeaModel):
+    def __init__(
+        self,
+        common_headers: Dict[str, str] = None,
+        x_acs_dingtalk_access_token: str = None,
+    ):
+        self.common_headers = common_headers
+        self.x_acs_dingtalk_access_token = x_acs_dingtalk_access_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.common_headers is not None:
+            result['commonHeaders'] = self.common_headers
+        if self.x_acs_dingtalk_access_token is not None:
+            result['x-acs-dingtalk-access-token'] = self.x_acs_dingtalk_access_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('commonHeaders') is not None:
+            self.common_headers = m.get('commonHeaders')
+        if m.get('x-acs-dingtalk-access-token') is not None:
+            self.x_acs_dingtalk_access_token = m.get('x-acs-dingtalk-access-token')
+        return self
+
+
+class TodoTasksRequest(TeaModel):
+    def __init__(
+        self,
+        actioner_user_id: str = None,
+        manager_user_id: str = None,
+        max_results: int = None,
+        next_token: int = None,
+    ):
+        # This parameter is required.
+        self.actioner_user_id = actioner_user_id
+        # This parameter is required.
+        self.manager_user_id = manager_user_id
+        # This parameter is required.
+        self.max_results = max_results
+        # This parameter is required.
+        self.next_token = next_token
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.actioner_user_id is not None:
+            result['actionerUserId'] = self.actioner_user_id
+        if self.manager_user_id is not None:
+            result['managerUserId'] = self.manager_user_id
+        if self.max_results is not None:
+            result['maxResults'] = self.max_results
+        if self.next_token is not None:
+            result['nextToken'] = self.next_token
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('actionerUserId') is not None:
+            self.actioner_user_id = m.get('actionerUserId')
+        if m.get('managerUserId') is not None:
+            self.manager_user_id = m.get('managerUserId')
+        if m.get('maxResults') is not None:
+            self.max_results = m.get('maxResults')
+        if m.get('nextToken') is not None:
+            self.next_token = m.get('nextToken')
+        return self
+
+
+class TodoTasksResponseBodyResultList(TeaModel):
+    def __init__(
+        self,
+        business_id: str = None,
+        can_redirect: bool = None,
+        create_time: int = None,
+        process_code: str = None,
+        process_instance_id: str = None,
+        task_id: int = None,
+        title: str = None,
+        user_id: str = None,
+    ):
+        self.business_id = business_id
+        self.can_redirect = can_redirect
+        self.create_time = create_time
+        self.process_code = process_code
+        self.process_instance_id = process_instance_id
+        self.task_id = task_id
+        self.title = title
+        self.user_id = user_id
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.business_id is not None:
+            result['businessId'] = self.business_id
+        if self.can_redirect is not None:
+            result['canRedirect'] = self.can_redirect
+        if self.create_time is not None:
+            result['createTime'] = self.create_time
+        if self.process_code is not None:
+            result['processCode'] = self.process_code
+        if self.process_instance_id is not None:
+            result['processInstanceId'] = self.process_instance_id
+        if self.task_id is not None:
+            result['taskId'] = self.task_id
+        if self.title is not None:
+            result['title'] = self.title
+        if self.user_id is not None:
+            result['userId'] = self.user_id
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('businessId') is not None:
+            self.business_id = m.get('businessId')
+        if m.get('canRedirect') is not None:
+            self.can_redirect = m.get('canRedirect')
+        if m.get('createTime') is not None:
+            self.create_time = m.get('createTime')
+        if m.get('processCode') is not None:
+            self.process_code = m.get('processCode')
+        if m.get('processInstanceId') is not None:
+            self.process_instance_id = m.get('processInstanceId')
+        if m.get('taskId') is not None:
+            self.task_id = m.get('taskId')
+        if m.get('title') is not None:
+            self.title = m.get('title')
+        if m.get('userId') is not None:
+            self.user_id = m.get('userId')
+        return self
+
+
+class TodoTasksResponseBodyResult(TeaModel):
+    def __init__(
+        self,
+        has_more: str = None,
+        list: List[TodoTasksResponseBodyResultList] = None,
+    ):
+        self.has_more = has_more
+        self.list = list
+
+    def validate(self):
+        if self.list:
+            for k in self.list:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.has_more is not None:
+            result['hasMore'] = self.has_more
+        result['list'] = []
+        if self.list is not None:
+            for k in self.list:
+                result['list'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('hasMore') is not None:
+            self.has_more = m.get('hasMore')
+        self.list = []
+        if m.get('list') is not None:
+            for k in m.get('list'):
+                temp_model = TodoTasksResponseBodyResultList()
+                self.list.append(temp_model.from_map(k))
+        return self
+
+
+class TodoTasksResponseBody(TeaModel):
+    def __init__(
+        self,
+        result: TodoTasksResponseBodyResult = None,
+    ):
+        self.result = result
+
+    def validate(self):
+        if self.result:
+            self.result.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.result is not None:
+            result['result'] = self.result.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('result') is not None:
+            temp_model = TodoTasksResponseBodyResult()
+            self.result = temp_model.from_map(m['result'])
+        return self
+
+
+class TodoTasksResponse(TeaModel):
+    def __init__(
+        self,
+        headers: Dict[str, str] = None,
+        status_code: int = None,
+        body: TodoTasksResponseBody = None,
+    ):
+        self.headers = headers
+        self.status_code = status_code
+        self.body = body
+
+    def validate(self):
+        if self.body:
+            self.body.validate()
+
+    def to_map(self):
+        _map = super().to_map()
+        if _map is not None:
+            return _map
+
+        result = dict()
+        if self.headers is not None:
+            result['headers'] = self.headers
+        if self.status_code is not None:
+            result['statusCode'] = self.status_code
+        if self.body is not None:
+            result['body'] = self.body.to_map()
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('headers') is not None:
+            self.headers = m.get('headers')
+        if m.get('statusCode') is not None:
+            self.status_code = m.get('statusCode')
+        if m.get('body') is not None:
+            temp_model = TodoTasksResponseBody()
+            self.body = temp_model.from_map(m['body'])
+        return self
+
+
 class UpdateIntegratedTaskHeaders(TeaModel):
     def __init__(
         self,
         common_headers: Dict[str, str] = None,
         x_acs_dingtalk_access_token: str = None,
     ):
         self.common_headers = common_headers
```

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/workrecord_1_0/client.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/workrecord_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/workrecord_1_0/models.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/workrecord_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/yida_1_0/client.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/yida_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/yida_1_0/models.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/yida_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/yun_shu_1_0/client.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/yun_shu_1_0/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk/yun_shu_1_0/models.py` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk/yun_shu_1_0/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk.egg-info/PKG-INFO` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-dingtalk
-Version: 2.1.13
+Version: 2.1.14
 Summary: Alibaba Cloud Dingtalk SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_dingtalk-2.1.13/alibabacloud_dingtalk.egg-info/SOURCES.txt` & `alibabacloud_dingtalk-2.1.14/alibabacloud_dingtalk.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -10,14 +10,17 @@
 alibabacloud_dingtalk.egg-info/SOURCES.txt
 alibabacloud_dingtalk.egg-info/dependency_links.txt
 alibabacloud_dingtalk.egg-info/requires.txt
 alibabacloud_dingtalk.egg-info/top_level.txt
 alibabacloud_dingtalk/activity_1_0/__init__.py
 alibabacloud_dingtalk/activity_1_0/client.py
 alibabacloud_dingtalk/activity_1_0/models.py
+alibabacloud_dingtalk/agoal_1_0/__init__.py
+alibabacloud_dingtalk/agoal_1_0/client.py
+alibabacloud_dingtalk/agoal_1_0/models.py
 alibabacloud_dingtalk/ai_interaction_1_0/__init__.py
 alibabacloud_dingtalk/ai_interaction_1_0/client.py
 alibabacloud_dingtalk/ai_interaction_1_0/models.py
 alibabacloud_dingtalk/ai_paa_s_1_0/__init__.py
 alibabacloud_dingtalk/ai_paa_s_1_0/client.py
 alibabacloud_dingtalk/ai_paa_s_1_0/models.py
 alibabacloud_dingtalk/algo_1_0/__init__.py
```

### Comparing `alibabacloud_dingtalk-2.1.13/setup.py` & `alibabacloud_dingtalk-2.1.14/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_dingtalk.
 
-Created on 22/05/2024
+Created on 23/05/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_dingtalk"
 NAME = "alibabacloud_dingtalk" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Dingtalk SDK Library for Python"
```

