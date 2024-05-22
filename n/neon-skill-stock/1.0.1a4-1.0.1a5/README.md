# Comparing `tmp/neon-skill-stock-1.0.1a4.tar.gz` & `tmp/neon-skill-stock-1.0.1a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-skill-stock-1.0.1a4.tar", last modified: Mon May  6 21:54:13 2024, max compression
+gzip compressed data, was "neon-skill-stock-1.0.1a5.tar", last modified: Wed May 22 22:11:51 2024, max compression
```

## Comparing `neon-skill-stock-1.0.1a4.tar` & `neon-skill-stock-1.0.1a5.tar`

### file list

```diff
@@ -1,111 +1,113 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:54:13.341797 neon-skill-stock-1.0.1a4/
--rwxr-xr-x   0 runner    (1001) docker     (127)    11558 2024-05-06 21:54:10.000000 neon-skill-stock-1.0.1a4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-05-06 21:54:10.000000 neon-skill-stock-1.0.1a4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-05-06 21:54:13.341797 neon-skill-stock-1.0.1a4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-06 21:54:10.000000 neon-skill-stock-1.0.1a4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     5755 2024-05-06 21:54:10.000000 neon-skill-stock-1.0.1a4/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:54:13.329797 neon-skill-stock-1.0.1a4/locale/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:54:13.325797 neon-skill-stock-1.0.1a4/locale/ca-es/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:54:13.329797 neon-skill-stock-1.0.1a4/locale/ca-es/dialog/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-06 21:54:10.000000 neon-skill-stock-1.0.1a4/locale/ca-es/dialog/api.error.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-06 21:54:10.000000 neon-skill-stock-1.0.1a4/locale/ca-es/dialog/not.found.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-06 21:54:10.000000 neon-skill-stock-1.0.1a4/locale/ca-es/dialog/stock.price.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:54:13.329797 neon-skill-stock-1.0.1a4/locale/ca-es/regex/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-06 21:54:10.000000 neon-skill-stock-1.0.1a4/locale/ca-es/regex/company.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:54:13.325797 neon-skill-stock-1.0.1a4/locale/de-de/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:54:13.333797 neon-skill-stock-1.0.1a4/locale/de-de/dialog/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-06 21:54:10.000000 neon-skill-stock-1.0.1a4/locale/de-de/dialog/api.error.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-06 21:54:10.000000 neon-skill-stock-1.0.1a4/locale/de-de/dialog/not.found.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-06 21:54:10.000000 neon-skill-stock-1.0.1a4/locale/de-de/dialog/stock.price.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:54:13.333797 neon-skill-stock-1.0.1a4/locale/de-de/regex/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-06 21:54:10.000000 neon-skill-stock-1.0.1a4/locale/de-de/regex/company.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:54:13.325797 neon-skill-stock-1.0.1a4/locale/el-gr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:54:13.333797 neon-skill-stock-1.0.1a4/locale/el-gr/dialog/
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-06 21:54:10.000000 neon-skill-stock-1.0.1a4/locale/el-gr/dialog/not.found.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-06 21:54:10.000000 neon-skill-stock-1.0.1a4/locale/el-gr/dialog/stock.price.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:54:13.333797 neon-skill-stock-1.0.1a4/locale/el-gr/regex/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-06 21:54:10.000000 neon-skill-stock-1.0.1a4/locale/el-gr/regex/company.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:54:13.325797 neon-skill-stock-1.0.1a4/locale/en-us/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:54:13.333797 neon-skill-stock-1.0.1a4/locale/en-us/dialog/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-06 21:54:10.000000 neon-skill-stock-1.0.1a4/locale/en-us/dialog/api.error.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-06 21:54:10.000000 neon-skill-stock-1.0.1a4/locale/en-us/dialog/not.found.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-06 21:54:10.000000 neon-skill-stock-1.0.1a4/locale/en-us/dialog/stock.price.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:54:13.333797 neon-skill-stock-1.0.1a4/locale/en-us/intent/
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-06 21:54:10.000000 neon-skill-stock-1.0.1a4/locale/en-us/intent/stock_price.intent
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:54:13.325797 neon-skill-stock-1.0.1a4/locale/es-es/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:54:13.333797 neon-skill-stock-1.0.1a4/locale/es-es/dialog/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-06 21:54:10.000000 neon-skill-stock-1.0.1a4/locale/es-es/dialog/api.error.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-06 21:54:10.000000 neon-skill-stock-1.0.1a4/locale/es-es/dialog/not.found.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-06 21:54:10.000000 neon-skill-stock-1.0.1a4/locale/es-es/dialog/stock.price.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:54:13.333797 neon-skill-stock-1.0.1a4/locale/es-es/regex/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-06 21:54:10.000000 neon-skill-stock-1.0.1a4/locale/es-es/regex/company.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:54:13.325797 neon-skill-stock-1.0.1a4/locale/fr-fr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:54:13.333797 neon-skill-stock-1.0.1a4/locale/fr-fr/dialog/
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-06 21:54:10.000000 neon-skill-stock-1.0.1a4/locale/fr-fr/dialog/api.error.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-06 21:54:10.000000 neon-skill-stock-1.0.1a4/locale/fr-fr/dialog/not.found.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-06 21:54:10.000000 neon-skill-stock-1.0.1a4/locale/fr-fr/dialog/stock.price.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:54:13.333797 neon-skill-stock-1.0.1a4/locale/fr-fr/regex/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-06 21:54:10.000000 neon-skill-stock-1.0.1a4/locale/fr-fr/regex/company.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:54:13.329797 neon-skill-stock-1.0.1a4/locale/gl-es/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:54:13.333797 neon-skill-stock-1.0.1a4/locale/gl-es/dialog/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-06 21:54:10.000000 neon-skill-stock-1.0.1a4/locale/gl-es/dialog/api.error.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-06 21:54:10.000000 neon-skill-stock-1.0.1a4/locale/gl-es/dialog/not.found.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-06 21:54:10.000000 neon-skill-stock-1.0.1a4/locale/gl-es/dialog/stock.price.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:54:13.333797 neon-skill-stock-1.0.1a4/locale/gl-es/regex/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-06 21:54:10.000000 neon-skill-stock-1.0.1a4/locale/gl-es/regex/company.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:54:13.329797 neon-skill-stock-1.0.1a4/locale/hu-hu/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:54:13.333797 neon-skill-stock-1.0.1a4/locale/hu-hu/dialog/
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-06 21:54:10.000000 neon-skill-stock-1.0.1a4/locale/hu-hu/dialog/not.found.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-06 21:54:10.000000 neon-skill-stock-1.0.1a4/locale/hu-hu/dialog/stock.price.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:54:13.333797 neon-skill-stock-1.0.1a4/locale/hu-hu/regex/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-06 21:54:10.000000 neon-skill-stock-1.0.1a4/locale/hu-hu/regex/company.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:54:13.329797 neon-skill-stock-1.0.1a4/locale/it-it/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:54:13.337797 neon-skill-stock-1.0.1a4/locale/it-it/dialog/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-06 21:54:10.000000 neon-skill-stock-1.0.1a4/locale/it-it/dialog/api.error.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-06 21:54:10.000000 neon-skill-stock-1.0.1a4/locale/it-it/dialog/not.found.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-06 21:54:10.000000 neon-skill-stock-1.0.1a4/locale/it-it/dialog/stock.price.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:54:13.337797 neon-skill-stock-1.0.1a4/locale/it-it/regex/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-06 21:54:10.000000 neon-skill-stock-1.0.1a4/locale/it-it/regex/company.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:54:13.329797 neon-skill-stock-1.0.1a4/locale/nl-nl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:54:13.337797 neon-skill-stock-1.0.1a4/locale/nl-nl/dialog/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-06 21:54:10.000000 neon-skill-stock-1.0.1a4/locale/nl-nl/dialog/api.error.dialog
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-06 21:54:10.000000 neon-skill-stock-1.0.1a4/locale/nl-nl/dialog/not.found.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-06 21:54:10.000000 neon-skill-stock-1.0.1a4/locale/nl-nl/dialog/stock.price.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:54:13.337797 neon-skill-stock-1.0.1a4/locale/nl-nl/regex/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-06 21:54:10.000000 neon-skill-stock-1.0.1a4/locale/nl-nl/regex/company.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:54:13.329797 neon-skill-stock-1.0.1a4/locale/pt-br/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:54:13.337797 neon-skill-stock-1.0.1a4/locale/pt-br/dialog/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-06 21:54:10.000000 neon-skill-stock-1.0.1a4/locale/pt-br/dialog/api.error.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-06 21:54:10.000000 neon-skill-stock-1.0.1a4/locale/pt-br/dialog/not.found.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-06 21:54:10.000000 neon-skill-stock-1.0.1a4/locale/pt-br/dialog/stock.price.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:54:13.337797 neon-skill-stock-1.0.1a4/locale/pt-br/regex/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-06 21:54:10.000000 neon-skill-stock-1.0.1a4/locale/pt-br/regex/company.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:54:13.329797 neon-skill-stock-1.0.1a4/locale/ru-ru/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:54:13.337797 neon-skill-stock-1.0.1a4/locale/ru-ru/dialog/
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-06 21:54:10.000000 neon-skill-stock-1.0.1a4/locale/ru-ru/dialog/not.found.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-06 21:54:10.000000 neon-skill-stock-1.0.1a4/locale/ru-ru/dialog/stock.price.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:54:13.337797 neon-skill-stock-1.0.1a4/locale/ru-ru/regex/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-06 21:54:10.000000 neon-skill-stock-1.0.1a4/locale/ru-ru/regex/company.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:54:13.329797 neon-skill-stock-1.0.1a4/locale/sv-se/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:54:13.337797 neon-skill-stock-1.0.1a4/locale/sv-se/dialog/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-06 21:54:10.000000 neon-skill-stock-1.0.1a4/locale/sv-se/dialog/api.error.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-06 21:54:10.000000 neon-skill-stock-1.0.1a4/locale/sv-se/dialog/not.found.dialog
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-06 21:54:10.000000 neon-skill-stock-1.0.1a4/locale/sv-se/dialog/stock.price.dialog
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:54:13.337797 neon-skill-stock-1.0.1a4/locale/sv-se/regex/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-06 21:54:10.000000 neon-skill-stock-1.0.1a4/locale/sv-se/regex/company.rx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:54:13.337797 neon-skill-stock-1.0.1a4/neon_skill_stock.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-05-06 21:54:13.000000 neon-skill-stock-1.0.1a4/neon_skill_stock.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2024-05-06 21:54:13.000000 neon-skill-stock-1.0.1a4/neon_skill_stock.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 21:54:13.000000 neon-skill-stock-1.0.1a4/neon_skill_stock.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-06 21:54:13.000000 neon-skill-stock-1.0.1a4/neon_skill_stock.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-06 21:54:13.000000 neon-skill-stock-1.0.1a4/neon_skill_stock.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-06 21:54:13.000000 neon-skill-stock-1.0.1a4/neon_skill_stock.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 21:54:13.341797 neon-skill-stock-1.0.1a4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4504 2024-05-06 21:54:10.000000 neon-skill-stock-1.0.1a4/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-05-06 21:54:10.000000 neon-skill-stock-1.0.1a4/skill.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:54:13.337797 neon-skill-stock-1.0.1a4/test/
--rw-r--r--   0 runner    (1001) docker     (127)     3650 2024-05-06 21:54:10.000000 neon-skill-stock-1.0.1a4/test/test_skill.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 21:54:13.337797 neon-skill-stock-1.0.1a4/ui/
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-06 21:54:10.000000 neon-skill-stock-1.0.1a4/ui/Stock.qml
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-06 21:54:10.000000 neon-skill-stock-1.0.1a4/ui/qmldir
--rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-05-06 21:54:10.000000 neon-skill-stock-1.0.1a4/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:11:51.557770 neon-skill-stock-1.0.1a5/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11558 2024-05-22 22:11:48.000000 neon-skill-stock-1.0.1a5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-05-22 22:11:48.000000 neon-skill-stock-1.0.1a5/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-05-22 22:11:51.557770 neon-skill-stock-1.0.1a5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-22 22:11:48.000000 neon-skill-stock-1.0.1a5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7779 2024-05-22 22:11:48.000000 neon-skill-stock-1.0.1a5/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:11:51.549770 neon-skill-stock-1.0.1a5/locale/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:11:51.545770 neon-skill-stock-1.0.1a5/locale/ca-es/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:11:51.549770 neon-skill-stock-1.0.1a5/locale/ca-es/dialog/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-22 22:11:48.000000 neon-skill-stock-1.0.1a5/locale/ca-es/dialog/api.error.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-22 22:11:48.000000 neon-skill-stock-1.0.1a5/locale/ca-es/dialog/not.found.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-22 22:11:48.000000 neon-skill-stock-1.0.1a5/locale/ca-es/dialog/stock.price.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:11:51.549770 neon-skill-stock-1.0.1a5/locale/ca-es/regex/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-22 22:11:48.000000 neon-skill-stock-1.0.1a5/locale/ca-es/regex/company.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:11:51.545770 neon-skill-stock-1.0.1a5/locale/de-de/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:11:51.549770 neon-skill-stock-1.0.1a5/locale/de-de/dialog/
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-22 22:11:48.000000 neon-skill-stock-1.0.1a5/locale/de-de/dialog/api.error.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-22 22:11:48.000000 neon-skill-stock-1.0.1a5/locale/de-de/dialog/not.found.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-22 22:11:48.000000 neon-skill-stock-1.0.1a5/locale/de-de/dialog/stock.price.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:11:51.549770 neon-skill-stock-1.0.1a5/locale/de-de/regex/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-22 22:11:48.000000 neon-skill-stock-1.0.1a5/locale/de-de/regex/company.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:11:51.545770 neon-skill-stock-1.0.1a5/locale/el-gr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:11:51.549770 neon-skill-stock-1.0.1a5/locale/el-gr/dialog/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-22 22:11:48.000000 neon-skill-stock-1.0.1a5/locale/el-gr/dialog/not.found.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-22 22:11:48.000000 neon-skill-stock-1.0.1a5/locale/el-gr/dialog/stock.price.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:11:51.549770 neon-skill-stock-1.0.1a5/locale/el-gr/regex/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-22 22:11:48.000000 neon-skill-stock-1.0.1a5/locale/el-gr/regex/company.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:11:51.545770 neon-skill-stock-1.0.1a5/locale/en-us/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:11:51.553770 neon-skill-stock-1.0.1a5/locale/en-us/dialog/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-22 22:11:48.000000 neon-skill-stock-1.0.1a5/locale/en-us/dialog/api.error.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-22 22:11:48.000000 neon-skill-stock-1.0.1a5/locale/en-us/dialog/not.found.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-22 22:11:48.000000 neon-skill-stock-1.0.1a5/locale/en-us/dialog/stock.price.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:11:51.553770 neon-skill-stock-1.0.1a5/locale/en-us/intent/
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-05-22 22:11:48.000000 neon-skill-stock-1.0.1a5/locale/en-us/intent/stock_price.intent
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:11:51.553770 neon-skill-stock-1.0.1a5/locale/en-us/regex/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-22 22:11:48.000000 neon-skill-stock-1.0.1a5/locale/en-us/regex/company.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:11:51.545770 neon-skill-stock-1.0.1a5/locale/es-es/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:11:51.553770 neon-skill-stock-1.0.1a5/locale/es-es/dialog/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-22 22:11:48.000000 neon-skill-stock-1.0.1a5/locale/es-es/dialog/api.error.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-22 22:11:48.000000 neon-skill-stock-1.0.1a5/locale/es-es/dialog/not.found.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-22 22:11:48.000000 neon-skill-stock-1.0.1a5/locale/es-es/dialog/stock.price.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:11:51.553770 neon-skill-stock-1.0.1a5/locale/es-es/regex/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-22 22:11:48.000000 neon-skill-stock-1.0.1a5/locale/es-es/regex/company.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:11:51.545770 neon-skill-stock-1.0.1a5/locale/fr-fr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:11:51.553770 neon-skill-stock-1.0.1a5/locale/fr-fr/dialog/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-22 22:11:48.000000 neon-skill-stock-1.0.1a5/locale/fr-fr/dialog/api.error.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-22 22:11:48.000000 neon-skill-stock-1.0.1a5/locale/fr-fr/dialog/not.found.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-22 22:11:48.000000 neon-skill-stock-1.0.1a5/locale/fr-fr/dialog/stock.price.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:11:51.553770 neon-skill-stock-1.0.1a5/locale/fr-fr/regex/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-22 22:11:48.000000 neon-skill-stock-1.0.1a5/locale/fr-fr/regex/company.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:11:51.545770 neon-skill-stock-1.0.1a5/locale/gl-es/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:11:51.553770 neon-skill-stock-1.0.1a5/locale/gl-es/dialog/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-22 22:11:48.000000 neon-skill-stock-1.0.1a5/locale/gl-es/dialog/api.error.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-22 22:11:48.000000 neon-skill-stock-1.0.1a5/locale/gl-es/dialog/not.found.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-22 22:11:48.000000 neon-skill-stock-1.0.1a5/locale/gl-es/dialog/stock.price.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:11:51.553770 neon-skill-stock-1.0.1a5/locale/gl-es/regex/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-22 22:11:48.000000 neon-skill-stock-1.0.1a5/locale/gl-es/regex/company.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:11:51.545770 neon-skill-stock-1.0.1a5/locale/hu-hu/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:11:51.553770 neon-skill-stock-1.0.1a5/locale/hu-hu/dialog/
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-22 22:11:48.000000 neon-skill-stock-1.0.1a5/locale/hu-hu/dialog/not.found.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-22 22:11:48.000000 neon-skill-stock-1.0.1a5/locale/hu-hu/dialog/stock.price.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:11:51.553770 neon-skill-stock-1.0.1a5/locale/hu-hu/regex/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-22 22:11:48.000000 neon-skill-stock-1.0.1a5/locale/hu-hu/regex/company.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:11:51.545770 neon-skill-stock-1.0.1a5/locale/it-it/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:11:51.553770 neon-skill-stock-1.0.1a5/locale/it-it/dialog/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-22 22:11:48.000000 neon-skill-stock-1.0.1a5/locale/it-it/dialog/api.error.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-22 22:11:48.000000 neon-skill-stock-1.0.1a5/locale/it-it/dialog/not.found.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-22 22:11:48.000000 neon-skill-stock-1.0.1a5/locale/it-it/dialog/stock.price.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:11:51.553770 neon-skill-stock-1.0.1a5/locale/it-it/regex/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-22 22:11:48.000000 neon-skill-stock-1.0.1a5/locale/it-it/regex/company.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:11:51.545770 neon-skill-stock-1.0.1a5/locale/nl-nl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:11:51.553770 neon-skill-stock-1.0.1a5/locale/nl-nl/dialog/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-22 22:11:48.000000 neon-skill-stock-1.0.1a5/locale/nl-nl/dialog/api.error.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-22 22:11:48.000000 neon-skill-stock-1.0.1a5/locale/nl-nl/dialog/not.found.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-22 22:11:48.000000 neon-skill-stock-1.0.1a5/locale/nl-nl/dialog/stock.price.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:11:51.553770 neon-skill-stock-1.0.1a5/locale/nl-nl/regex/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-22 22:11:48.000000 neon-skill-stock-1.0.1a5/locale/nl-nl/regex/company.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:11:51.545770 neon-skill-stock-1.0.1a5/locale/pt-br/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:11:51.557770 neon-skill-stock-1.0.1a5/locale/pt-br/dialog/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-22 22:11:48.000000 neon-skill-stock-1.0.1a5/locale/pt-br/dialog/api.error.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-22 22:11:48.000000 neon-skill-stock-1.0.1a5/locale/pt-br/dialog/not.found.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-22 22:11:48.000000 neon-skill-stock-1.0.1a5/locale/pt-br/dialog/stock.price.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:11:51.557770 neon-skill-stock-1.0.1a5/locale/pt-br/regex/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-22 22:11:48.000000 neon-skill-stock-1.0.1a5/locale/pt-br/regex/company.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:11:51.549770 neon-skill-stock-1.0.1a5/locale/ru-ru/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:11:51.557770 neon-skill-stock-1.0.1a5/locale/ru-ru/dialog/
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-22 22:11:48.000000 neon-skill-stock-1.0.1a5/locale/ru-ru/dialog/not.found.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-05-22 22:11:48.000000 neon-skill-stock-1.0.1a5/locale/ru-ru/dialog/stock.price.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:11:51.557770 neon-skill-stock-1.0.1a5/locale/ru-ru/regex/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-22 22:11:48.000000 neon-skill-stock-1.0.1a5/locale/ru-ru/regex/company.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:11:51.549770 neon-skill-stock-1.0.1a5/locale/sv-se/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:11:51.557770 neon-skill-stock-1.0.1a5/locale/sv-se/dialog/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-22 22:11:48.000000 neon-skill-stock-1.0.1a5/locale/sv-se/dialog/api.error.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-22 22:11:48.000000 neon-skill-stock-1.0.1a5/locale/sv-se/dialog/not.found.dialog
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-22 22:11:48.000000 neon-skill-stock-1.0.1a5/locale/sv-se/dialog/stock.price.dialog
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:11:51.557770 neon-skill-stock-1.0.1a5/locale/sv-se/regex/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-22 22:11:48.000000 neon-skill-stock-1.0.1a5/locale/sv-se/regex/company.rx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:11:51.557770 neon-skill-stock-1.0.1a5/neon_skill_stock.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-05-22 22:11:51.000000 neon-skill-stock-1.0.1a5/neon_skill_stock.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2142 2024-05-22 22:11:51.000000 neon-skill-stock-1.0.1a5/neon_skill_stock.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 22:11:51.000000 neon-skill-stock-1.0.1a5/neon_skill_stock.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-22 22:11:51.000000 neon-skill-stock-1.0.1a5/neon_skill_stock.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-22 22:11:51.000000 neon-skill-stock-1.0.1a5/neon_skill_stock.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-22 22:11:51.000000 neon-skill-stock-1.0.1a5/neon_skill_stock.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 22:11:51.557770 neon-skill-stock-1.0.1a5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4504 2024-05-22 22:11:48.000000 neon-skill-stock-1.0.1a5/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-22 22:11:48.000000 neon-skill-stock-1.0.1a5/skill.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:11:51.557770 neon-skill-stock-1.0.1a5/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     4187 2024-05-22 22:11:48.000000 neon-skill-stock-1.0.1a5/test/test_skill.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 22:11:51.557770 neon-skill-stock-1.0.1a5/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-22 22:11:48.000000 neon-skill-stock-1.0.1a5/ui/Stock.qml
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-22 22:11:48.000000 neon-skill-stock-1.0.1a5/ui/qmldir
+-rw-r--r--   0 runner    (1001) docker     (127)     1856 2024-05-22 22:11:48.000000 neon-skill-stock-1.0.1a5/version.py
```

### Comparing `neon-skill-stock-1.0.1a4/LICENSE` & `neon-skill-stock-1.0.1a5/LICENSE`

 * *Files identical despite different names*

### Comparing `neon-skill-stock-1.0.1a4/LICENSE.md` & `neon-skill-stock-1.0.1a5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-skill-stock-1.0.1a4/PKG-INFO` & `neon-skill-stock-1.0.1a5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-stock
-Version: 1.0.1a4
+Version: 1.0.1a5
 Home-page: https://github.com/NeonGeckoCom/skill-stock
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
```

### Comparing `neon-skill-stock-1.0.1a4/README.md` & `neon-skill-stock-1.0.1a5/README.md`

 * *Files identical despite different names*

### Comparing `neon-skill-stock-1.0.1a4/__init__.py` & `neon-skill-stock-1.0.1a5/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -22,26 +22,28 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-from typing import Optional
-from neon_utils.skills.neon_skill import NeonSkill
+import re
+
+from typing import Optional, Tuple
 from neon_utils.hana_utils import request_backend
 from ovos_utils import classproperty
 from ovos_utils.log import LOG
 from ovos_utils.process_utils import RuntimeRequirements
 from ovos_workshop.decorators import intent_handler
