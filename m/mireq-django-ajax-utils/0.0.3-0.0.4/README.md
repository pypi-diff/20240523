# Comparing `tmp/mireq_django_ajax_utils-0.0.3.tar.gz` & `tmp/mireq_django_ajax_utils-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mireq_django_ajax_utils-0.0.3.tar", last modified: Mon Nov 27 10:48:10 2023, max compression
+gzip compressed data, was "mireq_django_ajax_utils-0.0.4.tar", last modified: Thu May 23 09:44:47 2024, max compression
```

## Comparing `mireq_django_ajax_utils-0.0.3.tar` & `mireq_django_ajax_utils-0.0.4.tar`

### file list

```diff
@@ -1,95 +1,95 @@
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-11-27 10:48:10.513951 mireq_django_ajax_utils-0.0.3/
--rw-r--r--   0 mirec     (1000) mirec     (1000)       97 2022-12-31 17:04:39.000000 mireq_django_ajax_utils-0.0.3/.editorconfig
--rw-r--r--   0 mirec     (1000) mirec     (1000)      124 2022-12-31 17:20:35.000000 mireq_django_ajax_utils-0.0.3/.gitignore
--rw-r--r--   0 mirec     (1000) mirec     (1000)       45 2016-09-02 12:40:01.000000 mireq_django_ajax_utils-0.0.3/AUTHORS
--rw-r--r--   0 mirec     (1000) mirec     (1000)      648 2023-11-27 10:47:14.000000 mireq_django_ajax_utils-0.0.3/CHANGELOG.md
--rw-r--r--   0 mirec     (1000) mirec     (1000)     1073 2022-12-31 17:20:35.000000 mireq_django_ajax_utils-0.0.3/LICENSE
--rw-r--r--   0 mirec     (1000) mirec     (1000)      253 2017-05-20 17:52:50.000000 mireq_django_ajax_utils-0.0.3/MANIFEST.in
--rw-r--r--   0 mirec     (1000) mirec     (1000)     2022 2023-11-27 10:48:10.513951 mireq_django_ajax_utils-0.0.3/PKG-INFO
--rw-r--r--   0 mirec     (1000) mirec     (1000)      676 2022-12-31 17:20:35.000000 mireq_django_ajax_utils-0.0.3/README.rst
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-11-27 10:48:10.508951 mireq_django_ajax_utils-0.0.3/django_ajax_utils/
--rw-r--r--   0 mirec     (1000) mirec     (1000)      105 2021-06-01 10:29:41.000000 mireq_django_ajax_utils-0.0.3/django_ajax_utils/__init__.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)      205 2020-01-23 06:31:07.000000 mireq_django_ajax_utils-0.0.3/django_ajax_utils/apps.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)     4734 2021-02-05 14:51:47.000000 mireq_django_ajax_utils-0.0.3/django_ajax_utils/forms.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)      911 2021-02-17 11:53:01.000000 mireq_django_ajax_utils-0.0.3/django_ajax_utils/middleware.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)      933 2020-01-27 06:18:07.000000 mireq_django_ajax_utils-0.0.3/django_ajax_utils/models.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)     4278 2018-06-15 13:04:41.000000 mireq_django_ajax_utils-0.0.3/django_ajax_utils/multiforms.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)     8884 2022-02-04 08:18:18.000000 mireq_django_ajax_utils-0.0.3/django_ajax_utils/pjax.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)     2152 2020-01-23 06:31:59.000000 mireq_django_ajax_utils-0.0.3/django_ajax_utils/reactor_compiler.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)      337 2022-03-14 11:13:32.000000 mireq_django_ajax_utils-0.0.3/django_ajax_utils/response.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)      672 2022-02-04 08:18:18.000000 mireq_django_ajax_utils-0.0.3/django_ajax_utils/settings.py
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-11-27 10:48:10.505951 mireq_django_ajax_utils-0.0.3/django_ajax_utils/static/
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-11-27 10:48:10.505951 mireq_django_ajax_utils-0.0.3/django_ajax_utils/static/django_ajax_utils/
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-11-27 10:48:10.509951 mireq_django_ajax_utils-0.0.3/django_ajax_utils/static/django_ajax_utils/js/
--rw-r--r--   0 mirec     (1000) mirec     (1000)    17197 2023-07-19 17:21:55.000000 mireq_django_ajax_utils-0.0.3/django_ajax_utils/static/django_ajax_utils/js/ajaxform.js
--rw-r--r--   0 mirec     (1000) mirec     (1000)      991 2023-07-19 17:21:55.000000 mireq_django_ajax_utils-0.0.3/django_ajax_utils/static/django_ajax_utils/js/el.js
--rw-r--r--   0 mirec     (1000) mirec     (1000)     2990 2023-07-19 17:21:55.000000 mireq_django_ajax_utils-0.0.3/django_ajax_utils/static/django_ajax_utils/js/messages.js
--rw-r--r--   0 mirec     (1000) mirec     (1000)    10610 2023-11-27 10:47:09.000000 mireq_django_ajax_utils-0.0.3/django_ajax_utils/static/django_ajax_utils/js/pjax.js
--rw-r--r--   0 mirec     (1000) mirec     (1000)     1455 2023-07-19 17:21:55.000000 mireq_django_ajax_utils-0.0.3/django_ajax_utils/static/django_ajax_utils/js/polyfill.js
--rw-r--r--   0 mirec     (1000) mirec     (1000)     1711 2023-07-19 17:21:55.000000 mireq_django_ajax_utils-0.0.3/django_ajax_utils/static/django_ajax_utils/js/urls.js
--rw-r--r--   0 mirec     (1000) mirec     (1000)    23854 2023-07-19 17:21:55.000000 mireq_django_ajax_utils-0.0.3/django_ajax_utils/static/django_ajax_utils/js/utils.js
--rw-r--r--   0 mirec     (1000) mirec     (1000)     3672 2023-07-19 17:22:30.000000 mireq_django_ajax_utils-0.0.3/django_ajax_utils/static/django_ajax_utils/js/utils_ajax.js
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-11-27 10:48:10.505951 mireq_django_ajax_utils-0.0.3/django_ajax_utils/templates/
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-11-27 10:48:10.505951 mireq_django_ajax_utils-0.0.3/django_ajax_utils/templates/form_utils/
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-11-27 10:48:10.509951 mireq_django_ajax_utils-0.0.3/django_ajax_utils/templates/form_utils/layout/
--rw-r--r--   0 mirec     (1000) mirec     (1000)      460 2018-06-10 07:00:55.000000 mireq_django_ajax_utils-0.0.3/django_ajax_utils/templates/form_utils/layout/default.html
--rw-r--r--   0 mirec     (1000) mirec     (1000)      494 2018-06-10 07:00:55.000000 mireq_django_ajax_utils-0.0.3/django_ajax_utils/templates/form_utils/layout/foundation.html
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-11-27 10:48:10.510951 mireq_django_ajax_utils-0.0.3/django_ajax_utils/templates/form_utils/row/
--rw-r--r--   0 mirec     (1000) mirec     (1000)      717 2018-06-10 07:00:55.000000 mireq_django_ajax_utils-0.0.3/django_ajax_utils/templates/form_utils/row/default.html
--rw-r--r--   0 mirec     (1000) mirec     (1000)      987 2018-06-10 07:00:55.000000 mireq_django_ajax_utils-0.0.3/django_ajax_utils/templates/form_utils/row/foundation.html
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-11-27 10:48:10.510951 mireq_django_ajax_utils-0.0.3/django_ajax_utils/templatetags/
--rw-r--r--   0 mirec     (1000) mirec     (1000)        0 2018-06-10 07:00:55.000000 mireq_django_ajax_utils-0.0.3/django_ajax_utils/templatetags/__init__.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)     6343 2021-04-17 11:49:52.000000 mireq_django_ajax_utils-0.0.3/django_ajax_utils/templatetags/form_utils.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)     2281 2020-02-08 09:15:46.000000 mireq_django_ajax_utils-0.0.3/django_ajax_utils/templatetags/js_urlpatterns.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)     1118 2020-01-23 06:33:27.000000 mireq_django_ajax_utils-0.0.3/django_ajax_utils/templatetags/pjax_tags.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)     4976 2021-08-13 04:34:28.000000 mireq_django_ajax_utils-0.0.3/django_ajax_utils/utility.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)     4674 2022-09-03 16:43:27.000000 mireq_django_ajax_utils-0.0.3/django_ajax_utils/views.py
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-11-27 10:48:10.510951 mireq_django_ajax_utils-0.0.3/mireq_django_ajax_utils.egg-info/
--rw-r--r--   0 mirec     (1000) mirec     (1000)     2022 2023-11-27 10:48:10.000000 mireq_django_ajax_utils-0.0.3/mireq_django_ajax_utils.egg-info/PKG-INFO
--rw-r--r--   0 mirec     (1000) mirec     (1000)     2773 2023-11-27 10:48:10.000000 mireq_django_ajax_utils-0.0.3/mireq_django_ajax_utils.egg-info/SOURCES.txt
--rw-r--r--   0 mirec     (1000) mirec     (1000)        1 2023-11-27 10:48:10.000000 mireq_django_ajax_utils-0.0.3/mireq_django_ajax_utils.egg-info/dependency_links.txt
--rw-r--r--   0 mirec     (1000) mirec     (1000)      111 2023-11-27 10:48:10.000000 mireq_django_ajax_utils-0.0.3/mireq_django_ajax_utils.egg-info/requires.txt
--rw-r--r--   0 mirec     (1000) mirec     (1000)       18 2023-11-27 10:48:10.000000 mireq_django_ajax_utils-0.0.3/mireq_django_ajax_utils.egg-info/top_level.txt
--rw-r--r--   0 mirec     (1000) mirec     (1000)     1433 2023-11-27 10:47:14.000000 mireq_django_ajax_utils-0.0.3/pyproject.toml
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-11-27 10:48:10.510951 mireq_django_ajax_utils-0.0.3/sample_project/
--rwxr-xr-x   0 mirec     (1000) mirec     (1000)      749 2016-09-02 13:28:53.000000 mireq_django_ajax_utils-0.0.3/sample_project/manage.py
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-11-27 10:48:10.506951 mireq_django_ajax_utils-0.0.3/sample_project/static/
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-11-27 10:48:10.511951 mireq_django_ajax_utils-0.0.3/sample_project/static/css/
--rw-r--r--   0 mirec     (1000) mirec     (1000)     4642 2017-07-08 16:58:23.000000 mireq_django_ajax_utils-0.0.3/sample_project/static/css/style.css
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-11-27 10:48:10.511951 mireq_django_ajax_utils-0.0.3/sample_project/static/js/
--rw-r--r--   0 mirec     (1000) mirec     (1000)      312 2017-05-21 13:45:25.000000 mireq_django_ajax_utils-0.0.3/sample_project/static/js/ajaxform_init.js
--rw-r--r--   0 mirec     (1000) mirec     (1000)      724 2016-11-13 15:36:39.000000 mireq_django_ajax_utils-0.0.3/sample_project/static/js/pjax_init.js
--rw-r--r--   0 mirec     (1000) mirec     (1000)     1709 2017-04-24 08:22:51.000000 mireq_django_ajax_utils-0.0.3/sample_project/static/js/run_utils.js
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-11-27 10:48:10.512951 mireq_django_ajax_utils-0.0.3/sample_project/templates/
--rw-r--r--   0 mirec     (1000) mirec     (1000)      574 2016-11-19 18:58:10.000000 mireq_django_ajax_utils-0.0.3/sample_project/templates/ajaxform.html
--rw-r--r--   0 mirec     (1000) mirec     (1000)     1107 2017-05-21 07:45:23.000000 mireq_django_ajax_utils-0.0.3/sample_project/templates/base.html
--rw-r--r--   0 mirec     (1000) mirec     (1000)      544 2016-11-12 18:41:30.000000 mireq_django_ajax_utils-0.0.3/sample_project/templates/base_pjax.html
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-11-27 10:48:10.512951 mireq_django_ajax_utils-0.0.3/sample_project/templates/form_utils/
--rw-r--r--   0 mirec     (1000) mirec     (1000)      643 2017-07-08 17:05:10.000000 mireq_django_ajax_utils-0.0.3/sample_project/templates/form_utils/base.html
--rw-r--r--   0 mirec     (1000) mirec     (1000)      183 2017-07-08 13:02:14.000000 mireq_django_ajax_utils-0.0.3/sample_project/templates/form_utils/formset.html
--rw-r--r--   0 mirec     (1000) mirec     (1000)      824 2017-05-21 14:41:06.000000 mireq_django_ajax_utils-0.0.3/sample_project/templates/form_utils/foundation.html
--rw-r--r--   0 mirec     (1000) mirec     (1000)      855 2017-07-08 16:55:30.000000 mireq_django_ajax_utils-0.0.3/sample_project/templates/form_utils/multiforms.html
--rw-r--r--   0 mirec     (1000) mirec     (1000)      185 2016-11-06 16:24:25.000000 mireq_django_ajax_utils-0.0.3/sample_project/templates/home.html
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-11-27 10:48:10.512951 mireq_django_ajax_utils-0.0.3/sample_project/templates/includes/
--rw-r--r--   0 mirec     (1000) mirec     (1000)      974 2016-09-05 17:12:59.000000 mireq_django_ajax_utils-0.0.3/sample_project/templates/includes/form_loop.html
--rw-r--r--   0 mirec     (1000) mirec     (1000)      883 2016-11-12 19:45:37.000000 mireq_django_ajax_utils-0.0.3/sample_project/templates/messages.html
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-11-27 10:48:10.512951 mireq_django_ajax_utils-0.0.3/sample_project/templates/partials/
--rw-r--r--   0 mirec     (1000) mirec     (1000)      574 2017-07-08 16:31:47.000000 mireq_django_ajax_utils-0.0.3/sample_project/templates/partials/menu.html
--rw-r--r--   0 mirec     (1000) mirec     (1000)      357 2016-10-16 11:29:40.000000 mireq_django_ajax_utils-0.0.3/sample_project/templates/partials/messages.html
--rw-r--r--   0 mirec     (1000) mirec     (1000)      115 2016-11-12 18:40:45.000000 mireq_django_ajax_utils-0.0.3/sample_project/templates/partials/messages_pjax.html
--rw-r--r--   0 mirec     (1000) mirec     (1000)     1033 2016-11-13 17:44:54.000000 mireq_django_ajax_utils-0.0.3/sample_project/templates/pjax.html
--rw-r--r--   0 mirec     (1000) mirec     (1000)      816 2017-04-08 06:54:58.000000 mireq_django_ajax_utils-0.0.3/sample_project/templates/pjax_form_get.html
--rw-r--r--   0 mirec     (1000) mirec     (1000)      510 2017-04-08 06:55:10.000000 mireq_django_ajax_utils-0.0.3/sample_project/templates/pjax_form_post.html
--rw-r--r--   0 mirec     (1000) mirec     (1000)      891 2016-11-13 17:45:23.000000 mireq_django_ajax_utils-0.0.3/sample_project/templates/pjax_messages.html
--rw-r--r--   0 mirec     (1000) mirec     (1000)      637 2017-04-08 06:46:39.000000 mireq_django_ajax_utils-0.0.3/sample_project/templates/pjax_page.html
--rw-r--r--   0 mirec     (1000) mirec     (1000)     1552 2017-04-08 17:50:19.000000 mireq_django_ajax_utils-0.0.3/sample_project/templates/urlpatterns.html
--rw-r--r--   0 mirec     (1000) mirec     (1000)     7633 2017-05-20 14:49:49.000000 mireq_django_ajax_utils-0.0.3/sample_project/templates/utils.html
-drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2023-11-27 10:48:10.513951 mireq_django_ajax_utils-0.0.3/sample_project/web/
--rw-r--r--   0 mirec     (1000) mirec     (1000)        0 2016-09-02 12:55:53.000000 mireq_django_ajax_utils-0.0.3/sample_project/web/__init__.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)     1761 2017-07-08 13:01:08.000000 mireq_django_ajax_utils-0.0.3/sample_project/web/forms.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)     1847 2018-09-22 16:34:33.000000 mireq_django_ajax_utils-0.0.3/sample_project/web/settings.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)     1027 2017-07-08 16:31:28.000000 mireq_django_ajax_utils-0.0.3/sample_project/web/urls.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)     3483 2017-07-08 17:06:05.000000 mireq_django_ajax_utils-0.0.3/sample_project/web/views.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)      384 2016-09-02 12:55:53.000000 mireq_django_ajax_utils-0.0.3/sample_project/web/wsgi.py
--rw-r--r--   0 mirec     (1000) mirec     (1000)       38 2023-11-27 10:48:10.514951 mireq_django_ajax_utils-0.0.3/setup.cfg
--rw-r--r--   0 mirec     (1000) mirec     (1000)       38 2022-12-31 17:20:35.000000 mireq_django_ajax_utils-0.0.3/setup.py
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2024-05-23 09:44:47.802015 mireq_django_ajax_utils-0.0.4/
+-rw-r--r--   0 mirec     (1000) mirec     (1000)       97 2022-12-31 17:04:39.000000 mireq_django_ajax_utils-0.0.4/.editorconfig
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      124 2022-12-31 17:20:35.000000 mireq_django_ajax_utils-0.0.4/.gitignore
+-rw-r--r--   0 mirec     (1000) mirec     (1000)       45 2016-09-02 12:40:01.000000 mireq_django_ajax_utils-0.0.4/AUTHORS
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      720 2024-05-23 09:44:08.000000 mireq_django_ajax_utils-0.0.4/CHANGELOG.md
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     1073 2022-12-31 17:20:35.000000 mireq_django_ajax_utils-0.0.4/LICENSE
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      253 2017-05-20 17:52:50.000000 mireq_django_ajax_utils-0.0.4/MANIFEST.in
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     2022 2024-05-23 09:44:47.802015 mireq_django_ajax_utils-0.0.4/PKG-INFO
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      676 2022-12-31 17:20:35.000000 mireq_django_ajax_utils-0.0.4/README.rst
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2024-05-23 09:44:47.788015 mireq_django_ajax_utils-0.0.4/django_ajax_utils/
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      105 2021-06-01 10:29:41.000000 mireq_django_ajax_utils-0.0.4/django_ajax_utils/__init__.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      205 2020-01-23 06:31:07.000000 mireq_django_ajax_utils-0.0.4/django_ajax_utils/apps.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     4734 2021-02-05 14:51:47.000000 mireq_django_ajax_utils-0.0.4/django_ajax_utils/forms.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      911 2021-02-17 11:53:01.000000 mireq_django_ajax_utils-0.0.4/django_ajax_utils/middleware.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      933 2020-01-27 06:18:07.000000 mireq_django_ajax_utils-0.0.4/django_ajax_utils/models.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     4278 2018-06-15 13:04:41.000000 mireq_django_ajax_utils-0.0.4/django_ajax_utils/multiforms.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     8884 2022-02-04 08:18:18.000000 mireq_django_ajax_utils-0.0.4/django_ajax_utils/pjax.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     2152 2020-01-23 06:31:59.000000 mireq_django_ajax_utils-0.0.4/django_ajax_utils/reactor_compiler.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      337 2022-03-14 11:13:32.000000 mireq_django_ajax_utils-0.0.4/django_ajax_utils/response.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      672 2022-02-04 08:18:18.000000 mireq_django_ajax_utils-0.0.4/django_ajax_utils/settings.py
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2024-05-23 09:44:47.782015 mireq_django_ajax_utils-0.0.4/django_ajax_utils/static/
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2024-05-23 09:44:47.782015 mireq_django_ajax_utils-0.0.4/django_ajax_utils/static/django_ajax_utils/
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2024-05-23 09:44:47.791015 mireq_django_ajax_utils-0.0.4/django_ajax_utils/static/django_ajax_utils/js/
+-rw-r--r--   0 mirec     (1000) mirec     (1000)    17647 2024-05-23 09:37:46.000000 mireq_django_ajax_utils-0.0.4/django_ajax_utils/static/django_ajax_utils/js/ajaxform.js
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      991 2023-07-19 17:21:55.000000 mireq_django_ajax_utils-0.0.4/django_ajax_utils/static/django_ajax_utils/js/el.js
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     2990 2023-07-19 17:21:55.000000 mireq_django_ajax_utils-0.0.4/django_ajax_utils/static/django_ajax_utils/js/messages.js
+-rw-r--r--   0 mirec     (1000) mirec     (1000)    10610 2023-11-27 10:47:09.000000 mireq_django_ajax_utils-0.0.4/django_ajax_utils/static/django_ajax_utils/js/pjax.js
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     1455 2023-07-19 17:21:55.000000 mireq_django_ajax_utils-0.0.4/django_ajax_utils/static/django_ajax_utils/js/polyfill.js
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     1711 2023-07-19 17:21:55.000000 mireq_django_ajax_utils-0.0.4/django_ajax_utils/static/django_ajax_utils/js/urls.js
+-rw-r--r--   0 mirec     (1000) mirec     (1000)    23854 2023-07-19 17:21:55.000000 mireq_django_ajax_utils-0.0.4/django_ajax_utils/static/django_ajax_utils/js/utils.js
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     3672 2023-07-19 17:22:30.000000 mireq_django_ajax_utils-0.0.4/django_ajax_utils/static/django_ajax_utils/js/utils_ajax.js
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2024-05-23 09:44:47.782015 mireq_django_ajax_utils-0.0.4/django_ajax_utils/templates/
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2024-05-23 09:44:47.783015 mireq_django_ajax_utils-0.0.4/django_ajax_utils/templates/form_utils/
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2024-05-23 09:44:47.792015 mireq_django_ajax_utils-0.0.4/django_ajax_utils/templates/form_utils/layout/
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      460 2018-06-10 07:00:55.000000 mireq_django_ajax_utils-0.0.4/django_ajax_utils/templates/form_utils/layout/default.html
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      494 2018-06-10 07:00:55.000000 mireq_django_ajax_utils-0.0.4/django_ajax_utils/templates/form_utils/layout/foundation.html
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2024-05-23 09:44:47.792015 mireq_django_ajax_utils-0.0.4/django_ajax_utils/templates/form_utils/row/
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      717 2018-06-10 07:00:55.000000 mireq_django_ajax_utils-0.0.4/django_ajax_utils/templates/form_utils/row/default.html
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      987 2018-06-10 07:00:55.000000 mireq_django_ajax_utils-0.0.4/django_ajax_utils/templates/form_utils/row/foundation.html
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2024-05-23 09:44:47.794015 mireq_django_ajax_utils-0.0.4/django_ajax_utils/templatetags/
+-rw-r--r--   0 mirec     (1000) mirec     (1000)        0 2018-06-10 07:00:55.000000 mireq_django_ajax_utils-0.0.4/django_ajax_utils/templatetags/__init__.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     6343 2021-04-17 11:49:52.000000 mireq_django_ajax_utils-0.0.4/django_ajax_utils/templatetags/form_utils.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     2281 2020-02-08 09:15:46.000000 mireq_django_ajax_utils-0.0.4/django_ajax_utils/templatetags/js_urlpatterns.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     1118 2020-01-23 06:33:27.000000 mireq_django_ajax_utils-0.0.4/django_ajax_utils/templatetags/pjax_tags.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     4976 2021-08-13 04:34:28.000000 mireq_django_ajax_utils-0.0.4/django_ajax_utils/utility.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     4674 2022-09-03 16:43:27.000000 mireq_django_ajax_utils-0.0.4/django_ajax_utils/views.py
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2024-05-23 09:44:47.801015 mireq_django_ajax_utils-0.0.4/mireq_django_ajax_utils.egg-info/
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     2022 2024-05-23 09:44:47.000000 mireq_django_ajax_utils-0.0.4/mireq_django_ajax_utils.egg-info/PKG-INFO
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     2773 2024-05-23 09:44:47.000000 mireq_django_ajax_utils-0.0.4/mireq_django_ajax_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 mirec     (1000) mirec     (1000)        1 2024-05-23 09:44:47.000000 mireq_django_ajax_utils-0.0.4/mireq_django_ajax_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      111 2024-05-23 09:44:47.000000 mireq_django_ajax_utils-0.0.4/mireq_django_ajax_utils.egg-info/requires.txt
+-rw-r--r--   0 mirec     (1000) mirec     (1000)       18 2024-05-23 09:44:47.000000 mireq_django_ajax_utils-0.0.4/mireq_django_ajax_utils.egg-info/top_level.txt
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     1433 2024-05-23 09:44:08.000000 mireq_django_ajax_utils-0.0.4/pyproject.toml
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2024-05-23 09:44:47.795015 mireq_django_ajax_utils-0.0.4/sample_project/
+-rwxr-xr-x   0 mirec     (1000) mirec     (1000)      749 2016-09-02 13:28:53.000000 mireq_django_ajax_utils-0.0.4/sample_project/manage.py
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2024-05-23 09:44:47.783015 mireq_django_ajax_utils-0.0.4/sample_project/static/
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2024-05-23 09:44:47.795015 mireq_django_ajax_utils-0.0.4/sample_project/static/css/
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     4642 2017-07-08 16:58:23.000000 mireq_django_ajax_utils-0.0.4/sample_project/static/css/style.css
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2024-05-23 09:44:47.796015 mireq_django_ajax_utils-0.0.4/sample_project/static/js/
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      312 2017-05-21 13:45:25.000000 mireq_django_ajax_utils-0.0.4/sample_project/static/js/ajaxform_init.js
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      724 2016-11-13 15:36:39.000000 mireq_django_ajax_utils-0.0.4/sample_project/static/js/pjax_init.js
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     1709 2017-04-24 08:22:51.000000 mireq_django_ajax_utils-0.0.4/sample_project/static/js/run_utils.js
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2024-05-23 09:44:47.798015 mireq_django_ajax_utils-0.0.4/sample_project/templates/
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      574 2016-11-19 18:58:10.000000 mireq_django_ajax_utils-0.0.4/sample_project/templates/ajaxform.html
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     1107 2017-05-21 07:45:23.000000 mireq_django_ajax_utils-0.0.4/sample_project/templates/base.html
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      544 2016-11-12 18:41:30.000000 mireq_django_ajax_utils-0.0.4/sample_project/templates/base_pjax.html
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2024-05-23 09:44:47.799015 mireq_django_ajax_utils-0.0.4/sample_project/templates/form_utils/
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      643 2017-07-08 17:05:10.000000 mireq_django_ajax_utils-0.0.4/sample_project/templates/form_utils/base.html
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      183 2017-07-08 13:02:14.000000 mireq_django_ajax_utils-0.0.4/sample_project/templates/form_utils/formset.html
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      824 2017-05-21 14:41:06.000000 mireq_django_ajax_utils-0.0.4/sample_project/templates/form_utils/foundation.html
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      855 2017-07-08 16:55:30.000000 mireq_django_ajax_utils-0.0.4/sample_project/templates/form_utils/multiforms.html
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      185 2016-11-06 16:24:25.000000 mireq_django_ajax_utils-0.0.4/sample_project/templates/home.html
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2024-05-23 09:44:47.799015 mireq_django_ajax_utils-0.0.4/sample_project/templates/includes/
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      974 2016-09-05 17:12:59.000000 mireq_django_ajax_utils-0.0.4/sample_project/templates/includes/form_loop.html
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      883 2016-11-12 19:45:37.000000 mireq_django_ajax_utils-0.0.4/sample_project/templates/messages.html
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2024-05-23 09:44:47.800015 mireq_django_ajax_utils-0.0.4/sample_project/templates/partials/
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      574 2017-07-08 16:31:47.000000 mireq_django_ajax_utils-0.0.4/sample_project/templates/partials/menu.html
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      357 2016-10-16 11:29:40.000000 mireq_django_ajax_utils-0.0.4/sample_project/templates/partials/messages.html
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      115 2016-11-12 18:40:45.000000 mireq_django_ajax_utils-0.0.4/sample_project/templates/partials/messages_pjax.html
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     1033 2016-11-13 17:44:54.000000 mireq_django_ajax_utils-0.0.4/sample_project/templates/pjax.html
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      816 2017-04-08 06:54:58.000000 mireq_django_ajax_utils-0.0.4/sample_project/templates/pjax_form_get.html
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      510 2017-04-08 06:55:10.000000 mireq_django_ajax_utils-0.0.4/sample_project/templates/pjax_form_post.html
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      891 2016-11-13 17:45:23.000000 mireq_django_ajax_utils-0.0.4/sample_project/templates/pjax_messages.html
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      637 2017-04-08 06:46:39.000000 mireq_django_ajax_utils-0.0.4/sample_project/templates/pjax_page.html
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     1552 2017-04-08 17:50:19.000000 mireq_django_ajax_utils-0.0.4/sample_project/templates/urlpatterns.html
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     7633 2017-05-20 14:49:49.000000 mireq_django_ajax_utils-0.0.4/sample_project/templates/utils.html
+drwxr-xr-x   0 mirec     (1000) mirec     (1000)        0 2024-05-23 09:44:47.801015 mireq_django_ajax_utils-0.0.4/sample_project/web/
+-rw-r--r--   0 mirec     (1000) mirec     (1000)        0 2016-09-02 12:55:53.000000 mireq_django_ajax_utils-0.0.4/sample_project/web/__init__.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     1761 2017-07-08 13:01:08.000000 mireq_django_ajax_utils-0.0.4/sample_project/web/forms.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     1847 2018-09-22 16:34:33.000000 mireq_django_ajax_utils-0.0.4/sample_project/web/settings.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     1027 2017-07-08 16:31:28.000000 mireq_django_ajax_utils-0.0.4/sample_project/web/urls.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)     3483 2017-07-08 17:06:05.000000 mireq_django_ajax_utils-0.0.4/sample_project/web/views.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)      384 2016-09-02 12:55:53.000000 mireq_django_ajax_utils-0.0.4/sample_project/web/wsgi.py
+-rw-r--r--   0 mirec     (1000) mirec     (1000)       38 2024-05-23 09:44:47.803015 mireq_django_ajax_utils-0.0.4/setup.cfg
+-rw-r--r--   0 mirec     (1000) mirec     (1000)       38 2022-12-31 17:20:35.000000 mireq_django_ajax_utils-0.0.4/setup.py
```

### Comparing `mireq_django_ajax_utils-0.0.3/CHANGELOG.md` & `mireq_django_ajax_utils-0.0.4/CHANGELOG.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+## 0.0.4 (2024-05-23)
+
+### Feat
+
+- Added configurable form row classes
+
 ## 0.0.3 (2023-11-27)
 
 ### Feat
 
 - Pass pjaxOptions to request interceptor
 - Pass event to pjax load if loaded automatically
