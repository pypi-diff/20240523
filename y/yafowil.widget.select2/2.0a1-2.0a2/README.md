# Comparing `tmp/yafowil.widget.select2-2.0a1.tar.gz` & `tmp/yafowil_widget_select2-2.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yafowil.widget.select2-2.0a1.tar", last modified: Mon May 15 12:51:11 2023, max compression
+gzip compressed data, was "yafowil_widget_select2-2.0a2.tar", last modified: Thu May 23 14:25:09 2024, max compression
```

## Comparing `yafowil.widget.select2-2.0a1.tar` & `yafowil_widget_select2-2.0a2.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:51:11.554625 yafowil.widget.select2-2.0a1/
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1028 2023-05-15 12:46:13.000000 yafowil.widget.select2-2.0a1/CHANGES.rst
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1403 2022-10-30 11:16:34.000000 yafowil.widget.select2-2.0a1/LICENSE.rst
--rw-r--r--   0 rnix      (1000) rnix      (1000)       72 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/MANIFEST.in
--rw-r--r--   0 rnix      (1000) rnix      (1000)     4858 2023-05-15 12:51:11.554625 yafowil.widget.select2-2.0a1/PKG-INFO
--rw-r--r--   0 rnix      (1000) rnix      (1000)      708 2023-05-15 12:50:43.000000 yafowil.widget.select2-2.0a1/README.rst
--rw-r--r--   0 rnix      (1000) rnix      (1000)       38 2023-05-15 12:51:11.554625 yafowil.widget.select2-2.0a1/setup.cfg
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1731 2023-05-15 12:46:13.000000 yafowil.widget.select2-2.0a1/setup.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:51:11.550625 yafowil.widget.select2-2.0a1/src/
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:51:11.550625 yafowil.widget.select2-2.0a1/src/yafowil/
--rw-r--r--   0 rnix      (1000) rnix      (1000)       56 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/__init__.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:51:11.550625 yafowil.widget.select2-2.0a1/src/yafowil/widget/
--rw-r--r--   0 rnix      (1000) rnix      (1000)       56 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/__init__.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:51:11.550625 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/
--rw-r--r--   0 rnix      (1000) rnix      (1000)     2282 2022-10-30 11:16:34.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/__init__.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)     8299 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/example.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:51:11.550625 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:51:11.554625 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/
--rw-r--r--   0 rnix      (1000) rnix      (1000)      939 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/LICENSE
--rw-r--r--   0 rnix      (1000) rnix      (1000)     4174 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/README.md
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1732 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/component.json
--rwxr-xr-x   0 rnix      (1000) rnix      (1000)     1490 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/release.sh
--rw-r--r--   0 rnix      (1000) rnix      (1000)     3347 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2-bootstrap.css
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1849 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2-spinner.gif
--rw-r--r--   0 rnix      (1000) rnix      (1000)    19336 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2.css
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1030 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2.jquery.json
--rw-r--r--   0 rnix      (1000) rnix      (1000)   146080 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)    65514 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2.min.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)      613 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2.png
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1318 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_ar.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)      940 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_az.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1019 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_bg.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)      890 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_ca.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1929 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_cs.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)      791 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_da.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)      953 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_de.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1066 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_el.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1040 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_en.js.template
--rw-r--r--   0 rnix      (1000) rnix      (1000)      823 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_es.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)      824 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_et.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1251 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_eu.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1145 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_fa.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)      878 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_fi.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1015 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_fr.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1277 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_gl.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)      823 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_he.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)      940 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_hr.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)      740 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_hu.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)      829 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_id.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)      793 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_is.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)      804 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_it.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)      750 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_ja.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1016 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_ka.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)      809 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_ko.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1082 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_lt.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)      937 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_lv.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1002 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_mk.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)      774 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_ms.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)      789 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_nl.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)      789 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_no.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1078 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_pl.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)      807 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_pt-BR.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)      823 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_pt-PT.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)      840 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_ro.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)      996 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_rs.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1109 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_ru.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1858 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_sk.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)      785 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_sv.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1001 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_th.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)      769 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_tr.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1353 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_uk.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)      897 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_vi.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)      694 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_zh-CN.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)      706 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_zh-TW.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)      845 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2x2.png
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1771 2022-10-30 11:16:34.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/widget.css
--rw-r--r--   0 rnix      (1000) rnix      (1000)     4110 2023-03-13 08:17:16.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/widget.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)     1597 2023-03-13 08:17:16.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/widget.min.js
--rw-r--r--   0 rnix      (1000) rnix      (1000)    11732 2022-10-30 11:16:34.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/tests.py
--rw-r--r--   0 rnix      (1000) rnix      (1000)    22033 2022-04-02 11:07:47.000000 yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/widget.py
-drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2023-05-15 12:51:11.550625 yafowil.widget.select2-2.0a1/src/yafowil.widget.select2.egg-info/
--rw-r--r--   0 rnix      (1000) rnix      (1000)     4858 2023-05-15 12:51:11.000000 yafowil.widget.select2-2.0a1/src/yafowil.widget.select2.egg-info/PKG-INFO
--rw-r--r--   0 rnix      (1000) rnix      (1000)     4517 2023-05-15 12:51:11.000000 yafowil.widget.select2-2.0a1/src/yafowil.widget.select2.egg-info/SOURCES.txt
--rw-r--r--   0 rnix      (1000) rnix      (1000)        1 2023-05-15 12:51:11.000000 yafowil.widget.select2-2.0a1/src/yafowil.widget.select2.egg-info/dependency_links.txt
--rw-r--r--   0 rnix      (1000) rnix      (1000)      130 2023-05-15 12:51:11.000000 yafowil.widget.select2-2.0a1/src/yafowil.widget.select2.egg-info/entry_points.txt
--rw-r--r--   0 rnix      (1000) rnix      (1000)       23 2023-05-15 12:51:11.000000 yafowil.widget.select2-2.0a1/src/yafowil.widget.select2.egg-info/namespace_packages.txt
--rw-r--r--   0 rnix      (1000) rnix      (1000)        1 2022-04-02 11:08:00.000000 yafowil.widget.select2-2.0a1/src/yafowil.widget.select2.egg-info/not-zip-safe
--rw-r--r--   0 rnix      (1000) rnix      (1000)       55 2023-05-15 12:51:11.000000 yafowil.widget.select2-2.0a1/src/yafowil.widget.select2.egg-info/requires.txt
--rw-r--r--   0 rnix      (1000) rnix      (1000)        8 2023-05-15 12:51:11.000000 yafowil.widget.select2-2.0a1/src/yafowil.widget.select2.egg-info/top_level.txt
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-05-23 14:25:09.412974 yafowil_widget_select2-2.0a2/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1104 2024-05-23 14:25:09.000000 yafowil_widget_select2-2.0a2/CHANGES.rst
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1403 2024-05-23 14:25:09.000000 yafowil_widget_select2-2.0a2/LICENSE.rst
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       72 2024-05-23 14:25:09.000000 yafowil_widget_select2-2.0a2/MANIFEST.in
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     4102 2024-05-23 14:25:09.412974 yafowil_widget_select2-2.0a2/PKG-INFO
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      708 2024-05-23 14:25:09.000000 yafowil_widget_select2-2.0a2/README.rst
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       38 2024-05-23 14:25:09.412974 yafowil_widget_select2-2.0a2/setup.cfg
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1731 2024-05-23 14:25:09.000000 yafowil_widget_select2-2.0a2/setup.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-05-23 14:25:09.404975 yafowil_widget_select2-2.0a2/src/
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-05-23 14:25:09.404975 yafowil_widget_select2-2.0a2/src/yafowil/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       56 2024-05-23 14:25:09.000000 yafowil_widget_select2-2.0a2/src/yafowil/__init__.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-05-23 14:25:09.404975 yafowil_widget_select2-2.0a2/src/yafowil/widget/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       56 2024-05-23 14:25:09.000000 yafowil_widget_select2-2.0a2/src/yafowil/widget/__init__.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-05-23 14:25:09.404975 yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     2282 2024-05-23 14:25:09.000000 yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/__init__.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     8299 2024-05-23 14:25:09.000000 yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/example.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-05-23 14:25:09.404975 yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-05-23 14:25:09.412974 yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      939 2024-05-23 14:25:09.000000 yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/LICENSE
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     4174 2024-05-23 14:25:09.000000 yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/README.md
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1732 2024-05-23 14:25:09.000000 yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/component.json
+-rwxr-xr-x   0 rnix      (1000) rnix      (1000)     1490 2024-05-23 14:25:09.000000 yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/release.sh
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     3347 2024-05-23 14:25:09.000000 yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/select2-bootstrap.css
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1849 2024-05-23 14:25:09.000000 yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/select2-spinner.gif
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    19336 2024-05-23 14:25:09.000000 yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/select2.css
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1030 2024-05-23 14:25:09.000000 yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/select2.jquery.json
+-rw-r--r--   0 rnix      (1000) rnix      (1000)   146080 2024-05-23 14:25:09.000000 yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/select2.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    65514 2024-05-23 14:25:09.000000 yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/select2.min.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      613 2024-05-23 14:25:09.000000 yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/select2.png
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1318 2024-05-23 14:25:09.000000 yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/select2_locale_ar.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      940 2024-05-23 14:25:09.000000 yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/select2_locale_az.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1019 2024-05-23 14:25:09.000000 yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/select2_locale_bg.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      890 2024-05-23 14:25:09.000000 yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/select2_locale_ca.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1929 2024-05-23 14:25:09.000000 yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/select2_locale_cs.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      791 2024-05-23 14:25:09.000000 yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/select2_locale_da.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      953 2024-05-23 14:25:09.000000 yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/select2_locale_de.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1066 2024-05-23 14:25:09.000000 yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/select2_locale_el.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1040 2024-05-23 14:25:09.000000 yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/select2_locale_en.js.template
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      823 2024-05-23 14:25:09.000000 yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/select2_locale_es.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      824 2024-05-23 14:25:09.000000 yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/select2_locale_et.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1251 2024-05-23 14:25:09.000000 yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/select2_locale_eu.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1145 2024-05-23 14:25:09.000000 yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/select2_locale_fa.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      878 2024-05-23 14:25:09.000000 yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/select2_locale_fi.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1015 2024-05-23 14:25:09.000000 yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/select2_locale_fr.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1277 2024-05-23 14:25:09.000000 yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/select2_locale_gl.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      823 2024-05-23 14:25:09.000000 yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/select2_locale_he.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      940 2024-05-23 14:25:09.000000 yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/select2_locale_hr.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      740 2024-05-23 14:25:09.000000 yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/select2_locale_hu.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      829 2024-05-23 14:25:09.000000 yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/select2_locale_id.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      793 2024-05-23 14:25:09.000000 yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/select2_locale_is.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      804 2024-05-23 14:25:09.000000 yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/select2_locale_it.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      750 2024-05-23 14:25:09.000000 yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/select2_locale_ja.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1016 2024-05-23 14:25:09.000000 yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/select2_locale_ka.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      809 2024-05-23 14:25:09.000000 yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/select2_locale_ko.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1082 2024-05-23 14:25:09.000000 yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/select2_locale_lt.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      937 2024-05-23 14:25:09.000000 yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/select2_locale_lv.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1002 2024-05-23 14:25:09.000000 yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/select2_locale_mk.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      774 2024-05-23 14:25:09.000000 yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/select2_locale_ms.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      789 2024-05-23 14:25:09.000000 yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/select2_locale_nl.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      789 2024-05-23 14:25:09.000000 yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/select2_locale_no.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1078 2024-05-23 14:25:09.000000 yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/select2_locale_pl.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      807 2024-05-23 14:25:09.000000 yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/select2_locale_pt-BR.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      823 2024-05-23 14:25:09.000000 yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/select2_locale_pt-PT.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      840 2024-05-23 14:25:09.000000 yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/select2_locale_ro.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      996 2024-05-23 14:25:09.000000 yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/select2_locale_rs.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1109 2024-05-23 14:25:09.000000 yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/select2_locale_ru.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1858 2024-05-23 14:25:09.000000 yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/select2_locale_sk.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      785 2024-05-23 14:25:09.000000 yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/select2_locale_sv.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1001 2024-05-23 14:25:09.000000 yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/select2_locale_th.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      769 2024-05-23 14:25:09.000000 yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/select2_locale_tr.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1353 2024-05-23 14:25:09.000000 yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/select2_locale_uk.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      897 2024-05-23 14:25:09.000000 yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/select2_locale_vi.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      694 2024-05-23 14:25:09.000000 yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/select2_locale_zh-CN.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      706 2024-05-23 14:25:09.000000 yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/select2_locale_zh-TW.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      845 2024-05-23 14:25:09.000000 yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/select2x2.png
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1771 2024-05-23 14:25:09.000000 yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/widget.css
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     4110 2024-05-23 14:25:09.000000 yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/widget.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     1597 2024-05-23 14:25:09.000000 yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/widget.min.js
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    11732 2024-05-23 14:25:09.000000 yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/tests.py
+-rw-r--r--   0 rnix      (1000) rnix      (1000)    22033 2024-05-23 14:25:09.000000 yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/widget.py
+drwxr-xr-x   0 rnix      (1000) rnix      (1000)        0 2024-05-23 14:25:09.412974 yafowil_widget_select2-2.0a2/src/yafowil.widget.select2.egg-info/
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     4102 2024-05-23 14:25:09.000000 yafowil_widget_select2-2.0a2/src/yafowil.widget.select2.egg-info/PKG-INFO
+-rw-r--r--   0 rnix      (1000) rnix      (1000)     4517 2024-05-23 14:25:09.000000 yafowil_widget_select2-2.0a2/src/yafowil.widget.select2.egg-info/SOURCES.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)        1 2024-05-23 14:25:09.000000 yafowil_widget_select2-2.0a2/src/yafowil.widget.select2.egg-info/dependency_links.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)      113 2024-05-23 14:25:09.000000 yafowil_widget_select2-2.0a2/src/yafowil.widget.select2.egg-info/entry_points.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       23 2024-05-23 14:25:09.000000 yafowil_widget_select2-2.0a2/src/yafowil.widget.select2.egg-info/namespace_packages.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)        1 2024-05-23 14:25:09.000000 yafowil_widget_select2-2.0a2/src/yafowil.widget.select2.egg-info/not-zip-safe
+-rw-r--r--   0 rnix      (1000) rnix      (1000)       55 2024-05-23 14:25:09.000000 yafowil_widget_select2-2.0a2/src/yafowil.widget.select2.egg-info/requires.txt
+-rw-r--r--   0 rnix      (1000) rnix      (1000)        8 2024-05-23 14:25:09.000000 yafowil_widget_select2-2.0a2/src/yafowil.widget.select2.egg-info/top_level.txt
```

### Comparing `yafowil.widget.select2-2.0a1/CHANGES.rst` & `yafowil_widget_select2-2.0a2/CHANGES.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 Changes
 =======
 
