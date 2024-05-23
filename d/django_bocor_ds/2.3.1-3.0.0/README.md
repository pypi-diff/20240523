# Comparing `tmp/django_bocor_ds-2.3.1.tar.gz` & `tmp/django_bocor_ds-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_bocor_ds-2.3.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "django_bocor_ds-3.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `django_bocor_ds-2.3.1.tar` & `django_bocor_ds-3.0.0.tar`

### file list

```diff
@@ -1,136 +1,136 @@
--rw-r--r--   0        0        0    10244 2024-05-18 19:53:20.644327 django_bocor_ds-2.3.1/.DS_Store
--rw-r--r--   0        0        0       66 2024-03-21 05:49:50.372491 django_bocor_ds-2.3.1/.gitattributes
--rw-r--r--   0        0        0       29 2024-05-18 19:35:21.529731 django_bocor_ds-2.3.1/.gitignore
--rw-r--r--   0        0        0       52 2024-03-21 06:06:29.551428 django_bocor_ds-2.3.1/.idea/.gitignore
--rw-r--r--   0        0        0      405 2024-03-21 06:06:29.465715 django_bocor_ds-2.3.1/.idea/django-bocor-ds.iml
--rw-r--r--   0        0        0      174 2024-03-21 06:06:29.480874 django_bocor_ds-2.3.1/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      421 2024-03-21 06:08:26.611158 django_bocor_ds-2.3.1/.idea/misc.xml
--rw-r--r--   0        0        0      282 2024-03-21 06:06:29.471790 django_bocor_ds-2.3.1/.idea/modules.xml
--rw-r--r--   0        0        0      167 2024-03-21 06:06:29.484071 django_bocor_ds-2.3.1/.idea/vcs.xml
--rw-r--r--   0        0        0     1079 2024-03-19 03:45:10.033383 django_bocor_ds-2.3.1/LICENSE
--rw-r--r--   0        0        0     1924 2024-05-18 20:00:17.227329 django_bocor_ds-2.3.1/README.md
--rw-r--r--   0        0        0     6148 2024-04-13 00:02:19.172196 django_bocor_ds-2.3.1/django_bocor_ds/.DS_Store
--rw-r--r--   0        0        0        0 2024-03-21 06:07:02.999245 django_bocor_ds-2.3.1/django_bocor_ds/__init__.py
--rw-r--r--   0        0        0      495 2024-03-26 07:24:10.511682 django_bocor_ds-2.3.1/django_bocor_ds/admin.py
--rw-r--r--   0        0        0      160 2024-03-21 06:07:03.001129 django_bocor_ds-2.3.1/django_bocor_ds/apps.py
--rw-r--r--   0        0        0      947 2024-03-24 12:14:35.423434 django_bocor_ds-2.3.1/django_bocor_ds/forms.py
--rw-r--r--   0        0        0     1915 2024-03-26 07:22:15.008801 django_bocor_ds-2.3.1/django_bocor_ds/migrations/0001_initial.py
--rw-r--r--   0        0        0      540 2024-03-26 08:05:25.492109 django_bocor_ds-2.3.1/django_bocor_ds/migrations/0002_remove_portfolio_image3_remove_portfolio_image4_and_more.py
--rw-r--r--   0        0        0      502 2024-03-27 02:55:50.933146 django_bocor_ds-2.3.1/django_bocor_ds/migrations/0003_portfolio_redirect_link.py
--rw-r--r--   0        0        0      351 2024-03-27 05:19:19.375307 django_bocor_ds-2.3.1/django_bocor_ds/migrations/0004_remove_portfolio_redirect_link.py
--rw-r--r--   0        0        0        0 2024-03-21 06:07:03.001526 django_bocor_ds-2.3.1/django_bocor_ds/migrations/__init__.py
--rw-r--r--   0        0        0      948 2024-03-27 05:06:04.714022 django_bocor_ds-2.3.1/django_bocor_ds/models.py
--rw-r--r--   0        0        0      309 2024-05-18 20:02:52.214989 django_bocor_ds-2.3.1/django_bocor_ds/sitemaps.py
--rw-r--r--   0        0        0     6148 2024-03-21 08:10:33.959729 django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/.DS_Store
--rwxr-xr-x   0        0        0    24429 2024-04-03 08:25:58.403114 django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/css/style.css
--rwxr-xr-x   0        0        0   249630 2024-03-12 00:49:58.000000 django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/img/footer-bg.jpg
--rwxr-xr-x   0        0        0     5114 2024-03-17 05:37:08.000000 django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/js/main.js
--rwxr-xr-x   0        0        0     2893 2024-03-12 00:49:58.000000 django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/scss/_footer.scss
--rwxr-xr-x   0        0        0     1290 2024-03-12 00:49:58.000000 django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/scss/_general.scss
--rwxr-xr-x   0        0        0      709 2024-03-12 00:49:58.000000 django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/scss/_header.scss
--rwxr-xr-x   0        0        0     1422 2024-03-12 00:49:58.000000 django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/scss/_hero.scss
--rwxr-xr-x   0        0        0     4101 2024-03-12 00:49:58.000000 django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/scss/_nav.scss
--rwxr-xr-x   0        0        0    15555 2024-03-12 00:49:58.000000 django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/scss/_sections.scss
--rwxr-xr-x   0        0        0      454 2024-03-12 00:49:58.000000 django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/scss/_variables.scss
--rwxr-xr-x   0        0        0      136 2024-03-12 00:49:58.000000 django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/scss/style.scss
--rw-r--r--   0        0        0    19941 2024-03-12 00:49:58.000000 django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/aos/aos.cjs.js
--rw-r--r--   0        0        0    28765 2024-03-12 00:49:58.000000 django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/aos/aos.css
--rw-r--r--   0        0        0    19768 2024-03-12 00:49:58.000000 django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/aos/aos.esm.js
--rw-r--r--   0        0        0    13800 2024-03-12 00:49:58.000000 django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/aos/aos.js
--rw-r--r--   0        0        0    56459 2024-03-12 00:49:58.000000 django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/aos/aos.js.map
--rw-r--r--   0        0        0    98255 2024-03-12 00:49:58.000000 django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/bootstrap-icons/bootstrap-icons.css
--rw-r--r--   0        0        0    52358 2024-03-12 00:49:58.000000 django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/bootstrap-icons/bootstrap-icons.json
--rw-r--r--   0        0        0    85875 2024-03-12 00:49:58.000000 django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/bootstrap-icons/bootstrap-icons.min.css
--rw-r--r--   0        0        0    57755 2024-03-12 00:49:58.000000 django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/bootstrap-icons/bootstrap-icons.scss
--rw-r--r--   0        0        0   176032 2024-03-12 00:49:58.000000 django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/bootstrap-icons/fonts/bootstrap-icons.woff
--rw-r--r--   0        0        0   130396 2024-03-12 00:49:58.000000 django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/bootstrap-icons/fonts/bootstrap-icons.woff2
--rw-r--r--   0        0        0    70329 2024-03-12 00:49:58.000000 django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-grid.css
--rw-r--r--   0        0        0   203221 2024-03-12 00:49:58.000000 django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-grid.css.map
--rw-r--r--   0        0        0    51795 2024-03-12 00:49:58.000000 django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-grid.min.css
--rw-r--r--   0        0        0   115986 2024-03-12 00:49:58.000000 django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-grid.min.css.map
--rw-r--r--   0        0        0    70403 2024-03-12 00:49:58.000000 django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-grid.rtl.css
--rw-r--r--   0        0        0   203225 2024-03-12 00:49:58.000000 django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-grid.rtl.css.map
--rw-r--r--   0        0        0    51870 2024-03-12 00:49:58.000000 django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-grid.rtl.min.css
--rw-r--r--   0        0        0   116063 2024-03-12 00:49:58.000000 django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-grid.rtl.min.css.map
--rw-r--r--   0        0        0    12065 2024-03-12 00:49:58.000000 django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-reboot.css
--rw-r--r--   0        0        0   129371 2024-03-12 00:49:58.000000 django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-reboot.css.map
--rw-r--r--   0        0        0    10126 2024-03-12 00:49:58.000000 django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-reboot.min.css
--rw-r--r--   0        0        0    51369 2024-03-12 00:49:58.000000 django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-reboot.min.css.map
--rw-r--r--   0        0        0    12058 2024-03-12 00:49:58.000000 django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-reboot.rtl.css
--rw-r--r--   0        0        0   129386 2024-03-12 00:49:58.000000 django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-reboot.rtl.css.map
--rw-r--r--   0        0        0    10198 2024-03-12 00:49:58.000000 django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css
--rw-r--r--   0        0        0    63943 2024-03-12 00:49:58.000000 django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css.map
--rw-r--r--   0        0        0   107823 2024-03-12 00:49:58.000000 django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-utilities.css
--rw-r--r--   0        0        0   267535 2024-03-12 00:49:58.000000 django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-utilities.css.map
--rw-r--r--   0        0        0    85352 2024-03-12 00:49:58.000000 django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-utilities.min.css
--rw-r--r--   0        0        0   180381 2024-03-12 00:49:58.000000 django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-utilities.min.css.map
--rw-r--r--   0        0        0   107691 2024-03-12 00:49:58.000000 django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-utilities.rtl.css
--rw-r--r--   0        0        0   267476 2024-03-12 00:49:58.000000 django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-utilities.rtl.css.map
--rw-r--r--   0        0        0    85281 2024-03-12 00:49:58.000000 django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css
--rw-r--r--   0        0        0   180217 2024-03-12 00:49:58.000000 django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css.map
--rw-r--r--   0        0        0   281046 2024-03-12 00:49:58.000000 django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap.css
--rw-r--r--   0        0        0   679755 2024-03-12 00:49:58.000000 django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap.css.map
--rw-r--r--   0        0        0   232803 2024-03-12 00:49:58.000000 django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap.min.css
--rw-r--r--   0        0        0   589892 2024-03-12 00:49:58.000000 django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap.min.css.map
--rw-r--r--   0        0        0   280259 2024-03-12 00:49:58.000000 django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap.rtl.css
--rw-r--r--   0        0        0   679615 2024-03-12 00:49:58.000000 django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap.rtl.css.map
--rw-r--r--   0        0        0   232911 2024-03-12 00:49:58.000000 django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap.rtl.min.css
--rw-r--r--   0        0        0   589087 2024-03-12 00:49:58.000000 django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap.rtl.min.css.map
--rw-r--r--   0        0        0   207819 2024-03-12 00:49:58.000000 django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.bundle.js
--rw-r--r--   0        0        0   444579 2024-03-12 00:49:58.000000 django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.bundle.js.map
--rw-r--r--   0        0        0    80721 2024-03-12 00:49:58.000000 django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.bundle.min.js
--rw-r--r--   0        0        0   332090 2024-03-12 00:49:58.000000 django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.bundle.min.js.map
--rw-r--r--   0        0        0   135829 2024-03-12 00:49:58.000000 django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.esm.js
--rw-r--r--   0        0        0   305438 2024-03-12 00:49:58.000000 django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.esm.js.map
--rw-r--r--   0        0        0    73935 2024-03-12 00:49:58.000000 django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.esm.min.js
--rw-r--r--   0        0        0   222455 2024-03-12 00:49:58.000000 django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.esm.min.js.map
--rw-r--r--   0        0        0   145401 2024-03-12 00:49:58.000000 django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.js
--rw-r--r--   0        0        0   306606 2024-03-12 00:49:58.000000 django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.js.map
--rw-r--r--   0        0        0    60635 2024-03-12 00:49:58.000000 django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.min.js
--rw-r--r--   0        0        0   220561 2024-03-12 00:49:58.000000 django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.min.js.map
--rw-r--r--   0        0        0     7522 2024-03-12 00:49:58.000000 django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/boxicons/css/animations.css
--rw-r--r--   0        0        0    94202 2024-03-12 00:49:58.000000 django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/boxicons/css/boxicons.css
--rw-r--r--   0        0        0    68028 2024-03-12 00:49:58.000000 django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/boxicons/css/boxicons.min.css
--rw-r--r--   0        0        0      683 2024-03-12 00:49:58.000000 django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/boxicons/css/transformations.css
--rw-r--r--   0        0        0   405670 2024-03-12 00:49:58.000000 django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/boxicons/fonts/boxicons.eot
--rw-r--r--   0        0        0  1242122 2024-03-12 00:49:58.000000 django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/boxicons/fonts/boxicons.svg
--rw-r--r--   0        0        0   320944 2024-03-12 00:49:58.000000 django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/boxicons/fonts/boxicons.ttf
--rw-r--r--   0        0        0   321020 2024-03-12 00:49:58.000000 django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/boxicons/fonts/boxicons.woff
--rw-r--r--   0        0        0   115680 2024-03-12 00:49:58.000000 django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/boxicons/fonts/boxicons.woff2
--rw-r--r--   0        0        0    17372 2024-03-12 00:49:58.000000 django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/glightbox/css/glightbox.css
--rw-r--r--   0        0        0    13749 2024-03-12 00:49:58.000000 django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/glightbox/css/glightbox.min.css
--rw-r--r--   0        0        0    52561 2024-03-12 00:49:58.000000 django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/glightbox/css/plyr.css
--rw-r--r--   0        0        0    45081 2024-03-12 00:49:58.000000 django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/glightbox/css/plyr.min.css
--rw-r--r--   0        0        0   109391 2024-03-12 00:49:58.000000 django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/glightbox/js/glightbox.js
--rw-r--r--   0        0        0    55880 2024-03-12 00:49:58.000000 django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/glightbox/js/glightbox.min.js
--rw-r--r--   0        0        0    91398 2024-03-12 00:49:58.000000 django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/isotope-layout/isotope.pkgd.js
--rw-r--r--   0        0        0    35445 2024-03-12 00:49:58.000000 django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/isotope-layout/isotope.pkgd.min.js
--rwxr-xr-x   0        0        0   238381 2024-03-12 00:49:58.000000 django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/php-email-form/php-email-form.php
--rwxr-xr-x   0        0        0     2734 2024-03-12 00:49:58.000000 django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/php-email-form/validate.js
--rw-r--r--   0        0        0    18436 2024-03-12 00:49:58.000000 django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/swiper/swiper-bundle.min.css
--rw-r--r--   0        0        0   149147 2024-03-12 00:49:58.000000 django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/swiper/swiper-bundle.min.js
--rw-r--r--   0        0        0   201656 2024-03-12 00:49:58.000000 django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/swiper/swiper-bundle.min.js.map
--rw-r--r--   0        0        0     6148 2024-04-03 00:07:46.476654 django_bocor_ds-2.3.1/django_bocor_ds/templates/.DS_Store
--rwxr-xr-x   0        0        0     6381 2024-03-17 05:37:08.000000 django_bocor_ds-2.3.1/django_bocor_ds/templates/bocords/__inner-page.html
--rw-r--r--   0        0        0     8057 2024-03-26 07:30:05.640370 django_bocor_ds-2.3.1/django_bocor_ds/templates/bocords/__portfolio-details.html
--rw-r--r--   0        0        0     1241 2024-04-26 06:23:47.737266 django_bocor_ds-2.3.1/django_bocor_ds/templates/bocords/_about.html
--rw-r--r--   0        0        0      735 2024-03-25 05:29:33.069856 django_bocor_ds-2.3.1/django_bocor_ds/templates/bocords/_clients.html
--rw-r--r--   0        0        0     3506 2024-04-26 08:21:58.255733 django_bocor_ds-2.3.1/django_bocor_ds/templates/bocords/_contact.html
--rw-r--r--   0        0        0      794 2024-04-26 06:35:37.358645 django_bocor_ds-2.3.1/django_bocor_ds/templates/bocords/_faq.html
--rw-r--r--   0        0        0     1441 2024-04-26 06:22:56.117396 django_bocor_ds-2.3.1/django_bocor_ds/templates/bocords/_features.html
--rw-r--r--   0        0        0      626 2024-04-26 06:25:22.029168 django_bocor_ds-2.3.1/django_bocor_ds/templates/bocords/_hero.html
--rw-r--r--   0        0        0     1553 2024-04-26 06:25:22.020526 django_bocor_ds-2.3.1/django_bocor_ds/templates/bocords/_portfolio.html
--rw-r--r--   0        0        0     1185 2024-04-26 06:35:37.370423 django_bocor_ds-2.3.1/django_bocor_ds/templates/bocords/_pricing.html
--rw-r--r--   0        0        0     1156 2024-04-26 06:25:22.026522 django_bocor_ds-2.3.1/django_bocor_ds/templates/bocords/_services.html
--rw-r--r--   0        0        0     1653 2024-04-26 06:35:37.354165 django_bocor_ds-2.3.1/django_bocor_ds/templates/bocords/_team.html
--rw-r--r--   0        0        0     2404 2024-04-04 04:41:10.261572 django_bocor_ds-2.3.1/django_bocor_ds/templates/bocords/footer.html
--rw-r--r--   0        0        0     1452 2024-04-21 07:23:02.021277 django_bocor_ds-2.3.1/django_bocor_ds/templates/bocords/header.html
--rw-r--r--   0        0        0     3530 2024-05-02 03:31:09.760501 django_bocor_ds-2.3.1/django_bocor_ds/templates/bocords/index.html
--rw-r--r--   0        0        0     1914 2024-04-03 08:20:59.077335 django_bocor_ds-2.3.1/django_bocor_ds/templates/bocords/seo.html
--rw-r--r--   0        0        0        0 2023-03-21 07:32:09.033136 django_bocor_ds-2.3.1/django_bocor_ds/templatetags/__init__.py
--rw-r--r--   0        0        0     5223 2024-03-22 23:51:55.383813 django_bocor_ds-2.3.1/django_bocor_ds/templatetags/bocords_tags.py
--rw-r--r--   0        0        0       60 2024-03-21 06:07:03.001392 django_bocor_ds-2.3.1/django_bocor_ds/tests.py
--rw-r--r--   0        0        0      510 2024-05-18 20:04:17.759467 django_bocor_ds-2.3.1/django_bocor_ds/urls.py
--rw-r--r--   0        0        0     2469 2024-04-03 06:57:03.342404 django_bocor_ds-2.3.1/django_bocor_ds/views.py
--rw-r--r--   0        0        0      814 2024-05-18 20:09:58.274979 django_bocor_ds-2.3.1/pyproject.toml
--rw-r--r--   0        0        0     2464 1970-01-01 00:00:00.000000 django_bocor_ds-2.3.1/PKG-INFO
+-rw-r--r--   0        0        0    10244 2024-05-18 19:53:20.644327 django_bocor_ds-3.0.0/.DS_Store
+-rw-r--r--   0        0        0       66 2024-03-21 05:49:50.372491 django_bocor_ds-3.0.0/.gitattributes
+-rw-r--r--   0        0        0       29 2024-05-18 19:35:21.529731 django_bocor_ds-3.0.0/.gitignore
+-rw-r--r--   0        0        0       52 2024-03-21 06:06:29.551428 django_bocor_ds-3.0.0/.idea/.gitignore
+-rw-r--r--   0        0        0      405 2024-03-21 06:06:29.465715 django_bocor_ds-3.0.0/.idea/django-bocor-ds.iml
+-rw-r--r--   0        0        0      174 2024-03-21 06:06:29.480874 django_bocor_ds-3.0.0/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      421 2024-03-21 06:08:26.611158 django_bocor_ds-3.0.0/.idea/misc.xml
+-rw-r--r--   0        0        0      282 2024-03-21 06:06:29.471790 django_bocor_ds-3.0.0/.idea/modules.xml
+-rw-r--r--   0        0        0      167 2024-03-21 06:06:29.484071 django_bocor_ds-3.0.0/.idea/vcs.xml
+-rw-r--r--   0        0        0     1079 2024-03-19 03:45:10.033383 django_bocor_ds-3.0.0/LICENSE
+-rw-r--r--   0        0        0     1924 2024-05-23 03:25:39.977869 django_bocor_ds-3.0.0/README.md
+-rw-r--r--   0        0        0     6148 2024-04-13 00:02:19.172196 django_bocor_ds-3.0.0/django_bocor_ds/.DS_Store
+-rw-r--r--   0        0        0        0 2024-03-21 06:07:02.999245 django_bocor_ds-3.0.0/django_bocor_ds/__init__.py
+-rw-r--r--   0        0        0      495 2024-03-26 07:24:10.511682 django_bocor_ds-3.0.0/django_bocor_ds/admin.py
+-rw-r--r--   0        0        0      160 2024-03-21 06:07:03.001129 django_bocor_ds-3.0.0/django_bocor_ds/apps.py
+-rw-r--r--   0        0        0      947 2024-03-24 12:14:35.423434 django_bocor_ds-3.0.0/django_bocor_ds/forms.py
+-rw-r--r--   0        0        0     1915 2024-03-26 07:22:15.008801 django_bocor_ds-3.0.0/django_bocor_ds/migrations/0001_initial.py
+-rw-r--r--   0        0        0      540 2024-03-26 08:05:25.492109 django_bocor_ds-3.0.0/django_bocor_ds/migrations/0002_remove_portfolio_image3_remove_portfolio_image4_and_more.py
+-rw-r--r--   0        0        0      502 2024-03-27 02:55:50.933146 django_bocor_ds-3.0.0/django_bocor_ds/migrations/0003_portfolio_redirect_link.py
+-rw-r--r--   0        0        0      351 2024-03-27 05:19:19.375307 django_bocor_ds-3.0.0/django_bocor_ds/migrations/0004_remove_portfolio_redirect_link.py
+-rw-r--r--   0        0        0        0 2024-03-21 06:07:03.001526 django_bocor_ds-3.0.0/django_bocor_ds/migrations/__init__.py
+-rw-r--r--   0        0        0      948 2024-03-27 05:06:04.714022 django_bocor_ds-3.0.0/django_bocor_ds/models.py
+-rw-r--r--   0        0        0      388 2024-05-23 03:42:00.117360 django_bocor_ds-3.0.0/django_bocor_ds/sitemaps.py
+-rw-r--r--   0        0        0     6148 2024-03-21 08:10:33.959729 django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/.DS_Store
+-rwxr-xr-x   0        0        0    24429 2024-04-03 08:25:58.403114 django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/css/style.css
+-rwxr-xr-x   0        0        0   249630 2024-03-12 00:49:58.000000 django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/img/footer-bg.jpg
+-rwxr-xr-x   0        0        0     5114 2024-03-17 05:37:08.000000 django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/js/main.js
+-rwxr-xr-x   0        0        0     2893 2024-03-12 00:49:58.000000 django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/scss/_footer.scss
+-rwxr-xr-x   0        0        0     1290 2024-03-12 00:49:58.000000 django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/scss/_general.scss
+-rwxr-xr-x   0        0        0      709 2024-03-12 00:49:58.000000 django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/scss/_header.scss
+-rwxr-xr-x   0        0        0     1422 2024-03-12 00:49:58.000000 django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/scss/_hero.scss
+-rwxr-xr-x   0        0        0     4101 2024-03-12 00:49:58.000000 django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/scss/_nav.scss
+-rwxr-xr-x   0        0        0    15555 2024-03-12 00:49:58.000000 django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/scss/_sections.scss
+-rwxr-xr-x   0        0        0      454 2024-03-12 00:49:58.000000 django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/scss/_variables.scss
+-rwxr-xr-x   0        0        0      136 2024-03-12 00:49:58.000000 django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/scss/style.scss
+-rw-r--r--   0        0        0    19941 2024-03-12 00:49:58.000000 django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/aos/aos.cjs.js
+-rw-r--r--   0        0        0    28765 2024-03-12 00:49:58.000000 django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/aos/aos.css
+-rw-r--r--   0        0        0    19768 2024-03-12 00:49:58.000000 django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/aos/aos.esm.js
+-rw-r--r--   0        0        0    13800 2024-03-12 00:49:58.000000 django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/aos/aos.js
+-rw-r--r--   0        0        0    56459 2024-03-12 00:49:58.000000 django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/aos/aos.js.map
+-rw-r--r--   0        0        0    98255 2024-03-12 00:49:58.000000 django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/bootstrap-icons/bootstrap-icons.css
+-rw-r--r--   0        0        0    52358 2024-03-12 00:49:58.000000 django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/bootstrap-icons/bootstrap-icons.json
+-rw-r--r--   0        0        0    85875 2024-03-12 00:49:58.000000 django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/bootstrap-icons/bootstrap-icons.min.css
+-rw-r--r--   0        0        0    57755 2024-03-12 00:49:58.000000 django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/bootstrap-icons/bootstrap-icons.scss
+-rw-r--r--   0        0        0   176032 2024-03-12 00:49:58.000000 django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/bootstrap-icons/fonts/bootstrap-icons.woff
+-rw-r--r--   0        0        0   130396 2024-03-12 00:49:58.000000 django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/bootstrap-icons/fonts/bootstrap-icons.woff2
+-rw-r--r--   0        0        0    70329 2024-03-12 00:49:58.000000 django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-grid.css
+-rw-r--r--   0        0        0   203221 2024-03-12 00:49:58.000000 django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-grid.css.map
+-rw-r--r--   0        0        0    51795 2024-03-12 00:49:58.000000 django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-grid.min.css
+-rw-r--r--   0        0        0   115986 2024-03-12 00:49:58.000000 django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-grid.min.css.map
+-rw-r--r--   0        0        0    70403 2024-03-12 00:49:58.000000 django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-grid.rtl.css
+-rw-r--r--   0        0        0   203225 2024-03-12 00:49:58.000000 django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-grid.rtl.css.map
+-rw-r--r--   0        0        0    51870 2024-03-12 00:49:58.000000 django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-grid.rtl.min.css
+-rw-r--r--   0        0        0   116063 2024-03-12 00:49:58.000000 django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-grid.rtl.min.css.map
+-rw-r--r--   0        0        0    12065 2024-03-12 00:49:58.000000 django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-reboot.css
+-rw-r--r--   0        0        0   129371 2024-03-12 00:49:58.000000 django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-reboot.css.map
+-rw-r--r--   0        0        0    10126 2024-03-12 00:49:58.000000 django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-reboot.min.css
+-rw-r--r--   0        0        0    51369 2024-03-12 00:49:58.000000 django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-reboot.min.css.map
+-rw-r--r--   0        0        0    12058 2024-03-12 00:49:58.000000 django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-reboot.rtl.css
+-rw-r--r--   0        0        0   129386 2024-03-12 00:49:58.000000 django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-reboot.rtl.css.map
+-rw-r--r--   0        0        0    10198 2024-03-12 00:49:58.000000 django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css
+-rw-r--r--   0        0        0    63943 2024-03-12 00:49:58.000000 django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css.map
+-rw-r--r--   0        0        0   107823 2024-03-12 00:49:58.000000 django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-utilities.css
+-rw-r--r--   0        0        0   267535 2024-03-12 00:49:58.000000 django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-utilities.css.map
+-rw-r--r--   0        0        0    85352 2024-03-12 00:49:58.000000 django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-utilities.min.css
+-rw-r--r--   0        0        0   180381 2024-03-12 00:49:58.000000 django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-utilities.min.css.map
+-rw-r--r--   0        0        0   107691 2024-03-12 00:49:58.000000 django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-utilities.rtl.css
+-rw-r--r--   0        0        0   267476 2024-03-12 00:49:58.000000 django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-utilities.rtl.css.map
+-rw-r--r--   0        0        0    85281 2024-03-12 00:49:58.000000 django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css
+-rw-r--r--   0        0        0   180217 2024-03-12 00:49:58.000000 django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css.map
+-rw-r--r--   0        0        0   281046 2024-03-12 00:49:58.000000 django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap.css
+-rw-r--r--   0        0        0   679755 2024-03-12 00:49:58.000000 django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap.css.map
+-rw-r--r--   0        0        0   232803 2024-03-12 00:49:58.000000 django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap.min.css
+-rw-r--r--   0        0        0   589892 2024-03-12 00:49:58.000000 django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap.min.css.map
+-rw-r--r--   0        0        0   280259 2024-03-12 00:49:58.000000 django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap.rtl.css
+-rw-r--r--   0        0        0   679615 2024-03-12 00:49:58.000000 django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap.rtl.css.map
+-rw-r--r--   0        0        0   232911 2024-03-12 00:49:58.000000 django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap.rtl.min.css
+-rw-r--r--   0        0        0   589087 2024-03-12 00:49:58.000000 django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap.rtl.min.css.map
+-rw-r--r--   0        0        0   207819 2024-03-12 00:49:58.000000 django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.bundle.js
+-rw-r--r--   0        0        0   444579 2024-03-12 00:49:58.000000 django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.bundle.js.map
+-rw-r--r--   0        0        0    80721 2024-03-12 00:49:58.000000 django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.bundle.min.js
+-rw-r--r--   0        0        0   332090 2024-03-12 00:49:58.000000 django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.bundle.min.js.map
+-rw-r--r--   0        0        0   135829 2024-03-12 00:49:58.000000 django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.esm.js
+-rw-r--r--   0        0        0   305438 2024-03-12 00:49:58.000000 django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.esm.js.map
+-rw-r--r--   0        0        0    73935 2024-03-12 00:49:58.000000 django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.esm.min.js
+-rw-r--r--   0        0        0   222455 2024-03-12 00:49:58.000000 django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.esm.min.js.map
+-rw-r--r--   0        0        0   145401 2024-03-12 00:49:58.000000 django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.js
+-rw-r--r--   0        0        0   306606 2024-03-12 00:49:58.000000 django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.js.map
+-rw-r--r--   0        0        0    60635 2024-03-12 00:49:58.000000 django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.min.js
+-rw-r--r--   0        0        0   220561 2024-03-12 00:49:58.000000 django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.min.js.map
+-rw-r--r--   0        0        0     7522 2024-03-12 00:49:58.000000 django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/boxicons/css/animations.css
+-rw-r--r--   0        0        0    94202 2024-03-12 00:49:58.000000 django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/boxicons/css/boxicons.css
+-rw-r--r--   0        0        0    68028 2024-03-12 00:49:58.000000 django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/boxicons/css/boxicons.min.css
+-rw-r--r--   0        0        0      683 2024-03-12 00:49:58.000000 django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/boxicons/css/transformations.css
+-rw-r--r--   0        0        0   405670 2024-03-12 00:49:58.000000 django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/boxicons/fonts/boxicons.eot
+-rw-r--r--   0        0        0  1242122 2024-03-12 00:49:58.000000 django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/boxicons/fonts/boxicons.svg
+-rw-r--r--   0        0        0   320944 2024-03-12 00:49:58.000000 django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/boxicons/fonts/boxicons.ttf
+-rw-r--r--   0        0        0   321020 2024-03-12 00:49:58.000000 django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/boxicons/fonts/boxicons.woff
+-rw-r--r--   0        0        0   115680 2024-03-12 00:49:58.000000 django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/boxicons/fonts/boxicons.woff2
+-rw-r--r--   0        0        0    17372 2024-03-12 00:49:58.000000 django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/glightbox/css/glightbox.css
+-rw-r--r--   0        0        0    13749 2024-03-12 00:49:58.000000 django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/glightbox/css/glightbox.min.css
+-rw-r--r--   0        0        0    52561 2024-03-12 00:49:58.000000 django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/glightbox/css/plyr.css
+-rw-r--r--   0        0        0    45081 2024-03-12 00:49:58.000000 django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/glightbox/css/plyr.min.css
+-rw-r--r--   0        0        0   109391 2024-03-12 00:49:58.000000 django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/glightbox/js/glightbox.js
+-rw-r--r--   0        0        0    55880 2024-03-12 00:49:58.000000 django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/glightbox/js/glightbox.min.js
+-rw-r--r--   0        0        0    91398 2024-03-12 00:49:58.000000 django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/isotope-layout/isotope.pkgd.js
+-rw-r--r--   0        0        0    35445 2024-03-12 00:49:58.000000 django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/isotope-layout/isotope.pkgd.min.js
+-rwxr-xr-x   0        0        0   238381 2024-03-12 00:49:58.000000 django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/php-email-form/php-email-form.php
+-rwxr-xr-x   0        0        0     2734 2024-03-12 00:49:58.000000 django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/php-email-form/validate.js
+-rw-r--r--   0        0        0    18436 2024-03-12 00:49:58.000000 django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/swiper/swiper-bundle.min.css
+-rw-r--r--   0        0        0   149147 2024-03-12 00:49:58.000000 django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/swiper/swiper-bundle.min.js
+-rw-r--r--   0        0        0   201656 2024-03-12 00:49:58.000000 django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/swiper/swiper-bundle.min.js.map
+-rw-r--r--   0        0        0     6148 2024-04-03 00:07:46.476654 django_bocor_ds-3.0.0/django_bocor_ds/templates/.DS_Store
+-rwxr-xr-x   0        0        0     6381 2024-03-17 05:37:08.000000 django_bocor_ds-3.0.0/django_bocor_ds/templates/bocords/__inner-page.html
+-rw-r--r--   0        0        0     8057 2024-03-26 07:30:05.640370 django_bocor_ds-3.0.0/django_bocor_ds/templates/bocords/__portfolio-details.html
+-rw-r--r--   0        0        0     1259 2024-05-23 03:47:21.479468 django_bocor_ds-3.0.0/django_bocor_ds/templates/bocords/_about.html
+-rw-r--r--   0        0        0      771 2024-05-23 03:47:21.489312 django_bocor_ds-3.0.0/django_bocor_ds/templates/bocords/_clients.html
+-rw-r--r--   0        0        0     3517 2024-05-23 03:47:21.464622 django_bocor_ds-3.0.0/django_bocor_ds/templates/bocords/_contact.html
+-rw-r--r--   0        0        0      794 2024-04-26 06:35:37.358645 django_bocor_ds-3.0.0/django_bocor_ds/templates/bocords/_faq.html
+-rw-r--r--   0        0        0     1459 2024-05-23 03:47:21.487414 django_bocor_ds-3.0.0/django_bocor_ds/templates/bocords/_features.html
+-rw-r--r--   0        0        0      644 2024-05-23 03:47:21.485719 django_bocor_ds-3.0.0/django_bocor_ds/templates/bocords/_hero.html
+-rw-r--r--   0        0        0     1564 2024-05-23 03:47:21.483530 django_bocor_ds-3.0.0/django_bocor_ds/templates/bocords/_portfolio.html
+-rw-r--r--   0        0        0     1185 2024-04-26 06:35:37.370423 django_bocor_ds-3.0.0/django_bocor_ds/templates/bocords/_pricing.html
+-rw-r--r--   0        0        0     1174 2024-05-23 03:47:21.481503 django_bocor_ds-3.0.0/django_bocor_ds/templates/bocords/_services.html
+-rw-r--r--   0        0        0     1671 2024-05-23 03:44:16.688221 django_bocor_ds-3.0.0/django_bocor_ds/templates/bocords/_team.html
+-rw-r--r--   0        0        0     2415 2024-05-23 03:44:16.684177 django_bocor_ds-3.0.0/django_bocor_ds/templates/bocords/footer.html
+-rw-r--r--   0        0        0     1503 2024-05-23 03:44:16.694688 django_bocor_ds-3.0.0/django_bocor_ds/templates/bocords/header.html
+-rw-r--r--   0        0        0     3461 2024-05-23 03:42:00.114144 django_bocor_ds-3.0.0/django_bocor_ds/templates/bocords/index.html
+-rw-r--r--   0        0        0     1986 2024-05-23 03:44:16.691635 django_bocor_ds-3.0.0/django_bocor_ds/templates/bocords/seo.html
+-rw-r--r--   0        0        0        0 2023-03-21 07:32:09.033136 django_bocor_ds-3.0.0/django_bocor_ds/templatetags/__init__.py
+-rw-r--r--   0        0        0     6833 2024-05-23 03:42:00.095323 django_bocor_ds-3.0.0/django_bocor_ds/templatetags/bocords_tags.py
+-rw-r--r--   0        0        0       60 2024-03-21 06:07:03.001392 django_bocor_ds-3.0.0/django_bocor_ds/tests.py
+-rw-r--r--   0        0        0      559 2024-05-23 03:25:40.054748 django_bocor_ds-3.0.0/django_bocor_ds/urls.py
+-rw-r--r--   0        0        0     2534 2024-05-23 03:25:39.970776 django_bocor_ds-3.0.0/django_bocor_ds/views.py
+-rw-r--r--   0        0        0      814 2024-05-23 03:25:39.975560 django_bocor_ds-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2464 1970-01-01 00:00:00.000000 django_bocor_ds-3.0.0/PKG-INFO
```

