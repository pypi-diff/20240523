# Comparing `tmp/immanuel-1.3.3.tar.gz` & `tmp/immanuel-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "immanuel-1.3.3.tar", last modified: Fri Apr 26 02:31:29 2024, max compression
+gzip compressed data, was "immanuel-1.4.0.tar", last modified: Thu May 23 00:56:26 2024, max compression
```

## Comparing `immanuel-1.3.3.tar` & `immanuel-1.4.0.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxr-xr-x   0 robert     (501) staff       (20)        0 2024-04-26 02:31:29.194582 immanuel-1.3.3/
--rw-r--r--   0 robert     (501) staff       (20)    32096 2023-12-02 01:56:03.000000 immanuel-1.3.3/LICENSE.md
--rw-r--r--   0 robert     (501) staff       (20)       26 2024-04-16 01:50:25.000000 immanuel-1.3.3/MANIFEST.in
--rw-r--r--   0 robert     (501) staff       (20)    47556 2024-04-26 02:31:29.194167 immanuel-1.3.3/PKG-INFO
--rw-r--r--   0 robert     (501) staff       (20)     9563 2024-04-26 02:27:25.000000 immanuel-1.3.3/README.md
-drwxr-xr-x   0 robert     (501) staff       (20)        0 2024-04-26 02:31:29.101087 immanuel-1.3.3/immanuel/
--rw-r--r--   0 robert     (501) staff       (20)       66 2024-04-16 01:27:34.000000 immanuel-1.3.3/immanuel/__init__.py
--rw-r--r--   0 robert     (501) staff       (20)    18861 2024-04-21 20:24:34.000000 immanuel-1.3.3/immanuel/charts.py
-drwxr-xr-x   0 robert     (501) staff       (20)        0 2024-04-26 02:31:29.124369 immanuel-1.3.3/immanuel/classes/
--rw-r--r--   0 robert     (501) staff       (20)      619 2024-04-01 00:34:17.000000 immanuel-1.3.3/immanuel/classes/cache.py
--rw-r--r--   0 robert     (501) staff       (20)     2158 2024-04-16 01:25:04.000000 immanuel-1.3.3/immanuel/classes/localize.py
--rw-r--r--   0 robert     (501) staff       (20)      558 2024-01-16 22:54:01.000000 immanuel-1.3.3/immanuel/classes/serialize.py
--rw-r--r--   0 robert     (501) staff       (20)    12699 2024-04-26 01:40:11.000000 immanuel-1.3.3/immanuel/classes/wrap.py
-drwxr-xr-x   0 robert     (501) staff       (20)        0 2024-04-26 02:31:29.127755 immanuel-1.3.3/immanuel/const/
--rw-r--r--   0 robert     (501) staff       (20)     2399 2024-04-26 00:50:04.000000 immanuel-1.3.3/immanuel/const/calc.py
--rw-r--r--   0 robert     (501) staff       (20)     2613 2024-04-21 20:24:34.000000 immanuel-1.3.3/immanuel/const/chart.py
--rw-r--r--   0 robert     (501) staff       (20)      770 2024-01-16 22:54:01.000000 immanuel-1.3.3/immanuel/const/data.py
--rw-r--r--   0 robert     (501) staff       (20)    11276 2024-01-16 22:54:01.000000 immanuel-1.3.3/immanuel/const/dignities.py
--rw-r--r--   0 robert     (501) staff       (20)      255 2024-04-08 01:17:15.000000 immanuel-1.3.3/immanuel/const/genders.py
--rw-r--r--   0 robert     (501) staff       (20)     5692 2024-04-21 20:24:34.000000 immanuel-1.3.3/immanuel/const/names.py
-drwxr-xr-x   0 robert     (501) staff       (20)        0 2024-04-26 02:31:29.089329 immanuel-1.3.3/immanuel/locales/
-drwxr-xr-x   0 robert     (501) staff       (20)        0 2024-04-26 02:31:29.128547 immanuel-1.3.3/immanuel/locales/es_ES/
-drwxr-xr-x   0 robert     (501) staff       (20)        0 2024-04-26 02:31:29.129390 immanuel-1.3.3/immanuel/locales/es_ES/LC_MESSAGES/
--rw-r--r--   0 robert     (501) staff       (20)     7895 2024-04-22 13:27:14.000000 immanuel-1.3.3/immanuel/locales/es_ES/LC_MESSAGES/immanuel.mo
--rw-r--r--   0 robert     (501) staff       (20)     2130 2024-04-23 00:05:08.000000 immanuel-1.3.3/immanuel/locales/es_ES/mappings.py
-drwxr-xr-x   0 robert     (501) staff       (20)        0 2024-04-26 02:31:29.130160 immanuel-1.3.3/immanuel/locales/pt_BR/
-drwxr-xr-x   0 robert     (501) staff       (20)        0 2024-04-26 02:31:29.130720 immanuel-1.3.3/immanuel/locales/pt_BR/LC_MESSAGES/
--rw-r--r--   0 robert     (501) staff       (20)     8005 2024-04-15 00:27:49.000000 immanuel-1.3.3/immanuel/locales/pt_BR/LC_MESSAGES/immanuel.mo
--rw-r--r--   0 robert     (501) staff       (20)     2065 2024-04-23 00:05:21.000000 immanuel-1.3.3/immanuel/locales/pt_BR/mappings.py
-drwxr-xr-x   0 robert     (501) staff       (20)        0 2024-04-26 02:31:29.132623 immanuel-1.3.3/immanuel/reports/
--rw-r--r--   0 robert     (501) staff       (20)     4658 2024-04-16 01:27:34.000000 immanuel-1.3.3/immanuel/reports/aspect.py
--rw-r--r--   0 robert     (501) staff       (20)     7581 2024-04-16 01:27:34.000000 immanuel-1.3.3/immanuel/reports/dignity.py
--rw-r--r--   0 robert     (501) staff       (20)     2186 2024-04-16 01:27:34.000000 immanuel-1.3.3/immanuel/reports/pattern.py
--rw-r--r--   0 robert     (501) staff       (20)     1497 2024-01-16 22:54:01.000000 immanuel-1.3.3/immanuel/reports/weighting.py
-drwxr-xr-x   0 robert     (501) staff       (20)        0 2024-04-26 02:31:29.089609 immanuel-1.3.3/immanuel/resources/
-drwxr-xr-x   0 robert     (501) staff       (20)        0 2024-04-26 02:31:29.175200 immanuel-1.3.3/immanuel/resources/ephemeris/
--rw-r--r--   0 robert     (501) staff       (20)   225863 2024-03-29 02:29:31.000000 immanuel-1.3.3/immanuel/resources/ephemeris/seas_12.se1
--rw-r--r--   0 robert     (501) staff       (20)   225440 2024-03-29 02:29:31.000000 immanuel-1.3.3/immanuel/resources/ephemeris/seas_18.se1
--rw-r--r--   0 robert     (501) staff       (20)   225108 2024-03-29 02:29:31.000000 immanuel-1.3.3/immanuel/resources/ephemeris/seas_24.se1
--rw-r--r--   0 robert     (501) staff       (20)  1306782 2024-03-29 02:29:31.000000 immanuel-1.3.3/immanuel/resources/ephemeris/semo_12.se1
--rw-r--r--   0 robert     (501) staff       (20)  1305686 2024-03-29 02:29:31.000000 immanuel-1.3.3/immanuel/resources/ephemeris/semo_18.se1
--rw-r--r--   0 robert     (501) staff       (20)  1309017 2024-03-29 02:29:31.000000 immanuel-1.3.3/immanuel/resources/ephemeris/semo_24.se1
--rw-r--r--   0 robert     (501) staff       (20)  1326257 2024-03-29 02:29:31.000000 immanuel-1.3.3/immanuel/resources/ephemeris/semo_36.se1
--rw-r--r--   0 robert     (501) staff       (20)  1339659 2024-03-29 02:29:31.000000 immanuel-1.3.3/immanuel/resources/ephemeris/semo_42.se1
--rw-r--r--   0 robert     (501) staff       (20)   483763 2024-03-29 02:29:31.000000 immanuel-1.3.3/immanuel/resources/ephemeris/sepl_12.se1
--rw-r--r--   0 robert     (501) staff       (20)   484065 2024-03-29 02:29:31.000000 immanuel-1.3.3/immanuel/resources/ephemeris/sepl_18.se1
--rw-r--r--   0 robert     (501) staff       (20)   483399 2024-03-29 02:29:31.000000 immanuel-1.3.3/immanuel/resources/ephemeris/sepl_24.se1
--rw-r--r--   0 robert     (501) staff       (20)   484686 2024-03-29 02:29:31.000000 immanuel-1.3.3/immanuel/resources/ephemeris/sepl_36.se1
--rw-r--r--   0 robert     (501) staff       (20)   483628 2024-03-29 02:29:31.000000 immanuel-1.3.3/immanuel/resources/ephemeris/sepl_42.se1
--rw-r--r--   0 robert     (501) staff       (20)    12066 2024-04-21 20:24:34.000000 immanuel-1.3.3/immanuel/setup.py
-drwxr-xr-x   0 robert     (501) staff       (20)        0 2024-04-26 02:31:29.179799 immanuel-1.3.3/immanuel/tools/
--rw-r--r--   0 robert     (501) staff       (20)     4211 2024-04-26 01:06:56.000000 immanuel-1.3.3/immanuel/tools/calculate.py
--rw-r--r--   0 robert     (501) staff       (20)     6023 2024-01-16 22:54:01.000000 immanuel-1.3.3/immanuel/tools/convert.py
--rw-r--r--   0 robert     (501) staff       (20)     3181 2024-01-17 23:18:15.000000 immanuel-1.3.3/immanuel/tools/date.py
--rw-r--r--   0 robert     (501) staff       (20)    21046 2024-04-21 20:24:34.000000 immanuel-1.3.3/immanuel/tools/ephemeris.py
--rw-r--r--   0 robert     (501) staff       (20)     5702 2024-04-09 19:59:42.000000 immanuel-1.3.3/immanuel/tools/find.py
--rw-r--r--   0 robert     (501) staff       (20)     2027 2024-01-16 22:54:01.000000 immanuel-1.3.3/immanuel/tools/forecast.py
--rw-r--r--   0 robert     (501) staff       (20)     1824 2024-01-16 22:54:01.000000 immanuel-1.3.3/immanuel/tools/midpoint.py
--rw-r--r--   0 robert     (501) staff       (20)     2709 2024-04-22 00:25:50.000000 immanuel-1.3.3/immanuel/tools/position.py
-drwxr-xr-x   0 robert     (501) staff       (20)        0 2024-04-26 02:31:29.193389 immanuel-1.3.3/immanuel.egg-info/
--rw-r--r--   0 robert     (501) staff       (20)    47556 2024-04-26 02:31:28.000000 immanuel-1.3.3/immanuel.egg-info/PKG-INFO
--rw-r--r--   0 robert     (501) staff       (20)     1894 2024-04-26 02:31:29.000000 immanuel-1.3.3/immanuel.egg-info/SOURCES.txt
--rw-r--r--   0 robert     (501) staff       (20)        1 2024-04-26 02:31:28.000000 immanuel-1.3.3/immanuel.egg-info/dependency_links.txt
--rw-r--r--   0 robert     (501) staff       (20)       60 2024-04-26 02:31:28.000000 immanuel-1.3.3/immanuel.egg-info/requires.txt
--rw-r--r--   0 robert     (501) staff       (20)        9 2024-04-26 02:31:28.000000 immanuel-1.3.3/immanuel.egg-info/top_level.txt
--rw-r--r--   0 robert     (501) staff       (20)     1070 2024-04-26 02:27:12.000000 immanuel-1.3.3/pyproject.toml
--rw-r--r--   0 robert     (501) staff       (20)       38 2024-04-26 02:31:29.194646 immanuel-1.3.3/setup.cfg
-drwxr-xr-x   0 robert     (501) staff       (20)        0 2024-04-26 02:31:29.192888 immanuel-1.3.3/tests/
--rw-r--r--   0 robert     (501) staff       (20)    40905 2023-12-02 01:56:03.000000 immanuel-1.3.3/tests/se01181s.se1
--rw-r--r--   0 robert     (501) staff       (20)     3920 2024-04-21 20:24:34.000000 immanuel-1.3.3/tests/test_aspect.py
--rw-r--r--   0 robert     (501) staff       (20)     3530 2024-04-21 20:24:34.000000 immanuel-1.3.3/tests/test_calculate.py
--rw-r--r--   0 robert     (501) staff       (20)    23308 2024-04-21 20:24:34.000000 immanuel-1.3.3/tests/test_charts.py
--rw-r--r--   0 robert     (501) staff       (20)    28783 2024-01-17 23:16:08.000000 immanuel-1.3.3/tests/test_convert.py
--rw-r--r--   0 robert     (501) staff       (20)     4579 2024-01-17 23:18:15.000000 immanuel-1.3.3/tests/test_date.py
--rw-r--r--   0 robert     (501) staff       (20)     9521 2024-04-16 01:27:34.000000 immanuel-1.3.3/tests/test_dignity.py
--rw-r--r--   0 robert     (501) staff       (20)    15068 2024-04-21 20:24:34.000000 immanuel-1.3.3/tests/test_ephemeris.py
--rw-r--r--   0 robert     (501) staff       (20)     3714 2024-01-20 20:35:37.000000 immanuel-1.3.3/tests/test_find.py
--rw-r--r--   0 robert     (501) staff       (20)     6735 2024-01-20 20:36:29.000000 immanuel-1.3.3/tests/test_forecast.py
--rw-r--r--   0 robert     (501) staff       (20)    18927 2024-04-21 20:24:34.000000 immanuel-1.3.3/tests/test_localization.py
--rw-r--r--   0 robert     (501) staff       (20)     5374 2024-04-21 20:24:34.000000 immanuel-1.3.3/tests/test_midpoint.py
--rw-r--r--   0 robert     (501) staff       (20)     2393 2024-01-16 22:54:01.000000 immanuel-1.3.3/tests/test_pattern.py
--rw-r--r--   0 robert     (501) staff       (20)     5157 2024-04-21 20:24:34.000000 immanuel-1.3.3/tests/test_position.py
--rw-r--r--   0 robert     (501) staff       (20)     3169 2024-04-16 01:27:34.000000 immanuel-1.3.3/tests/test_setup.py
--rw-r--r--   0 robert     (501) staff       (20)     2286 2024-04-01 00:40:36.000000 immanuel-1.3.3/tests/test_weighting.py
+drwxr-xr-x   0 robert     (501) staff       (20)        0 2024-05-23 00:56:26.315792 immanuel-1.4.0/
+-rw-r--r--   0 robert     (501) staff       (20)    32096 2023-12-02 01:56:03.000000 immanuel-1.4.0/LICENSE.md
+-rw-r--r--   0 robert     (501) staff       (20)       26 2024-04-16 01:50:25.000000 immanuel-1.4.0/MANIFEST.in
+-rw-r--r--   0 robert     (501) staff       (20)    47784 2024-05-23 00:56:26.315414 immanuel-1.4.0/PKG-INFO
+-rw-r--r--   0 robert     (501) staff       (20)     9791 2024-05-22 22:08:54.000000 immanuel-1.4.0/README.md
+drwxr-xr-x   0 robert     (501) staff       (20)        0 2024-05-23 00:56:26.211808 immanuel-1.4.0/immanuel/
+-rw-r--r--   0 robert     (501) staff       (20)       66 2024-04-16 01:27:34.000000 immanuel-1.4.0/immanuel/__init__.py
+-rw-r--r--   0 robert     (501) staff       (20)    20725 2024-05-20 20:31:04.000000 immanuel-1.4.0/immanuel/charts.py
+drwxr-xr-x   0 robert     (501) staff       (20)        0 2024-05-23 00:56:26.217759 immanuel-1.4.0/immanuel/classes/
+-rw-r--r--   0 robert     (501) staff       (20)      619 2024-04-01 00:34:17.000000 immanuel-1.4.0/immanuel/classes/cache.py
+-rw-r--r--   0 robert     (501) staff       (20)     2158 2024-04-16 01:25:04.000000 immanuel-1.4.0/immanuel/classes/localize.py
+-rw-r--r--   0 robert     (501) staff       (20)      558 2024-01-16 22:54:01.000000 immanuel-1.4.0/immanuel/classes/serialize.py
+-rw-r--r--   0 robert     (501) staff       (20)    12930 2024-05-22 00:44:44.000000 immanuel-1.4.0/immanuel/classes/wrap.py
+drwxr-xr-x   0 robert     (501) staff       (20)        0 2024-05-23 00:56:26.230644 immanuel-1.4.0/immanuel/const/
+-rw-r--r--   0 robert     (501) staff       (20)     2397 2024-05-13 22:15:25.000000 immanuel-1.4.0/immanuel/const/calc.py
+-rw-r--r--   0 robert     (501) staff       (20)     2703 2024-05-06 16:28:14.000000 immanuel-1.4.0/immanuel/const/chart.py
+-rw-r--r--   0 robert     (501) staff       (20)      770 2024-01-16 22:54:01.000000 immanuel-1.4.0/immanuel/const/data.py
+-rw-r--r--   0 robert     (501) staff       (20)    11276 2024-01-16 22:54:01.000000 immanuel-1.4.0/immanuel/const/dignities.py
+-rw-r--r--   0 robert     (501) staff       (20)      255 2024-04-08 01:17:15.000000 immanuel-1.4.0/immanuel/const/genders.py
+-rw-r--r--   0 robert     (501) staff       (20)     5833 2024-05-06 16:28:22.000000 immanuel-1.4.0/immanuel/const/names.py
+drwxr-xr-x   0 robert     (501) staff       (20)        0 2024-05-23 00:56:26.207803 immanuel-1.4.0/immanuel/locales/
+drwxr-xr-x   0 robert     (501) staff       (20)        0 2024-05-23 00:56:26.231744 immanuel-1.4.0/immanuel/locales/es_ES/
+drwxr-xr-x   0 robert     (501) staff       (20)        0 2024-05-23 00:56:26.232391 immanuel-1.4.0/immanuel/locales/es_ES/LC_MESSAGES/
+-rw-r--r--   0 robert     (501) staff       (20)     8060 2024-05-07 22:42:51.000000 immanuel-1.4.0/immanuel/locales/es_ES/LC_MESSAGES/immanuel.mo
+-rw-r--r--   0 robert     (501) staff       (20)     2271 2024-05-06 22:10:21.000000 immanuel-1.4.0/immanuel/locales/es_ES/mappings.py
+drwxr-xr-x   0 robert     (501) staff       (20)        0 2024-05-23 00:56:26.234349 immanuel-1.4.0/immanuel/locales/pt_BR/
+drwxr-xr-x   0 robert     (501) staff       (20)        0 2024-05-23 00:56:26.235165 immanuel-1.4.0/immanuel/locales/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 robert     (501) staff       (20)     8061 2024-05-07 22:42:49.000000 immanuel-1.4.0/immanuel/locales/pt_BR/LC_MESSAGES/immanuel.mo
+-rw-r--r--   0 robert     (501) staff       (20)     2203 2024-05-06 22:10:29.000000 immanuel-1.4.0/immanuel/locales/pt_BR/mappings.py
+drwxr-xr-x   0 robert     (501) staff       (20)        0 2024-05-23 00:56:26.238625 immanuel-1.4.0/immanuel/reports/
+-rw-r--r--   0 robert     (501) staff       (20)     4658 2024-04-16 01:27:34.000000 immanuel-1.4.0/immanuel/reports/aspect.py
+-rw-r--r--   0 robert     (501) staff       (20)     7581 2024-04-16 01:27:34.000000 immanuel-1.4.0/immanuel/reports/dignity.py
+-rw-r--r--   0 robert     (501) staff       (20)     2186 2024-04-16 01:27:34.000000 immanuel-1.4.0/immanuel/reports/pattern.py
+-rw-r--r--   0 robert     (501) staff       (20)     1497 2024-01-16 22:54:01.000000 immanuel-1.4.0/immanuel/reports/weighting.py
+drwxr-xr-x   0 robert     (501) staff       (20)        0 2024-05-23 00:56:26.208064 immanuel-1.4.0/immanuel/resources/
+drwxr-xr-x   0 robert     (501) staff       (20)        0 2024-05-23 00:56:26.291541 immanuel-1.4.0/immanuel/resources/ephemeris/
+-rw-r--r--   0 robert     (501) staff       (20)   225863 2024-03-29 02:29:31.000000 immanuel-1.4.0/immanuel/resources/ephemeris/seas_12.se1
+-rw-r--r--   0 robert     (501) staff       (20)   225440 2024-03-29 02:29:31.000000 immanuel-1.4.0/immanuel/resources/ephemeris/seas_18.se1
+-rw-r--r--   0 robert     (501) staff       (20)   225108 2024-03-29 02:29:31.000000 immanuel-1.4.0/immanuel/resources/ephemeris/seas_24.se1
+-rw-r--r--   0 robert     (501) staff       (20)  1306782 2024-03-29 02:29:31.000000 immanuel-1.4.0/immanuel/resources/ephemeris/semo_12.se1
+-rw-r--r--   0 robert     (501) staff       (20)  1305686 2024-03-29 02:29:31.000000 immanuel-1.4.0/immanuel/resources/ephemeris/semo_18.se1
+-rw-r--r--   0 robert     (501) staff       (20)  1309017 2024-03-29 02:29:31.000000 immanuel-1.4.0/immanuel/resources/ephemeris/semo_24.se1
+-rw-r--r--   0 robert     (501) staff       (20)  1326257 2024-03-29 02:29:31.000000 immanuel-1.4.0/immanuel/resources/ephemeris/semo_36.se1
+-rw-r--r--   0 robert     (501) staff       (20)  1339659 2024-03-29 02:29:31.000000 immanuel-1.4.0/immanuel/resources/ephemeris/semo_42.se1
+-rw-r--r--   0 robert     (501) staff       (20)   483763 2024-03-29 02:29:31.000000 immanuel-1.4.0/immanuel/resources/ephemeris/sepl_12.se1
+-rw-r--r--   0 robert     (501) staff       (20)   484065 2024-03-29 02:29:31.000000 immanuel-1.4.0/immanuel/resources/ephemeris/sepl_18.se1
+-rw-r--r--   0 robert     (501) staff       (20)   483399 2024-03-29 02:29:31.000000 immanuel-1.4.0/immanuel/resources/ephemeris/sepl_24.se1
+-rw-r--r--   0 robert     (501) staff       (20)   484686 2024-03-29 02:29:31.000000 immanuel-1.4.0/immanuel/resources/ephemeris/sepl_36.se1
+-rw-r--r--   0 robert     (501) staff       (20)   483628 2024-03-29 02:29:31.000000 immanuel-1.4.0/immanuel/resources/ephemeris/sepl_42.se1
+-rw-r--r--   0 robert     (501) staff       (20)    12514 2024-05-13 23:27:03.000000 immanuel-1.4.0/immanuel/setup.py
+drwxr-xr-x   0 robert     (501) staff       (20)        0 2024-05-23 00:56:26.296487 immanuel-1.4.0/immanuel/tools/
+-rw-r--r--   0 robert     (501) staff       (20)     6164 2024-05-22 00:44:44.000000 immanuel-1.4.0/immanuel/tools/calculate.py
+-rw-r--r--   0 robert     (501) staff       (20)     6023 2024-01-16 22:54:01.000000 immanuel-1.4.0/immanuel/tools/convert.py
+-rw-r--r--   0 robert     (501) staff       (20)     3181 2024-01-17 23:18:15.000000 immanuel-1.4.0/immanuel/tools/date.py
+-rw-r--r--   0 robert     (501) staff       (20)    20985 2024-05-08 01:53:36.000000 immanuel-1.4.0/immanuel/tools/ephemeris.py
+-rw-r--r--   0 robert     (501) staff       (20)     5702 2024-04-09 19:59:42.000000 immanuel-1.4.0/immanuel/tools/find.py
+-rw-r--r--   0 robert     (501) staff       (20)     2027 2024-01-16 22:54:01.000000 immanuel-1.4.0/immanuel/tools/forecast.py
+-rw-r--r--   0 robert     (501) staff       (20)     1824 2024-01-16 22:54:01.000000 immanuel-1.4.0/immanuel/tools/midpoint.py
+-rw-r--r--   0 robert     (501) staff       (20)     2709 2024-04-22 00:25:50.000000 immanuel-1.4.0/immanuel/tools/position.py
+drwxr-xr-x   0 robert     (501) staff       (20)        0 2024-05-23 00:56:26.314756 immanuel-1.4.0/immanuel.egg-info/
+-rw-r--r--   0 robert     (501) staff       (20)    47784 2024-05-23 00:56:25.000000 immanuel-1.4.0/immanuel.egg-info/PKG-INFO
+-rw-r--r--   0 robert     (501) staff       (20)     1894 2024-05-23 00:56:26.000000 immanuel-1.4.0/immanuel.egg-info/SOURCES.txt
+-rw-r--r--   0 robert     (501) staff       (20)        1 2024-05-23 00:56:25.000000 immanuel-1.4.0/immanuel.egg-info/dependency_links.txt
+-rw-r--r--   0 robert     (501) staff       (20)       60 2024-05-23 00:56:25.000000 immanuel-1.4.0/immanuel.egg-info/requires.txt
+-rw-r--r--   0 robert     (501) staff       (20)        9 2024-05-23 00:56:25.000000 immanuel-1.4.0/immanuel.egg-info/top_level.txt
+-rw-r--r--   0 robert     (501) staff       (20)     1070 2024-05-22 22:08:08.000000 immanuel-1.4.0/pyproject.toml
+-rw-r--r--   0 robert     (501) staff       (20)       38 2024-05-23 00:56:26.315842 immanuel-1.4.0/setup.cfg
+drwxr-xr-x   0 robert     (501) staff       (20)        0 2024-05-23 00:56:26.312327 immanuel-1.4.0/tests/
+-rw-r--r--   0 robert     (501) staff       (20)    40905 2023-12-02 01:56:03.000000 immanuel-1.4.0/tests/se01181s.se1
+-rw-r--r--   0 robert     (501) staff       (20)     3926 2024-05-06 00:46:22.000000 immanuel-1.4.0/tests/test_aspect.py
+-rw-r--r--   0 robert     (501) staff       (20)     8664 2024-05-22 02:06:16.000000 immanuel-1.4.0/tests/test_calculate.py
+-rw-r--r--   0 robert     (501) staff       (20)    29979 2024-05-22 00:39:24.000000 immanuel-1.4.0/tests/test_charts.py
+-rw-r--r--   0 robert     (501) staff       (20)    28783 2024-01-17 23:16:08.000000 immanuel-1.4.0/tests/test_convert.py
+-rw-r--r--   0 robert     (501) staff       (20)     4579 2024-01-17 23:18:15.000000 immanuel-1.4.0/tests/test_date.py
+-rw-r--r--   0 robert     (501) staff       (20)     9521 2024-04-16 01:27:34.000000 immanuel-1.4.0/tests/test_dignity.py
+-rw-r--r--   0 robert     (501) staff       (20)    15098 2024-05-06 00:46:22.000000 immanuel-1.4.0/tests/test_ephemeris.py
+-rw-r--r--   0 robert     (501) staff       (20)     3714 2024-01-20 20:35:37.000000 immanuel-1.4.0/tests/test_find.py
+-rw-r--r--   0 robert     (501) staff       (20)     6735 2024-01-20 20:36:29.000000 immanuel-1.4.0/tests/test_forecast.py
+-rw-r--r--   0 robert     (501) staff       (20)    18946 2024-05-06 00:46:22.000000 immanuel-1.4.0/tests/test_localization.py
+-rw-r--r--   0 robert     (501) staff       (20)     5377 2024-05-06 00:46:22.000000 immanuel-1.4.0/tests/test_midpoint.py
+-rw-r--r--   0 robert     (501) staff       (20)     2393 2024-01-16 22:54:01.000000 immanuel-1.4.0/tests/test_pattern.py
+-rw-r--r--   0 robert     (501) staff       (20)     5160 2024-05-06 00:46:22.000000 immanuel-1.4.0/tests/test_position.py
+-rw-r--r--   0 robert     (501) staff       (20)     3169 2024-04-16 01:27:34.000000 immanuel-1.4.0/tests/test_setup.py
+-rw-r--r--   0 robert     (501) staff       (20)     2286 2024-04-01 00:40:36.000000 immanuel-1.4.0/tests/test_weighting.py
```

### Comparing `immanuel-1.3.3/LICENSE.md` & `immanuel-1.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `immanuel-1.3.3/PKG-INFO` & `immanuel-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: immanuel
-Version: 1.3.3
+Version: 1.4.0
 Summary: Quickly produce both human-readable and JSON-formatted astrology chart data based on the Swiss Ephemeris and astro.com.
 Author-email: Robert Davies <robert@theriftlab.com>
 License: # GNU AFFERO GENERAL PUBLIC LICENSE
         
         Version 3, 19 November 2007
         
         Copyright (C) 2007 Free Software Foundation, Inc.
@@ -654,19 +654,19 @@
 
 Immanuel's output is currently available in the following locales / languages:
 
 * **en_US:** (default) US English
 * **pt_BR:** Brazilian Portuguese
 * **es_ES:** Spanish
 
-See [here](https://github.com/theriftlab/immanuel-python/tree/v1.3.3/docs/5-settings.md#locale) for details on how to switch. The documentation itself is not currently available in other translations. To contribute in-software translations, see [here](https://github.com/theriftlab/immanuel-python/tree/v1.3.3/docs/7-contributions.md).
+See [here](https://github.com/theriftlab/immanuel-python/tree/v1.4.0/docs/5-settings.md#locale) for details on how to switch. The documentation itself is not currently available in other translations. To contribute in-software translations, see [here](https://github.com/theriftlab/immanuel-python/tree/v1.4.0/docs/7-contributions.md).
 
 ## Documentation
 
-Full documentation is available [here](https://github.com/theriftlab/immanuel-python/tree/v1.3.3/docs/0-contents.md), or follow the Quick Start below to see how to quickly generate a natal chart.
+Full documentation is available [here](https://github.com/theriftlab/immanuel-python/tree/v1.4.0/docs/0-contents.md), or follow the Quick Start below to see how to quickly generate a natal chart.
 
 ## Quick Start
 
 You can get started with full natal chart data in minutes. Simply install Immanuel:
 
 ```bash
 pip install immanuel
