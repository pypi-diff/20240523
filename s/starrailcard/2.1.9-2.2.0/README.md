# Comparing `tmp/starrailcard-2.1.9.tar.gz` & `tmp/starrailcard-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starrailcard-2.1.9.tar", last modified: Fri May 17 21:35:53 2024, max compression
+gzip compressed data, was "starrailcard-2.2.0.tar", last modified: Wed May 22 22:14:46 2024, max compression
```

## Comparing `starrailcard-2.1.9.tar` & `starrailcard-2.2.0.tar`

### file list

```diff
@@ -1,81 +1,77 @@
-drwxrwxrwx   0        0        0        0 2024-05-17 21:35:53.837346 starrailcard-2.1.9/
--rw-rw-rw-   0        0        0     1721 2024-03-20 15:38:40.000000 starrailcard-2.1.9/LICENSE
--rw-rw-rw-   0        0        0       38 2024-04-29 22:20:14.000000 starrailcard-2.1.9/MANIFEST.in
--rw-rw-rw-   0        0        0     4762 2024-05-17 21:35:53.836347 starrailcard-2.1.9/PKG-INFO
--rw-rw-rw-   0        0        0     3642 2024-03-18 20:36:48.000000 starrailcard-2.1.9/README.md
--rw-rw-rw-   0        0        0     1106 2024-04-18 21:49:53.000000 starrailcard-2.1.9/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-17 21:35:53.837346 starrailcard-2.1.9/setup.cfg
--rw-rw-rw-   0        0        0     1571 2024-05-11 16:52:16.000000 starrailcard-2.1.9/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-17 21:35:53.613661 starrailcard-2.1.9/starrailcard/
--rw-rw-rw-   0        0        0     1967 2024-05-17 21:35:04.000000 starrailcard-2.1.9/starrailcard/__init__.py
--rw-rw-rw-   0        0        0    13231 2024-05-17 19:34:28.000000 starrailcard-2.1.9/starrailcard/client.py
-drwxrwxrwx   0        0        0        0 2024-05-17 21:35:53.598151 starrailcard-2.1.9/starrailcard/src/
-drwxrwxrwx   0        0        0        0 2024-05-17 21:35:53.644660 starrailcard-2.1.9/starrailcard/src/api/
--rw-rw-rw-   0        0        0     3721 2024-05-16 22:45:16.000000 starrailcard-2.1.9/starrailcard/src/api/api.py
--rw-rw-rw-   0        0        0     2995 2024-05-17 20:03:31.000000 starrailcard-2.1.9/starrailcard/src/api/enka.py
--rw-rw-rw-   0        0        0    26807 2024-05-16 23:12:27.000000 starrailcard-2.1.9/starrailcard/src/api/enka_parsed.py
--rw-rw-rw-   0        0        0      487 2024-04-09 16:19:13.000000 starrailcard-2.1.9/starrailcard/src/api/error.py
-drwxrwxrwx   0        0        0        0 2024-05-17 21:35:53.597151 starrailcard-2.1.9/starrailcard/src/assets/
-drwxrwxrwx   0        0        0        0 2024-05-17 21:35:53.648661 starrailcard-2.1.9/starrailcard/src/assets/font/
--rw-rw-rw-   0        0        0   201292 2023-10-12 08:13:59.000000 starrailcard-2.1.9/starrailcard/src/assets/font/font_hsr.ttf
-drwxrwxrwx   0        0        0        0 2024-05-17 21:35:53.671661 starrailcard-2.1.9/starrailcard/src/data/
--rw-rw-rw-   0        0        0     1751 2024-03-28 18:26:38.000000 starrailcard-2.1.9/starrailcard/src/data/avatar.json
--rw-rw-rw-   0        0        0      252 2024-03-28 18:26:38.000000 starrailcard-2.1.9/starrailcard/src/data/element.json
--rw-rw-rw-   0        0        0       70 2024-03-28 18:26:38.000000 starrailcard-2.1.9/starrailcard/src/data/keys.json
--rw-rw-rw-   0        0        0      293 2024-03-28 18:26:38.000000 starrailcard-2.1.9/starrailcard/src/data/paths.json
--rw-rw-rw-   0        0        0     1915 2024-03-28 18:26:38.000000 starrailcard-2.1.9/starrailcard/src/data/relict_sets.json
--rw-rw-rw-   0        0        0     4947 2024-03-28 18:26:38.000000 starrailcard-2.1.9/starrailcard/src/data/stats.json
--rw-rw-rw-   0        0        0     4738 2024-03-28 18:26:38.000000 starrailcard-2.1.9/starrailcard/src/data/weapons.json
-drwxrwxrwx   0        0        0        0 2024-05-17 21:35:53.691664 starrailcard-2.1.9/starrailcard/src/generator/
--rw-rw-rw-   0        0        0    26099 2024-05-17 19:35:40.000000 starrailcard-2.1.9/starrailcard/src/generator/style_card.py
--rw-rw-rw-   0        0        0     6675 2024-05-17 19:35:00.000000 starrailcard-2.1.9/starrailcard/src/generator/style_profile_phone.py
--rw-rw-rw-   0        0        0    24905 2024-05-17 19:39:00.000000 starrailcard-2.1.9/starrailcard/src/generator/style_relict_score.py
--rw-rw-rw-   0        0        0    30869 2024-05-17 19:59:09.000000 starrailcard-2.1.9/starrailcard/src/generator/style_ticket.py
-drwxrwxrwx   0        0        0        0 2024-05-17 21:35:53.714172 starrailcard-2.1.9/starrailcard/src/model/
--rw-rw-rw-   0        0        0     4208 2024-05-10 18:23:13.000000 starrailcard-2.1.9/starrailcard/src/model/StarRailCard.py
-drwxrwxrwx   0        0        0        0 2024-05-17 21:35:53.719171 starrailcard-2.1.9/starrailcard/src/model/__pycache__/
--rw-rw-rw-   0        0        0     7142 2024-05-12 06:48:27.000000 starrailcard-2.1.9/starrailcard/src/model/__pycache__/StarRailCard.cpython-312.pyc
--rw-rw-rw-   0        0        0    19407 2024-05-12 08:45:20.000000 starrailcard-2.1.9/starrailcard/src/model/__pycache__/api_mihomo.cpython-312.pyc
--rw-rw-rw-   0        0        0     6999 2024-05-12 06:48:26.000000 starrailcard-2.1.9/starrailcard/src/model/__pycache__/style.cpython-312.pyc
--rw-rw-rw-   0        0        0      975 2024-05-12 06:48:25.000000 starrailcard-2.1.9/starrailcard/src/model/__pycache__/ukrainization_model.cpython-312.pyc
--rw-rw-rw-   0        0        0     1609 2024-05-12 06:48:30.000000 starrailcard-2.1.9/starrailcard/src/model/__pycache__/utils_model.cpython-312.pyc
--rw-rw-rw-   0        0        0    12705 2024-05-12 08:45:15.000000 starrailcard-2.1.9/starrailcard/src/model/api_mihomo.py
--rw-rw-rw-   0        0        0     8565 2024-05-10 22:49:33.000000 starrailcard-2.1.9/starrailcard/src/model/style.py
--rw-rw-rw-   0        0        0      493 2024-03-13 13:48:02.000000 starrailcard-2.1.9/starrailcard/src/model/ukrainization_model.py
--rw-rw-rw-   0        0        0      845 2024-03-13 13:48:07.000000 starrailcard-2.1.9/starrailcard/src/model/utils_model.py
-drwxrwxrwx   0        0        0        0 2024-05-17 21:35:53.766172 starrailcard-2.1.9/starrailcard/src/tools/
--rw-rw-rw-   0        0        0     2526 2024-02-22 12:56:12.000000 starrailcard-2.1.9/starrailcard/src/tools/cache.py
-drwxrwxrwx   0        0        0        0 2024-05-17 21:35:53.771173 starrailcard-2.1.9/starrailcard/src/tools/calculator/
-drwxrwxrwx   0        0        0        0 2024-05-17 21:35:53.775171 starrailcard-2.1.9/starrailcard/src/tools/calculator/src/
-drwxrwxrwx   0        0        0        0 2024-05-17 21:35:53.792183 starrailcard-2.1.9/starrailcard/src/tools/calculator/src/assets/
--rw-rw-rw-   0        0        0      373 2024-04-06 18:51:59.000000 starrailcard-2.1.9/starrailcard/src/tools/calculator/src/assets/max.json
--rw-rw-rw-   0        0        0       49 2024-04-06 18:52:00.000000 starrailcard-2.1.9/starrailcard/src/tools/calculator/src/assets/relic_id.json
--rw-rw-rw-   0        0        0     3434 2024-04-06 18:52:00.000000 starrailcard-2.1.9/starrailcard/src/tools/calculator/src/assets/rolls.json
--rw-rw-rw-   0        0        0    92881 2024-04-06 18:52:01.000000 starrailcard-2.1.9/starrailcard/src/tools/calculator/src/assets/score.json
--rw-rw-rw-   0        0        0     1959 2024-03-13 13:47:21.000000 starrailcard-2.1.9/starrailcard/src/tools/calculator/src/utils.py
--rw-rw-rw-   0        0        0     5802 2024-05-03 21:15:03.000000 starrailcard-2.1.9/starrailcard/src/tools/calculator/stats.py
--rw-rw-rw-   0        0        0      709 2024-04-09 17:29:46.000000 starrailcard-2.1.9/starrailcard/src/tools/enums.py
--rw-rw-rw-   0        0        0    12292 2024-05-10 21:23:50.000000 starrailcard-2.1.9/starrailcard/src/tools/git.py
--rw-rw-rw-   0        0        0     9968 2024-04-29 22:09:02.000000 starrailcard-2.1.9/starrailcard/src/tools/http.py
--rw-rw-rw-   0        0        0      938 2024-04-09 16:56:51.000000 starrailcard-2.1.9/starrailcard/src/tools/json_data.py
--rw-rw-rw-   0        0        0     8371 2024-05-17 19:30:07.000000 starrailcard-2.1.9/starrailcard/src/tools/options.py
-drwxrwxrwx   0        0        0        0 2024-05-17 21:35:53.835346 starrailcard-2.1.9/starrailcard/src/tools/pill/
--rw-rw-rw-   0        0        0      220 2024-05-10 22:00:17.000000 starrailcard-2.1.9/starrailcard/src/tools/pill/__init__.py
--rw-rw-rw-   0        0        0     3851 2024-05-10 22:00:17.000000 starrailcard-2.1.9/starrailcard/src/tools/pill/color.py
--rw-rw-rw-   0        0        0     2328 2024-05-10 22:00:17.000000 starrailcard-2.1.9/starrailcard/src/tools/pill/color_control.py
--rw-rw-rw-   0        0        0     5277 2024-05-10 21:27:12.000000 starrailcard-2.1.9/starrailcard/src/tools/pill/diagrama.py
--rw-rw-rw-   0        0        0     5517 2024-05-10 21:26:51.000000 starrailcard-2.1.9/starrailcard/src/tools/pill/gradient_v2.py
--rw-rw-rw-   0        0        0     3279 2024-05-10 22:00:17.000000 starrailcard-2.1.9/starrailcard/src/tools/pill/grandient_v1.py
--rw-rw-rw-   0        0        0     5481 2024-05-12 09:44:45.000000 starrailcard-2.1.9/starrailcard/src/tools/pill/image_control.py
--rw-rw-rw-   0        0        0     5717 2024-05-16 23:08:35.000000 starrailcard-2.1.9/starrailcard/src/tools/pill/style_editor.py
--rw-rw-rw-   0        0        0     2116 2024-05-10 22:00:17.000000 starrailcard-2.1.9/starrailcard/src/tools/pill/text_control.py
--rw-rw-rw-   0        0        0     2360 2024-03-13 13:31:40.000000 starrailcard-2.1.9/starrailcard/src/tools/translator.py
--rw-rw-rw-   0        0        0     8286 2024-05-09 19:05:04.000000 starrailcard-2.1.9/starrailcard/src/tools/treePaths.py
--rw-rw-rw-   0        0        0     1748 2024-03-28 18:26:54.000000 starrailcard-2.1.9/starrailcard/src/tools/ukrainization.py
--rw-rw-rw-   0        0        0     6884 2024-05-10 22:00:17.000000 starrailcard-2.1.9/starrailcard/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-17 21:35:53.835346 starrailcard-2.1.9/starrailcard.egg-info/
--rw-rw-rw-   0        0        0     4762 2024-05-17 21:35:53.000000 starrailcard-2.1.9/starrailcard.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2405 2024-05-17 21:35:53.000000 starrailcard-2.1.9/starrailcard.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 21:35:53.000000 starrailcard-2.1.9/starrailcard.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      102 2024-05-17 21:35:53.000000 starrailcard-2.1.9/starrailcard.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-17 21:35:53.000000 starrailcard-2.1.9/starrailcard.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-22 22:14:46.132206 starrailcard-2.2.0/
+-rw-rw-rw-   0        0        0     1721 2024-03-20 15:38:40.000000 starrailcard-2.2.0/LICENSE
+-rw-rw-rw-   0        0        0       38 2024-04-29 22:20:14.000000 starrailcard-2.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     4762 2024-05-22 22:14:46.131207 starrailcard-2.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3642 2024-03-18 20:36:48.000000 starrailcard-2.2.0/README.md
+-rw-rw-rw-   0        0        0     1106 2024-04-18 21:49:53.000000 starrailcard-2.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-22 22:14:46.132206 starrailcard-2.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1571 2024-05-11 16:52:16.000000 starrailcard-2.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 22:14:46.038205 starrailcard-2.2.0/starrailcard/
+-rw-rw-rw-   0        0        0     1967 2024-05-22 22:14:43.000000 starrailcard-2.2.0/starrailcard/__init__.py
+-rw-rw-rw-   0        0        0    25256 2024-05-20 11:59:09.000000 starrailcard-2.2.0/starrailcard/client.py
+drwxrwxrwx   0        0        0        0 2024-05-22 22:14:46.028698 starrailcard-2.2.0/starrailcard/src/
+drwxrwxrwx   0        0        0        0 2024-05-22 22:14:46.063660 starrailcard-2.2.0/starrailcard/src/api/
+-rw-rw-rw-   0        0        0     3740 2024-05-19 22:23:39.000000 starrailcard-2.2.0/starrailcard/src/api/api.py
+-rw-rw-rw-   0        0        0     5892 2024-05-20 10:36:13.000000 starrailcard-2.2.0/starrailcard/src/api/enka.py
+-rw-rw-rw-   0        0        0    27773 2024-05-20 10:45:25.000000 starrailcard-2.2.0/starrailcard/src/api/enka_parsed.py
+-rw-rw-rw-   0        0        0      487 2024-04-09 16:19:13.000000 starrailcard-2.2.0/starrailcard/src/api/error.py
+-rw-rw-rw-   0        0        0     2271 2024-05-20 08:43:12.000000 starrailcard-2.2.0/starrailcard/src/api/hoyolab.py
+-rw-rw-rw-   0        0        0    28814 2024-05-20 09:23:13.000000 starrailcard-2.2.0/starrailcard/src/api/hoyolab_parsed.py
+drwxrwxrwx   0        0        0        0 2024-05-22 22:14:46.028698 starrailcard-2.2.0/starrailcard/src/assets/
+drwxrwxrwx   0        0        0        0 2024-05-22 22:14:46.068163 starrailcard-2.2.0/starrailcard/src/assets/font/
+-rw-rw-rw-   0        0        0   201292 2023-10-12 08:13:59.000000 starrailcard-2.2.0/starrailcard/src/assets/font/font_hsr.ttf
+drwxrwxrwx   0        0        0        0 2024-05-22 22:14:46.091716 starrailcard-2.2.0/starrailcard/src/data/
+-rw-rw-rw-   0        0        0     1751 2024-03-28 18:26:38.000000 starrailcard-2.2.0/starrailcard/src/data/avatar.json
+-rw-rw-rw-   0        0        0      252 2024-03-28 18:26:38.000000 starrailcard-2.2.0/starrailcard/src/data/element.json
+-rw-rw-rw-   0        0        0       70 2024-03-28 18:26:38.000000 starrailcard-2.2.0/starrailcard/src/data/keys.json
+-rw-rw-rw-   0        0        0      293 2024-03-28 18:26:38.000000 starrailcard-2.2.0/starrailcard/src/data/paths.json
+-rw-rw-rw-   0        0        0     1915 2024-03-28 18:26:38.000000 starrailcard-2.2.0/starrailcard/src/data/relict_sets.json
+-rw-rw-rw-   0        0        0     4947 2024-03-28 18:26:38.000000 starrailcard-2.2.0/starrailcard/src/data/stats.json
+-rw-rw-rw-   0        0        0     4738 2024-03-28 18:26:38.000000 starrailcard-2.2.0/starrailcard/src/data/weapons.json
+drwxrwxrwx   0        0        0        0 2024-05-22 22:14:46.094717 starrailcard-2.2.0/starrailcard/src/generator/
+-rw-rw-rw-   0        0        0    26195 2024-05-20 11:30:55.000000 starrailcard-2.2.0/starrailcard/src/generator/style_card.py
+-rw-rw-rw-   0        0        0     6675 2024-05-17 19:35:00.000000 starrailcard-2.2.0/starrailcard/src/generator/style_profile_phone.py
+-rw-rw-rw-   0        0        0    24987 2024-05-20 11:28:47.000000 starrailcard-2.2.0/starrailcard/src/generator/style_relict_score.py
+-rw-rw-rw-   0        0        0    30954 2024-05-20 11:29:47.000000 starrailcard-2.2.0/starrailcard/src/generator/style_ticket.py
+drwxrwxrwx   0        0        0        0 2024-05-22 22:14:46.098223 starrailcard-2.2.0/starrailcard/src/model/
+-rw-rw-rw-   0        0        0     4352 2024-05-20 11:35:59.000000 starrailcard-2.2.0/starrailcard/src/model/StarRailCard.py
+-rw-rw-rw-   0        0        0    12740 2024-05-20 11:41:22.000000 starrailcard-2.2.0/starrailcard/src/model/api_mihomo.py
+-rw-rw-rw-   0        0        0     8565 2024-05-10 22:49:33.000000 starrailcard-2.2.0/starrailcard/src/model/style.py
+-rw-rw-rw-   0        0        0      493 2024-03-13 13:48:02.000000 starrailcard-2.2.0/starrailcard/src/model/ukrainization_model.py
+-rw-rw-rw-   0        0        0      845 2024-03-13 13:48:07.000000 starrailcard-2.2.0/starrailcard/src/model/utils_model.py
+drwxrwxrwx   0        0        0        0 2024-05-22 22:14:46.105222 starrailcard-2.2.0/starrailcard/src/tools/
+-rw-rw-rw-   0        0        0     2526 2024-02-22 12:56:12.000000 starrailcard-2.2.0/starrailcard/src/tools/cache.py
+drwxrwxrwx   0        0        0        0 2024-05-22 22:14:46.105222 starrailcard-2.2.0/starrailcard/src/tools/calculator/
+drwxrwxrwx   0        0        0        0 2024-05-22 22:14:46.106222 starrailcard-2.2.0/starrailcard/src/tools/calculator/src/
+drwxrwxrwx   0        0        0        0 2024-05-22 22:14:46.124700 starrailcard-2.2.0/starrailcard/src/tools/calculator/src/assets/
+-rw-rw-rw-   0        0        0      373 2024-05-19 22:33:34.000000 starrailcard-2.2.0/starrailcard/src/tools/calculator/src/assets/max.json
+-rw-rw-rw-   0        0        0       49 2024-05-19 22:33:34.000000 starrailcard-2.2.0/starrailcard/src/tools/calculator/src/assets/relic_id.json
+-rw-rw-rw-   0        0        0     3434 2024-05-19 22:33:34.000000 starrailcard-2.2.0/starrailcard/src/tools/calculator/src/assets/rolls.json
+-rw-rw-rw-   0        0        0   100343 2024-05-19 22:33:35.000000 starrailcard-2.2.0/starrailcard/src/tools/calculator/src/assets/score.json
+-rw-rw-rw-   0        0        0     1959 2024-03-13 13:47:21.000000 starrailcard-2.2.0/starrailcard/src/tools/calculator/src/utils.py
+-rw-rw-rw-   0        0        0     5912 2024-05-19 22:51:06.000000 starrailcard-2.2.0/starrailcard/src/tools/calculator/stats.py
+-rw-rw-rw-   0        0        0      709 2024-04-09 17:29:46.000000 starrailcard-2.2.0/starrailcard/src/tools/enums.py
+-rw-rw-rw-   0        0        0    12292 2024-05-10 21:23:50.000000 starrailcard-2.2.0/starrailcard/src/tools/git.py
+-rw-rw-rw-   0        0        0     9968 2024-04-29 22:09:02.000000 starrailcard-2.2.0/starrailcard/src/tools/http.py
+-rw-rw-rw-   0        0        0      938 2024-04-09 16:56:51.000000 starrailcard-2.2.0/starrailcard/src/tools/json_data.py
+-rw-rw-rw-   0        0        0     8371 2024-05-17 19:30:07.000000 starrailcard-2.2.0/starrailcard/src/tools/options.py
+drwxrwxrwx   0        0        0        0 2024-05-22 22:14:46.130206 starrailcard-2.2.0/starrailcard/src/tools/pill/
+-rw-rw-rw-   0        0        0      220 2024-05-10 22:00:17.000000 starrailcard-2.2.0/starrailcard/src/tools/pill/__init__.py
+-rw-rw-rw-   0        0        0     3851 2024-05-10 22:00:17.000000 starrailcard-2.2.0/starrailcard/src/tools/pill/color.py
+-rw-rw-rw-   0        0        0     2328 2024-05-10 22:00:17.000000 starrailcard-2.2.0/starrailcard/src/tools/pill/color_control.py
+-rw-rw-rw-   0        0        0     5277 2024-05-10 21:27:12.000000 starrailcard-2.2.0/starrailcard/src/tools/pill/diagrama.py
+-rw-rw-rw-   0        0        0     5517 2024-05-10 21:26:51.000000 starrailcard-2.2.0/starrailcard/src/tools/pill/gradient_v2.py
+-rw-rw-rw-   0        0        0     3279 2024-05-10 22:00:17.000000 starrailcard-2.2.0/starrailcard/src/tools/pill/grandient_v1.py
+-rw-rw-rw-   0        0        0     5481 2024-05-12 09:44:45.000000 starrailcard-2.2.0/starrailcard/src/tools/pill/image_control.py
+-rw-rw-rw-   0        0        0     5717 2024-05-16 23:08:35.000000 starrailcard-2.2.0/starrailcard/src/tools/pill/style_editor.py
+-rw-rw-rw-   0        0        0     2116 2024-05-10 22:00:17.000000 starrailcard-2.2.0/starrailcard/src/tools/pill/text_control.py
+-rw-rw-rw-   0        0        0     2360 2024-03-13 13:31:40.000000 starrailcard-2.2.0/starrailcard/src/tools/translator.py
+-rw-rw-rw-   0        0        0     8286 2024-05-09 19:05:04.000000 starrailcard-2.2.0/starrailcard/src/tools/treePaths.py
+-rw-rw-rw-   0        0        0     1748 2024-03-28 18:26:54.000000 starrailcard-2.2.0/starrailcard/src/tools/ukrainization.py
+-rw-rw-rw-   0        0        0     6884 2024-05-10 22:00:17.000000 starrailcard-2.2.0/starrailcard/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-22 22:14:46.130206 starrailcard-2.2.0/starrailcard.egg-info/
+-rw-rw-rw-   0        0        0     4762 2024-05-22 22:14:45.000000 starrailcard-2.2.0/starrailcard.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2159 2024-05-22 22:14:45.000000 starrailcard-2.2.0/starrailcard.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 22:14:45.000000 starrailcard-2.2.0/starrailcard.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      102 2024-05-22 22:14:45.000000 starrailcard-2.2.0/starrailcard.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-22 22:14:45.000000 starrailcard-2.2.0/starrailcard.egg-info/top_level.txt
```

### Comparing `starrailcard-2.1.9/LICENSE` & `starrailcard-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.9/PKG-INFO` & `starrailcard-2.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starrailcard
-Version: 2.1.9
+Version: 2.2.0
 Summary: This Python module provides the ability to create captivating character cards based on player data from Honkai Star Rail, obtained through their unique user identifiers (UIDs). StarRailCard streamlines the process of generating personalized character assembly cards, relying on the information provided by players.
 Home-page: https://github.com/DEViantUA/StarRailCard
 Author: DeviantUa
 Author-email: deviantapi@gmail.com
 Keywords: honkai,cards,generation,honkaistarraill,raill,starraill,builds,honkairail,honkai,genshin,build,api
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `starrailcard-2.1.9/README.md` & `starrailcard-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.9/pyproject.toml` & `starrailcard-2.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.9/setup.py` & `starrailcard-2.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.9/starrailcard/__init__.py` & `starrailcard-2.2.0/starrailcard/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
 __title__ = 'StarRailCard.py'
 __author__ = 'DeviantUa'
-__version__ = '2.1.9'
+__version__ = '2.2.0'
 __license__ = 'MIT'
 __copyright__ = 'Copyright 2024-present DeviantUa'
 
 from .client import *
 from .utils import *
 from .src.tools.enums import *
```

