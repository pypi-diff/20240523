# Comparing `tmp/zopyx_fastapi_auth-0.1.1.1.tar.gz` & `tmp/zopyx_fastapi_auth-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zopyx_fastapi_auth-0.1.1.1.tar", last modified: Tue May 21 18:22:29 2024, max compression
+gzip compressed data, was "zopyx_fastapi_auth-0.2.0.tar", last modified: Thu May 23 10:34:15 2024, max compression
```

## Comparing `zopyx_fastapi_auth-0.1.1.1.tar` & `zopyx_fastapi_auth-0.2.0.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwx------   0 ajung      (501) staff       (20)        0 2024-05-21 18:22:29.475366 zopyx_fastapi_auth-0.1.1.1/
--rw-------   0 ajung      (501) staff       (20)       27 2024-05-21 18:06:00.000000 zopyx_fastapi_auth-0.1.1.1/MANIFEST.in
--rw-r--r--   0 ajung      (501) staff       (20)     4686 2024-05-21 18:22:29.475000 zopyx_fastapi_auth-0.1.1.1/PKG-INFO
--rw-------   0 ajung      (501) staff       (20)     4183 2024-05-21 17:13:14.000000 zopyx_fastapi_auth-0.1.1.1/README.md
-drwx------   0 ajung      (501) staff       (20)        0 2024-05-21 18:22:29.393782 zopyx_fastapi_auth-0.1.1.1/fastapi_auth/
--rw-------   0 ajung      (501) staff       (20)       14 2024-05-19 14:39:22.000000 zopyx_fastapi_auth-0.1.1.1/fastapi_auth/__init__.py
--rw-r--r--   0 ajung      (501) staff       (20)      373 2024-05-21 15:46:25.000000 zopyx_fastapi_auth-0.1.1.1/fastapi_auth/auth_config.py
--rw-------   0 ajung      (501) staff       (20)     2828 2024-05-21 16:26:03.000000 zopyx_fastapi_auth-0.1.1.1/fastapi_auth/auth_routes.py
--rw-------   0 ajung      (501) staff       (20)     2849 2024-05-21 16:53:06.000000 zopyx_fastapi_auth-0.1.1.1/fastapi_auth/demo_app.py
--rw-------   0 ajung      (501) staff       (20)     1972 2024-05-21 17:09:49.000000 zopyx_fastapi_auth-0.1.1.1/fastapi_auth/dependencies.py
--rw-------   0 ajung      (501) staff       (20)      466 2024-05-21 00:44:36.000000 zopyx_fastapi_auth-0.1.1.1/fastapi_auth/jinja2_templates.py
--rw-------   0 ajung      (501) staff       (20)      106 2024-05-20 17:48:26.000000 zopyx_fastapi_auth-0.1.1.1/fastapi_auth/logger.py
--rw-------   0 ajung      (501) staff       (20)      294 2024-05-21 00:42:54.000000 zopyx_fastapi_auth-0.1.1.1/fastapi_auth/permissions.py
--rw-------   0 ajung      (501) staff       (20)     1722 2024-05-21 00:44:16.000000 zopyx_fastapi_auth-0.1.1.1/fastapi_auth/roles.py
--rw-------   0 ajung      (501) staff       (20)     2096 2024-05-21 15:48:34.000000 zopyx_fastapi_auth-0.1.1.1/fastapi_auth/user_cmd.py
--rw-------   0 ajung      (501) staff       (20)     4591 2024-05-21 15:48:28.000000 zopyx_fastapi_auth-0.1.1.1/fastapi_auth/user_management.py
--rw-------   0 ajung      (501) staff       (20)     1242 2024-05-21 16:49:33.000000 zopyx_fastapi_auth-0.1.1.1/fastapi_auth/users.py
--rw-------   0 ajung      (501) staff       (20)      728 2024-05-21 18:22:14.000000 zopyx_fastapi_auth-0.1.1.1/pyproject.toml
--rw-------   0 ajung      (501) staff       (20)       38 2024-05-21 18:22:29.475412 zopyx_fastapi_auth-0.1.1.1/setup.cfg
-drwx------   0 ajung      (501) staff       (20)        0 2024-05-21 18:22:29.387816 zopyx_fastapi_auth-0.1.1.1/static/
-drwx------   0 ajung      (501) staff       (20)        0 2024-05-21 18:22:29.388345 zopyx_fastapi_auth-0.1.1.1/static/bootstrap-5.3.3-dist/
-drwx------   0 ajung      (501) staff       (20)        0 2024-05-21 18:22:29.450226 zopyx_fastapi_auth-0.1.1.1/static/bootstrap-5.3.3-dist/css/
--rw-------   0 ajung      (501) staff       (20)    70329 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.1.1.1/static/bootstrap-5.3.3-dist/css/bootstrap-grid.css
--rw-------   0 ajung      (501) staff       (20)   203221 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.1.1.1/static/bootstrap-5.3.3-dist/css/bootstrap-grid.css.map
--rw-------   0 ajung      (501) staff       (20)    51795 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.1.1.1/static/bootstrap-5.3.3-dist/css/bootstrap-grid.min.css
--rw-------   0 ajung      (501) staff       (20)   115986 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.1.1.1/static/bootstrap-5.3.3-dist/css/bootstrap-grid.min.css.map
--rw-------   0 ajung      (501) staff       (20)    70403 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.1.1.1/static/bootstrap-5.3.3-dist/css/bootstrap-grid.rtl.css
--rw-------   0 ajung      (501) staff       (20)   203225 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.1.1.1/static/bootstrap-5.3.3-dist/css/bootstrap-grid.rtl.css.map
--rw-------   0 ajung      (501) staff       (20)    51870 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.1.1.1/static/bootstrap-5.3.3-dist/css/bootstrap-grid.rtl.min.css
--rw-------   0 ajung      (501) staff       (20)   116063 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.1.1.1/static/bootstrap-5.3.3-dist/css/bootstrap-grid.rtl.min.css.map
--rw-------   0 ajung      (501) staff       (20)    12065 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.1.1.1/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.css
--rw-------   0 ajung      (501) staff       (20)   129371 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.1.1.1/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.css.map
--rw-------   0 ajung      (501) staff       (20)    10126 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.1.1.1/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.min.css
--rw-------   0 ajung      (501) staff       (20)    51369 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.1.1.1/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.min.css.map
--rw-------   0 ajung      (501) staff       (20)    12058 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.1.1.1/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.rtl.css
--rw-------   0 ajung      (501) staff       (20)   129386 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.1.1.1/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.rtl.css.map
--rw-------   0 ajung      (501) staff       (20)    10198 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.1.1.1/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.rtl.min.css
--rw-------   0 ajung      (501) staff       (20)    63943 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.1.1.1/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.rtl.min.css.map
--rw-------   0 ajung      (501) staff       (20)   107823 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.1.1.1/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.css
--rw-------   0 ajung      (501) staff       (20)   267535 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.1.1.1/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.css.map
--rw-------   0 ajung      (501) staff       (20)    85352 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.1.1.1/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.min.css
--rw-------   0 ajung      (501) staff       (20)   180381 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.1.1.1/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.min.css.map
--rw-------   0 ajung      (501) staff       (20)   107691 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.1.1.1/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.rtl.css
--rw-------   0 ajung      (501) staff       (20)   267476 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.1.1.1/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.rtl.css.map
--rw-------   0 ajung      (501) staff       (20)    85281 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.1.1.1/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.rtl.min.css
--rw-------   0 ajung      (501) staff       (20)   180217 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.1.1.1/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.rtl.min.css.map
--rw-------   0 ajung      (501) staff       (20)   281046 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.1.1.1/static/bootstrap-5.3.3-dist/css/bootstrap.css
--rw-------   0 ajung      (501) staff       (20)   679755 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.1.1.1/static/bootstrap-5.3.3-dist/css/bootstrap.css.map
--rw-------   0 ajung      (501) staff       (20)   232803 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.1.1.1/static/bootstrap-5.3.3-dist/css/bootstrap.min.css
--rw-------   0 ajung      (501) staff       (20)   589892 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.1.1.1/static/bootstrap-5.3.3-dist/css/bootstrap.min.css.map
--rw-------   0 ajung      (501) staff       (20)   280259 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.1.1.1/static/bootstrap-5.3.3-dist/css/bootstrap.rtl.css
--rw-------   0 ajung      (501) staff       (20)   679615 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.1.1.1/static/bootstrap-5.3.3-dist/css/bootstrap.rtl.css.map
--rw-------   0 ajung      (501) staff       (20)   232911 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.1.1.1/static/bootstrap-5.3.3-dist/css/bootstrap.rtl.min.css
--rw-------   0 ajung      (501) staff       (20)   589087 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.1.1.1/static/bootstrap-5.3.3-dist/css/bootstrap.rtl.min.css.map
-drwx------   0 ajung      (501) staff       (20)        0 2024-05-21 18:22:29.462584 zopyx_fastapi_auth-0.1.1.1/static/bootstrap-5.3.3-dist/js/
--rw-------   0 ajung      (501) staff       (20)   207819 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.1.1.1/static/bootstrap-5.3.3-dist/js/bootstrap.bundle.js
--rw-------   0 ajung      (501) staff       (20)   444579 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.1.1.1/static/bootstrap-5.3.3-dist/js/bootstrap.bundle.js.map
--rw-------   0 ajung      (501) staff       (20)    80721 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.1.1.1/static/bootstrap-5.3.3-dist/js/bootstrap.bundle.min.js
--rw-------   0 ajung      (501) staff       (20)   332090 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.1.1.1/static/bootstrap-5.3.3-dist/js/bootstrap.bundle.min.js.map
--rw-------   0 ajung      (501) staff       (20)   135829 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.1.1.1/static/bootstrap-5.3.3-dist/js/bootstrap.esm.js
--rw-------   0 ajung      (501) staff       (20)   305438 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.1.1.1/static/bootstrap-5.3.3-dist/js/bootstrap.esm.js.map
--rw-------   0 ajung      (501) staff       (20)    73935 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.1.1.1/static/bootstrap-5.3.3-dist/js/bootstrap.esm.min.js
--rw-------   0 ajung      (501) staff       (20)   222455 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.1.1.1/static/bootstrap-5.3.3-dist/js/bootstrap.esm.min.js.map
--rw-------   0 ajung      (501) staff       (20)   145401 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.1.1.1/static/bootstrap-5.3.3-dist/js/bootstrap.js
--rw-------   0 ajung      (501) staff       (20)   306606 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.1.1.1/static/bootstrap-5.3.3-dist/js/bootstrap.js.map
--rw-------   0 ajung      (501) staff       (20)    60635 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.1.1.1/static/bootstrap-5.3.3-dist/js/bootstrap.min.js
--rw-------   0 ajung      (501) staff       (20)   220561 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.1.1.1/static/bootstrap-5.3.3-dist/js/bootstrap.min.js.map
-drwx------   0 ajung      (501) staff       (20)        0 2024-05-21 18:22:29.474367 zopyx_fastapi_auth-0.1.1.1/zopyx_fastapi_auth.egg-info/
--rw-r--r--   0 ajung      (501) staff       (20)     4686 2024-05-21 18:22:29.000000 zopyx_fastapi_auth-0.1.1.1/zopyx_fastapi_auth.egg-info/PKG-INFO
--rw-------   0 ajung      (501) staff       (20)     3070 2024-05-21 18:22:29.000000 zopyx_fastapi_auth-0.1.1.1/zopyx_fastapi_auth.egg-info/SOURCES.txt
--rw-------   0 ajung      (501) staff       (20)        1 2024-05-21 18:22:29.000000 zopyx_fastapi_auth-0.1.1.1/zopyx_fastapi_auth.egg-info/dependency_links.txt
--rw-------   0 ajung      (501) staff       (20)       71 2024-05-21 18:22:29.000000 zopyx_fastapi_auth-0.1.1.1/zopyx_fastapi_auth.egg-info/entry_points.txt
--rw-------   0 ajung      (501) staff       (20)      124 2024-05-21 18:22:29.000000 zopyx_fastapi_auth-0.1.1.1/zopyx_fastapi_auth.egg-info/requires.txt
--rw-------   0 ajung      (501) staff       (20)       13 2024-05-21 18:22:29.000000 zopyx_fastapi_auth-0.1.1.1/zopyx_fastapi_auth.egg-info/top_level.txt
+drwx------   0 ajung     (1000) ajung     (1000)        0 2024-05-23 10:34:15.038082 zopyx_fastapi_auth-0.2.0/
+-rw-------   0 ajung     (1000) ajung     (1000)       27 2024-05-23 05:55:07.000000 zopyx_fastapi_auth-0.2.0/MANIFEST.in
+-rw-r--r--   0 ajung     (1000) ajung     (1000)     5033 2024-05-23 10:34:15.038082 zopyx_fastapi_auth-0.2.0/PKG-INFO
+-rw-------   0 ajung     (1000) ajung     (1000)     4183 2024-05-23 05:55:07.000000 zopyx_fastapi_auth-0.2.0/README.md
+drwx------   0 ajung     (1000) ajung     (1000)        0 2024-05-23 10:34:15.030081 zopyx_fastapi_auth-0.2.0/fastapi_auth/
+-rw-------   0 ajung     (1000) ajung     (1000)       14 2024-05-23 05:55:07.000000 zopyx_fastapi_auth-0.2.0/fastapi_auth/__init__.py
+-rw-------   0 ajung     (1000) ajung     (1000)      336 2024-05-23 09:47:35.000000 zopyx_fastapi_auth-0.2.0/fastapi_auth/auth_config.py
+-rw-------   0 ajung     (1000) ajung     (1000)     2856 2024-05-23 09:44:02.000000 zopyx_fastapi_auth-0.2.0/fastapi_auth/auth_routes.py
+-rw-------   0 ajung     (1000) ajung     (1000)     3008 2024-05-23 09:24:56.000000 zopyx_fastapi_auth-0.2.0/fastapi_auth/demo_app.py
+-rw-------   0 ajung     (1000) ajung     (1000)     2465 2024-05-23 05:55:07.000000 zopyx_fastapi_auth-0.2.0/fastapi_auth/dependencies.py
+-rw-------   0 ajung     (1000) ajung     (1000)      290 2024-05-23 05:55:07.000000 zopyx_fastapi_auth-0.2.0/fastapi_auth/jinja2_templates.py
+-rw-------   0 ajung     (1000) ajung     (1000)      106 2024-05-23 05:55:07.000000 zopyx_fastapi_auth-0.2.0/fastapi_auth/logger.py
+-rw-------   0 ajung     (1000) ajung     (1000)      294 2024-05-23 05:55:07.000000 zopyx_fastapi_auth-0.2.0/fastapi_auth/permissions.py
+-rw-------   0 ajung     (1000) ajung     (1000)     1716 2024-05-23 05:55:07.000000 zopyx_fastapi_auth-0.2.0/fastapi_auth/roles.py
+-rw-------   0 ajung     (1000) ajung     (1000)     2163 2024-05-23 09:54:30.000000 zopyx_fastapi_auth-0.2.0/fastapi_auth/user_cmd.py
+-rw-------   0 ajung     (1000) ajung     (1000)     2778 2024-05-23 09:57:10.000000 zopyx_fastapi_auth-0.2.0/fastapi_auth/user_management_sqlobject.py
+-rw-------   0 ajung     (1000) ajung     (1000)     1242 2024-05-23 05:55:07.000000 zopyx_fastapi_auth-0.2.0/fastapi_auth/users.py
+-rw-------   0 ajung     (1000) ajung     (1000)      969 2024-05-23 10:33:20.000000 zopyx_fastapi_auth-0.2.0/pyproject.toml
+-rw-------   0 ajung     (1000) ajung     (1000)       38 2024-05-23 10:34:15.038082 zopyx_fastapi_auth-0.2.0/setup.cfg
+drwx------   0 ajung     (1000) ajung     (1000)        0 2024-05-23 10:34:15.030081 zopyx_fastapi_auth-0.2.0/static/
+drwx------   0 ajung     (1000) ajung     (1000)        0 2024-05-23 10:34:15.030081 zopyx_fastapi_auth-0.2.0/static/bootstrap-5.3.3-dist/
+drwx------   0 ajung     (1000) ajung     (1000)        0 2024-05-23 10:34:15.038082 zopyx_fastapi_auth-0.2.0/static/bootstrap-5.3.3-dist/css/
+-rw-------   0 ajung     (1000) ajung     (1000)    70329 2024-05-23 05:55:07.000000 zopyx_fastapi_auth-0.2.0/static/bootstrap-5.3.3-dist/css/bootstrap-grid.css
+-rw-------   0 ajung     (1000) ajung     (1000)   203221 2024-05-23 05:55:07.000000 zopyx_fastapi_auth-0.2.0/static/bootstrap-5.3.3-dist/css/bootstrap-grid.css.map
+-rw-------   0 ajung     (1000) ajung     (1000)    51795 2024-05-23 05:55:07.000000 zopyx_fastapi_auth-0.2.0/static/bootstrap-5.3.3-dist/css/bootstrap-grid.min.css
+-rw-------   0 ajung     (1000) ajung     (1000)   115986 2024-05-23 05:55:07.000000 zopyx_fastapi_auth-0.2.0/static/bootstrap-5.3.3-dist/css/bootstrap-grid.min.css.map
+-rw-------   0 ajung     (1000) ajung     (1000)    70403 2024-05-23 05:55:07.000000 zopyx_fastapi_auth-0.2.0/static/bootstrap-5.3.3-dist/css/bootstrap-grid.rtl.css
+-rw-------   0 ajung     (1000) ajung     (1000)   203225 2024-05-23 05:55:07.000000 zopyx_fastapi_auth-0.2.0/static/bootstrap-5.3.3-dist/css/bootstrap-grid.rtl.css.map
+-rw-------   0 ajung     (1000) ajung     (1000)    51870 2024-05-23 05:55:07.000000 zopyx_fastapi_auth-0.2.0/static/bootstrap-5.3.3-dist/css/bootstrap-grid.rtl.min.css
+-rw-------   0 ajung     (1000) ajung     (1000)   116063 2024-05-23 05:55:07.000000 zopyx_fastapi_auth-0.2.0/static/bootstrap-5.3.3-dist/css/bootstrap-grid.rtl.min.css.map
+-rw-------   0 ajung     (1000) ajung     (1000)    12065 2024-05-23 05:55:07.000000 zopyx_fastapi_auth-0.2.0/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.css
+-rw-------   0 ajung     (1000) ajung     (1000)   129371 2024-05-23 05:55:07.000000 zopyx_fastapi_auth-0.2.0/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.css.map
+-rw-------   0 ajung     (1000) ajung     (1000)    10126 2024-05-23 05:55:07.000000 zopyx_fastapi_auth-0.2.0/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.min.css
+-rw-------   0 ajung     (1000) ajung     (1000)    51369 2024-05-23 05:55:07.000000 zopyx_fastapi_auth-0.2.0/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.min.css.map
+-rw-------   0 ajung     (1000) ajung     (1000)    12058 2024-05-23 05:55:07.000000 zopyx_fastapi_auth-0.2.0/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.rtl.css
+-rw-------   0 ajung     (1000) ajung     (1000)   129386 2024-05-23 05:55:07.000000 zopyx_fastapi_auth-0.2.0/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.rtl.css.map
+-rw-------   0 ajung     (1000) ajung     (1000)    10198 2024-05-23 05:55:07.000000 zopyx_fastapi_auth-0.2.0/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.rtl.min.css
+-rw-------   0 ajung     (1000) ajung     (1000)    63943 2024-05-23 05:55:07.000000 zopyx_fastapi_auth-0.2.0/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.rtl.min.css.map
+-rw-------   0 ajung     (1000) ajung     (1000)   107823 2024-05-23 05:55:07.000000 zopyx_fastapi_auth-0.2.0/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.css
+-rw-------   0 ajung     (1000) ajung     (1000)   267535 2024-05-23 05:55:07.000000 zopyx_fastapi_auth-0.2.0/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.css.map
+-rw-------   0 ajung     (1000) ajung     (1000)    85352 2024-05-23 05:55:07.000000 zopyx_fastapi_auth-0.2.0/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.min.css
+-rw-------   0 ajung     (1000) ajung     (1000)   180381 2024-05-23 05:55:07.000000 zopyx_fastapi_auth-0.2.0/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.min.css.map
+-rw-------   0 ajung     (1000) ajung     (1000)   107691 2024-05-23 05:55:07.000000 zopyx_fastapi_auth-0.2.0/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.rtl.css
+-rw-------   0 ajung     (1000) ajung     (1000)   267476 2024-05-23 05:55:07.000000 zopyx_fastapi_auth-0.2.0/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.rtl.css.map
+-rw-------   0 ajung     (1000) ajung     (1000)    85281 2024-05-23 05:55:07.000000 zopyx_fastapi_auth-0.2.0/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.rtl.min.css
+-rw-------   0 ajung     (1000) ajung     (1000)   180217 2024-05-23 05:55:07.000000 zopyx_fastapi_auth-0.2.0/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.rtl.min.css.map
+-rw-------   0 ajung     (1000) ajung     (1000)   281046 2024-05-23 05:55:07.000000 zopyx_fastapi_auth-0.2.0/static/bootstrap-5.3.3-dist/css/bootstrap.css
+-rw-------   0 ajung     (1000) ajung     (1000)   679755 2024-05-23 05:55:07.000000 zopyx_fastapi_auth-0.2.0/static/bootstrap-5.3.3-dist/css/bootstrap.css.map
+-rw-------   0 ajung     (1000) ajung     (1000)   232803 2024-05-23 05:55:07.000000 zopyx_fastapi_auth-0.2.0/static/bootstrap-5.3.3-dist/css/bootstrap.min.css
+-rw-------   0 ajung     (1000) ajung     (1000)   589892 2024-05-23 05:55:07.000000 zopyx_fastapi_auth-0.2.0/static/bootstrap-5.3.3-dist/css/bootstrap.min.css.map
+-rw-------   0 ajung     (1000) ajung     (1000)   280259 2024-05-23 05:55:07.000000 zopyx_fastapi_auth-0.2.0/static/bootstrap-5.3.3-dist/css/bootstrap.rtl.css
+-rw-------   0 ajung     (1000) ajung     (1000)   679615 2024-05-23 05:55:07.000000 zopyx_fastapi_auth-0.2.0/static/bootstrap-5.3.3-dist/css/bootstrap.rtl.css.map
+-rw-------   0 ajung     (1000) ajung     (1000)   232911 2024-05-23 05:55:07.000000 zopyx_fastapi_auth-0.2.0/static/bootstrap-5.3.3-dist/css/bootstrap.rtl.min.css
+-rw-------   0 ajung     (1000) ajung     (1000)   589087 2024-05-23 05:55:07.000000 zopyx_fastapi_auth-0.2.0/static/bootstrap-5.3.3-dist/css/bootstrap.rtl.min.css.map
+drwx------   0 ajung     (1000) ajung     (1000)        0 2024-05-23 10:34:15.038082 zopyx_fastapi_auth-0.2.0/static/bootstrap-5.3.3-dist/js/
+-rw-------   0 ajung     (1000) ajung     (1000)   207819 2024-05-23 05:55:07.000000 zopyx_fastapi_auth-0.2.0/static/bootstrap-5.3.3-dist/js/bootstrap.bundle.js
+-rw-------   0 ajung     (1000) ajung     (1000)   444579 2024-05-23 05:55:07.000000 zopyx_fastapi_auth-0.2.0/static/bootstrap-5.3.3-dist/js/bootstrap.bundle.js.map
+-rw-------   0 ajung     (1000) ajung     (1000)    80721 2024-05-23 05:55:07.000000 zopyx_fastapi_auth-0.2.0/static/bootstrap-5.3.3-dist/js/bootstrap.bundle.min.js
+-rw-------   0 ajung     (1000) ajung     (1000)   332090 2024-05-23 05:55:07.000000 zopyx_fastapi_auth-0.2.0/static/bootstrap-5.3.3-dist/js/bootstrap.bundle.min.js.map
+-rw-------   0 ajung     (1000) ajung     (1000)   135829 2024-05-23 05:55:07.000000 zopyx_fastapi_auth-0.2.0/static/bootstrap-5.3.3-dist/js/bootstrap.esm.js
+-rw-------   0 ajung     (1000) ajung     (1000)   305438 2024-05-23 05:55:07.000000 zopyx_fastapi_auth-0.2.0/static/bootstrap-5.3.3-dist/js/bootstrap.esm.js.map
+-rw-------   0 ajung     (1000) ajung     (1000)    73935 2024-05-23 05:55:07.000000 zopyx_fastapi_auth-0.2.0/static/bootstrap-5.3.3-dist/js/bootstrap.esm.min.js
+-rw-------   0 ajung     (1000) ajung     (1000)   222455 2024-05-23 05:55:07.000000 zopyx_fastapi_auth-0.2.0/static/bootstrap-5.3.3-dist/js/bootstrap.esm.min.js.map
+-rw-------   0 ajung     (1000) ajung     (1000)   145401 2024-05-23 05:55:07.000000 zopyx_fastapi_auth-0.2.0/static/bootstrap-5.3.3-dist/js/bootstrap.js
+-rw-------   0 ajung     (1000) ajung     (1000)   306606 2024-05-23 05:55:07.000000 zopyx_fastapi_auth-0.2.0/static/bootstrap-5.3.3-dist/js/bootstrap.js.map
+-rw-------   0 ajung     (1000) ajung     (1000)    60635 2024-05-23 05:55:07.000000 zopyx_fastapi_auth-0.2.0/static/bootstrap-5.3.3-dist/js/bootstrap.min.js
+-rw-------   0 ajung     (1000) ajung     (1000)   220561 2024-05-23 05:55:07.000000 zopyx_fastapi_auth-0.2.0/static/bootstrap-5.3.3-dist/js/bootstrap.min.js.map
+drwx------   0 ajung     (1000) ajung     (1000)        0 2024-05-23 10:34:15.038082 zopyx_fastapi_auth-0.2.0/zopyx_fastapi_auth.egg-info/
+-rw-r--r--   0 ajung     (1000) ajung     (1000)     5033 2024-05-23 10:34:15.000000 zopyx_fastapi_auth-0.2.0/zopyx_fastapi_auth.egg-info/PKG-INFO
+-rw-------   0 ajung     (1000) ajung     (1000)     3080 2024-05-23 10:34:15.000000 zopyx_fastapi_auth-0.2.0/zopyx_fastapi_auth.egg-info/SOURCES.txt
+-rw-------   0 ajung     (1000) ajung     (1000)        1 2024-05-23 10:34:15.000000 zopyx_fastapi_auth-0.2.0/zopyx_fastapi_auth.egg-info/dependency_links.txt
+-rw-------   0 ajung     (1000) ajung     (1000)       71 2024-05-23 10:34:15.000000 zopyx_fastapi_auth-0.2.0/zopyx_fastapi_auth.egg-info/entry_points.txt
+-rw-------   0 ajung     (1000) ajung     (1000)      173 2024-05-23 10:34:15.000000 zopyx_fastapi_auth-0.2.0/zopyx_fastapi_auth.egg-info/requires.txt
+-rw-------   0 ajung     (1000) ajung     (1000)       13 2024-05-23 10:34:15.000000 zopyx_fastapi_auth-0.2.0/zopyx_fastapi_auth.egg-info/top_level.txt
```

### Comparing `zopyx_fastapi_auth-0.1.1.1/PKG-INFO` & `zopyx_fastapi_auth-0.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,35 @@
 Metadata-Version: 2.1
 Name: zopyx-fastapi-auth