+from ovos_workshop.skills.common_query_skill import CommonQuerySkill, CQSMatchLevel
 
 
-class StockSkill(NeonSkill):
+class StockSkill(CommonQuerySkill):
     def __init__(self, **kwargs):
-        NeonSkill.__init__(self, **kwargs)
+        CommonQuerySkill.__init__(self, **kwargs)
         self.preferred_market = "United States"
         self.translate_co = {"3 m": "mmm",
                              "3m": "mmm",
                              "coca cola": "ko",
                              "coca-cola": "ko",
                              "google": "goog",
                              "exxonmobil": "xom"}
@@ -94,25 +96,60 @@
                 self.gui["title"] = company
                 self.gui["text"] = f"${quote}"
                 self.gui.show_page("Stock.qml")
         except Exception as e:
             LOG.exception(e)
             self.speak_dialog("not.found", data={'company': company})
 
+    def CQS_match_query_phrase(self, phrase: str):
+        company = self._extract_company(phrase)
+        if not company:
+            LOG.debug(f"no company found in {phrase}")
+            return None
+        try:
+            match = self._search_company(company)
+        except Exception as e:
+            LOG.exception(e)
+            return None
+        if not match:
+            LOG.info(f"not a company: {company}")
+            return None
+        company = match.get("2. name")
+        symbol = match.get("1. symbol")
+        try:
+            quote = self._get_stock_price(symbol)
+        except Exception as e:
+            LOG.exception(e)
+            return None
+
+        response = {'symbol': symbol,
+                    'company': company,
+                    'price': quote,
+                    'provider': "Alpha Vantage"}
+        dialog = self.dialog_renderer.render("stock.price",
+                                             response)
+        callback_data = {"company": company, "quote": quote, "answer": dialog}
+        return phrase, CQSMatchLevel.EXACT, dialog, callback_data
+
+    def CQS_action(self, phrase: str, callback_data: dict):
+        self.gui["title"] = callback_data.get("company")
+        self.gui["text"] = f"${callback_data.get('quote')}"
+        self.gui.show_page("Stock")
+
     def _search_company(self, company: str) -> Optional[dict]:
         """
         Find a traded company by name
         :param company: Company to search
         :return: dict company data: `symbol`, `name`, `region`, `currency`
         """
         kwargs = {"region": self.preferred_market,
                   "company": company}
         stocks = request_backend("/proxy/stock/symbol", kwargs)
         LOG.info(f"stocks={stocks}")
