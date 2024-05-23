# Comparing `tmp/django_medilab_ds-3.0.0.tar.gz` & `tmp/django_medilab_ds-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_medilab_ds-3.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "django_medilab_ds-3.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `django_medilab_ds-3.0.0.tar` & `django_medilab_ds-3.0.1.tar`

### file list

```diff
@@ -1,160 +1,160 @@
--rw-r--r--   0        0        0     8196 2024-05-18 02:13:53.922895 django_medilab_ds-3.0.0/.DS_Store
--rw-r--r--   0        0        0       66 2024-05-17 05:13:00.571402 django_medilab_ds-3.0.0/.gitattributes
--rw-r--r--   0        0        0       20 2024-05-18 20:39:00.979987 django_medilab_ds-3.0.0/.gitignore
--rw-r--r--   0        0        0       52 2024-05-17 05:14:27.086201 django_medilab_ds-3.0.0/.idea/.gitignore
--rw-r--r--   0        0        0      407 2024-05-17 05:14:26.986248 django_medilab_ds-3.0.0/.idea/django-medilab-ds.iml
--rw-r--r--   0        0        0      174 2024-05-17 05:14:26.999981 django_medilab_ds-3.0.0/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      425 2024-05-17 05:28:06.742745 django_medilab_ds-3.0.0/.idea/misc.xml
--rw-r--r--   0        0        0      286 2024-05-17 05:14:26.992984 django_medilab_ds-3.0.0/.idea/modules.xml
--rw-r--r--   0        0        0      167 2024-05-17 05:14:27.010809 django_medilab_ds-3.0.0/.idea/vcs.xml
--rw-r--r--   0        0        0     1079 2024-03-19 03:45:10.033383 django_medilab_ds-3.0.0/LICENSE
--rw-r--r--   0        0        0     1764 2024-05-22 06:35:29.378054 django_medilab_ds-3.0.0/README.md
--rw-r--r--   0        0        0        0 2024-05-17 05:17:43.155593 django_medilab_ds-3.0.0/django_medilab_ds/__init__.py
--rw-r--r--   0        0        0       63 2024-05-17 05:17:43.156131 django_medilab_ds-3.0.0/django_medilab_ds/admin.py
--rw-r--r--   0        0        0      164 2024-05-17 05:17:43.157309 django_medilab_ds-3.0.0/django_medilab_ds/apps.py
--rw-r--r--   0        0        0      921 2024-05-21 05:02:10.461971 django_medilab_ds-3.0.0/django_medilab_ds/forms.py
--rw-r--r--   0        0        0        0 2024-05-17 05:17:43.157727 django_medilab_ds-3.0.0/django_medilab_ds/migrations/__init__.py
--rw-r--r--   0        0        0       57 2024-05-17 05:17:43.157460 django_medilab_ds-3.0.0/django_medilab_ds/models.py
--rwxr-xr-x   0        0        0    30612 2024-05-21 00:40:32.551366 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/css/style.css
--rwxr-xr-x   0        0        0     5371 2024-03-17 05:37:08.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/js/main.js
--rwxr-xr-x   0        0        0     3160 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/scss/_footer.scss
--rwxr-xr-x   0        0        0     1769 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/scss/_general.scss
--rwxr-xr-x   0        0        0     1981 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/scss/_header.scss
--rwxr-xr-x   0        0        0     1424 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/scss/_hero.scss
--rwxr-xr-x   0        0        0     3911 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/scss/_nav.scss
--rwxr-xr-x   0        0        0    20291 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/scss/_sections.scss
--rwxr-xr-x   0        0        0      454 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/scss/_variables.scss
--rwxr-xr-x   0        0        0      136 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/scss/style.scss
--rw-r--r--   0        0        0    70607 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/animate.css/animate.compat.css
--rw-r--r--   0        0        0    95374 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/animate.css/animate.css
--rwxr-xr-x   0        0        0    71750 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/animate.css/animate.min.css
--rw-r--r--   0        0        0    98255 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/bootstrap-icons/bootstrap-icons.css
--rw-r--r--   0        0        0    52358 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/bootstrap-icons/bootstrap-icons.json
--rw-r--r--   0        0        0    85875 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/bootstrap-icons/bootstrap-icons.min.css
--rw-r--r--   0        0        0    57755 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/bootstrap-icons/bootstrap-icons.scss
--rw-r--r--   0        0        0   176032 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/bootstrap-icons/fonts/bootstrap-icons.woff
--rw-r--r--   0        0        0   130396 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/bootstrap-icons/fonts/bootstrap-icons.woff2
--rw-r--r--   0        0        0    70329 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap-grid.css
--rw-r--r--   0        0        0   203221 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap-grid.css.map
--rw-r--r--   0        0        0    51795 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap-grid.min.css
--rw-r--r--   0        0        0   115986 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap-grid.min.css.map
--rw-r--r--   0        0        0    70403 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap-grid.rtl.css
--rw-r--r--   0        0        0   203225 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap-grid.rtl.css.map
--rw-r--r--   0        0        0    51870 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap-grid.rtl.min.css
--rw-r--r--   0        0        0   116063 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap-grid.rtl.min.css.map
--rw-r--r--   0        0        0    12065 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap-reboot.css
--rw-r--r--   0        0        0   129371 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap-reboot.css.map
--rw-r--r--   0        0        0    10126 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap-reboot.min.css
--rw-r--r--   0        0        0    51369 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap-reboot.min.css.map
--rw-r--r--   0        0        0    12058 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap-reboot.rtl.css
--rw-r--r--   0        0        0   129386 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap-reboot.rtl.css.map
--rw-r--r--   0        0        0    10198 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css
--rw-r--r--   0        0        0    63943 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css.map
--rw-r--r--   0        0        0   107823 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap-utilities.css
--rw-r--r--   0        0        0   267535 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap-utilities.css.map
--rw-r--r--   0        0        0    85352 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap-utilities.min.css
--rw-r--r--   0        0        0   180381 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap-utilities.min.css.map
--rw-r--r--   0        0        0   107691 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap-utilities.rtl.css
--rw-r--r--   0        0        0   267476 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap-utilities.rtl.css.map
--rw-r--r--   0        0        0    85281 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css
--rw-r--r--   0        0        0   180217 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css.map
--rw-r--r--   0        0        0   281046 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap.css
--rw-r--r--   0        0        0   679755 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap.css.map
--rw-r--r--   0        0        0   232803 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap.min.css
--rw-r--r--   0        0        0   589892 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap.min.css.map
--rw-r--r--   0        0        0   280259 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap.rtl.css
--rw-r--r--   0        0        0   679615 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap.rtl.css.map
--rw-r--r--   0        0        0   232911 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap.rtl.min.css
--rw-r--r--   0        0        0   589087 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap.rtl.min.css.map
--rw-r--r--   0        0        0   207819 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/bootstrap/js/bootstrap.bundle.js
--rw-r--r--   0        0        0   444579 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/bootstrap/js/bootstrap.bundle.js.map
--rw-r--r--   0        0        0    80721 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/bootstrap/js/bootstrap.bundle.min.js
--rw-r--r--   0        0        0   332090 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/bootstrap/js/bootstrap.bundle.min.js.map
--rw-r--r--   0        0        0   135829 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/bootstrap/js/bootstrap.esm.js
--rw-r--r--   0        0        0   305438 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/bootstrap/js/bootstrap.esm.js.map
--rw-r--r--   0        0        0    73935 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/bootstrap/js/bootstrap.esm.min.js
--rw-r--r--   0        0        0   222455 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/bootstrap/js/bootstrap.esm.min.js.map
--rw-r--r--   0        0        0   145401 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/bootstrap/js/bootstrap.js
--rw-r--r--   0        0        0   306606 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/bootstrap/js/bootstrap.js.map
--rw-r--r--   0        0        0    60635 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/bootstrap/js/bootstrap.min.js
--rw-r--r--   0        0        0   220561 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/bootstrap/js/bootstrap.min.js.map
--rw-r--r--   0        0        0     7522 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/boxicons/css/animations.css
--rw-r--r--   0        0        0    94202 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/boxicons/css/boxicons.css
--rw-r--r--   0        0        0    68028 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/boxicons/css/boxicons.min.css
--rw-r--r--   0        0        0      683 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/boxicons/css/transformations.css
--rw-r--r--   0        0        0   405670 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/boxicons/fonts/boxicons.eot
--rw-r--r--   0        0        0  1242122 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/boxicons/fonts/boxicons.svg
--rw-r--r--   0        0        0   320944 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/boxicons/fonts/boxicons.ttf
--rw-r--r--   0        0        0   321020 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/boxicons/fonts/boxicons.woff
--rw-r--r--   0        0        0   115680 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/boxicons/fonts/boxicons.woff2
--rw-r--r--   0        0        0   141265 2024-04-07 13:11:34.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/fontawesome-free/css/all.css
--rw-r--r--   0        0        0   103009 2024-04-07 13:11:34.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/fontawesome-free/css/all.min.css
--rw-r--r--   0        0        0    24920 2024-04-07 13:11:34.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/fontawesome-free/css/brands.css
--rw-r--r--   0        0        0    19582 2024-04-07 13:11:34.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/fontawesome-free/css/brands.min.css
--rw-r--r--   0        0        0   113480 2024-04-07 13:11:34.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/fontawesome-free/css/fontawesome.css
--rw-r--r--   0        0        0    80888 2024-04-07 13:11:34.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/fontawesome-free/css/fontawesome.min.css
--rw-r--r--   0        0        0      633 2024-04-07 13:11:34.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/fontawesome-free/css/regular.css
--rw-r--r--   0        0        0      580 2024-04-07 13:11:34.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/fontawesome-free/css/regular.min.css
--rw-r--r--   0        0        0      625 2024-04-07 13:11:34.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/fontawesome-free/css/solid.css
--rw-r--r--   0        0        0      572 2024-04-07 13:11:34.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/fontawesome-free/css/solid.min.css
--rw-r--r--   0        0        0    21696 2024-04-07 13:11:34.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/fontawesome-free/css/svg-with-js.css
--rw-r--r--   0        0        0    17011 2024-04-07 13:11:34.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/fontawesome-free/css/svg-with-js.min.css
--rw-r--r--   0        0        0     1831 2024-04-07 13:11:34.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/fontawesome-free/css/v4-font-face.css
--rw-r--r--   0        0        0     1736 2024-04-07 13:11:34.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/fontawesome-free/css/v4-font-face.min.css
--rw-r--r--   0        0        0    41574 2024-04-07 13:11:34.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/fontawesome-free/css/v4-shims.css
--rw-r--r--   0        0        0    27593 2024-04-07 13:11:34.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/fontawesome-free/css/v4-shims.min.css
--rw-r--r--   0        0        0      871 2024-04-07 13:11:34.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/fontawesome-free/css/v5-font-face.css
--rw-r--r--   0        0        0      794 2024-04-07 13:11:34.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/fontawesome-free/css/v5-font-face.min.css
--rw-r--r--   0        0        0   209128 2024-04-07 13:11:34.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/fontawesome-free/webfonts/fa-brands-400.ttf
--rw-r--r--   0        0        0   117852 2024-04-07 13:11:34.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/fontawesome-free/webfonts/fa-brands-400.woff2
--rw-r--r--   0        0        0    67860 2024-04-07 13:11:34.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/fontawesome-free/webfonts/fa-regular-400.ttf
--rw-r--r--   0        0        0    25392 2024-04-07 13:11:34.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/fontawesome-free/webfonts/fa-regular-400.woff2
--rw-r--r--   0        0        0   420332 2024-04-07 13:11:34.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/fontawesome-free/webfonts/fa-solid-900.ttf
--rw-r--r--   0        0        0   156400 2024-04-07 13:11:34.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/fontawesome-free/webfonts/fa-solid-900.woff2
--rw-r--r--   0        0        0    10832 2024-04-07 13:11:34.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/fontawesome-free/webfonts/fa-v4compatibility.ttf
--rw-r--r--   0        0        0     4792 2024-04-07 13:11:34.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/fontawesome-free/webfonts/fa-v4compatibility.woff2
--rw-r--r--   0        0        0    17372 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/glightbox/css/glightbox.css
--rw-r--r--   0        0        0    13749 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/glightbox/css/glightbox.min.css
--rw-r--r--   0        0        0   109600 2024-04-07 13:11:34.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/glightbox/js/glightbox.js
--rw-r--r--   0        0        0    56300 2024-04-07 13:11:34.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/glightbox/js/glightbox.min.js
--rwxr-xr-x   0        0        0   238381 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/php-email-form/php-email-form.php
--rwxr-xr-x   0        0        0     2734 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/php-email-form/validate.js
--rw-r--r--   0        0        0     5417 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/purecounter/purecounter_vanilla.js
--rw-r--r--   0        0        0    24750 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/purecounter/purecounter_vanilla.js.map
--rw-r--r--   0        0        0   138761 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/remixicon/remixicon.css
--rw-r--r--   0        0        0   525744 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/remixicon/remixicon.eot
--rw-r--r--   0        0        0  3776084 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/remixicon/remixicon.glyph.json
--rw-r--r--   0        0        0   138773 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/remixicon/remixicon.less
--rw-r--r--   0        0        0  2460531 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/remixicon/remixicon.svg
--rw-r--r--   0        0        0  1582046 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/remixicon/remixicon.symbol.svg
--rw-r--r--   0        0        0   525572 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/remixicon/remixicon.ttf
--rw-r--r--   0        0        0   224116 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/remixicon/remixicon.woff
--rw-r--r--   0        0        0   163200 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/remixicon/remixicon.woff2
--rw-r--r--   0        0        0    18432 2024-04-20 04:09:20.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/swiper/swiper-bundle.min.css
--rw-r--r--   0        0        0   149982 2024-04-20 04:09:20.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/swiper/swiper-bundle.min.js
--rw-r--r--   0        0        0   203001 2024-04-20 04:09:20.000000 django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/swiper/swiper-bundle.min.js.map
--rw-r--r--   0        0        0     1085 2024-05-22 06:34:05.468294 django_medilab_ds-3.0.0/django_medilab_ds/templates/medilabds/_about.html
--rw-r--r--   0        0        0     1201 2024-05-22 06:34:05.457467 django_medilab_ds-3.0.0/django_medilab_ds/templates/medilabds/_appointment.html
--rw-r--r--   0        0        0     2451 2024-05-22 03:10:40.068399 django_medilab_ds-3.0.0/django_medilab_ds/templates/medilabds/_contact.html
--rw-r--r--   0        0        0      481 2024-05-21 02:28:41.815055 django_medilab_ds-3.0.0/django_medilab_ds/templates/medilabds/_counts.html
--rw-r--r--   0        0        0     1407 2024-05-22 06:34:05.464894 django_medilab_ds-3.0.0/django_medilab_ds/templates/medilabds/_departments.html
--rw-r--r--   0        0        0     1397 2024-05-22 06:34:05.481019 django_medilab_ds-3.0.0/django_medilab_ds/templates/medilabds/_doctors.html
--rw-r--r--   0        0        0     1009 2024-05-21 07:04:19.229553 django_medilab_ds-3.0.0/django_medilab_ds/templates/medilabds/_faq.html
--rw-r--r--   0        0        0      705 2024-05-22 01:55:04.082872 django_medilab_ds-3.0.0/django_medilab_ds/templates/medilabds/_gallery.html
--rw-r--r--   0        0        0      528 2024-05-22 06:34:05.461548 django_medilab_ds-3.0.0/django_medilab_ds/templates/medilabds/_hero.html
--rw-r--r--   0        0        0      630 2024-05-21 05:04:08.067506 django_medilab_ds-3.0.0/django_medilab_ds/templates/medilabds/_services.html
--rw-r--r--   0        0        0     1021 2024-05-22 06:34:05.473750 django_medilab_ds-3.0.0/django_medilab_ds/templates/medilabds/_testimonials.html
--rw-r--r--   0        0        0     1198 2024-05-21 01:13:06.372770 django_medilab_ds-3.0.0/django_medilab_ds/templates/medilabds/_why-us.html
--rw-r--r--   0        0        0     2635 2024-05-18 00:37:24.994770 django_medilab_ds-3.0.0/django_medilab_ds/templates/medilabds/footer.html
--rwxr-xr-x   0        0        0     1579 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.0/django_medilab_ds/templates/medilabds/forms/appointment.php
--rwxr-xr-x   0        0        0     1341 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.0/django_medilab_ds/templates/medilabds/forms/contact.php
--rw-r--r--   0        0        0     2780 2024-05-22 06:15:39.187054 django_medilab_ds-3.0.0/django_medilab_ds/templates/medilabds/header.html
--rwxr-xr-x   0        0        0     4113 2024-05-22 06:23:37.291337 django_medilab_ds-3.0.0/django_medilab_ds/templates/medilabds/index.html
--rwxr-xr-x   0        0        0     8842 2024-03-17 05:37:08.000000 django_medilab_ds-3.0.0/django_medilab_ds/templates/medilabds/inner-page.html
--rw-r--r--   0        0        0     1935 2024-05-22 06:20:30.241173 django_medilab_ds-3.0.0/django_medilab_ds/templates/medilabds/seo.html
--rw-r--r--   0        0        0     5187 2024-05-22 06:23:37.288480 django_medilab_ds-3.0.0/django_medilab_ds/templatetags/medilabds_tags.py
--rw-r--r--   0        0        0       60 2024-05-17 05:17:43.157588 django_medilab_ds-3.0.0/django_medilab_ds/tests.py
--rw-r--r--   0        0        0      264 2024-05-22 06:34:05.476964 django_medilab_ds-3.0.0/django_medilab_ds/urls.py
--rw-r--r--   0        0        0     2382 2024-05-22 00:53:17.156916 django_medilab_ds-3.0.0/django_medilab_ds/views.py
--rw-r--r--   0        0        0      786 2024-05-22 06:35:29.374021 django_medilab_ds-3.0.0/pyproject.toml
--rw-r--r--   0        0        0     2269 1970-01-01 00:00:00.000000 django_medilab_ds-3.0.0/PKG-INFO
+-rw-r--r--   0        0        0     8196 2024-05-18 02:13:53.922895 django_medilab_ds-3.0.1/.DS_Store
+-rw-r--r--   0        0        0       66 2024-05-17 05:13:00.571402 django_medilab_ds-3.0.1/.gitattributes
+-rw-r--r--   0        0        0       20 2024-05-18 20:39:00.979987 django_medilab_ds-3.0.1/.gitignore
+-rw-r--r--   0        0        0       52 2024-05-17 05:14:27.086201 django_medilab_ds-3.0.1/.idea/.gitignore
+-rw-r--r--   0        0        0      407 2024-05-17 05:14:26.986248 django_medilab_ds-3.0.1/.idea/django-medilab-ds.iml
+-rw-r--r--   0        0        0      174 2024-05-17 05:14:26.999981 django_medilab_ds-3.0.1/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      425 2024-05-17 05:28:06.742745 django_medilab_ds-3.0.1/.idea/misc.xml
+-rw-r--r--   0        0        0      286 2024-05-17 05:14:26.992984 django_medilab_ds-3.0.1/.idea/modules.xml
+-rw-r--r--   0        0        0      167 2024-05-17 05:14:27.010809 django_medilab_ds-3.0.1/.idea/vcs.xml
+-rw-r--r--   0        0        0     1079 2024-03-19 03:45:10.033383 django_medilab_ds-3.0.1/LICENSE
+-rw-r--r--   0        0        0     1764 2024-05-22 06:35:29.378054 django_medilab_ds-3.0.1/README.md
+-rw-r--r--   0        0        0        0 2024-05-17 05:17:43.155593 django_medilab_ds-3.0.1/django_medilab_ds/__init__.py
+-rw-r--r--   0        0        0       63 2024-05-17 05:17:43.156131 django_medilab_ds-3.0.1/django_medilab_ds/admin.py
+-rw-r--r--   0        0        0      164 2024-05-17 05:17:43.157309 django_medilab_ds-3.0.1/django_medilab_ds/apps.py
+-rw-r--r--   0        0        0      921 2024-05-21 05:02:10.461971 django_medilab_ds-3.0.1/django_medilab_ds/forms.py
+-rw-r--r--   0        0        0        0 2024-05-17 05:17:43.157727 django_medilab_ds-3.0.1/django_medilab_ds/migrations/__init__.py
+-rw-r--r--   0        0        0       57 2024-05-17 05:17:43.157460 django_medilab_ds-3.0.1/django_medilab_ds/models.py
+-rwxr-xr-x   0        0        0    30612 2024-05-21 00:40:32.551366 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/css/style.css
+-rwxr-xr-x   0        0        0     5371 2024-03-17 05:37:08.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/js/main.js
+-rwxr-xr-x   0        0        0     3160 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/scss/_footer.scss
+-rwxr-xr-x   0        0        0     1769 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/scss/_general.scss
+-rwxr-xr-x   0        0        0     1981 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/scss/_header.scss
+-rwxr-xr-x   0        0        0     1424 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/scss/_hero.scss
+-rwxr-xr-x   0        0        0     3911 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/scss/_nav.scss
+-rwxr-xr-x   0        0        0    20291 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/scss/_sections.scss
+-rwxr-xr-x   0        0        0      454 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/scss/_variables.scss
+-rwxr-xr-x   0        0        0      136 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/scss/style.scss
+-rw-r--r--   0        0        0    70607 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/animate.css/animate.compat.css
+-rw-r--r--   0        0        0    95374 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/animate.css/animate.css
+-rwxr-xr-x   0        0        0    71750 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/animate.css/animate.min.css
+-rw-r--r--   0        0        0    98255 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/bootstrap-icons/bootstrap-icons.css
+-rw-r--r--   0        0        0    52358 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/bootstrap-icons/bootstrap-icons.json
+-rw-r--r--   0        0        0    85875 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/bootstrap-icons/bootstrap-icons.min.css
+-rw-r--r--   0        0        0    57755 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/bootstrap-icons/bootstrap-icons.scss
+-rw-r--r--   0        0        0   176032 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/bootstrap-icons/fonts/bootstrap-icons.woff
+-rw-r--r--   0        0        0   130396 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/bootstrap-icons/fonts/bootstrap-icons.woff2
+-rw-r--r--   0        0        0    70329 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap-grid.css
+-rw-r--r--   0        0        0   203221 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap-grid.css.map
+-rw-r--r--   0        0        0    51795 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap-grid.min.css
+-rw-r--r--   0        0        0   115986 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap-grid.min.css.map
+-rw-r--r--   0        0        0    70403 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap-grid.rtl.css
+-rw-r--r--   0        0        0   203225 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap-grid.rtl.css.map
+-rw-r--r--   0        0        0    51870 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap-grid.rtl.min.css
+-rw-r--r--   0        0        0   116063 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap-grid.rtl.min.css.map
+-rw-r--r--   0        0        0    12065 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap-reboot.css
+-rw-r--r--   0        0        0   129371 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap-reboot.css.map
+-rw-r--r--   0        0        0    10126 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap-reboot.min.css
+-rw-r--r--   0        0        0    51369 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap-reboot.min.css.map
+-rw-r--r--   0        0        0    12058 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap-reboot.rtl.css
+-rw-r--r--   0        0        0   129386 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap-reboot.rtl.css.map
+-rw-r--r--   0        0        0    10198 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css
+-rw-r--r--   0        0        0    63943 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css.map
+-rw-r--r--   0        0        0   107823 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap-utilities.css
+-rw-r--r--   0        0        0   267535 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap-utilities.css.map
+-rw-r--r--   0        0        0    85352 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap-utilities.min.css
+-rw-r--r--   0        0        0   180381 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap-utilities.min.css.map
+-rw-r--r--   0        0        0   107691 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap-utilities.rtl.css
+-rw-r--r--   0        0        0   267476 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap-utilities.rtl.css.map
+-rw-r--r--   0        0        0    85281 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css
+-rw-r--r--   0        0        0   180217 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css.map
+-rw-r--r--   0        0        0   281046 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap.css
+-rw-r--r--   0        0        0   679755 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap.css.map
+-rw-r--r--   0        0        0   232803 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap.min.css
+-rw-r--r--   0        0        0   589892 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap.min.css.map
+-rw-r--r--   0        0        0   280259 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap.rtl.css
+-rw-r--r--   0        0        0   679615 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap.rtl.css.map
+-rw-r--r--   0        0        0   232911 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap.rtl.min.css
+-rw-r--r--   0        0        0   589087 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap.rtl.min.css.map
+-rw-r--r--   0        0        0   207819 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/bootstrap/js/bootstrap.bundle.js
+-rw-r--r--   0        0        0   444579 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/bootstrap/js/bootstrap.bundle.js.map
+-rw-r--r--   0        0        0    80721 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/bootstrap/js/bootstrap.bundle.min.js
+-rw-r--r--   0        0        0   332090 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/bootstrap/js/bootstrap.bundle.min.js.map
+-rw-r--r--   0        0        0   135829 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/bootstrap/js/bootstrap.esm.js
+-rw-r--r--   0        0        0   305438 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/bootstrap/js/bootstrap.esm.js.map
+-rw-r--r--   0        0        0    73935 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/bootstrap/js/bootstrap.esm.min.js
+-rw-r--r--   0        0        0   222455 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/bootstrap/js/bootstrap.esm.min.js.map
+-rw-r--r--   0        0        0   145401 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/bootstrap/js/bootstrap.js
+-rw-r--r--   0        0        0   306606 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/bootstrap/js/bootstrap.js.map
+-rw-r--r--   0        0        0    60635 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/bootstrap/js/bootstrap.min.js
+-rw-r--r--   0        0        0   220561 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/bootstrap/js/bootstrap.min.js.map
+-rw-r--r--   0        0        0     7522 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/boxicons/css/animations.css
+-rw-r--r--   0        0        0    94202 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/boxicons/css/boxicons.css
+-rw-r--r--   0        0        0    68028 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/boxicons/css/boxicons.min.css
+-rw-r--r--   0        0        0      683 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/boxicons/css/transformations.css
+-rw-r--r--   0        0        0   405670 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/boxicons/fonts/boxicons.eot
+-rw-r--r--   0        0        0  1242122 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/boxicons/fonts/boxicons.svg
+-rw-r--r--   0        0        0   320944 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/boxicons/fonts/boxicons.ttf
+-rw-r--r--   0        0        0   321020 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/boxicons/fonts/boxicons.woff
+-rw-r--r--   0        0        0   115680 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/boxicons/fonts/boxicons.woff2
+-rw-r--r--   0        0        0   141265 2024-04-07 13:11:34.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/fontawesome-free/css/all.css
+-rw-r--r--   0        0        0   103009 2024-04-07 13:11:34.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/fontawesome-free/css/all.min.css
+-rw-r--r--   0        0        0    24920 2024-04-07 13:11:34.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/fontawesome-free/css/brands.css
+-rw-r--r--   0        0        0    19582 2024-04-07 13:11:34.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/fontawesome-free/css/brands.min.css
+-rw-r--r--   0        0        0   113480 2024-04-07 13:11:34.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/fontawesome-free/css/fontawesome.css
+-rw-r--r--   0        0        0    80888 2024-04-07 13:11:34.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/fontawesome-free/css/fontawesome.min.css
+-rw-r--r--   0        0        0      633 2024-04-07 13:11:34.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/fontawesome-free/css/regular.css
+-rw-r--r--   0        0        0      580 2024-04-07 13:11:34.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/fontawesome-free/css/regular.min.css
+-rw-r--r--   0        0        0      625 2024-04-07 13:11:34.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/fontawesome-free/css/solid.css
+-rw-r--r--   0        0        0      572 2024-04-07 13:11:34.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/fontawesome-free/css/solid.min.css
+-rw-r--r--   0        0        0    21696 2024-04-07 13:11:34.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/fontawesome-free/css/svg-with-js.css
+-rw-r--r--   0        0        0    17011 2024-04-07 13:11:34.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/fontawesome-free/css/svg-with-js.min.css
+-rw-r--r--   0        0        0     1831 2024-04-07 13:11:34.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/fontawesome-free/css/v4-font-face.css
+-rw-r--r--   0        0        0     1736 2024-04-07 13:11:34.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/fontawesome-free/css/v4-font-face.min.css
+-rw-r--r--   0        0        0    41574 2024-04-07 13:11:34.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/fontawesome-free/css/v4-shims.css
+-rw-r--r--   0        0        0    27593 2024-04-07 13:11:34.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/fontawesome-free/css/v4-shims.min.css
+-rw-r--r--   0        0        0      871 2024-04-07 13:11:34.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/fontawesome-free/css/v5-font-face.css
+-rw-r--r--   0        0        0      794 2024-04-07 13:11:34.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/fontawesome-free/css/v5-font-face.min.css
+-rw-r--r--   0        0        0   209128 2024-04-07 13:11:34.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/fontawesome-free/webfonts/fa-brands-400.ttf
+-rw-r--r--   0        0        0   117852 2024-04-07 13:11:34.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/fontawesome-free/webfonts/fa-brands-400.woff2
+-rw-r--r--   0        0        0    67860 2024-04-07 13:11:34.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/fontawesome-free/webfonts/fa-regular-400.ttf
+-rw-r--r--   0        0        0    25392 2024-04-07 13:11:34.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/fontawesome-free/webfonts/fa-regular-400.woff2
+-rw-r--r--   0        0        0   420332 2024-04-07 13:11:34.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/fontawesome-free/webfonts/fa-solid-900.ttf
+-rw-r--r--   0        0        0   156400 2024-04-07 13:11:34.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/fontawesome-free/webfonts/fa-solid-900.woff2
+-rw-r--r--   0        0        0    10832 2024-04-07 13:11:34.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/fontawesome-free/webfonts/fa-v4compatibility.ttf
+-rw-r--r--   0        0        0     4792 2024-04-07 13:11:34.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/fontawesome-free/webfonts/fa-v4compatibility.woff2
+-rw-r--r--   0        0        0    17372 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/glightbox/css/glightbox.css
+-rw-r--r--   0        0        0    13749 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/glightbox/css/glightbox.min.css
+-rw-r--r--   0        0        0   109600 2024-04-07 13:11:34.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/glightbox/js/glightbox.js
+-rw-r--r--   0        0        0    56300 2024-04-07 13:11:34.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/glightbox/js/glightbox.min.js
+-rwxr-xr-x   0        0        0   238381 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/php-email-form/php-email-form.php
+-rwxr-xr-x   0        0        0     2734 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/php-email-form/validate.js
+-rw-r--r--   0        0        0     5417 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/purecounter/purecounter_vanilla.js
+-rw-r--r--   0        0        0    24750 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/purecounter/purecounter_vanilla.js.map
+-rw-r--r--   0        0        0   138761 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/remixicon/remixicon.css
+-rw-r--r--   0        0        0   525744 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/remixicon/remixicon.eot
+-rw-r--r--   0        0        0  3776084 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/remixicon/remixicon.glyph.json
+-rw-r--r--   0        0        0   138773 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/remixicon/remixicon.less
+-rw-r--r--   0        0        0  2460531 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/remixicon/remixicon.svg
+-rw-r--r--   0        0        0  1582046 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/remixicon/remixicon.symbol.svg
+-rw-r--r--   0        0        0   525572 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/remixicon/remixicon.ttf
+-rw-r--r--   0        0        0   224116 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/remixicon/remixicon.woff
+-rw-r--r--   0        0        0   163200 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/remixicon/remixicon.woff2
+-rw-r--r--   0        0        0    18432 2024-04-20 04:09:20.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/swiper/swiper-bundle.min.css
+-rw-r--r--   0        0        0   149982 2024-04-20 04:09:20.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/swiper/swiper-bundle.min.js
+-rw-r--r--   0        0        0   203001 2024-04-20 04:09:20.000000 django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/swiper/swiper-bundle.min.js.map
+-rw-r--r--   0        0        0     1085 2024-05-22 06:34:05.468294 django_medilab_ds-3.0.1/django_medilab_ds/templates/medilabds/_about.html
+-rw-r--r--   0        0        0     1201 2024-05-22 06:34:05.457467 django_medilab_ds-3.0.1/django_medilab_ds/templates/medilabds/_appointment.html
+-rw-r--r--   0        0        0     2451 2024-05-22 03:10:40.068399 django_medilab_ds-3.0.1/django_medilab_ds/templates/medilabds/_contact.html
+-rw-r--r--   0        0        0      481 2024-05-21 02:28:41.815055 django_medilab_ds-3.0.1/django_medilab_ds/templates/medilabds/_counts.html
+-rw-r--r--   0        0        0     1407 2024-05-22 06:34:05.464894 django_medilab_ds-3.0.1/django_medilab_ds/templates/medilabds/_departments.html
+-rw-r--r--   0        0        0     1397 2024-05-22 06:34:05.481019 django_medilab_ds-3.0.1/django_medilab_ds/templates/medilabds/_doctors.html
+-rw-r--r--   0        0        0     1009 2024-05-21 07:04:19.229553 django_medilab_ds-3.0.1/django_medilab_ds/templates/medilabds/_faq.html
+-rw-r--r--   0        0        0      705 2024-05-22 01:55:04.082872 django_medilab_ds-3.0.1/django_medilab_ds/templates/medilabds/_gallery.html
+-rw-r--r--   0        0        0      528 2024-05-22 06:34:05.461548 django_medilab_ds-3.0.1/django_medilab_ds/templates/medilabds/_hero.html
+-rw-r--r--   0        0        0      630 2024-05-21 05:04:08.067506 django_medilab_ds-3.0.1/django_medilab_ds/templates/medilabds/_services.html
+-rw-r--r--   0        0        0     1021 2024-05-22 06:34:05.473750 django_medilab_ds-3.0.1/django_medilab_ds/templates/medilabds/_testimonials.html
+-rw-r--r--   0        0        0     1198 2024-05-21 01:13:06.372770 django_medilab_ds-3.0.1/django_medilab_ds/templates/medilabds/_why-us.html
+-rw-r--r--   0        0        0     2635 2024-05-18 00:37:24.994770 django_medilab_ds-3.0.1/django_medilab_ds/templates/medilabds/footer.html
+-rwxr-xr-x   0        0        0     1579 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.1/django_medilab_ds/templates/medilabds/forms/appointment.php
+-rwxr-xr-x   0        0        0     1341 2024-03-12 00:49:58.000000 django_medilab_ds-3.0.1/django_medilab_ds/templates/medilabds/forms/contact.php
+-rw-r--r--   0        0        0     2780 2024-05-22 06:15:39.187054 django_medilab_ds-3.0.1/django_medilab_ds/templates/medilabds/header.html
+-rwxr-xr-x   0        0        0     4113 2024-05-22 06:23:37.291337 django_medilab_ds-3.0.1/django_medilab_ds/templates/medilabds/index.html
+-rwxr-xr-x   0        0        0     8842 2024-03-17 05:37:08.000000 django_medilab_ds-3.0.1/django_medilab_ds/templates/medilabds/inner-page.html
+-rw-r--r--   0        0        0     1935 2024-05-22 06:20:30.241173 django_medilab_ds-3.0.1/django_medilab_ds/templates/medilabds/seo.html
+-rw-r--r--   0        0        0     5188 2024-05-22 07:05:42.441819 django_medilab_ds-3.0.1/django_medilab_ds/templatetags/medilabds_tags.py
+-rw-r--r--   0        0        0       60 2024-05-17 05:17:43.157588 django_medilab_ds-3.0.1/django_medilab_ds/tests.py
+-rw-r--r--   0        0        0      264 2024-05-22 07:05:42.452261 django_medilab_ds-3.0.1/django_medilab_ds/urls.py
+-rw-r--r--   0        0        0     2383 2024-05-22 07:05:42.445726 django_medilab_ds-3.0.1/django_medilab_ds/views.py
+-rw-r--r--   0        0        0      786 2024-05-22 07:06:01.954893 django_medilab_ds-3.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2269 1970-01-01 00:00:00.000000 django_medilab_ds-3.0.1/PKG-INFO
```