+2.0a2 (2024-05-23)
+------------------
+
+- Fix deprecated imports.
+  [rnix]
+
+
 2.0a1 (2023-05-15)
 ------------------
 
 - Add ``webresource`` support.
   [rnix]
 
 - Extend JS by ``select2_on_array_add``, ``register_array_subscribers``
```

### Comparing `yafowil.widget.select2-2.0a1/LICENSE.rst` & `yafowil_widget_select2-2.0a2/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-2.0a1/README.rst` & `yafowil_widget_select2-2.0a2/README.rst`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-2.0a1/setup.py` & `yafowil_widget_select2-2.0a2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 def read_file(name):
     with open(os.path.join(os.path.dirname(__file__), name)) as f:
         return f.read()
 
 
-version = '2.0a1'
+version = '2.0a2'
 shortdesc = 'Select2 widget for YAFOWIL'
 longdesc = '\n\n'.join([read_file(name) for name in [
     'README.rst',
     'CHANGES.rst',
     'LICENSE.rst'
 ]])
```

### Comparing `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/__init__.py` & `yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/__init__.py`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/example.py` & `yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/example.py`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/LICENSE` & `yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/LICENSE`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/README.md` & `yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/README.md`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/component.json` & `yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/component.json`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/release.sh` & `yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/release.sh`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2-bootstrap.css` & `yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/select2-bootstrap.css`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2-spinner.gif` & `yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/select2-spinner.gif`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2.css` & `yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/select2.css`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2.jquery.json` & `yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/select2.jquery.json`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2.js` & `yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/select2.js`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2.min.js` & `yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/select2.min.js`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2.png` & `yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/select2.png`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_ar.js` & `yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/select2_locale_ar.js`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_az.js` & `yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/select2_locale_az.js`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_bg.js` & `yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/select2_locale_bg.js`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_ca.js` & `yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/select2_locale_ca.js`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_cs.js` & `yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/select2_locale_cs.js`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_da.js` & `yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/select2_locale_da.js`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_de.js` & `yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/select2_locale_de.js`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_el.js` & `yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/select2_locale_el.js`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_en.js.template` & `yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/select2_locale_en.js.template`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_es.js` & `yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/select2_locale_es.js`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_et.js` & `yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/select2_locale_et.js`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_eu.js` & `yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/select2_locale_eu.js`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_fa.js` & `yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/select2_locale_fa.js`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_fi.js` & `yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/select2_locale_fi.js`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_fr.js` & `yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/select2_locale_fr.js`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_gl.js` & `yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/select2_locale_gl.js`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_he.js` & `yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/select2_locale_he.js`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_hr.js` & `yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/select2_locale_hr.js`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_hu.js` & `yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/select2_locale_hu.js`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_id.js` & `yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/select2_locale_id.js`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_is.js` & `yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/select2_locale_is.js`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_it.js` & `yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/select2_locale_it.js`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_ja.js` & `yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/select2_locale_ja.js`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_ka.js` & `yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/select2_locale_ka.js`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_ko.js` & `yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/select2_locale_ko.js`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_lt.js` & `yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/select2_locale_lt.js`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_lv.js` & `yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/select2_locale_lv.js`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_mk.js` & `yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/select2_locale_mk.js`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_ms.js` & `yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/select2_locale_ms.js`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_nl.js` & `yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/select2_locale_nl.js`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_no.js` & `yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/select2_locale_no.js`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_pl.js` & `yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/select2_locale_pl.js`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_pt-BR.js` & `yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/select2_locale_pt-BR.js`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_pt-PT.js` & `yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/select2_locale_pt-PT.js`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_ro.js` & `yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/select2_locale_ro.js`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_rs.js` & `yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/select2_locale_rs.js`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_ru.js` & `yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/select2_locale_ru.js`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_sk.js` & `yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/select2_locale_sk.js`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_sv.js` & `yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/select2_locale_sv.js`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_th.js` & `yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/select2_locale_th.js`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_tr.js` & `yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/select2_locale_tr.js`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_uk.js` & `yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/select2_locale_uk.js`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_vi.js` & `yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/select2_locale_vi.js`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_zh-CN.js` & `yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/select2_locale_zh-CN.js`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2_locale_zh-TW.js` & `yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/select2_locale_zh-TW.js`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/select2/select2x2.png` & `yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/select2/select2x2.png`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/widget.css` & `yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/widget.css`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/widget.js` & `yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/widget.js`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/resources/widget.min.js` & `yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/resources/widget.min.js`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/tests.py` & `yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/tests.py`

 * *Files identical despite different names*

### Comparing `yafowil.widget.select2-2.0a1/src/yafowil/widget/select2/widget.py` & `yafowil_widget_select2-2.0a2/src/yafowil/widget/select2/widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from collections import OrderedDict
 from node.utils import UNSET
 from yafowil.base import factory
 from yafowil.common import generic_extractor, display_proxy_renderer
 from yafowil.common import generic_required_extractor
 from yafowil.common import input_generic_renderer
-from yafowil.common import select_display_renderer
-from yafowil.common import select_edit_renderer
-from yafowil.common import select_extractor
+from yafowil.select import select_display_renderer
+from yafowil.select import select_edit_renderer
+from yafowil.select import select_extractor
 from yafowil.utils import attr_value
 from yafowil.utils import data_attrs_helper
 from yafowil.utils import managedprops
 from yafowil.utils import vocabulary
 
 
 select2_options = [
```

### Comparing `yafowil.widget.select2-2.0a1/src/yafowil.widget.select2.egg-info/SOURCES.txt` & `yafowil_widget_select2-2.0a2/src/yafowil.widget.select2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