-Version: 0.1.1.1
+Version: 0.2.0
 Summary: FastAPI authentication and authorization
 Author-email: Andreas Jung <info@zopyx.com>
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 Requires-Dist: fastapi
 Requires-Dist: pydantic
 Requires-Dist: pydantic-settings
 Requires-Dist: uvicorn
 Requires-Dist: markdown
 Requires-Dist: starlette-session
 Requires-Dist: loguru
 Requires-Dist: bcrypt
 Requires-Dist: jinja2
+Requires-Dist: sqlmodel
+Requires-Dist: rich
 Requires-Dist: python-multipart
 Requires-Dist: typer
 Requires-Dist: typeguard
+Provides-Extra: dev
+Requires-Dist: tox; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: ruff; extra == "dev"
+Requires-Dist: twine; extra == "dev"
+Requires-Dist: build; extra == "dev"
 
 # fastapi-auth
 
 An opionated authentication and authorization system for FastAPI.
 
 ## Features
```

### Comparing `zopyx_fastapi_auth-0.1.1.1/README.md` & `zopyx_fastapi_auth-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.1.1.1/fastapi_auth/auth_routes.py` & `zopyx_fastapi_auth-0.2.0/fastapi_auth/auth_routes.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,18 @@
+from typing import Optional
+
 from fastapi import Depends, Form, Request, APIRouter
 from fastapi.responses import HTMLResponse, RedirectResponse
 from starlette import status
 from datetime import timedelta
 
 from .dependencies import get_user
 from .logger import LOG
 from .users import User, ANONYMOUS_USER
