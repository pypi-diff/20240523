# Comparing `tmp/cubicweb-web-1.2.9.tar.gz` & `tmp/cubicweb-web-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cubicweb-web-1.2.9.tar", last modified: Wed Feb  7 09:13:18 2024, max compression
+gzip compressed data, was "cubicweb-web-1.3.0.tar", last modified: Thu May 23 10:07:06 2024, max compression
```

## Comparing `cubicweb-web-1.2.9.tar` & `cubicweb-web-1.3.0.tar`

### file list

```diff
@@ -1,466 +1,466 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 09:13:18.538511 cubicweb-web-1.2.9/
--rw-rw-rw-   0 root         (0) root         (0)     1234 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1272 2024-02-07 09:13:18.534511 cubicweb-web-1.2.9/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      785 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 09:13:18.310508 cubicweb-web-1.2.9/cubicweb_web/
--rw-rw-rw-   0 root         (0) root         (0)     2821 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      661 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)     3696 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/_exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     4320 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/action.py
--rw-rw-rw-   0 root         (0) root         (0)    21197 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/application.py
--rw-rw-rw-   0 root         (0) root         (0)     6976 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/box.py
--rw-rw-rw-   0 root         (0) root         (0)    21418 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/bwcompat.py
--rw-rw-rw-   0 root         (0) root         (0)     3939 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/captcha.py
--rw-rw-rw-   0 root         (0) root         (0)     4834 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/ccplugin.py
--rw-rw-rw-   0 root         (0) root         (0)    29066 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/component.py
--rw-rw-rw-   0 root         (0) root         (0)     8635 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/controller.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 09:13:18.402509 cubicweb-web-1.2.9/cubicweb_web/data/
--rw-rw-rw-   0 root         (0) root         (0)      414 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/accessories-text-editor.png
--rw-rw-rw-   0 root         (0) root         (0)      190 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/add_button.png
--rw-rw-rw-   0 root         (0) root         (0)       54 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/asc.gif
--rw-rw-rw-   0 root         (0) root         (0)      579 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/banner.png
--rw-rw-rw-   0 root         (0) root         (0)       64 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/bg.gif
--rw-rw-rw-   0 root         (0) root         (0)      112 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/bg_trame_grise.png
--rw-rw-rw-   0 root         (0) root         (0)      719 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/black-check.png
--rw-rw-rw-   0 root         (0) root         (0)      526 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/black-uncheck.png
--rw-rw-rw-   0 root         (0) root         (0)      113 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/bullet.png
--rw-rw-rw-   0 root         (0) root         (0)      110 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/bullet_orange.png
--rw-rw-rw-   0 root         (0) root         (0)      110 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/button.png
--rw-rw-rw-   0 root         (0) root         (0)       75 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/calendar.gif
--rw-rw-rw-   0 root         (0) root         (0)      655 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/cancel.png
--rw-rw-rw-   0 root         (0) root         (0)      112 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/contextFreeBoxHeader.png
--rw-rw-rw-   0 root         (0) root         (0)      128 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/contextualBoxHeader.png
--rw-rw-rw-   0 root         (0) root         (0)      414 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/critical.png
--rw-rw-rw-   0 root         (0) root         (0)      924 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/cubicweb.acl.css
--rw-rw-rw-   0 root         (0) root         (0)     3589 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/cubicweb.ajax.box.js
--rw-rw-rw-   0 root         (0) root         (0)    24133 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/cubicweb.ajax.js
--rw-rw-rw-   0 root         (0) root         (0)     7895 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/cubicweb.calendar.css
--rw-rw-rw-   0 root         (0) root         (0)     9665 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/cubicweb.calendar.js
--rw-rw-rw-   0 root         (0) root         (0)     1179 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/cubicweb.calendar_popup.css
--rw-rw-rw-   0 root         (0) root         (0)      564 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/cubicweb.compat.js
--rw-rw-rw-   0 root         (0) root         (0)    18494 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/cubicweb.css
--rw-rw-rw-   0 root         (0) root         (0)    18779 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/cubicweb.edition.js
--rw-rw-rw-   0 root         (0) root         (0)     2019 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/cubicweb.facets.css
--rw-rw-rw-   0 root         (0) root         (0)    12099 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/cubicweb.facets.js
--rw-rw-rw-   0 root         (0) root         (0)     1488 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/cubicweb.fckcwconfig-full.js
--rw-rw-rw-   0 root         (0) root         (0)      592 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/cubicweb.fckcwconfig.js
--rw-rw-rw-   0 root         (0) root         (0)     1505 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/cubicweb.flot.js
--rw-rw-rw-   0 root         (0) root         (0)     3811 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/cubicweb.form.css
--rw-rw-rw-   0 root         (0) root         (0)     1408 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/cubicweb.html_tree.css
--rw-rw-rw-   0 root         (0) root         (0)     4595 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/cubicweb.htmlhelpers.js
--rw-rw-rw-   0 root         (0) root         (0)      550 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/cubicweb.ie.css
--rw-rw-rw-   0 root         (0) root         (0)     1318 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/cubicweb.image.js
--rw-rw-rw-   0 root         (0) root         (0)    12621 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/cubicweb.js
--rw-rw-rw-   0 root         (0) root         (0)     1975 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/cubicweb.log.css
--rw-rw-rw-   0 root         (0) root         (0)      384 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/cubicweb.log.js
--rw-rw-rw-   0 root         (0) root         (0)     1756 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/cubicweb.login.css
--rw-rw-rw-   0 root         (0) root         (0)      331 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/cubicweb.manageview.css
--rw-rw-rw-   0 root         (0) root         (0)    16860 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/cubicweb.pictograms.css
--rw-rw-rw-   0 root         (0) root         (0)     1671 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/cubicweb.preferences.css
--rw-rw-rw-   0 root         (0) root         (0)     4559 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/cubicweb.preferences.js
--rw-rw-rw-   0 root         (0) root         (0)      189 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/cubicweb.print.css
--rw-rw-rw-   0 root         (0) root         (0)     7718 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/cubicweb.python.js
--rw-rw-rw-   0 root         (0) root         (0)     2754 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/cubicweb.reledit.js
--rw-rw-rw-   0 root         (0) root         (0)     1930 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/cubicweb.schema.css
--rw-rw-rw-   0 root         (0) root         (0)      756 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/cubicweb.suggest.css
--rw-rw-rw-   0 root         (0) root         (0)      350 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/cubicweb.tablesorter.css
--rw-rw-rw-   0 root         (0) root         (0)      822 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/cubicweb.tableview.css
--rw-rw-rw-   0 root         (0) root         (0)     2901 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/cubicweb.timetable.css
--rw-rw-rw-   0 root         (0) root         (0)       89 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/cubicweb.treeview.css
--rw-rw-rw-   0 root         (0) root         (0)    19668 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/cubicweb.widgets.js
--rw-rw-rw-   0 root         (0) root         (0)       54 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/desc.gif
--rw-rw-rw-   0 root         (0) root         (0)      860 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/download.gif
--rw-rw-rw-   0 root         (0) root         (0)      973 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/dublincore-button.png
--rw-rw-rw-   0 root         (0) root         (0)     2179 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/dublincore-icon.png
--rw-rw-rw-   0 root         (0) root         (0)    67968 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/entypo.eot
--rw-rw-rw-   0 root         (0) root         (0)    97203 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/entypo.svg
--rw-rw-rw-   0 root         (0) root         (0)    67680 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/entypo.ttf
--rw-rw-rw-   0 root         (0) root         (0)    42064 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/entypo.woff
--rw-rw-rw-   0 root         (0) root         (0)      930 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/error.png
--rw-rw-rw-   0 root         (0) root         (0)    42086 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/excanvas.js
--rw-rw-rw-   0 root         (0) root         (0)    34494 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/favicon.ico
--rw-rw-rw-   0 root         (0) root         (0)     5468 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/feed-icon.png
--rw-rw-rw-   0 root         (0) root         (0)      715 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/feed-icon16x16.png
--rw-rw-rw-   0 root         (0) root         (0)     1646 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/feed-icon32x32.png
--rw-rw-rw-   0 root         (0) root         (0)      110 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/file.gif
--rw-rw-rw-   0 root         (0) root         (0)      105 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/folder-closed.gif
--rw-rw-rw-   0 root         (0) root         (0)      106 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/folder.gif
--rw-rw-rw-   0 root         (0) root         (0)    11147 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/fullcalendar.css
--rw-rw-rw-   0 root         (0) root         (0)   151629 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/fullcalendar.js
--rw-rw-rw-   0 root         (0) root         (0)     1250 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/fullcalendar.locale.js
--rw-rw-rw-   0 root         (0) root         (0)    51213 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/fullcalendar.min.js
--rw-rw-rw-   0 root         (0) root         (0)      668 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/fullcalendar.print.css
--rw-rw-rw-   0 root         (0) root         (0)      377 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/go.png
--rw-rw-rw-   0 root         (0) root         (0)     1074 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/go_next.png
--rw-rw-rw-   0 root         (0) root         (0)      976 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/go_prev.png
--rw-rw-rw-   0 root         (0) root         (0)      462 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/gradient-grey-up.png
--rw-rw-rw-   0 root         (0) root         (0)      581 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/gradient-grey.gif
--rw-rw-rw-   0 root         (0) root         (0)      916 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/help.png
--rw-rw-rw-   0 root         (0) root         (0)      721 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/help_ie.png
--rw-rw-rw-   0 root         (0) root         (0)      314 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/icon_blank.png
--rw-rw-rw-   0 root         (0) root         (0)      393 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/icon_bookmark.gif
--rw-rw-rw-   0 root         (0) root         (0)      401 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/icon_emailaddress.gif
--rw-rw-rw-   0 root         (0) root         (0)      166 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/icon_euser.gif
--rw-rw-rw-   0 root         (0) root         (0)     1023 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/icon_map.png
--rw-rw-rw-   0 root         (0) root         (0)      132 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/icon_state.gif
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 09:13:18.410509 cubicweb-web-1.2.9/cubicweb_web/data/images/
--rw-rw-rw-   0 root         (0) root         (0)     1738 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/images/animated-overlay.gif
--rw-rw-rw-   0 root         (0) root         (0)      180 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/images/ui-bg_flat_0_aaaaaa_40x100.png
--rw-rw-rw-   0 root         (0) root         (0)      178 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/images/ui-bg_flat_75_ffffff_40x100.png
--rw-rw-rw-   0 root         (0) root         (0)      120 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/images/ui-bg_glass_55_fbf9ee_1x400.png
--rw-rw-rw-   0 root         (0) root         (0)       99 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/images/ui-bg_glass_65_ffffff_1x400.png
--rw-rw-rw-   0 root         (0) root         (0)      111 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/images/ui-bg_glass_75_dadada_1x400.png
--rw-rw-rw-   0 root         (0) root         (0)      110 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/images/ui-bg_glass_75_e6e6e6_1x400.png
--rw-rw-rw-   0 root         (0) root         (0)      119 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/images/ui-bg_glass_95_fef1ec_1x400.png
--rw-rw-rw-   0 root         (0) root         (0)      101 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/images/ui-bg_highlight-soft_75_cccccc_1x100.png
--rw-rw-rw-   0 root         (0) root         (0)     3824 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/images/ui-icons_222222_256x240.png
--rw-rw-rw-   0 root         (0) root         (0)     4369 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/images/ui-icons_2e83ff_256x240.png
--rw-rw-rw-   0 root         (0) root         (0)     4369 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/images/ui-icons_454545_256x240.png
--rw-rw-rw-   0 root         (0) root         (0)     4369 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/images/ui-icons_888888_256x240.png
--rw-rw-rw-   0 root         (0) root         (0)     4369 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/images/ui-icons_cd0a0a_256x240.png
--rw-rw-rw-   0 root         (0) root         (0)      112 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/incontextBoxHeader.png
--rw-rw-rw-   0 root         (0) root         (0)      206 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/information.png
--rw-rw-rw-   0 root         (0) root         (0)    16621 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/jquery-migrate.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 09:13:18.414509 cubicweb-web-1.2.9/cubicweb_web/data/jquery-treeview/
--rw-rw-rw-   0 root         (0) root         (0)     1772 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/jquery-treeview/changelog.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 09:13:18.422509 cubicweb-web-1.2.9/cubicweb_web/data/jquery-treeview/images/
--rw-rw-rw-   0 root         (0) root         (0)      649 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/jquery-treeview/images/ajax-loader.gif
--rw-rw-rw-   0 root         (0) root         (0)      109 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/jquery-treeview/images/file.gif
--rw-rw-rw-   0 root         (0) root         (0)      102 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/jquery-treeview/images/folder-closed.gif
--rw-rw-rw-   0 root         (0) root         (0)      106 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/jquery-treeview/images/folder.gif
--rw-rw-rw-   0 root         (0) root         (0)       58 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/jquery-treeview/images/minus.gif
--rw-rw-rw-   0 root         (0) root         (0)       61 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/jquery-treeview/images/plus.gif
--rw-rw-rw-   0 root         (0) root         (0)     1010 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/jquery-treeview/images/treeview-black-line.gif
--rw-rw-rw-   0 root         (0) root         (0)      381 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/jquery-treeview/images/treeview-black.gif
--rw-rw-rw-   0 root         (0) root         (0)      848 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/jquery-treeview/images/treeview-default-line.gif
--rw-rw-rw-   0 root         (0) root         (0)      387 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/jquery-treeview/images/treeview-default.gif
--rw-rw-rw-   0 root         (0) root         (0)       37 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/jquery-treeview/images/treeview-famfamfam-line.gif
--rw-rw-rw-   0 root         (0) root         (0)      545 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/jquery-treeview/images/treeview-famfamfam.gif
--rw-rw-rw-   0 root         (0) root         (0)     1010 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/jquery-treeview/images/treeview-gray-line.gif
--rw-rw-rw-   0 root         (0) root         (0)      394 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/jquery-treeview/images/treeview-gray.gif
--rw-rw-rw-   0 root         (0) root         (0)     1010 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/jquery-treeview/images/treeview-red-line.gif
--rw-rw-rw-   0 root         (0) root         (0)      394 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/jquery-treeview/images/treeview-red.gif
--rw-rw-rw-   0 root         (0) root         (0)     2946 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/jquery-treeview/jquery.treeview.async.js
--rw-rw-rw-   0 root         (0) root         (0)     2725 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/jquery-treeview/jquery.treeview.css
--rw-rw-rw-   0 root         (0) root         (0)     1566 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/jquery-treeview/jquery.treeview.edit.js
--rw-rw-rw-   0 root         (0) root         (0)     8065 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/jquery-treeview/jquery.treeview.js
--rw-rw-rw-   0 root         (0) root         (0)    13015 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/jquery-treeview/jquery.treeview.sortable.js
--rw-rw-rw-   0 root         (0) root         (0)     1563 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/jquery-treeview/readme.md
--rw-rw-rw-   0 root         (0) root         (0)     2387 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/jquery-treeview/screenshot.png
--rw-rw-rw-   0 root         (0) root         (0)     1536 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/jquery.cookie.js
--rw-rw-rw-   0 root         (0) root         (0)    89666 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/jquery.flot.js
--rw-rw-rw-   0 root         (0) root         (0)   273199 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/jquery.js
--rw-rw-rw-   0 root         (0) root         (0)    85184 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/jquery.qtip.js
--rw-rw-rw-   0 root         (0) root         (0)    38404 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/jquery.qtip.min.js
--rw-rw-rw-   0 root         (0) root         (0)    41257 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/jquery.tablesorter.js
--rw-rw-rw-   0 root         (0) root         (0)     8760 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/jquery.timePicker.js
--rw-rw-rw-   0 root         (0) root         (0)     1024 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/jquery.timepicker.css
--rw-rw-rw-   0 root         (0) root         (0)    32456 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/jquery.ui.css
--rw-rw-rw-   0 root         (0) root         (0)      884 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/jquery.ui.datepicker-de.js
--rw-rw-rw-   0 root         (0) root         (0)      895 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/jquery.ui.datepicker-es.js
--rw-rw-rw-   0 root         (0) root         (0)      932 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/jquery.ui.datepicker-fr.js
--rw-rw-rw-   0 root         (0) root         (0)   435844 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/jquery.ui.js
--rw-rw-rw-   0 root         (0) root         (0)      645 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/liveclipboard-icon.png
--rw-rw-rw-   0 root         (0) root         (0)     2606 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/loading.gif
--rw-rw-rw-   0 root         (0) root         (0)     9083 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/logo-cubicweb-gray.svg
--rw-rw-rw-   0 root         (0) root         (0)     3438 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/logo-cubicweb-icon.svg
--rw-rw-rw-   0 root         (0) root         (0)     7325 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/logo-cubicweb-text.svg
--rw-rw-rw-   0 root         (0) root         (0)     9202 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/logo-cubicweb.svg
--rw-rw-rw-   0 root         (0) root         (0)     2775 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/logo-logilab.png
--rw-rw-rw-   0 root         (0) root         (0)     4835 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/logo.png
--rw-rw-rw-   0 root         (0) root         (0)     1637 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/microformats-button.png
--rw-rw-rw-   0 root         (0) root         (0)     4147 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/microformats-icon.png
--rw-rw-rw-   0 root         (0) root         (0)      837 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/minus.gif
--rw-rw-rw-   0 root         (0) root         (0)       98 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/no-check-no-border.png
--rw-rw-rw-   0 root         (0) root         (0)      537 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/ok.png
--rw-rw-rw-   0 root         (0) root         (0)      272 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/pen_icon.png
--rw-rw-rw-   0 root         (0) root         (0)      841 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/plus.gif
--rw-rw-rw-   0 root         (0) root         (0)      443 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/plus.png
--rw-rw-rw-   0 root         (0) root         (0)    79752 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/porkys.ttf
--rw-rw-rw-   0 root         (0) root         (0)      144 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/puce.png
--rw-rw-rw-   0 root         (0) root         (0)      141 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/puce_down.png
--rw-rw-rw-   0 root         (0) root         (0)      111 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/puce_down_black.png
--rw-rw-rw-   0 root         (0) root         (0)      136 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/puce_up.png
--rw-rw-rw-   0 root         (0) root         (0)     3151 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/pygments.css
--rw-rw-rw-   0 root         (0) root         (0)       86 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/required.png
--rw-rw-rw-   0 root         (0) root         (0)      695 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/rss-button.png
--rw-rw-rw-   0 root         (0) root         (0)      288 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/rss.png
--rw-rw-rw-   0 root         (0) root         (0)      417 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/search.png
--rw-rw-rw-   0 root         (0) root         (0)      959 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/sendcancel.png
--rw-rw-rw-   0 root         (0) root         (0)     1257 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/sendok.png
--rw-rw-rw-   0 root         (0) root         (0)     1279 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/trash_can.png
--rw-rw-rw-   0 root         (0) root         (0)      983 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/trash_can_small.png
--rw-rw-rw-   0 root         (0) root         (0)    27374 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/ui.all.css
--rw-rw-rw-   0 root         (0) root         (0)     5055 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/uiprops.py
--rw-rw-rw-   0 root         (0) root         (0)       83 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/up.gif
--rw-rw-rw-   0 root         (0) root         (0)     2224 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/data/upload.gif
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 09:13:18.422509 cubicweb-web-1.2.9/cubicweb_web/devtools/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/devtools/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    39625 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/devtools/testlib.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 09:13:18.426509 cubicweb-web-1.2.9/cubicweb_web/ext/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/ext/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    17396 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/ext/rest.py
--rw-rw-rw-   0 root         (0) root         (0)    69654 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/facet.py
--rw-rw-rw-   0 root         (0) root         (0)    11036 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/form.py
--rw-rw-rw-   0 root         (0) root         (0)    49324 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/formfields.py
--rw-rw-rw-   0 root         (0) root         (0)    42455 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/formwidgets.py
--rw-rw-rw-   0 root         (0) root         (0)    11225 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/htmlwidgets.py
--rw-rw-rw-   0 root         (0) root         (0)    55646 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/http_headers.py
--rw-rw-rw-   0 root         (0) root         (0)     6189 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/httpcache.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 09:13:18.426509 cubicweb-web-1.2.9/cubicweb_web/i18n/
--rw-rw-rw-   0 root         (0) root         (0)    28312 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/i18n/de.po
--rw-rw-rw-   0 root         (0) root         (0)    21085 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/i18n/en.po
--rw-rw-rw-   0 root         (0) root         (0)    29875 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/i18n/es.po
--rw-rw-rw-   0 root         (0) root         (0)    30400 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/i18n/fr.po
--rw-rw-rw-   0 root         (0) root         (0)     5407 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/i18n.py
--rw-rw-rw-   0 root         (0) root         (0)     2187 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/predicates.py
--rw-rw-rw-   0 root         (0) root         (0)     4971 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/propertysheet.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 09:13:18.430509 cubicweb-web-1.2.9/cubicweb_web/pyramid/
--rw-rw-rw-   0 root         (0) root         (0)     1000 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/pyramid/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5611 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/pyramid/login.py
--rw-rw-rw-   0 root         (0) root         (0)     1803 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/pyramid/predicates.py
--rw-rw-rw-   0 root         (0) root         (0)     5584 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/pyramid/test.py
--rw-rw-rw-   0 root         (0) root         (0)     3920 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/pyramid/url_redirection.py
--rw-rw-rw-   0 root         (0) root         (0)    40224 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/request.py
--rw-rw-rw-   0 root         (0) root         (0)    10174 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/schemaviewer.py
--rw-rw-rw-   0 root         (0) root         (0)     6699 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/uihelper.py
--rw-rw-rw-   0 root         (0) root         (0)    11061 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/utils.py
--rw-rw-rw-   0 root         (0) root         (0)    19971 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/view.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 09:13:18.462510 cubicweb-web-1.2.9/cubicweb_web/views/
--rw-rw-rw-   0 root         (0) root         (0)     4261 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/views/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      577 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/views/_vid_by_mimetype.py
--rw-rw-rw-   0 root         (0) root         (0)    14805 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/views/actions.py
--rw-rw-rw-   0 root         (0) root         (0)    16562 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/views/ajaxcontroller.py
--rw-rw-rw-   0 root         (0) root         (0)     5027 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/views/ajaxedit.py
--rw-rw-rw-   0 root         (0) root         (0)     4072 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/views/apacherewrite.py
--rw-rw-rw-   0 root         (0) root         (0)     6730 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/views/authentication.py
--rw-rw-rw-   0 root         (0) root         (0)    46306 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/views/autoform.py
--rw-rw-rw-   0 root         (0) root         (0)     8971 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/views/basecomponents.py
--rw-rw-rw-   0 root         (0) root         (0)    11545 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/views/basecontrollers.py
--rw-rw-rw-   0 root         (0) root         (0)    20464 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/views/basetemplates.py
--rw-rw-rw-   0 root         (0) root         (0)    22595 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/views/baseviews.py
--rw-rw-rw-   0 root         (0) root         (0)     6181 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/views/bookmark.py
--rw-rw-rw-   0 root         (0) root         (0)     9230 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/views/boxes.py
--rw-rw-rw-   0 root         (0) root         (0)     9783 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/views/calendar.py
--rw-rw-rw-   0 root         (0) root         (0)     4352 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/views/csvexport.py
--rw-rw-rw-   0 root         (0) root         (0)    17004 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/views/cwproperties.py
--rw-rw-rw-   0 root         (0) root         (0)    16247 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/views/cwsources.py
--rw-rw-rw-   0 root         (0) root         (0)    10521 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/views/cwuser.py
--rw-rw-rw-   0 root         (0) root         (0)     7008 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/views/debug.py
--rw-rw-rw-   0 root         (0) root         (0)     2465 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/views/dotgraphview.py
--rw-rw-rw-   0 root         (0) root         (0)      697 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/views/edit_attributes.pt
--rw-rw-rw-   0 root         (0) root         (0)    20973 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/views/editcontroller.py
--rw-rw-rw-   0 root         (0) root         (0)    12498 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/views/editforms.py
--rw-rw-rw-   0 root         (0) root         (0)     4687 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/views/editviews.py
--rw-rw-rw-   0 root         (0) root         (0)     5183 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/views/emailaddress.py
--rw-rw-rw-   0 root         (0) root         (0)     1357 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/views/error.py
--rw-rw-rw-   0 root         (0) root         (0)    16339 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/views/facets.py
--rw-rw-rw-   0 root         (0) root         (0)    20026 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/views/formrenderers.py
--rw-rw-rw-   0 root         (0) root         (0)    18227 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/views/forms.py
--rw-rw-rw-   0 root         (0) root         (0)     7798 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/views/ibreadcrumbs.py
--rw-rw-rw-   0 root         (0) root         (0)     8266 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/views/idownloadable.py
--rw-rw-rw-   0 root         (0) root         (0)     5584 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/views/json.py
--rw-rw-rw-   0 root         (0) root         (0)    16883 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/views/magicsearch.py
--rw-rw-rw-   0 root         (0) root         (0)     9042 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/views/management.py
--rw-rw-rw-   0 root         (0) root         (0)    17293 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/views/navigation.py
--rw-rw-rw-   0 root         (0) root         (0)     9023 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/views/owl.py
--rw-rw-rw-   0 root         (0) root         (0)     4632 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/views/plots.py
--rw-rw-rw-   0 root         (0) root         (0)    18381 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/views/primary.py
--rw-rw-rw-   0 root         (0) root         (0)     4299 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/views/pyviews.py
--rw-rw-rw-   0 root         (0) root         (0)     5345 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/views/rdf.py
--rw-rw-rw-   0 root         (0) root         (0)    21998 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/views/reledit.py
--rw-rw-rw-   0 root         (0) root         (0)    29416 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/views/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     1073 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/views/searchrestriction.py
--rw-rw-rw-   0 root         (0) root         (0)     7050 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/views/sessions.py
--rw-rw-rw-   0 root         (0) root         (0)     7293 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/views/startup.py
--rw-rw-rw-   0 root         (0) root         (0)    11528 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/views/staticcontrollers.py
--rw-rw-rw-   0 root         (0) root         (0)    48952 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/views/tableview.py
--rw-rw-rw-   0 root         (0) root         (0)     9630 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/views/tabs.py
--rw-rw-rw-   0 root         (0) root         (0)     8971 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/views/timetable.py
--rw-rw-rw-   0 root         (0) root         (0)    12731 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/views/treeview.py
--rw-rw-rw-   0 root         (0) root         (0)    29957 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/views/uicfg.py
--rw-rw-rw-   0 root         (0) root         (0)     8484 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/views/undohistory.py
--rw-rw-rw-   0 root         (0) root         (0)    16377 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/views/urlpublishing.py
--rw-rw-rw-   0 root         (0) root         (0)     9037 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/views/urlrewrite.py
--rw-rw-rw-   0 root         (0) root         (0)     2278 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/views/vcard.py
--rw-rw-rw-   0 root         (0) root         (0)     7288 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/views/wdoc.py
--rw-rw-rw-   0 root         (0) root         (0)    17746 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/views/workflow.py
--rw-rw-rw-   0 root         (0) root         (0)     2320 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/views/xbel.py
--rw-rw-rw-   0 root         (0) root         (0)    10739 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/views/xmlrss.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 09:13:18.474510 cubicweb-web-1.2.9/cubicweb_web/wdoc/
--rw-rw-rw-   0 root         (0) root         (0)      994 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/wdoc/about_en.rst
--rw-rw-rw-   0 root         (0) root         (0)     1148 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/wdoc/about_fr.rst
--rw-rw-rw-   0 root         (0) root         (0)      281 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/wdoc/add_content_en.rst
--rw-rw-rw-   0 root         (0) root         (0)      429 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/wdoc/add_content_fr.rst
--rw-rw-rw-   0 root         (0) root         (0)       37 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/wdoc/advanced_usage_en.rst
--rw-rw-rw-   0 root         (0) root         (0)      365 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/wdoc/advanced_usage_schema_en.rst
--rw-rw-rw-   0 root         (0) root         (0)      720 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/wdoc/advanced_usage_schema_fr.rst
--rw-rw-rw-   0 root         (0) root         (0)     1164 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/wdoc/bookmarks_en.rst
--rw-rw-rw-   0 root         (0) root         (0)     1521 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/wdoc/bookmarks_fr.rst
--rw-rw-rw-   0 root         (0) root         (0)      706 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/wdoc/custom_view_en.rst
--rw-rw-rw-   0 root         (0) root         (0)      884 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/wdoc/custom_view_fr.rst
--rw-rw-rw-   0 root         (0) root         (0)      215 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/wdoc/custom_view_last_update_en.rst
--rw-rw-rw-   0 root         (0) root         (0)      330 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/wdoc/custom_view_last_update_fr.rst
--rw-rw-rw-   0 root         (0) root         (0)      459 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/wdoc/custom_view_rss_en.rst
--rw-rw-rw-   0 root         (0) root         (0)      648 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/wdoc/custom_view_rss_fr.rst
--rw-rw-rw-   0 root         (0) root         (0)      507 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/wdoc/glossary_en.rst
--rw-rw-rw-   0 root         (0) root         (0)      728 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/wdoc/glossary_fr.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 09:13:18.478510 cubicweb-web-1.2.9/cubicweb_web/wdoc/images/
--rw-rw-rw-   0 root         (0) root         (0)     5590 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/wdoc/images/userprefs_en.png
--rw-rw-rw-   0 root         (0) root         (0)     6423 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/wdoc/images/userprefs_fr.png
--rw-rw-rw-   0 root         (0) root         (0)       20 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/wdoc/main_en.rst
--rw-rw-rw-   0 root         (0) root         (0)      312 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/wdoc/search_en.rst
--rw-rw-rw-   0 root         (0) root         (0)      393 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/wdoc/search_fr.rst
--rw-rw-rw-   0 root         (0) root         (0)      108 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/wdoc/search_sample_queries_en.rst
--rw-rw-rw-   0 root         (0) root         (0)      125 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/wdoc/search_sample_queries_fr.rst
--rw-rw-rw-   0 root         (0) root         (0)      398 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/wdoc/standard_usage_en.rst
--rw-rw-rw-   0 root         (0) root         (0)      582 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/wdoc/standard_usage_fr.rst
--rw-rw-rw-   0 root         (0) root         (0)     1708 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/wdoc/toc.xml
--rw-rw-rw-   0 root         (0) root         (0)     6393 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/wdoc/tut_rql_en.rst
--rw-rw-rw-   0 root         (0) root         (0)     7275 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/wdoc/tut_rql_fr.rst
--rw-rw-rw-   0 root         (0) root         (0)      486 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/wdoc/userprefs_en.rst
--rw-rw-rw-   0 root         (0) root         (0)     2412 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/wdoc/userprefs_fr.rst
--rw-rw-rw-   0 root         (0) root         (0)    17696 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/cubicweb_web/webconfig.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 09:13:18.534511 cubicweb-web-1.2.9/cubicweb_web.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1272 2024-02-07 09:13:17.000000 cubicweb-web-1.2.9/cubicweb_web.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    15081 2024-02-07 09:13:18.000000 cubicweb-web-1.2.9/cubicweb_web.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-07 09:13:17.000000 cubicweb-web-1.2.9/cubicweb_web.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      109 2024-02-07 09:13:17.000000 cubicweb-web-1.2.9/cubicweb_web.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-07 09:13:17.000000 cubicweb-web-1.2.9/cubicweb_web.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       34 2024-02-07 09:13:17.000000 cubicweb-web-1.2.9/cubicweb_web.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       23 2024-02-07 09:13:17.000000 cubicweb-web-1.2.9/cubicweb_web.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-02-07 09:13:18.538511 cubicweb-web-1.2.9/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     2708 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 09:13:18.510510 cubicweb-web-1.2.9/test/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 09:13:18.514510 cubicweb-web-1.2.9/test/data/
--rw-rw-rw-   0 root         (0) root         (0)       27 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/data/bootstrap_cubes
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 09:13:18.514510 cubicweb-web-1.2.9/test/data/cubicweb_blog/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/data/cubicweb_blog/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/data/cubicweb_blog/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      201 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/data/cubicweb_blog/entities.py
--rw-rw-rw-   0 root         (0) root         (0)      961 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/data/cubicweb_blog/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 09:13:18.518510 cubicweb-web-1.2.9/test/data/cubicweb_card/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/data/cubicweb_card/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/data/cubicweb_card/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      441 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/data/cubicweb_card/entities.py
--rw-rw-rw-   0 root         (0) root         (0)      664 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/data/cubicweb_card/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 09:13:18.518510 cubicweb-web-1.2.9/test/data/cubicweb_file/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/data/cubicweb_file/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/data/cubicweb_file/__pkginfo__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 09:13:18.522511 cubicweb-web-1.2.9/test/data/cubicweb_file/data/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/data/cubicweb_file/data/file.png
--rw-rw-rw-   0 root         (0) root         (0)     2000 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/data/cubicweb_file/entities.py
--rw-rw-rw-   0 root         (0) root         (0)     2431 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/data/cubicweb_file/hooks.py
--rw-rw-rw-   0 root         (0) root         (0)     1277 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/data/cubicweb_file/schema.py
--rw-rw-rw-   0 root         (0) root         (0)       43 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/data/cubicweb_file/uiprops.py
--rw-rw-rw-   0 root         (0) root         (0)      387 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/data/cubicweb_file/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 09:13:18.522511 cubicweb-web-1.2.9/test/data/cubicweb_file/wdoc/
--rw-rw-rw-   0 root         (0) root         (0)      185 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/data/cubicweb_file/wdoc/toc.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 09:13:18.522511 cubicweb-web-1.2.9/test/data/cubicweb_tag/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/data/cubicweb_tag/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       41 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/data/cubicweb_tag/__pkginfo__.py
--rw-rw-rw-   0 root         (0) root         (0)      622 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/data/cubicweb_tag/schema.py
--rw-rw-rw-   0 root         (0) root         (0)      985 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/data/cubicweb_tag/views.py
--rw-rw-rw-   0 root         (0) root         (0)     1836 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/data/entities.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 09:13:18.286507 cubicweb-web-1.2.9/test/data/libpython/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 09:13:18.526511 cubicweb-web-1.2.9/test/data/libpython/cubicweb_i18ntestcube/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/data/libpython/cubicweb_i18ntestcube/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      486 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/data/libpython/cubicweb_i18ntestcube/__pkginfo__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 09:13:18.526511 cubicweb-web-1.2.9/test/data/libpython/cubicweb_i18ntestcube/excludeme/
--rw-rw-rw-   0 root         (0) root         (0)       39 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/data/libpython/cubicweb_i18ntestcube/excludeme/somefile.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 09:13:18.526511 cubicweb-web-1.2.9/test/data/libpython/cubicweb_i18ntestcube/i18n/
--rw-rw-rw-   0 root         (0) root         (0)     2657 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/data/libpython/cubicweb_i18ntestcube/i18n/en.po.ref
--rw-rw-rw-   0 root         (0) root         (0)     1725 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/data/libpython/cubicweb_i18ntestcube/schema.py
--rw-rw-rw-   0 root         (0) root         (0)     2266 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/data/libpython/cubicweb_i18ntestcube/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 09:13:18.526511 cubicweb-web-1.2.9/test/data/libpython/cubicweb_i18ntestcube-0.1.0.dist-info/
--rw-rw-rw-   0 root         (0) root         (0)        4 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/data/libpython/cubicweb_i18ntestcube-0.1.0.dist-info/INSTALLER
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/data/libpython/cubicweb_i18ntestcube-0.1.0.dist-info/METADATA
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/data/libpython/cubicweb_i18ntestcube-0.1.0.dist-info/RECORD
--rw-rw-rw-   0 root         (0) root         (0)       92 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/data/libpython/cubicweb_i18ntestcube-0.1.0.dist-info/WHEEL
--rw-rw-rw-   0 root         (0) root         (0)      136 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/data/libpython/cubicweb_i18ntestcube-0.1.0.dist-info/entry_points.txt
--rw-rw-rw-   0 root         (0) root         (0)       22 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/data/libpython/cubicweb_i18ntestcube-0.1.0.dist-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       67 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/data/pouet.css
--rw-rw-rw-   0 root         (0) root         (0)     8663 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/data/schema.py
--rw-rw-rw-   0 root         (0) root         (0)      133 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/data/sheet1.py
--rw-rw-rw-   0 root         (0) root         (0)      109 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/data/sheet2.py
--rw-rw-rw-   0 root         (0) root         (0)     2839 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/data/views.py
--rw-rw-rw-   0 root         (0) root         (0)    35939 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/test_application.py
--rw-rw-rw-   0 root         (0) root         (0)     2260 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/test_breadcrumbs.py
--rw-rw-rw-   0 root         (0) root         (0)     3166 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/test_bw_request.py
--rw-rw-rw-   0 root         (0) root         (0)     2319 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/test_controller.py
--rw-rw-rw-   0 root         (0) root         (0)     4974 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/test_csrf.py
--rw-rw-rw-   0 root         (0) root         (0)    12892 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/test_entity.py
--rw-rw-rw-   0 root         (0) root         (0)    24397 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/test_facet.py
--rw-rw-rw-   0 root         (0) root         (0)    17841 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/test_form.py
--rw-rw-rw-   0 root         (0) root         (0)     9449 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/test_formfields.py
--rw-rw-rw-   0 root         (0) root         (0)     3296 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/test_formwidgets.py
--rw-rw-rw-   0 root         (0) root         (0)     9718 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/test_http.py
--rw-rw-rw-   0 root         (0) root         (0)      563 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/test_http_headers.py
--rw-rw-rw-   0 root         (0) root         (0)     2414 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/test_httptest.py
--rw-rw-rw-   0 root         (0) root         (0)     1966 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/test_i18n.py
--rw-rw-rw-   0 root         (0) root         (0)     6673 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/test_idownloadable.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 09:13:18.530511 cubicweb-web-1.2.9/test/test_js_scripts/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 09:13:18.530511 cubicweb-web-1.2.9/test/test_js_scripts/data/
--rw-rw-rw-   0 root         (0) root         (0)       44 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/test_js_scripts/data/ajax_url0.html
--rw-rw-rw-   0 root         (0) root         (0)      166 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/test_js_scripts/data/ajax_url1.html
--rw-rw-rw-   0 root         (0) root         (0)       15 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/test_js_scripts/data/ajaxresult.json
--rw-rw-rw-   0 root         (0) root         (0)     1071 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/test_js_scripts/data/test_htmlhelpers.html
--rw-rw-rw-   0 root         (0) root         (0)     1008 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/test_js_scripts/data/test_utils.html
--rw-rw-rw-   0 root         (0) root         (0)     6549 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/test_js_scripts/jest.config.js
--rw-rw-rw-   0 root         (0) root         (0)   122226 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/test_js_scripts/package-lock.json
--rw-rw-rw-   0 root         (0) root         (0)      336 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/test_js_scripts/package.json
--rw-rw-rw-   0 root         (0) root         (0)      407 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/test_js_scripts/setup.js
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 09:13:18.534511 cubicweb-web-1.2.9/test/test_js_scripts/test/
--rw-rw-rw-   0 root         (0) root         (0)     7373 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/test_js_scripts/test/ajax.test.js
--rw-rw-rw-   0 root         (0) root         (0)     1242 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/test_js_scripts/test/htmlhelpers.test.js
--rw-rw-rw-   0 root         (0) root         (0)      821 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/test_js_scripts/test/utils.js
--rw-rw-rw-   0 root         (0) root         (0)     3723 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/test_js_scripts/test/utils.test.js
--rw-rw-rw-   0 root         (0) root         (0)     4843 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/test_login.py
--rw-rw-rw-   0 root         (0) root         (0)    13290 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/test_magicsearch.py
--rw-rw-rw-   0 root         (0) root         (0)     6991 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/test_predicates.py
--rw-rw-rw-   0 root         (0) root         (0)     2469 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/test_propertysheet.py
--rw-rw-rw-   0 root         (0) root         (0)      958 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/test_pyramid.py
--rw-rw-rw-   0 root         (0) root         (0)     3124 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/test_pyramid_hooks.py
--rw-rw-rw-   0 root         (0) root         (0)     3122 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/test_pyramid_predicates.py
--rw-rw-rw-   0 root         (0) root         (0)    23077 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/test_reledit.py
--rw-rw-rw-   0 root         (0) root         (0)     6166 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/test_request.py
--rw-rw-rw-   0 root         (0) root         (0)    10906 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/test_rest.py
--rw-rw-rw-   0 root         (0) root         (0)     1452 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/test_rset.py
--rw-rw-rw-   0 root         (0) root         (0)     5569 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/test_testlib.py
--rw-rw-rw-   0 root         (0) root         (0)     9091 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/test_uicfg.py
--rw-rw-rw-   0 root         (0) root         (0)     1332 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/test_url_redirection.py
--rw-rw-rw-   0 root         (0) root         (0)     8483 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/test_urlpublisher.py
--rw-rw-rw-   0 root         (0) root         (0)     9697 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/test_urlrewrite.py
--rw-rw-rw-   0 root         (0) root         (0)     3147 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/test_views_actions.py
--rw-rw-rw-   0 root         (0) root         (0)     2791 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/test_views_apacherewrite.py
--rw-rw-rw-   0 root         (0) root         (0)    54787 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/test_views_basecontrollers.py
--rw-rw-rw-   0 root         (0) root         (0)     2089 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/test_views_basetemplates.py
--rw-rw-rw-   0 root         (0) root         (0)    13844 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/test_views_baseviews.py
--rw-rw-rw-   0 root         (0) root         (0)     2265 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/test_views_csv.py
--rw-rw-rw-   0 root         (0) root         (0)     2120 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/test_views_cwsources.py
--rw-rw-rw-   0 root         (0) root         (0)     1796 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/test_views_debug_html.py
--rw-rw-rw-   0 root         (0) root         (0)    19638 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/test_views_editforms.py
--rw-rw-rw-   0 root         (0) root         (0)     3424 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/test_views_errorform.py
--rw-rw-rw-   0 root         (0) root         (0)     4432 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/test_views_forms.py
--rw-rw-rw-   0 root         (0) root         (0)     4536 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/test_views_json.py
--rw-rw-rw-   0 root         (0) root         (0)     6177 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/test_views_navigation.py
--rw-rw-rw-   0 root         (0) root         (0)     2113 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/test_views_pyviews.py
--rw-rw-rw-   0 root         (0) root         (0)     4912 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/test_views_searchrestriction.py
--rw-rw-rw-   0 root         (0) root         (0)     7239 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/test_views_staticcontrollers.py
--rw-rw-rw-   0 root         (0) root         (0)     2030 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/test_views_treeview.py
--rw-rw-rw-   0 root         (0) root         (0)      800 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/test_views_wdoc.py
--rw-rw-rw-   0 root         (0) root         (0)     1560 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/test_views_xmlrss.py
--rw-rw-rw-   0 root         (0) root         (0)    29065 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/test_viewselector.py
--rw-rw-rw-   0 root         (0) root         (0)     3908 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/test_vregistry.py
--rw-rw-rw-   0 root         (0) root         (0)     6074 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/test_web.py
--rw-rw-rw-   0 root         (0) root         (0)     2920 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/test_webconfig.py
--rw-rw-rw-   0 root         (0) root         (0)     1225 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/test_webtest.py
--rw-rw-rw-   0 root         (0) root         (0)      719 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/testutils.js
--rw-rw-rw-   0 root         (0) root         (0)     6438 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test/unittest_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 09:13:18.534511 cubicweb-web-1.2.9/test_auto/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test_auto/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-07 09:13:18.534511 cubicweb-web-1.2.9/test_auto/data/
--rw-rw-rw-   0 root         (0) root         (0)        4 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test_auto/data/bootstrap_cubes
--rw-rw-rw-   0 root         (0) root         (0)     3560 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/test_auto/test_views.py
--rw-rw-rw-   0 root         (0) root         (0)     1794 2024-02-07 09:12:56.000000 cubicweb-web-1.2.9/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:07:06.077506 cubicweb-web-1.3.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1234 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1272 2024-05-23 10:07:06.077506 cubicweb-web-1.3.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      785 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:07:05.869501 cubicweb-web-1.3.0/cubicweb_web/
+-rw-rw-rw-   0 root         (0) root         (0)     2821 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      661 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3696 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/_exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     4320 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/action.py
+-rw-rw-rw-   0 root         (0) root         (0)    21197 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/application.py
+-rw-rw-rw-   0 root         (0) root         (0)     6976 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/box.py
+-rw-rw-rw-   0 root         (0) root         (0)    21418 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/bwcompat.py
+-rw-rw-rw-   0 root         (0) root         (0)     3939 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/captcha.py
+-rw-rw-rw-   0 root         (0) root         (0)     4834 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/ccplugin.py
+-rw-rw-rw-   0 root         (0) root         (0)    29066 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/component.py
+-rw-rw-rw-   0 root         (0) root         (0)     8635 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/controller.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:07:05.941503 cubicweb-web-1.3.0/cubicweb_web/data/
+-rw-rw-rw-   0 root         (0) root         (0)      414 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/accessories-text-editor.png
+-rw-rw-rw-   0 root         (0) root         (0)      190 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/add_button.png
+-rw-rw-rw-   0 root         (0) root         (0)       54 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/asc.gif
+-rw-rw-rw-   0 root         (0) root         (0)      579 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/banner.png
+-rw-rw-rw-   0 root         (0) root         (0)       64 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/bg.gif
+-rw-rw-rw-   0 root         (0) root         (0)      112 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/bg_trame_grise.png
+-rw-rw-rw-   0 root         (0) root         (0)      719 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/black-check.png
+-rw-rw-rw-   0 root         (0) root         (0)      526 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/black-uncheck.png
+-rw-rw-rw-   0 root         (0) root         (0)      113 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/bullet.png
+-rw-rw-rw-   0 root         (0) root         (0)      110 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/bullet_orange.png
+-rw-rw-rw-   0 root         (0) root         (0)      110 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/button.png
+-rw-rw-rw-   0 root         (0) root         (0)       75 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/calendar.gif
+-rw-rw-rw-   0 root         (0) root         (0)      655 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/cancel.png
+-rw-rw-rw-   0 root         (0) root         (0)      112 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/contextFreeBoxHeader.png
+-rw-rw-rw-   0 root         (0) root         (0)      128 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/contextualBoxHeader.png
+-rw-rw-rw-   0 root         (0) root         (0)      414 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/critical.png
+-rw-rw-rw-   0 root         (0) root         (0)      924 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/cubicweb.acl.css
+-rw-rw-rw-   0 root         (0) root         (0)     3589 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/cubicweb.ajax.box.js
+-rw-rw-rw-   0 root         (0) root         (0)    24133 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/cubicweb.ajax.js
+-rw-rw-rw-   0 root         (0) root         (0)     7895 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/cubicweb.calendar.css
+-rw-rw-rw-   0 root         (0) root         (0)     9665 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/cubicweb.calendar.js
+-rw-rw-rw-   0 root         (0) root         (0)     1179 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/cubicweb.calendar_popup.css
+-rw-rw-rw-   0 root         (0) root         (0)      564 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/cubicweb.compat.js
+-rw-rw-rw-   0 root         (0) root         (0)    18494 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/cubicweb.css
+-rw-rw-rw-   0 root         (0) root         (0)    18779 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/cubicweb.edition.js
+-rw-rw-rw-   0 root         (0) root         (0)     2019 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/cubicweb.facets.css
+-rw-rw-rw-   0 root         (0) root         (0)    12099 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/cubicweb.facets.js
+-rw-rw-rw-   0 root         (0) root         (0)     1488 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/cubicweb.fckcwconfig-full.js
+-rw-rw-rw-   0 root         (0) root         (0)      592 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/cubicweb.fckcwconfig.js
+-rw-rw-rw-   0 root         (0) root         (0)     1505 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/cubicweb.flot.js
+-rw-rw-rw-   0 root         (0) root         (0)     3811 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/cubicweb.form.css
+-rw-rw-rw-   0 root         (0) root         (0)     1408 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/cubicweb.html_tree.css
+-rw-rw-rw-   0 root         (0) root         (0)     4595 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/cubicweb.htmlhelpers.js
+-rw-rw-rw-   0 root         (0) root         (0)      550 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/cubicweb.ie.css
+-rw-rw-rw-   0 root         (0) root         (0)     1318 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/cubicweb.image.js
+-rw-rw-rw-   0 root         (0) root         (0)    12621 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/cubicweb.js
+-rw-rw-rw-   0 root         (0) root         (0)     1975 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/cubicweb.log.css
+-rw-rw-rw-   0 root         (0) root         (0)      384 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/cubicweb.log.js
+-rw-rw-rw-   0 root         (0) root         (0)     1756 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/cubicweb.login.css
+-rw-rw-rw-   0 root         (0) root         (0)      331 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/cubicweb.manageview.css
+-rw-rw-rw-   0 root         (0) root         (0)    16860 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/cubicweb.pictograms.css
+-rw-rw-rw-   0 root         (0) root         (0)     1671 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/cubicweb.preferences.css
+-rw-rw-rw-   0 root         (0) root         (0)     4559 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/cubicweb.preferences.js
+-rw-rw-rw-   0 root         (0) root         (0)      189 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/cubicweb.print.css
+-rw-rw-rw-   0 root         (0) root         (0)     7718 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/cubicweb.python.js
+-rw-rw-rw-   0 root         (0) root         (0)     2754 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/cubicweb.reledit.js
+-rw-rw-rw-   0 root         (0) root         (0)     1930 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/cubicweb.schema.css
+-rw-rw-rw-   0 root         (0) root         (0)      756 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/cubicweb.suggest.css
+-rw-rw-rw-   0 root         (0) root         (0)      350 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/cubicweb.tablesorter.css
+-rw-rw-rw-   0 root         (0) root         (0)      822 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/cubicweb.tableview.css
+-rw-rw-rw-   0 root         (0) root         (0)     2901 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/cubicweb.timetable.css
+-rw-rw-rw-   0 root         (0) root         (0)       89 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/cubicweb.treeview.css
+-rw-rw-rw-   0 root         (0) root         (0)    19668 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/cubicweb.widgets.js
+-rw-rw-rw-   0 root         (0) root         (0)       54 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/desc.gif
+-rw-rw-rw-   0 root         (0) root         (0)      860 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/download.gif
+-rw-rw-rw-   0 root         (0) root         (0)      973 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/dublincore-button.png
+-rw-rw-rw-   0 root         (0) root         (0)     2179 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/dublincore-icon.png
+-rw-rw-rw-   0 root         (0) root         (0)    67968 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/entypo.eot
+-rw-rw-rw-   0 root         (0) root         (0)    97203 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/entypo.svg
+-rw-rw-rw-   0 root         (0) root         (0)    67680 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/entypo.ttf
+-rw-rw-rw-   0 root         (0) root         (0)    42064 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/entypo.woff
+-rw-rw-rw-   0 root         (0) root         (0)      930 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/error.png
+-rw-rw-rw-   0 root         (0) root         (0)    42086 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/excanvas.js
+-rw-rw-rw-   0 root         (0) root         (0)    34494 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/favicon.ico
+-rw-rw-rw-   0 root         (0) root         (0)     5468 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/feed-icon.png
+-rw-rw-rw-   0 root         (0) root         (0)      715 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/feed-icon16x16.png
+-rw-rw-rw-   0 root         (0) root         (0)     1646 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/feed-icon32x32.png
+-rw-rw-rw-   0 root         (0) root         (0)      110 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/file.gif
+-rw-rw-rw-   0 root         (0) root         (0)      105 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/folder-closed.gif
+-rw-rw-rw-   0 root         (0) root         (0)      106 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/folder.gif
+-rw-rw-rw-   0 root         (0) root         (0)    11147 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/fullcalendar.css
+-rw-rw-rw-   0 root         (0) root         (0)   151629 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/fullcalendar.js
+-rw-rw-rw-   0 root         (0) root         (0)     1250 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/fullcalendar.locale.js
+-rw-rw-rw-   0 root         (0) root         (0)    51213 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/fullcalendar.min.js
+-rw-rw-rw-   0 root         (0) root         (0)      668 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/fullcalendar.print.css
+-rw-rw-rw-   0 root         (0) root         (0)      377 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/go.png
+-rw-rw-rw-   0 root         (0) root         (0)     1074 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/go_next.png
+-rw-rw-rw-   0 root         (0) root         (0)      976 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/go_prev.png
+-rw-rw-rw-   0 root         (0) root         (0)      462 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/gradient-grey-up.png
+-rw-rw-rw-   0 root         (0) root         (0)      581 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/gradient-grey.gif
+-rw-rw-rw-   0 root         (0) root         (0)      916 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/help.png
+-rw-rw-rw-   0 root         (0) root         (0)      721 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/help_ie.png
+-rw-rw-rw-   0 root         (0) root         (0)      314 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/data/icon_blank.png
+-rw-rw-rw-   0 root         (0) root         (0)      393 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/icon_bookmark.gif
+-rw-rw-rw-   0 root         (0) root         (0)      401 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/icon_emailaddress.gif
+-rw-rw-rw-   0 root         (0) root         (0)      166 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/icon_euser.gif
+-rw-rw-rw-   0 root         (0) root         (0)     1023 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/icon_map.png
+-rw-rw-rw-   0 root         (0) root         (0)      132 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/icon_state.gif
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:07:05.949503 cubicweb-web-1.3.0/cubicweb_web/data/images/
+-rw-rw-rw-   0 root         (0) root         (0)     1738 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/images/animated-overlay.gif
+-rw-rw-rw-   0 root         (0) root         (0)      180 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/images/ui-bg_flat_0_aaaaaa_40x100.png
+-rw-rw-rw-   0 root         (0) root         (0)      178 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/data/images/ui-bg_flat_75_ffffff_40x100.png
+-rw-rw-rw-   0 root         (0) root         (0)      120 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/images/ui-bg_glass_55_fbf9ee_1x400.png
+-rw-rw-rw-   0 root         (0) root         (0)       99 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/images/ui-bg_glass_65_ffffff_1x400.png
+-rw-rw-rw-   0 root         (0) root         (0)      111 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/images/ui-bg_glass_75_dadada_1x400.png
+-rw-rw-rw-   0 root         (0) root         (0)      110 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/images/ui-bg_glass_75_e6e6e6_1x400.png
+-rw-rw-rw-   0 root         (0) root         (0)      119 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/images/ui-bg_glass_95_fef1ec_1x400.png
+-rw-rw-rw-   0 root         (0) root         (0)      101 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/images/ui-bg_highlight-soft_75_cccccc_1x100.png
+-rw-rw-rw-   0 root         (0) root         (0)     3824 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/images/ui-icons_222222_256x240.png
+-rw-rw-rw-   0 root         (0) root         (0)     4369 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/data/images/ui-icons_2e83ff_256x240.png
+-rw-rw-rw-   0 root         (0) root         (0)     4369 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/images/ui-icons_454545_256x240.png
+-rw-rw-rw-   0 root         (0) root         (0)     4369 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/images/ui-icons_888888_256x240.png
+-rw-rw-rw-   0 root         (0) root         (0)     4369 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/images/ui-icons_cd0a0a_256x240.png
+-rw-rw-rw-   0 root         (0) root         (0)      112 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/incontextBoxHeader.png
+-rw-rw-rw-   0 root         (0) root         (0)      206 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/information.png
+-rw-rw-rw-   0 root         (0) root         (0)    16621 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/jquery-migrate.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:07:05.953503 cubicweb-web-1.3.0/cubicweb_web/data/jquery-treeview/
+-rw-rw-rw-   0 root         (0) root         (0)     1772 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/data/jquery-treeview/changelog.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:07:05.961503 cubicweb-web-1.3.0/cubicweb_web/data/jquery-treeview/images/
+-rw-rw-rw-   0 root         (0) root         (0)      649 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/data/jquery-treeview/images/ajax-loader.gif
+-rw-rw-rw-   0 root         (0) root         (0)      109 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/jquery-treeview/images/file.gif
+-rw-rw-rw-   0 root         (0) root         (0)      102 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/jquery-treeview/images/folder-closed.gif
+-rw-rw-rw-   0 root         (0) root         (0)      106 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/jquery-treeview/images/folder.gif
+-rw-rw-rw-   0 root         (0) root         (0)       58 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/jquery-treeview/images/minus.gif
+-rw-rw-rw-   0 root         (0) root         (0)       61 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/jquery-treeview/images/plus.gif
+-rw-rw-rw-   0 root         (0) root         (0)     1010 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/jquery-treeview/images/treeview-black-line.gif
+-rw-rw-rw-   0 root         (0) root         (0)      381 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/data/jquery-treeview/images/treeview-black.gif
+-rw-rw-rw-   0 root         (0) root         (0)      848 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/data/jquery-treeview/images/treeview-default-line.gif
+-rw-rw-rw-   0 root         (0) root         (0)      387 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/jquery-treeview/images/treeview-default.gif
+-rw-rw-rw-   0 root         (0) root         (0)       37 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/jquery-treeview/images/treeview-famfamfam-line.gif
+-rw-rw-rw-   0 root         (0) root         (0)      545 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/jquery-treeview/images/treeview-famfamfam.gif
+-rw-rw-rw-   0 root         (0) root         (0)     1010 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/jquery-treeview/images/treeview-gray-line.gif
+-rw-rw-rw-   0 root         (0) root         (0)      394 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/jquery-treeview/images/treeview-gray.gif
+-rw-rw-rw-   0 root         (0) root         (0)     1010 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/jquery-treeview/images/treeview-red-line.gif
+-rw-rw-rw-   0 root         (0) root         (0)      394 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/data/jquery-treeview/images/treeview-red.gif
+-rw-rw-rw-   0 root         (0) root         (0)     2946 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/data/jquery-treeview/jquery.treeview.async.js
+-rw-rw-rw-   0 root         (0) root         (0)     2725 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/jquery-treeview/jquery.treeview.css
+-rw-rw-rw-   0 root         (0) root         (0)     1566 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/jquery-treeview/jquery.treeview.edit.js
+-rw-rw-rw-   0 root         (0) root         (0)     8065 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/jquery-treeview/jquery.treeview.js
+-rw-rw-rw-   0 root         (0) root         (0)    13015 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/jquery-treeview/jquery.treeview.sortable.js
+-rw-rw-rw-   0 root         (0) root         (0)     1563 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/jquery-treeview/readme.md
+-rw-rw-rw-   0 root         (0) root         (0)     2387 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/jquery-treeview/screenshot.png
+-rw-rw-rw-   0 root         (0) root         (0)     1536 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/data/jquery.cookie.js
+-rw-rw-rw-   0 root         (0) root         (0)    89666 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/data/jquery.flot.js
+-rw-rw-rw-   0 root         (0) root         (0)   273199 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/jquery.js
+-rw-rw-rw-   0 root         (0) root         (0)    85184 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/jquery.qtip.js
+-rw-rw-rw-   0 root         (0) root         (0)    38404 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/jquery.qtip.min.js
+-rw-rw-rw-   0 root         (0) root         (0)    41257 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/jquery.tablesorter.js
+-rw-rw-rw-   0 root         (0) root         (0)     8760 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/jquery.timePicker.js
+-rw-rw-rw-   0 root         (0) root         (0)     1024 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/jquery.timepicker.css
+-rw-rw-rw-   0 root         (0) root         (0)    32456 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/data/jquery.ui.css
+-rw-rw-rw-   0 root         (0) root         (0)      884 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/data/jquery.ui.datepicker-de.js
+-rw-rw-rw-   0 root         (0) root         (0)      895 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/jquery.ui.datepicker-es.js
+-rw-rw-rw-   0 root         (0) root         (0)      932 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/jquery.ui.datepicker-fr.js
+-rw-rw-rw-   0 root         (0) root         (0)   435844 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/jquery.ui.js
+-rw-rw-rw-   0 root         (0) root         (0)      645 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/liveclipboard-icon.png
+-rw-rw-rw-   0 root         (0) root         (0)     2606 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/data/loading.gif
+-rw-rw-rw-   0 root         (0) root         (0)     9083 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/logo-cubicweb-gray.svg
+-rw-rw-rw-   0 root         (0) root         (0)     3438 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/data/logo-cubicweb-icon.svg
+-rw-rw-rw-   0 root         (0) root         (0)     7325 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/data/logo-cubicweb-text.svg
+-rw-rw-rw-   0 root         (0) root         (0)     9202 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/logo-cubicweb.svg
+-rw-rw-rw-   0 root         (0) root         (0)     2775 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/logo-logilab.png
+-rw-rw-rw-   0 root         (0) root         (0)     4835 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/logo.png
+-rw-rw-rw-   0 root         (0) root         (0)     1637 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/microformats-button.png
+-rw-rw-rw-   0 root         (0) root         (0)     4147 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/data/microformats-icon.png
+-rw-rw-rw-   0 root         (0) root         (0)      837 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/minus.gif
+-rw-rw-rw-   0 root         (0) root         (0)       98 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/data/no-check-no-border.png
+-rw-rw-rw-   0 root         (0) root         (0)      537 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/data/ok.png
+-rw-rw-rw-   0 root         (0) root         (0)      272 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/pen_icon.png
+-rw-rw-rw-   0 root         (0) root         (0)      841 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/plus.gif
+-rw-rw-rw-   0 root         (0) root         (0)      443 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/plus.png
+-rw-rw-rw-   0 root         (0) root         (0)    79752 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/porkys.ttf
+-rw-rw-rw-   0 root         (0) root         (0)      144 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/data/puce.png
+-rw-rw-rw-   0 root         (0) root         (0)      141 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/puce_down.png
+-rw-rw-rw-   0 root         (0) root         (0)      111 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/data/puce_down_black.png
+-rw-rw-rw-   0 root         (0) root         (0)      136 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/data/puce_up.png
+-rw-rw-rw-   0 root         (0) root         (0)     3151 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/pygments.css
+-rw-rw-rw-   0 root         (0) root         (0)       86 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/required.png
+-rw-rw-rw-   0 root         (0) root         (0)      695 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/rss-button.png
+-rw-rw-rw-   0 root         (0) root         (0)      288 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/rss.png
+-rw-rw-rw-   0 root         (0) root         (0)      417 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/data/search.png
+-rw-rw-rw-   0 root         (0) root         (0)      959 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/sendcancel.png
+-rw-rw-rw-   0 root         (0) root         (0)     1257 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/data/sendok.png
+-rw-rw-rw-   0 root         (0) root         (0)     1279 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/data/trash_can.png
+-rw-rw-rw-   0 root         (0) root         (0)      983 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/trash_can_small.png
+-rw-rw-rw-   0 root         (0) root         (0)    27374 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/ui.all.css
+-rw-rw-rw-   0 root         (0) root         (0)     5055 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/uiprops.py
+-rw-rw-rw-   0 root         (0) root         (0)       83 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/data/up.gif
+-rw-rw-rw-   0 root         (0) root         (0)     2224 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/data/upload.gif
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:07:05.965503 cubicweb-web-1.3.0/cubicweb_web/devtools/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/devtools/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    39625 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/devtools/testlib.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:07:05.965503 cubicweb-web-1.3.0/cubicweb_web/ext/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/ext/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    17396 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/ext/rest.py
+-rw-rw-rw-   0 root         (0) root         (0)    69654 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/facet.py
+-rw-rw-rw-   0 root         (0) root         (0)    11036 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/form.py
+-rw-rw-rw-   0 root         (0) root         (0)    49324 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/formfields.py
+-rw-rw-rw-   0 root         (0) root         (0)    42455 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/formwidgets.py
+-rw-rw-rw-   0 root         (0) root         (0)    11225 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/htmlwidgets.py
+-rw-rw-rw-   0 root         (0) root         (0)    55646 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/http_headers.py
+-rw-rw-rw-   0 root         (0) root         (0)     6189 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/httpcache.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:07:05.965503 cubicweb-web-1.3.0/cubicweb_web/i18n/
+-rw-rw-rw-   0 root         (0) root         (0)    28312 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/i18n/de.po
+-rw-rw-rw-   0 root         (0) root         (0)    21085 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/i18n/en.po
+-rw-rw-rw-   0 root         (0) root         (0)    29875 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/i18n/es.po
+-rw-rw-rw-   0 root         (0) root         (0)    30400 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/i18n/fr.po
+-rw-rw-rw-   0 root         (0) root         (0)     5407 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/i18n.py
+-rw-rw-rw-   0 root         (0) root         (0)     2187 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/predicates.py
+-rw-rw-rw-   0 root         (0) root         (0)     4971 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/propertysheet.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:07:05.969503 cubicweb-web-1.3.0/cubicweb_web/pyramid/
+-rw-rw-rw-   0 root         (0) root         (0)     1000 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/pyramid/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5611 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/pyramid/login.py
+-rw-rw-rw-   0 root         (0) root         (0)     1803 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/pyramid/predicates.py
+-rw-rw-rw-   0 root         (0) root         (0)     5584 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/pyramid/test.py
+-rw-rw-rw-   0 root         (0) root         (0)     3920 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/pyramid/url_redirection.py
+-rw-rw-rw-   0 root         (0) root         (0)    40224 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/request.py
+-rw-rw-rw-   0 root         (0) root         (0)    10174 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/schemaviewer.py
+-rw-rw-rw-   0 root         (0) root         (0)     6699 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/uihelper.py
+-rw-rw-rw-   0 root         (0) root         (0)    11061 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    19971 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/view.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:07:06.001504 cubicweb-web-1.3.0/cubicweb_web/views/
+-rw-rw-rw-   0 root         (0) root         (0)     4261 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/views/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      577 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/views/_vid_by_mimetype.py
+-rw-rw-rw-   0 root         (0) root         (0)    14805 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/views/actions.py
+-rw-rw-rw-   0 root         (0) root         (0)    16562 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/views/ajaxcontroller.py
+-rw-rw-rw-   0 root         (0) root         (0)     5027 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/views/ajaxedit.py
+-rw-rw-rw-   0 root         (0) root         (0)     4072 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/views/apacherewrite.py
+-rw-rw-rw-   0 root         (0) root         (0)     6730 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/views/authentication.py
+-rw-rw-rw-   0 root         (0) root         (0)    46306 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/views/autoform.py
+-rw-rw-rw-   0 root         (0) root         (0)     8971 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/views/basecomponents.py
+-rw-rw-rw-   0 root         (0) root         (0)    11545 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/views/basecontrollers.py
+-rw-rw-rw-   0 root         (0) root         (0)    20464 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/views/basetemplates.py
+-rw-rw-rw-   0 root         (0) root         (0)    22591 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/views/baseviews.py
+-rw-rw-rw-   0 root         (0) root         (0)     6181 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/views/bookmark.py
+-rw-rw-rw-   0 root         (0) root         (0)     9230 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/views/boxes.py
+-rw-rw-rw-   0 root         (0) root         (0)     9783 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/views/calendar.py
+-rw-rw-rw-   0 root         (0) root         (0)     4352 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/views/csvexport.py
+-rw-rw-rw-   0 root         (0) root         (0)    17004 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/views/cwproperties.py
+-rw-rw-rw-   0 root         (0) root         (0)    16247 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/views/cwsources.py
+-rw-rw-rw-   0 root         (0) root         (0)    10707 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/views/cwuser.py
+-rw-rw-rw-   0 root         (0) root         (0)     7008 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/views/debug.py
+-rw-rw-rw-   0 root         (0) root         (0)     2465 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/views/dotgraphview.py
+-rw-rw-rw-   0 root         (0) root         (0)      697 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/views/edit_attributes.pt
+-rw-rw-rw-   0 root         (0) root         (0)    20973 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/views/editcontroller.py
+-rw-rw-rw-   0 root         (0) root         (0)    12498 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/views/editforms.py
+-rw-rw-rw-   0 root         (0) root         (0)     4687 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/views/editviews.py
+-rw-rw-rw-   0 root         (0) root         (0)     5183 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/views/emailaddress.py
+-rw-rw-rw-   0 root         (0) root         (0)     1357 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/views/error.py
+-rw-rw-rw-   0 root         (0) root         (0)    16339 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/views/facets.py
+-rw-rw-rw-   0 root         (0) root         (0)    20026 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/views/formrenderers.py
+-rw-rw-rw-   0 root         (0) root         (0)    18227 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/views/forms.py
+-rw-rw-rw-   0 root         (0) root         (0)     7798 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/views/ibreadcrumbs.py
+-rw-rw-rw-   0 root         (0) root         (0)     8266 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/views/idownloadable.py
+-rw-rw-rw-   0 root         (0) root         (0)     5940 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/views/json.py
+-rw-rw-rw-   0 root         (0) root         (0)    16883 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/views/magicsearch.py
+-rw-rw-rw-   0 root         (0) root         (0)     9359 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/views/management.py
+-rw-rw-rw-   0 root         (0) root         (0)    17293 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/views/navigation.py
+-rw-rw-rw-   0 root         (0) root         (0)     9023 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/views/owl.py
+-rw-rw-rw-   0 root         (0) root         (0)     4632 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/views/plots.py
+-rw-rw-rw-   0 root         (0) root         (0)    18381 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/views/primary.py
+-rw-rw-rw-   0 root         (0) root         (0)     4299 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/views/pyviews.py
+-rw-rw-rw-   0 root         (0) root         (0)     5345 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/views/rdf.py
+-rw-rw-rw-   0 root         (0) root         (0)    21998 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/views/reledit.py
+-rw-rw-rw-   0 root         (0) root         (0)    29416 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/views/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     1073 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/views/searchrestriction.py
+-rw-rw-rw-   0 root         (0) root         (0)     7050 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/views/sessions.py
+-rw-rw-rw-   0 root         (0) root         (0)     7293 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/views/startup.py
+-rw-rw-rw-   0 root         (0) root         (0)    11528 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/views/staticcontrollers.py
+-rw-rw-rw-   0 root         (0) root         (0)    48952 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/views/tableview.py
+-rw-rw-rw-   0 root         (0) root         (0)     9630 2024-05-23 10:06:39.000000 cubicweb-web-1.3.0/cubicweb_web/views/tabs.py
+-rw-rw-rw-   0 root         (0) root         (0)     8971 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/views/timetable.py
+-rw-rw-rw-   0 root         (0) root         (0)    12731 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/views/treeview.py
+-rw-rw-rw-   0 root         (0) root         (0)    29957 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/views/uicfg.py
+-rw-rw-rw-   0 root         (0) root         (0)     8484 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/views/undohistory.py
+-rw-rw-rw-   0 root         (0) root         (0)    16377 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/views/urlpublishing.py
+-rw-rw-rw-   0 root         (0) root         (0)     9037 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/views/urlrewrite.py
+-rw-rw-rw-   0 root         (0) root         (0)     2278 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/views/vcard.py
+-rw-rw-rw-   0 root         (0) root         (0)     7288 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/views/wdoc.py
+-rw-rw-rw-   0 root         (0) root         (0)    17746 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/views/workflow.py
+-rw-rw-rw-   0 root         (0) root         (0)     2320 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/views/xbel.py
+-rw-rw-rw-   0 root         (0) root         (0)    10739 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/views/xmlrss.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:07:06.017505 cubicweb-web-1.3.0/cubicweb_web/wdoc/
+-rw-rw-rw-   0 root         (0) root         (0)      994 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/wdoc/about_en.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1148 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/wdoc/about_fr.rst
+-rw-rw-rw-   0 root         (0) root         (0)      281 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/wdoc/add_content_en.rst
+-rw-rw-rw-   0 root         (0) root         (0)      429 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/wdoc/add_content_fr.rst
+-rw-rw-rw-   0 root         (0) root         (0)       37 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/wdoc/advanced_usage_en.rst
+-rw-rw-rw-   0 root         (0) root         (0)      365 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/wdoc/advanced_usage_schema_en.rst
+-rw-rw-rw-   0 root         (0) root         (0)      720 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/wdoc/advanced_usage_schema_fr.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1164 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/wdoc/bookmarks_en.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1521 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/wdoc/bookmarks_fr.rst
+-rw-rw-rw-   0 root         (0) root         (0)      706 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/wdoc/custom_view_en.rst
+-rw-rw-rw-   0 root         (0) root         (0)      884 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/wdoc/custom_view_fr.rst
+-rw-rw-rw-   0 root         (0) root         (0)      215 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/wdoc/custom_view_last_update_en.rst
+-rw-rw-rw-   0 root         (0) root         (0)      330 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/wdoc/custom_view_last_update_fr.rst
+-rw-rw-rw-   0 root         (0) root         (0)      459 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/wdoc/custom_view_rss_en.rst
+-rw-rw-rw-   0 root         (0) root         (0)      648 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/wdoc/custom_view_rss_fr.rst
+-rw-rw-rw-   0 root         (0) root         (0)      507 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/wdoc/glossary_en.rst
+-rw-rw-rw-   0 root         (0) root         (0)      728 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/wdoc/glossary_fr.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:07:06.017505 cubicweb-web-1.3.0/cubicweb_web/wdoc/images/
+-rw-rw-rw-   0 root         (0) root         (0)     5590 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/wdoc/images/userprefs_en.png
+-rw-rw-rw-   0 root         (0) root         (0)     6423 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/wdoc/images/userprefs_fr.png
+-rw-rw-rw-   0 root         (0) root         (0)       20 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/wdoc/main_en.rst
+-rw-rw-rw-   0 root         (0) root         (0)      312 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/wdoc/search_en.rst
+-rw-rw-rw-   0 root         (0) root         (0)      393 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/wdoc/search_fr.rst
+-rw-rw-rw-   0 root         (0) root         (0)      108 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/wdoc/search_sample_queries_en.rst
+-rw-rw-rw-   0 root         (0) root         (0)      125 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/wdoc/search_sample_queries_fr.rst
+-rw-rw-rw-   0 root         (0) root         (0)      398 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/wdoc/standard_usage_en.rst
+-rw-rw-rw-   0 root         (0) root         (0)      582 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/wdoc/standard_usage_fr.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1708 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/wdoc/toc.xml
+-rw-rw-rw-   0 root         (0) root         (0)     6393 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/wdoc/tut_rql_en.rst
+-rw-rw-rw-   0 root         (0) root         (0)     7275 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/wdoc/tut_rql_fr.rst
+-rw-rw-rw-   0 root         (0) root         (0)      486 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/wdoc/userprefs_en.rst
+-rw-rw-rw-   0 root         (0) root         (0)     2412 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/wdoc/userprefs_fr.rst
+-rw-rw-rw-   0 root         (0) root         (0)    17696 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/cubicweb_web/webconfig.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:07:06.077506 cubicweb-web-1.3.0/cubicweb_web.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1272 2024-05-23 10:07:05.000000 cubicweb-web-1.3.0/cubicweb_web.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    15081 2024-05-23 10:07:05.000000 cubicweb-web-1.3.0/cubicweb_web.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-23 10:07:05.000000 cubicweb-web-1.3.0/cubicweb_web.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      109 2024-05-23 10:07:05.000000 cubicweb-web-1.3.0/cubicweb_web.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-23 10:07:05.000000 cubicweb-web-1.3.0/cubicweb_web.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       34 2024-05-23 10:07:05.000000 cubicweb-web-1.3.0/cubicweb_web.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       23 2024-05-23 10:07:05.000000 cubicweb-web-1.3.0/cubicweb_web.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-23 10:07:06.077506 cubicweb-web-1.3.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2708 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:07:06.045505 cubicweb-web-1.3.0/test/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:07:06.049505 cubicweb-web-1.3.0/test/data/
+-rw-rw-rw-   0 root         (0) root         (0)       27 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/data/bootstrap_cubes
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:07:06.049505 cubicweb-web-1.3.0/test/data/cubicweb_blog/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/data/cubicweb_blog/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/data/cubicweb_blog/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      201 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/data/cubicweb_blog/entities.py
+-rw-rw-rw-   0 root         (0) root         (0)      961 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/data/cubicweb_blog/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:07:06.053505 cubicweb-web-1.3.0/test/data/cubicweb_card/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/data/cubicweb_card/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/data/cubicweb_card/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      441 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/data/cubicweb_card/entities.py
+-rw-rw-rw-   0 root         (0) root         (0)      664 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/data/cubicweb_card/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:07:06.057505 cubicweb-web-1.3.0/test/data/cubicweb_file/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/data/cubicweb_file/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/data/cubicweb_file/__pkginfo__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:07:06.057505 cubicweb-web-1.3.0/test/data/cubicweb_file/data/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/data/cubicweb_file/data/file.png
+-rw-rw-rw-   0 root         (0) root         (0)     2000 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/data/cubicweb_file/entities.py
+-rw-rw-rw-   0 root         (0) root         (0)     2431 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/data/cubicweb_file/hooks.py
+-rw-rw-rw-   0 root         (0) root         (0)     1277 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/data/cubicweb_file/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)       43 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/data/cubicweb_file/uiprops.py
+-rw-rw-rw-   0 root         (0) root         (0)      387 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/data/cubicweb_file/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:07:06.057505 cubicweb-web-1.3.0/test/data/cubicweb_file/wdoc/
+-rw-rw-rw-   0 root         (0) root         (0)      185 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/data/cubicweb_file/wdoc/toc.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:07:06.061505 cubicweb-web-1.3.0/test/data/cubicweb_tag/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/data/cubicweb_tag/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       41 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/data/cubicweb_tag/__pkginfo__.py
+-rw-rw-rw-   0 root         (0) root         (0)      622 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/data/cubicweb_tag/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)      985 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/data/cubicweb_tag/views.py
+-rw-rw-rw-   0 root         (0) root         (0)     1836 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/data/entities.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:07:05.849501 cubicweb-web-1.3.0/test/data/libpython/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:07:06.061505 cubicweb-web-1.3.0/test/data/libpython/cubicweb_i18ntestcube/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/data/libpython/cubicweb_i18ntestcube/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      486 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/data/libpython/cubicweb_i18ntestcube/__pkginfo__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:07:06.065506 cubicweb-web-1.3.0/test/data/libpython/cubicweb_i18ntestcube/excludeme/
+-rw-rw-rw-   0 root         (0) root         (0)       39 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/data/libpython/cubicweb_i18ntestcube/excludeme/somefile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:07:06.065506 cubicweb-web-1.3.0/test/data/libpython/cubicweb_i18ntestcube/i18n/
+-rw-rw-rw-   0 root         (0) root         (0)     2657 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/data/libpython/cubicweb_i18ntestcube/i18n/en.po.ref
+-rw-rw-rw-   0 root         (0) root         (0)     1725 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/data/libpython/cubicweb_i18ntestcube/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     2266 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/data/libpython/cubicweb_i18ntestcube/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:07:06.065506 cubicweb-web-1.3.0/test/data/libpython/cubicweb_i18ntestcube-0.1.0.dist-info/
+-rw-rw-rw-   0 root         (0) root         (0)        4 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/data/libpython/cubicweb_i18ntestcube-0.1.0.dist-info/INSTALLER
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/data/libpython/cubicweb_i18ntestcube-0.1.0.dist-info/METADATA
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/data/libpython/cubicweb_i18ntestcube-0.1.0.dist-info/RECORD
+-rw-rw-rw-   0 root         (0) root         (0)       92 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/data/libpython/cubicweb_i18ntestcube-0.1.0.dist-info/WHEEL
+-rw-rw-rw-   0 root         (0) root         (0)      136 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/data/libpython/cubicweb_i18ntestcube-0.1.0.dist-info/entry_points.txt
+-rw-rw-rw-   0 root         (0) root         (0)       22 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/data/libpython/cubicweb_i18ntestcube-0.1.0.dist-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       67 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/data/pouet.css
+-rw-rw-rw-   0 root         (0) root         (0)     8663 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/data/schema.py
+-rw-rw-rw-   0 root         (0) root         (0)      133 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/data/sheet1.py
+-rw-rw-rw-   0 root         (0) root         (0)      109 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/data/sheet2.py
+-rw-rw-rw-   0 root         (0) root         (0)     2839 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/data/views.py
+-rw-rw-rw-   0 root         (0) root         (0)    35939 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/test_application.py
+-rw-rw-rw-   0 root         (0) root         (0)     2260 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/test_breadcrumbs.py
+-rw-rw-rw-   0 root         (0) root         (0)     3166 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/test_bw_request.py
+-rw-rw-rw-   0 root         (0) root         (0)     2319 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/test_controller.py
+-rw-rw-rw-   0 root         (0) root         (0)     4974 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/test_csrf.py
+-rw-rw-rw-   0 root         (0) root         (0)    12892 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/test_entity.py
+-rw-rw-rw-   0 root         (0) root         (0)    24397 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/test_facet.py
+-rw-rw-rw-   0 root         (0) root         (0)    17841 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/test_form.py
+-rw-rw-rw-   0 root         (0) root         (0)     9449 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/test_formfields.py
+-rw-rw-rw-   0 root         (0) root         (0)     3296 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/test_formwidgets.py
+-rw-rw-rw-   0 root         (0) root         (0)     9718 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/test_http.py
+-rw-rw-rw-   0 root         (0) root         (0)      563 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/test_http_headers.py
+-rw-rw-rw-   0 root         (0) root         (0)     2414 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/test_httptest.py
+-rw-rw-rw-   0 root         (0) root         (0)     1966 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/test_i18n.py
+-rw-rw-rw-   0 root         (0) root         (0)     6673 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/test_idownloadable.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:07:06.069506 cubicweb-web-1.3.0/test/test_js_scripts/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:07:06.073506 cubicweb-web-1.3.0/test/test_js_scripts/data/
+-rw-rw-rw-   0 root         (0) root         (0)       44 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/test_js_scripts/data/ajax_url0.html
+-rw-rw-rw-   0 root         (0) root         (0)      166 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/test_js_scripts/data/ajax_url1.html
+-rw-rw-rw-   0 root         (0) root         (0)       15 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/test_js_scripts/data/ajaxresult.json
+-rw-rw-rw-   0 root         (0) root         (0)     1071 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/test_js_scripts/data/test_htmlhelpers.html
+-rw-rw-rw-   0 root         (0) root         (0)     1008 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/test_js_scripts/data/test_utils.html
+-rw-rw-rw-   0 root         (0) root         (0)     6549 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/test_js_scripts/jest.config.js
+-rw-rw-rw-   0 root         (0) root         (0)   122226 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/test_js_scripts/package-lock.json
+-rw-rw-rw-   0 root         (0) root         (0)      336 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/test_js_scripts/package.json
+-rw-rw-rw-   0 root         (0) root         (0)      407 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/test_js_scripts/setup.js
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:07:06.073506 cubicweb-web-1.3.0/test/test_js_scripts/test/
+-rw-rw-rw-   0 root         (0) root         (0)     7373 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/test_js_scripts/test/ajax.test.js
+-rw-rw-rw-   0 root         (0) root         (0)     1242 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/test_js_scripts/test/htmlhelpers.test.js
+-rw-rw-rw-   0 root         (0) root         (0)      821 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/test_js_scripts/test/utils.js
+-rw-rw-rw-   0 root         (0) root         (0)     3723 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/test_js_scripts/test/utils.test.js
+-rw-rw-rw-   0 root         (0) root         (0)     4847 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/test_login.py
+-rw-rw-rw-   0 root         (0) root         (0)    13290 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/test_magicsearch.py
+-rw-rw-rw-   0 root         (0) root         (0)     6991 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/test_predicates.py
+-rw-rw-rw-   0 root         (0) root         (0)     2469 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/test_propertysheet.py
+-rw-rw-rw-   0 root         (0) root         (0)      958 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/test_pyramid.py
+-rw-rw-rw-   0 root         (0) root         (0)     3124 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/test_pyramid_hooks.py
+-rw-rw-rw-   0 root         (0) root         (0)     3122 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/test_pyramid_predicates.py
+-rw-rw-rw-   0 root         (0) root         (0)    23077 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/test_reledit.py
+-rw-rw-rw-   0 root         (0) root         (0)     6166 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/test_request.py
+-rw-rw-rw-   0 root         (0) root         (0)    10906 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/test_rest.py
+-rw-rw-rw-   0 root         (0) root         (0)     1452 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/test_rset.py
+-rw-rw-rw-   0 root         (0) root         (0)     5569 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/test_testlib.py
+-rw-rw-rw-   0 root         (0) root         (0)     9080 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/test_uicfg.py
+-rw-rw-rw-   0 root         (0) root         (0)     1332 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/test_url_redirection.py
+-rw-rw-rw-   0 root         (0) root         (0)     8483 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/test_urlpublisher.py
+-rw-rw-rw-   0 root         (0) root         (0)     9697 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/test_urlrewrite.py
+-rw-rw-rw-   0 root         (0) root         (0)     3147 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/test_views_actions.py
+-rw-rw-rw-   0 root         (0) root         (0)     2791 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/test_views_apacherewrite.py
+-rw-rw-rw-   0 root         (0) root         (0)    54787 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/test_views_basecontrollers.py
+-rw-rw-rw-   0 root         (0) root         (0)     2089 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/test_views_basetemplates.py
+-rw-rw-rw-   0 root         (0) root         (0)    13844 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/test_views_baseviews.py
+-rw-rw-rw-   0 root         (0) root         (0)     2265 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/test_views_csv.py
+-rw-rw-rw-   0 root         (0) root         (0)     2120 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/test_views_cwsources.py
+-rw-rw-rw-   0 root         (0) root         (0)     1796 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/test_views_debug_html.py
+-rw-rw-rw-   0 root         (0) root         (0)    19638 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/test_views_editforms.py
+-rw-rw-rw-   0 root         (0) root         (0)     3424 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/test_views_errorform.py
+-rw-rw-rw-   0 root         (0) root         (0)     4432 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/test_views_forms.py
+-rw-rw-rw-   0 root         (0) root         (0)     4536 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/test_views_json.py
+-rw-rw-rw-   0 root         (0) root         (0)     6177 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/test_views_navigation.py
+-rw-rw-rw-   0 root         (0) root         (0)     2113 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/test_views_pyviews.py
+-rw-rw-rw-   0 root         (0) root         (0)     4912 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/test_views_searchrestriction.py
+-rw-rw-rw-   0 root         (0) root         (0)     7239 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/test_views_staticcontrollers.py
+-rw-rw-rw-   0 root         (0) root         (0)     2030 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/test_views_treeview.py
+-rw-rw-rw-   0 root         (0) root         (0)      800 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/test_views_wdoc.py
+-rw-rw-rw-   0 root         (0) root         (0)     1560 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/test_views_xmlrss.py
+-rw-rw-rw-   0 root         (0) root         (0)    29065 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/test_viewselector.py
+-rw-rw-rw-   0 root         (0) root         (0)     3908 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/test_vregistry.py
+-rw-rw-rw-   0 root         (0) root         (0)     6074 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/test_web.py
+-rw-rw-rw-   0 root         (0) root         (0)     2914 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/test_webconfig.py
+-rw-rw-rw-   0 root         (0) root         (0)     1225 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/test_webtest.py
+-rw-rw-rw-   0 root         (0) root         (0)      719 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/testutils.js
+-rw-rw-rw-   0 root         (0) root         (0)     6438 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test/unittest_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:07:06.073506 cubicweb-web-1.3.0/test_auto/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test_auto/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-23 10:07:06.077506 cubicweb-web-1.3.0/test_auto/data/
+-rw-rw-rw-   0 root         (0) root         (0)        4 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test_auto/data/bootstrap_cubes
+-rw-rw-rw-   0 root         (0) root         (0)     3560 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/test_auto/test_views.py
+-rw-rw-rw-   0 root         (0) root         (0)     1794 2024-05-23 10:06:40.000000 cubicweb-web-1.3.0/tox.ini
```

### Comparing `cubicweb-web-1.2.9/MANIFEST.in` & `cubicweb-web-1.3.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/PKG-INFO` & `cubicweb-web-1.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cubicweb-web
-Version: 1.2.9
+Version: 1.3.0
 Summary: Legacy component for web application
 Home-page: https://forge.extranet.logilab.fr/cubicweb/cubes/web
 Author: LOGILAB S.A. (Paris, FRANCE)
 Author-email: contact@logilab.fr
 License: LGPL
 Classifier: Environment :: Web Environment
 Classifier: Framework :: CubicWeb
