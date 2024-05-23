# Comparing `tmp/linktest-2.8.4.tar.gz` & `tmp/linktest-2.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linktest-2.8.4.tar", last modified: Wed May 22 08:26:48 2024, max compression
+gzip compressed data, was "linktest-2.8.6.tar", last modified: Thu May 23 14:59:54 2024, max compression
```

## Comparing `linktest-2.8.4.tar` & `linktest-2.8.6.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-05-22 08:26:48.355761 linktest-2.8.4/
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-05-22 08:26:48.355485 linktest-2.8.4/PKG-INFO
-drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-05-22 08:26:48.351803 linktest-2.8.4/linktest/
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       22 2024-05-22 08:23:18.000000 linktest-2.8.4/linktest/__init__.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      487 2024-05-17 06:35:25.000000 linktest-2.8.4/linktest/android_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      187 2024-05-17 06:35:25.000000 linktest-2.8.4/linktest/api_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10759 2024-05-17 06:35:25.000000 linktest-2.8.4/linktest/appium_utils.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    29054 2024-05-17 06:35:25.000000 linktest-2.8.4/linktest/auto_generate_testcase_list-backup.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    28841 2024-05-17 06:35:25.000000 linktest-2.8.4/linktest/auto_generate_testcase_list.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10326 2024-05-17 06:35:25.000000 linktest-2.8.4/linktest/auto_generate_testcase_list_from_csv.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     9984 2024-05-17 06:35:25.000000 linktest-2.8.4/linktest/base_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1792 2024-05-17 06:35:25.000000 linktest-2.8.4/linktest/clean_data.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1403 2024-05-17 06:35:25.000000 linktest-2.8.4/linktest/conver_xml_into_db.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     7817 2024-05-17 06:35:25.000000 linktest-2.8.4/linktest/database_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2471 2024-05-17 06:35:25.000000 linktest-2.8.4/linktest/date_utilities.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      232 2024-05-17 06:35:25.000000 linktest-2.8.4/linktest/detect_delimiter.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    16568 2024-05-17 06:35:25.000000 linktest-2.8.4/linktest/doctor.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      959 2024-05-17 06:35:25.000000 linktest-2.8.4/linktest/framework_log.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    16243 2024-05-17 06:35:25.000000 linktest-2.8.4/linktest/generate_html_log.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      987 2024-05-17 06:35:25.000000 linktest-2.8.4/linktest/get_adb_devices.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      924 2024-05-17 06:35:25.000000 linktest-2.8.4/linktest/get_ios_devices_list.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1775 2024-05-17 06:35:25.000000 linktest-2.8.4/linktest/get_platform_info.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3137 2024-05-17 06:35:25.000000 linktest-2.8.4/linktest/get_project_info.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    38554 2024-05-17 06:35:25.000000 linktest-2.8.4/linktest/html_report.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      280 2024-05-17 06:35:25.000000 linktest-2.8.4/linktest/ios_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      195 2024-05-17 06:35:25.000000 linktest-2.8.4/linktest/linktest_setup.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     8899 2024-05-17 06:35:25.000000 linktest-2.8.4/linktest/logged_requests.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)   102436 2024-05-22 08:21:55.000000 linktest-2.8.4/linktest/main.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      982 2024-05-17 06:35:25.000000 linktest-2.8.4/linktest/memory_usage.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     4811 2024-05-17 06:35:25.000000 linktest-2.8.4/linktest/re_func.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1334 2024-05-17 06:35:25.000000 linktest-2.8.4/linktest/run.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2170 2024-05-17 06:35:25.000000 linktest-2.8.4/linktest/run_testcase_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1048 2024-05-17 06:35:25.000000 linktest-2.8.4/linktest/scp_report_to_specified_path.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     9534 2024-05-17 06:35:25.000000 linktest-2.8.4/linktest/selenium_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      396 2024-05-17 06:35:25.000000 linktest-2.8.4/linktest/set_run_flag_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-05-22 08:23:23.000000 linktest-2.8.4/linktest/setup.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      173 2024-05-17 06:35:25.000000 linktest-2.8.4/linktest/testcase_order.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      140 2024-05-17 06:35:25.000000 linktest-2.8.4/linktest/testcase_timeout_exception.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      801 2024-05-17 06:35:25.000000 linktest-2.8.4/linktest/timeout_thread.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      931 2024-05-17 06:35:25.000000 linktest-2.8.4/linktest/ui_testcase.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3445 2024-05-17 06:35:25.000000 linktest-2.8.4/linktest/update_config.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    14288 2024-05-17 06:35:25.000000 linktest-2.8.4/linktest/webdriver_wrapper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    14075 2024-05-17 06:35:25.000000 linktest-2.8.4/linktest/webdriver_wrapper_chrome.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    13707 2024-05-17 06:35:25.000000 linktest-2.8.4/linktest/webdriver_wrapper_edge.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    13725 2024-05-17 06:35:25.000000 linktest-2.8.4/linktest/webdriver_wrapper_firefox.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    13695 2024-05-17 06:35:25.000000 linktest-2.8.4/linktest/webdriver_wrapper_ie.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    14139 2024-05-17 06:35:25.000000 linktest-2.8.4/linktest/webdriver_wrapper_safari.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      406 2024-05-17 06:35:25.000000 linktest-2.8.4/linktest/windows_helper.py
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3544 2024-05-17 06:35:25.000000 linktest-2.8.4/linktest/xml_report.py
-drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-05-22 08:26:48.355097 linktest-2.8.4/linktest.egg-info/
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-05-22 08:26:48.000000 linktest-2.8.4/linktest.egg-info/PKG-INFO
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1498 2024-05-22 08:26:48.000000 linktest-2.8.4/linktest.egg-info/SOURCES.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        1 2024-05-22 08:26:48.000000 linktest-2.8.4/linktest.egg-info/dependency_links.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      123 2024-05-22 08:26:48.000000 linktest-2.8.4/linktest.egg-info/requires.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        9 2024-05-22 08:26:48.000000 linktest-2.8.4/linktest.egg-info/top_level.txt
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       38 2024-05-22 08:26:48.355814 linktest-2.8.4/setup.cfg
--rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-05-22 08:26:42.000000 linktest-2.8.4/setup.py
+drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-05-23 14:59:54.465455 linktest-2.8.6/
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-05-23 14:59:54.465161 linktest-2.8.6/PKG-INFO
+drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-05-23 14:59:54.462285 linktest-2.8.6/linktest/
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       22 2024-05-23 14:24:46.000000 linktest-2.8.6/linktest/__init__.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      487 2024-05-22 08:27:18.000000 linktest-2.8.6/linktest/android_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      187 2024-05-22 08:27:18.000000 linktest-2.8.6/linktest/api_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10759 2024-05-22 08:27:18.000000 linktest-2.8.6/linktest/appium_utils.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    29054 2024-05-22 08:27:18.000000 linktest-2.8.6/linktest/auto_generate_testcase_list-backup.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    28841 2024-05-22 08:27:18.000000 linktest-2.8.6/linktest/auto_generate_testcase_list.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    10326 2024-05-22 08:27:18.000000 linktest-2.8.6/linktest/auto_generate_testcase_list_from_csv.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     9984 2024-05-22 08:27:18.000000 linktest-2.8.6/linktest/base_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1792 2024-05-22 08:27:18.000000 linktest-2.8.6/linktest/clean_data.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1403 2024-05-22 08:27:18.000000 linktest-2.8.6/linktest/conver_xml_into_db.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     7817 2024-05-22 08:27:18.000000 linktest-2.8.6/linktest/database_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2471 2024-05-22 08:27:18.000000 linktest-2.8.6/linktest/date_utilities.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      232 2024-05-22 08:27:18.000000 linktest-2.8.6/linktest/detect_delimiter.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    16958 2024-05-23 14:49:44.000000 linktest-2.8.6/linktest/doctor.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      959 2024-05-22 08:27:18.000000 linktest-2.8.6/linktest/framework_log.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    16243 2024-05-22 08:27:18.000000 linktest-2.8.6/linktest/generate_html_log.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      987 2024-05-22 08:27:18.000000 linktest-2.8.6/linktest/get_adb_devices.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      924 2024-05-22 08:27:18.000000 linktest-2.8.6/linktest/get_ios_devices_list.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1775 2024-05-22 08:27:18.000000 linktest-2.8.6/linktest/get_platform_info.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3137 2024-05-22 08:27:18.000000 linktest-2.8.6/linktest/get_project_info.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    38554 2024-05-22 08:27:18.000000 linktest-2.8.6/linktest/html_report.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      280 2024-05-22 08:27:18.000000 linktest-2.8.6/linktest/ios_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      195 2024-05-22 08:27:18.000000 linktest-2.8.6/linktest/linktest_setup.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     9581 2024-05-23 14:52:18.000000 linktest-2.8.6/linktest/logged_requests.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)   102433 2024-05-23 14:46:43.000000 linktest-2.8.6/linktest/main.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      982 2024-05-22 08:27:18.000000 linktest-2.8.6/linktest/memory_usage.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     4811 2024-05-22 08:27:18.000000 linktest-2.8.6/linktest/re_func.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1334 2024-05-22 08:27:18.000000 linktest-2.8.6/linktest/run.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     2170 2024-05-22 08:27:18.000000 linktest-2.8.6/linktest/run_testcase_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1048 2024-05-22 08:27:18.000000 linktest-2.8.6/linktest/scp_report_to_specified_path.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     9534 2024-05-22 08:27:18.000000 linktest-2.8.6/linktest/selenium_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      396 2024-05-22 08:27:18.000000 linktest-2.8.6/linktest/set_run_flag_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-05-23 14:24:51.000000 linktest-2.8.6/linktest/setup.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      173 2024-05-22 08:27:18.000000 linktest-2.8.6/linktest/testcase_order.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      140 2024-05-22 08:27:18.000000 linktest-2.8.6/linktest/testcase_timeout_exception.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      801 2024-05-22 08:27:18.000000 linktest-2.8.6/linktest/timeout_thread.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      931 2024-05-22 08:27:18.000000 linktest-2.8.6/linktest/ui_testcase.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3445 2024-05-22 08:27:18.000000 linktest-2.8.6/linktest/update_config.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    14288 2024-05-22 08:27:18.000000 linktest-2.8.6/linktest/webdriver_wrapper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    14075 2024-05-22 08:27:18.000000 linktest-2.8.6/linktest/webdriver_wrapper_chrome.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    13707 2024-05-22 08:27:18.000000 linktest-2.8.6/linktest/webdriver_wrapper_edge.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    13725 2024-05-22 08:27:18.000000 linktest-2.8.6/linktest/webdriver_wrapper_firefox.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    13695 2024-05-22 08:27:18.000000 linktest-2.8.6/linktest/webdriver_wrapper_ie.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)    14139 2024-05-22 08:27:18.000000 linktest-2.8.6/linktest/webdriver_wrapper_safari.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      406 2024-05-22 08:27:18.000000 linktest-2.8.6/linktest/windows_helper.py
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     3544 2024-05-22 08:27:18.000000 linktest-2.8.6/linktest/xml_report.py
+drwxr-xr-x   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        0 2024-05-23 14:59:54.464773 linktest-2.8.6/linktest.egg-info/
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      111 2024-05-23 14:59:54.000000 linktest-2.8.6/linktest.egg-info/PKG-INFO
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)     1498 2024-05-23 14:59:54.000000 linktest-2.8.6/linktest.egg-info/SOURCES.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        1 2024-05-23 14:59:54.000000 linktest-2.8.6/linktest.egg-info/dependency_links.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      123 2024-05-23 14:59:54.000000 linktest-2.8.6/linktest.egg-info/requires.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)        9 2024-05-23 14:59:54.000000 linktest-2.8.6/linktest.egg-info/top_level.txt
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)       38 2024-05-23 14:59:54.465505 linktest-2.8.6/setup.cfg
+-rw-r--r--   0 liwan76  (1619044882) IKEA\Domain Users (619956085)      452 2024-05-23 14:59:41.000000 linktest-2.8.6/setup.py
```

### Comparing `linktest-2.8.4/linktest/appium_utils.py` & `linktest-2.8.6/linktest/appium_utils.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.4/linktest/auto_generate_testcase_list-backup.py` & `linktest-2.8.6/linktest/auto_generate_testcase_list-backup.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.4/linktest/auto_generate_testcase_list.py` & `linktest-2.8.6/linktest/auto_generate_testcase_list.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.4/linktest/auto_generate_testcase_list_from_csv.py` & `linktest-2.8.6/linktest/auto_generate_testcase_list_from_csv.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.4/linktest/base_testcase.py` & `linktest-2.8.6/linktest/base_testcase.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.4/linktest/clean_data.py` & `linktest-2.8.6/linktest/clean_data.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.4/linktest/conver_xml_into_db.py` & `linktest-2.8.6/linktest/conver_xml_into_db.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.4/linktest/database_helper.py` & `linktest-2.8.6/linktest/database_helper.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.4/linktest/date_utilities.py` & `linktest-2.8.6/linktest/date_utilities.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.4/linktest/doctor.py` & `linktest-2.8.6/linktest/doctor.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,14 +42,16 @@
 #  19. ANDROID_TESTCASE_ACCOUNT
 #  20. SAVE_SCREENSHOT_FOR_PASSED_TESTS
 #  21. Configuration for Browser option ( update follow your business)
 #  22. generate_xunit_result (default value is False)
 #  23. AUTO_DOWNLOAD_CHROMEDRIVER (default value is False)
 #  24. ALWAYS_GENERATE_CURL (default value is False)
 #  25. AUTO_SCREENSHOT_ON_ACTION(default value is False)