### Comparing `starrailcard-2.1.9/starrailcard/src/api/api.py` & `starrailcard-2.2.0/starrailcard/src/api/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,20 +23,16 @@
         self.proxy: str = proxy
         api_mihomo.UA_LANG = False
         if lang == "ua":
             self.ua_lang = True
             api_mihomo.UA_LANG = True
             
         self.v = v
-
-    async def recollect(self, data):
-        
-        pass
     
-    async def get(self) -> Optional[api_mihomo.MiHoMoApi]:
+    async def get(self, parse: bool = True) -> Optional[api_mihomo.MiHoMoApi]:
         """Get data from the MiHoMo API."""
         try:
             params = {
                 'lang': self.lang,
                 'is_force_update': str(self.force_update),
                 'version': f"v{self.v}"
             }
@@ -68,15 +64,18 @@
         if data["player"]["space_info"].get("book_count") is None:
             self.dop_info = await http.AioSession.get(_API_MIHOMO_NAKED.format(uid=self.uid), headers = headers, params=params, proxy= self.proxy)
             data = await self.add_info(data)
         
         if self.ua_lang:
             await ukrainization.TranslateDataManager().load_translate_data()
         
-        return api_mihomo.MiHoMoApi(player=data["player"], characters=data["characters"], dont_update_link= False)
+        if parse:
+            return api_mihomo.MiHoMoApi(player=data["player"], characters=data["characters"], dont_update_link= False)
+        else:
+            return data
     
     async def add_info(self, data):
         info = self.dop_info["detailInfo"]["recordInfo"]
         
         data["player"]["space_info"]["relicCount"] = info.get("relicCount", 0)
         data["player"]["space_info"]["musicCount"] = info.get("musicCount", 0)
         data["player"]["space_info"]["bookCount"] = info.get("bookCount", 0)