```

### Comparing `cubicweb-web-1.2.9/README.rst` & `cubicweb-web-1.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/__init__.py` & `cubicweb-web-1.3.0/cubicweb_web/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/__pkginfo__.py` & `cubicweb-web-1.3.0/cubicweb_web/__pkginfo__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # pylint: disable=W0622
 """cubicweb_web application packaging information"""
 
 
 modname = "web"
 distname = "cubicweb-web"
 
-numversion = (1, 2, 9)
+numversion = (1, 3, 0)
 version = ".".join(str(num) for num in numversion)
 
 license = "LGPL"
 author = "LOGILAB S.A. (Paris, FRANCE)"
 author_email = "contact@logilab.fr"
 description = "Legacy component for web application"
 web = "https://forge.extranet.logilab.fr/cubicweb/cubes/web"
```

### Comparing `cubicweb-web-1.2.9/cubicweb_web/_exceptions.py` & `cubicweb-web-1.3.0/cubicweb_web/_exceptions.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/action.py` & `cubicweb-web-1.3.0/cubicweb_web/action.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/application.py` & `cubicweb-web-1.3.0/cubicweb_web/application.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/box.py` & `cubicweb-web-1.3.0/cubicweb_web/box.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/bwcompat.py` & `cubicweb-web-1.3.0/cubicweb_web/bwcompat.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/captcha.py` & `cubicweb-web-1.3.0/cubicweb_web/captcha.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/ccplugin.py` & `cubicweb-web-1.3.0/cubicweb_web/ccplugin.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/component.py` & `cubicweb-web-1.3.0/cubicweb_web/component.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/controller.py` & `cubicweb-web-1.3.0/cubicweb_web/controller.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/banner.png` & `cubicweb-web-1.3.0/cubicweb_web/data/banner.png`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/black-check.png` & `cubicweb-web-1.3.0/cubicweb_web/data/black-check.png`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/black-uncheck.png` & `cubicweb-web-1.3.0/cubicweb_web/data/black-uncheck.png`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/cancel.png` & `cubicweb-web-1.3.0/cubicweb_web/data/cancel.png`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/cubicweb.acl.css` & `cubicweb-web-1.3.0/cubicweb_web/data/cubicweb.acl.css`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/cubicweb.ajax.box.js` & `cubicweb-web-1.3.0/cubicweb_web/data/cubicweb.ajax.box.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/cubicweb.ajax.js` & `cubicweb-web-1.3.0/cubicweb_web/data/cubicweb.ajax.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/cubicweb.calendar.css` & `cubicweb-web-1.3.0/cubicweb_web/data/cubicweb.calendar.css`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/cubicweb.calendar.js` & `cubicweb-web-1.3.0/cubicweb_web/data/cubicweb.calendar.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/cubicweb.calendar_popup.css` & `cubicweb-web-1.3.0/cubicweb_web/data/cubicweb.calendar_popup.css`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/cubicweb.compat.js` & `cubicweb-web-1.3.0/cubicweb_web/data/cubicweb.compat.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/cubicweb.css` & `cubicweb-web-1.3.0/cubicweb_web/data/cubicweb.css`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/cubicweb.edition.js` & `cubicweb-web-1.3.0/cubicweb_web/data/cubicweb.edition.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/cubicweb.facets.css` & `cubicweb-web-1.3.0/cubicweb_web/data/cubicweb.facets.css`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/cubicweb.facets.js` & `cubicweb-web-1.3.0/cubicweb_web/data/cubicweb.facets.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/cubicweb.fckcwconfig-full.js` & `cubicweb-web-1.3.0/cubicweb_web/data/cubicweb.fckcwconfig-full.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/cubicweb.fckcwconfig.js` & `cubicweb-web-1.3.0/cubicweb_web/data/cubicweb.fckcwconfig.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/cubicweb.flot.js` & `cubicweb-web-1.3.0/cubicweb_web/data/cubicweb.flot.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/cubicweb.form.css` & `cubicweb-web-1.3.0/cubicweb_web/data/cubicweb.form.css`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/cubicweb.html_tree.css` & `cubicweb-web-1.3.0/cubicweb_web/data/cubicweb.html_tree.css`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/cubicweb.htmlhelpers.js` & `cubicweb-web-1.3.0/cubicweb_web/data/cubicweb.htmlhelpers.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/cubicweb.ie.css` & `cubicweb-web-1.3.0/cubicweb_web/data/cubicweb.ie.css`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/cubicweb.image.js` & `cubicweb-web-1.3.0/cubicweb_web/data/cubicweb.image.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/cubicweb.js` & `cubicweb-web-1.3.0/cubicweb_web/data/cubicweb.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/cubicweb.log.css` & `cubicweb-web-1.3.0/cubicweb_web/data/cubicweb.log.css`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/cubicweb.login.css` & `cubicweb-web-1.3.0/cubicweb_web/data/cubicweb.login.css`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/cubicweb.pictograms.css` & `cubicweb-web-1.3.0/cubicweb_web/data/cubicweb.pictograms.css`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/cubicweb.preferences.css` & `cubicweb-web-1.3.0/cubicweb_web/data/cubicweb.preferences.css`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/cubicweb.preferences.js` & `cubicweb-web-1.3.0/cubicweb_web/data/cubicweb.preferences.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/cubicweb.python.js` & `cubicweb-web-1.3.0/cubicweb_web/data/cubicweb.python.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/cubicweb.reledit.js` & `cubicweb-web-1.3.0/cubicweb_web/data/cubicweb.reledit.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/cubicweb.schema.css` & `cubicweb-web-1.3.0/cubicweb_web/data/cubicweb.schema.css`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/cubicweb.suggest.css` & `cubicweb-web-1.3.0/cubicweb_web/data/cubicweb.suggest.css`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/cubicweb.tableview.css` & `cubicweb-web-1.3.0/cubicweb_web/data/cubicweb.tableview.css`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/cubicweb.timetable.css` & `cubicweb-web-1.3.0/cubicweb_web/data/cubicweb.timetable.css`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/cubicweb.widgets.js` & `cubicweb-web-1.3.0/cubicweb_web/data/cubicweb.widgets.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/download.gif` & `cubicweb-web-1.3.0/cubicweb_web/data/download.gif`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/dublincore-button.png` & `cubicweb-web-1.3.0/cubicweb_web/data/dublincore-button.png`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/dublincore-icon.png` & `cubicweb-web-1.3.0/cubicweb_web/data/dublincore-icon.png`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/entypo.eot` & `cubicweb-web-1.3.0/cubicweb_web/data/entypo.eot`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/entypo.svg` & `cubicweb-web-1.3.0/cubicweb_web/data/entypo.svg`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/entypo.ttf` & `cubicweb-web-1.3.0/cubicweb_web/data/entypo.ttf`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/entypo.woff` & `cubicweb-web-1.3.0/cubicweb_web/data/entypo.woff`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/error.png` & `cubicweb-web-1.3.0/cubicweb_web/data/error.png`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/excanvas.js` & `cubicweb-web-1.3.0/cubicweb_web/data/excanvas.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/favicon.ico` & `cubicweb-web-1.3.0/cubicweb_web/data/favicon.ico`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/feed-icon.png` & `cubicweb-web-1.3.0/cubicweb_web/data/feed-icon.png`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/feed-icon16x16.png` & `cubicweb-web-1.3.0/cubicweb_web/data/feed-icon16x16.png`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/feed-icon32x32.png` & `cubicweb-web-1.3.0/cubicweb_web/data/feed-icon32x32.png`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/fullcalendar.css` & `cubicweb-web-1.3.0/cubicweb_web/data/fullcalendar.css`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/fullcalendar.js` & `cubicweb-web-1.3.0/cubicweb_web/data/fullcalendar.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/fullcalendar.locale.js` & `cubicweb-web-1.3.0/cubicweb_web/data/fullcalendar.locale.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/fullcalendar.min.js` & `cubicweb-web-1.3.0/cubicweb_web/data/fullcalendar.min.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/fullcalendar.print.css` & `cubicweb-web-1.3.0/cubicweb_web/data/fullcalendar.print.css`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/go_next.png` & `cubicweb-web-1.3.0/cubicweb_web/data/go_next.png`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/go_prev.png` & `cubicweb-web-1.3.0/cubicweb_web/data/go_prev.png`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/gradient-grey.gif` & `cubicweb-web-1.3.0/cubicweb_web/data/gradient-grey.gif`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/help.png` & `cubicweb-web-1.3.0/cubicweb_web/data/help.png`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/help_ie.png` & `cubicweb-web-1.3.0/cubicweb_web/data/help_ie.png`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/icon_map.png` & `cubicweb-web-1.3.0/cubicweb_web/data/icon_map.png`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/images/animated-overlay.gif` & `cubicweb-web-1.3.0/cubicweb_web/data/images/animated-overlay.gif`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/images/ui-icons_222222_256x240.png` & `cubicweb-web-1.3.0/cubicweb_web/data/images/ui-icons_222222_256x240.png`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/images/ui-icons_2e83ff_256x240.png` & `cubicweb-web-1.3.0/cubicweb_web/data/images/ui-icons_2e83ff_256x240.png`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/images/ui-icons_454545_256x240.png` & `cubicweb-web-1.3.0/cubicweb_web/data/images/ui-icons_454545_256x240.png`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/images/ui-icons_888888_256x240.png` & `cubicweb-web-1.3.0/cubicweb_web/data/images/ui-icons_888888_256x240.png`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/images/ui-icons_cd0a0a_256x240.png` & `cubicweb-web-1.3.0/cubicweb_web/data/images/ui-icons_cd0a0a_256x240.png`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/jquery-migrate.js` & `cubicweb-web-1.3.0/cubicweb_web/data/jquery-migrate.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/jquery-treeview/changelog.md` & `cubicweb-web-1.3.0/cubicweb_web/data/jquery-treeview/changelog.md`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/jquery-treeview/images/ajax-loader.gif` & `cubicweb-web-1.3.0/cubicweb_web/data/jquery-treeview/images/ajax-loader.gif`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/jquery-treeview/images/treeview-black-line.gif` & `cubicweb-web-1.3.0/cubicweb_web/data/jquery-treeview/images/treeview-black-line.gif`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/jquery-treeview/images/treeview-default-line.gif` & `cubicweb-web-1.3.0/cubicweb_web/data/jquery-treeview/images/treeview-default-line.gif`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/jquery-treeview/images/treeview-famfamfam.gif` & `cubicweb-web-1.3.0/cubicweb_web/data/jquery-treeview/images/treeview-famfamfam.gif`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/jquery-treeview/images/treeview-gray-line.gif` & `cubicweb-web-1.3.0/cubicweb_web/data/jquery-treeview/images/treeview-gray-line.gif`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/jquery-treeview/images/treeview-red-line.gif` & `cubicweb-web-1.3.0/cubicweb_web/data/jquery-treeview/images/treeview-red-line.gif`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/jquery-treeview/jquery.treeview.async.js` & `cubicweb-web-1.3.0/cubicweb_web/data/jquery-treeview/jquery.treeview.async.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/jquery-treeview/jquery.treeview.css` & `cubicweb-web-1.3.0/cubicweb_web/data/jquery-treeview/jquery.treeview.css`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/jquery-treeview/jquery.treeview.edit.js` & `cubicweb-web-1.3.0/cubicweb_web/data/jquery-treeview/jquery.treeview.edit.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/jquery-treeview/jquery.treeview.js` & `cubicweb-web-1.3.0/cubicweb_web/data/jquery-treeview/jquery.treeview.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/jquery-treeview/jquery.treeview.sortable.js` & `cubicweb-web-1.3.0/cubicweb_web/data/jquery-treeview/jquery.treeview.sortable.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/jquery-treeview/readme.md` & `cubicweb-web-1.3.0/cubicweb_web/data/jquery-treeview/readme.md`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/jquery-treeview/screenshot.png` & `cubicweb-web-1.3.0/cubicweb_web/data/jquery-treeview/screenshot.png`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/jquery.cookie.js` & `cubicweb-web-1.3.0/cubicweb_web/data/jquery.cookie.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/jquery.flot.js` & `cubicweb-web-1.3.0/cubicweb_web/data/jquery.flot.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/jquery.js` & `cubicweb-web-1.3.0/cubicweb_web/data/jquery.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/jquery.qtip.js` & `cubicweb-web-1.3.0/cubicweb_web/data/jquery.qtip.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/jquery.qtip.min.js` & `cubicweb-web-1.3.0/cubicweb_web/data/jquery.qtip.min.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/jquery.tablesorter.js` & `cubicweb-web-1.3.0/cubicweb_web/data/jquery.tablesorter.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/jquery.timePicker.js` & `cubicweb-web-1.3.0/cubicweb_web/data/jquery.timePicker.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/jquery.timepicker.css` & `cubicweb-web-1.3.0/cubicweb_web/data/jquery.timepicker.css`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/jquery.ui.css` & `cubicweb-web-1.3.0/cubicweb_web/data/jquery.ui.css`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/jquery.ui.datepicker-de.js` & `cubicweb-web-1.3.0/cubicweb_web/data/jquery.ui.datepicker-de.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/jquery.ui.datepicker-es.js` & `cubicweb-web-1.3.0/cubicweb_web/data/jquery.ui.datepicker-es.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/jquery.ui.datepicker-fr.js` & `cubicweb-web-1.3.0/cubicweb_web/data/jquery.ui.datepicker-fr.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/jquery.ui.js` & `cubicweb-web-1.3.0/cubicweb_web/data/jquery.ui.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/liveclipboard-icon.png` & `cubicweb-web-1.3.0/cubicweb_web/data/liveclipboard-icon.png`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/loading.gif` & `cubicweb-web-1.3.0/cubicweb_web/data/loading.gif`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/logo-cubicweb-gray.svg` & `cubicweb-web-1.3.0/cubicweb_web/data/logo-cubicweb-gray.svg`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/logo-cubicweb-icon.svg` & `cubicweb-web-1.3.0/cubicweb_web/data/logo-cubicweb-icon.svg`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/logo-cubicweb-text.svg` & `cubicweb-web-1.3.0/cubicweb_web/data/logo-cubicweb-text.svg`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/logo-cubicweb.svg` & `cubicweb-web-1.3.0/cubicweb_web/data/logo-cubicweb.svg`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/logo-logilab.png` & `cubicweb-web-1.3.0/cubicweb_web/data/logo-logilab.png`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/logo.png` & `cubicweb-web-1.3.0/cubicweb_web/data/logo.png`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/microformats-button.png` & `cubicweb-web-1.3.0/cubicweb_web/data/microformats-button.png`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/microformats-icon.png` & `cubicweb-web-1.3.0/cubicweb_web/data/microformats-icon.png`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/minus.gif` & `cubicweb-web-1.3.0/cubicweb_web/data/minus.gif`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/ok.png` & `cubicweb-web-1.3.0/cubicweb_web/data/ok.png`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/plus.gif` & `cubicweb-web-1.3.0/cubicweb_web/data/plus.gif`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/porkys.ttf` & `cubicweb-web-1.3.0/cubicweb_web/data/porkys.ttf`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/pygments.css` & `cubicweb-web-1.3.0/cubicweb_web/data/pygments.css`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/rss-button.png` & `cubicweb-web-1.3.0/cubicweb_web/data/rss-button.png`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/sendcancel.png` & `cubicweb-web-1.3.0/cubicweb_web/data/sendcancel.png`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/sendok.png` & `cubicweb-web-1.3.0/cubicweb_web/data/sendok.png`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/trash_can.png` & `cubicweb-web-1.3.0/cubicweb_web/data/trash_can.png`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/trash_can_small.png` & `cubicweb-web-1.3.0/cubicweb_web/data/trash_can_small.png`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/ui.all.css` & `cubicweb-web-1.3.0/cubicweb_web/data/ui.all.css`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/uiprops.py` & `cubicweb-web-1.3.0/cubicweb_web/data/uiprops.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/data/upload.gif` & `cubicweb-web-1.3.0/cubicweb_web/data/upload.gif`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/devtools/testlib.py` & `cubicweb-web-1.3.0/cubicweb_web/devtools/testlib.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/ext/rest.py` & `cubicweb-web-1.3.0/cubicweb_web/ext/rest.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/facet.py` & `cubicweb-web-1.3.0/cubicweb_web/facet.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/form.py` & `cubicweb-web-1.3.0/cubicweb_web/form.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/formfields.py` & `cubicweb-web-1.3.0/cubicweb_web/formfields.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/formwidgets.py` & `cubicweb-web-1.3.0/cubicweb_web/formwidgets.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/htmlwidgets.py` & `cubicweb-web-1.3.0/cubicweb_web/htmlwidgets.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/http_headers.py` & `cubicweb-web-1.3.0/cubicweb_web/http_headers.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/httpcache.py` & `cubicweb-web-1.3.0/cubicweb_web/httpcache.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/i18n/de.po` & `cubicweb-web-1.3.0/cubicweb_web/i18n/de.po`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/i18n/en.po` & `cubicweb-web-1.3.0/cubicweb_web/i18n/en.po`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/i18n/es.po` & `cubicweb-web-1.3.0/cubicweb_web/i18n/es.po`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/i18n/fr.po` & `cubicweb-web-1.3.0/cubicweb_web/i18n/fr.po`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/i18n.py` & `cubicweb-web-1.3.0/cubicweb_web/i18n.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/predicates.py` & `cubicweb-web-1.3.0/cubicweb_web/predicates.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/propertysheet.py` & `cubicweb-web-1.3.0/cubicweb_web/propertysheet.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/pyramid/__init__.py` & `cubicweb-web-1.3.0/cubicweb_web/pyramid/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/pyramid/login.py` & `cubicweb-web-1.3.0/cubicweb_web/pyramid/login.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/pyramid/predicates.py` & `cubicweb-web-1.3.0/cubicweb_web/pyramid/predicates.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/pyramid/test.py` & `cubicweb-web-1.3.0/cubicweb_web/pyramid/test.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/pyramid/url_redirection.py` & `cubicweb-web-1.3.0/cubicweb_web/pyramid/url_redirection.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/request.py` & `cubicweb-web-1.3.0/cubicweb_web/request.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/schemaviewer.py` & `cubicweb-web-1.3.0/cubicweb_web/schemaviewer.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/uihelper.py` & `cubicweb-web-1.3.0/cubicweb_web/uihelper.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/utils.py` & `cubicweb-web-1.3.0/cubicweb_web/utils.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/view.py` & `cubicweb-web-1.3.0/cubicweb_web/view.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/views/__init__.py` & `cubicweb-web-1.3.0/cubicweb_web/views/__init__.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/views/_vid_by_mimetype.py` & `cubicweb-web-1.3.0/cubicweb_web/views/_vid_by_mimetype.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/views/actions.py` & `cubicweb-web-1.3.0/cubicweb_web/views/actions.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/views/ajaxcontroller.py` & `cubicweb-web-1.3.0/cubicweb_web/views/ajaxcontroller.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/views/ajaxedit.py` & `cubicweb-web-1.3.0/cubicweb_web/views/ajaxedit.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/views/apacherewrite.py` & `cubicweb-web-1.3.0/cubicweb_web/views/apacherewrite.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/views/authentication.py` & `cubicweb-web-1.3.0/cubicweb_web/views/authentication.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/views/autoform.py` & `cubicweb-web-1.3.0/cubicweb_web/views/autoform.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/views/basecomponents.py` & `cubicweb-web-1.3.0/cubicweb_web/views/basecomponents.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/views/basecontrollers.py` & `cubicweb-web-1.3.0/cubicweb_web/views/basecontrollers.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/views/basetemplates.py` & `cubicweb-web-1.3.0/cubicweb_web/views/basetemplates.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/views/baseviews.py` & `cubicweb-web-1.3.0/cubicweb_web/views/baseviews.py`

 * *Files 2% similar despite different names*

```diff
@@ -497,15 +497,15 @@
             self.w(" (<span>%s</span>", _("cw_source"))
             self.w(
                 ' <span class="value">%s</span>)', source.view("oneline"), escape=False
             )
             source_def = self._cw.source_defs()[source.name]
             if source_def.get("use-cwuri-as-url"):
                 self.w(
-                    ' <a href="%s">%s</span>', entity.cwuri, self._cw._("view original")
+                    ' <a href="%s">%s</a>', entity.cwuri, self._cw._("view original")
                 )
         self.w("</div>")
 
 
 class TreeItemView(ListItemView):
     __regid__ = "treeitem"
 