+#  26. AUTO_LOG_HTTP_REQUEST (Whether to auto log request and response for API test cases. default is True)
+#  27. USE_JSON_INDENTATION (Whether to use JSON indentation in log. default is True)
 
 import logging
 
 # ------ testcase's log setting ------
 - LOG_LEVEL = logging.DEBUG # default value is DEBUG
 - LOG_TO_CONSOLE = True # default value is True
 
@@ -94,14 +96,20 @@
 
 # Whether to always generate a curl command for each test case regardless of its execution result (passed or failed). default value is False
 ALWAYS_GENERATE_CURL = False
 
 # auto download chromedriver, default value is False
 AUTO_DOWNLOAD_CHROMEDRIVER = False
 
+# Whether to auto log request and response for API test cases. default is True
+AUTO_LOG_HTTP_REQUEST = True
+
+# Whether to use JSON indentation in log. default is True
+USE_JSON_INDENTATION = True
+
 # configure for Database
 if ENVIRONMENT == Environment.UAT:
     DATABASE = {
         "Server": "uat-server",
         "User": "uat-user",
         "Password": "uat-password"
     }
```

### Comparing `linktest-2.8.4/linktest/framework_log.py` & `linktest-2.8.6/linktest/framework_log.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.4/linktest/generate_html_log.py` & `linktest-2.8.6/linktest/generate_html_log.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.4/linktest/get_adb_devices.py` & `linktest-2.8.6/linktest/get_adb_devices.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.4/linktest/get_ios_devices_list.py` & `linktest-2.8.6/linktest/get_ios_devices_list.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.4/linktest/get_platform_info.py` & `linktest-2.8.6/linktest/get_platform_info.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.4/linktest/get_project_info.py` & `linktest-2.8.6/linktest/get_project_info.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.4/linktest/html_report.py` & `linktest-2.8.6/linktest/html_report.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.4/linktest/logged_requests.py` & `linktest-2.8.6/linktest/logged_requests.py`

 * *Files 8% similar despite different names*

```diff
@@ -87,15 +87,15 @@
             return res
 
         return wrapper
 
     @log_curl
     def get(self, url, params=None, **kwargs):
         if not getattr(settings, "AUTO_LOG_HTTP_REQUEST", True):