### Comparing `django_bocor_ds-2.3.1/.DS_Store` & `django_bocor_ds-3.0.0/.DS_Store`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.3.1/LICENSE` & `django_bocor_ds-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.3.1/README.md` & `django_bocor_ds-3.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #### Requirements
 
 Django >= 4.2.11
 libsass>=0.23.0
 django-analyticsds >= 0.3.1
 django-calendards >= 0.4.0
 django-modalds >= 0.1.0
-django-utilsds >= 0.4.0
+django-utilsds >= 0.6.0
 django-light >= 0.1.0   # 밝은 admin 화면
 
 ---
 #### Install
 
 settings.py  
 ```
```

### Comparing `django_bocor_ds-2.3.1/django_bocor_ds/.DS_Store` & `django_bocor_ds-3.0.0/django_bocor_ds/.DS_Store`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.3.1/django_bocor_ds/forms.py` & `django_bocor_ds-3.0.0/django_bocor_ds/forms.py`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.3.1/django_bocor_ds/migrations/0001_initial.py` & `django_bocor_ds-3.0.0/django_bocor_ds/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.3.1/django_bocor_ds/migrations/0002_remove_portfolio_image3_remove_portfolio_image4_and_more.py` & `django_bocor_ds-3.0.0/django_bocor_ds/migrations/0002_remove_portfolio_image3_remove_portfolio_image4_and_more.py`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.3.1/django_bocor_ds/models.py` & `django_bocor_ds-3.0.0/django_bocor_ds/models.py`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/.DS_Store` & `django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/.DS_Store`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/css/style.css` & `django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/css/style.css`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/img/footer-bg.jpg` & `django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/img/footer-bg.jpg`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/js/main.js` & `django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/js/main.js`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/scss/_footer.scss` & `django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/scss/_footer.scss`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/scss/_general.scss` & `django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/scss/_general.scss`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/scss/_header.scss` & `django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/scss/_header.scss`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/scss/_hero.scss` & `django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/scss/_hero.scss`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/scss/_nav.scss` & `django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/scss/_nav.scss`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/scss/_sections.scss` & `django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/scss/_sections.scss`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/aos/aos.cjs.js` & `django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/aos/aos.cjs.js`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/aos/aos.css` & `django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/aos/aos.css`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/aos/aos.esm.js` & `django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/aos/aos.esm.js`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/aos/aos.js` & `django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/aos/aos.js`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/aos/aos.js.map` & `django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/aos/aos.js.map`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/bootstrap-icons/bootstrap-icons.css` & `django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/bootstrap-icons/bootstrap-icons.css`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/bootstrap-icons/bootstrap-icons.json` & `django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/bootstrap-icons/bootstrap-icons.json`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/bootstrap-icons/bootstrap-icons.min.css` & `django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/bootstrap-icons/bootstrap-icons.min.css`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/bootstrap-icons/bootstrap-icons.scss` & `django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/bootstrap-icons/bootstrap-icons.scss`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/bootstrap-icons/fonts/bootstrap-icons.woff` & `django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/bootstrap-icons/fonts/bootstrap-icons.woff`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/bootstrap-icons/fonts/bootstrap-icons.woff2` & `django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/bootstrap-icons/fonts/bootstrap-icons.woff2`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-grid.css` & `django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-grid.css`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-grid.css.map` & `django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-grid.css.map`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-grid.min.css` & `django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-grid.min.css`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-grid.min.css.map` & `django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-grid.min.css.map`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-grid.rtl.css` & `django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-grid.rtl.css`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-grid.rtl.css.map` & `django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-grid.rtl.css.map`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-grid.rtl.min.css` & `django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-grid.rtl.min.css`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-grid.rtl.min.css.map` & `django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-grid.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-reboot.css` & `django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-reboot.css`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-reboot.css.map` & `django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-reboot.css.map`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-reboot.min.css` & `django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-reboot.min.css`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-reboot.min.css.map` & `django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-reboot.min.css.map`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-reboot.rtl.css` & `django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-reboot.rtl.css`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-reboot.rtl.css.map` & `django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-reboot.rtl.css.map`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css` & `django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css.map` & `django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-utilities.css` & `django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-utilities.css`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-utilities.css.map` & `django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-utilities.css.map`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-utilities.min.css` & `django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-utilities.min.css`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-utilities.min.css.map` & `django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-utilities.min.css.map`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-utilities.rtl.css` & `django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-utilities.rtl.css`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-utilities.rtl.css.map` & `django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-utilities.rtl.css.map`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css` & `django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css.map` & `django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap.css` & `django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap.css.map` & `django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap.min.css` & `django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap.min.css.map` & `django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap.rtl.css` & `django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap.rtl.css`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap.rtl.css.map` & `django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap.rtl.css.map`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap.rtl.min.css` & `django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap.rtl.min.css`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap.rtl.min.css.map` & `django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/bootstrap/css/bootstrap.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.bundle.js` & `django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.bundle.js`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.bundle.js.map` & `django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.bundle.js.map`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.bundle.min.js` & `django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.bundle.min.js.map` & `django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.esm.js` & `django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.esm.js`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.esm.js.map` & `django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.esm.js.map`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.esm.min.js` & `django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.esm.min.js`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.esm.min.js.map` & `django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.esm.min.js.map`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.js` & `django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.js.map` & `django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.js.map`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.min.js` & `django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.min.js.map` & `django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/bootstrap/js/bootstrap.min.js.map`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/boxicons/css/animations.css` & `django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/boxicons/css/animations.css`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/boxicons/css/boxicons.css` & `django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/boxicons/css/boxicons.css`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/boxicons/css/boxicons.min.css` & `django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/boxicons/css/boxicons.min.css`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/boxicons/css/transformations.css` & `django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/boxicons/css/transformations.css`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/boxicons/fonts/boxicons.eot` & `django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/boxicons/fonts/boxicons.eot`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/boxicons/fonts/boxicons.svg` & `django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/boxicons/fonts/boxicons.svg`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/boxicons/fonts/boxicons.ttf` & `django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/boxicons/fonts/boxicons.ttf`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/boxicons/fonts/boxicons.woff` & `django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/boxicons/fonts/boxicons.woff`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/boxicons/fonts/boxicons.woff2` & `django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/boxicons/fonts/boxicons.woff2`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/glightbox/css/glightbox.css` & `django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/glightbox/css/glightbox.css`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/glightbox/css/glightbox.min.css` & `django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/glightbox/css/glightbox.min.css`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/glightbox/css/plyr.css` & `django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/glightbox/css/plyr.css`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/glightbox/css/plyr.min.css` & `django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/glightbox/css/plyr.min.css`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/glightbox/js/glightbox.js` & `django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/glightbox/js/glightbox.js`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/glightbox/js/glightbox.min.js` & `django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/glightbox/js/glightbox.min.js`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/isotope-layout/isotope.pkgd.js` & `django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/isotope-layout/isotope.pkgd.js`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/isotope-layout/isotope.pkgd.min.js` & `django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/isotope-layout/isotope.pkgd.min.js`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/php-email-form/php-email-form.php` & `django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/php-email-form/php-email-form.php`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/php-email-form/validate.js` & `django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/php-email-form/validate.js`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/swiper/swiper-bundle.min.css` & `django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/swiper/swiper-bundle.min.css`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/swiper/swiper-bundle.min.js` & `django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/swiper/swiper-bundle.min.js`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.3.1/django_bocor_ds/static/bocords/vendor/swiper/swiper-bundle.min.js.map` & `django_bocor_ds-3.0.0/django_bocor_ds/static/bocords/vendor/swiper/swiper-bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.3.1/django_bocor_ds/templates/.DS_Store` & `django_bocor_ds-3.0.0/django_bocor_ds/templates/.DS_Store`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.3.1/django_bocor_ds/templates/bocords/__inner-page.html` & `django_bocor_ds-3.0.0/django_bocor_ds/templates/bocords/__inner-page.html`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.3.1/django_bocor_ds/templates/bocords/__portfolio-details.html` & `django_bocor_ds-3.0.0/django_bocor_ds/templates/bocords/__portfolio-details.html`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.3.1/django_bocor_ds/templates/bocords/_about.html` & `django_bocor_ds-3.0.0/django_bocor_ds/templates/bocords/_about.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 {% load static %}
 
 <style>
   .about .image {
-    background: url("{% static 'img/bocords/about.jpg' %}") center center no-repeat;
+    background: url("{% static 'img/'|add:template_name|add:'/about.jpg' %}") center center no-repeat;
     background-size: cover;
     min-height: 400px;
   }
 </style>
 
 <section id="about" class="about section-bg">
   <div class="container">