@@ -526,31 +526,31 @@
     def cell_call(self, row, col, **kwargs):
         entity = self.cw_rset.complete_entity(row, col)
         self.w(entity.view("incontext"))
         searched = self.cw_rset.searched_text()
         if searched is None:
             return
         searched = searched.lower()
-        highlighted = "<b>%s</b>" % searched
+        highlighted = "<b>%s</b>" % xml_escape(searched)
         for attr in entity.e_schema.indexable_attributes():
             try:
                 value = entity.printable_value(attr, format="text/plain").lower()
             except TransformError:
                 continue
             except Exception:
                 continue
             if searched in value:
                 contexts = []
                 for ctx in value.split(searched):
                     if len(ctx) > 30:
                         contexts.append("..." + ctx[-30:])
                     else:
                         contexts.append(ctx)
-                value = "\n" + highlighted.join(contexts)
-                self.w(xml_escape(value).replace("\n", "<br/>"))
+                self.w("<br/>")
+                self.w(highlighted.join(xml_escape(ctx) for ctx in contexts))
 
 
 class TooltipView(EntityView):
     """A entity view used in a tooltip"""
 
     __regid__ = "tooltip"
```

### Comparing `cubicweb-web-1.2.9/cubicweb_web/views/bookmark.py` & `cubicweb-web-1.3.0/cubicweb_web/views/bookmark.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/views/boxes.py` & `cubicweb-web-1.3.0/cubicweb_web/views/boxes.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/views/calendar.py` & `cubicweb-web-1.3.0/cubicweb_web/views/calendar.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/views/csvexport.py` & `cubicweb-web-1.3.0/cubicweb_web/views/csvexport.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/views/cwproperties.py` & `cubicweb-web-1.3.0/cubicweb_web/views/cwproperties.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/views/cwsources.py` & `cubicweb-web-1.3.0/cubicweb_web/views/cwsources.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/views/cwuser.py` & `cubicweb-web-1.3.0/cubicweb_web/views/cwuser.py`

 * *Files 4% similar despite different names*

```diff
@@ -160,16 +160,24 @@
         self.render_objtype_access(entity, "CWRelation", objtype_access, rql_cwrelation)
 
     def render_objtype_access(self, entity, objtype, objtype_access, rql):
         self.w("<h4>%s</h4>", self._cw._(objtype))
         for access_type in objtype_access[objtype]:
             rset = self._cw.execute(rql % access_type, {"e": entity.eid})
             if rset:
-                self.w("<div>%s:</div>", self._cw.__(access_type + "_permission"))
-                self.w("<div>%s</div><br/>", self._cw.view("csv", rset, "null"))
+                self.w(
+                    "<div>%s:</div>",
+                    self._cw.__(access_type + "_permission"),
+                    escape=False,
+                )
+                self.w(
+                    "<div>%s</div><br/>",
+                    self._cw.view("csv", rset, "null"),
+                    escape=False,
+                )
 
 
 class CWGroupInContextView(EntityView):
     __regid__ = "incontext"
     __select__ = is_instance("CWGroup")
 
     def entity_call(self, entity, **kwargs):
```

### Comparing `cubicweb-web-1.2.9/cubicweb_web/views/debug.py` & `cubicweb-web-1.3.0/cubicweb_web/views/debug.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/views/dotgraphview.py` & `cubicweb-web-1.3.0/cubicweb_web/views/dotgraphview.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/views/edit_attributes.pt` & `cubicweb-web-1.3.0/cubicweb_web/views/edit_attributes.pt`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/views/editcontroller.py` & `cubicweb-web-1.3.0/cubicweb_web/views/editcontroller.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/views/editforms.py` & `cubicweb-web-1.3.0/cubicweb_web/views/editforms.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/views/editviews.py` & `cubicweb-web-1.3.0/cubicweb_web/views/editviews.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/views/emailaddress.py` & `cubicweb-web-1.3.0/cubicweb_web/views/emailaddress.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/views/error.py` & `cubicweb-web-1.3.0/cubicweb_web/views/error.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/views/facets.py` & `cubicweb-web-1.3.0/cubicweb_web/views/facets.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/views/formrenderers.py` & `cubicweb-web-1.3.0/cubicweb_web/views/formrenderers.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/views/forms.py` & `cubicweb-web-1.3.0/cubicweb_web/views/forms.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/views/ibreadcrumbs.py` & `cubicweb-web-1.3.0/cubicweb_web/views/ibreadcrumbs.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/views/idownloadable.py` & `cubicweb-web-1.3.0/cubicweb_web/views/idownloadable.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/views/json.py` & `cubicweb-web-1.3.0/cubicweb_web/views/json.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 # FOR A PARTICULAR PURPOSE.  See the GNU Lesser General Public License for more
 # details.
 #
 # You should have received a copy of the GNU Lesser General Public License along
 # with CubicWeb.  If not, see <https://www.gnu.org/licenses/>.
 """json export views"""
 
+import sys
+import traceback
 
 from cubicweb import _
 from cubicweb.predicates import ExpectedValuePredicate, any_rset, empty_rset
 from cubicweb.uilib import rest_traceback
 from cubicweb.utils import json_dumps
 from cubicweb_web.view import EntityView, AnyRsetView
 from cubicweb_web.application import anonymized_request
@@ -149,14 +151,23 @@
 
     __select__ = management.ErrorView.__select__ & _requested_vid(
         "jsonexport", "ejsonexport"
     )
 
     def call(self):
         errmsg, exclass, excinfo = self._excinfo()
+        # displaying the exception of stderr for debugging
+        traceback.print_tb(tb=excinfo[-1])
+        print()
+        print(excinfo[1], file=sys.stderr)
+
         self.wdata(
             {
                 "errmsg": errmsg,
                 "exclass": exclass,
-                "traceback": rest_traceback(excinfo, errmsg),
+                "traceback": (
+                    rest_traceback(excinfo, errmsg)
+                    if self._cw.vreg.config.debugmode
+                    else "please see server log or activate debug mode"
+                ),
             }
         )
```