-            return requests.post(url, data, json, **kwargs)
+            return requests.get(url, params, **kwargs)
 
         self.logger.info(">>>>>>>>>>>>>>>>>>>>>>>>> GET Request Started >>>>>>>>>>>>>>>>>>>>>>>>>")
         self.logger.info("URL: " + url)
 
         if params is not None:
             self.logger.info("params: " + pformat(params))
 
@@ -107,15 +107,19 @@
         self.logger.info("<<<<<<<< GET Response:")
         self.logger.info(response)
 
         if response.status_code == 200:
             if 'application/json' in response.headers.get('Content-Type'):
                 try:
                     data = response.json()
-                    self.logger.info(os.linesep + json_func.dumps(response.json(), ensure_ascii=False, indent=2))
+
+                    if getattr(settings, "USE_JSON_INDENTATION", True):
+                        self.logger.info(os.linesep + json_func.dumps(data, ensure_ascii=False, indent=2))
+                    else:
+                        self.logger.info(os.linesep + json_func.dumps(data, ensure_ascii=False))
                 except json.JSONDecodeError:
                     self.logger.error("Response is not valid JSON.")
             else:
                 self.logger.info(os.linesep + response.text)
 
         self.logger.info("<<<<<<<<<<<<<<<<<<<<<<<<< GET Request Completed <<<<<<<<<<<<<<<<<<<<<<<<<" + os.linesep)
 
