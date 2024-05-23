# Comparing `tmp/fnschool-20240523.80109.809.tar.gz` & `tmp/fnschool-20240523.80119.832.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fnschool-20240523.80109.809.tar", last modified: Wed May 22 17:09:14 2024, max compression
+gzip compressed data, was "fnschool-20240523.80119.832.tar", last modified: Wed May 22 17:19:37 2024, max compression
```

## Comparing `fnschool-20240523.80109.809.tar` & `fnschool-20240523.80119.832.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-22 17:09:14.272530 fnschool-20240523.80109.809/
--rw-rw-r--   0 larry     (1000) larry     (1000)     7651 2024-03-07 04:52:18.000000 fnschool-20240523.80109.809/LICENSE
--rw-r--r--   0 larry     (1000) larry     (1000)    12298 2024-05-22 17:09:14.272530 fnschool-20240523.80109.809/PKG-INFO
--rw-rw-r--   0 larry     (1000) larry     (1000)     2331 2024-04-12 15:01:09.000000 fnschool-20240523.80109.809/README.md
--rw-rw-r--   0 larry     (1000) larry     (1000)     1427 2024-03-28 13:47:09.000000 fnschool-20240523.80109.809/pyproject.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)       38 2024-05-22 17:09:14.272530 fnschool-20240523.80109.809/setup.cfg
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-22 17:09:14.248530 fnschool-20240523.80109.809/src/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-22 17:09:14.255530 fnschool-20240523.80109.809/src/fnschool/
--rw-rw-r--   0 larry     (1000) larry     (1000)      449 2024-05-22 17:09:09.000000 fnschool-20240523.80109.809/src/fnschool/__init__.py
--rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-19 23:33:33.000000 fnschool-20240523.80109.809/src/fnschool/__main__.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     4902 2024-05-22 16:23:26.000000 fnschool-20240523.80109.809/src/fnschool/app.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-22 17:09:14.263530 fnschool-20240523.80109.809/src/fnschool/canteen/
--rw-rw-r--   0 larry     (1000) larry     (1000)       35 2024-05-19 23:33:33.000000 fnschool-20240523.80109.809/src/fnschool/canteen/__init__.py
--rw-rw-r--   0 larry     (1000) larry     (1000)       44 2024-05-19 23:33:33.000000 fnschool-20240523.80109.809/src/fnschool/canteen/__main__.py
--rw-rw-r--   0 larry     (1000) larry     (1000)    13817 2024-05-19 23:33:33.000000 fnschool-20240523.80109.809/src/fnschool/canteen/bill.cp.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     6638 2024-05-19 23:33:33.000000 fnschool-20240523.80109.809/src/fnschool/canteen/bill.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      866 2024-05-07 20:27:50.000000 fnschool-20240523.80109.809/src/fnschool/canteen/canteen.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)     2035 2024-05-19 23:33:33.000000 fnschool-20240523.80109.809/src/fnschool/canteen/config.py
--rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-19 23:33:33.000000 fnschool-20240523.80109.809/src/fnschool/canteen/consume.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     1468 2024-05-21 13:49:15.000000 fnschool-20240523.80109.809/src/fnschool/canteen/consuming.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      295 2024-05-21 13:58:04.000000 fnschool-20240523.80109.809/src/fnschool/canteen/currency.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-22 17:09:14.264530 fnschool-20240523.80109.809/src/fnschool/canteen/data/
--rw-rw-r--   0 larry     (1000) larry     (1000)   255585 2024-05-22 03:00:22.000000 fnschool-20240523.80109.809/src/fnschool/canteen/data/bill.xlsx
--rw-rw-r--   0 larry     (1000) larry     (1000)    46566 2024-03-25 11:21:24.000000 fnschool-20240523.80109.809/src/fnschool/canteen/data/consuming.xlsx
--rw-rw-r--   0 larry     (1000) larry     (1000)    16095 2024-04-14 21:51:37.000000 fnschool-20240523.80109.809/src/fnschool/canteen/data/purchase_list.xlsx
--rw-rw-r--   0 larry     (1000) larry     (1000)    14566 2024-05-19 23:33:33.000000 fnschool-20240523.80109.809/src/fnschool/canteen/food.cp.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     1894 2024-05-22 16:23:26.000000 fnschool-20240523.80109.809/src/fnschool/canteen/food.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      883 2024-05-15 05:52:50.000000 fnschool-20240523.80109.809/src/fnschool/canteen/food_classes.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-07 17:51:29.000000 fnschool-20240523.80109.809/src/fnschool/canteen/food_recount.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-07 17:51:29.000000 fnschool-20240523.80109.809/src/fnschool/canteen/food_recounts.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)     5262 2024-05-22 02:49:11.000000 fnschool-20240523.80109.809/src/fnschool/canteen/operator.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      778 2024-05-21 13:49:15.000000 fnschool-20240523.80109.809/src/fnschool/canteen/path.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     2863 2024-05-21 13:49:15.000000 fnschool-20240523.80109.809/src/fnschool/canteen/profile.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-22 17:09:14.268530 fnschool-20240523.80109.809/src/fnschool/canteen/spreadsheet/
--rw-rw-r--   0 larry     (1000) larry     (1000)        1 2024-05-19 23:33:33.000000 fnschool-20240523.80109.809/src/fnschool/canteen/spreadsheet/__init__.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     4097 2024-05-21 13:49:15.000000 fnschool-20240523.80109.809/src/fnschool/canteen/spreadsheet/base.py
--rw-rw-r--   0 larry     (1000) larry     (1000)    10382 2024-05-19 23:33:33.000000 fnschool-20240523.80109.809/src/fnschool/canteen/spreadsheet/consuming.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     2067 2024-05-21 13:49:15.000000 fnschool-20240523.80109.809/src/fnschool/canteen/spreadsheet/consumingsum.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     1886 2024-05-19 23:33:33.000000 fnschool-20240523.80109.809/src/fnschool/canteen/spreadsheet/cover.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     9332 2024-05-21 13:49:16.000000 fnschool-20240523.80109.809/src/fnschool/canteen/spreadsheet/ctspreadsheet.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     9381 2024-05-19 23:33:33.000000 fnschool-20240523.80109.809/src/fnschool/canteen/spreadsheet/food.py
--rw-rw-r--   0 larry     (1000) larry     (1000)    10420 2024-05-22 06:21:13.000000 fnschool-20240523.80109.809/src/fnschool/canteen/spreadsheet/inventory.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     9265 2024-05-22 02:49:28.000000 fnschool-20240523.80109.809/src/fnschool/canteen/spreadsheet/preconsuming.py
--rw-rw-r--   0 larry     (1000) larry     (1000)    18265 2024-05-22 16:59:27.000000 fnschool-20240523.80109.809/src/fnschool/canteen/spreadsheet/purchasing.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     2704 2024-05-19 23:33:33.000000 fnschool-20240523.80109.809/src/fnschool/canteen/spreadsheet/purchasingsum.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     4450 2024-05-21 13:49:16.000000 fnschool-20240523.80109.809/src/fnschool/canteen/spreadsheet/unwarehousing.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      210 2024-05-19 23:33:33.000000 fnschool-20240523.80109.809/src/fnschool/canteen/spreadsheet/unwarehousingsum.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     9692 2024-05-19 23:33:33.000000 fnschool-20240523.80109.809/src/fnschool/canteen/spreadsheet/warehousing.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     3126 2024-05-19 23:33:33.000000 fnschool-20240523.80109.809/src/fnschool/canteen/test.py
--rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-19 23:33:33.000000 fnschool-20240523.80109.809/src/fnschool/canteen/warehouse.py
--rw-rw-r--   0 larry     (1000) larry     (1000)    98944 2024-05-21 13:49:22.000000 fnschool-20240523.80109.809/src/fnschool/canteen/workbook.py
--rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-07 17:51:29.000000 fnschool-20240523.80109.809/src/fnschool/canteen/workbook.toml
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-22 17:09:14.269530 fnschool-20240523.80109.809/src/fnschool/data/
--rw-rw-r--   0 larry     (1000) larry     (1000)      144 2024-03-13 04:48:21.000000 fnschool-20240523.80109.809/src/fnschool/data/config0.toml
--rw-rw-r--   0 larry     (1000) larry     (1000)     1034 2024-05-19 23:33:33.000000 fnschool-20240523.80109.809/src/fnschool/entry.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     1375 2024-05-21 13:49:16.000000 fnschool-20240523.80109.809/src/fnschool/external.py
--rw-rw-r--   0 larry     (1000) larry     (1000)     1715 2024-05-21 13:49:16.000000 fnschool-20240523.80109.809/src/fnschool/fnprint.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      824 2024-05-19 23:33:33.000000 fnschool-20240523.80109.809/src/fnschool/language.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-22 17:09:14.251530 fnschool-20240523.80109.809/src/fnschool/locales/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-22 17:09:14.250530 fnschool-20240523.80109.809/src/fnschool/locales/en_US/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-22 17:09:14.269530 fnschool-20240523.80109.809/src/fnschool/locales/en_US/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)      451 2024-05-22 17:09:09.000000 fnschool-20240523.80109.809/src/fnschool/locales/en_US/LC_MESSAGES/fnschool.mo
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-22 17:09:14.250530 fnschool-20240523.80109.809/src/fnschool/locales/zh_CN/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-22 17:09:14.269530 fnschool-20240523.80109.809/src/fnschool/locales/zh_CN/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)    20655 2024-05-22 17:09:09.000000 fnschool-20240523.80109.809/src/fnschool/locales/zh_CN/LC_MESSAGES/fnschool.mo
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-22 17:09:14.250530 fnschool-20240523.80109.809/src/fnschool/locales/zh_HK/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-22 17:09:14.270530 fnschool-20240523.80109.809/src/fnschool/locales/zh_HK/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-05-22 17:09:09.000000 fnschool-20240523.80109.809/src/fnschool/locales/zh_HK/LC_MESSAGES/fnschool.mo
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-22 17:09:14.251530 fnschool-20240523.80109.809/src/fnschool/locales/zh_SG/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-22 17:09:14.270530 fnschool-20240523.80109.809/src/fnschool/locales/zh_SG/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-05-22 17:09:09.000000 fnschool-20240523.80109.809/src/fnschool/locales/zh_SG/LC_MESSAGES/fnschool.mo
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-22 17:09:14.251530 fnschool-20240523.80109.809/src/fnschool/locales/zh_TW/
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-22 17:09:14.271530 fnschool-20240523.80109.809/src/fnschool/locales/zh_TW/LC_MESSAGES/
--rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-05-22 17:09:09.000000 fnschool-20240523.80109.809/src/fnschool/locales/zh_TW/LC_MESSAGES/fnschool.mo
--rw-rw-r--   0 larry     (1000) larry     (1000)     1215 2024-05-21 13:49:16.000000 fnschool-20240523.80109.809/src/fnschool/path.py
--rw-rw-r--   0 larry     (1000) larry     (1000)      517 2024-05-19 23:33:33.000000 fnschool-20240523.80109.809/src/fnschool/test.py
-drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-22 17:09:14.271530 fnschool-20240523.80109.809/src/fnschool.egg-info/
--rw-r--r--   0 larry     (1000) larry     (1000)    12298 2024-05-22 17:09:14.000000 fnschool-20240523.80109.809/src/fnschool.egg-info/PKG-INFO
--rw-rw-r--   0 larry     (1000) larry     (1000)     2218 2024-05-22 17:09:14.000000 fnschool-20240523.80109.809/src/fnschool.egg-info/SOURCES.txt
--rw-rw-r--   0 larry     (1000) larry     (1000)        1 2024-05-22 17:09:14.000000 fnschool-20240523.80109.809/src/fnschool.egg-info/dependency_links.txt
--rw-rw-r--   0 larry     (1000) larry     (1000)       99 2024-05-22 17:09:14.000000 fnschool-20240523.80109.809/src/fnschool.egg-info/entry_points.txt
--rw-rw-r--   0 larry     (1000) larry     (1000)       53 2024-05-22 17:09:14.000000 fnschool-20240523.80109.809/src/fnschool.egg-info/requires.txt
--rw-rw-r--   0 larry     (1000) larry     (1000)        9 2024-05-22 17:09:14.000000 fnschool-20240523.80109.809/src/fnschool.egg-info/top_level.txt
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-22 17:19:37.421984 fnschool-20240523.80119.832/
+-rw-rw-r--   0 larry     (1000) larry     (1000)     7651 2024-03-07 04:52:18.000000 fnschool-20240523.80119.832/LICENSE
+-rw-r--r--   0 larry     (1000) larry     (1000)    12298 2024-05-22 17:19:37.421984 fnschool-20240523.80119.832/PKG-INFO
+-rw-rw-r--   0 larry     (1000) larry     (1000)     2331 2024-04-12 15:01:09.000000 fnschool-20240523.80119.832/README.md
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1427 2024-03-28 13:47:09.000000 fnschool-20240523.80119.832/pyproject.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)       38 2024-05-22 17:19:37.421984 fnschool-20240523.80119.832/setup.cfg
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-22 17:19:37.394984 fnschool-20240523.80119.832/src/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-22 17:19:37.402984 fnschool-20240523.80119.832/src/fnschool/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      449 2024-05-22 17:19:32.000000 fnschool-20240523.80119.832/src/fnschool/__init__.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-19 23:33:33.000000 fnschool-20240523.80119.832/src/fnschool/__main__.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     4902 2024-05-22 16:23:26.000000 fnschool-20240523.80119.832/src/fnschool/app.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-22 17:19:37.412984 fnschool-20240523.80119.832/src/fnschool/canteen/
+-rw-rw-r--   0 larry     (1000) larry     (1000)       35 2024-05-19 23:33:33.000000 fnschool-20240523.80119.832/src/fnschool/canteen/__init__.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)       44 2024-05-19 23:33:33.000000 fnschool-20240523.80119.832/src/fnschool/canteen/__main__.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)    13817 2024-05-19 23:33:33.000000 fnschool-20240523.80119.832/src/fnschool/canteen/bill.cp.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     6638 2024-05-19 23:33:33.000000 fnschool-20240523.80119.832/src/fnschool/canteen/bill.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      866 2024-05-07 20:27:50.000000 fnschool-20240523.80119.832/src/fnschool/canteen/canteen.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)     2035 2024-05-19 23:33:33.000000 fnschool-20240523.80119.832/src/fnschool/canteen/config.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-19 23:33:33.000000 fnschool-20240523.80119.832/src/fnschool/canteen/consume.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1468 2024-05-21 13:49:15.000000 fnschool-20240523.80119.832/src/fnschool/canteen/consuming.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      295 2024-05-21 13:58:04.000000 fnschool-20240523.80119.832/src/fnschool/canteen/currency.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-22 17:19:37.413984 fnschool-20240523.80119.832/src/fnschool/canteen/data/
+-rw-rw-r--   0 larry     (1000) larry     (1000)   255585 2024-05-22 03:00:22.000000 fnschool-20240523.80119.832/src/fnschool/canteen/data/bill.xlsx
+-rw-rw-r--   0 larry     (1000) larry     (1000)    46566 2024-03-25 11:21:24.000000 fnschool-20240523.80119.832/src/fnschool/canteen/data/consuming.xlsx
+-rw-rw-r--   0 larry     (1000) larry     (1000)    16095 2024-04-14 21:51:37.000000 fnschool-20240523.80119.832/src/fnschool/canteen/data/purchase_list.xlsx
+-rw-rw-r--   0 larry     (1000) larry     (1000)    14566 2024-05-19 23:33:33.000000 fnschool-20240523.80119.832/src/fnschool/canteen/food.cp.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1894 2024-05-22 16:23:26.000000 fnschool-20240523.80119.832/src/fnschool/canteen/food.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      883 2024-05-15 05:52:50.000000 fnschool-20240523.80119.832/src/fnschool/canteen/food_classes.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-07 17:51:29.000000 fnschool-20240523.80119.832/src/fnschool/canteen/food_recount.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-07 17:51:29.000000 fnschool-20240523.80119.832/src/fnschool/canteen/food_recounts.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)     5262 2024-05-22 02:49:11.000000 fnschool-20240523.80119.832/src/fnschool/canteen/operator.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      778 2024-05-21 13:49:15.000000 fnschool-20240523.80119.832/src/fnschool/canteen/path.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     2863 2024-05-21 13:49:15.000000 fnschool-20240523.80119.832/src/fnschool/canteen/profile.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-22 17:19:37.417984 fnschool-20240523.80119.832/src/fnschool/canteen/spreadsheet/
+-rw-rw-r--   0 larry     (1000) larry     (1000)        1 2024-05-19 23:33:33.000000 fnschool-20240523.80119.832/src/fnschool/canteen/spreadsheet/__init__.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     4097 2024-05-21 13:49:15.000000 fnschool-20240523.80119.832/src/fnschool/canteen/spreadsheet/base.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)    10382 2024-05-19 23:33:33.000000 fnschool-20240523.80119.832/src/fnschool/canteen/spreadsheet/consuming.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     2067 2024-05-21 13:49:15.000000 fnschool-20240523.80119.832/src/fnschool/canteen/spreadsheet/consumingsum.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1886 2024-05-19 23:33:33.000000 fnschool-20240523.80119.832/src/fnschool/canteen/spreadsheet/cover.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     9332 2024-05-21 13:49:16.000000 fnschool-20240523.80119.832/src/fnschool/canteen/spreadsheet/ctspreadsheet.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     9381 2024-05-19 23:33:33.000000 fnschool-20240523.80119.832/src/fnschool/canteen/spreadsheet/food.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)    10420 2024-05-22 06:21:13.000000 fnschool-20240523.80119.832/src/fnschool/canteen/spreadsheet/inventory.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     9265 2024-05-22 02:49:28.000000 fnschool-20240523.80119.832/src/fnschool/canteen/spreadsheet/preconsuming.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)    18266 2024-05-22 17:17:36.000000 fnschool-20240523.80119.832/src/fnschool/canteen/spreadsheet/purchasing.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     2704 2024-05-19 23:33:33.000000 fnschool-20240523.80119.832/src/fnschool/canteen/spreadsheet/purchasingsum.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     4450 2024-05-21 13:49:16.000000 fnschool-20240523.80119.832/src/fnschool/canteen/spreadsheet/unwarehousing.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      210 2024-05-19 23:33:33.000000 fnschool-20240523.80119.832/src/fnschool/canteen/spreadsheet/unwarehousingsum.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     9692 2024-05-19 23:33:33.000000 fnschool-20240523.80119.832/src/fnschool/canteen/spreadsheet/warehousing.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     3126 2024-05-19 23:33:33.000000 fnschool-20240523.80119.832/src/fnschool/canteen/test.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-19 23:33:33.000000 fnschool-20240523.80119.832/src/fnschool/canteen/warehouse.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)    98944 2024-05-21 13:49:22.000000 fnschool-20240523.80119.832/src/fnschool/canteen/workbook.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)        0 2024-05-07 17:51:29.000000 fnschool-20240523.80119.832/src/fnschool/canteen/workbook.toml
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-22 17:19:37.418984 fnschool-20240523.80119.832/src/fnschool/data/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      144 2024-03-13 04:48:21.000000 fnschool-20240523.80119.832/src/fnschool/data/config0.toml
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1034 2024-05-19 23:33:33.000000 fnschool-20240523.80119.832/src/fnschool/entry.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1375 2024-05-21 13:49:16.000000 fnschool-20240523.80119.832/src/fnschool/external.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1715 2024-05-21 13:49:16.000000 fnschool-20240523.80119.832/src/fnschool/fnprint.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      824 2024-05-19 23:33:33.000000 fnschool-20240523.80119.832/src/fnschool/language.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-22 17:19:37.396984 fnschool-20240523.80119.832/src/fnschool/locales/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-22 17:19:37.395984 fnschool-20240523.80119.832/src/fnschool/locales/en_US/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-22 17:19:37.418984 fnschool-20240523.80119.832/src/fnschool/locales/en_US/LC_MESSAGES/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      451 2024-05-22 17:19:32.000000 fnschool-20240523.80119.832/src/fnschool/locales/en_US/LC_MESSAGES/fnschool.mo
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-22 17:19:37.395984 fnschool-20240523.80119.832/src/fnschool/locales/zh_CN/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-22 17:19:37.419984 fnschool-20240523.80119.832/src/fnschool/locales/zh_CN/LC_MESSAGES/
+-rw-rw-r--   0 larry     (1000) larry     (1000)    20656 2024-05-22 17:19:32.000000 fnschool-20240523.80119.832/src/fnschool/locales/zh_CN/LC_MESSAGES/fnschool.mo
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-22 17:19:37.396984 fnschool-20240523.80119.832/src/fnschool/locales/zh_HK/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-22 17:19:37.419984 fnschool-20240523.80119.832/src/fnschool/locales/zh_HK/LC_MESSAGES/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-05-22 17:19:32.000000 fnschool-20240523.80119.832/src/fnschool/locales/zh_HK/LC_MESSAGES/fnschool.mo
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-22 17:19:37.396984 fnschool-20240523.80119.832/src/fnschool/locales/zh_SG/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-22 17:19:37.419984 fnschool-20240523.80119.832/src/fnschool/locales/zh_SG/LC_MESSAGES/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-05-22 17:19:32.000000 fnschool-20240523.80119.832/src/fnschool/locales/zh_SG/LC_MESSAGES/fnschool.mo
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-22 17:19:37.397984 fnschool-20240523.80119.832/src/fnschool/locales/zh_TW/
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-22 17:19:37.420984 fnschool-20240523.80119.832/src/fnschool/locales/zh_TW/LC_MESSAGES/
+-rw-rw-r--   0 larry     (1000) larry     (1000)      454 2024-05-22 17:19:32.000000 fnschool-20240523.80119.832/src/fnschool/locales/zh_TW/LC_MESSAGES/fnschool.mo
+-rw-rw-r--   0 larry     (1000) larry     (1000)     1215 2024-05-21 13:49:16.000000 fnschool-20240523.80119.832/src/fnschool/path.py
+-rw-rw-r--   0 larry     (1000) larry     (1000)      517 2024-05-19 23:33:33.000000 fnschool-20240523.80119.832/src/fnschool/test.py
+drwxrwxr-x   0 larry     (1000) larry     (1000)        0 2024-05-22 17:19:37.420984 fnschool-20240523.80119.832/src/fnschool.egg-info/
+-rw-r--r--   0 larry     (1000) larry     (1000)    12298 2024-05-22 17:19:37.000000 fnschool-20240523.80119.832/src/fnschool.egg-info/PKG-INFO
+-rw-rw-r--   0 larry     (1000) larry     (1000)     2218 2024-05-22 17:19:37.000000 fnschool-20240523.80119.832/src/fnschool.egg-info/SOURCES.txt
+-rw-rw-r--   0 larry     (1000) larry     (1000)        1 2024-05-22 17:19:37.000000 fnschool-20240523.80119.832/src/fnschool.egg-info/dependency_links.txt
+-rw-rw-r--   0 larry     (1000) larry     (1000)       99 2024-05-22 17:19:37.000000 fnschool-20240523.80119.832/src/fnschool.egg-info/entry_points.txt
+-rw-rw-r--   0 larry     (1000) larry     (1000)       53 2024-05-22 17:19:37.000000 fnschool-20240523.80119.832/src/fnschool.egg-info/requires.txt
+-rw-rw-r--   0 larry     (1000) larry     (1000)        9 2024-05-22 17:19:37.000000 fnschool-20240523.80119.832/src/fnschool.egg-info/top_level.txt
```

### Comparing `fnschool-20240523.80109.809/LICENSE` & `fnschool-20240523.80119.832/LICENSE`

 * *Files identical despite different names*

### Comparing `fnschool-20240523.80109.809/PKG-INFO` & `fnschool-20240523.80119.832/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fnschool
-Version: 20240523.80109.809
+Version: 20240523.80119.832
 Summary: Just some school related scripts, without any ambition.
 Author-email: larryw3i <larryw3i@163.com>, Larry Wei <larryw3i@126.com>, Larry W3i <larryw3i@yeah.net>
 Maintainer-email: larryw3i <larryw3i@163.com>, Larry Wei <larryw3i@126.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