### Comparing `cubicweb-web-1.2.9/cubicweb_web/views/magicsearch.py` & `cubicweb-web-1.3.0/cubicweb_web/views/magicsearch.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/views/management.py` & `cubicweb-web-1.3.0/cubicweb_web/views/management.py`

 * *Files 3% similar despite different names*

```diff
@@ -131,45 +131,51 @@
         title = self._cw._("an error occurred")
         self.w("<h2>%s</h2>", title)
 
         ex, exclass, excinfo = self._excinfo()
         # save excinfo on req for easier debugging in interactive shell
         req.excinfo = ex, exclass, excinfo
 
-        if excinfo is not None and self._cw.vreg.config["print-traceback"]:
-            if exclass is None:
+        # if excinfo is not None, it's probably not a bug
+        if excinfo is None:
+            return
+
+        # only render traceback in debugmode
+        if self._cw.vreg.config.debugmode:
+            if self._cw.vreg.config["print-traceback"]:
+                if exclass is None:
+                    self.w(
+                        '<div class="tb">%s</div>',
+                        xml_escape(ex).replace("\n", "<br />"),
+                        escape=False,
+                    )
+                else:
+                    self.w(
+                        '<div class="tb">%s: %s</div>',
+                        xml_escape(exclass),
+                        xml_escape(ex).replace("\n", "<br />"),
+                        escape=False,
+                    )
+                self.w("<hr />")
                 self.w(
                     '<div class="tb">%s</div>',
-                    xml_escape(ex).replace("\n", "<br />"),
+                    html_traceback(excinfo, ex, ""),
                     escape=False,
                 )
             else:
                 self.w(
-                    '<div class="tb">%s: %s</div>',
-                    xml_escape(exclass),
+                    '<div class="tb">%s</div>',
                     xml_escape(ex).replace("\n", "<br />"),
                     escape=False,
                 )
-            self.w("<hr />")
-            self.w(
-                '<div class="tb">%s</div>',
-                html_traceback(excinfo, ex, ""),
-                escape=False,
-            )
         else:
             self.w(
-                '<div class="tb">%s</div>',
-                xml_escape(ex).replace("\n", "<br />"),
-                escape=False,
+                "<div>Error 500, please contact the server administrator for more information</div>"
             )
 
-        # if excinfo is not None, it's probably not a bug
-        if excinfo is None:
-            return
-
         # displaying the exception of stderr for debugging
         traceback.print_tb(tb=excinfo[-1])
         print()
         print(excinfo[1], file=sys.stderr)
 
         if self._cw.cnx:
             vcconf = self._cw.cnx.repo.get_versions()
```