```

### Comparing `mireq_django_ajax_utils-0.0.3/LICENSE` & `mireq_django_ajax_utils-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mireq_django_ajax_utils-0.0.3/PKG-INFO` & `mireq_django_ajax_utils-0.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mireq_django_ajax_utils
-Version: 0.0.3
+Version: 0.0.4
 Summary: Django ajax utils
 Author-email: Miroslav Bendík <miroslav.bendik@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/mireq/django-ajax-utils
 Project-URL: documentation, https://github.com/mireq/django-ajax-utils
 Project-URL: repository, https://github.com/mireq/django-ajax-utils
 Project-URL: changelog, https://github.com/mireq/django-ajax-utils/blob/master/CHANGELOG.md
```

### Comparing `mireq_django_ajax_utils-0.0.3/README.rst` & `mireq_django_ajax_utils-0.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `mireq_django_ajax_utils-0.0.3/django_ajax_utils/forms.py` & `mireq_django_ajax_utils-0.0.4/django_ajax_utils/forms.py`

 * *Files identical despite different names*

### Comparing `mireq_django_ajax_utils-0.0.3/django_ajax_utils/middleware.py` & `mireq_django_ajax_utils-0.0.4/django_ajax_utils/middleware.py`

 * *Files identical despite different names*

### Comparing `mireq_django_ajax_utils-0.0.3/django_ajax_utils/models.py` & `mireq_django_ajax_utils-0.0.4/django_ajax_utils/models.py`

 * *Files identical despite different names*