### Comparing `django_medilab_ds-3.0.0/.DS_Store` & `django_medilab_ds-3.0.1/.DS_Store`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/LICENSE` & `django_medilab_ds-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/README.md` & `django_medilab_ds-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/forms.py` & `django_medilab_ds-3.0.1/django_medilab_ds/forms.py`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/css/style.css` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/css/style.css`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/js/main.js` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/js/main.js`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/scss/_footer.scss` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/scss/_footer.scss`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/scss/_general.scss` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/scss/_general.scss`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/scss/_header.scss` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/scss/_header.scss`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/scss/_hero.scss` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/scss/_hero.scss`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/scss/_nav.scss` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/scss/_nav.scss`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/scss/_sections.scss` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/scss/_sections.scss`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/animate.css/animate.compat.css` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/animate.css/animate.compat.css`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/animate.css/animate.css` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/animate.css/animate.css`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/animate.css/animate.min.css` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/animate.css/animate.min.css`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/bootstrap-icons/bootstrap-icons.css` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/bootstrap-icons/bootstrap-icons.css`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/bootstrap-icons/bootstrap-icons.json` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/bootstrap-icons/bootstrap-icons.json`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/bootstrap-icons/bootstrap-icons.min.css` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/bootstrap-icons/bootstrap-icons.min.css`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/bootstrap-icons/bootstrap-icons.scss` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/bootstrap-icons/bootstrap-icons.scss`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/bootstrap-icons/fonts/bootstrap-icons.woff` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/bootstrap-icons/fonts/bootstrap-icons.woff`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/bootstrap-icons/fonts/bootstrap-icons.woff2` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/bootstrap-icons/fonts/bootstrap-icons.woff2`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap-grid.css` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap-grid.css`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap-grid.css.map` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap-grid.css.map`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap-grid.min.css` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap-grid.min.css`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap-grid.min.css.map` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap-grid.min.css.map`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap-grid.rtl.css` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap-grid.rtl.css`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap-grid.rtl.css.map` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap-grid.rtl.css.map`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap-grid.rtl.min.css` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap-grid.rtl.min.css`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap-grid.rtl.min.css.map` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap-grid.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap-reboot.css` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap-reboot.css`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap-reboot.css.map` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap-reboot.css.map`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap-reboot.min.css` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap-reboot.min.css`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap-reboot.min.css.map` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap-reboot.min.css.map`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap-reboot.rtl.css` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap-reboot.rtl.css`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap-reboot.rtl.css.map` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap-reboot.rtl.css.map`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css.map` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap-utilities.css` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap-utilities.css`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap-utilities.css.map` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap-utilities.css.map`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap-utilities.min.css` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap-utilities.min.css`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap-utilities.min.css.map` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap-utilities.min.css.map`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap-utilities.rtl.css` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap-utilities.rtl.css`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap-utilities.rtl.css.map` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap-utilities.rtl.css.map`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css.map` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap.css` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap.css.map` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap.min.css` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap.min.css.map` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap.rtl.css` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap.rtl.css`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap.rtl.css.map` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap.rtl.css.map`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap.rtl.min.css` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap.rtl.min.css`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap.rtl.min.css.map` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/bootstrap/css/bootstrap.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/bootstrap/js/bootstrap.bundle.js` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/bootstrap/js/bootstrap.bundle.js`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/bootstrap/js/bootstrap.bundle.js.map` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/bootstrap/js/bootstrap.bundle.js.map`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/bootstrap/js/bootstrap.bundle.min.js` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/bootstrap/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/bootstrap/js/bootstrap.bundle.min.js.map` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/bootstrap/js/bootstrap.bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/bootstrap/js/bootstrap.esm.js` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/bootstrap/js/bootstrap.esm.js`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/bootstrap/js/bootstrap.esm.js.map` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/bootstrap/js/bootstrap.esm.js.map`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/bootstrap/js/bootstrap.esm.min.js` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/bootstrap/js/bootstrap.esm.min.js`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/bootstrap/js/bootstrap.esm.min.js.map` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/bootstrap/js/bootstrap.esm.min.js.map`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/bootstrap/js/bootstrap.js` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/bootstrap/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/bootstrap/js/bootstrap.js.map` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/bootstrap/js/bootstrap.js.map`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/bootstrap/js/bootstrap.min.js` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/bootstrap/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/bootstrap/js/bootstrap.min.js.map` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/bootstrap/js/bootstrap.min.js.map`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/boxicons/css/animations.css` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/boxicons/css/animations.css`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/boxicons/css/boxicons.css` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/boxicons/css/boxicons.css`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/boxicons/css/boxicons.min.css` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/boxicons/css/boxicons.min.css`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/boxicons/css/transformations.css` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/boxicons/css/transformations.css`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/boxicons/fonts/boxicons.eot` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/boxicons/fonts/boxicons.eot`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/boxicons/fonts/boxicons.svg` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/boxicons/fonts/boxicons.svg`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/boxicons/fonts/boxicons.ttf` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/boxicons/fonts/boxicons.ttf`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/boxicons/fonts/boxicons.woff` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/boxicons/fonts/boxicons.woff`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/boxicons/fonts/boxicons.woff2` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/boxicons/fonts/boxicons.woff2`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/fontawesome-free/css/all.css` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/fontawesome-free/css/all.css`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/fontawesome-free/css/all.min.css` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/fontawesome-free/css/all.min.css`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/fontawesome-free/css/brands.css` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/fontawesome-free/css/brands.css`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/fontawesome-free/css/brands.min.css` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/fontawesome-free/css/brands.min.css`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/fontawesome-free/css/fontawesome.css` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/fontawesome-free/css/fontawesome.css`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/fontawesome-free/css/fontawesome.min.css` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/fontawesome-free/css/fontawesome.min.css`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/fontawesome-free/css/regular.css` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/fontawesome-free/css/regular.css`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/fontawesome-free/css/regular.min.css` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/fontawesome-free/css/regular.min.css`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/fontawesome-free/css/solid.css` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/fontawesome-free/css/solid.css`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/fontawesome-free/css/solid.min.css` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/fontawesome-free/css/solid.min.css`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/fontawesome-free/css/svg-with-js.css` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/fontawesome-free/css/svg-with-js.css`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/fontawesome-free/css/svg-with-js.min.css` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/fontawesome-free/css/svg-with-js.min.css`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/fontawesome-free/css/v4-font-face.css` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/fontawesome-free/css/v4-font-face.css`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/fontawesome-free/css/v4-font-face.min.css` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/fontawesome-free/css/v4-font-face.min.css`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/fontawesome-free/css/v4-shims.css` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/fontawesome-free/css/v4-shims.css`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/fontawesome-free/css/v4-shims.min.css` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/fontawesome-free/css/v4-shims.min.css`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/fontawesome-free/css/v5-font-face.css` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/fontawesome-free/css/v5-font-face.css`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/fontawesome-free/css/v5-font-face.min.css` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/fontawesome-free/css/v5-font-face.min.css`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/fontawesome-free/webfonts/fa-brands-400.ttf` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/fontawesome-free/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/fontawesome-free/webfonts/fa-brands-400.woff2` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/fontawesome-free/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/fontawesome-free/webfonts/fa-regular-400.ttf` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/fontawesome-free/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/fontawesome-free/webfonts/fa-regular-400.woff2` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/fontawesome-free/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/fontawesome-free/webfonts/fa-solid-900.ttf` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/fontawesome-free/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/fontawesome-free/webfonts/fa-solid-900.woff2` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/fontawesome-free/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/fontawesome-free/webfonts/fa-v4compatibility.ttf` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/fontawesome-free/webfonts/fa-v4compatibility.ttf`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/fontawesome-free/webfonts/fa-v4compatibility.woff2` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/fontawesome-free/webfonts/fa-v4compatibility.woff2`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/glightbox/css/glightbox.css` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/glightbox/css/glightbox.css`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/glightbox/css/glightbox.min.css` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/glightbox/css/glightbox.min.css`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/glightbox/js/glightbox.js` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/glightbox/js/glightbox.js`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/glightbox/js/glightbox.min.js` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/glightbox/js/glightbox.min.js`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/php-email-form/php-email-form.php` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/php-email-form/php-email-form.php`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/php-email-form/validate.js` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/php-email-form/validate.js`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/purecounter/purecounter_vanilla.js` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/purecounter/purecounter_vanilla.js`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/purecounter/purecounter_vanilla.js.map` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/purecounter/purecounter_vanilla.js.map`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/remixicon/remixicon.css` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/remixicon/remixicon.css`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/remixicon/remixicon.eot` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/remixicon/remixicon.eot`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/remixicon/remixicon.glyph.json` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/remixicon/remixicon.glyph.json`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/remixicon/remixicon.less` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/remixicon/remixicon.less`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/remixicon/remixicon.svg` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/remixicon/remixicon.svg`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/remixicon/remixicon.symbol.svg` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/remixicon/remixicon.symbol.svg`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/remixicon/remixicon.ttf` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/remixicon/remixicon.ttf`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/remixicon/remixicon.woff` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/remixicon/remixicon.woff`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/remixicon/remixicon.woff2` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/remixicon/remixicon.woff2`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/swiper/swiper-bundle.min.css` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/swiper/swiper-bundle.min.css`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/swiper/swiper-bundle.min.js` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/swiper/swiper-bundle.min.js`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/static/medilabds/vendor/swiper/swiper-bundle.min.js.map` & `django_medilab_ds-3.0.1/django_medilab_ds/static/medilabds/vendor/swiper/swiper-bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/templates/medilabds/_about.html` & `django_medilab_ds-3.0.1/django_medilab_ds/templates/medilabds/_about.html`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/templates/medilabds/_appointment.html` & `django_medilab_ds-3.0.1/django_medilab_ds/templates/medilabds/_appointment.html`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/templates/medilabds/_contact.html` & `django_medilab_ds-3.0.1/django_medilab_ds/templates/medilabds/_contact.html`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/templates/medilabds/_departments.html` & `django_medilab_ds-3.0.1/django_medilab_ds/templates/medilabds/_departments.html`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/templates/medilabds/_doctors.html` & `django_medilab_ds-3.0.1/django_medilab_ds/templates/medilabds/_doctors.html`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/templates/medilabds/_faq.html` & `django_medilab_ds-3.0.1/django_medilab_ds/templates/medilabds/_faq.html`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/templates/medilabds/_gallery.html` & `django_medilab_ds-3.0.1/django_medilab_ds/templates/medilabds/_gallery.html`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/templates/medilabds/_hero.html` & `django_medilab_ds-3.0.1/django_medilab_ds/templates/medilabds/_hero.html`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/templates/medilabds/_services.html` & `django_medilab_ds-3.0.1/django_medilab_ds/templates/medilabds/_services.html`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/templates/medilabds/_testimonials.html` & `django_medilab_ds-3.0.1/django_medilab_ds/templates/medilabds/_testimonials.html`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/templates/medilabds/_why-us.html` & `django_medilab_ds-3.0.1/django_medilab_ds/templates/medilabds/_why-us.html`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/templates/medilabds/footer.html` & `django_medilab_ds-3.0.1/django_medilab_ds/templates/medilabds/footer.html`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/templates/medilabds/forms/appointment.php` & `django_medilab_ds-3.0.1/django_medilab_ds/templates/medilabds/forms/appointment.php`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/templates/medilabds/forms/contact.php` & `django_medilab_ds-3.0.1/django_medilab_ds/templates/medilabds/forms/contact.php`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/templates/medilabds/header.html` & `django_medilab_ds-3.0.1/django_medilab_ds/templates/medilabds/header.html`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/templates/medilabds/index.html` & `django_medilab_ds-3.0.1/django_medilab_ds/templates/medilabds/index.html`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/templates/medilabds/inner-page.html` & `django_medilab_ds-3.0.1/django_medilab_ds/templates/medilabds/inner-page.html`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/templates/medilabds/seo.html` & `django_medilab_ds-3.0.1/django_medilab_ds/templates/medilabds/seo.html`

 * *Files identical despite different names*

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/templatetags/medilabds_tags.py` & `django_medilab_ds-3.0.1/django_medilab_ds/templatetags/medilabds_tags.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 
 register = Library()
 
 # https://localcoder.org/django-inclusion-tag-with-configurable-template
 
 