### Comparing `cubicweb-web-1.2.9/cubicweb_web/views/navigation.py` & `cubicweb-web-1.3.0/cubicweb_web/views/navigation.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/views/owl.py` & `cubicweb-web-1.3.0/cubicweb_web/views/owl.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/views/plots.py` & `cubicweb-web-1.3.0/cubicweb_web/views/plots.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/views/primary.py` & `cubicweb-web-1.3.0/cubicweb_web/views/primary.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/views/pyviews.py` & `cubicweb-web-1.3.0/cubicweb_web/views/pyviews.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/views/rdf.py` & `cubicweb-web-1.3.0/cubicweb_web/views/rdf.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/views/reledit.py` & `cubicweb-web-1.3.0/cubicweb_web/views/reledit.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/views/schema.py` & `cubicweb-web-1.3.0/cubicweb_web/views/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/views/searchrestriction.py` & `cubicweb-web-1.3.0/cubicweb_web/views/searchrestriction.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/views/sessions.py` & `cubicweb-web-1.3.0/cubicweb_web/views/sessions.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/views/startup.py` & `cubicweb-web-1.3.0/cubicweb_web/views/startup.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/views/staticcontrollers.py` & `cubicweb-web-1.3.0/cubicweb_web/views/staticcontrollers.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/views/tableview.py` & `cubicweb-web-1.3.0/cubicweb_web/views/tableview.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/views/tabs.py` & `cubicweb-web-1.3.0/cubicweb_web/views/tabs.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/views/timetable.py` & `cubicweb-web-1.3.0/cubicweb_web/views/timetable.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/views/treeview.py` & `cubicweb-web-1.3.0/cubicweb_web/views/treeview.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/views/uicfg.py` & `cubicweb-web-1.3.0/cubicweb_web/views/uicfg.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/views/undohistory.py` & `cubicweb-web-1.3.0/cubicweb_web/views/undohistory.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/views/urlpublishing.py` & `cubicweb-web-1.3.0/cubicweb_web/views/urlpublishing.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/views/urlrewrite.py` & `cubicweb-web-1.3.0/cubicweb_web/views/urlrewrite.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/views/vcard.py` & `cubicweb-web-1.3.0/cubicweb_web/views/vcard.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/views/wdoc.py` & `cubicweb-web-1.3.0/cubicweb_web/views/wdoc.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/views/workflow.py` & `cubicweb-web-1.3.0/cubicweb_web/views/workflow.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/views/xbel.py` & `cubicweb-web-1.3.0/cubicweb_web/views/xbel.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/views/xmlrss.py` & `cubicweb-web-1.3.0/cubicweb_web/views/xmlrss.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/wdoc/about_en.rst` & `cubicweb-web-1.3.0/cubicweb_web/wdoc/about_en.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/wdoc/about_fr.rst` & `cubicweb-web-1.3.0/cubicweb_web/wdoc/about_fr.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/wdoc/advanced_usage_schema_fr.rst` & `cubicweb-web-1.3.0/cubicweb_web/wdoc/advanced_usage_schema_fr.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/wdoc/bookmarks_en.rst` & `cubicweb-web-1.3.0/cubicweb_web/wdoc/bookmarks_en.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/wdoc/bookmarks_fr.rst` & `cubicweb-web-1.3.0/cubicweb_web/wdoc/bookmarks_fr.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/wdoc/custom_view_en.rst` & `cubicweb-web-1.3.0/cubicweb_web/wdoc/custom_view_en.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/wdoc/custom_view_fr.rst` & `cubicweb-web-1.3.0/cubicweb_web/wdoc/custom_view_fr.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/wdoc/custom_view_rss_fr.rst` & `cubicweb-web-1.3.0/cubicweb_web/wdoc/custom_view_rss_fr.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/wdoc/glossary_fr.rst` & `cubicweb-web-1.3.0/cubicweb_web/wdoc/glossary_fr.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/wdoc/images/userprefs_en.png` & `cubicweb-web-1.3.0/cubicweb_web/wdoc/images/userprefs_en.png`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/wdoc/images/userprefs_fr.png` & `cubicweb-web-1.3.0/cubicweb_web/wdoc/images/userprefs_fr.png`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/wdoc/standard_usage_fr.rst` & `cubicweb-web-1.3.0/cubicweb_web/wdoc/standard_usage_fr.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/wdoc/toc.xml` & `cubicweb-web-1.3.0/cubicweb_web/wdoc/toc.xml`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/wdoc/tut_rql_en.rst` & `cubicweb-web-1.3.0/cubicweb_web/wdoc/tut_rql_en.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/wdoc/tut_rql_fr.rst` & `cubicweb-web-1.3.0/cubicweb_web/wdoc/tut_rql_fr.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/wdoc/userprefs_fr.rst` & `cubicweb-web-1.3.0/cubicweb_web/wdoc/userprefs_fr.rst`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web/webconfig.py` & `cubicweb-web-1.3.0/cubicweb_web/webconfig.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/cubicweb_web.egg-info/PKG-INFO` & `cubicweb-web-1.3.0/cubicweb_web.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cubicweb-web
-Version: 1.2.9
+Version: 1.3.0
 Summary: Legacy component for web application
 Home-page: https://forge.extranet.logilab.fr/cubicweb/cubes/web
 Author: LOGILAB S.A. (Paris, FRANCE)
 Author-email: contact@logilab.fr
 License: LGPL
 Classifier: Environment :: Web Environment
 Classifier: Framework :: CubicWeb