@@ -137,15 +141,14 @@
             # if kwargs['headers']['Content-Type'] == 'application/x-www-form-urlencoded':
             #     self.logger.info(os.linesep + pformat(data))
             # else:
             #     self.logger.info(os.linesep + pformat(json_func.loads(data)))
 
             try:
                 # 此处省去各种判断逻辑, 如果 json.loads()报错，则直接 记录原始data
-                # self.logger.info(os.linesep + pformat(json_func.loads(data)))
                 self.logger.info(json_func.dumps(json_func.loads(data), ensure_ascii=False, indent=2))
             except BaseException:
                 self.logger.info(pformat(data))
 
         if json is not None:
             self.logger.info("JSON: " + os.linesep + json_func.dumps(json, ensure_ascii=False, indent=2))
 
@@ -156,27 +159,31 @@
 
         self.logger.info("<<<<<<<< POST Response: ")
         self.logger.info(response)
 
         if response.status_code == 200:
             try:
                 # dumps()方法中的 indent参数 如果 不为空 则会自动format输出结果
-                self.logger.info(os.linesep + json_func.dumps(response.json(), ensure_ascii=False, indent=2))
+                if getattr(settings, "USE_JSON_INDENTATION", True):
+                    self.logger.info(os.linesep + json_func.dumps(response.json(), ensure_ascii=False, indent=2))
+                else:
+                    self.logger.info(os.linesep + json_func.dumps(response.json(), ensure_ascii=False))
+
             except BaseException:
                 self.logger.info(response.__dict__)
                 return response
 
         self.logger.info("<<<<<<<<<<<<<<<<<<<<<<<<< POST Request Completed <<<<<<<<<<<<<<<<<<<<<<<<<" + os.linesep)
 
         return response
 
     @log_curl
     def put(self, url, data=None, **kwargs):
         if not getattr(settings, "AUTO_LOG_HTTP_REQUEST", True):