-from .user_management import UserManagement
+from .user_management_sqlobject import UserManagement
 from .jinja2_templates import templates
 from .roles import ROLES_REGISTRY
 from datetime import datetime, timezone
 
 from starlette.middleware.sessions import SessionMiddleware
 
 from .auth_config import AUTH_SETTINGS
@@ -25,21 +27,21 @@
     app.add_middleware(SessionMiddleware, secret_key=AUTH_SETTINGS.secret_key.get_secret_value())
 
 
 @router.get("/login", response_class=HTMLResponse)
 async def login(
     request: Request,
     user: User = Depends(get_user),
-    message: str = None,
-    error_message: str = None,
+    message: Optional[str] = None,
+    error_message: Optional[str] = None,
 ):
     return templates.TemplateResponse(
+        request,
         "login.html",
         {
-            "request": request,
             "user": user,
             "message": message,
             "error_message": error_message,
         },
     )
 
 
@@ -56,15 +58,15 @@
 @router.post("/login")
 async def login_post(
     request: Request,
     username: str = Form(...),
     password: str = Form(...),
     user: User = Depends(get_user),
 ):
-    um = UserManagement(AUTH_SETTINGS.db_name)
+    um = UserManagement(AUTH_SETTINGS.db_uri)
     user_data = um.get_user(username, password)
 
     if user_data is not None:
         roles = user_data["roles"]
         roles = [ROLES_REGISTRY.get_role(r) for r in roles if ROLES_REGISTRY.has_role(r)]
 
         now = datetime.now(timezone.utc)