```

### Comparing `django_bocor_ds-2.3.1/django_bocor_ds/templates/bocords/_contact.html` & `django_bocor_ds-3.0.0/django_bocor_ds/templates/bocords/_contact.html`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
               {% endif %}
             </div>
 
           </div>
 
           <div class="col-lg-6 mt-4 mt-lg-0">
             <!-- url 태그 안에 앵커 이동 가능하다 -->
-            <form action="{% url 'bocords:home' %}#contact" method="POST" role="form" class="php-email-form  w-100" data-aos="fade-up">
+            <form action="{% url template_name|add:':home' %}#contact" method="POST" role="form" class="php-email-form  w-100" data-aos="fade-up">
               {% csrf_token %}
               <div class="row">
                 <div class="col-md-6 form-group">
                   {{ form.name }}
                 </div>
                 <div class="col-md-6 form-group mt-3 mt-md-0">
                   {{ form.email }}
```

### Comparing `django_bocor_ds-2.3.1/django_bocor_ds/templates/bocords/_faq.html` & `django_bocor_ds-3.0.0/django_bocor_ds/templates/bocords/_faq.html`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.3.1/django_bocor_ds/templates/bocords/_features.html` & `django_bocor_ds-3.0.0/django_bocor_ds/templates/bocords/_features.html`

 * *Files 9% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     <div class="row content">
       <!-- 홀수 짝수 구분 -->
       {% if forloop.counter|divisibleby:2 %}
       <div class="col-md-5 order-1 order-md-2" data-aos="fade-left">
       {% else %}
       <div class="col-md-5" data-aos="fade-right">
       {% endif %}