-        if stocks:
+        if stocks and stocks.get("bestMatches"):
             return stocks["bestMatches"][0]
         else:
             return None
 
     @staticmethod
     def _get_stock_price(symbol: str):
         """
@@ -121,7 +158,24 @@
         :return:
         """
         stock_data = request_backend("/proxy/stock/quote", {"symbol": symbol})
         price = stock_data.get("Global Quote", {}).get("05. price")
         if not price:
             return None
         return str(round(float(price), 2))
+
+    def _extract_company(self, utt):
+        rx_file = self.find_resource('company.rx', 'regex')
+        LOG.debug(f"Resolved: {rx_file}")
+        if rx_file:
+            with open(rx_file) as f:
+                for pat in f.read().splitlines():
+                    pat = pat.strip()
+                    if pat and pat[0] == "#":
+                        continue
+                    res = re.search(pat, utt)
+                    if res:
+                        try:
+                            return res.group("Company")
+                        except IndexError:
+                            pass
+        return None
```

### Comparing `neon-skill-stock-1.0.1a4/neon_skill_stock.egg-info/PKG-INFO` & `neon-skill-stock-1.0.1a5/neon_skill_stock.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-skill-stock
-Version: 1.0.1a4
+Version: 1.0.1a5
 Home-page: https://github.com/NeonGeckoCom/skill-stock
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3-Clause
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
```

### Comparing `neon-skill-stock-1.0.1a4/neon_skill_stock.egg-info/SOURCES.txt` & `neon-skill-stock-1.0.1a5/neon_skill_stock.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 locale/el-gr/dialog/not.found.dialog
 locale/el-gr/dialog/stock.price.dialog
 locale/el-gr/regex/company.rx
 locale/en-us/dialog/api.error.dialog
 locale/en-us/dialog/not.found.dialog
 locale/en-us/dialog/stock.price.dialog
 locale/en-us/intent/stock_price.intent