-            return requests.post(url, data, json, **kwargs)
+            return requests.put(url, data, **kwargs)
 
         self.logger.info(">>>>>>>>>>>>>>>>>>>>>>>>> PUT Request Start >>>>>>>>>>>>>>>>>>>>>>>>>" + os.linesep)
         self.logger.info("URL: " + url)
 
         if data is not None:
             try:
                 self.logger.info("data: " + os.linesep + pformat(json_func.loads(data)))
@@ -189,40 +196,46 @@
         response = requests.put(url, data, **kwargs)
 
         self.logger.info("<<<<<<<< PUT Response:")
         self.logger.info(response)
 
         if response.status_code == 200:
             try:
-                self.logger.info(os.linesep + json_func.dumps(response.json(), ensure_ascii=False, indent=2))
+                if getattr(settings, "USE_JSON_INDENTATION", True):
+                    self.logger.info(os.linesep + json_func.dumps(response.json(), ensure_ascii=False, indent=2))
+                else:
+                    self.logger.info(os.linesep + json_func.dumps(response.json(), ensure_ascii=False))
             except BaseException:
                 return response
 
         self.logger.info("<<<<<<<<<<<<<<<<<<<<<<<<< PUT Request Completed <<<<<<<<<<<<<<<<<<<<<<<<<" + os.linesep)
 
         return response
 
     @log_curl
     def delete(self, url, **kwargs):
         if not getattr(settings, "AUTO_LOG_HTTP_REQUEST", True):
-            return requests.post(url, data, json, **kwargs)
+            return requests.delete(url, **kwargs)
 
         self.logger.info(">>>>>>>>>>>>>>>>>>>>>>>>> DELETE Request Start >>>>>>>>>>>>>>>>>>>>>>>>>" + os.linesep)
         self.logger.info("URL: " + url)
 
         if len(kwargs.keys()) > 0:
             self.logger.info("kwargs: " + os.linesep + json_func.dumps(kwargs, ensure_ascii=False, indent=2))
 
         response = requests.delete(url, **kwargs)
 
         self.logger.info("<<<<<<<< DELETE Response:")
         self.logger.info(response)
 
         if response.status_code == 200:
             try:
-                self.logger.info(os.linesep + json_func.dumps(response.json(), ensure_ascii=False, indent=2))
+                if getattr(settings, "USE_JSON_INDENTATION", True):
+                    self.logger.info(os.linesep + json_func.dumps(response.json(), ensure_ascii=False, indent=2))
+                else:
+                    self.logger.info(os.linesep + json_func.dumps(response.json(), ensure_ascii=False))
             except BaseException:
                 return response
 
         self.logger.info("<<<<<<<<<<<<<<<<<<<<<<<<< DELETE Request Completed <<<<<<<<<<<<<<<<<<<<<<<<<" + os.linesep)
 
         return response