-        <img src="{% static 'img/bocords/features/'|add:item.photo %}" class="img-fluid" alt="">
+        <img src="{% static 'img/'|add:template_name|add:'/features/'|add:item.photo %}" class="img-fluid" alt="">
       </div>
       <!-- 홀수 짝수 구분 -->
       {% if forloop.counter|divisibleby:2 %}
       <div class="col-md-7 pt-5 order-2 order-md-1" data-aos="fade-right">
       {% else %}
       <div class="col-md-7 pt-4" data-aos="fade-left">
       {% endif %}
```

### Comparing `django_bocor_ds-2.3.1/django_bocor_ds/templates/bocords/_hero.html` & `django_bocor_ds-3.0.0/django_bocor_ds/templates/bocords/_hero.html`

 * *Files 17% similar despite different names*

```diff
@@ -8,13 +8,13 @@
       {% autoescape off %}
       <h1>{{ hero.h1 | safe }}</h1>
       <h2>{{ hero.h2 | safe }}</h2>
       {% endautoescape %}
       <a href="{{ hero.btn.link }}" class="btn-get-started scrollto">{{ hero.btn.title }}</a>
     </div>
     <div class="col-lg-6 order-1 order-lg-2 hero-img" data-aos="fade-left">
-      <img src="{% static 'img/bocords/'|add:hero.bg %}" class="img-fluid" alt="">
+      <img src="{% static 'img/'|add:template_name|add:'/'|add:hero.bg %}" class="img-fluid" alt="">
     </div>
   </div>
   </div>
 
 </section>