### Comparing `mireq_django_ajax_utils-0.0.3/django_ajax_utils/multiforms.py` & `mireq_django_ajax_utils-0.0.4/django_ajax_utils/multiforms.py`

 * *Files identical despite different names*

### Comparing `mireq_django_ajax_utils-0.0.3/django_ajax_utils/pjax.py` & `mireq_django_ajax_utils-0.0.4/django_ajax_utils/pjax.py`

 * *Files identical despite different names*

### Comparing `mireq_django_ajax_utils-0.0.3/django_ajax_utils/reactor_compiler.py` & `mireq_django_ajax_utils-0.0.4/django_ajax_utils/reactor_compiler.py`

 * *Files identical despite different names*

### Comparing `mireq_django_ajax_utils-0.0.3/django_ajax_utils/settings.py` & `mireq_django_ajax_utils-0.0.4/django_ajax_utils/settings.py`

 * *Files identical despite different names*

### Comparing `mireq_django_ajax_utils-0.0.3/django_ajax_utils/static/django_ajax_utils/js/ajaxform.js` & `mireq_django_ajax_utils-0.0.4/django_ajax_utils/static/django_ajax_utils/js/ajaxform.js`

 * *Files 6% similar despite different names*

#### js-beautify {}

```diff
@@ -376,15 +376,18 @@
     };
 
 
     var ajaxform = function(formElement, options) {
         var o = _.lightCopy(options);
         o.nonFieldErrorsClass = o.nonFieldErrorsClass || _.getData(formElement, 'nonFieldErrorsClass') || 'non-field-errors';
         o.fieldErrorsClass = o.fieldErrorsClass || _.getData(formElement, 'fieldErrorsClass') || 'field-errors';
+        o.fieldErrorClass = o.fieldErrorClass || _.getData(formElement, 'fieldErrorClass') || 'field-errors';
         o.rowClass = o.rowClass || _.getData(formElement, 'rowClass') || 'form-row';
+        o.rowHasErrorsClass = o.rowHasErrorsClass || _.getData(formElement, 'rowHasErrorsClass') || 'has-errors';
+        o.rowNoErrorsClass = o.rowNoErrorsClass || _.getData(formElement, 'rowNoErrorsClass') || 'no-errors';
         if (!_.has(o, 'liveValidate')) {
             o.liveValidate = (_.getData(formElement, 'liveValidate') !== 'false');
         }
 
         var self = ajaxformBase(formElement, o);
         self.disabler = submitDisabler(formElement);
         var showErrorsOnFly = {
@@ -448,55 +451,55 @@
             var errorContainer = self.getErrorContainer(fieldName);
             var errorsElement = _.tag(errorContainer, 'ul')[0];
             if (errorsElement === undefined) {
                 errorsElement = _.elem('ul');
                 errorContainer.appendChild(errorsElement);
             }
 
-            var errorsElementClassName = o.fieldErrorsClass + ' has-errors count-' + errorList.length;
-            errorsElement.className = errorsElementClassName;
+            errorsElement.className = '';
+            _.addClass(errorsElement, o.fieldErrorsClass);
+            _.addClass(errorsElement, o.fieldErrorsClass + '--count-' + errorList.length);
 
             _.forEach(errorList, function(error) {
                 var messageElement = _.elem('li', {}, error.message);
+                messageElement.classList.add(self.options.fieldErrorClass);
                 if (error.code) {
-                    messageElement.className = 'form-error code-' + error.code;
-                } else {
-                    messageElement.className = 'form-error';
+                    messageElement.classList.add(self.options.fieldErrorClass + '--code-' + error.code);
                 }
                 errorsElement.appendChild(messageElement);
             });
 
             var row = self.findFormRow(errorContainer);
             if (row !== null) {
-                _.removeClass(row, 'no-errors');
-                _.addClass(row, 'has-errors');
+                _.removeClass(row, self.options.rowNoErrorsClass);
+                _.addClass(row, self.options.rowHasErrorsClass);
             }
         };
 
         self.setValid = function(fieldName) {
             var errorContainer = self.getErrorContainer(fieldName, true);
             if (errorContainer === null) {
                 return;
             }
             var row = self.findFormRow(errorContainer);
             if (row !== null) {
-                _.addClass(row, 'no-errors');
+                _.addClass(row, self.options.rowNoErrorsClass);
             }
         };
 
         self.clearStatus = function(fieldName) {
             var errorContainer = self.getErrorContainer(fieldName, fieldName !== '__all__');
             if (errorContainer === null) {
                 return;
             }
             errorContainer.innerHTML = '';
             var row = self.findFormRow(errorContainer);
             if (row !== null) {
-                _.removeClass(row, 'has-errors');
-                _.removeClass(row, 'no-errors');
+                _.removeClass(row, self.options.rowHasErrorsClass);
+                _.removeClass(row, self.options.rowNoErrorsClass);
             }
         };
 
         self.onFormSubmit = function(e) {
             self.submit();
             self.disabler.disable();
             e.preventDefault();
@@ -548,14 +551,15 @@
                 self.setValid(key);
             });
         };
 
         return self;
     };
 
+
     var ajaxformFoundation = function(formElement, options) {
         var self = ajaxform(formElement, options);
 
         self.addErrors = function(fieldName, errorList) {
             var errorContainer = self.getErrorContainer(fieldName);
             if (fieldName === '__all__') {
                 var box = _.cls(errorContainer, 'alert')[0];
@@ -616,14 +620,15 @@
             }
         };
 
         return self;
     };
 
 
+
     window._utils.ajaxformBase = ajaxformBase;
     window._utils.ajaxform = ajaxform;
     window._utils.ajaxformFoundation = ajaxformFoundation;
 
 
     function dispatchEvent(eventType, e) {
         var form;
```