```

### Comparing `starrailcard-2.1.9/starrailcard/src/api/enka_parsed.py` & `starrailcard-2.2.0/starrailcard/src/api/enka_parsed.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import json
 import math
 from pathlib import Path
 from copy import deepcopy
 
 from ..tools.json_data import JsonManager
 from ..tools.enums import PathData
 
@@ -38,19 +37,39 @@
         self.relics_set = await JsonManager(PathData.ENKA_INDEX.value / self.lang / "relic_sets.json").read()
         self.relic_main_affixes = await JsonManager(PathData.ENKA_INDEX.value / self.lang / "relic_main_affixes.json").read()
         self.relic_sub_affixes = await JsonManager(PathData.ENKA_INDEX.value / self.lang / "relic_sub_affixes.json").read()
         self.relic_set = await JsonManager(PathData.ENKA_INDEX.value / self.lang / "relic_sets.json").read()
         self.light_cone_promotion = await JsonManager(PathData.ENKA_INDEX.value / self.lang / "light_cone_promotions.json").read()
         self.avatar = await JsonManager(PathData.ENKA_INDEX.value / self.lang / "avatars.json").read()
     
-    async def collect(self):
+    async def collect(self, build = False):
         await self.load_assets()
+        if build:
+            charters = []
+            for key in self.data["detailInfo"]["avatarDetailList"]:
+                for k in key:
+                    if isinstance(key[k], list):
+                        for data in key[k]:
+                            buildInfo = {
+                                "id": data.get("id", 0),
+                                "name_build": data.get("name", ""),
+                            }
+                            charters.append(await self.get_character(data["avatar_data"], buildInfo))
+                    else:
+                        buildInfo = {
+                                "id": key[k].get("id", 0),
+                                "name_build": key[k].get("name", ""),
+                            }
+                        charters.append(await self.get_character(key[k], buildInfo))
+        else:
+            charters = [await self.get_character(key) for key in self.data["detailInfo"]["avatarDetailList"]]
+            
         data = {
             "player": await self.get_player(),
-            "characters": [await self.get_character(key) for key in self.data["detailInfo"]["avatarDetailList"]]
+            "characters": charters
         }
         
         return data
     
     async def get_memory_data(self):
         data = self.data["detailInfo"]["recordInfo"]["challengeInfo"]
         return {
@@ -176,29 +195,29 @@
                     "value": v["base"] + v["step"] * (level - 1),
                     "display": await self.get_display(v["base"] + v["step"] * (level - 1), property["percent"]),
                     "percent": property["percent"],
                 }
             )
         return attributes
     