```

### Comparing `django_bocor_ds-2.3.1/django_bocor_ds/templates/bocords/_portfolio.html` & `django_bocor_ds-3.0.0/django_bocor_ds/templates/bocords/_portfolio.html`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         <div class="row portfolio-container" data-aos="fade-up">
           {% for item in items.all %}
           <div class="col-lg-4 col-md-6 portfolio-item filter-{{ item.filter }}">
             <div class="portfolio-wrap">
               <img src="{{ item.image1.url }}" class="img-fluid" alt="">
               <div class="portfolio-links">
                 <a href="{{ item.image1.url }}" data-gallery="portfolioGallery" class="portfolio-lightbox" title="{{ item.title }}"><i class="bi bi-plus"></i></a>
-                <a href="{% url 'bocords:details' item.id %}" title="More Details" target="_blank"><i class="bi bi-link"></i></a>
+                <a href="{% url template_name|add:':details' item.id %}" title="More Details" target="_blank"><i class="bi bi-link"></i></a>
               </div>
               <div class="portfolio-info">
                 <h4>{{ item.title }}</h4>
                 <p>{{ item.subtitle }}</p>
               </div>
             </div>
           </div>
```

### Comparing `django_bocor_ds-2.3.1/django_bocor_ds/templates/bocords/_pricing.html` & `django_bocor_ds-3.0.0/django_bocor_ds/templates/bocords/_pricing.html`

 * *Files identical despite different names*