+locale/en-us/regex/company.rx
 locale/es-es/dialog/api.error.dialog
 locale/es-es/dialog/not.found.dialog
 locale/es-es/dialog/stock.price.dialog
 locale/es-es/regex/company.rx
 locale/fr-fr/dialog/api.error.dialog
 locale/fr-fr/dialog/not.found.dialog
 locale/fr-fr/dialog/stock.price.dialog
```

### Comparing `neon-skill-stock-1.0.1a4/setup.py` & `neon-skill-stock-1.0.1a5/setup.py`

 * *Files identical despite different names*

### Comparing `neon-skill-stock-1.0.1a4/skill.json` & `neon-skill-stock-1.0.1a5/skill.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9981060606060607%*

 * *Differences: {"'requirements'": "{'python': {insert: [(2, 'ovos-workshop~=0.0.15,>=0.0.16a29')], delete: [2]}}"}*

```diff
@@ -28,15 +28,15 @@
         "arm64",
         "arm"
     ],
     "requirements": {
         "python": [
             "neon-utils~=1.9",
             "ovos-utils~=0.0, >=0.0.28",
-            "ovos-workshop~=0.0.15"
+            "ovos-workshop~=0.0.15,>=0.0.16a29"
         ],
         "skill": [],
         "system": {}
     },
     "short_description": "This skill provides stock values.",
     "skillname": "skill-stock",
     "summary": "This skill provides stock values.",
```