-    async def get_character(self, data):
+    async def get_character(self, data, build = {}):
         id = str(data.get("avatarId"))
         name = self.character.get(str(id)).get("name")
         rarity = self.character.get(str(id)).get("rarity")
         rank = data.get("rank", 0)
         level = data.get("level")
         promotion = data.get("promotion", 0)
         icon = self.character.get(str(id)).get("icon")
         preview = self.character.get(str(id)).get("preview")
         portrait = self.character.get(str(id)).get("portrait")
         rank_icons = [await self.get_rank_icons(key) for key in self.character.get(str(id)).get("ranks")]
         path = await self.get_path(self.character.get(str(id)).get("path"))
         element = await self.get_element(self.character.get(str(id)).get("element"))
         skills = await self.get_skill(data, str(id), self.character.get(str(id)).get("element"))
-        skill_trees = await self.get_skill_trees(data, str(id))
+        skill_trees = await self.get_skill_trees(data, str(id), rank)
         light_cone = await self.get_light_cone(data.get("equipment")) if data.get("equipment") else None
         attributes = await self.get_attributes(str(id), promotion, level)
         properties = await self.get_properties(str(id), data["skillTreeList"])
                 
         relic_infos = [await self.get_relic_info(relic) for relic in data["relicList"]]
         relics = [
             relic_info for relic_info in relic_infos if relic_info is not None
@@ -236,16 +255,15 @@
             [
                 properties,
                 light_cone["properties"] if light_cone else [],
                 relic_properties,
             ]
         )
         