### Comparing `django_bocor_ds-2.3.1/django_bocor_ds/templates/bocords/_services.html` & `django_bocor_ds-3.0.0/django_bocor_ds/templates/bocords/_services.html`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,15 @@
       {% if forloop.counter|divisibleby:2 %}
       <div class="col-md-6 d-flex" data-aos="fade-left">
       {% else %}
       <div class="col-md-6 d-flex" data-aos="fade-right">
       {% endif %}
         <div class="card">
           <div class="card-img">
-            <img src="{% static 'img/bocords/services/'|add:item.image %}" alt="...">
+            <img src="{% static 'img/'|add:template_name|add:'/services/'|add:item.image %}" alt="...">
           </div>
           <div class="card-body">
             <h5 class="card-title"><a href="">{{ item.title }}</a></h5>
             <p class="card-text">{{ item.desc | safe }}</p>
             {% if item.link %}
             <div class="read-more"><a href="{{ item.link }}" target="_blank"><i class="bi bi-arrow-right"></i> Read More</a></div>
             {% endif %}
```

### Comparing `django_bocor_ds-2.3.1/django_bocor_ds/templates/bocords/_team.html` & `django_bocor_ds-3.0.0/django_bocor_ds/templates/bocords/_team.html`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,15 @@
         {% if forloop.first %}
         <div class="member" data-aos="fade-up">
         {% else %}
         <div class="member" data-aos="fade-up" data-aos-delay="{% cycle '100' '200' '300' '400' %}">
         {% endif %}
           <div class="member" data-aos="fade-up">
           {% cycle 'member1' 'member2' 'member3' 'member4' 'member5' 'member6' as member_dir silent %}
-          <div class="pic"><img src="{% static 'img/bocords/team/'|add:member_dir|add:'/profile.jpg' %}" alt=""></div>
+          <div class="pic"><img src="{% static 'img/'|add:template_name|add:'/team/'|add:member_dir|add:'/profile.jpg' %}" alt=""></div>
           <h4>{{ member.name }}</h4>
           <span>{{ member.title }}</span>
           <div class="social">
             {% if member.social.twitter %}
             <a href="{{ member.social.twitter }}"><i class="bi bi-twitter"></i></a>
             {% endif %}
             {% if member.social.facebook %}
```