@@ -677,17 +677,29 @@
 ```python
 from immanuel import charts
 
 
 native = charts.Subject(
         date_time='2000-01-01 10:00',
         latitude='32n43',
-        longitude='117w09'
+        longitude='117w09',
     )
 
+# or, alternatively...
+
+from datetime import datetime
+
+native = charts.Subject(
+        date_time=datetime(2000, 1, 1, 10, 0, 0),
+        latitude=32.71667,
+        longitude=-117.15,
+    )
+
+# and then...
+
 natal = charts.Natal(native)
 
 for object in natal.objects.values():
     print(object)
 ```
 
 This will output all the chart objects (planets, points, asteroids etc.) in this format:
@@ -815,14 +827,15 @@
         "formatted": "-23\u00b000'45\"",
         "direction": "-",
         "degrees": 23,
         "minutes": 0,
         "seconds": 45
     },
     "out_of_bounds": false,
+    "in_sect": true,
     "dignities": {
         "ruler": false,
         "exalted": false,
         "triplicity_ruler": false,
         "term_ruler": false,
         "face_ruler": false,
         "mutual_reception_ruler": false,
```

### Comparing `immanuel-1.3.3/README.md` & `immanuel-1.4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -17,19 +17,19 @@
 
 Immanuel's output is currently available in the following locales / languages:
 
 * **en_US:** (default) US English
 * **pt_BR:** Brazilian Portuguese
 * **es_ES:** Spanish
 
-See [here](https://github.com/theriftlab/immanuel-python/tree/v1.3.3/docs/5-settings.md#locale) for details on how to switch. The documentation itself is not currently available in other translations. To contribute in-software translations, see [here](https://github.com/theriftlab/immanuel-python/tree/v1.3.3/docs/7-contributions.md).
+See [here](https://github.com/theriftlab/immanuel-python/tree/v1.4.0/docs/5-settings.md#locale) for details on how to switch. The documentation itself is not currently available in other translations. To contribute in-software translations, see [here](https://github.com/theriftlab/immanuel-python/tree/v1.4.0/docs/7-contributions.md).
 
 ## Documentation
 
-Full documentation is available [here](https://github.com/theriftlab/immanuel-python/tree/v1.3.3/docs/0-contents.md), or follow the Quick Start below to see how to quickly generate a natal chart.
+Full documentation is available [here](https://github.com/theriftlab/immanuel-python/tree/v1.4.0/docs/0-contents.md), or follow the Quick Start below to see how to quickly generate a natal chart.
 
 ## Quick Start
 
 You can get started with full natal chart data in minutes. Simply install Immanuel:
 
 ```bash
 pip install immanuel
@@ -40,17 +40,29 @@
 ```python
 from immanuel import charts
 
 
 native = charts.Subject(
         date_time='2000-01-01 10:00',
         latitude='32n43',
-        longitude='117w09'
+        longitude='117w09',
     )
 
+# or, alternatively...
+
+from datetime import datetime
+
+native = charts.Subject(
+        date_time=datetime(2000, 1, 1, 10, 0, 0),
+        latitude=32.71667,
+        longitude=-117.15,
+    )
+
+# and then...
+
 natal = charts.Natal(native)
 
 for object in natal.objects.values():
     print(object)
 ```
 
 This will output all the chart objects (planets, points, asteroids etc.) in this format:
@@ -178,14 +190,15 @@
         "formatted": "-23\u00b000'45\"",
         "direction": "-",
         "degrees": 23,
         "minutes": 0,
         "seconds": 45
     },
     "out_of_bounds": false,
+    "in_sect": true,
     "dignities": {
         "ruler": false,
         "exalted": false,
         "triplicity_ruler": false,
         "term_ruler": false,
         "face_ruler": false,
         "mutual_reception_ruler": false,
```

### Comparing `immanuel-1.3.3/immanuel/charts.py` & `immanuel-1.4.0/immanuel/charts.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 """
 
 from datetime import datetime
 from zoneinfo import ZoneInfo
 
 from immanuel.classes import wrap
 from immanuel.classes.localize import _
-from immanuel.const import chart, names
-from immanuel.reports import aspect, pattern
+from immanuel.const import calc, chart, names
+from immanuel.reports import aspect, dignity, pattern, weighting
 from immanuel.setup import settings
 from immanuel.tools import calculate, convert, date, ephemeris, forecast, midpoint, position
 
 
 class Subject:
     """ Simple class to model a chart subject - essentially just
     a time and place. """
@@ -46,32 +46,40 @@
 class Chart:
     """ Base chart class. This acts as an abstract class for the actual chart
     classes to inherit from. """
     def __init__(self, type: int, aspects_to: 'Chart' = None) -> None:
         self.type = _(names.CHART_TYPES[type])
         self._type = type
         self._aspects_to = aspects_to
+
+        self._native: Subject
+        self._obliquity: float
+        self._diurnal: bool
+        self._moon_phase: int
+        self._triad: dict = {
+            chart.SUN: None,
+            chart.MOON: None,
+            chart.ASC: None,
+        }
+        self._objects: dict
+        self._houses: dict
+
         self.generate()
         self.wrap()
 
     def house_for(self, object: wrap.Object) -> int:
         """ Returns the index of the house where any passed arbitrary object
         would appear in the current chart. Useful for synastries and
         transit charts. """
         return position.house(object.longitude.raw, self._houses)['index']
 
     def generate(self) -> None:
-        """ Generating the raw data is each descendant class's responsibility,
-        but placeholders for properties common to all charts are set here. """
-        self._native: Subject = None
-        self._obliquity: float = None
-        self._diurnal: bool = None
-        self._moon_phase: int = None
-        self._objects: dict = {}
-        self._houses: dict = {}
+        """ Generating the raw data is each descendant class's
+        responsibility. """
+        pass
 
     def wrap(self) -> None:
         """ Loop through the required data and wrap each one with a custom
         function. """
         for index in settings.chart_data[self._type]:
             method = f'set_wrapped_{index}'
             if hasattr(self, method):
@@ -91,69 +99,93 @@
         self.diurnal = self._diurnal
 
     def set_wrapped_moon_phase(self) -> None:
         self.moon_phase = wrap.MoonPhase(self._moon_phase)
 
     def set_wrapped_objects(self) -> None:
         self.objects = {}
+
         for index, object in self._objects.items():
-            if 'jd' in object:
-                object['date_time'] = date.to_datetime(
-                        dt=object['jd'],
-                        lat=self._native.latitude,
-                        lon=self._native.longitude,
-                    )
-            self.objects[index] = wrap.Object(
+            house = position.house(
                     object=object,
-                    objects=self._objects,
                     houses=self._houses,
-                    is_daytime=self._diurnal,
+                )
+            out_of_bounds = calculate.is_out_of_bounds(
+                    object=object,
                     obliquity=self._obliquity,
                 )
+            in_sect = calculate.is_in_sect(
+                    object=object,
+                    is_daytime=self._diurnal,
+                    sun=self._triad[chart.SUN],
+                ) if object['index'] in (chart.SUN, chart.MOON, chart.MERCURY, chart.VENUS, chart.MARS, chart.JUPITER, chart.SATURN) else None
+            dignity_state = dignity.all(
+                    object=object,
+                    objects=self._objects,
+                    is_daytime=self._diurnal,
+                ) if object['type'] == chart.PLANET and self._diurnal and calc.PLANETS.issubset(self._objects) else None
+            date_time = date.to_datetime(
+                    dt=object['jd'],
+                    lat=self._native.latitude,
+                    lon=self._native.longitude,
+                ) if 'jd' in object else None
+
+            self.objects[index] = wrap.Object(
+                    object=object,
+                    date_time=date_time,
+                    house=house,
+                    out_of_bounds=out_of_bounds,
+                    in_sect=in_sect,
+                    dignity_state=dignity_state,
+                )
 
     def set_wrapped_houses(self) -> None:
         self.houses = {index: wrap.Object(object=house) for index, house in self._houses.items()}
 
     def set_wrapped_aspects(self) -> None:
         aspects = aspect.all(self._objects) if self._aspects_to is None else aspect.synastry(self._objects, self._aspects_to._objects)
-        self.aspects = {index: {object_index: wrap.Aspect(aspect=object_aspect, objects=self._objects) for object_index, object_aspect in aspect_list.items()} for index, aspect_list in aspects.items()}
+        self.aspects = {index: {object_index: wrap.Aspect(aspect=object_aspect, active_name=self._objects[object_aspect['active']]['name'], passive_name=self._objects[object_aspect['passive']]['name']) for object_index, object_aspect in aspect_list.items()} for index, aspect_list in aspects.items()}
 
     def set_wrapped_weightings(self) -> None:
-        self.weightings = wrap.Weightings(self._objects, self._houses)
+        self.weightings = wrap.Weightings(
+                elements=weighting.elements(self._objects),
+                modalities=weighting.modalities(self._objects),
+                quadrants=weighting.quadrants(self._objects, self._houses),
+            )
 
 
 class Natal(Chart):
     """ Standard natal chart generates data straight from the passed
     native information. """
     def __init__(self, native: Subject, aspects_to: Chart = None) -> None:
         self._native = native
         super().__init__(chart.NATAL, aspects_to)
 
     def generate(self) -> None:
         self._obliquity = ephemeris.obliquity(self._native.julian_date)
 
-        sun = ephemeris.planet(chart.SUN, self._native.julian_date)
-        moon = ephemeris.planet(chart.MOON, self._native.julian_date)
-        asc = ephemeris.angle(
+        self._triad[chart.SUN] = ephemeris.planet(chart.SUN, self._native.julian_date)
+        self._triad[chart.MOON] = ephemeris.planet(chart.MOON, self._native.julian_date)
+        self._triad[chart.ASC] = ephemeris.angle(
                 index=chart.ASC,
                 jd=self._native.julian_date,
                 lat=self._native.latitude,
                 lon=self._native.longitude,
                 house_system=settings.house_system,
             )
 
-        self._diurnal = calculate.is_daytime(sun, asc)
-        self._moon_phase = calculate.moon_phase(sun, moon)
+        self._diurnal = calculate.is_daytime(self._triad[chart.SUN], self._triad[chart.ASC])
+        self._moon_phase = calculate.moon_phase(self._triad[chart.SUN], self._triad[chart.MOON])
         self._objects = ephemeris.objects(
                 object_list=settings.objects,
                 jd=self._native.julian_date,
                 lat=self._native.latitude,
                 lon=self._native.longitude,
                 house_system=settings.house_system,
-                pars_fortuna_formula=settings.pars_fortuna_formula,
+                part_formula=settings.part_formula,
             )
         self._houses = ephemeris.houses(
                 jd=self._native.julian_date,
                 lat=self._native.latitude,
                 lon=self._native.longitude,
                 house_system=settings.house_system,
             )
@@ -173,33 +205,33 @@
                 index=chart.ARMC,
                 jd=self._solar_return_jd,
                 lat=self._native.latitude,
                 lon=self._native.longitude,
                 house_system=settings.house_system,
             )
 
-        sun = ephemeris.planet(chart.SUN, self._solar_return_jd)
-        moon = ephemeris.planet(chart.MOON, self._solar_return_jd)
-        asc = ephemeris.angle(
+        self._triad[chart.SUN] = ephemeris.planet(chart.SUN, self._solar_return_jd)
+        self._triad[chart.MOON] = ephemeris.planet(chart.MOON, self._solar_return_jd)
+        self._triad[chart.ASC] = ephemeris.angle(
                 index=chart.ASC,
                 jd=self._solar_return_jd,
                 lat=self._native.latitude,
                 lon=self._native.longitude,
                 house_system=settings.house_system,
             )
 
-        self._diurnal = calculate.is_daytime(sun, asc)
-        self._moon_phase = calculate.moon_phase(sun, moon)
+        self._diurnal = calculate.is_daytime(self._triad[chart.SUN], self._triad[chart.ASC])
+        self._moon_phase = calculate.moon_phase(self._triad[chart.SUN], self._triad[chart.MOON])
         self._objects = ephemeris.objects(
                 object_list=settings.objects,
                 jd=self._solar_return_jd,
                 lat=self._native.latitude,
                 lon=self._native.longitude,
                 house_system=settings.house_system,
-                pars_fortuna_formula=settings.pars_fortuna_formula,
+                part_formula=settings.part_formula,
             )
         self._houses = ephemeris.houses(
                 jd=self._solar_return_jd,
                 lat=self._native.latitude,
                 lon=self._native.longitude,
                 house_system=settings.house_system,
             )
@@ -246,35 +278,35 @@
                 lon=self._native.longitude,
                 pjd=progression_jd,
                 house_system=settings.house_system,
                 method=settings.mc_progression_method,
             )
         self._obliquity = ephemeris.obliquity(self._progressed_jd)
 
-        sun = ephemeris.planet(chart.SUN, self._progressed_jd)
-        moon = ephemeris.planet(chart.MOON, self._progressed_jd)
-        asc = ephemeris.armc_angle(
+        self._triad[chart.SUN] = ephemeris.planet(chart.SUN, self._progressed_jd)
+        self._triad[chart.MOON] = ephemeris.planet(chart.MOON, self._progressed_jd)
+        self._triad[chart.ASC] = ephemeris.armc_angle(
             index=chart.ASC,
                 armc=self._progressed_armc_longitude,
                 lat=self._native.latitude,
                 obliquity=self._obliquity,
                 house_system=settings.house_system,
             )
 
-        self._diurnal = calculate.is_daytime(sun, asc)
-        self._moon_phase = calculate.moon_phase(sun, moon)
+        self._diurnal = calculate.is_daytime(self._triad[chart.SUN], self._triad[chart.ASC])
+        self._moon_phase = calculate.moon_phase(self._triad[chart.SUN], self._triad[chart.MOON])
         self._objects = ephemeris.armc_objects(
                 object_list=settings.objects,
                 jd=self._progressed_jd,
                 armc=self._progressed_armc_longitude,
                 lat=self._native.latitude,
                 lon=self._native.longitude,
                 obliquity=self._obliquity,
                 house_system=settings.house_system,
-                pars_fortuna_formula=settings.pars_fortuna_formula,
+                part_formula=settings.part_formula,
             )
         self._houses = ephemeris.armc_houses(
                 armc=self._progressed_armc_longitude,
                 lat=self._native.latitude,
                 obliquity=self._obliquity,
                 house_system=settings.house_system,
             )
@@ -309,23 +341,23 @@
 
         native_objects = ephemeris.objects(
                 object_list=settings.objects,
                 jd=self._native.julian_date,
                 lat=self._native.latitude,
                 lon=self._native.longitude,
                 house_system=settings.house_system,
-                pars_fortuna_formula=settings.pars_fortuna_formula,
+                part_formula=settings.part_formula,
             )
         partner_objects = ephemeris.objects(
                 object_list=settings.objects,
                 jd=self._partner.julian_date,
                 lat=self._partner.latitude,
                 lon=self._partner.longitude,
                 house_system=settings.house_system,
-                pars_fortuna_formula=settings.pars_fortuna_formula,
+                part_formula=settings.part_formula,
             )
         self._objects = midpoint.all(
                 objects1=native_objects,
                 objects2=partner_objects,
                 obliquity=self._obliquity,
             )
 
@@ -369,15 +401,15 @@
             self._houses = midpoint.all(
                     objects1=native_houses,
                     objects2=partner_houses,
                     obliquity=self._obliquity,
                 )
 
         if chart.ASC in self._objects:
-            asc = self._objects[chart.ASC]
+            self._triad[chart.ASC] = self._objects[chart.ASC]
         else:
             native_asc = ephemeris.angle(
                     index=chart.ASC,
                     jd=self._native.julian_date,
                     lat=self._native.latitude,
                     lon=self._native.longitude,
                     house_system=settings.house_system,
@@ -385,32 +417,32 @@
             partner_asc = ephemeris.angle(
                     index=chart.ASC,
                     jd=self._partner.julian_date,
                     lat=self._partner.latitude,
                     lon=self._partner.longitude,
                     house_system=settings.house_system,
                 )
-            asc = midpoint.composite(native_asc, partner_asc, self._obliquity)
+            self._triad[chart.ASC] = midpoint.composite(native_asc, partner_asc, self._obliquity)
 
         if chart.SUN in self._objects:
-            sun = self._objects[chart.SUN]
+            self._triad[chart.SUN] = self._objects[chart.SUN]
         else:
             native_sun = ephemeris.planet(chart.SUN, self._native.julian_date)
             partner_sun = ephemeris.planet(chart.SUN, self._partner.julian_date)
-            sun = midpoint.composite(native_sun, partner_sun, self._obliquity)
+            self._triad[chart.SUN] = midpoint.composite(native_sun, partner_sun, self._obliquity)
 
         if chart.MOON in self._objects:
-            moon = self._objects[chart.MOON]
+            self._triad[chart.MOON] = self._objects[chart.MOON]
         else:
             native_moon = ephemeris.planet(chart.MOON, self._native.julian_date)
             partner_moon = ephemeris.planet(chart.MOON, self._partner.julian_date)
-            moon = midpoint.composite(native_moon, partner_moon, self._obliquity)
+            self._triad[chart.MOON] = midpoint.composite(native_moon, partner_moon, self._obliquity)
 
-        self._diurnal = calculate.is_daytime(sun, asc)
-        self._moon_phase = calculate.moon_phase(sun, moon)
+        self._diurnal = calculate.is_daytime(self._triad[chart.SUN], self._triad[chart.ASC])
+        self._moon_phase = calculate.moon_phase(self._triad[chart.SUN], self._triad[chart.MOON])
 
     def set_wrapped_partner(self):
         self.partner = wrap.Subject(self._partner)
 
 
 class Transits(Chart):
     """ Chart of the moment for the given coordinates. Structurally identical
@@ -421,33 +453,33 @@
         date_time = datetime.now(tz=ZoneInfo(timezone))
         self._native = Subject(date_time, lat, lon)
         super().__init__(chart.TRANSITS, aspects_to)
 
     def generate(self) -> None:
         self._obliquity = ephemeris.obliquity(self._native.julian_date)
 
-        sun = ephemeris.planet(chart.SUN, self._native.julian_date)
-        moon = ephemeris.planet(chart.MOON, self._native.julian_date)
-        asc = ephemeris.angle(
+        self._triad[chart.SUN] = ephemeris.planet(chart.SUN, self._native.julian_date)
+        self._triad[chart.MOON] = ephemeris.planet(chart.MOON, self._native.julian_date)
+        self._triad[chart.ASC] = ephemeris.angle(
                 index=chart.ASC,
                 jd=self._native.julian_date,
                 lat=self._native.latitude,
                 lon=self._native.longitude,
                 house_system=settings.house_system,
             )
 
-        self._diurnal = calculate.is_daytime(sun, asc)
-        self._moon_phase = calculate.moon_phase(sun, moon)
+        self._diurnal = calculate.is_daytime(self._triad[chart.SUN], self._triad[chart.ASC])
+        self._moon_phase = calculate.moon_phase(self._triad[chart.SUN], self._triad[chart.MOON])
         self._objects = ephemeris.objects(
                 object_list=settings.objects,
                 jd=self._native.julian_date,
                 lat=self._native.latitude,
                 lon=self._native.longitude,
                 house_system=settings.house_system,
-                pars_fortuna_formula=settings.pars_fortuna_formula,
+                part_formula=settings.part_formula,
             )
         self._houses = ephemeris.houses(
                 jd=self._native.julian_date,
                 lat=self._native.latitude,
                 lon=self._native.longitude,
                 house_system=settings.house_system,
             )
```

### Comparing `immanuel-1.3.3/immanuel/classes/cache.py` & `immanuel-1.4.0/immanuel/classes/cache.py`

 * *Files identical despite different names*

### Comparing `immanuel-1.3.3/immanuel/classes/localize.py` & `immanuel-1.4.0/immanuel/classes/localize.py`

 * *Files identical despite different names*

### Comparing `immanuel-1.3.3/immanuel/classes/serialize.py` & `immanuel-1.4.0/immanuel/classes/serialize.py`

 * *Files identical despite different names*

### Comparing `immanuel-1.3.3/immanuel/classes/wrap.py` & `immanuel-1.4.0/immanuel/classes/wrap.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,45 +8,51 @@
     JSON keys are defined here, either explicitly or as class members.
 
 """
 
 from datetime import datetime
 
 from immanuel.const import calc, chart, dignities, names
-from immanuel.reports import dignity, weighting
+from immanuel.reports import dignity
 from immanuel.setup import settings
 from immanuel.tools import calculate, convert, date, ephemeris, position
 from immanuel.classes.localize import gender, _
 
 
 class Angle:
-    def __init__(self, angle: float, format: int = convert.FORMAT_DMS) -> None:
+    precision = {
+        calc.DEGREE: convert.ROUND_DEGREE,
+        calc.MINUTE: convert.ROUND_MINUTE,
+        calc.SECOND: convert.ROUND_SECOND,
+    }
+
+    def __init__(self, angle: float, format: int = convert.FORMAT_DMS, round_to: int = calc.SECOND) -> None:
         self.raw = angle
-        self.formatted = convert.dec_to_string(angle, format)
+        self.formatted = convert.dec_to_string(angle, format, Angle.precision[round_to])
         self.direction = None
         self.degrees = None
         self.minutes = None
         self.seconds = None
         self.__dict__.update(dict(zip(('direction', 'degrees', 'minutes', 'seconds'), convert.dec_to_dms(self.raw))))
 
     def __str__(self) -> str:
         return self.formatted
 
 
 class Aspect:
-    def __init__(self, aspect: dict, objects: dict) -> None:
-        self._active_name = objects[aspect['active']]['name']
-        self._passive_name = objects[aspect['passive']]['name']
+    def __init__(self, aspect: dict, active_name: str, passive_name: str) -> None:
+        self._active_name = active_name
+        self._passive_name = passive_name
         self.active = aspect['active']
         self.passive = aspect['passive']
         self.type = _(names.ASPECTS[aspect['aspect']])
         self.aspect = aspect['aspect']
         self.orb = aspect['orb']
-        self.distance = Angle(aspect['distance'])
-        self.difference = Angle(aspect['difference'])
+        self.distance = Angle(aspect['distance'], round_to=settings.angle_precision)
+        self.difference = Angle(aspect['difference'], round_to=settings.angle_precision)
         self.movement = AspectMovement(aspect)
         self.condition = AspectCondition(aspect)
 
     def __str__(self) -> str:
         return _('{active} {passive} {type} within {difference} ({movement}, {condition})').format(
                 active=self._active_name,
                 passive=self._passive_name,
@@ -173,59 +179,69 @@
         self.formatted = _(names.MOON_PHASES[moon_phase])
 
     def __str__(self) -> str:
         return self.formatted
 
 
 class Object:
-    def __init__(self, object: dict, objects: dict = None, houses: dict = None, is_daytime: bool = None, obliquity: float = None) -> None:
+    def __init__(
+        self,
+        object: dict,
+        date_time: datetime = None,
+        house: int = None,
+        out_of_bounds: bool = None,
+        in_sect: bool = None,
+        dignity_state: dict = None,
+    ) -> None:
         self.index = object['index']
 
         if object['type'] == chart.HOUSE:
             self.number = object['number']
 
         self.name = object['name']
         self.type = ObjectType(object['type'])
 
         if 'eclipse_type' in object:
             self.eclipse_type = EclipseType(object['eclipse_type'])
 
-        if 'date_time' in object:
-            self.date_time = DateTime(object['date_time'])
+        if date_time is not None:
+            self.date_time = DateTime(date_time)
 
         if 'lat' in object:
-            self.latitude = Angle(object['lat'])
+            self.latitude = Angle(object['lat'], round_to=settings.angle_precision)
 
-        self.longitude = Angle(object['lon'])
-        self.sign_longitude = Angle(position.sign_longitude(object))
+        self.longitude = Angle(object['lon'], round_to=settings.angle_precision)
+        self.sign_longitude = Angle(position.sign_longitude(object), round_to=settings.angle_precision)
         self.sign = Sign(position.sign(object))
         self.decan = Decan(position.decan(object))
 
-        if houses is not None:
-            self.house = House(position.house(object, houses))
+        if house is not None:
+            self.house = House(house)
 
         if 'dist' in object:
             self.distance = object['dist']
 
         self.speed = object['speed']
 
         if object['type'] not in (chart.HOUSE, chart.ANGLE, chart.FIXED_STAR):
             self.movement = ObjectMovement(object)
 
         if 'dec' in object:
-            self.declination = Angle(object['dec'])
+            self.declination = Angle(object['dec'], round_to=settings.angle_precision)
 
-            if object['type'] not in (chart.HOUSE, chart.ANGLE, chart.FIXED_STAR):
-                self.out_of_bounds = calculate.is_out_of_bounds(object=object, obliquity=obliquity)
+        if object['type'] not in (chart.HOUSE, chart.ANGLE, chart.FIXED_STAR):
+            self.out_of_bounds = out_of_bounds
 
         if 'size' in object:
             self.size = object['size']
 
-        if objects is not None and object['type'] == chart.PLANET and is_daytime is not None and calc.PLANETS.issubset(objects):
-            dignity_state = dignity.all(object=object, objects=objects, is_daytime=is_daytime)
+        if in_sect is not None:
+            self.in_sect = in_sect
+
+        if dignity_state is not None:
             self.dignities = DignityState(object=object, dignity_state=dignity_state)
             self.score = dignity.score(dignity_state)
 
     def __str__(self) -> str:
         formatted = _('{name} {longitude} in {sign}').format(
                 name=self.name,
                 longitude=self.sign_longitude,
@@ -243,15 +259,15 @@
 
 class ObjectMovement:
     def __init__(self, object: dict) -> None:
         self._movement = calculate.object_movement(object)
         self.direct = self._movement == calc.DIRECT
         self.stationary = self._movement == calc.STATIONARY
         self.retrograde = self._movement == calc.RETROGRADE
-        self.typical = calculate.object_movement_typical(object)
+        self.typical = calculate.is_object_movement_typical(object)
         self.formatted = _(names.OBJECT_MOVEMENTS[self._movement], gender(object['index']))
 
     def __str__(self) -> str:
         return self.formatted
 
 
 class ObjectType:
@@ -300,18 +316,18 @@
                 date_time=self.date_time,
                 lat=self.coordinates.latitude,
                 lon=self.coordinates.longitude,
             )
 
 
 class Weightings:
-    def __init__(self, objects: dict, houses: dict) -> None:
-        self.elements = Elements(weighting.elements(objects))
-        self.modalities = Modalities(weighting.modalities(objects))
-        self.quadrants = Quadrants(weighting.quadrants(objects, houses))
+    def __init__(self, elements: dict, modalities: dict, quadrants: dict) -> None:
+        self.elements = Elements(elements)
+        self.modalities = Modalities(modalities)
+        self.quadrants = Quadrants(quadrants)
 
     def __str__(self) -> str:
         return f'{self.elements}\n{self.modalities}\n{self.quadrants}'
 
 
 class Elements:
     def __init__(self, elements: dict) -> None:
```

### Comparing `immanuel-1.3.3/immanuel/const/calc.py` & `immanuel-1.4.0/immanuel/const/calc.py`

 * *Files 6% similar despite different names*

```diff
@@ -80,23 +80,19 @@
 ORIENTAL = 1
 
 """ MC progression formulae. """
 NAIBOD = 0
 SOLAR_ARC = 1
 DAILY_HOUSES = 2
 
-""" Part of Fortune formulae. """
+""" Part of Fortune / Spirit / Eros formulae. """
 DAY_FORMULA = 0
 NIGHT_FORMULA = 1
 DAY_NIGHT_FORMULA = 2
 
-""" Composite Part of Fortune calculations. """
-MIDPOINT = 0
-COMPOSITE = 1
-
 """ Orb calculation when two chart objects have different orbs. """
 MEAN = 0
 MAX = 1
 
 """ Aspect information. """
 APPLICATIVE = 0
 EXACT = 1
@@ -109,7 +105,12 @@
 BUNDLE = 0
 BUCKET = 1
 BOWL = 2
 LOCOMOTIVE = 3
 SEESAW = 4
 SPLAY = 5
 SPLASH = 6
+
+""" Angle rounding. """
+DEGREE = 0
+MINUTE = 1
+SECOND = 2
```

### Comparing `immanuel-1.3.3/immanuel/const/chart.py` & `immanuel-1.4.0/immanuel/const/chart.py`

 * *Files 10% similar despite different names*

```diff
@@ -116,16 +116,19 @@
 NORTH_NODE = POINT + 1
 SOUTH_NODE = POINT + 2
 TRUE_NORTH_NODE = POINT + 3
 TRUE_SOUTH_NODE = POINT + 4
 VERTEX = POINT + 5
 LILITH = POINT + 6
 TRUE_LILITH = POINT + 7
-SYZYGY = POINT + 8
-PARS_FORTUNA = POINT + 9
+INTERPOLATED_LILITH = POINT + 8
+SYZYGY = POINT + 9
+PART_OF_FORTUNE = POINT + 10
+PART_OF_SPIRIT = POINT + 11
+PART_OF_EROS = POINT + 12
 
 """ Fixed stars. """
 FIXED_STAR = 7 * TYPE_MULTIPLIER
 
 """ Pre & post-natal eclipses. """
 ECLIPSE = 8 * TYPE_MULTIPLIER
 PRE_NATAL_SOLAR_ECLIPSE = ECLIPSE + 1
```

### Comparing `immanuel-1.3.3/immanuel/const/data.py` & `immanuel-1.4.0/immanuel/const/data.py`

 * *Files identical despite different names*

### Comparing `immanuel-1.3.3/immanuel/const/dignities.py` & `immanuel-1.4.0/immanuel/const/dignities.py`

 * *Files identical despite different names*

### Comparing `immanuel-1.3.3/immanuel/const/names.py` & `immanuel-1.4.0/immanuel/const/names.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,16 +127,19 @@
     chart.NORTH_NODE: 'North Node',
     chart.SOUTH_NODE: 'South Node',
     chart.TRUE_NORTH_NODE: 'True North Node',
     chart.TRUE_SOUTH_NODE: 'True South Node',
     chart.VERTEX: 'Vertex',
     chart.LILITH: 'Lilith',
     chart.TRUE_LILITH: 'True Lilith',
+    chart.INTERPOLATED_LILITH: 'Interpolated Lilith',
     chart.SYZYGY: 'Syzygy',
-    chart.PARS_FORTUNA: 'Part of Fortune',
+    chart.PART_OF_FORTUNE: 'Part of Fortune',
+    chart.PART_OF_SPIRIT: 'Part of Spirit',
+    chart.PART_OF_EROS: 'Part of Eros',
 }
 
 ECLIPSES = {
     chart.PRE_NATAL_LUNAR_ECLIPSE: 'Pre-natal Lunar Eclipse',
     chart.PRE_NATAL_SOLAR_ECLIPSE: 'Pre-natal Solar Eclipse',
     chart.POST_NATAL_LUNAR_ECLIPSE: 'Post-natal Lunar Eclipse',
     chart.POST_NATAL_SOLAR_ECLIPSE: 'Post-natal Solar Eclipse',
```

### Comparing `immanuel-1.3.3/immanuel/locales/es_ES/LC_MESSAGES/immanuel.mo` & `immanuel-1.4.0/immanuel/locales/pt_BR/LC_MESSAGES/immanuel.mo`

 * *Files 10% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,11 +1,11 @@
 msgid ""
 msgstr ""
 "Last-Translator: Nathan Octavio\n"
-"Language: Spanish\n"
+"Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 
 msgid "10th House"
 msgstr "Casa 10"
 
@@ -51,433 +51,442 @@
 msgid "9th House"
 msgstr "Casa 9"
 
 msgid "ARMC"
 msgstr "ARMC"
 
 msgid "Air"
-msgstr "Aire"
+msgstr "Ar"
 
 msgid "Alcabitus"
 msgstr "Alcabitius"
 
 msgid "Angle"
-msgstr "Ángulo"
+msgstr "Ângulo"
 
 msgid "Annular"
 msgstr "Anelar"
 
 msgid "Annular Total"
 msgstr "Anelar Total"
 
 msgid "Aquarius"
-msgstr "Acuario"
+msgstr "Aquário"
 
 msgid "Aries"
-msgstr "Aries"
+msgstr "Áries"
 
 msgid "Asc"
 msgstr "Ascendente"
 
 msgid "Asteroid"
-msgstr "Asteroide"
+msgstr "Asteróide"
 
 msgid "Azimuthal"
 msgstr "Azimutal"
 
 msgid "Balsamic"
 msgstr "Minguante"
 
 msgid "Biquintile"
 msgstr "Biquintil"
 
 msgid "Bowl"
-msgstr "Cuenco"
+msgstr "Tigela"
 
 msgid "Bucket"
-msgstr "Cubo"
+msgstr "Balde"
 
 msgid "Bundle"
-msgstr "Haz"
+msgstr "Feixe"
 
 msgid "Campanus"
 msgstr "Campanus"
 
 msgid "Cancer"
-msgstr "Cáncer"
+msgstr "Câncer"
 
 msgid "Capricorn"
-msgstr "Capricornio"
+msgstr "Capricórnio"
 
 msgid "Cardinal"
 msgstr "Cardinal"
 
 msgid "Ceres"
 msgstr "Ceres"
 
 msgid "Chiron"
-msgstr "Quirón"
+msgstr "Quiron"
 
 msgid "Composite"
-msgstr "Compuesto"
+msgstr "Composto"
 
 msgid "Conjunction"
-msgstr "Conjunción"
+msgstr "Conjunção"
 
 msgid "Daily Houses"
-msgstr "Casas Diarias"
+msgstr "Casas Diárias"
 
 msgid "Desc"
 msgstr "Descendente"
 
 msgid "Detriment"
-msgstr "Em Detrimento"
+msgstr "Em Exílio"
 
 msgid "Disseminating"
-msgstr "Gibosa Menguante"
+msgstr "Minguante Gibosa"
 
 msgid "Earth"
-msgstr "Tierra"
+msgstr "Terra"
 
 msgid "Eclipse"
 msgstr "Eclipse"
 
 msgid "Equal House"
-msgstr "Casas iguales"
+msgstr "Casas iguais"
 
 msgid "Face Ruler"
-msgstr "Regente de Decanato"
+msgstr "Regente de Face"
 
 msgid "Face Ruler by mutual reception"
-msgstr "Regente de Decanato por recepción mutua"
+msgstr "Regente de Face por recepção mútua"
 
 msgid "Fall"
-msgstr "Em Caída"
+msgstr "Em Queda"
 
 msgid "Fire"
-msgstr "Fuego"
+msgstr "Fogo"
 
 msgid "First"
-msgstr "Primero"
+msgstr "Primeiro"
 
 msgid "First Quarter"
-msgstr "Cuarto Creciente"
+msgstr "Quarto Crescente"
 
 msgid "Fixed"
-msgstr "Fijo"
+msgstr "Fixo"
 
 msgid "Fixed star"
-msgstr "Estrella fija"
+msgstr "Estrela fixa"
 
 msgid "Fourth"
-msgstr "Cuarto"
+msgstr "Quarto"
 
 msgid "Full"
-msgstr "Llena"
+msgstr "Cheia"
 
 msgid "Gemini"
-msgstr "Géminis"
+msgstr "Gêmeos"
 
 msgid "House"
 msgstr "Casa"
 
 msgid "IC"
-msgstr "Fondo del Cielo"
+msgstr "Fundo do Céu"
 
 msgid "In rulership element"
-msgstr "En su elemento de regencia"
+msgstr "No elemento de regência"
+
+msgid "Interpolated Lilith"
+msgstr "Lilith interpolada"
 
 msgid "Juno"
 msgstr "Juno"
 
 msgid "Jupiter"
 msgstr "Júpiter"
 
 msgid "Koch"
 msgstr "Koch"
 
 msgid "Leo"
-msgstr "Leo"
+msgstr "Leão"
 
 msgid "Libra"
 msgstr "Libra"
 
 msgid "Lilith"
 msgstr "Lilith"
 
 msgid "Locomotive"
-msgstr "Locomotora"
+msgstr "Locomotiva"
 
 msgid "MC"
-msgstr "Medio Cielo"
+msgstr "Meio do Céu"
 
 msgid "Mars"
 msgstr "Marte"
 
 msgid "Mercury"
-msgstr "Mercurio"
+msgstr "Mercúrio"
 
 msgid "Meridian"
 msgstr "Meridiano"
 
 msgid "Moon"
-msgstr "Luna"
+msgstr "Lua"
 
 msgid "Morinus"
 msgstr "Morinus"
 
 msgid "Mutable"
-msgstr "Mutable"
+msgstr "Mutável"
 
 msgid "Naibod"
 msgstr "Naibod"
 
 msgid "Natal"
 msgstr "Natal"
 
 msgid "Neptune"
-msgstr "Neptuno"
+msgstr "Netuno"
 
 msgid "New"
-msgstr "Nueva"
+msgstr "Nova"
 
 msgid "North Node"
 msgstr "Nodo Norte"
 
 msgid "Opposition"
-msgstr "Oposición"
+msgstr "Oposição"
 
 msgid "Pallas"
-msgstr "Palas"
+msgstr "Pallas"
+
+msgid "Part of Eros"
+msgstr "Parte de Eros"
 
 msgid "Part of Fortune"
-msgstr "Parte de la Fortuna"
+msgstr "Roda da Fortuna"
+
+msgid "Part of Spirit"
+msgstr "Parte do Espírito"
 
 msgid "Partial"
 msgstr "Parcial"
 
 msgid "Penumbral"
 msgstr "Penumbral"
 
 msgid "Pholus"
-msgstr "Folo"
+msgstr "Pholus"
 
 msgid "Pisces"
-msgstr "Piscis"
+msgstr "Peixes"
 
 msgid "Placidus"
 msgstr "Placidus"
 
 msgid "Planet"
 msgstr "Planeta"
 
 msgid "Pluto"
-msgstr "Plutón"
+msgstr "Plutão"
 
 msgid "Point"
-msgstr "Punto"
+msgstr "Ponto"
 
 msgid "Polich Page"
 msgstr "Polich Page"
 
 msgid "Porphyrius"
-msgstr "Porfirio"
+msgstr "Porfírio"
 
 msgid "Post-natal Lunar Eclipse"
-msgstr "Eclipse Lunar Postnatal"
+msgstr "Eclipse Lunar Pós-natal"
 
 msgid "Post-natal Solar Eclipse"
-msgstr "Eclipse Solar Postnatal"
+msgstr "Eclipse Solar Pós-natal"
 
 msgid "Pre-natal Lunar Eclipse"
-msgstr "Eclipse Lunar Prenatal"
+msgstr "Eclipse Lunar Pré-natal"
 
 msgid "Pre-natal Solar Eclipse"
-msgstr "Eclipse Solar Prenatal"
+msgstr "Eclipse Solar Pré-natal"
 
 msgid "Progressed"
-msgstr "Progressado"
+msgstr "Progredido"
 
 msgid "Quincunx"
-msgstr "Quincuncio"
+msgstr "Quincúncio"
 
 msgid "Quintile"
 msgstr "Quintil"
 
 msgid "Regiomontanus"
 msgstr "Regiomontanus"
 
 msgid "Ruler"
 msgstr "Regente"
 
 msgid "Ruler by mutual reception"
-msgstr "Regente por recepción mutua"
+msgstr "Regente por recepção mútua"
 
 msgid "Sagittarius"
-msgstr "Sagitario"
+msgstr "Sagitário"
 
 msgid "Saturn"
 msgstr "Saturno"
 
 msgid "Scorpio"
-msgstr "Escorpio"
+msgstr "Escorpião"
 
 msgid "Second"
 msgstr "Segundo"
 
 msgid "Seesaw"
-msgstr "Balancín"
+msgstr "Gangorra"
 
 msgid "Semisextile"
-msgstr "Semisextil"
+msgstr "Semi-sextil"
 
 msgid "Semisquare"
-msgstr "Semiquadratura"
+msgstr "Semi-quadratura"
 
 msgid "Septile"
 msgstr "Septil"
 
 msgid "Sesquisquare"
-msgstr "Sesquicuadratura"
+msgstr "Sesqui-quadratura"
 
 msgid "Sextile"
 msgstr "Sextil"
 
 msgid "Solar Arc"
 msgstr "Arco Solar"
 
 msgid "Solar Return"
 msgstr "Retorno Solar"
 
 msgid "South Node"
-msgstr "Nodo Sur"
+msgstr "Nodo Sul"
 
 msgid "Splash"
-msgstr "Salpicadura"
+msgstr "Salpicado"
 
 msgid "Splay"
-msgstr "Disperso"
+msgstr "Espalhado"
 
 msgid "Square"
-msgstr "Cuadratura"
+msgstr "Quadratura"
 
 msgid "Sun"
 msgstr "Sol"
 
 msgid "Syzygy"
-msgstr "Sizigia"
+msgstr "Sizígia"
 
 msgid "Taurus"
-msgstr "Tauro"
+msgstr "Touro"
 
 msgid "Term Ruler"
-msgstr "Regente de Término"
+msgstr "Regente de Termo"
 
 msgid "Term Ruler by mutual reception"
-msgstr "Regente de Término por recepción mutua"
+msgstr "Regente de Termo por recepção mútua"
 
 msgid "Third"
-msgstr "Tercero"
+msgstr "Terceiro"
 
 msgid "Third Quarter"
-msgstr "Cuarto Menguante"
+msgstr "Quarto Minguante"
 
 msgid "Total"
 msgstr "Total"
 
 msgid "Trine"
 msgstr "Trígono"
 
 msgid "Triplicity Ruler"
-msgstr "Regente de Triplicidad"
+msgstr "Regente de Triplicidade"
 
 msgid "Triplicity Ruler by mutual reception"
-msgstr "Regente de Triplicidad por recepción mutua"
+msgstr "Regente de Triplicidade por recepção mútua"
 
 msgid "True Lilith"
-msgstr "Lilith Verdadera"
+msgstr "Lilith Verdadeira"
 
 msgid "True North Node"
-msgstr "Nodo Norte Verdadero"
+msgstr "Nodo Norte Verdadeiro"
 
 msgid "True South Node"
-msgstr "Nodo Sur Verdadero"
+msgstr "Nodo Sul Verdadeiro"
 
 msgid "Uranus"
 msgstr "Urano"
 
 msgid "Vehlow Equal House"
 msgstr "Vehlow"
 
 msgid "Venus"
-msgstr "Venus"
+msgstr "Vênus"
 
 msgid "Vertex"
-msgstr "Vértice"
+msgstr "Vertex"
 
 msgid "Vesta"
 msgstr "Vesta"
 
 msgid "Virgo"
-msgstr "Virgo"
+msgstr "Virgem"
 
 msgid "Water"
-msgstr "Agua"
+msgstr "Água"
 
 msgid "Waxing Crescent"
-msgstr "Creciente"
+msgstr "Crescente"
 
 msgid "Waxing Gibbous"
-msgstr "Gibosa Creciente"
+msgstr "Crescente Gibosa"
 
 msgid "Whole Sign"
-msgstr "Signos enteros"
+msgstr "Signos Inteiros"
 
 msgid "ambiguous"
 msgstr "ambíguo"
 
 msgctxt "ambiguous"
 msgid "Direct"
-msgstr "Directo(a)"
+msgstr "Direto(a)"
 
 msgctxt "ambiguous"
 msgid "Retrograde"
 msgstr "Retrógrado(a)"
 
 msgctxt "ambiguous"
 msgid "Stationary"
-msgstr "Estacionario(a)"
+msgstr "Estacionário(a)"
 
 msgctxt "feminine"
 msgid "Applicative"
 msgstr "Aplicativa"
 
 msgctxt "feminine"
 msgid "Associate"
-msgstr "Asociada"
+msgstr "Associada"
 
 msgctxt "feminine"
 msgid "Direct"
-msgstr "Directa"
+msgstr "Direta"
 
 msgctxt "feminine"
 msgid "Dissociate"
-msgstr "Disociada"
+msgstr "Dissociada"
 
 msgctxt "feminine"
 msgid "Exact"
 msgstr "Exacta"
 
 msgctxt "feminine"
 msgid "Exalted"
 msgstr "Exaltada"
 
 msgctxt "feminine"
 msgid "Exalted by mutual reception"
-msgstr "Exaltada por recepción mutua"
+msgstr "Exaltada por recepção mútua"
 
 msgctxt "feminine"
 msgid "Peregrine"
 msgstr "Peregrina"
 
 msgctxt "feminine"
 msgid "Retrograde"
@@ -485,43 +494,43 @@
 
 msgctxt "feminine"
 msgid "Separative"
 msgstr "Separativa"
 
 msgctxt "feminine"
 msgid "Stationary"
-msgstr "Estacionaria"
+msgstr "Estacionária"
 
 msgctxt "masculine"
 msgid "Applicative"
 msgstr "Aplicativo"
 
 msgctxt "masculine"
 msgid "Associate"
-msgstr "Asociado"
+msgstr "Associado"
 
 msgctxt "masculine"
 msgid "Direct"
-msgstr "Directo"
+msgstr "Direto"
 
 msgctxt "masculine"
 msgid "Dissociate"
-msgstr "Disociado"
+msgstr "Dissociado"
 
 msgctxt "masculine"
 msgid "Exact"
 msgstr "Exacto"
 
 msgctxt "masculine"
 msgid "Exalted"
 msgstr "Exaltado"
 
 msgctxt "masculine"
 msgid "Exalted by mutual reception"
-msgstr "Exaltado por recepción mutua"
+msgstr "Exaltado por recepção mútua"
 
 msgctxt "masculine"
 msgid "Peregrine"
 msgstr "Peregrino"
 
 msgctxt "masculine"
 msgid "Retrograde"
@@ -529,19 +538,19 @@
 
 msgctxt "masculine"
 msgid "Separative"
 msgstr "Separativo"
 
 msgctxt "masculine"
 msgid "Stationary"
-msgstr "Estacionario"
+msgstr "Estacionário"
 
 msgid "{active} {passive} {type} within {difference} ({movement}, {condition})"
 msgstr ""
-"{type} entre {active} y {passive} dentro de {difference} ({movement}, "
+"{type} entre {active} e {passive} dentro de {difference} ({movement}, "
 "{condition})"
 
 msgid "{date_time} at {lat}, {lon}"
-msgstr "{date_time} en {lat}, {lon}"
+msgstr "{date_time} em {lat}, {lon}"
 
 msgid "{name} {longitude} in {sign}"
-msgstr "{name} {longitude} en {sign}"
+msgstr "{name} {longitude} em {sign}"
```

### Comparing `immanuel-1.3.3/immanuel/locales/es_ES/mappings.py` & `immanuel-1.4.0/immanuel/locales/es_ES/mappings.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,16 +38,19 @@
     chart.NORTH_NODE: genders.MASCULINE,
     chart.SOUTH_NODE: genders.MASCULINE,
     chart.TRUE_NORTH_NODE: genders.MASCULINE,
     chart.TRUE_SOUTH_NODE: genders.MASCULINE,
     chart.VERTEX: genders.MASCULINE,
     chart.LILITH: genders.FEMININE,
     chart.TRUE_LILITH: genders.FEMININE,
+    chart.INTERPOLATED_LILITH: genders.FEMININE,
     chart.SYZYGY: genders.FEMININE,
-    chart.PARS_FORTUNA: genders.FEMININE,
+    chart.PART_OF_FORTUNE: genders.FEMININE,
+    chart.PART_OF_SPIRIT: genders.FEMININE,
+    chart.PART_OF_EROS: genders.FEMININE,
 
     chart.PRE_NATAL_SOLAR_ECLIPSE: genders.MASCULINE,
     chart.PRE_NATAL_LUNAR_ECLIPSE: genders.MASCULINE,
     chart.POST_NATAL_SOLAR_ECLIPSE: genders.MASCULINE,
     chart.POST_NATAL_LUNAR_ECLIPSE: genders.MASCULINE,
 
     calc.CONJUNCTION: genders.FEMININE,
```

### Comparing `immanuel-1.3.3/immanuel/locales/pt_BR/LC_MESSAGES/immanuel.mo` & `immanuel-1.4.0/immanuel/locales/es_ES/LC_MESSAGES/immanuel.mo`

 * *Files 17% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,11 +1,11 @@
 msgid ""
 msgstr ""
 "Last-Translator: Nathan Octavio\n"
-"Language: \n"
+"Language: Spanish\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 
 msgid "10th House"
 msgstr "Casa 10"
 
@@ -51,433 +51,442 @@
 msgid "9th House"
 msgstr "Casa 9"
 
 msgid "ARMC"
 msgstr "ARMC"
 
 msgid "Air"
-msgstr "Ar"
+msgstr "Aire"
 
 msgid "Alcabitus"
 msgstr "Alcabitius"
 
 msgid "Angle"
-msgstr "Ângulo"
+msgstr "Ángulo"
 
 msgid "Annular"
 msgstr "Anelar"
 
 msgid "Annular Total"
 msgstr "Anelar Total"
 
 msgid "Aquarius"
-msgstr "Aquário"
+msgstr "Acuario"
 
 msgid "Aries"
-msgstr "Áries"
+msgstr "Aries"
 
 msgid "Asc"
 msgstr "Ascendente"
 
 msgid "Asteroid"
-msgstr "Asteróide"
+msgstr "Asteroide"
 
 msgid "Azimuthal"
 msgstr "Azimutal"
 
 msgid "Balsamic"
 msgstr "Minguante"
 
 msgid "Biquintile"
 msgstr "Biquintil"
 
 msgid "Bowl"
-msgstr "Tigela"
+msgstr "Cuenco"
 
 msgid "Bucket"
-msgstr "Balde"
+msgstr "Cubo"
 
 msgid "Bundle"
-msgstr "Feixe"
+msgstr "Haz"
 
 msgid "Campanus"
 msgstr "Campanus"
 
 msgid "Cancer"
-msgstr "Câncer"
+msgstr "Cáncer"
 
 msgid "Capricorn"
-msgstr "Capricórnio"
+msgstr "Capricornio"
 
 msgid "Cardinal"
 msgstr "Cardinal"
 
 msgid "Ceres"
 msgstr "Ceres"
 
 msgid "Chiron"
-msgstr "Quiron"
+msgstr "Quirón"
 
 msgid "Composite"
-msgstr "Composto"
+msgstr "Compuesto"
 
 msgid "Conjunction"
-msgstr "Conjunção"
+msgstr "Conjunción"
 
 msgid "Daily Houses"
-msgstr "Casas Diárias"
+msgstr "Casas Diarias"
 
 msgid "Desc"
 msgstr "Descendente"
 
 msgid "Detriment"
-msgstr "Em Exílio"
+msgstr "Em Detrimento"
 
 msgid "Disseminating"
-msgstr "Minguante Gibosa"
+msgstr "Gibosa Menguante"
 
 msgid "Earth"
-msgstr "Terra"
+msgstr "Tierra"
 
 msgid "Eclipse"
 msgstr "Eclipse"
 
 msgid "Equal House"
-msgstr "Casas iguais"
+msgstr "Casas iguales"
 
 msgid "Face Ruler"
-msgstr "Regente de Face"
+msgstr "Regente de Decanato"
 
 msgid "Face Ruler by mutual reception"
-msgstr "Regente de Face por recepção mútua"
+msgstr "Regente de Decanato por recepción mutua"
 
 msgid "Fall"
-msgstr "Em Queda"
+msgstr "Em Caída"
 
 msgid "Fire"
-msgstr "Fogo"
+msgstr "Fuego"
 
 msgid "First"
-msgstr "Primeiro"
+msgstr "Primero"
 
 msgid "First Quarter"
-msgstr "Quarto Crescente"
+msgstr "Cuarto Creciente"
 
 msgid "Fixed"
-msgstr "Fixo"
+msgstr "Fijo"
 
 msgid "Fixed star"
-msgstr "Estrela fixa"
+msgstr "Estrella fija"
 
 msgid "Fourth"
-msgstr "Quarto"
+msgstr "Cuarto"
 
 msgid "Full"
-msgstr "Cheia"
+msgstr "Llena"
 
 msgid "Gemini"
-msgstr "Gêmeos"
+msgstr "Géminis"
 
 msgid "House"
 msgstr "Casa"
 
 msgid "IC"
-msgstr "Fundo do Céu"
+msgstr "Fondo del Cielo"
 
 msgid "In rulership element"
-msgstr "No elemento de regência"
+msgstr "En su elemento de regencia"
+
+msgid "Interpolated Lilith"
+msgstr "Lilith interpolada"
 
 msgid "Juno"
 msgstr "Juno"
 
 msgid "Jupiter"
 msgstr "Júpiter"
 
 msgid "Koch"
 msgstr "Koch"
 
 msgid "Leo"
-msgstr "Leão"
+msgstr "Leo"
 
 msgid "Libra"
 msgstr "Libra"
 
 msgid "Lilith"
 msgstr "Lilith"
 
 msgid "Locomotive"
-msgstr "Locomotiva"
+msgstr "Locomotora"
 
 msgid "MC"
-msgstr "Meio do Céu"
+msgstr "Medio Cielo"
 
 msgid "Mars"
 msgstr "Marte"
 
 msgid "Mercury"
-msgstr "Mercúrio"
+msgstr "Mercurio"
 
 msgid "Meridian"
 msgstr "Meridiano"
 
 msgid "Moon"
-msgstr "Lua"
+msgstr "Luna"
 
 msgid "Morinus"
 msgstr "Morinus"
 
 msgid "Mutable"
-msgstr "Mutável"
+msgstr "Mutable"
 
 msgid "Naibod"
 msgstr "Naibod"
 
 msgid "Natal"
 msgstr "Natal"
 
 msgid "Neptune"
-msgstr "Netuno"
+msgstr "Neptuno"
 
 msgid "New"
-msgstr "Nova"
+msgstr "Nueva"
 
 msgid "North Node"
 msgstr "Nodo Norte"
 
 msgid "Opposition"
-msgstr "Oposição"
+msgstr "Oposición"
 
 msgid "Pallas"
-msgstr "Pallas"
+msgstr "Palas"
+
+msgid "Part of Eros"
+msgstr "Parte de Eros"
 
 msgid "Part of Fortune"
-msgstr "Roda da Fortuna"
+msgstr "Parte de la Fortuna"
+
+msgid "Part of Spirit"
+msgstr "Parte del Espíritu"
 
 msgid "Partial"
 msgstr "Parcial"
 
 msgid "Penumbral"
 msgstr "Penumbral"
 
 msgid "Pholus"
-msgstr "Pholus"
+msgstr "Folo"
 
 msgid "Pisces"
-msgstr "Peixes"
+msgstr "Piscis"
 
 msgid "Placidus"
 msgstr "Placidus"
 
 msgid "Planet"
 msgstr "Planeta"
 
 msgid "Pluto"
-msgstr "Plutão"
+msgstr "Plutón"
 
 msgid "Point"
-msgstr "Ponto"
+msgstr "Punto"
 
 msgid "Polich Page"
 msgstr "Polich Page"
 
 msgid "Porphyrius"
-msgstr "Porfírio"
+msgstr "Porfirio"
 
 msgid "Post-natal Lunar Eclipse"
-msgstr "Eclipse Lunar Pós-natal"
+msgstr "Eclipse Lunar Postnatal"
 
 msgid "Post-natal Solar Eclipse"
-msgstr "Eclipse Solar Pós-natal"
+msgstr "Eclipse Solar Postnatal"
 
 msgid "Pre-natal Lunar Eclipse"
-msgstr "Eclipse Lunar Pré-natal"
+msgstr "Eclipse Lunar Prenatal"
 
 msgid "Pre-natal Solar Eclipse"
-msgstr "Eclipse Solar Pré-natal"
+msgstr "Eclipse Solar Prenatal"
 
 msgid "Progressed"
-msgstr "Progredido"
+msgstr "Progressado"
 
 msgid "Quincunx"
-msgstr "Quincúncio"
+msgstr "Quincuncio"
 
 msgid "Quintile"
 msgstr "Quintil"
 
 msgid "Regiomontanus"
 msgstr "Regiomontanus"
 
 msgid "Ruler"
 msgstr "Regente"
 
 msgid "Ruler by mutual reception"
-msgstr "Regente por recepção mútua"
+msgstr "Regente por recepción mutua"
 
 msgid "Sagittarius"
-msgstr "Sagitário"
+msgstr "Sagitario"
 
 msgid "Saturn"
 msgstr "Saturno"
 
 msgid "Scorpio"
-msgstr "Escorpião"
+msgstr "Escorpio"
 
 msgid "Second"
 msgstr "Segundo"
 
 msgid "Seesaw"
-msgstr "Gangorra"
+msgstr "Balancín"
 
 msgid "Semisextile"
-msgstr "Semi-sextil"
+msgstr "Semisextil"
 
 msgid "Semisquare"
-msgstr "Semi-quadratura"
+msgstr "Semiquadratura"
 
 msgid "Septile"
 msgstr "Septil"
 
 msgid "Sesquisquare"
-msgstr "Sesqui-quadratura"
+msgstr "Sesquicuadratura"
 
 msgid "Sextile"
 msgstr "Sextil"
 
 msgid "Solar Arc"
 msgstr "Arco Solar"
 
 msgid "Solar Return"
 msgstr "Retorno Solar"
 
 msgid "South Node"
-msgstr "Nodo Sul"
+msgstr "Nodo Sur"
 
 msgid "Splash"
-msgstr "Salpicado"
+msgstr "Salpicadura"
 
 msgid "Splay"
-msgstr "Espalhado"
+msgstr "Disperso"
 
 msgid "Square"
-msgstr "Quadratura"
+msgstr "Cuadratura"
 
 msgid "Sun"
 msgstr "Sol"
 
 msgid "Syzygy"
-msgstr "Sizígia"
+msgstr "Sizigia"
 
 msgid "Taurus"
-msgstr "Touro"
+msgstr "Tauro"
 
 msgid "Term Ruler"
-msgstr "Regente de Termo"
+msgstr "Regente de Término"
 
 msgid "Term Ruler by mutual reception"
-msgstr "Regente de Termo por recepção mútua"
+msgstr "Regente de Término por recepción mutua"
 
 msgid "Third"
-msgstr "Terceiro"
+msgstr "Tercero"
 
 msgid "Third Quarter"
-msgstr "Quarto Minguante"
+msgstr "Cuarto Menguante"
 
 msgid "Total"
 msgstr "Total"
 
 msgid "Trine"
 msgstr "Trígono"
 
 msgid "Triplicity Ruler"
-msgstr "Regente de Triplicidade"
+msgstr "Regente de Triplicidad"
 
 msgid "Triplicity Ruler by mutual reception"
-msgstr "Regente de Triplicidade por recepção mútua"
+msgstr "Regente de Triplicidad por recepción mutua"
 
 msgid "True Lilith"
-msgstr "Lilith Verdadeira"
+msgstr "Lilith Verdadera"
 
 msgid "True North Node"
-msgstr "Nodo Norte Verdadeiro"
+msgstr "Nodo Norte Verdadero"
 
 msgid "True South Node"
-msgstr "Nodo Sul Verdadeiro"
+msgstr "Nodo Sur Verdadero"
 
 msgid "Uranus"
 msgstr "Urano"
 
 msgid "Vehlow Equal House"
 msgstr "Vehlow"
 
 msgid "Venus"
-msgstr "Vênus"
+msgstr "Venus"
 
 msgid "Vertex"
-msgstr "Vertex"
+msgstr "Vértice"
 
 msgid "Vesta"
 msgstr "Vesta"
 
 msgid "Virgo"
-msgstr "Virgem"
+msgstr "Virgo"
 
 msgid "Water"
-msgstr "Água"
+msgstr "Agua"
 
 msgid "Waxing Crescent"
-msgstr "Crescente"
+msgstr "Creciente"
 
 msgid "Waxing Gibbous"
-msgstr "Crescente Gibosa"
+msgstr "Gibosa Creciente"
 
 msgid "Whole Sign"
-msgstr "Signos Inteiros"
+msgstr "Signos enteros"
 
 msgid "ambiguous"
 msgstr "ambíguo"
 
 msgctxt "ambiguous"
 msgid "Direct"
-msgstr "Direto(a)"
+msgstr "Directo(a)"
 
 msgctxt "ambiguous"
 msgid "Retrograde"
 msgstr "Retrógrado(a)"
 
 msgctxt "ambiguous"
 msgid "Stationary"
-msgstr "Estacionário(a)"
+msgstr "Estacionario(a)"
 
 msgctxt "feminine"
 msgid "Applicative"
 msgstr "Aplicativa"
 
 msgctxt "feminine"
 msgid "Associate"
-msgstr "Associada"
+msgstr "Asociada"
 
 msgctxt "feminine"
 msgid "Direct"
-msgstr "Direta"
+msgstr "Directa"
 
 msgctxt "feminine"
 msgid "Dissociate"
-msgstr "Dissociada"
+msgstr "Disociada"
 
 msgctxt "feminine"
 msgid "Exact"
 msgstr "Exacta"
 
 msgctxt "feminine"
 msgid "Exalted"
 msgstr "Exaltada"
 
 msgctxt "feminine"
 msgid "Exalted by mutual reception"
-msgstr "Exaltada por recepção mútua"
+msgstr "Exaltada por recepción mutua"
 
 msgctxt "feminine"
 msgid "Peregrine"
 msgstr "Peregrina"
 
 msgctxt "feminine"
 msgid "Retrograde"
@@ -485,43 +494,43 @@
 
 msgctxt "feminine"
 msgid "Separative"
 msgstr "Separativa"
 
 msgctxt "feminine"
 msgid "Stationary"
-msgstr "Estacionária"
+msgstr "Estacionaria"
 
 msgctxt "masculine"
 msgid "Applicative"
 msgstr "Aplicativo"
 
 msgctxt "masculine"
 msgid "Associate"
-msgstr "Associado"
+msgstr "Asociado"
 
 msgctxt "masculine"
 msgid "Direct"
-msgstr "Direto"
+msgstr "Directo"
 
 msgctxt "masculine"
 msgid "Dissociate"
-msgstr "Dissociado"
+msgstr "Disociado"
 
 msgctxt "masculine"
 msgid "Exact"
 msgstr "Exacto"
 
 msgctxt "masculine"
 msgid "Exalted"
 msgstr "Exaltado"
 
 msgctxt "masculine"
 msgid "Exalted by mutual reception"
-msgstr "Exaltado por recepção mútua"
+msgstr "Exaltado por recepción mutua"
 
 msgctxt "masculine"
 msgid "Peregrine"
 msgstr "Peregrino"
 
 msgctxt "masculine"
 msgid "Retrograde"
@@ -529,22 +538,19 @@
 
 msgctxt "masculine"
 msgid "Separative"
 msgstr "Separativo"
 
 msgctxt "masculine"
 msgid "Stationary"
-msgstr "Estacionário"
+msgstr "Estacionario"
 
 msgid "{active} {passive} {type} within {difference} ({movement}, {condition})"
 msgstr ""
-"{type} entre {active} e {passive} dentro de {difference} ({movement}, "
+"{type} entre {active} y {passive} dentro de {difference} ({movement}, "
 "{condition})"
 
 msgid "{date_time} at {lat}, {lon}"
-msgstr "{date_time} em {lat}, {lon}"
+msgstr "{date_time} en {lat}, {lon}"
 
 msgid "{name} {longitude} in {sign}"
-msgstr "{name} {longitude} em {sign}"
-
-msgid "{name} {longitude} in {sign}, {house}"
-msgstr "{name} {longitude} em {sign}, {house}"
+msgstr "{name} {longitude} en {sign}"
```

### Comparing `immanuel-1.3.3/immanuel/locales/pt_BR/mappings.py` & `immanuel-1.4.0/immanuel/locales/pt_BR/mappings.py`

 * *Files 9% similar despite different names*

```diff
@@ -38,16 +38,19 @@
     chart.NORTH_NODE: genders.MASCULINE,
     chart.SOUTH_NODE: genders.MASCULINE,
     chart.TRUE_NORTH_NODE: genders.MASCULINE,
     chart.TRUE_SOUTH_NODE: genders.MASCULINE,
     chart.VERTEX: genders.MASCULINE,
     chart.LILITH: genders.FEMININE,
     chart.TRUE_LILITH: genders.FEMININE,
+    chart.INTERPOLATED_LILITH: genders.FEMININE,
     chart.SYZYGY: genders.FEMININE,
-    chart.PARS_FORTUNA: genders.FEMININE,
+    chart.PART_OF_FORTUNE: genders.FEMININE,
+    chart.PART_OF_SPIRIT: genders.FEMININE,
+    chart.PART_OF_EROS: genders.FEMININE,
 
     chart.PRE_NATAL_SOLAR_ECLIPSE: genders.MASCULINE,
     chart.PRE_NATAL_LUNAR_ECLIPSE: genders.MASCULINE,
     chart.POST_NATAL_SOLAR_ECLIPSE: genders.MASCULINE,
     chart.POST_NATAL_LUNAR_ECLIPSE: genders.MASCULINE,
 
     calc.CONJUNCTION: genders.FEMININE,
```

### Comparing `immanuel-1.3.3/immanuel/reports/aspect.py` & `immanuel-1.4.0/immanuel/reports/aspect.py`

 * *Files identical despite different names*

### Comparing `immanuel-1.3.3/immanuel/reports/dignity.py` & `immanuel-1.4.0/immanuel/reports/dignity.py`

 * *Files identical despite different names*

### Comparing `immanuel-1.3.3/immanuel/reports/pattern.py` & `immanuel-1.4.0/immanuel/reports/pattern.py`

 * *Files identical despite different names*

### Comparing `immanuel-1.3.3/immanuel/reports/weighting.py` & `immanuel-1.4.0/immanuel/reports/weighting.py`

 * *Files identical despite different names*

### Comparing `immanuel-1.3.3/immanuel/resources/ephemeris/seas_12.se1` & `immanuel-1.4.0/immanuel/resources/ephemeris/seas_12.se1`

 * *Files identical despite different names*

### Comparing `immanuel-1.3.3/immanuel/resources/ephemeris/seas_18.se1` & `immanuel-1.4.0/immanuel/resources/ephemeris/seas_18.se1`

 * *Files identical despite different names*

### Comparing `immanuel-1.3.3/immanuel/resources/ephemeris/seas_24.se1` & `immanuel-1.4.0/immanuel/resources/ephemeris/seas_24.se1`

 * *Files identical despite different names*

### Comparing `immanuel-1.3.3/immanuel/resources/ephemeris/semo_12.se1` & `immanuel-1.4.0/immanuel/resources/ephemeris/semo_12.se1`

 * *Files identical despite different names*

### Comparing `immanuel-1.3.3/immanuel/resources/ephemeris/semo_18.se1` & `immanuel-1.4.0/immanuel/resources/ephemeris/semo_18.se1`

 * *Files identical despite different names*

### Comparing `immanuel-1.3.3/immanuel/resources/ephemeris/semo_24.se1` & `immanuel-1.4.0/immanuel/resources/ephemeris/semo_24.se1`

 * *Files identical despite different names*

### Comparing `immanuel-1.3.3/immanuel/resources/ephemeris/semo_36.se1` & `immanuel-1.4.0/immanuel/resources/ephemeris/semo_36.se1`

 * *Files identical despite different names*

### Comparing `immanuel-1.3.3/immanuel/resources/ephemeris/semo_42.se1` & `immanuel-1.4.0/immanuel/resources/ephemeris/semo_42.se1`

 * *Files identical despite different names*

### Comparing `immanuel-1.3.3/immanuel/resources/ephemeris/sepl_12.se1` & `immanuel-1.4.0/immanuel/resources/ephemeris/sepl_12.se1`

 * *Files identical despite different names*

### Comparing `immanuel-1.3.3/immanuel/resources/ephemeris/sepl_18.se1` & `immanuel-1.4.0/immanuel/resources/ephemeris/sepl_18.se1`

 * *Files identical despite different names*

### Comparing `immanuel-1.3.3/immanuel/resources/ephemeris/sepl_24.se1` & `immanuel-1.4.0/immanuel/resources/ephemeris/sepl_24.se1`

 * *Files identical despite different names*

### Comparing `immanuel-1.3.3/immanuel/resources/ephemeris/sepl_36.se1` & `immanuel-1.4.0/immanuel/resources/ephemeris/sepl_36.se1`

 * *Files identical despite different names*

### Comparing `immanuel-1.3.3/immanuel/resources/ephemeris/sepl_42.se1` & `immanuel-1.4.0/immanuel/resources/ephemeris/sepl_42.se1`

 * *Files identical despite different names*

### Comparing `immanuel-1.3.3/immanuel/setup.py` & `immanuel-1.4.0/immanuel/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,22 +97,25 @@
         self.default_longitude = -0.0015
 
         """ Whether or not the stringified output of chart objects should
         always display the object's motion even when it is typical for
         that object. """
         self.output_typical_object_motion = False
 
+        """ Rounding for formatted angle strings. """
+        self.angle_precision = calc.SECOND
+
         """ House system as supported by pyswisseph. """
         self.house_system = chart.PLACIDUS
 
         """ Which planets, points etc. to show. """
         self.objects = [
             chart.ASC, chart.DESC, chart.MC, chart.IC,
             chart.TRUE_NORTH_NODE, chart.TRUE_SOUTH_NODE,
-            chart.VERTEX, chart.PARS_FORTUNA,
+            chart.VERTEX, chart.PART_OF_FORTUNE,
             chart.TRUE_LILITH,
             chart.SUN, chart.MOON, chart.MERCURY, chart.VENUS, chart.MARS,
             chart.JUPITER, chart.SATURN, chart.URANUS, chart.NEPTUNE, chart.PLUTO,
             chart.CHIRON,
         ]
 
         """ Which planets, points etc. to use in chart shape calculations. """
@@ -166,16 +169,16 @@
 
         """ Orb for calculating chart shapes. """
         self.chart_shape_orb = 5.0
 
         """ MC progression formula for secondary progressions. """
         self.mc_progression_method = calc.NAIBOD
 
-        """ Part of Fortune formula. """
-        self.pars_fortuna_formula = calc.DAY_NIGHT_FORMULA
+        """ Part of Fortune / Spirit / Eros formula. """
+        self.part_formula = calc.DAY_NIGHT_FORMULA
 
         """ Dignity settings. """
         self.rulerships = dignities.MODERN_RULERSHIPS
 
         self.triplicities = dignities.PTOLEMAIC_TRIPLICITIES
 
         self.terms = dignities.EGYPTIAN_TERMS
@@ -273,18 +276,21 @@
             chart.PLUTO: self.planet_aspect_rule,
 
             chart.NORTH_NODE: self.point_aspect_rule,
             chart.SOUTH_NODE: self.point_aspect_rule,
             chart.TRUE_NORTH_NODE: self.point_aspect_rule,
             chart.TRUE_SOUTH_NODE: self.point_aspect_rule,
             chart.SYZYGY: self.point_aspect_rule,
-            chart.PARS_FORTUNA: self.point_aspect_rule,
+            chart.PART_OF_FORTUNE: self.point_aspect_rule,
+            chart.PART_OF_SPIRIT: self.point_aspect_rule,
+            chart.PART_OF_EROS: self.point_aspect_rule,
             chart.VERTEX: self.point_aspect_rule,
             chart.LILITH: self.point_aspect_rule,
             chart.TRUE_LILITH: self.point_aspect_rule,
+            chart.INTERPOLATED_LILITH: self.point_aspect_rule,
         } | self._aspect_rules
 
     @aspect_rules.setter
     def aspect_rules(self, value: dict) -> None:
         self._aspect_rules = value
 
     @property
@@ -308,18 +314,21 @@
             chart.PLUTO: self.planet_orbs,
 
             chart.NORTH_NODE: self.point_orbs,
             chart.SOUTH_NODE: self.point_orbs,
             chart.TRUE_NORTH_NODE: self.point_orbs,
             chart.TRUE_SOUTH_NODE: self.point_orbs,
             chart.SYZYGY: self.point_orbs,
-            chart.PARS_FORTUNA: self.point_orbs,
+            chart.PART_OF_FORTUNE: self.point_orbs,
+            chart.PART_OF_SPIRIT: self.point_orbs,
+            chart.PART_OF_EROS: self.point_orbs,
             chart.VERTEX: self.point_orbs,
             chart.LILITH: self.point_orbs,
             chart.TRUE_LILITH: self.point_orbs,
+            chart.INTERPOLATED_LILITH: self.point_orbs,
         } | self._orbs
 
     @orbs.setter
     def orbs(self, value: dict) -> None:
         self._orbs = value
 
     def add_filepath(self, path: str, default: bool = False) -> None:
```

### Comparing `immanuel-1.3.3/immanuel/tools/calculate.py` & `immanuel-1.4.0/immanuel/tools/calculate.py`

 * *Files 23% similar despite different names*

```diff
@@ -27,26 +27,47 @@
 
 def is_daytime(sun: dict | float, asc: dict | float) -> bool:
     """ Returns whether the sun is above the ascendant. """
     sun_lon, asc_lon = (object['lon'] if isinstance(object, dict) else object for object in (sun, asc))
     return swe.difdeg2n(sun_lon, asc_lon) < 0
 
 
-def pars_fortuna_longitude(sun: dict | float, moon: dict | float, asc: dict | float, formula: int) -> float:
-    """ Returns the Part of Fortune longitude. """
+def part_longitude(index: int, sun: dict | float, moon: dict | float, asc: dict | float, venus: dict | float = None, formula: int = calc.DAY_NIGHT_FORMULA) -> float:
+    """ Returns the longitude of the given Part - currently supports Parts of
+    Fortune, Spirit and Eros. """
     sun_lon, moon_lon, asc_lon = (object['lon'] if isinstance(object, dict) else object for object in (sun, moon, asc))
+    night = formula == calc.NIGHT_FORMULA or (formula == calc.DAY_NIGHT_FORMULA and not is_daytime(sun_lon, asc_lon))
 
-    if formula == calc.NIGHT_FORMULA or (formula == calc.DAY_NIGHT_FORMULA and not is_daytime(sun_lon, asc_lon)):
-        lon = asc_lon + sun_lon - moon_lon
-    else:
-        lon = asc_lon + moon_lon - sun_lon
+    if index == chart.PART_OF_FORTUNE:
+        lon = _part_of_fortune(sun_lon, moon_lon, asc_lon, night)
+    elif index == chart.PART_OF_SPIRIT:
+        lon = _part_of_spirit(sun_lon, moon_lon, asc_lon, night)
+    elif index == chart.PART_OF_EROS:
+        venus_lon = venus['lon'] if isinstance(venus, dict) else venus
+        spirit_lon = _part_of_spirit(sun_lon, moon_lon, asc_lon, night)
+        lon = _part_of_eros(venus_lon, spirit_lon, asc_lon, night)
 
     return swe.degnorm(lon)
 
 
+def _part_of_fortune(sun_lon: float, moon_lon: float, asc_lon: float, night: bool) -> float:
+    """ Night & day calculations for Part of Fortune. """
+    return asc_lon + sun_lon - moon_lon if night else asc_lon + moon_lon - sun_lon
+
+
+def _part_of_spirit(sun_lon: float, moon_lon: float, asc_lon: float, night: bool) -> float:
+    """ Night & day calculations for Part of Spirit. """
+    return asc_lon + moon_lon - sun_lon if night else asc_lon + sun_lon - moon_lon
+
+
+def _part_of_eros(venus_lon: float, spirit_lon: float, asc_lon: float, night: bool) -> float:
+    """ Night & day calculations for Part of Eros. """
+    return asc_lon + spirit_lon - venus_lon if night else asc_lon + venus_lon - spirit_lon
+
+
 def sidereal_time(armc: dict | float) -> float:
     """ Returns sidereal time based on ARMC longitude. """
     return (armc['lon'] if isinstance(armc, dict) else armc) / 15
 
 
 def object_movement(object: dict | float) -> int:
     """ Returns whether a chart object is direct, stationary or retrograde. """
@@ -54,34 +75,63 @@
 
     if -calc.STATION_SPEED <= speed <= calc.STATION_SPEED:
         return calc.STATIONARY
 
     return calc.DIRECT if speed > calc.STATION_SPEED else calc.RETROGRADE
 
 
-def object_movement_typical(object: dict) -> bool:
+def is_object_movement_typical(object: dict) -> bool:
     """ Returns whether an object's movement is typical, ie. direct for planets,
-    retrograde for nodes, stationary for Part of Fortune and eclipses. """
-    if object['index'] in (chart.PARS_FORTUNA, chart.PRE_NATAL_SOLAR_ECLIPSE, chart.PRE_NATAL_LUNAR_ECLIPSE, chart.POST_NATAL_SOLAR_ECLIPSE, chart.POST_NATAL_SOLAR_ECLIPSE):
+    retrograde for nodes, stationary for Parts and eclipses. """
+    if object['index'] in (
+            chart.PART_OF_FORTUNE,
+            chart.PART_OF_SPIRIT,
+            chart.PART_OF_EROS,
+            chart.PRE_NATAL_SOLAR_ECLIPSE,
+            chart.PRE_NATAL_LUNAR_ECLIPSE,
+            chart.POST_NATAL_SOLAR_ECLIPSE,
+            chart.POST_NATAL_SOLAR_ECLIPSE
+        ):
         return object['speed'] == 0.0
 
     movement = object_movement(object)
-    is_node = object['index'] in (chart.NORTH_NODE, chart.SOUTH_NODE, chart.TRUE_NORTH_NODE, chart.TRUE_SOUTH_NODE)
+
+    is_node = object['index'] in (
+            chart.NORTH_NODE,
+            chart.SOUTH_NODE,
+            chart.TRUE_NORTH_NODE,
+            chart.TRUE_SOUTH_NODE
+        )
 
     return movement == calc.RETROGRADE if is_node else movement == calc.DIRECT
 
 
 def relative_position(object1: dict | float, object2: dict | float) -> int:
     """ Calculate which side of object1 object2 is. """
     lon1 = object1['lon'] if isinstance(object1, dict) else object1
     lon2 = object2['lon'] if isinstance(object2, dict) else object2
 
     return calc.OCCIDENTAL if swe.difdegn(lon1, lon2) > 180 else calc.ORIENTAL
 
 
+def is_in_sect(object: dict, is_daytime: bool, sun: dict | float = None) -> bool:
+    """ Returns whether the passed planet is in sect. """
+    if object['index'] in (chart.SUN, chart.JUPITER, chart.SATURN):
+        return is_daytime
+
+    if object['index'] in (chart.MOON, chart.VENUS, chart.MARS):
+        return not is_daytime
+
+    if object['index'] == chart.MERCURY:
+        sun_mercury_position = relative_position(sun, object)
+        return sun_mercury_position == calc.ORIENTAL if is_daytime else sun_mercury_position == calc.OCCIDENTAL
+
+    return False
+
+
 def is_out_of_bounds(object: dict | float, jd: float = None, obliquity: float = None) -> bool:
     """ Returns whether the passed object is out of bounds either on the passed
     Julian date or relative to the passed obliquity. """
     if isinstance(object, dict):
         if 'dec' not in object:
             return None
         dec = object['dec']
```

### Comparing `immanuel-1.3.3/immanuel/tools/convert.py` & `immanuel-1.4.0/immanuel/tools/convert.py`

 * *Files identical despite different names*

### Comparing `immanuel-1.3.3/immanuel/tools/date.py` & `immanuel-1.4.0/immanuel/tools/date.py`

 * *Files identical despite different names*

### Comparing `immanuel-1.3.3/immanuel/tools/ephemeris.py` & `immanuel-1.4.0/immanuel/tools/ephemeris.py`

 * *Files 13% similar despite different names*

```diff
@@ -65,74 +65,77 @@
     chart.NORTH_NODE: swe.MEAN_NODE,
     chart.SOUTH_NODE: swe.MEAN_NODE,
     chart.TRUE_NORTH_NODE: swe.TRUE_NODE,
     chart.TRUE_SOUTH_NODE: swe.TRUE_NODE,
     chart.VERTEX: swe.VERTEX,
     chart.LILITH: swe.MEAN_APOG,
     chart.TRUE_LILITH: swe.OSCU_APOG,
+    chart.INTERPOLATED_LILITH: swe.INTP_APOG,
     chart.SYZYGY: chart.SYZYGY,
-    chart.PARS_FORTUNA: chart.PARS_FORTUNA,
+    chart.PART_OF_FORTUNE: chart.PART_OF_FORTUNE,
+    chart.PART_OF_SPIRIT: chart.PART_OF_SPIRIT,
+    chart.PART_OF_EROS: chart.PART_OF_EROS,
 }
 
 
-def objects(object_list: tuple, jd: float, lat: float = None, lon: float = None, house_system: int = None, pars_fortuna_formula: int = None) -> dict:
+def objects(object_list: tuple, jd: float, lat: float = None, lon: float = None, house_system: int = None, part_formula: int = None) -> dict:
     """ Helper function returns a dict of all passed chart objects. """
     return _objects(
         object_list=object_list,
         jd=jd,
         lat=lat,
         lon=lon,
         house_system=house_system,
-        pars_fortuna_formula=pars_fortuna_formula,
+        part_formula=part_formula,
         armc=None,
         armc_obliquity=None
     )
 
 
-def armc_objects(object_list: tuple, jd: float, armc: float, lat: float = None, lon: float = None, obliquity: float = None, house_system: int = None, pars_fortuna_formula: int = None) -> dict:
+def armc_objects(object_list: tuple, jd: float, armc: float, lat: float = None, lon: float = None, obliquity: float = None, house_system: int = None, part_formula: int = None) -> dict:
     """ Helper function returns a dict of all passed chart objects
     with points & angles calculated from the passed ARMC. """
     return _objects(
         object_list=object_list,
         jd=jd,
         lat=lat,
         lon=lon,
         house_system=house_system,
-        pars_fortuna_formula=pars_fortuna_formula,
+        part_formula=part_formula,
         armc=armc,
         armc_obliquity=obliquity
     )
 
 
-def get(index: int | str, jd: float, lat: float = None, lon: float = None, house_system: int = None, pars_fortuna_formula: int = None) -> dict:
+def get(index: int | str, jd: float, lat: float = None, lon: float = None, house_system: int = None, part_formula: int = None) -> dict:
     """ Helper function to retrieve an angle, house, planet, point,
     asteroid, or fixed star. """
     return _get(
         index=index,
         jd=jd,
         lat=lat,
         lon=lon,
         house_system=house_system,
-        pars_fortuna_formula=pars_fortuna_formula,
+        part_formula=part_formula,
         armc=None,
         armc_obliquity=None
     )
 
 
-def armc_get(index: int | str, jd: float, armc: float, lat: float = None, lon: float = None, obliquity: float = None, house_system: int = None, pars_fortuna_formula: int = None) -> dict:
+def armc_get(index: int | str, jd: float, armc: float, lat: float = None, lon: float = None, obliquity: float = None, house_system: int = None, part_formula: int = None) -> dict:
     """ Helper function to retrieve an angle, house, planet, point,
     asteroid, or fixed star with houses & angles calculated from the
     passed ARMC. """
     return _get(
         index=index,
         jd=jd,
         lat=lat,
         lon=lon,
         house_system=house_system,
-        pars_fortuna_formula=pars_fortuna_formula,
+        part_formula=part_formula,
         armc=armc,
         armc_obliquity=obliquity
     )
 
 
 def angles(jd: float, lat: float, lon: float, house_system: int) -> dict:
     """ Returns all four main chart angles & ARMC. """
@@ -238,55 +241,55 @@
         lon=None,
         house_system=house_system,
         armc=armc,
         armc_obliquity=obliquity
     )
 
 
-def point(index: int, jd: float, lat: float = None, lon: float = None, house_system: int = None, pars_fortuna_formula: int = None) -> dict:
+def point(index: int, jd: float, lat: float = None, lon: float = None, house_system: int = None, part_formula: int = None) -> dict:
     """ Returns a calculated point by Julian date, and additionally by lat / lon
     coordinates. """
     return _point(
         index=index,
         jd=jd,
         lat=lat,
         lon=lon,
         house_system=house_system,
-        pars_fortuna_formula=pars_fortuna_formula,
+        part_formula=part_formula,
         armc=None,
         armc_obliquity=None
     )
 
 
-def armc_point(index: int, jd: float, armc: float, lat: float, obliquity: float, house_system: int = None, pars_fortuna_formula: int = None) -> dict:
+def armc_point(index: int, jd: float, armc: float, lat: float, obliquity: float, house_system: int = None, part_formula: int = None) -> dict:
     """ Returns a calculated point by Julian date, and additionally by the
     passed ARMC. """
     return _point(
         index=index,
         jd=jd,
         lat=lat,
         lon=None,
         house_system=house_system,
-        pars_fortuna_formula=pars_fortuna_formula,
+        part_formula=part_formula,
         armc=armc,
         armc_obliquity=obliquity
     )
 
 
-def _objects(object_list: tuple, jd: float, lat: float, lon: float, house_system: int, pars_fortuna_formula: int, armc: float, armc_obliquity: float) -> dict:
+def _objects(object_list: tuple, jd: float, lat: float, lon: float, house_system: int, part_formula: int, armc: float, armc_obliquity: float) -> dict:
     """ Function for items() and armc_items(). """
     objects = {}
 
     for index in object_list:
-        objects[index] = _get(index, jd, lat, lon, house_system, pars_fortuna_formula, armc, armc_obliquity)
+        objects[index] = _get(index, jd, lat, lon, house_system, part_formula, armc, armc_obliquity)
 
     return objects
 
 
-def _get(index: int | str, jd: float, lat: float, lon: float, house_system: int, pars_fortuna_formula: int, armc: float, armc_obliquity: float) -> dict:
+def _get(index: int | str, jd: float, lat: float, lon: float, house_system: int, part_formula: int, armc: float, armc_obliquity: float) -> dict:
     """ Function for get() and armc_get(). """
     if armc is not None and armc_obliquity is None:
         armc_obliquity = obliquity(jd)
 
     if isinstance(index, int):
         if index < chart.TYPE_MULTIPLIER:
             return asteroid(index, jd)
@@ -299,15 +302,15 @@
 
         match _type(index):
             case chart.ANGLE:
                 return _angle(index, jd, lat, lon, house_system, armc, armc_obliquity)
             case chart.HOUSE:
                 return _house(index, jd, lat, lon, house_system, armc, armc_obliquity)
             case chart.POINT:
-                return _point(index, jd, lat, lon, house_system, pars_fortuna_formula, armc, armc_obliquity)
+                return _point(index, jd, lat, lon, house_system, part_formula, armc, armc_obliquity)
             case chart.ECLIPSE:
                 return eclipse(index, jd)
             case (chart.ASTEROID|chart.PLANET):
                 return planet(index, jd)
     else:
         return fixed_star(index, jd)
 
@@ -340,27 +343,27 @@
 
     if index in houses:
         return houses[index]
 
     return None
 
 
-def _point(index: int, jd: float, lat: float, lon: float, house_system: int, pars_fortuna_formula: int, armc: float, armc_obliquity: float) -> dict:
+def _point(index: int, jd: float, lat: float, lon: float, house_system: int, part_formula: int, armc: float, armc_obliquity: float) -> dict:
     """ Function for point() and armc_point(). """
     if index == chart.VERTEX:
         if armc is not None:
             return _angles_houses_vertex_armc(armc, lat, armc_obliquity, house_system)['vertex']
         else:
             return _angles_houses_vertex(jd, lat, lon, house_system)['vertex']
 
     if index == chart.SYZYGY:
         return _syzygy(jd)
 
-    if index == chart.PARS_FORTUNA:
-        return _pars_fortuna(jd, lat, lon, pars_fortuna_formula, armc, armc_obliquity)
+    if index in (chart.PART_OF_FORTUNE, chart.PART_OF_SPIRIT, chart.PART_OF_EROS):
+        return _part(index, jd, lat, lon, part_formula, armc, armc_obliquity)
 
     return _swisseph_point(index, jd)
 
 
 @cache
 def planet(index: int, jd: float) -> dict:
     """ Returns a pyswisseph object by Julian date. Can be used to
@@ -618,28 +621,27 @@
         'lat': syzygy_moon['lat'],
         'speed': syzygy_moon['speed'],
         'dec': syzygy_moon['dec'],
     }
 
 
 @cache
-def _pars_fortuna(jd: float, lat: float, lon: float, formula: int, armc: float = None, armc_obliquity: float = None) -> dict:
-    """ Calculate Part of Fortune - this relies on the ascendant which will be
-    consistent across all supported systems, so it is safe to pass Placidus as
-    the default. """
+def _part(index: int, jd: float, lat: float, lon: float, formula: int, armc: float = None, armc_obliquity: float = None) -> dict:
+    """ Calculates Parts of Fortune, Spirit, and Eros. """
     sun = planet(chart.SUN, jd)
     moon = planet(chart.MOON, jd)
+    venus = planet(chart.VENUS, jd) if index == chart.PART_OF_EROS else None
     asc = angle(chart.ASC, jd, lat, lon, chart.PLACIDUS) if armc is None else armc_angle(chart.ASC, armc, lat, armc_obliquity, chart.PLACIDUS)
-    lon = calculate.pars_fortuna_longitude(sun, moon, asc, formula)
+    lon = calculate.part_longitude(index, sun, moon, asc, venus, formula)
     dec = swe.cotrans((lon, 0, 0), -obliquity(jd))[1]
 
     return {
-        'index': chart.PARS_FORTUNA,
+        'index': index,
         'type': chart.POINT,
-        'name': _(names.POINTS[chart.PARS_FORTUNA]),
+        'name': _(names.POINTS[index]),
         'lon': lon,
         'lat': 0.0,
         'speed': 0.0,
         'dec': dec,
     }
```

### Comparing `immanuel-1.3.3/immanuel/tools/find.py` & `immanuel-1.4.0/immanuel/tools/find.py`

 * *Files identical despite different names*

### Comparing `immanuel-1.3.3/immanuel/tools/forecast.py` & `immanuel-1.4.0/immanuel/tools/forecast.py`

 * *Files identical despite different names*

### Comparing `immanuel-1.3.3/immanuel/tools/midpoint.py` & `immanuel-1.4.0/immanuel/tools/midpoint.py`

 * *Files identical despite different names*

### Comparing `immanuel-1.3.3/immanuel/tools/position.py` & `immanuel-1.4.0/immanuel/tools/position.py`

 * *Files identical despite different names*

### Comparing `immanuel-1.3.3/immanuel.egg-info/PKG-INFO` & `immanuel-1.4.0/immanuel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: immanuel
-Version: 1.3.3
+Version: 1.4.0
 Summary: Quickly produce both human-readable and JSON-formatted astrology chart data based on the Swiss Ephemeris and astro.com.
 Author-email: Robert Davies <robert@theriftlab.com>
 License: # GNU AFFERO GENERAL PUBLIC LICENSE
         
         Version 3, 19 November 2007
         
         Copyright (C) 2007 Free Software Foundation, Inc.
@@ -654,19 +654,19 @@
 
 Immanuel's output is currently available in the following locales / languages:
 
 * **en_US:** (default) US English
 * **pt_BR:** Brazilian Portuguese
 * **es_ES:** Spanish
 
-See [here](https://github.com/theriftlab/immanuel-python/tree/v1.3.3/docs/5-settings.md#locale) for details on how to switch. The documentation itself is not currently available in other translations. To contribute in-software translations, see [here](https://github.com/theriftlab/immanuel-python/tree/v1.3.3/docs/7-contributions.md).
+See [here](https://github.com/theriftlab/immanuel-python/tree/v1.4.0/docs/5-settings.md#locale) for details on how to switch. The documentation itself is not currently available in other translations. To contribute in-software translations, see [here](https://github.com/theriftlab/immanuel-python/tree/v1.4.0/docs/7-contributions.md).
 
 ## Documentation
 
-Full documentation is available [here](https://github.com/theriftlab/immanuel-python/tree/v1.3.3/docs/0-contents.md), or follow the Quick Start below to see how to quickly generate a natal chart.
+Full documentation is available [here](https://github.com/theriftlab/immanuel-python/tree/v1.4.0/docs/0-contents.md), or follow the Quick Start below to see how to quickly generate a natal chart.
 
 ## Quick Start
 
 You can get started with full natal chart data in minutes. Simply install Immanuel:
 
 ```bash
 pip install immanuel
@@ -677,17 +677,29 @@
 ```python
 from immanuel import charts
 
 
 native = charts.Subject(
         date_time='2000-01-01 10:00',
         latitude='32n43',
-        longitude='117w09'
+        longitude='117w09',
     )
 
+# or, alternatively...
+
+from datetime import datetime
+
+native = charts.Subject(
+        date_time=datetime(2000, 1, 1, 10, 0, 0),
+        latitude=32.71667,
+        longitude=-117.15,
+    )
+
+# and then...
+
 natal = charts.Natal(native)
 
 for object in natal.objects.values():
     print(object)
 ```
 
 This will output all the chart objects (planets, points, asteroids etc.) in this format:
@@ -815,14 +827,15 @@
         "formatted": "-23\u00b000'45\"",
         "direction": "-",
         "degrees": 23,
         "minutes": 0,
         "seconds": 45
     },
     "out_of_bounds": false,
+    "in_sect": true,
     "dignities": {
         "ruler": false,
         "exalted": false,
         "triplicity_ruler": false,
         "term_ruler": false,
         "face_ruler": false,
         "mutual_reception_ruler": false,
```

### Comparing `immanuel-1.3.3/immanuel.egg-info/SOURCES.txt` & `immanuel-1.4.0/immanuel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `immanuel-1.3.3/pyproject.toml` & `immanuel-1.4.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "immanuel"
-version = "1.3.3"
+version = "1.4.0"
 description = "Quickly produce both human-readable and JSON-formatted astrology chart data based on the Swiss Ephemeris and astro.com."
 authors = [
   { name = "Robert Davies", email = "robert@theriftlab.com" },
 ]
 license = { file = "LICENSE.md" }
 readme = "README.md"
 keywords = ["astrology", "api", "pyswisseph", "swisseph", "swiss ephemeris", "astro.com", "astro gold"]
```

### Comparing `immanuel-1.3.3/tests/se01181s.se1` & `immanuel-1.4.0/tests/se01181s.se1`

 * *Files identical despite different names*

### Comparing `immanuel-1.3.3/tests/test_aspect.py` & `immanuel-1.4.0/tests/test_aspect.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,17 +46,17 @@
 
 
 def test_for_object(objects):
     settings.aspect_rules = {
         chart.ASC: settings.default_aspect_rule,          # astro.com chart visual does not include aspects to Asc but its aspects table does
     }
     a = aspect.for_object(objects[chart.SUN], objects)
-    assert sorted(tuple(a.keys())) == sorted((chart.ASC, chart.PARS_FORTUNA, chart.MOON, chart.MERCURY, chart.SATURN))
+    assert sorted(tuple(a.keys())) == sorted((chart.ASC, chart.PART_OF_FORTUNE, chart.MOON, chart.MERCURY, chart.SATURN))
     assert a[chart.ASC]['aspect'] == calc.SEXTILE
-    assert a[chart.PARS_FORTUNA]['aspect'] == calc.CONJUNCTION
+    assert a[chart.PART_OF_FORTUNE]['aspect'] == calc.CONJUNCTION
     assert a[chart.MOON]['aspect'] == calc.SEXTILE
     assert a[chart.MERCURY]['aspect'] == calc.CONJUNCTION
     assert a[chart.SATURN]['aspect'] == calc.TRINE
 
 
 def test_all(objects):
     settings.aspect_rules = {
```

### Comparing `immanuel-1.3.3/tests/test_charts.py` & `immanuel-1.4.0/tests/test_charts.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,15 +16,16 @@
 
 from datetime import datetime
 from zoneinfo import ZoneInfo
 
 from pytest import fixture
 
 from immanuel import charts
-from immanuel.const import calc, chart, names
+from immanuel.classes import wrap
+from immanuel.const import calc, chart, dignities, names
 from immanuel.setup import settings
 from immanuel.tools import convert
 
 
 @fixture
 def dob():
     return '2000-01-01 10:00'
@@ -91,14 +92,175 @@
     assert native.julian_date == julian_date
 
     ambiguous_date_time = datetime(2022, 11, 6, 1, 30)
     ambiguous_native = charts.Subject(ambiguous_date_time, lat, lon)
     assert ambiguous_native.date_time_ambiguous == True
 
 
+def test_wrapped_data(native):
+    settings.objects.append(chart.PRE_NATAL_LUNAR_ECLIPSE)
+    natal_chart = charts.Natal(native)
+
+    # Angle
+    longitude = natal_chart.objects[chart.SUN].longitude
+    assert longitude.raw == 280.6237802656368
+    assert longitude.formatted == '280°37\'26"'
+    assert longitude.direction == '+'
+    assert longitude.degrees == 280
+    assert longitude.minutes == 37
+    assert longitude.seconds == 26
+
+    # Aspect
+    aspect = natal_chart.aspects[chart.SUN][chart.MOON]
+    assert aspect.active == chart.MOON
+    assert aspect.passive == chart.SUN
+    assert aspect.type == names.ASPECTS[calc.SEXTILE]
+    assert aspect.aspect == calc.SEXTILE
+    assert aspect.orb == settings.planet_orbs[calc.SEXTILE]
+    assert type(aspect.distance) is wrap.Angle                      # Tested separately, just ensure type
+    assert type(aspect.difference) is wrap.Angle                    # Tested separately, just ensure type
+
+    # AspectCondition
+    assert aspect.condition.associate == True
+    assert aspect.condition.dissociate == False
+    assert aspect.condition.formatted == names.ASPECT_CONDITIONS[calc.ASSOCIATE]
+
+    # AspectMovement
+    assert aspect.movement.applicative == False
+    assert aspect.movement.exact == False
+    assert aspect.movement.separative == True
+    assert aspect.movement.formatted == names.ASPECT_MOVEMENTS[calc.SEPARATIVE]
+
+    # Coordinates
+    assert type(natal_chart.native.coordinates.latitude) is wrap.Angle      # Tested separately, just ensure type
+    assert type(natal_chart.native.coordinates.longitude) is wrap.Angle     # Tested separately, just ensure type
+
+    # DateTime
+    date_time = natal_chart.native.date_time
+    assert type(date_time.datetime) is datetime
+    assert date_time.timezone == 'PST'
+    assert date_time.ambiguous == False
+    assert date_time.julian == 2451545.25
+    assert date_time.deltat == 0.0007387629899254968
+    assert date_time.sidereal_time == '16:54:13'
+
+    # MoonPhase
+    moon_phase = natal_chart.moon_phase
+    assert moon_phase.new_moon == False
+    assert moon_phase.waxing_crescent == False
+    assert moon_phase.first_quarter == False
+    assert moon_phase.waxing_gibbous == False
+    assert moon_phase.full_moon == False
+    assert moon_phase.disseminating == False
+    assert moon_phase.third_quarter == True
+    assert moon_phase.balsamic == False
+    assert moon_phase.formatted == names.MOON_PHASES[calc.THIRD_QUARTER]
+
+    # Object
+    sun = natal_chart.objects[chart.SUN]
+    assert sun.index == chart.SUN
+    assert sun.name == names.PLANETS[chart.SUN]
+    assert sun.distance == 0.9833259257690341
+    assert sun.speed == 1.0194579691359147
+    assert sun.out_of_bounds == False
+    assert sun.in_sect == True
+    assert sun.score == 3
+
+    assert type(sun.latitude) is wrap.Angle             # Tested separately, just ensure type
+    assert type(sun.longitude) is wrap.Angle            # Tested separately, just ensure type
+    assert type(sun.sign_longitude) is wrap.Angle       # Tested separately, just ensure type
+    assert type(sun.declination) is wrap.Angle          # Tested separately, just ensure type
+
+    # ObjectType
+    assert sun.type.index == chart.PLANET
+    assert sun.type.name == names.OBJECTS[chart.PLANET]
+
+    # Sign
+    assert sun.sign.number == chart.CAPRICORN
+    assert sun.sign.name == names.SIGNS[chart.CAPRICORN]
+    assert sun.sign.element == names.ELEMENTS[chart.EARTH]
+    assert sun.sign.modality == names.MODALITIES[chart.CARDINAL]
+
+    # Decan
+    assert sun.decan.number == chart.DECAN2
+    assert sun.decan.name == names.DECANS[chart.DECAN2]
+
+    # House
+    assert sun.house.index == chart.HOUSE11
+    assert sun.house.number == 11
+    assert sun.house.name == names.HOUSES[chart.HOUSE11]
+
+    # ObjectMovement
+    assert sun.movement.direct == True
+    assert sun.movement.stationary == False
+    assert sun.movement.retrograde == False
+    assert sun.movement.typical == True
+    assert sun.movement.formatted == names.OBJECT_MOVEMENTS[calc.DIRECT]
+
+    # DignityState
+    assert sun.dignities.ruler == False
+    assert sun.dignities.exalted == False
+    assert sun.dignities.triplicity_ruler == False
+    assert sun.dignities.term_ruler == False
+    assert sun.dignities.face_ruler == False
+    assert sun.dignities.mutual_reception_ruler == False
+    assert sun.dignities.mutual_reception_exalted == False
+    assert sun.dignities.mutual_reception_triplicity_ruler == True
+    assert sun.dignities.mutual_reception_term_ruler == False
+    assert sun.dignities.mutual_reception_face_ruler == False
+    assert sun.dignities.detriment == False
+    assert sun.dignities.fall == False
+    assert sun.dignities.peregrine == False
+    assert sun.dignities.formatted == [
+        names.DIGNITIES[dignities.MUTUAL_RECEPTION_TRIPLICITY_RULER],
+    ]
+
+    # EclipseType
+    eclipse = natal_chart.objects[chart.PRE_NATAL_LUNAR_ECLIPSE]
+    assert eclipse.eclipse_type.total == False
+    assert eclipse.eclipse_type.annular == False
+    assert eclipse.eclipse_type.partial == True
+    assert eclipse.eclipse_type.annular_total == False
+    assert eclipse.eclipse_type.penumbral == False
+    assert eclipse.eclipse_type.formatted == names.ECLIPSE_TYPES[chart.PARTIAL]
+
+    assert type(eclipse.date_time) is wrap.DateTime         # Tested separately, just ensure type
+
+    # Subject
+    subject = natal_chart.native
+    assert type(subject.date_time) is wrap.DateTime         # Tested separately, just ensure type
+    assert type(subject.coordinates) is wrap.Coordinates    # Tested separately, just ensure type
+
+    # Weightings
+    weightings = natal_chart.weightings
+    assert type(weightings.elements) is wrap.Elements       # Tested separately, just ensure type
+    assert type(weightings.modalities) is wrap.Modalities   # Tested separately, just ensure type
+    assert type(weightings.quadrants) is wrap.Quadrants     # Tested separately, just ensure type
+
+    # Elements
+    elements = natal_chart.weightings.elements
+    assert type(elements.fire) is list
+    assert type(elements.earth) is list
+    assert type(elements.air) is list
+    assert type(elements.water) is list
+
+    # Modalities
+    modalities = natal_chart.weightings.modalities
+    assert type(modalities.cardinal) is list
+    assert type(modalities.fixed) is list
+    assert type(modalities.mutable) is list
+
+    # Quadrants
+    quadrants = natal_chart.weightings.quadrants
+    assert type(quadrants.first) is list
+    assert type(quadrants.second) is list
+    assert type(quadrants.third) is list
+    assert type(quadrants.fourth) is list
+
+
 def test_natal(native, lat, lon):
     natal_chart = charts.Natal(native)
 
     assert natal_chart.type == names.CHART_TYPES[chart.NATAL]
 
     assert round(natal_chart.native.date_time.julian + natal_chart.native.date_time.deltat, 6) == 2451545.250739
     assert natal_chart.native.date_time.timezone == 'PST'
@@ -116,17 +278,17 @@
     assert natal_chart.objects[chart.SUN].sign.name == names.SIGNS[chart.CAPRICORN]
     assert natal_chart.objects[chart.SUN].sign_longitude.formatted == '10°37\'26"'
 
     assert natal_chart.objects[chart.MOON].name == names.PLANETS[chart.MOON]
     assert natal_chart.objects[chart.MOON].sign.name == names.SIGNS[chart.SCORPIO]
     assert natal_chart.objects[chart.MOON].sign_longitude.formatted == '16°19\'29"'
 
-    assert natal_chart.objects[chart.PARS_FORTUNA].name == names.POINTS[chart.PARS_FORTUNA]
-    assert natal_chart.objects[chart.PARS_FORTUNA].sign.name == names.SIGNS[chart.CAPRICORN]
-    assert natal_chart.objects[chart.PARS_FORTUNA].sign_longitude.formatted == '11°18\'41"'
+    assert natal_chart.objects[chart.PART_OF_FORTUNE].name == names.POINTS[chart.PART_OF_FORTUNE]
+    assert natal_chart.objects[chart.PART_OF_FORTUNE].sign.name == names.SIGNS[chart.CAPRICORN]
+    assert natal_chart.objects[chart.PART_OF_FORTUNE].sign_longitude.formatted == '11°18\'41"'
 
     # Spot-check for correct object data against astro.com & Astro Gold
     assert natal_chart.objects[chart.SATURN].movement.retrograde is True
     assert natal_chart.objects[chart.MARS].dignities.peregrine is True
     assert natal_chart.objects[chart.MARS].score == -5
 
     # Spot-check for correct angle positions against astro.com
@@ -182,17 +344,17 @@
     assert solar_return_chart.objects[chart.SUN].sign.name == names.SIGNS[chart.CAPRICORN]
     assert solar_return_chart.objects[chart.SUN].sign_longitude.formatted == '10°37\'26"'
 
     assert solar_return_chart.objects[chart.MOON].name == names.PLANETS[chart.MOON]
     assert solar_return_chart.objects[chart.MOON].sign.name == names.SIGNS[chart.SCORPIO]
     assert solar_return_chart.objects[chart.MOON].sign_longitude.formatted == '28°43\'43"'
 
-    assert solar_return_chart.objects[chart.PARS_FORTUNA].name == names.POINTS[chart.PARS_FORTUNA]
-    assert solar_return_chart.objects[chart.PARS_FORTUNA].sign.name == names.SIGNS[chart.TAURUS]
-    assert solar_return_chart.objects[chart.PARS_FORTUNA].sign_longitude.formatted == '24°41\'28"'
+    assert solar_return_chart.objects[chart.PART_OF_FORTUNE].name == names.POINTS[chart.PART_OF_FORTUNE]
+    assert solar_return_chart.objects[chart.PART_OF_FORTUNE].sign.name == names.SIGNS[chart.TAURUS]
+    assert solar_return_chart.objects[chart.PART_OF_FORTUNE].sign_longitude.formatted == '24°41\'28"'
 
     # Spot-check for correct object data against astro.com & Astro Gold
     assert solar_return_chart.objects[chart.SATURN].movement.retrograde is True
     assert solar_return_chart.objects[chart.MARS].dignities.peregrine is True
     assert solar_return_chart.objects[chart.MARS].score == -5
 
     # Spot-check for correct angle positions against astro.com
@@ -256,17 +418,17 @@
     assert progressed_chart.objects[chart.SUN].sign.name == names.SIGNS[chart.AQUARIUS]
     assert progressed_chart.objects[chart.SUN].sign_longitude.formatted == '06°33\'41"'
 
     assert progressed_chart.objects[chart.MOON].name == names.PLANETS[chart.MOON]
     assert progressed_chart.objects[chart.MOON].sign.name == names.SIGNS[chart.LIBRA]
     assert progressed_chart.objects[chart.MOON].sign_longitude.formatted == '23°50\'57"'
 
-    assert progressed_chart.objects[chart.PARS_FORTUNA].name == names.POINTS[chart.PARS_FORTUNA]
-    assert progressed_chart.objects[chart.PARS_FORTUNA].sign.name == names.SIGNS[chart.CAPRICORN]
-    assert progressed_chart.objects[chart.PARS_FORTUNA].sign_longitude.formatted == '00°17\'45"'
+    assert progressed_chart.objects[chart.PART_OF_FORTUNE].name == names.POINTS[chart.PART_OF_FORTUNE]
+    assert progressed_chart.objects[chart.PART_OF_FORTUNE].sign.name == names.SIGNS[chart.CAPRICORN]
+    assert progressed_chart.objects[chart.PART_OF_FORTUNE].sign_longitude.formatted == '00°17\'45"'
 
     # Spot-check for correct object data against Astro Gold
     assert progressed_chart.objects[chart.SUN].dignities.detriment is True
     assert progressed_chart.objects[chart.SUN].dignities.peregrine is True
     assert progressed_chart.objects[chart.SUN].score == -10
 
     # Spot-check for correct angle positions against astro.com
@@ -328,17 +490,17 @@
     assert composite_chart.objects[chart.SUN].sign.name == names.SIGNS[chart.AQUARIUS]
     assert composite_chart.objects[chart.SUN].sign_longitude.formatted == '04°17\'35"'
 
     assert composite_chart.objects[chart.MOON].name == names.PLANETS[chart.MOON]
     assert composite_chart.objects[chart.MOON].sign.name == names.SIGNS[chart.SAGITTARIUS]
     assert composite_chart.objects[chart.MOON].sign_longitude.formatted == '00°22\'35"'
 
-    assert composite_chart.objects[chart.PARS_FORTUNA].name == names.POINTS[chart.PARS_FORTUNA]
-    assert composite_chart.objects[chart.PARS_FORTUNA].sign.name == names.SIGNS[chart.PISCES]
-    assert composite_chart.objects[chart.PARS_FORTUNA].sign_longitude.formatted == '01°03\'58"'
+    assert composite_chart.objects[chart.PART_OF_FORTUNE].name == names.POINTS[chart.PART_OF_FORTUNE]
+    assert composite_chart.objects[chart.PART_OF_FORTUNE].sign.name == names.SIGNS[chart.PISCES]
+    assert composite_chart.objects[chart.PART_OF_FORTUNE].sign_longitude.formatted == '01°03\'58"'
 
     # Spot-check for correct object data against Astro Gold
     assert composite_chart.objects[chart.SUN].dignities.detriment is True
     assert composite_chart.objects[chart.SUN].dignities.peregrine is True
     assert composite_chart.objects[chart.SUN].score == -10
 
     # Spot-check for correct angle positions against astro.com
```

### Comparing `immanuel-1.3.3/tests/test_convert.py` & `immanuel-1.4.0/tests/test_convert.py`

 * *Files identical despite different names*

### Comparing `immanuel-1.3.3/tests/test_date.py` & `immanuel-1.4.0/tests/test_date.py`

 * *Files identical despite different names*

### Comparing `immanuel-1.3.3/tests/test_dignity.py` & `immanuel-1.4.0/tests/test_dignity.py`

 * *Files identical despite different names*

### Comparing `immanuel-1.3.3/tests/test_ephemeris.py` & `immanuel-1.4.0/tests/test_ephemeris.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,16 +66,17 @@
         chart.NORTH_NODE,
         chart.SOUTH_NODE,
         chart.TRUE_NORTH_NODE,
         chart.TRUE_SOUTH_NODE,
         chart.VERTEX,
         chart.LILITH,
         chart.TRUE_LILITH,
+        chart.INTERPOLATED_LILITH,
         chart.SYZYGY,
-        chart.PARS_FORTUNA,
+        chart.PART_OF_FORTUNE,
     )
 
 @fixture
 def all_planets():
     return (
         chart.SUN,
         chart.MOON,
@@ -187,43 +188,43 @@
 def teardown_function():
     settings.reset()
 
 
 """ These tests simply check the correct chart objects are being
 returned. Data is checked separately afterwards. """
 def test_objects(jd, coords):
-    chart_objects = (chart.SUN, chart.MOON, chart.PARS_FORTUNA, chart.SYZYGY, chart.NORTH_NODE, chart.ASC)
+    chart_objects = (chart.SUN, chart.MOON, chart.PART_OF_FORTUNE, chart.SYZYGY, chart.NORTH_NODE, chart.ASC)
     objects = ephemeris.objects(chart_objects, jd, *coords, chart.PLACIDUS, calc.DAY_NIGHT_FORMULA)
     assert tuple(objects.keys()) == chart_objects
 
 
 def test_armc_objects(jd, coords, armc):
-    chart_objects = (chart.SUN, chart.MOON, chart.PARS_FORTUNA, chart.SYZYGY, chart.NORTH_NODE, chart.ASC)
+    chart_objects = (chart.SUN, chart.MOON, chart.PART_OF_FORTUNE, chart.SYZYGY, chart.NORTH_NODE, chart.ASC)
     objects = ephemeris.armc_objects(chart_objects, jd, armc, *coords, None, chart.PLACIDUS, calc.DAY_NIGHT_FORMULA)
     assert tuple(objects.keys()) == chart_objects
 
 
 def test_get(jd, coords):
     settings.add_filepath(os.path.dirname(__file__))
     assert ephemeris.get(chart.ASC, jd, *coords, chart.PLACIDUS)['index'] == chart.ASC
     assert ephemeris.get(chart.HOUSE2, jd, *coords, chart.PLACIDUS)['index'] == chart.HOUSE2
     assert ephemeris.get(chart.SUN, jd)['index'] == chart.SUN
-    assert ephemeris.get(chart.PARS_FORTUNA, jd, *coords, pars_fortuna_formula=calc.DAY_NIGHT_FORMULA)['index'] == chart.PARS_FORTUNA
+    assert ephemeris.get(chart.PART_OF_FORTUNE, jd, *coords, part_formula=calc.DAY_NIGHT_FORMULA)['index'] == chart.PART_OF_FORTUNE
     assert ephemeris.get(chart.JUNO, jd)['index'] == chart.JUNO   # Included with planets
     lilith = ephemeris.get(1181, jd)                              # From external file
     antares = ephemeris.get('Antares', jd)
     assert lilith['index'] == 1181 and lilith['type'] == chart.ASTEROID
     assert antares['index'] == 'Antares' and antares['type'] == chart.FIXED_STAR
 
 
 def test_armc_get(jd, coords, armc):
     settings.add_filepath(os.path.dirname(__file__))
     assert ephemeris.armc_get(chart.ASC, jd, armc, coords[0], house_system=chart.PLACIDUS)['index'] == chart.ASC
     assert ephemeris.armc_get(chart.HOUSE2, jd, armc, coords[0], house_system=chart.PLACIDUS)['index'] == chart.HOUSE2
-    assert ephemeris.armc_get(chart.PARS_FORTUNA, jd, armc, coords[0], pars_fortuna_formula=calc.DAY_NIGHT_FORMULA)['index'] == chart.PARS_FORTUNA
+    assert ephemeris.armc_get(chart.PART_OF_FORTUNE, jd, armc, coords[0], part_formula=calc.DAY_NIGHT_FORMULA)['index'] == chart.PART_OF_FORTUNE
 
 
 def test_get_angles(jd, coords, all_angles):
     angles = ephemeris.get(chart.ANGLE, jd, *coords, chart.PLACIDUS)
     assert sorted(all_angles) == sorted(angles)
 
 
@@ -353,15 +354,15 @@
 def test_get_data(coords, jd, astro):
     settings.add_filepath(os.path.dirname(__file__))
 
     data = {
         'asc': ephemeris.angle(chart.ASC, jd, *coords, chart.PLACIDUS),
         'house_2': ephemeris.house(chart.HOUSE2, jd, *coords, chart.PLACIDUS),
         'sun': ephemeris.planet(chart.SUN, jd),
-        'pof': ephemeris.point(chart.PARS_FORTUNA, jd, *coords, pars_fortuna_formula=calc.DAY_NIGHT_FORMULA),
+        'pof': ephemeris.point(chart.PART_OF_FORTUNE, jd, *coords, part_formula=calc.DAY_NIGHT_FORMULA),
         'juno': ephemeris.asteroid(chart.JUNO, jd),    # Included with planets
         'lilith': ephemeris.asteroid(1181, jd),        # From external file
         'antares': ephemeris.fixed_star('Antares', jd),
         'pre_natal_solar_eclipse': ephemeris.eclipse(chart.PRE_NATAL_SOLAR_ECLIPSE, jd),
         'pre_natal_lunar_eclipse': ephemeris.eclipse(chart.PRE_NATAL_LUNAR_ECLIPSE, jd),
         'post_natal_solar_eclipse': ephemeris.eclipse(chart.POST_NATAL_SOLAR_ECLIPSE, jd),
         'post_natal_lunar_eclipse': ephemeris.eclipse(chart.POST_NATAL_LUNAR_ECLIPSE, jd),
@@ -389,15 +390,15 @@
     settings.add_filepath(os.path.dirname(__file__))
 
     obliquity = ephemeris.obliquity(jd)
 
     data = {
         'asc': ephemeris.armc_angle(chart.ASC, armc, coords[0], obliquity, chart.PLACIDUS),
         'house_2': ephemeris.armc_house(chart.HOUSE2, armc, coords[0], obliquity, chart.PLACIDUS),
-        'pof': ephemeris.armc_point(chart.PARS_FORTUNA, jd, armc, coords[0], obliquity, pars_fortuna_formula=calc.DAY_NIGHT_FORMULA),
+        'pof': ephemeris.armc_point(chart.PART_OF_FORTUNE, jd, armc, coords[0], obliquity, part_formula=calc.DAY_NIGHT_FORMULA),
     }
 
     for key, eph_object in data.items():
         # Convert ecliptic longitude to sign-based
         object = eph_object.copy()
         object['lon'] = position.sign_longitude(object)
```

### Comparing `immanuel-1.3.3/tests/test_find.py` & `immanuel-1.4.0/tests/test_find.py`

 * *Files identical despite different names*

### Comparing `immanuel-1.3.3/tests/test_forecast.py` & `immanuel-1.4.0/tests/test_forecast.py`

 * *Files identical despite different names*

### Comparing `immanuel-1.3.3/tests/test_localization.py` & `immanuel-1.4.0/tests/test_localization.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,15 +82,15 @@
         chart.SOUTH_NODE: 'Nodo Sul',
         chart.TRUE_NORTH_NODE: 'Nodo Norte Verdadeiro',
         chart.TRUE_SOUTH_NODE: 'Nodo Sul Verdadeiro',
         chart.VERTEX: 'Vertex',
         chart.LILITH: 'Lilith',
         chart.TRUE_LILITH: 'Lilith Verdadeira',
         chart.SYZYGY: 'Sizígia',
-        chart.PARS_FORTUNA: 'Roda da Fortuna',
+        chart.PART_OF_FORTUNE: 'Roda da Fortuna',
 
         chart.PRE_NATAL_LUNAR_ECLIPSE: 'Eclipse Lunar Pré-natal',
         chart.PRE_NATAL_SOLAR_ECLIPSE: 'Eclipse Solar Pré-natal',
         chart.POST_NATAL_LUNAR_ECLIPSE: 'Eclipse Lunar Pós-natal',
         chart.POST_NATAL_SOLAR_ECLIPSE: 'Eclipse Solar Pós-natal',
     }
 
@@ -342,46 +342,46 @@
 
 def test_properties_aspects(native, aspects):
     settings.locale = 'pt_BR'
     settings.aspects = aspects
 
     natal = charts.Natal(native)
 
-    assert natal.aspects[chart.SUN][chart.PARS_FORTUNA].type == 'Conjunção'
+    assert natal.aspects[chart.SUN][chart.PART_OF_FORTUNE].type == 'Conjunção'
     assert natal.aspects[chart.MOON][chart.SATURN].type == 'Oposição'
     assert natal.aspects[chart.MOON][chart.URANUS].type == 'Quadratura'
-    assert natal.aspects[chart.SATURN][chart.PARS_FORTUNA].type == 'Trígono'
+    assert natal.aspects[chart.SATURN][chart.PART_OF_FORTUNE].type == 'Trígono'
     assert natal.aspects[chart.MOON][chart.SUN].type == 'Sextil'
     assert natal.aspects[chart.NEPTUNE][chart.PLUTO].type == 'Septil'
     assert natal.aspects[chart.SUN][chart.MARS].type == 'Semi-quadratura'
     assert natal.aspects[chart.JUPITER][chart.PLUTO].type == 'Sesqui-quadratura'
-    assert natal.aspects[chart.PLUTO][chart.PARS_FORTUNA].type == 'Semi-sextil'
+    assert natal.aspects[chart.PLUTO][chart.PART_OF_FORTUNE].type == 'Semi-sextil'
     assert natal.aspects[chart.PLUTO][chart.SATURN].type == 'Quincúncio'
     assert natal.aspects[chart.VENUS][chart.URANUS].type == 'Quintil'
     assert natal.aspects[chart.VENUS][chart.JUPITER].type == 'Biquintil'
 
 
 def test_properties_aspect_movements(native, aspects):
     settings.locale = 'pt_BR'
     settings.aspects = aspects
 
     natal = charts.Natal(native)
 
-    assert natal.aspects[chart.SUN][chart.PARS_FORTUNA].movement.formatted == 'Aplicativa'
-    assert natal.aspects[chart.PLUTO][chart.PARS_FORTUNA].movement.formatted == 'Exacto'
+    assert natal.aspects[chart.SUN][chart.PART_OF_FORTUNE].movement.formatted == 'Aplicativa'
+    assert natal.aspects[chart.PLUTO][chart.PART_OF_FORTUNE].movement.formatted == 'Exacto'
     assert natal.aspects[chart.MOON][chart.SUN].movement.formatted == 'Separativo'
 
 
 def test_properties_aspect_conditions(native, aspects):
     settings.locale = 'pt_BR'
     settings.aspects = aspects
 
     natal = charts.Natal(native)
 
-    assert natal.aspects[chart.SUN][chart.PARS_FORTUNA].condition.formatted == 'Associada'
+    assert natal.aspects[chart.SUN][chart.PART_OF_FORTUNE].condition.formatted == 'Associada'
     assert natal.aspects[chart.MERCURY][chart.MARS].condition.formatted == 'Dissociado'
 
 
 def test_properties_dignities(native):
     settings.locale = 'pt_BR'
 
     natal = charts.Natal(native)
@@ -450,15 +450,15 @@
 
 def test_properties_object_movement(native):
     settings.locale = 'pt_BR'
 
     natal = charts.Natal(native)
 
     assert natal.objects[chart.SUN].movement.formatted == 'Direto'
-    assert natal.objects[chart.PARS_FORTUNA].movement.formatted == 'Estacionária'
+    assert natal.objects[chart.PART_OF_FORTUNE].movement.formatted == 'Estacionária'
     assert natal.objects[chart.SATURN].movement.formatted == 'Retrógrado'
 
 
 def test_properties_chart_shape(chart_pattern_birth_data):
     settings.locale = 'pt_BR'
 
     for data in chart_pattern_birth_data.values():
@@ -488,21 +488,21 @@
     natal = charts.Natal(ambiguous_native)
     assert str(natal.native.date_time) == 'Dom Nov 06 2022 01:30:00 PDT (ambíguo)'
 
 
 def test_formatted_aspect(native):
     settings.locale = 'pt_BR'
     natal = charts.Natal(native)
-    assert str(natal.aspects[chart.SUN][chart.PARS_FORTUNA]) == 'Conjunção entre Sol e Roda da Fortuna dentro de 00°41\'15" (Aplicativa, Associada)'
+    assert str(natal.aspects[chart.SUN][chart.PART_OF_FORTUNE]) == 'Conjunção entre Sol e Roda da Fortuna dentro de 00°41\'15" (Aplicativa, Associada)'
 
 
 def test_formatted_object(native):
     settings.locale = 'pt_BR'
     natal = charts.Natal(native)
-    assert str(natal.objects[chart.SUN]) == 'Sol 10°37\'26" em Capricórnio, Casa 11, Direto'
+    assert str(natal.objects[chart.SUN]) == 'Sol 10°37\'26" em Capricórnio, Casa 11'
     assert str(natal.objects[chart.ASC]) == 'Ascendente 05°36\'38" em Peixes, Casa 1'
     assert str(natal.houses[chart.HOUSE2]) == 'Casa 2 17°59\'40" em Áries'
 
 
 def test_formatted_subject(native):
     settings.locale = 'pt_BR'
     natal = charts.Natal(native)
```

### Comparing `immanuel-1.3.3/tests/test_midpoint.py` & `immanuel-1.4.0/tests/test_midpoint.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,15 +114,15 @@
         chart.TRUE_NORTH_NODE: {
             'sign': chart.TAURUS,
             'lon': '28°04\'05"',
             'lat': '00°00\'00"',
             'speed': '-00°03\'45"',
             'dec': '19°43\'43"',
         },
-        chart.PARS_FORTUNA: {
+        chart.PART_OF_FORTUNE: {
             'sign': chart.PISCES,
             'lon': '09°54\'57"',
             'lat': '00°00\'00"',
             'speed': '00°00\'00"',
             'dec': '-07°51\'02"',
         },
     }
```

### Comparing `immanuel-1.3.3/tests/test_pattern.py` & `immanuel-1.4.0/tests/test_pattern.py`

 * *Files identical despite different names*

### Comparing `immanuel-1.3.3/tests/test_position.py` & `immanuel-1.4.0/tests/test_position.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 def data(jd, coords):
     settings.add_filepath(os.path.dirname(__file__))
 
     return {
         'asc': ephemeris.angle(chart.ASC, jd, *coords, chart.PLACIDUS),
         'house_2': ephemeris.house(chart.HOUSE2, jd, *coords, chart.PLACIDUS),
         'sun': ephemeris.planet(chart.SUN, jd),
-        'pof': ephemeris.point(chart.PARS_FORTUNA, jd, *coords, chart.PLACIDUS, calc.DAY_NIGHT_FORMULA),
+        'pof': ephemeris.point(chart.PART_OF_FORTUNE, jd, *coords, chart.PLACIDUS, calc.DAY_NIGHT_FORMULA),
         'juno': ephemeris.asteroid(chart.JUNO, jd),       # Included with planets
         'lilith': ephemeris.asteroid(1181, jd),           # From its own file
         'antares': ephemeris.fixed_star('Antares', jd),
     }
 
 @fixture
 def astro():
```

### Comparing `immanuel-1.3.3/tests/test_setup.py` & `immanuel-1.4.0/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `immanuel-1.3.3/tests/test_weighting.py` & `immanuel-1.4.0/tests/test_weighting.py`

 * *Files identical despite different names*