### Comparing `mireq_django_ajax_utils-0.0.3/django_ajax_utils/static/django_ajax_utils/js/el.js` & `mireq_django_ajax_utils-0.0.4/django_ajax_utils/static/django_ajax_utils/js/el.js`

 * *Files identical despite different names*

### Comparing `mireq_django_ajax_utils-0.0.3/django_ajax_utils/static/django_ajax_utils/js/messages.js` & `mireq_django_ajax_utils-0.0.4/django_ajax_utils/static/django_ajax_utils/js/messages.js`

 * *Files identical despite different names*

### Comparing `mireq_django_ajax_utils-0.0.3/django_ajax_utils/static/django_ajax_utils/js/pjax.js` & `mireq_django_ajax_utils-0.0.4/django_ajax_utils/static/django_ajax_utils/js/pjax.js`

 * *Files identical despite different names*

### Comparing `mireq_django_ajax_utils-0.0.3/django_ajax_utils/static/django_ajax_utils/js/polyfill.js` & `mireq_django_ajax_utils-0.0.4/django_ajax_utils/static/django_ajax_utils/js/polyfill.js`

 * *Files identical despite different names*

### Comparing `mireq_django_ajax_utils-0.0.3/django_ajax_utils/static/django_ajax_utils/js/urls.js` & `mireq_django_ajax_utils-0.0.4/django_ajax_utils/static/django_ajax_utils/js/urls.js`

 * *Files identical despite different names*