### Comparing `django_bocor_ds-2.3.1/django_bocor_ds/templates/bocords/footer.html` & `django_bocor_ds-3.0.0/django_bocor_ds/templates/bocords/footer.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 {% load static %}
 
 <style>
 #footer {
-  background: url("{% static 'bocords/img/footer-bg.jpg' %}") center center no-repeat;
+  background: url("{% static template_name|add:'/img/footer-bg.jpg' %}") center center no-repeat;
   color: #fff;
   font-size: 14px;
   position: relative;
 }
 </style>
 
 <footer id="footer">
```

### Comparing `django_bocor_ds-2.3.1/django_bocor_ds/templates/bocords/header.html` & `django_bocor_ds-3.0.0/django_bocor_ds/templates/bocords/header.html`

 * *Files 13% similar despite different names*

```diff
@@ -3,30 +3,30 @@
 
 <header id="header">
   <div class="container d-flex align-items-center justify-content-between">
 
     <!-- 로고 -->
     <div class="logo">
       {% if use_logo %}
-      <a href="{% url 'bocords:home' %}"><img src="{% static 'img/bocords/logo.png' %}" alt="" class="img-fluid"></a>
+      <a href="{% url template_name|add:':home' %}"><img src="{% static 'img/'|add:template_name|add:'/logo.png' %}" alt="" class="img-fluid"></a>
       {% else %}
-      <h1><a href="{% url 'bocords:home' %}">{{ logo_text }}<span>.</span></a></h1>
+      <h1><a href="{% url template_name|add:':home' %}">{{ logo_text }}<span>.</span></a></h1>
       {% endif %}
     </div>
 
     <nav id="navbar" class="navbar">
       <ul>
         <li><a class="nav-link scrollto active" href="#hero">Home</a></li>
         <!-- 메뉴 -->
         {% for component, etc, title, is_show in components %}
           {% if is_show %}
             {% if component == 'direct_link' %}
               <li><a class="nav-link scrollto" href="{{ etc }}" target="_blank">{{ title }}</a></li>
             {% else %}
-              <li><a class="nav-link scrollto" href="{% url 'bocords:home' %}#{{ component | underscore_to_hyphen }}">{{ title }}</a></li>
+              <li><a class="nav-link scrollto" href="{% url template_name|add:':home' %}#{{ component | underscore_to_hyphen }}">{{ title }}</a></li>
             {% endif %}
           {% endif %}
         {% endfor %}
 
         {% for component, is_use, _, _ in components %}
         {% if component == menu_btn.component and is_use %}
         <li><a class="getstarted scrollto" href="#{{ menu_btn.component }}">{{ menu_btn.title }}</a></li>