```

### Comparing `cubicweb-web-1.2.9/cubicweb_web.egg-info/SOURCES.txt` & `cubicweb-web-1.3.0/cubicweb_web.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/setup.py` & `cubicweb-web-1.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/test/data/cubicweb_blog/schema.py` & `cubicweb-web-1.3.0/test/data/cubicweb_blog/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/test/data/cubicweb_card/schema.py` & `cubicweb-web-1.3.0/test/data/cubicweb_card/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/test/data/cubicweb_file/entities.py` & `cubicweb-web-1.3.0/test/data/cubicweb_file/entities.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/test/data/cubicweb_file/hooks.py` & `cubicweb-web-1.3.0/test/data/cubicweb_file/hooks.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/test/data/cubicweb_file/schema.py` & `cubicweb-web-1.3.0/test/data/cubicweb_file/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/test/data/cubicweb_tag/schema.py` & `cubicweb-web-1.3.0/test/data/cubicweb_tag/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/test/data/cubicweb_tag/views.py` & `cubicweb-web-1.3.0/test/data/cubicweb_tag/views.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/test/data/entities.py` & `cubicweb-web-1.3.0/test/data/entities.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/test/data/libpython/cubicweb_i18ntestcube/i18n/en.po.ref` & `cubicweb-web-1.3.0/test/data/libpython/cubicweb_i18ntestcube/i18n/en.po.ref`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/test/data/libpython/cubicweb_i18ntestcube/schema.py` & `cubicweb-web-1.3.0/test/data/libpython/cubicweb_i18ntestcube/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/test/data/libpython/cubicweb_i18ntestcube/views.py` & `cubicweb-web-1.3.0/test/data/libpython/cubicweb_i18ntestcube/views.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/test/data/schema.py` & `cubicweb-web-1.3.0/test/data/schema.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/test/data/views.py` & `cubicweb-web-1.3.0/test/data/views.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/test/test_application.py` & `cubicweb-web-1.3.0/test/test_application.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/test/test_breadcrumbs.py` & `cubicweb-web-1.3.0/test/test_breadcrumbs.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/test/test_bw_request.py` & `cubicweb-web-1.3.0/test/test_bw_request.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/test/test_controller.py` & `cubicweb-web-1.3.0/test/test_controller.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/test/test_csrf.py` & `cubicweb-web-1.3.0/test/test_csrf.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/test/test_entity.py` & `cubicweb-web-1.3.0/test/test_entity.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/test/test_facet.py` & `cubicweb-web-1.3.0/test/test_facet.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/test/test_form.py` & `cubicweb-web-1.3.0/test/test_form.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/test/test_formfields.py` & `cubicweb-web-1.3.0/test/test_formfields.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/test/test_formwidgets.py` & `cubicweb-web-1.3.0/test/test_formwidgets.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/test/test_http.py` & `cubicweb-web-1.3.0/test/test_http.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/test/test_http_headers.py` & `cubicweb-web-1.3.0/test/test_http_headers.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/test/test_httptest.py` & `cubicweb-web-1.3.0/test/test_httptest.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/test/test_i18n.py` & `cubicweb-web-1.3.0/test/test_i18n.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/test/test_idownloadable.py` & `cubicweb-web-1.3.0/test/test_idownloadable.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/test/test_js_scripts/data/test_htmlhelpers.html` & `cubicweb-web-1.3.0/test/test_js_scripts/data/test_htmlhelpers.html`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/test/test_js_scripts/data/test_utils.html` & `cubicweb-web-1.3.0/test/test_js_scripts/data/test_utils.html`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/test/test_js_scripts/jest.config.js` & `cubicweb-web-1.3.0/test/test_js_scripts/jest.config.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/test/test_js_scripts/package-lock.json` & `cubicweb-web-1.3.0/test/test_js_scripts/package-lock.json`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/test/test_js_scripts/test/ajax.test.js` & `cubicweb-web-1.3.0/test/test_js_scripts/test/ajax.test.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/test/test_js_scripts/test/htmlhelpers.test.js` & `cubicweb-web-1.3.0/test/test_js_scripts/test/htmlhelpers.test.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/test/test_js_scripts/test/utils.js` & `cubicweb-web-1.3.0/test/test_js_scripts/test/utils.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/test/test_js_scripts/test/utils.test.js` & `cubicweb-web-1.3.0/test/test_js_scripts/test/utils.test.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/test/test_login.py` & `cubicweb-web-1.3.0/test/test_login.py`

 * *Files 5% similar despite different names*

```diff
@@ -89,15 +89,15 @@
     def test_same_site_lax_by_default(self):
         res = self.webapp.post(
             urljoin(BASE_URL, "login"),
             {"__login": self.admlogin, "__password": self.admpassword},
         )
         for cookie in res.headers.getall("Set-Cookie"):
             self.assertIn("SameSite=Lax", cookie)