@@ -85,14 +87,14 @@
         LOG.info(f"User {user_data['username']} logged in")
         return RedirectResponse(f"/?message={message}", status_code=status.HTTP_302_FOUND)
 
     else:
         message = f"You {username} could not be logged in. Please try again."
         LOG.error(message)
         return templates.TemplateResponse(
+            request,
             "login.html",
             {
                 "user": ANONYMOUS_USER,
-                "request": request,
                 "error_message": message,
             },
         )
```

### Comparing `zopyx_fastapi_auth-0.1.1.1/fastapi_auth/demo_app.py` & `zopyx_fastapi_auth-0.2.0/fastapi_auth/demo_app.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """This is a demo app to show how to use the fastapi_auth package."""
 
+from typing import Optional
+
 from fastapi import FastAPI, Depends, Request
 from fastapi.staticfiles import StaticFiles
 from starlette.responses import HTMLResponse
 
 from .auth_routes import router as auth_router, install_middleware
 from .dependencies import get_user
 from .users import User
@@ -20,17 +22,26 @@
 # add endpoints for authentication examples
 app.mount("/auth", auth_router)
 
 # add static files (for demo login form)
 app.mount("/static", StaticFiles(directory="static"), name="static")
 
 # here, we define some permissions
-VIEW_PERMISSION = Permission(name="view", description="View permission")
-EDIT_PERMISSION = Permission(name="edit", description="Edit permission")
-DELETE_PERMISSION = Permission(name="delete", description="Delete permission")
+VIEW_PERMISSION = Permission(
+    name="view",
+    description="View permission",
+)
+EDIT_PERMISSION = Permission(
+    name="edit",
+    description="Edit permission",
+)
+DELETE_PERMISSION = Permission(
+    name="delete",
+    description="Delete permission",
+)
 
 # and some roles that use these permissions
 ADMIN_ROLE = Role(
     name="Administrator",
     description="Admin role",
     permissions=[VIEW_PERMISSION, EDIT_PERMISSION, DELETE_PERMISSION],
 )