### Comparing `mireq_django_ajax_utils-0.0.3/django_ajax_utils/static/django_ajax_utils/js/utils.js` & `mireq_django_ajax_utils-0.0.4/django_ajax_utils/static/django_ajax_utils/js/utils.js`

 * *Files identical despite different names*

### Comparing `mireq_django_ajax_utils-0.0.3/django_ajax_utils/static/django_ajax_utils/js/utils_ajax.js` & `mireq_django_ajax_utils-0.0.4/django_ajax_utils/static/django_ajax_utils/js/utils_ajax.js`

 * *Files identical despite different names*

### Comparing `mireq_django_ajax_utils-0.0.3/django_ajax_utils/templates/form_utils/row/default.html` & `mireq_django_ajax_utils-0.0.4/django_ajax_utils/templates/form_utils/row/default.html`

 * *Files identical despite different names*

### Comparing `mireq_django_ajax_utils-0.0.3/django_ajax_utils/templates/form_utils/row/foundation.html` & `mireq_django_ajax_utils-0.0.4/django_ajax_utils/templates/form_utils/row/foundation.html`

 * *Files identical despite different names*

### Comparing `mireq_django_ajax_utils-0.0.3/django_ajax_utils/templatetags/form_utils.py` & `mireq_django_ajax_utils-0.0.4/django_ajax_utils/templatetags/form_utils.py`

 * *Files identical despite different names*