-template_name = medilabds.context['templatename']
+template_name = medilabds.context['template_name']
 
 
 @register.simple_tag(takes_context=True)
 def seo(context):
     t = loader.get_template(template_name + "/seo.html")
     context.update({
         'template_name': template_name,
```

### Comparing `django_medilab_ds-3.0.0/django_medilab_ds/views.py` & `django_medilab_ds-3.0.1/django_medilab_ds/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 logger = logging.getLogger(__name__)
 formatter = logging.Formatter('%(levelname)s: [%(name)s] %(message)s')
 ch = logging.StreamHandler()
 ch.setFormatter(formatter)
 logger.addHandler(ch)
 logger.setLevel(logging.ERROR)
 
-template_name = medilabds.context['templatename']
+template_name = medilabds.context['template_name']
 
 
 def robots(request):
     from django.shortcuts import HttpResponse
     file_content = utils.make_robots()
     return HttpResponse(file_content, content_type="text/plain")
```

### Comparing `django_medilab_ds-3.0.0/pyproject.toml` & `django_medilab_ds-3.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "django_medilab_ds"
-version = "3.0.0"
+version = "3.0.1"
 description = "my demiansoft templates"
 authors = [{name = "Hyungjin Kim", email = "hj3415@gmail.com"}]
 readme = "README.md"
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: MIT License"]
 dependencies = [
     "Django >= 4.2.11",
```

### Comparing `django_medilab_ds-3.0.0/PKG-INFO` & `django_medilab_ds-3.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_medilab_ds
-Version: 3.0.0
+Version: 3.0.1
 Summary: my demiansoft templates
 Author-email: Hyungjin Kim <hj3415@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: Django >= 4.2.11
 Requires-Dist: libsass>=0.23.0
 Requires-Dist: django-analyticsds >= 0.3.1
```