-        additions = await self.get_additions(attributes, properties)
-    
+        additions = await self.get_additions(attributes, properties)        
       
         return {
             "id": id,
             "name": name,
             "rarity": rarity,
             "rank": rank,
             "level": level,
@@ -261,14 +279,15 @@
             "light_cone": light_cone,
             
             "relics": relics,
             "relic_sets": relic_sets,
             "attributes": attributes,
             "additions": additions,
             "properties": properties,
+            "build": build,
             "pos": [data.get("pos", 0)],
         }
         
     async def get_additions(self, attributes, properties):
         attribute_dict = {}
         addition_dict = {}
         for attribute in attributes:
@@ -362,21 +381,21 @@
                             "display": await self.get_display( i["value"], property["percent"]),
                             "percent": property["percent"],
                             "type": i["type"],
                         }
                     )
         return properties
     
-    async def get_skill_trees(self, data, character_id):
+    async def get_skill_trees(self, data, character_id, rank):
         return [{
             "id": str(key["pointId"]),
             "level": key["level"],
             "anchor": self.skill_trees_info.get(str(key["pointId"]))["anchor"],
             "icon": self.skill_trees_info.get(str(key["pointId"]))["icon"],
-            "max_level": await self.get_max_level(self.character.get(character_id)["ranks"], str(key["pointId"]),key.get("rank",0)),
+            "max_level": await self.get_max_level(self.character.get(character_id)["ranks"], str(key["pointId"]), rank),
             "parent": await self.get_parent(key["pointId"])
             } for key in data["skillTreeList"]]
     
     async def get_skill(self, data, character_data, element):
 
         character_data = self.character.get(character_data)
```

### Comparing `starrailcard-2.1.9/starrailcard/src/assets/font/font_hsr.ttf` & `starrailcard-2.2.0/starrailcard/src/assets/font/font_hsr.ttf`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.9/starrailcard/src/data/avatar.json` & `starrailcard-2.2.0/starrailcard/src/data/avatar.json`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.9/starrailcard/src/data/relict_sets.json` & `starrailcard-2.2.0/starrailcard/src/data/relict_sets.json`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.9/starrailcard/src/data/stats.json` & `starrailcard-2.2.0/starrailcard/src/data/stats.json`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.9/starrailcard/src/data/weapons.json` & `starrailcard-2.2.0/starrailcard/src/data/weapons.json`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.9/starrailcard/src/generator/style_card.py` & `starrailcard-2.2.0/starrailcard/src/generator/style_card.py`

 * *Files 1% similar despite different names*

```diff
@@ -187,15 +187,15 @@
         x = int(657 / (len(result)))
         position_line = 0
         for key in result:
             self.background_stats.alpha_composite(key, (0, position_line))
             position_line += x
     
     async def get_score(self):
-        self.score_info = await stats.Calculator(self.data).start()
+        self.score_info = await stats.Calculator(self.data).start(self.hoyo)
         
     async def create_relict(self,relict):
         background_main = Image.new(Card.RGBA,Card.relict_size, (0,0,0,0))
         background = Image.new(Card.RGBA,Card.relict_size, (0,0,0,0))
         background_image = Image.new("RGBA",Card.relict_size, (0,0,0,0))
         relict_frame = await _of.relict_frame
         relict_mask = await _of.relict_maska
@@ -464,16 +464,17 @@
         max_level = options.max_lvl(self.data.promotion)
         level = f"{self.lang.lvl}: {self.data.level}/{max_level}"
         d.text((Card.position_name_level[0]-1,Card.position_name_level[1]+1,), level, font=font_17, fill= (0,0,0,255))
         d.text(Card.position_name_level, level, font=font_17, fill= Card.color_name_level)
         starts = await options.get_stars(self.data.rarity)
         self.background_name.alpha_composite(starts, Card.position_name_star)
 
-    async def start(self):
+    async def start(self, build = None, hoyo = False ):
         _of.set_mapping(4)
+        self.hoyo = hoyo
         
         if self.art:
             if "gif" in self.art:
                 self.gif = True
             self.art = await pill.get_user_image(self.art)
             if self.gif:    
                 n = 2           
@@ -532,10 +533,11 @@
                 "id": self.data.id,
                 "name": self.data.name,
                 "animation": self.gif,
                 "rarity": self.data.rarity,
                 "card": self.background,
                 "size": Card.background_size,
                 "color": self.element_color,
+                "build": build
             }
             
         return data
```

### Comparing `starrailcard-2.1.9/starrailcard/src/generator/style_profile_phone.py` & `starrailcard-2.2.0/starrailcard/src/generator/style_profile_phone.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.9/starrailcard/src/generator/style_relict_score.py` & `starrailcard-2.2.0/starrailcard/src/generator/style_relict_score.py`

 * *Files 2% similar despite different names*

```diff
@@ -330,15 +330,15 @@
         
         return {"position": str(relict.id)[-1:] , "img": background_main}
     
     async def get_path(self):
         self.background_path = await pill.create_path(self.data)
     
     async def get_score(self):
-        self.score_info = await stats.Calculator(self.data).start()
+        self.score_info = await stats.Calculator(self.data).start(self.hoyo)
         
     async def build_relict(self):
         self.background_relict = Image.new(RelictScore.RGBA, (1131,297), (0,0,0,0))
         none_relict = await _of.none_relict
         position = {
             "1": (0,163),
             "2": (286,163),
@@ -434,17 +434,17 @@
             self.background = []
             for key in self.GIFT_BG:
                 key.alpha_composite(bg)
                 self.background.append(key.convert("RGB"))
         else:
             self.background.alpha_composite(bg)
                     
-    async def start(self):
+    async def start(self, build = None, hoyo = False):
         _of.set_mapping(1)
-        
+        self.hoyo = hoyo
         if self.art:
             if "gif" in self.art:
                 self.gif = True
             self.art = await pill.get_user_image(self.art)
             
         if self.gif:    
             n = 2           
@@ -504,11 +504,12 @@
         data = {
             "id": self.data.id,
             "animation":  self.gif,
             "name": self.data.name,
             "rarity": self.data.rarity,
             "card": self.background,
             "size": RelictScore.background_size,
-            "color": self.element_color
+            "color": self.element_color,
+            "build": build
         }
         
         return data
```

### Comparing `starrailcard-2.1.9/starrailcard/src/generator/style_ticket.py` & `starrailcard-2.2.0/starrailcard/src/generator/style_ticket.py`

 * *Files 0% similar despite different names*

```diff
@@ -314,15 +314,15 @@
                 self.background_sets.alpha_composite(key["line"],(0,0))
             elif key["setap"] == 3:
                 self.background_sets.alpha_composite(key["line"],(413,507))
             else:
                 self.background_sets.alpha_composite(key["line"],(0,45))
                 
     async def get_score(self):
-        self.score_info = await stats.Calculator(self.data).start()
+        self.score_info = await stats.Calculator(self.data).start(self.hoyo)
     
     async def create_stats(self):
         self.background_stats = Image.new(Ticket.RGBA, (434, 692), (0, 0, 0, 0))
 
         combined_attributes = {}
         dop = {}
         
@@ -597,17 +597,17 @@
             self.background = []
             for key in self.GIFT_BG:
                 key.alpha_composite(bg)
                 self.background.append(key.convert("RGB"))
         else:
             self.background.alpha_composite(bg)
         
-    async def start(self):
+    async def start(self, build = None, hoyo = False):
         _of.set_mapping(2)
-        
+        self.hoyo = hoyo
         if self.art:
             if "gif" in self.art:
                 self.gif = True
             self.art = await pill.get_user_image(self.art)
             if self.gif:    
                 n = 2           
                 frame_count = 0
@@ -670,10 +670,11 @@
                 "id": self.data.id,
                 "name": self.data.name,
                 "animation": self.gif,
                 "rarity": self.data.rarity,
                 "card": self.background,
                 "size": Ticket.background_size,
                 "color": self.element_color,
+                "build": build
             }
             
         return data
```