```

### Comparing `fnschool-20240523.80109.809/README.md` & `fnschool-20240523.80119.832/README.md`

 * *Files identical despite different names*

### Comparing `fnschool-20240523.80109.809/pyproject.toml` & `fnschool-20240523.80119.832/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fnschool-20240523.80109.809/src/fnschool/app.py` & `fnschool-20240523.80119.832/src/fnschool/app.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240523.80109.809/src/fnschool/canteen/bill.cp.py` & `fnschool-20240523.80119.832/src/fnschool/canteen/bill.cp.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240523.80109.809/src/fnschool/canteen/bill.py` & `fnschool-20240523.80119.832/src/fnschool/canteen/bill.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240523.80109.809/src/fnschool/canteen/canteen.toml` & `fnschool-20240523.80119.832/src/fnschool/canteen/canteen.toml`

 * *Files identical despite different names*

### Comparing `fnschool-20240523.80109.809/src/fnschool/canteen/config.py` & `fnschool-20240523.80119.832/src/fnschool/canteen/config.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240523.80109.809/src/fnschool/canteen/consuming.py` & `fnschool-20240523.80119.832/src/fnschool/canteen/consuming.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240523.80109.809/src/fnschool/canteen/data/bill.xlsx` & `fnschool-20240523.80119.832/src/fnschool/canteen/data/bill.xlsx`

 * *Files identical despite different names*

### Comparing `fnschool-20240523.80109.809/src/fnschool/canteen/data/consuming.xlsx` & `fnschool-20240523.80119.832/src/fnschool/canteen/data/consuming.xlsx`

 * *Files identical despite different names*

### Comparing `fnschool-20240523.80109.809/src/fnschool/canteen/data/purchase_list.xlsx` & `fnschool-20240523.80119.832/src/fnschool/canteen/data/purchase_list.xlsx`

 * *Files identical despite different names*

### Comparing `fnschool-20240523.80109.809/src/fnschool/canteen/food.cp.py` & `fnschool-20240523.80119.832/src/fnschool/canteen/food.cp.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240523.80109.809/src/fnschool/canteen/food.py` & `fnschool-20240523.80119.832/src/fnschool/canteen/food.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240523.80109.809/src/fnschool/canteen/food_classes.toml` & `fnschool-20240523.80119.832/src/fnschool/canteen/food_classes.toml`

 * *Files identical despite different names*

### Comparing `fnschool-20240523.80109.809/src/fnschool/canteen/operator.py` & `fnschool-20240523.80119.832/src/fnschool/canteen/operator.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240523.80109.809/src/fnschool/canteen/path.py` & `fnschool-20240523.80119.832/src/fnschool/canteen/path.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240523.80109.809/src/fnschool/canteen/profile.py` & `fnschool-20240523.80119.832/src/fnschool/canteen/profile.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240523.80109.809/src/fnschool/canteen/spreadsheet/base.py` & `fnschool-20240523.80119.832/src/fnschool/canteen/spreadsheet/base.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240523.80109.809/src/fnschool/canteen/spreadsheet/consuming.py` & `fnschool-20240523.80119.832/src/fnschool/canteen/spreadsheet/consuming.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240523.80109.809/src/fnschool/canteen/spreadsheet/consumingsum.py` & `fnschool-20240523.80119.832/src/fnschool/canteen/spreadsheet/consumingsum.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240523.80109.809/src/fnschool/canteen/spreadsheet/cover.py` & `fnschool-20240523.80119.832/src/fnschool/canteen/spreadsheet/cover.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240523.80109.809/src/fnschool/canteen/spreadsheet/ctspreadsheet.py` & `fnschool-20240523.80119.832/src/fnschool/canteen/spreadsheet/ctspreadsheet.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240523.80109.809/src/fnschool/canteen/spreadsheet/food.py` & `fnschool-20240523.80119.832/src/fnschool/canteen/spreadsheet/food.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240523.80109.809/src/fnschool/canteen/spreadsheet/inventory.py` & `fnschool-20240523.80119.832/src/fnschool/canteen/spreadsheet/inventory.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240523.80109.809/src/fnschool/canteen/spreadsheet/preconsuming.py` & `fnschool-20240523.80119.832/src/fnschool/canteen/spreadsheet/preconsuming.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240523.80109.809/src/fnschool/canteen/spreadsheet/purchasing.py` & `fnschool-20240523.80119.832/src/fnschool/canteen/spreadsheet/purchasing.py`

 * *Files 0% similar despite different names*

```diff
@@ -414,15 +414,15 @@
                 ) 
                 print_info(saved_ifoods_s)
                 print_warning(saved_ifoods_info)
                 print_warning(
                     (
                         _('Fill them in "{0}"? (YyNn)')
                         if len(saved_ifoods) > 1
-                        else _('Fill it in "{0}" (YyNn)')
+                        else _('Fill it in "{0}"? (YyNn)')
                     ).format(self.path)
                 )
 
                 f_input = input(">_ ").replace(" ", "")
                 if len(f_input) > 0 and f_input in "Yy":
                     max_row = len(
                         [
```

### Comparing `fnschool-20240523.80109.809/src/fnschool/canteen/spreadsheet/purchasingsum.py` & `fnschool-20240523.80119.832/src/fnschool/canteen/spreadsheet/purchasingsum.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240523.80109.809/src/fnschool/canteen/spreadsheet/unwarehousing.py` & `fnschool-20240523.80119.832/src/fnschool/canteen/spreadsheet/unwarehousing.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240523.80109.809/src/fnschool/canteen/spreadsheet/warehousing.py` & `fnschool-20240523.80119.832/src/fnschool/canteen/spreadsheet/warehousing.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240523.80109.809/src/fnschool/canteen/test.py` & `fnschool-20240523.80119.832/src/fnschool/canteen/test.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240523.80109.809/src/fnschool/canteen/workbook.py` & `fnschool-20240523.80119.832/src/fnschool/canteen/workbook.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240523.80109.809/src/fnschool/entry.py` & `fnschool-20240523.80119.832/src/fnschool/entry.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240523.80109.809/src/fnschool/external.py` & `fnschool-20240523.80119.832/src/fnschool/external.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240523.80109.809/src/fnschool/fnprint.py` & `fnschool-20240523.80119.832/src/fnschool/fnprint.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240523.80109.809/src/fnschool/language.py` & `fnschool-20240523.80119.832/src/fnschool/language.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240523.80109.809/src/fnschool/locales/zh_CN/LC_MESSAGES/fnschool.mo` & `fnschool-20240523.80119.832/src/fnschool/locales/zh_CN/LC_MESSAGES/fnschool.mo`

 * *Files 3% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,13 +1,13 @@
 msgid ""
 msgstr ""
 "Project-Id-Version:  fnschool\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2024-05-23 00:49+0800\n"
-"PO-Revision-Date: 2024-05-23 00:49+0800\n"
+"POT-Creation-Date: 2024-05-23 01:17+0800\n"
+"PO-Revision-Date: 2024-05-23 01:17+0800\n"
 "Last-Translator: larryw3i <larryw3i@163.com>\n"
 "Language: zh_CN\n"
 "Language-Team: Chinese - China <larryw3i@163.com>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -120,15 +120,15 @@
 msgid "Failed to read remaining foods from Sheet {0} of Spreadsheet {1}."
 msgstr ""
 "从 工作簿 “{1}” 中读取 工作表 “{0}” 失败。（可能为表头的盘存信息格式错误）"
 
 msgid "File or directory '%s' doesn't exist."
 msgstr "文件 或 目录 “%s” 不存在。"
 
-msgid "Fill it in \"{0}\" (YyNn)"
+msgid "Fill it in \"{0}\"? (YyNn)"
 msgstr "把它填入 “{0}” 吗？（是的：“Y”，“y”）"
 
 msgid "Fill them in \"{0}\"? (YyNn)"
 msgstr "把它们填入 “{0}” 吗？（是的：“Y”，“y”）"
 
 msgid "Food 'negligible' mark index"
 msgstr "食材 “可忽略” 标记索引"
```

### Comparing `fnschool-20240523.80109.809/src/fnschool/path.py` & `fnschool-20240523.80119.832/src/fnschool/path.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240523.80109.809/src/fnschool/test.py` & `fnschool-20240523.80119.832/src/fnschool/test.py`

 * *Files identical despite different names*

### Comparing `fnschool-20240523.80109.809/src/fnschool.egg-info/PKG-INFO` & `fnschool-20240523.80119.832/src/fnschool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fnschool
-Version: 20240523.80109.809
+Version: 20240523.80119.832
 Summary: Just some school related scripts, without any ambition.
 Author-email: larryw3i <larryw3i@163.com>, Larry Wei <larryw3i@126.com>, Larry W3i <larryw3i@yeah.net>
 Maintainer-email: larryw3i <larryw3i@163.com>, Larry Wei <larryw3i@126.com>
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
```

### Comparing `fnschool-20240523.80109.809/src/fnschool.egg-info/SOURCES.txt` & `fnschool-20240523.80119.832/src/fnschool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