### Comparing `neon-skill-stock-1.0.1a4/test/test_skill.py` & `neon-skill-stock-1.0.1a5/test/test_skill.py`

 * *Files 22% similar despite different names*

```diff
@@ -22,26 +22,26 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
+import os
 import unittest
 
 from ovos_bus_client import Message
 from neon_minerva.tests.skill_unit_test_base import SkillTestCase
 
+os.environ["TEST_SKILL_ENTRYPOINT"] = "skill-stock.neongeckocom"
+
 
 class TestSkillMethods(SkillTestCase):
     def test_00_skill_init(self):
         # Test any parameters expected to be set in init or initialize methods
-        from neon_utils.skills.neon_skill import NeonSkill
-
-        self.assertIsInstance(self.skill, NeonSkill)
         self.assertIsInstance(self.skill.translate_co, dict)
         self.assertIsInstance(self.skill.preferred_market, str)
 
     def test_handle_stock_price(self):
         message = Message("test", {"company": "3m"})
         self.skill.handle_stock_price(message)
         self.skill.speak_dialog.assert_called_once()
@@ -50,29 +50,39 @@
         data = args[1]["data"]
         self.assertEqual(data["symbol"], "MMM")
         self.assertEqual(data["company"], "3M Company")
         self.assertIsInstance(float(data["price"]), float)
         self.assertEqual(data["provider"], "Alpha Vantage")
         self.assertIsInstance(args[1]["data"], dict)
 
-        message = Message("test", {"company": "microsoft"})
-        self.skill.handle_stock_price(message)
-        args = self.skill.speak_dialog.call_args
-        self.assertEqual(args[0][0], "stock.price")
-        data = args[1]["data"]
-        self.assertEqual(data["symbol"], "MSFT")
-        self.assertEqual(data["company"], "Microsoft Corporation")
-        self.assertIsInstance(float(data["price"]), float)
-        self.assertEqual(data["provider"], "Alpha Vantage")
-        self.assertIsInstance(args[1]["data"], dict)
+        # message = Message("test", {"company": "microsoft"})
+        # self.skill.handle_stock_price(message)
+        # args = self.skill.speak_dialog.call_args
+        # self.assertEqual(args[0][0], "stock.price")
+        # data = args[1]["data"]
+        # self.assertEqual(data["symbol"], "MSFT")
+        # self.assertEqual(data["company"], "Microsoft Corporation")
+        # self.assertIsInstance(float(data["price"]), float)
+        # self.assertEqual(data["provider"], "Alpha Vantage")
+        # self.assertIsInstance(args[1]["data"], dict)
 
     def test_search_company(self):
         # TODO
         pass
 
     def test_get_stock_price(self):
         # TODO
         pass
 
+    def test_extract_company(self):
+        test_ms = "what is microsoft trading at"
+        test_google = "what is the stock price for google"
+        test_apple = "what is apple stock valued at"
+        test_amazon = "tell me about amazon stock"
+        self.assertEqual(self.skill._extract_company(test_ms), "microsoft")
+        self.assertEqual(self.skill._extract_company(test_google), "google")
+        self.assertEqual(self.skill._extract_company(test_apple), "apple")
+        self.assertEqual(self.skill._extract_company(test_amazon), "amazon")
+
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `neon-skill-stock-1.0.1a4/ui/Stock.qml` & `neon-skill-stock-1.0.1a5/ui/Stock.qml`

 * *Files identical despite different names*

### Comparing `neon-skill-stock-1.0.1a4/version.py` & `neon-skill-stock-1.0.1a5/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA,
 # OR PROFITS;  OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-__version__ = "1.0.1a4"
+__version__ = "1.0.1a5"
```