```

### Comparing `linktest-2.8.4/linktest/main.py` & `linktest-2.8.6/linktest/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     - RERUN_FLAG (controls rerunning of failed test cases; default is False)
     - DEBUG_RUN (keeps the browser active after execution is done; default value is False)
     - Show_All_Chrome_Driver_Logs (determines whether to show all webdriver logs; default value is False)
     - QUEUE_SIZE (setting queue_size to 8, for example, means that a maximum of 8 test cases can be executed concurrently)
     - SAVE_LOG_TO_DB (saves execution logs into testdb; must be used in conjunction with linktest-dashboard, default value is False)
     - generate_xunit_result (saves xunit report; default value is False; used for TestLink integration)
     - AUTO_LOG_HTTP_REQUEST (default value is True; automatically logs request actions)
+    - USE_JSON_INDENTATION (default value is True; uses JSON indentation in log)
     - AUTO_DOWNLOAD_CHROMEDRIVER (default value is False; automatically downloads the appropriate Chromedriver based on the Chrome version)
     - AUTO_SCREENSHOT_ON_ACTION (default value is False; automatically generates a screenshot for each WebDriver action)
     - DEFAULT_BROWSER_NAME (default browser name for UI test cases; default value is "chrome")
     - HEAD_LESS (default value is False; runs the browser in headless mode)
     - WEBDRIVER_IMPLICIT_WAIT (default value is 10 seconds; maximum time the WebDriver should wait for an element to be present before throwing an exception)
     - LOG_TO_CONSOLE (default value is True; always logs to the console)
     - ALWAYS_GENERATE_CURL (default value is False; always generates cURL commands)
@@ -1207,15 +1208,14 @@
                             executing_testcase.execution_log = execution_log
 
                     finally:
                         try:
                             generate_html_log.generate_html_log(executing_testcase)
                         except BaseException:
                             traceback.print_exc()
-                            executing_testcase.logger.error(traceback.format_exc())
 
                         if os.sep + "jenkins" + os.sep + "workspace" + os.sep in project_info.project_path:
                             TestCaseExecutor.jenkins_job_name = \
                                 project_info.project_path.split(os.sep + "jenkins" + os.sep + "workspace" + os.sep)[
                                     1].split(os.sep)[0]
 
                 try:
```

### Comparing `linktest-2.8.4/linktest/memory_usage.py` & `linktest-2.8.6/linktest/memory_usage.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.4/linktest/re_func.py` & `linktest-2.8.6/linktest/re_func.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.4/linktest/run.py` & `linktest-2.8.6/linktest/run.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.4/linktest/run_testcase_thread.py` & `linktest-2.8.6/linktest/run_testcase_thread.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.4/linktest/scp_report_to_specified_path.py` & `linktest-2.8.6/linktest/scp_report_to_specified_path.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.4/linktest/selenium_helper.py` & `linktest-2.8.6/linktest/selenium_helper.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.4/linktest/timeout_thread.py` & `linktest-2.8.6/linktest/timeout_thread.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.4/linktest/ui_testcase.py` & `linktest-2.8.6/linktest/ui_testcase.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.4/linktest/update_config.py` & `linktest-2.8.6/linktest/update_config.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.4/linktest/webdriver_wrapper.py` & `linktest-2.8.6/linktest/webdriver_wrapper.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.4/linktest/webdriver_wrapper_chrome.py` & `linktest-2.8.6/linktest/webdriver_wrapper_chrome.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.4/linktest/webdriver_wrapper_edge.py` & `linktest-2.8.6/linktest/webdriver_wrapper_edge.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.4/linktest/webdriver_wrapper_firefox.py` & `linktest-2.8.6/linktest/webdriver_wrapper_firefox.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.4/linktest/webdriver_wrapper_ie.py` & `linktest-2.8.6/linktest/webdriver_wrapper_ie.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.4/linktest/webdriver_wrapper_safari.py` & `linktest-2.8.6/linktest/webdriver_wrapper_safari.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.4/linktest/xml_report.py` & `linktest-2.8.6/linktest/xml_report.py`

 * *Files identical despite different names*

### Comparing `linktest-2.8.4/linktest.egg-info/SOURCES.txt` & `linktest-2.8.6/linktest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