-        self.assertTrue(len(res.headers.getall("Set-Cookie")) > 0)
+        self.assertGreater(len(res.headers.getall("Set-Cookie")), 0)
 
 
 class LoginRedirectionTC(PyramidWebCWTC):
     anonymous_allowed = False
 
     def setUp(self):
         self.route_prefix = urlparse(BASE_URL).path
@@ -129,14 +129,14 @@
     def test_same_site_set_from_config(self):
         res = self.webapp.post(
             urljoin(BASE_URL, "login"),
             {"__login": self.admlogin, "__password": self.admpassword},
         )
         for cookie in res.headers.getall("Set-Cookie"):
             self.assertIn("SameSite=None", cookie)
-        self.assertTrue(len(res.headers.getall("Set-Cookie")) > 0)
+        self.assertGreater(len(res.headers.getall("Set-Cookie")), 0)
 
 
 if __name__ == "__main__":
     from unittest import main
 
     main()
```

### Comparing `cubicweb-web-1.2.9/test/test_magicsearch.py` & `cubicweb-web-1.3.0/test/test_magicsearch.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/test/test_predicates.py` & `cubicweb-web-1.3.0/test/test_predicates.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/test/test_propertysheet.py` & `cubicweb-web-1.3.0/test/test_propertysheet.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/test/test_pyramid.py` & `cubicweb-web-1.3.0/test/test_pyramid.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/test/test_pyramid_hooks.py` & `cubicweb-web-1.3.0/test/test_pyramid_hooks.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/test/test_pyramid_predicates.py` & `cubicweb-web-1.3.0/test/test_pyramid_predicates.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/test/test_reledit.py` & `cubicweb-web-1.3.0/test/test_reledit.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/test/test_request.py` & `cubicweb-web-1.3.0/test/test_request.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/test/test_rest.py` & `cubicweb-web-1.3.0/test/test_rest.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/test/test_rset.py` & `cubicweb-web-1.3.0/test/test_rset.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/test/test_testlib.py` & `cubicweb-web-1.3.0/test/test_testlib.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/test/test_uicfg.py` & `cubicweb-web-1.3.0/test/test_uicfg.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,23 +144,23 @@
 
 class UicfgRegistryCWTC(WebCWTC):
     def test_default_uicfg_object(self):
         "CW default ui config objects must be registered in uicfg registry"
         onames = ("autoform_field", "autoform_section", "autoform_field_kwargs")
         for oname in onames:
             obj = self.vreg["uicfg"].select_or_none(oname)
-            self.assertTrue(obj is not None, "%s not found in uicfg registry" % oname)
+            self.assertIsNotNone(obj, "%s not found in uicfg registry" % oname)
 
     def test_custom_uicfg(self):
         ASRT = uicfg.AutoformSectionRelationTags
         custom_afs = ASRT()
         custom_afs.__select__ = ASRT.__select__ & ASRT.__select__
         self.vreg["uicfg"].register(custom_afs)
         obj = self.vreg["uicfg"].select_or_none("autoform_section")
-        self.assertTrue(obj is custom_afs)
+        self.assertIs(obj, custom_afs)
 
 
 def _schema():
     class Personne(EntityType):
         pass
 
     class Societe(EntityType):
```

### Comparing `cubicweb-web-1.2.9/test/test_url_redirection.py` & `cubicweb-web-1.3.0/test/test_url_redirection.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/test/test_urlpublisher.py` & `cubicweb-web-1.3.0/test/test_urlpublisher.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/test/test_urlrewrite.py` & `cubicweb-web-1.3.0/test/test_urlrewrite.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/test/test_views_actions.py` & `cubicweb-web-1.3.0/test/test_views_actions.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/test/test_views_apacherewrite.py` & `cubicweb-web-1.3.0/test/test_views_apacherewrite.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/test/test_views_basecontrollers.py` & `cubicweb-web-1.3.0/test/test_views_basecontrollers.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/test/test_views_basetemplates.py` & `cubicweb-web-1.3.0/test/test_views_basetemplates.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/test/test_views_baseviews.py` & `cubicweb-web-1.3.0/test/test_views_baseviews.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/test/test_views_csv.py` & `cubicweb-web-1.3.0/test/test_views_csv.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/test/test_views_cwsources.py` & `cubicweb-web-1.3.0/test/test_views_cwsources.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/test/test_views_debug_html.py` & `cubicweb-web-1.3.0/test/test_views_debug_html.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/test/test_views_editforms.py` & `cubicweb-web-1.3.0/test/test_views_editforms.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/test/test_views_errorform.py` & `cubicweb-web-1.3.0/test/test_views_errorform.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/test/test_views_forms.py` & `cubicweb-web-1.3.0/test/test_views_forms.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/test/test_views_json.py` & `cubicweb-web-1.3.0/test/test_views_json.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/test/test_views_navigation.py` & `cubicweb-web-1.3.0/test/test_views_navigation.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/test/test_views_pyviews.py` & `cubicweb-web-1.3.0/test/test_views_pyviews.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/test/test_views_searchrestriction.py` & `cubicweb-web-1.3.0/test/test_views_searchrestriction.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/test/test_views_staticcontrollers.py` & `cubicweb-web-1.3.0/test/test_views_staticcontrollers.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/test/test_views_treeview.py` & `cubicweb-web-1.3.0/test/test_views_treeview.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/test/test_views_wdoc.py` & `cubicweb-web-1.3.0/test/test_views_wdoc.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/test/test_views_xmlrss.py` & `cubicweb-web-1.3.0/test/test_views_xmlrss.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/test/test_viewselector.py` & `cubicweb-web-1.3.0/test/test_viewselector.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/test/test_vregistry.py` & `cubicweb-web-1.3.0/test/test_vregistry.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/test/test_web.py` & `cubicweb-web-1.3.0/test/test_web.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/test/test_webconfig.py` & `cubicweb-web-1.3.0/test/test_webconfig.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         self.config._cubes = ["file"]
         self.config.load_configuration()
 
     def test_nonregr_print_css_as_list(self):
         """make sure PRINT_CSS *must* is a list"""
         config = self.config
         print_css = config.uiprops["STYLESHEETS_PRINT"]
-        self.assertTrue(isinstance(print_css, list))
+        self.assertIsInstance(print_css, list)
 
     def test_locate_resource(self):
         self.assertIn("FILE_ICON", self.config.uiprops)
         rname = self.config.uiprops["FILE_ICON"].replace(self.config.datadir_url, "")
         self.assertIn(
             "cubicweb_file", self.config.locate_resource(rname)[0].split(os.sep)
         )
```

### Comparing `cubicweb-web-1.2.9/test/test_webtest.py` & `cubicweb-web-1.3.0/test/test_webtest.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/test/testutils.js` & `cubicweb-web-1.3.0/test/testutils.js`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/test/unittest_utils.py` & `cubicweb-web-1.3.0/test/unittest_utils.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/test_auto/test_views.py` & `cubicweb-web-1.3.0/test_auto/test_views.py`

 * *Files identical despite different names*

### Comparing `cubicweb-web-1.2.9/tox.ini` & `cubicweb-web-1.3.0/tox.ini`

 * *Files identical despite different names*