### Comparing `mireq_django_ajax_utils-0.0.3/django_ajax_utils/templatetags/js_urlpatterns.py` & `mireq_django_ajax_utils-0.0.4/django_ajax_utils/templatetags/js_urlpatterns.py`

 * *Files identical despite different names*

### Comparing `mireq_django_ajax_utils-0.0.3/django_ajax_utils/templatetags/pjax_tags.py` & `mireq_django_ajax_utils-0.0.4/django_ajax_utils/templatetags/pjax_tags.py`

 * *Files identical despite different names*

### Comparing `mireq_django_ajax_utils-0.0.3/django_ajax_utils/utility.py` & `mireq_django_ajax_utils-0.0.4/django_ajax_utils/utility.py`

 * *Files identical despite different names*

### Comparing `mireq_django_ajax_utils-0.0.3/django_ajax_utils/views.py` & `mireq_django_ajax_utils-0.0.4/django_ajax_utils/views.py`

 * *Files identical despite different names*

### Comparing `mireq_django_ajax_utils-0.0.3/mireq_django_ajax_utils.egg-info/PKG-INFO` & `mireq_django_ajax_utils-0.0.4/mireq_django_ajax_utils.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: mireq-django-ajax-utils
-Version: 0.0.3
+Name: mireq_django_ajax_utils
+Version: 0.0.4
 Summary: Django ajax utils
 Author-email: Miroslav Bendík <miroslav.bendik@gmail.com>
 License: MIT
 Project-URL: homepage, https://github.com/mireq/django-ajax-utils
 Project-URL: documentation, https://github.com/mireq/django-ajax-utils
 Project-URL: repository, https://github.com/mireq/django-ajax-utils
 Project-URL: changelog, https://github.com/mireq/django-ajax-utils/blob/master/CHANGELOG.md