@@ -58,28 +69,34 @@
 # ANONYMOUS_USER as an unauthenticated user.
 
 
 @app.get("/", response_class=HTMLResponse)
 def read_root(
     request: Request,
     user: User = Depends(get_user),
-    message: str = None,
-    error_message: str = None,
+    message: Optional[str] = None,
+    error_message: Optional[str] = None,
 ):
     return templates.TemplateResponse(
+        request,
         "demo.html",
-        {"request": request, "user": user, "message": message, "error_message": error_message},
+        {
+            "request": request,
+            "user": user,
+            "message": message,
+            "error_message": error_message,
+        },
     )
 
 
 # This is an endpoint that requires the user to be authenticated.  In this case,
 # the user must have the ADMIN_ROLE role.  It is also possible to require a
 # permission instead.  Use the Protected dependency to require authentication.
 # An unauthenticated request as ANONYMOUS_USER will be rejected.
 @app.get("/admin")
 def admin(user: User = Depends(Protected(required_roles=[ADMIN_ROLE]))):
     return {"user": user}
 
 
 @app.get("/admin2")
-def admin(user: User = Depends(Protected(required_permission=VIEW_PERMISSION))):
+def admin2(user: User = Depends(Protected(required_permission=VIEW_PERMISSION))):
     return {"user": user}