### Comparing `starrailcard-2.1.9/starrailcard/src/model/StarRailCard.py` & `starrailcard-2.2.0/starrailcard/src/model/StarRailCard.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,22 +30,27 @@
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         #self.icon = MAIN_LINK.format(icon = self.icon)
     
         if UA_LANG:
             self.name = TranslateDataManager._data.avatar.get(self.id, self.name)
 
+class BuildSetting(BaseModel):
+    id: Optional[Union[str,int]]
+    name_build: Optional[str]
+
 class Card(BaseModel):
     id: int
     name: Optional[str]
     rarity: int
     card: Union[Image.Image,list]
     animation: bool
     size: Optional[tuple]
     color: Optional[tuple]
+    build: Optional[BuildSetting]
     class Config:
         arbitrary_types_allowed = True
     
     async def get_info(self, lang = "en"):
         #await AioSession.get_session()
         url = f"https://api.yatta.top/hsr/v2/{lang}/avatar/{self.id}"
         data = await AioSession.get(url, response_format = "json")
@@ -85,15 +90,15 @@
             self.card.save(f"{name_file}.png")
         
 class Setting(BaseModel):
     uid: int
     lang: Optional[str]
     hide_uid: bool
     save: bool
-    force_update: bool
+    force_update: Optional[bool]
     style: int
     
 class StarRail(BaseModel):
     settings: Setting
     player: Player
     card: Union[List[Card], Image.Image]
     character_id: list
```

### Comparing `starrailcard-2.1.9/starrailcard/src/model/api_mihomo.py` & `starrailcard-2.2.0/starrailcard/src/model/api_mihomo.py`

 * *Files 1% similar despite different names*

```diff
@@ -272,15 +272,15 @@
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         #self.icon = MAIN_LINK.format(icon = self.icon)
 
         if UA_LANG:
             self.name = TranslateDataManager._data.stats.get(self.field, self.name)            
 
-        
+  
 class Character(BaseModel):
     id: Optional[str]
     name: Optional[str]
     rarity: int
     rank: int
     level: int
     promotion: int
@@ -294,14 +294,15 @@
     skill_trees: List[SkillTree]
     light_cone: Optional[LightCone]
     relics: Optional[List[Relic]]
     relic_sets: Optional[List[RelicSet]] = Field([], alias="relic_sets")
     attributes: List[CharacterAttributes]
     additions: List[CharacterAttributes]
     properties: Optional[List[CharacterProperties]]
+    build: Optional[dict] = Field(None)
     pos: list
     
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         #self.icon = MAIN_LINK.format(icon = self.icon)
         #self.preview = MAIN_LINK.format(icon = self.preview)
         #self.portrait = MAIN_LINK.format(icon = self.portrait)
```

### Comparing `starrailcard-2.1.9/starrailcard/src/model/style.py` & `starrailcard-2.2.0/starrailcard/src/model/style.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.9/starrailcard/src/model/utils_model.py` & `starrailcard-2.2.0/starrailcard/src/model/utils_model.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.9/starrailcard/src/tools/cache.py` & `starrailcard-2.2.0/starrailcard/src/tools/cache.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.9/starrailcard/src/tools/calculator/src/assets/rolls.json` & `starrailcard-2.2.0/starrailcard/src/tools/calculator/src/assets/rolls.json`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.9/starrailcard/src/tools/calculator/src/assets/score.json` & `starrailcard-2.2.0/starrailcard/src/tools/calculator/src/assets/score.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9252071391828336%*

 * *Differences: {"'1304'": "{'main': {'3': {'HPAddedRatio': 0, 'CriticalChanceBase': 0.8, 'CriticalDamageBase': "*

 * *           "1}, '4': {'HPAddedRatio': 0, 'DefenceAddedRatio': 1, 'SpeedDelta': 0.8}, '5': "*

 * *           "{'HPAddedRatio': 0, 'ImaginaryAddedRatio': 0.8}, '6': {'BreakDamageAddedRatioBase': 0, "*

 * *           "'SPRatioBase': 0, 'HPAddedRatio': 0, 'DefenceAddedRatio': 1}}, 'weight': {'HPDelta': "*

 * *           "0, 'DefenceDelta': 0.5, 'HPAddedRatio': 0, 'DefenceAddedRatio': 1, 'SpeedDelta': 0.8, "*

 * *           "'CriticalC […]*

```diff
@@ -2365,61 +2365,61 @@
                 "HPDelta": 1
             },
             "2": {
                 "AttackDelta": 1
             },
             "3": {
                 "AttackAddedRatio": 0,
-                "CriticalChanceBase": 0,
-                "CriticalDamageBase": 0,
+                "CriticalChanceBase": 0.8,
+                "CriticalDamageBase": 1,
                 "DefenceAddedRatio": 1,
-                "HPAddedRatio": 1,
+                "HPAddedRatio": 0,
                 "HealRatioBase": 0,
                 "StatusProbabilityBase": 0
             },
             "4": {
                 "AttackAddedRatio": 0,
-                "DefenceAddedRatio": 0.8,
-                "HPAddedRatio": 0.8,
-                "SpeedDelta": 1
+                "DefenceAddedRatio": 1,
+                "HPAddedRatio": 0,
+                "SpeedDelta": 0.8
             },
             "5": {
                 "AttackAddedRatio": 0,
                 "DefenceAddedRatio": 1,
                 "FireAddedRatio": 0,
-                "HPAddedRatio": 1,
+                "HPAddedRatio": 0,
                 "IceAddedRatio": 0,
-                "ImaginaryAddedRatio": 0,
+                "ImaginaryAddedRatio": 0.8,
                 "PhysicalAddedRatio": 0,
                 "QuantumAddedRatio": 0,
                 "ThunderAddedRatio": 0,
                 "WindAddedRatio": 0
             },
             "6": {
                 "AttackAddedRatio": 0,
-                "BreakDamageAddedRatioBase": 1,
-                "DefenceAddedRatio": 0.8,
-                "HPAddedRatio": 0.8,
-                "SPRatioBase": 1
+                "BreakDamageAddedRatioBase": 0,
+                "DefenceAddedRatio": 1,
+                "HPAddedRatio": 0,
+                "SPRatioBase": 0
             }
         },
         "max": 10.0,
         "weight": {
             "AttackAddedRatio": 0,
             "AttackDelta": 0,
-            "BreakDamageAddedRatioBase": 1,
-            "CriticalChanceBase": 0,
-            "CriticalDamageBase": 0,
-            "DefenceAddedRatio": 0.8,
-            "DefenceDelta": 0.3,
-            "HPAddedRatio": 0.8,
-            "HPDelta": 0.3,
-            "SpeedDelta": 1,
+            "BreakDamageAddedRatioBase": 0,
+            "CriticalChanceBase": 0.8,
+            "CriticalDamageBase": 1,
+            "DefenceAddedRatio": 1,
+            "DefenceDelta": 0.5,
+            "HPAddedRatio": 0,
+            "HPDelta": 0,
+            "SpeedDelta": 0.8,
             "StatusProbabilityBase": 0,
-            "StatusResistanceBase": 0.5
+            "StatusResistanceBase": 0
         }
     },
     "1305": {
         "main": {
             "1": {
                 "HPDelta": 1
             },
@@ -2650,14 +2650,73 @@
             "HPAddedRatio": 0,
             "HPDelta": 0,
             "SpeedDelta": 0.6,
             "StatusProbabilityBase": 0,
             "StatusResistanceBase": 0
         }
     },