```

### Comparing `mireq_django_ajax_utils-0.0.3/mireq_django_ajax_utils.egg-info/SOURCES.txt` & `mireq_django_ajax_utils-0.0.4/mireq_django_ajax_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mireq_django_ajax_utils-0.0.3/pyproject.toml` & `mireq_django_ajax_utils-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -49,9 +49,9 @@
 where = ["."]
 include = ["django_ajax_utils*"]
 
 [tool.setuptools_scm]
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.0.3"
+version = "0.0.4"
 tag_format = "$version"
```

### Comparing `mireq_django_ajax_utils-0.0.3/sample_project/manage.py` & `mireq_django_ajax_utils-0.0.4/sample_project/manage.py`

 * *Files identical despite different names*

### Comparing `mireq_django_ajax_utils-0.0.3/sample_project/static/css/style.css` & `mireq_django_ajax_utils-0.0.4/sample_project/static/css/style.css`

 * *Files identical despite different names*

### Comparing `mireq_django_ajax_utils-0.0.3/sample_project/static/js/pjax_init.js` & `mireq_django_ajax_utils-0.0.4/sample_project/static/js/pjax_init.js`

 * *Files identical despite different names*

### Comparing `mireq_django_ajax_utils-0.0.3/sample_project/static/js/run_utils.js` & `mireq_django_ajax_utils-0.0.4/sample_project/static/js/run_utils.js`

 * *Files identical despite different names*

### Comparing `mireq_django_ajax_utils-0.0.3/sample_project/templates/ajaxform.html` & `mireq_django_ajax_utils-0.0.4/sample_project/templates/ajaxform.html`

 * *Files identical despite different names*

### Comparing `mireq_django_ajax_utils-0.0.3/sample_project/templates/base.html` & `mireq_django_ajax_utils-0.0.4/sample_project/templates/base.html`

 * *Files identical despite different names*

### Comparing `mireq_django_ajax_utils-0.0.3/sample_project/templates/base_pjax.html` & `mireq_django_ajax_utils-0.0.4/sample_project/templates/base_pjax.html`

 * *Files identical despite different names*

### Comparing `mireq_django_ajax_utils-0.0.3/sample_project/templates/form_utils/base.html` & `mireq_django_ajax_utils-0.0.4/sample_project/templates/form_utils/base.html`

 * *Files identical despite different names*

### Comparing `mireq_django_ajax_utils-0.0.3/sample_project/templates/form_utils/foundation.html` & `mireq_django_ajax_utils-0.0.4/sample_project/templates/form_utils/foundation.html`

 * *Files identical despite different names*

### Comparing `mireq_django_ajax_utils-0.0.3/sample_project/templates/form_utils/multiforms.html` & `mireq_django_ajax_utils-0.0.4/sample_project/templates/form_utils/multiforms.html`

 * *Files identical despite different names*

### Comparing `mireq_django_ajax_utils-0.0.3/sample_project/templates/includes/form_loop.html` & `mireq_django_ajax_utils-0.0.4/sample_project/templates/includes/form_loop.html`

 * *Files identical despite different names*

### Comparing `mireq_django_ajax_utils-0.0.3/sample_project/templates/messages.html` & `mireq_django_ajax_utils-0.0.4/sample_project/templates/messages.html`

 * *Files identical despite different names*

### Comparing `mireq_django_ajax_utils-0.0.3/sample_project/templates/partials/menu.html` & `mireq_django_ajax_utils-0.0.4/sample_project/templates/partials/menu.html`

 * *Files identical despite different names*

### Comparing `mireq_django_ajax_utils-0.0.3/sample_project/templates/pjax.html` & `mireq_django_ajax_utils-0.0.4/sample_project/templates/pjax.html`

 * *Files identical despite different names*

### Comparing `mireq_django_ajax_utils-0.0.3/sample_project/templates/pjax_form_get.html` & `mireq_django_ajax_utils-0.0.4/sample_project/templates/pjax_form_get.html`

 * *Files identical despite different names*

### Comparing `mireq_django_ajax_utils-0.0.3/sample_project/templates/pjax_messages.html` & `mireq_django_ajax_utils-0.0.4/sample_project/templates/pjax_messages.html`

 * *Files identical despite different names*

### Comparing `mireq_django_ajax_utils-0.0.3/sample_project/templates/pjax_page.html` & `mireq_django_ajax_utils-0.0.4/sample_project/templates/pjax_page.html`

 * *Files identical despite different names*

### Comparing `mireq_django_ajax_utils-0.0.3/sample_project/templates/urlpatterns.html` & `mireq_django_ajax_utils-0.0.4/sample_project/templates/urlpatterns.html`

 * *Files identical despite different names*

### Comparing `mireq_django_ajax_utils-0.0.3/sample_project/templates/utils.html` & `mireq_django_ajax_utils-0.0.4/sample_project/templates/utils.html`

 * *Files identical despite different names*

### Comparing `mireq_django_ajax_utils-0.0.3/sample_project/web/forms.py` & `mireq_django_ajax_utils-0.0.4/sample_project/web/forms.py`

 * *Files identical despite different names*

### Comparing `mireq_django_ajax_utils-0.0.3/sample_project/web/settings.py` & `mireq_django_ajax_utils-0.0.4/sample_project/web/settings.py`

 * *Files identical despite different names*

### Comparing `mireq_django_ajax_utils-0.0.3/sample_project/web/urls.py` & `mireq_django_ajax_utils-0.0.4/sample_project/web/urls.py`

 * *Files identical despite different names*

### Comparing `mireq_django_ajax_utils-0.0.3/sample_project/web/views.py` & `mireq_django_ajax_utils-0.0.4/sample_project/web/views.py`

 * *Files identical despite different names*