```

### Comparing `zopyx_fastapi_auth-0.1.1.1/fastapi_auth/dependencies.py` & `zopyx_fastapi_auth-0.2.0/fastapi_auth/dependencies.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,22 +8,30 @@
 from .users import User, ANONYMOUS_USER
 from .roles import Role
 from .permissions import Permission
 from .logger import LOG
 
 
 def get_user(request: Request) -> User:
-    """A dependency to get the dependencies."""
+    """This dependency return either an authenticated user depending on the
+    presented token or an anonymous user if no token is presented."""
+
     if "user" not in request.session:
         return ANONYMOUS_USER
     return User(**request.session["user"])
 
 
 class Protected:
-    """A dependency to protect routes."""
+    """A dependency to protect routes.  The user must have the required
+    permission or role to access the route.  Using a permission and role(s) are
+    mutually exclusive. You must specify either a permission or a list of roles.
+    This dependency should be used for authenticated routes only. only.  The
+    authenticated user must either have a specified role or one of its role must
+    support the required permission.
+    """
 
     @typechecked
     def __init__(
         self,
         required_permission: Optional[Permission] = None,
         required_roles: Optional[list[Role]] = None,
     ):
```

### Comparing `zopyx_fastapi_auth-0.1.1.1/fastapi_auth/roles.py` & `zopyx_fastapi_auth-0.2.0/fastapi_auth/roles.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,30 +19,30 @@
     """Registry for roles."""
 
     def __init__(self):
         """Initialize the registry."""
         self.roles = dict()
 
     @typechecked
-    def register(self, role: "Role") -> None:
+    def register(self, role: Role) -> None:
         """Register a role."""
         self.roles[role.name] = role
 
     @typechecked
     def all_roles(self) -> list[Role]:
         """Return all roles."""
         return [r for r in self.roles.values()]
 
     @typechecked
     def all_role_names(self) -> list[str]:
         """Return all role names."""
         return list(self.roles.keys())
 
     @typechecked
-    def get_role(self, role_name: str) -> "Role":
+    def get_role(self, role_name: str) -> Role:
         """Get a role by name."""
         try:
             return self.roles[role_name]
         except KeyError:
             raise ValueError(f"Role {role_name} not found in role registry")
 
     @typechecked
@@ -54,13 +54,13 @@
     def __getattr__(self, role_name: str):
         """Get a role by name."""
         if role_name in self.roles:
             return self.roles[role_name]
         raise ValueError(f"Role {role_name} not found in role registry")
 
     @typechecked
-    def as_dict(self) -> dict[str, "Role"]:
+    def as_dict(self) -> dict[str, Role]:
         """Return the roles as a dictionary."""
         return self.roles
 
 
 ROLES_REGISTRY = RolesRegistry()
```

### Comparing `zopyx_fastapi_auth-0.1.1.1/fastapi_auth/user_cmd.py` & `zopyx_fastapi_auth-0.2.0/fastapi_auth/user_cmd.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,34 @@
 """Command line interface for user management."""
 
 import typer
 
 from .logger import LOG
 from .auth_config import AUTH_SETTINGS
+from rich.table import Table
+from rich.console import Console
 
-# from kataster.user import ROLES_REGISTRY
-from .user_management import UserManagement
+
+# from .user_management import UserManagement
+from .user_management_sqlobject import UserManagement
 
 
 app = typer.Typer()
 
 
 def get_user_management() -> UserManagement:
     """Get a UserManagement instance."""
-    LOG.debug(f"Using database file {AUTH_SETTINGS.db_name}")
-    return UserManagement(AUTH_SETTINGS.db_name)
+    LOG.debug(f"Using database {AUTH_SETTINGS.db_uri}")
+    return UserManagement(AUTH_SETTINGS.db_uri)
 
 
 @app.command()
 def add(username: str, password: str, roles: str) -> None:
     """Add a user to the database."""
     um = get_user_management()