+    "1309": {
+        "main": {
+            "1": {
+                "HPDelta": 1
+            },
+            "2": {
+                "AttackDelta": 1
+            },
+            "3": {
+                "AttackAddedRatio": 1,
+                "CriticalChanceBase": 0,
+                "CriticalDamageBase": 0,
+                "DefenceAddedRatio": 0.9,
+                "HPAddedRatio": 0.8,
+                "HealRatioBase": 0,
+                "StatusProbabilityBase": 0
+            },
+            "4": {
+                "AttackAddedRatio": 1,
+                "DefenceAddedRatio": 0.9,
+                "HPAddedRatio": 0.8,
+                "SpeedDelta": 0.9
+            },
+            "5": {
+                "AttackAddedRatio": 1,
+                "DefenceAddedRatio": 0.9,
+                "FireAddedRatio": 0,
+                "HPAddedRatio": 0.8,
+                "IceAddedRatio": 0,
+                "ImaginaryAddedRatio": 0,
+                "PhysicalAddedRatio": 1,
+                "QuantumAddedRatio": 0,
+                "ThunderAddedRatio": 0,
+                "WindAddedRatio": 0
+            },
+            "6": {
+                "AttackAddedRatio": 1,
+                "BreakDamageAddedRatioBase": 0,
+                "DefenceAddedRatio": 0.9,
+                "HPAddedRatio": 0.8,
+                "SPRatioBase": 1
+            }
+        },
+        "max": 0.0,
+        "weight": {
+            "AttackAddedRatio": 1,
+            "AttackDelta": 0.6,
+            "BreakDamageAddedRatioBase": 0,
+            "CriticalChanceBase": 0,
+            "CriticalDamageBase": 0,
+            "DefenceAddedRatio": 0.9,
+            "DefenceDelta": 0.5,
+            "HPAddedRatio": 0.8,
+            "HPDelta": 0.4,
+            "SpeedDelta": 0.9,
+            "StatusProbabilityBase": 0,
+            "StatusResistanceBase": 0.8
+        }
+    },
     "1312": {
         "main": {
             "1": {
                 "HPDelta": 1
             },
             "2": {
                 "AttackDelta": 1
@@ -2709,14 +2768,73 @@
             "HPAddedRatio": 0,
             "HPDelta": 0,
             "SpeedDelta": 0.8,
             "StatusProbabilityBase": 0.6,
             "StatusResistanceBase": 0
         }
     },
+    "1315": {
+        "main": {
+            "1": {
+                "HPDelta": 1
+            },
+            "2": {
+                "AttackDelta": 1
+            },
+            "3": {
+                "AttackAddedRatio": 0.8,
+                "CriticalChanceBase": 1,
+                "CriticalDamageBase": 1,
+                "DefenceAddedRatio": 0,
+                "HPAddedRatio": 0,
+                "HealRatioBase": 0,
+                "StatusProbabilityBase": 0.6
+            },
+            "4": {
+                "AttackAddedRatio": 1,
+                "DefenceAddedRatio": 0,
+                "HPAddedRatio": 0,
+                "SpeedDelta": 1
+            },
+            "5": {
+                "AttackAddedRatio": 1,
+                "DefenceAddedRatio": 0,
+                "FireAddedRatio": 0,
+                "HPAddedRatio": 0,
+                "IceAddedRatio": 1,
+                "ImaginaryAddedRatio": 0,
+                "PhysicalAddedRatio": 0,
+                "QuantumAddedRatio": 0,
+                "ThunderAddedRatio": 0,
+                "WindAddedRatio": 0
+            },
+            "6": {
+                "AttackAddedRatio": 1,
+                "BreakDamageAddedRatioBase": 0,
+                "DefenceAddedRatio": 0,
+                "HPAddedRatio": 0,
+                "SPRatioBase": 0
+            }
+        },
+        "max": 0.0,
+        "weight": {
+            "AttackAddedRatio": 0.8,
+            "AttackDelta": 0.3,
+            "BreakDamageAddedRatioBase": 0,
+            "CriticalChanceBase": 1,
+            "CriticalDamageBase": 1,
+            "DefenceAddedRatio": 0,
+            "DefenceDelta": 0,
+            "HPAddedRatio": 0,
+            "HPDelta": 0,
+            "SpeedDelta": 0.8,
+            "StatusProbabilityBase": 0.6,
+            "StatusResistanceBase": 0
+        }
+    },
     "8001": {
         "main": {
             "1": {
                 "HPDelta": 1
             },
             "2": {
                 "AttackDelta": 1
@@ -2944,9 +3062,127 @@
             "DefenceDelta": 0.5,
             "HPAddedRatio": 0.5,
             "HPDelta": 0.2,
             "SpeedDelta": 1,
             "StatusProbabilityBase": 1,
             "StatusResistanceBase": 0.5
         }
+    },
+    "8005": {
+        "main": {
+            "1": {
+                "HPDelta": 1
+            },
+            "2": {
+                "AttackDelta": 1
+            },
+            "3": {
+                "AttackAddedRatio": 0.8,
+                "CriticalChanceBase": 0,
+                "CriticalDamageBase": 0,
+                "DefenceAddedRatio": 1,
+                "HPAddedRatio": 1,
+                "HealRatioBase": 0,
+                "StatusProbabilityBase": 0
+            },
+            "4": {
+                "AttackAddedRatio": 0.8,
+                "DefenceAddedRatio": 0,
+                "HPAddedRatio": 0,
+                "SpeedDelta": 1
+            },
+            "5": {
+                "AttackAddedRatio": 0.8,
+                "DefenceAddedRatio": 1,
+                "FireAddedRatio": 0,
+                "HPAddedRatio": 1,
+                "IceAddedRatio": 0,
+                "ImaginaryAddedRatio": 0.8,
+                "PhysicalAddedRatio": 0,
+                "QuantumAddedRatio": 0,
+                "ThunderAddedRatio": 0,
+                "WindAddedRatio": 0
+            },
+            "6": {
+                "AttackAddedRatio": 0.8,
+                "BreakDamageAddedRatioBase": 1,
+                "DefenceAddedRatio": 0,
+                "HPAddedRatio": 0,
+                "SPRatioBase": 1
+            }
+        },
+        "max": 9.8,
+        "weight": {
+            "AttackAddedRatio": 0.8,
+            "AttackDelta": 0.4,
+            "BreakDamageAddedRatioBase": 0.9,
+            "CriticalChanceBase": 0.7,
+            "CriticalDamageBase": 0.7,
+            "DefenceAddedRatio": 0.7,
+            "DefenceDelta": 0.3,
+            "HPAddedRatio": 0.7,
+            "HPDelta": 0.3,
+            "SpeedDelta": 1,
+            "StatusProbabilityBase": 0.7,
+            "StatusResistanceBase": 0.7
+        }
+    },
+    "8006": {
+        "main": {
+            "1": {
+                "HPDelta": 1
+            },
+            "2": {
+                "AttackDelta": 1
+            },
+            "3": {
+                "AttackAddedRatio": 0.8,
+                "CriticalChanceBase": 0,
+                "CriticalDamageBase": 0,
+                "DefenceAddedRatio": 1,
+                "HPAddedRatio": 1,
+                "HealRatioBase": 0,
+                "StatusProbabilityBase": 0
+            },
+            "4": {
+                "AttackAddedRatio": 0.8,
+                "DefenceAddedRatio": 0,
+                "HPAddedRatio": 0,
+                "SpeedDelta": 1
+            },
+            "5": {
+                "AttackAddedRatio": 0.8,
+                "DefenceAddedRatio": 1,
+                "FireAddedRatio": 0,
+                "HPAddedRatio": 1,
+                "IceAddedRatio": 0,
+                "ImaginaryAddedRatio": 0.8,
+                "PhysicalAddedRatio": 0,
+                "QuantumAddedRatio": 0,
+                "ThunderAddedRatio": 0,
+                "WindAddedRatio": 0
+            },
+            "6": {
+                "AttackAddedRatio": 0.8,
+                "BreakDamageAddedRatioBase": 1,
+                "DefenceAddedRatio": 0,
+                "HPAddedRatio": 0,
+                "SPRatioBase": 1
+            }
+        },
+        "max": 9.8,
+        "weight": {
+            "AttackAddedRatio": 0.8,
+            "AttackDelta": 0.4,
+            "BreakDamageAddedRatioBase": 0.9,
+            "CriticalChanceBase": 0.7,
+            "CriticalDamageBase": 0.7,
+            "DefenceAddedRatio": 0.7,
+            "DefenceDelta": 0.3,
+            "HPAddedRatio": 0.7,
+            "HPDelta": 0.3,
+            "SpeedDelta": 1,
+            "StatusProbabilityBase": 0.7,
+            "StatusResistanceBase": 0.7
+        }
     }
 }
```

### Comparing `starrailcard-2.1.9/starrailcard/src/tools/calculator/src/utils.py` & `starrailcard-2.2.0/starrailcard/src/tools/calculator/src/utils.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.9/starrailcard/src/tools/calculator/stats.py` & `starrailcard-2.2.0/starrailcard/src/tools/calculator/stats.py`

 * *Files 3% similar despite different names*

```diff
@@ -79,16 +79,18 @@
                     if abs(value_sum - value) < max_margin:
                         max_margin = abs(value_sum - value)
                         result = i+j+k 
         return result
     
     async def get_relic_score(self, chara_id, relic_json):
         result_json = {}
-        
-        main_weight = self.score[chara_id]["main"][self.relict_id.get(relic_json.id, relic_json.id)[-1]][relic_json.main_affix.type]
+        try:
+            main_weight = self.score[chara_id]["main"][self.relict_id.get(relic_json.id, relic_json.id)[-1]][relic_json.main_affix.type]
+        except:
+            main_weight = 0
         main_affix_score = (relic_json.level + 1) / 16 * main_weight
         result_json["main_formula"] = f'{round((relic_json.level + 1) / 16 * 100, 1)}×{main_weight}={main_affix_score * 100}'
         
         sub_affix_formulas = []
         dont_sub = []
         for sub_affix_json in relic_json.sub_affix:
             if self.score[chara_id]["weight"][sub_affix_json.type] <= 0.3:
@@ -97,15 +99,17 @@
         sub_affix_score = sum((sub_affix_json.value / self.max[sub_affix_json.type]) * self.score[chara_id]["weight"][sub_affix_json.type] for sub_affix_json in relic_json.sub_affix)
 
         result_json["score"] = main_affix_score * 0.2 + sub_affix_score * 0.2
         result_json["sub_formulas"] = sub_affix_formulas
 
         return result_json,dont_sub
 
-    async def start(self):
+    async def start(self, hoyo):
+        if hoyo:
+            return self.result
         
         if not self.data.id in self.score:
             await self.update_score(self.data.id)
             self.score = open_score("score")
         if not self.data.id in self.score:
             return self.result
         for key in self.data.relics:
```

### Comparing `starrailcard-2.1.9/starrailcard/src/tools/enums.py` & `starrailcard-2.2.0/starrailcard/src/tools/enums.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.9/starrailcard/src/tools/git.py` & `starrailcard-2.2.0/starrailcard/src/tools/git.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.9/starrailcard/src/tools/http.py` & `starrailcard-2.2.0/starrailcard/src/tools/http.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.9/starrailcard/src/tools/json_data.py` & `starrailcard-2.2.0/starrailcard/src/tools/json_data.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.9/starrailcard/src/tools/options.py` & `starrailcard-2.2.0/starrailcard/src/tools/options.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.9/starrailcard/src/tools/pill/color.py` & `starrailcard-2.2.0/starrailcard/src/tools/pill/color.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.9/starrailcard/src/tools/pill/color_control.py` & `starrailcard-2.2.0/starrailcard/src/tools/pill/color_control.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.9/starrailcard/src/tools/pill/diagrama.py` & `starrailcard-2.2.0/starrailcard/src/tools/pill/diagrama.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.9/starrailcard/src/tools/pill/gradient_v2.py` & `starrailcard-2.2.0/starrailcard/src/tools/pill/gradient_v2.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.9/starrailcard/src/tools/pill/grandient_v1.py` & `starrailcard-2.2.0/starrailcard/src/tools/pill/grandient_v1.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.9/starrailcard/src/tools/pill/image_control.py` & `starrailcard-2.2.0/starrailcard/src/tools/pill/image_control.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.9/starrailcard/src/tools/pill/style_editor.py` & `starrailcard-2.2.0/starrailcard/src/tools/pill/style_editor.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.9/starrailcard/src/tools/pill/text_control.py` & `starrailcard-2.2.0/starrailcard/src/tools/pill/text_control.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.9/starrailcard/src/tools/translator.py` & `starrailcard-2.2.0/starrailcard/src/tools/translator.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.9/starrailcard/src/tools/treePaths.py` & `starrailcard-2.2.0/starrailcard/src/tools/treePaths.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.9/starrailcard/src/tools/ukrainization.py` & `starrailcard-2.2.0/starrailcard/src/tools/ukrainization.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.9/starrailcard/utils.py` & `starrailcard-2.2.0/starrailcard/utils.py`

 * *Files identical despite different names*

### Comparing `starrailcard-2.1.9/starrailcard.egg-info/PKG-INFO` & `starrailcard-2.2.0/starrailcard.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starrailcard
-Version: 2.1.9
+Version: 2.2.0
 Summary: This Python module provides the ability to create captivating character cards based on player data from Honkai Star Rail, obtained through their unique user identifiers (UIDs). StarRailCard streamlines the process of generating personalized character assembly cards, relying on the information provided by players.
 Home-page: https://github.com/DEViantUA/StarRailCard
 Author: DeviantUa
 Author-email: deviantapi@gmail.com
 Keywords: honkai,cards,generation,honkaistarraill,raill,starraill,builds,honkairail,honkai,genshin,build,api
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `starrailcard-2.1.9/starrailcard.egg-info/SOURCES.txt` & `starrailcard-2.2.0/starrailcard.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 starrailcard.egg-info/dependency_links.txt
 starrailcard.egg-info/requires.txt
 starrailcard.egg-info/top_level.txt
 starrailcard/src/api/api.py
 starrailcard/src/api/enka.py
 starrailcard/src/api/enka_parsed.py
 starrailcard/src/api/error.py
+starrailcard/src/api/hoyolab.py
+starrailcard/src/api/hoyolab_parsed.py
 starrailcard/src/assets/font/font_hsr.ttf
 starrailcard/src/data/avatar.json
 starrailcard/src/data/element.json
 starrailcard/src/data/keys.json
 starrailcard/src/data/paths.json
 starrailcard/src/data/relict_sets.json
 starrailcard/src/data/stats.json
@@ -28,19 +30,14 @@
 starrailcard/src/generator/style_relict_score.py
 starrailcard/src/generator/style_ticket.py
 starrailcard/src/model/StarRailCard.py
 starrailcard/src/model/api_mihomo.py
 starrailcard/src/model/style.py
 starrailcard/src/model/ukrainization_model.py
 starrailcard/src/model/utils_model.py
-starrailcard/src/model/__pycache__/StarRailCard.cpython-312.pyc
-starrailcard/src/model/__pycache__/api_mihomo.cpython-312.pyc
-starrailcard/src/model/__pycache__/style.cpython-312.pyc
-starrailcard/src/model/__pycache__/ukrainization_model.cpython-312.pyc
-starrailcard/src/model/__pycache__/utils_model.cpython-312.pyc
 starrailcard/src/tools/cache.py
 starrailcard/src/tools/enums.py
 starrailcard/src/tools/git.py
 starrailcard/src/tools/http.py
 starrailcard/src/tools/json_data.py
 starrailcard/src/tools/options.py
 starrailcard/src/tools/translator.py
```