```

### Comparing `django_bocor_ds-2.3.1/django_bocor_ds/templates/bocords/index.html` & `django_bocor_ds-3.0.0/django_bocor_ds/templates/bocords/index.html`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 {% load django_modalds_tags %}
 {% load django_analyticsds_tags %}
 
 <!DOCTYPE html>
 <html lang="en">
 
 <head>
-  <!-- ======= SEO ======= -->{% include 'bocords/seo.html' %}<!-- End SEO -->
+  <!-- ======= SEO ======= -->{% seo %}<!-- End SEO -->
 
   <!-- Vendor CSS Files -->
   <link rel="stylesheet"
         href="{% static 'bocords/vendor/bootstrap/css/bootstrap.min.css' %}" crossorigin="anonymous">
   <link rel="stylesheet" href="{% static 'bocords/vendor/bootstrap-icons/bootstrap-icons.min.css' %}">
   <link href="{% static 'bocords/vendor/aos/aos.css' %}" rel="stylesheet">
   <link href="{% static 'bocords/vendor/boxicons/css/boxicons.min.css' %}" rel="stylesheet">
@@ -22,15 +22,15 @@
   <!-- Template Main CSS File -->
   <link href="{% static 'bocords/css/style.css' %}" rel="stylesheet">
 
 </head>
 
 <body>
 
-  <!-- ======= Header ======= -->{% include 'bocords/header.html' %}<!-- End Header -->
+  <!-- ======= Header ======= -->{% header %}<!-- End Header -->
 
   <!-- ======= Hero Section ======= -->{% hero %}<!-- End Hero -->
 
   <main id="main">
     {% show_calendar %}
     {% show_modal %}
     {% make_analytics %}
@@ -56,15 +56,15 @@
         {% elif component == 'contact' %}
           <!-- ======= Contact Section ======= -->{% contact %}<!-- End Contact Section -->
         {% endif %}
       {% endif %}
     {% endfor %}
   </main><!-- End #main -->
 
-  <!-- ======= Footer ======= -->{% include 'bocords/footer.html' %}<!-- End Footer -->
+  <!-- ======= Footer ======= -->{% footer %}<!-- End Footer -->
 
   <a href="#" class="back-to-top d-flex align-items-center justify-content-center"><i class="bi bi-arrow-up-short"></i></a>
 
   <!-- Vendor JS Files -->
   <script src="{% static 'bocords/vendor/bootstrap/js/bootstrap.bundle.min.js' %}"
           crossorigin="anonymous"></script>
   <script src="{% static 'bocords/vendor/aos/aos.js' %}"></script>
```

#### html2text {}

```diff
@@ -1,12 +1,11 @@
 {% load static %} {% load bocords_tags %} {% load django_calendards_tags %} {%
 load django_modalds_tags %} {% load django_analyticsds_tags %}
-{% include 'bocords/seo.html' %}
-{% include 'bocords/header.html' %} {% hero %} {% show_calendar %} {%
-show_modal %} {% make_analytics %} {% for component, is_use, _, _ in components
-%} {% if is_use %} {% if component == 'clients' %} {% clients %} {% elif
-component == 'about' %} {% about %} {% elif component == 'services' %} {%
-services %} {% elif component == 'features' %} {% features %} {% elif component
-== 'portfolio' %} {% portfolio %} {% elif component == 'team' %} {% team %} {%
-elif component == 'pricing' %} {% pricing %} {% elif component == 'faq' %} {%
-faq %} {% elif component == 'contact' %} {% contact %} {% endif %} {% endif %}
-{% endfor %} {% include 'bocords/footer.html' %}
+{% seo %}
+{% header %} {% hero %} {% show_calendar %} {% show_modal %} {% make_analytics
+%} {% for component, is_use, _, _ in components %} {% if is_use %} {% if
+component == 'clients' %} {% clients %} {% elif component == 'about' %} {%
+about %} {% elif component == 'services' %} {% services %} {% elif component ==
+'features' %} {% features %} {% elif component == 'portfolio' %} {% portfolio
+%} {% elif component == 'team' %} {% team %} {% elif component == 'pricing' %}
+{% pricing %} {% elif component == 'faq' %} {% faq %} {% elif component ==
+'contact' %} {% contact %} {% endif %} {% endif %} {% endfor %} {% footer %}
```

### Comparing `django_bocor_ds-2.3.1/django_bocor_ds/views.py` & `django_bocor_ds-3.0.0/django_bocor_ds/views.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,42 @@
 from django.shortcuts import render, get_object_or_404, redirect
 from django_utilsds import utils
 from .forms import AppointmentForm
 from _data import bocords
+
 from .models import Portfolio
 
 import logging
 logger = logging.getLogger(__name__)
 formatter = logging.Formatter('%(levelname)s: [%(name)s] %(message)s')
 ch = logging.StreamHandler()
 ch.setFormatter(formatter)
 logger.addHandler(ch)
 logger.setLevel(logging.ERROR)
 
 
+template_name = bocords.context['template_name']
+c = bocords.context
+
+
 def robots(request):
     from django.shortcuts import HttpResponse
     file_content = utils.make_robots()
     return HttpResponse(file_content, content_type="text/plain")
 
 
 def home(request):
-    c = bocords.context
-
     logger.info(c)
     if request.method == 'GET':
         c.update({'form': AppointmentForm()})
         c['post_message'] = None
-        return render(request, 'bocords/index.html', c)
+        return render(request, template_name + '/index.html', c)
     elif request.method == "POST":
         c.update(make_post_context(request.POST, c['basic_info']['consult_email']))
-        return render(request, 'bocords/index.html', c)
+        return render(request, template_name + '/index.html', c)
 
 
 def make_post_context(request_post, consult_mail):
     logger.info(request_post)
     context = {}
     # appointment 앱에서 post 요청을 처리함.
     logger.info(f'request.POST : {request_post}')
```

### Comparing `django_bocor_ds-2.3.1/pyproject.toml` & `django_bocor_ds-3.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "django_bocor_ds"
-version = "2.3.1"
+version = "3.0.0"
 description = "my demiansoft templates"
 authors = [{name = "Hyungjin Kim", email = "hj3415@gmail.com"}]
 readme = "README.md"
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: MIT License"]
 dependencies = [
     "Django >= 4.2.11",
     "libsass>=0.23.0",
     "django-analyticsds >= 0.3.1",
     "django-calendards >= 0.4.0",
     "django-modalds >= 0.1.0",
-    "django-utilsds >= 0.5.1",
+    "django-utilsds >= 0.6.0",
     "django-light >= 0.1.0",
 
 ]
 
 [project.urls]
 Home = "https://www.demiansoft.com"
```

### Comparing `django_bocor_ds-2.3.1/PKG-INFO` & `django_bocor_ds-3.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: django_bocor_ds
-Version: 2.3.1
+Version: 3.0.0
 Summary: my demiansoft templates
 Author-email: Hyungjin Kim <hj3415@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: Django >= 4.2.11
 Requires-Dist: libsass>=0.23.0
 Requires-Dist: django-analyticsds >= 0.3.1
 Requires-Dist: django-calendards >= 0.4.0
 Requires-Dist: django-modalds >= 0.1.0
-Requires-Dist: django-utilsds >= 0.5.1
+Requires-Dist: django-utilsds >= 0.6.0
 Requires-Dist: django-light >= 0.1.0
 Project-URL: Home, https://www.demiansoft.com
 
 ### django-bocor-ds
 
 #### Introduction 
 demiansoft homepage templates
@@ -23,15 +23,15 @@
 #### Requirements
 
 Django >= 4.2.11
 libsass>=0.23.0
 django-analyticsds >= 0.3.1
 django-calendards >= 0.4.0
 django-modalds >= 0.1.0
-django-utilsds >= 0.4.0
+django-utilsds >= 0.6.0
 django-light >= 0.1.0   # 밝은 admin 화면
 
 ---
 #### Install
 
 settings.py  
 ```
```