-    um.create_db()
-
-    roles_lst = roles.split(",")
-    #    allowed_roles = ROLES_REGISTRY.all_role_names()
-    #    if not all(role in allowed_roles for role in roles_lst):
-    #        msg = f"Invalid roles: {roles}"
-    #        raise ValueError(msg)
-
     um.add_user(username, password, roles)
     LOG.debug(f"Added user {username} with roles {roles}")
 
 
 @app.command()
 def delete(user: str) -> None:
     """Delete a user from the database."""
@@ -61,16 +56,23 @@
 
 
 @app.command()
 def list_users() -> None:
     """List all users in the database."""
     um = get_user_management()
     users = um.get_users()
+
+    console = Console()
+    table = Table(show_header=True, header_style="bold magenta")
+    table.add_column("Name")
+    table.add_column("Role")
+    table.add_column("Created")
     for user in users:
-        typer.echo(user)
+        table.add_row(user.username, user.roles, user.created.isoformat())
+    console.print(table)
 
 
 @app.command()
 def delete_db() -> None:
     """Delete the database."""
     um = get_user_management()
     um.delete_db()
```

### Comparing `zopyx_fastapi_auth-0.1.1.1/fastapi_auth/users.py` & `zopyx_fastapi_auth-0.2.0/fastapi_auth/users.py`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.1.1.1/pyproject.toml` & `zopyx_fastapi_auth-0.2.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,46 @@
 [project]
 name = "zopyx-fastapi-auth"
 description = "FastAPI authentication and authorization"
-version = "0.1.1.1"
+version = "0.2.0"
 readme = "README.md"
 authors = [
     { name = "Andreas Jung", email = "info@zopyx.com" }
 ]
+classifiers = [
+  "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3.12",
+]
 dependencies = [
     "fastapi",
     "pydantic",
     "pydantic-settings",
     "uvicorn",
     "markdown",
     "starlette-session",
     "loguru",
     "bcrypt",
     "jinja2",
+    "sqlmodel", 
+    "rich",
     "python-multipart",
     "typer",
     "typeguard",
 ]
 
+
+[project.optional-dependencies]
+dev = [
+    "tox",
+    "pytest",
+    "ruff",
+    "twine", 
+    "build",
+]
+
 [tool.setuptools]
 packages = ["fastapi_auth"]
 
 [project.scripts]
 fastapi-auth-user-admin= "fastapi_auth.user_cmd:main"
 
 [tool.ruff.lint]
```

### Comparing `zopyx_fastapi_auth-0.1.1.1/static/bootstrap-5.3.3-dist/css/bootstrap-grid.css` & `zopyx_fastapi_auth-0.2.0/static/bootstrap-5.3.3-dist/css/bootstrap-grid.css`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.1.1.1/static/bootstrap-5.3.3-dist/css/bootstrap-grid.css.map` & `zopyx_fastapi_auth-0.2.0/static/bootstrap-5.3.3-dist/css/bootstrap-grid.css.map`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.1.1.1/static/bootstrap-5.3.3-dist/css/bootstrap-grid.min.css` & `zopyx_fastapi_auth-0.2.0/static/bootstrap-5.3.3-dist/css/bootstrap-grid.min.css`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.1.1.1/static/bootstrap-5.3.3-dist/css/bootstrap-grid.min.css.map` & `zopyx_fastapi_auth-0.2.0/static/bootstrap-5.3.3-dist/css/bootstrap-grid.min.css.map`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.1.1.1/static/bootstrap-5.3.3-dist/css/bootstrap-grid.rtl.css` & `zopyx_fastapi_auth-0.2.0/static/bootstrap-5.3.3-dist/css/bootstrap-grid.rtl.css`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.1.1.1/static/bootstrap-5.3.3-dist/css/bootstrap-grid.rtl.css.map` & `zopyx_fastapi_auth-0.2.0/static/bootstrap-5.3.3-dist/css/bootstrap-grid.rtl.css.map`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.1.1.1/static/bootstrap-5.3.3-dist/css/bootstrap-grid.rtl.min.css` & `zopyx_fastapi_auth-0.2.0/static/bootstrap-5.3.3-dist/css/bootstrap-grid.rtl.min.css`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.1.1.1/static/bootstrap-5.3.3-dist/css/bootstrap-grid.rtl.min.css.map` & `zopyx_fastapi_auth-0.2.0/static/bootstrap-5.3.3-dist/css/bootstrap-grid.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.1.1.1/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.css` & `zopyx_fastapi_auth-0.2.0/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.css`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.1.1.1/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.css.map` & `zopyx_fastapi_auth-0.2.0/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.css.map`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.1.1.1/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.min.css` & `zopyx_fastapi_auth-0.2.0/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.min.css`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.1.1.1/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.min.css.map` & `zopyx_fastapi_auth-0.2.0/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.min.css.map`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.1.1.1/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.rtl.css` & `zopyx_fastapi_auth-0.2.0/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.rtl.css`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.1.1.1/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.rtl.css.map` & `zopyx_fastapi_auth-0.2.0/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.rtl.css.map`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.1.1.1/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.rtl.min.css` & `zopyx_fastapi_auth-0.2.0/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.rtl.min.css`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.1.1.1/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.rtl.min.css.map` & `zopyx_fastapi_auth-0.2.0/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.1.1.1/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.css` & `zopyx_fastapi_auth-0.2.0/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.css`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.1.1.1/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.css.map` & `zopyx_fastapi_auth-0.2.0/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.css.map`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.1.1.1/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.min.css` & `zopyx_fastapi_auth-0.2.0/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.min.css`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.1.1.1/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.min.css.map` & `zopyx_fastapi_auth-0.2.0/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.min.css.map`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.1.1.1/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.rtl.css` & `zopyx_fastapi_auth-0.2.0/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.rtl.css`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.1.1.1/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.rtl.css.map` & `zopyx_fastapi_auth-0.2.0/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.rtl.css.map`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.1.1.1/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.rtl.min.css` & `zopyx_fastapi_auth-0.2.0/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.rtl.min.css`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.1.1.1/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.rtl.min.css.map` & `zopyx_fastapi_auth-0.2.0/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.1.1.1/static/bootstrap-5.3.3-dist/css/bootstrap.css` & `zopyx_fastapi_auth-0.2.0/static/bootstrap-5.3.3-dist/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.1.1.1/static/bootstrap-5.3.3-dist/css/bootstrap.css.map` & `zopyx_fastapi_auth-0.2.0/static/bootstrap-5.3.3-dist/css/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.1.1.1/static/bootstrap-5.3.3-dist/css/bootstrap.min.css` & `zopyx_fastapi_auth-0.2.0/static/bootstrap-5.3.3-dist/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.1.1.1/static/bootstrap-5.3.3-dist/css/bootstrap.min.css.map` & `zopyx_fastapi_auth-0.2.0/static/bootstrap-5.3.3-dist/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.1.1.1/static/bootstrap-5.3.3-dist/css/bootstrap.rtl.css` & `zopyx_fastapi_auth-0.2.0/static/bootstrap-5.3.3-dist/css/bootstrap.rtl.css`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.1.1.1/static/bootstrap-5.3.3-dist/css/bootstrap.rtl.css.map` & `zopyx_fastapi_auth-0.2.0/static/bootstrap-5.3.3-dist/css/bootstrap.rtl.css.map`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.1.1.1/static/bootstrap-5.3.3-dist/css/bootstrap.rtl.min.css` & `zopyx_fastapi_auth-0.2.0/static/bootstrap-5.3.3-dist/css/bootstrap.rtl.min.css`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.1.1.1/static/bootstrap-5.3.3-dist/css/bootstrap.rtl.min.css.map` & `zopyx_fastapi_auth-0.2.0/static/bootstrap-5.3.3-dist/css/bootstrap.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.1.1.1/static/bootstrap-5.3.3-dist/js/bootstrap.bundle.js` & `zopyx_fastapi_auth-0.2.0/static/bootstrap-5.3.3-dist/js/bootstrap.bundle.js`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.1.1.1/static/bootstrap-5.3.3-dist/js/bootstrap.bundle.js.map` & `zopyx_fastapi_auth-0.2.0/static/bootstrap-5.3.3-dist/js/bootstrap.bundle.js.map`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.1.1.1/static/bootstrap-5.3.3-dist/js/bootstrap.bundle.min.js` & `zopyx_fastapi_auth-0.2.0/static/bootstrap-5.3.3-dist/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.1.1.1/static/bootstrap-5.3.3-dist/js/bootstrap.bundle.min.js.map` & `zopyx_fastapi_auth-0.2.0/static/bootstrap-5.3.3-dist/js/bootstrap.bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.1.1.1/static/bootstrap-5.3.3-dist/js/bootstrap.esm.js` & `zopyx_fastapi_auth-0.2.0/static/bootstrap-5.3.3-dist/js/bootstrap.esm.js`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.1.1.1/static/bootstrap-5.3.3-dist/js/bootstrap.esm.js.map` & `zopyx_fastapi_auth-0.2.0/static/bootstrap-5.3.3-dist/js/bootstrap.esm.js.map`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.1.1.1/static/bootstrap-5.3.3-dist/js/bootstrap.esm.min.js` & `zopyx_fastapi_auth-0.2.0/static/bootstrap-5.3.3-dist/js/bootstrap.esm.min.js`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.1.1.1/static/bootstrap-5.3.3-dist/js/bootstrap.esm.min.js.map` & `zopyx_fastapi_auth-0.2.0/static/bootstrap-5.3.3-dist/js/bootstrap.esm.min.js.map`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.1.1.1/static/bootstrap-5.3.3-dist/js/bootstrap.js` & `zopyx_fastapi_auth-0.2.0/static/bootstrap-5.3.3-dist/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.1.1.1/static/bootstrap-5.3.3-dist/js/bootstrap.js.map` & `zopyx_fastapi_auth-0.2.0/static/bootstrap-5.3.3-dist/js/bootstrap.js.map`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.1.1.1/static/bootstrap-5.3.3-dist/js/bootstrap.min.js` & `zopyx_fastapi_auth-0.2.0/static/bootstrap-5.3.3-dist/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.1.1.1/static/bootstrap-5.3.3-dist/js/bootstrap.min.js.map` & `zopyx_fastapi_auth-0.2.0/static/bootstrap-5.3.3-dist/js/bootstrap.min.js.map`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.1.1.1/zopyx_fastapi_auth.egg-info/PKG-INFO` & `zopyx_fastapi_auth-0.2.0/zopyx_fastapi_auth.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,35 @@
 Metadata-Version: 2.1
 Name: zopyx-fastapi-auth
-Version: 0.1.1.1
+Version: 0.2.0
 Summary: FastAPI authentication and authorization
 Author-email: Andreas Jung <info@zopyx.com>
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 Requires-Dist: fastapi
 Requires-Dist: pydantic
 Requires-Dist: pydantic-settings
 Requires-Dist: uvicorn
 Requires-Dist: markdown
 Requires-Dist: starlette-session
 Requires-Dist: loguru
 Requires-Dist: bcrypt
 Requires-Dist: jinja2
+Requires-Dist: sqlmodel
+Requires-Dist: rich
 Requires-Dist: python-multipart
 Requires-Dist: typer
 Requires-Dist: typeguard
+Provides-Extra: dev
+Requires-Dist: tox; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: ruff; extra == "dev"
+Requires-Dist: twine; extra == "dev"
+Requires-Dist: build; extra == "dev"
 
 # fastapi-auth
 
 An opionated authentication and authorization system for FastAPI.
 
 ## Features
```

### Comparing `zopyx_fastapi_auth-0.1.1.1/zopyx_fastapi_auth.egg-info/SOURCES.txt` & `zopyx_fastapi_auth-0.2.0/zopyx_fastapi_auth.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 fastapi_auth/demo_app.py
 fastapi_auth/dependencies.py
 fastapi_auth/jinja2_templates.py
 fastapi_auth/logger.py
 fastapi_auth/permissions.py
 fastapi_auth/roles.py
 fastapi_auth/user_cmd.py
-fastapi_auth/user_management.py
+fastapi_auth/user_management_sqlobject.py
 fastapi_auth/users.py
 static/bootstrap-5.3.3-dist/css/bootstrap-grid.css
 static/bootstrap-5.3.3-dist/css/bootstrap-grid.css.map
 static/bootstrap-5.3.3-dist/css/bootstrap-grid.min.css
 static/bootstrap-5.3.3-dist/css/bootstrap-grid.min.css.map
 static/bootstrap-5.3.3-dist/css/bootstrap-grid.rtl.css
 static/bootstrap-5.3.3-dist/css/bootstrap-grid.rtl.css.map
```

