# Comparing `tmp/django_herobiz_ds-2.3.0.tar.gz` & `tmp/django_herobiz_ds-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_herobiz_ds-2.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "django_herobiz_ds-3.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `django_herobiz_ds-2.3.0.tar` & `django_herobiz_ds-3.0.0.tar`

### file list

```diff
@@ -1,179 +1,179 @@
--rw-r--r--   0        0        0    10244 2024-05-07 00:45:14.907601 django_herobiz_ds-2.3.0/.DS_Store
--rw-r--r--   0        0        0       66 2024-03-20 23:56:06.731106 django_herobiz_ds-2.3.0/.gitattributes
--rw-r--r--   0        0        0       40 2024-05-07 00:28:25.952876 django_herobiz_ds-2.3.0/.gitignore
--rw-r--r--   0        0        0       52 2024-03-20 23:57:31.872658 django_herobiz_ds-2.3.0/.idea/.gitignore
--rw-r--r--   0        0        0      407 2024-03-20 23:57:31.821245 django_herobiz_ds-2.3.0/.idea/django-herobiz-ds.iml
--rw-r--r--   0        0        0      174 2024-03-20 23:57:31.832580 django_herobiz_ds-2.3.0/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      425 2024-03-21 00:02:45.749953 django_herobiz_ds-2.3.0/.idea/misc.xml
--rw-r--r--   0        0        0      286 2024-03-20 23:57:31.826587 django_herobiz_ds-2.3.0/.idea/modules.xml
--rw-r--r--   0        0        0      167 2024-03-20 23:57:31.834402 django_herobiz_ds-2.3.0/.idea/vcs.xml
--rw-r--r--   0        0        0     1079 2024-03-19 03:45:10.033383 django_herobiz_ds-2.3.0/LICENSE
--rw-r--r--   0        0        0     5021 2024-05-07 00:57:37.575559 django_herobiz_ds-2.3.0/README.md
--rw-r--r--   0        0        0     8196 2024-03-28 02:01:43.009711 django_herobiz_ds-2.3.0/django_herobiz_ds/.DS_Store
--rw-r--r--   0        0        0        0 2024-03-28 01:56:00.401301 django_herobiz_ds-2.3.0/django_herobiz_ds/__init__.py
--rw-r--r--   0        0        0      612 2024-04-20 01:31:00.212458 django_herobiz_ds-2.3.0/django_herobiz_ds/admin.py
--rw-r--r--   0        0        0      164 2024-03-28 01:56:00.402678 django_herobiz_ds-2.3.0/django_herobiz_ds/apps.py
--rw-r--r--   0        0        0     1201 2024-04-20 02:08:26.881448 django_herobiz_ds-2.3.0/django_herobiz_ds/forms.py
--rw-r--r--   0        0        0     1988 2024-04-05 02:30:48.031309 django_herobiz_ds-2.3.0/django_herobiz_ds/migrations/0001_initial.py
--rw-r--r--   0        0        0      421 2024-04-05 03:09:43.264596 django_herobiz_ds-2.3.0/django_herobiz_ds/migrations/0002_portfolio_client.py
--rw-r--r--   0        0        0     2353 2024-04-19 06:58:00.234598 django_herobiz_ds-2.3.0/django_herobiz_ds/migrations/0003_post_profile.py
--rw-r--r--   0        0        0        0 2024-03-28 01:56:00.403238 django_herobiz_ds-2.3.0/django_herobiz_ds/migrations/__init__.py
--rw-r--r--   0        0        0     3116 2024-05-03 07:26:53.545281 django_herobiz_ds-2.3.0/django_herobiz_ds/models.py
--rw-r--r--   0        0        0      555 2024-04-19 06:57:49.960018 django_herobiz_ds-2.3.0/django_herobiz_ds/sitemaps.py
--rwxr-xr-x   0        0        0    60252 2024-03-29 01:14:08.439726 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/css/main.css
--rwxr-xr-x   0        0        0     7992 2024-04-03 08:26:33.002126 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/css/variables-blue.css
--rwxr-xr-x   0        0        0     7989 2024-04-03 08:32:44.614276 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/css/variables-green.css
--rwxr-xr-x   0        0        0     7992 2024-04-03 08:32:44.619981 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/css/variables-orange.css
--rwxr-xr-x   0        0        0     7994 2024-04-03 08:32:44.616432 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/css/variables-pink.css
--rwxr-xr-x   0        0        0     7992 2024-04-03 08:32:44.612088 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/css/variables-purple.css
--rwxr-xr-x   0        0        0     7986 2024-04-03 08:32:44.607824 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/css/variables-red.css
--rwxr-xr-x   0        0        0     7985 2024-04-03 08:32:44.618152 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/css/variables.css
--rwxr-xr-x   0        0        0      766 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/img/about-bg.png
--rwxr-xr-x   0        0        0    95604 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/img/faq.jpg
--rwxr-xr-x   0        0        0    13287 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/img/hero-bg.png
--rwxr-xr-x   0        0        0    13081 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/img/onfocus-content-bg.jpg
--rwxr-xr-x   0        0        0    61855 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/img/pricing-bg.jpg
--rwxr-xr-x   0        0        0     8186 2024-03-17 05:37:08.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/js/main.js
--rwxr-xr-x   0        0        0      281 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/_blog.scss
--rwxr-xr-x   0        0        0     3649 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/_footer.scss
--rwxr-xr-x   0        0        0     3770 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/_general.scss
--rwxr-xr-x   0        0        0     1118 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/_header.scss
--rwxr-xr-x   0        0        0      643 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/_index.scss
--rwxr-xr-x   0        0        0     5712 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/_nav.scss
--rwxr-xr-x   0        0        0     1320 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/_portfolio-details.scss
--rwxr-xr-x   0        0        0     2172 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/blog/_comments.scss
--rwxr-xr-x   0        0        0     3738 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/blog/_details.scss
--rwxr-xr-x   0        0        0      758 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/blog/_pagination.scss
--rwxr-xr-x   0        0        0     1813 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/blog/_posts-list.scss
--rwxr-xr-x   0        0        0     3480 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/blog/_sidebar.scss
--rwxr-xr-x   0        0        0     1676 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/index/_about.scss
--rwxr-xr-x   0        0        0      377 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/index/_clients.scss
--rwxr-xr-x   0        0        0     3086 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/index/_contact.scss
--rwxr-xr-x   0        0        0     1882 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/index/_cta.scss
--rwxr-xr-x   0        0        0     1674 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/index/_faq.scss
--rwxr-xr-x   0        0        0      981 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/index/_featured-services.scss
--rwxr-xr-x   0        0        0     1762 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/index/_features.scss
--rwxr-xr-x   0        0        0     2205 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/index/_hero-animated.scss
--rwxr-xr-x   0        0        0     1990 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/index/_hero-fullscreen.scss
--rwxr-xr-x   0        0        0     1764 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/index/_hero-static.scss
--rwxr-xr-x   0        0        0     3481 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/index/_hero.scss
--rwxr-xr-x   0        0        0     3798 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/index/_onfocus.scss
--rwxr-xr-x   0        0        0     2264 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/index/_portfolio.scss
--rwxr-xr-x   0        0        0     2551 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/index/_pricing.scss
--rwxr-xr-x   0        0        0     1512 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/index/_recent-blog-posts.scss
--rwxr-xr-x   0        0        0     1718 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/index/_services.scss
--rwxr-xr-x   0        0        0     1922 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/index/_team.scss
--rwxr-xr-x   0        0        0     2203 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/index/_testimonials.scss
--rwxr-xr-x   0        0        0      253 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/main.scss
--rwxr-xr-x   0        0        0     7960 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/variables-blue.css
--rwxr-xr-x   0        0        0     7957 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/variables-green.css
--rwxr-xr-x   0        0        0     7960 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/variables-orange.css
--rwxr-xr-x   0        0        0     7962 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/variables-pink.css
--rwxr-xr-x   0        0        0     7960 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/variables-purple.css
--rwxr-xr-x   0        0        0     7954 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/variables-red.css
--rwxr-xr-x   0        0        0     7953 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/variables.css
--rw-r--r--   0        0        0    19941 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/aos/aos.cjs.js
--rw-r--r--   0        0        0    28765 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/aos/aos.css
--rw-r--r--   0        0        0    19768 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/aos/aos.esm.js
--rw-r--r--   0        0        0    13800 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/aos/aos.js
--rw-r--r--   0        0        0    56459 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/aos/aos.js.map
--rw-r--r--   0        0        0    98255 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap-icons/bootstrap-icons.css
--rw-r--r--   0        0        0    52358 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap-icons/bootstrap-icons.json
--rw-r--r--   0        0        0    85875 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap-icons/bootstrap-icons.min.css
--rw-r--r--   0        0        0    57755 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap-icons/bootstrap-icons.scss
--rw-r--r--   0        0        0   176032 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap-icons/fonts/bootstrap-icons.woff
--rw-r--r--   0        0        0   130396 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap-icons/fonts/bootstrap-icons.woff2
--rw-r--r--   0        0        0    70329 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-grid.css
--rw-r--r--   0        0        0   203221 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-grid.css.map
--rw-r--r--   0        0        0    51795 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-grid.min.css
--rw-r--r--   0        0        0   115986 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-grid.min.css.map
--rw-r--r--   0        0        0    70403 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-grid.rtl.css
--rw-r--r--   0        0        0   203225 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-grid.rtl.css.map
--rw-r--r--   0        0        0    51870 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-grid.rtl.min.css
--rw-r--r--   0        0        0   116063 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-grid.rtl.min.css.map
--rw-r--r--   0        0        0    12065 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-reboot.css
--rw-r--r--   0        0        0   129371 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-reboot.css.map
--rw-r--r--   0        0        0    10126 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-reboot.min.css
--rw-r--r--   0        0        0    51369 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-reboot.min.css.map
--rw-r--r--   0        0        0    12058 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-reboot.rtl.css
--rw-r--r--   0        0        0   129386 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-reboot.rtl.css.map
--rw-r--r--   0        0        0    10198 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css
--rw-r--r--   0        0        0    63943 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css.map
--rw-r--r--   0        0        0   107823 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-utilities.css
--rw-r--r--   0        0        0   267535 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-utilities.css.map
--rw-r--r--   0        0        0    85352 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-utilities.min.css
--rw-r--r--   0        0        0   180381 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-utilities.min.css.map
--rw-r--r--   0        0        0   107691 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-utilities.rtl.css
--rw-r--r--   0        0        0   267476 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-utilities.rtl.css.map
--rw-r--r--   0        0        0    85281 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css
--rw-r--r--   0        0        0   180217 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css.map
--rw-r--r--   0        0        0   281046 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap.css
--rw-r--r--   0        0        0   679755 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap.css.map
--rw-r--r--   0        0        0   232803 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap.min.css
--rw-r--r--   0        0        0   589892 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap.min.css.map
--rw-r--r--   0        0        0   280259 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap.rtl.css
--rw-r--r--   0        0        0   679615 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap.rtl.css.map
--rw-r--r--   0        0        0   232911 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap.rtl.min.css
--rw-r--r--   0        0        0   589087 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap.rtl.min.css.map
--rw-r--r--   0        0        0   207819 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/js/bootstrap.bundle.js
--rw-r--r--   0        0        0   444579 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/js/bootstrap.bundle.js.map
--rw-r--r--   0        0        0    80721 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/js/bootstrap.bundle.min.js
--rw-r--r--   0        0        0   332090 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/js/bootstrap.bundle.min.js.map
--rw-r--r--   0        0        0   135829 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/js/bootstrap.esm.js
--rw-r--r--   0        0        0   305438 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/js/bootstrap.esm.js.map
--rw-r--r--   0        0        0    73935 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/js/bootstrap.esm.min.js
--rw-r--r--   0        0        0   222455 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/js/bootstrap.esm.min.js.map
--rw-r--r--   0        0        0   145401 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/js/bootstrap.js
--rw-r--r--   0        0        0   306606 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/js/bootstrap.js.map
--rw-r--r--   0        0        0    60635 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/js/bootstrap.min.js
--rw-r--r--   0        0        0   220561 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/js/bootstrap.min.js.map
--rw-r--r--   0        0        0    17372 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/glightbox/css/glightbox.css
--rw-r--r--   0        0        0    13749 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/glightbox/css/glightbox.min.css
--rw-r--r--   0        0        0    52561 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/glightbox/css/plyr.css
--rw-r--r--   0        0        0    45081 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/glightbox/css/plyr.min.css
--rw-r--r--   0        0        0   109391 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/glightbox/js/glightbox.js
--rw-r--r--   0        0        0    55880 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/glightbox/js/glightbox.min.js
--rw-r--r--   0        0        0    91398 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/isotope-layout/isotope.pkgd.js
--rw-r--r--   0        0        0    35445 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/isotope-layout/isotope.pkgd.min.js
--rwxr-xr-x   0        0        0   238381 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/php-email-form/php-email-form.php
--rwxr-xr-x   0        0        0     2734 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/php-email-form/validate.js
--rw-r--r--   0        0        0    18436 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/swiper/swiper-bundle.min.css
--rw-r--r--   0        0        0   149147 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/swiper/swiper-bundle.min.js
--rw-r--r--   0        0        0   201656 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/swiper/swiper-bundle.min.js.map
--rw-r--r--   0        0        0     2088 2024-04-09 00:06:50.834370 django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/_about.html
--rw-r--r--   0        0        0      430 2024-03-29 06:35:13.298882 django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/_clients.html
--rw-r--r--   0        0        0     2983 2024-04-03 07:06:14.783362 django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/_contact.html
--rw-r--r--   0        0        0     1149 2024-05-07 00:54:12.174157 django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/_cta.html
--rw-r--r--   0        0        0     1595 2024-04-02 01:30:23.624024 django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/_faq.html
--rw-r--r--   0        0        0      794 2024-03-29 06:50:25.784512 django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/_featured-services.html
--rw-r--r--   0        0        0     2035 2024-03-30 02:24:00.706893 django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/_features.html
--rw-r--r--   0        0        0      963 2024-04-05 08:07:21.261387 django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/_hero-animated.html
--rw-r--r--   0        0        0     1819 2024-03-29 05:34:15.457629 django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/_hero-carousel.html
--rw-r--r--   0        0        0      857 2024-03-29 05:40:32.332271 django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/_hero-fullscreen.html
--rw-r--r--   0        0        0      867 2024-03-29 05:42:02.021045 django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/_hero-static.html
--rw-r--r--   0        0        0     1873 2024-05-07 00:56:09.871135 django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/_onfocus.html
--rw-r--r--   0        0        0     1482 2024-04-02 05:48:18.679857 django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/_portfolio.html
--rw-r--r--   0        0        0     1530 2024-04-02 01:24:08.992741 django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/_pricing.html
--rw-r--r--   0        0        0     1085 2024-04-21 01:06:13.810908 django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/_recent-blog-posts.html
--rw-r--r--   0        0        0      956 2024-03-30 02:24:56.706034 django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/_services.html
--rw-r--r--   0        0        0     1660 2024-04-20 23:25:08.777077 django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/_sidebar.html
--rw-r--r--   0        0        0     1485 2024-04-02 07:02:37.695381 django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/_team.html
--rw-r--r--   0        0        0     1325 2024-04-02 00:03:23.122974 django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/_testimonials.html
--rwxr-xr-x   0        0        0    10257 2024-04-21 02:26:19.039647 django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/blog-details.html
--rwxr-xr-x   0        0        0     2859 2024-04-21 01:06:13.803930 django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/blog.html
--rw-r--r--   0        0        0      342 2024-04-05 03:18:33.503234 django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/breadcrumb.html
--rw-r--r--   0        0        0     3934 2024-04-04 04:44:18.713512 django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/footer.html
--rwxr-xr-x   0        0        0     1341 2024-03-12 00:49:58.000000 django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/forms/contact.php
--rw-r--r--   0        0        0     1366 2024-04-21 07:21:08.296478 django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/header.html
--rwxr-xr-x   0        0        0     5086 2024-05-02 04:57:47.243792 django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/index.html
--rwxr-xr-x   0        0        0     2532 2024-04-20 00:39:34.120518 django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/portfolio-details.html
--rwxr-xr-x   0        0        0    16269 2024-04-21 00:18:44.160532 django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/privacy.html
--rw-r--r--   0        0        0     2012 2024-04-03 07:59:23.373918 django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/seo.html
--rwxr-xr-x   0        0        0    16309 2024-04-21 00:18:44.168769 django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/terms.html
--rw-r--r--   0        0        0        0 2023-03-21 07:32:09.033136 django_herobiz_ds-2.3.0/django_herobiz_ds/templatetags/__init__.py
--rw-r--r--   0        0        0     4745 2024-05-03 01:09:29.808810 django_herobiz_ds-2.3.0/django_herobiz_ds/templatetags/herobizds_tags.py
--rw-r--r--   0        0        0       60 2024-03-28 01:56:00.403087 django_herobiz_ds-2.3.0/django_herobiz_ds/tests.py
--rw-r--r--   0        0        0     1111 2024-04-21 00:26:33.998664 django_herobiz_ds-2.3.0/django_herobiz_ds/urls.py
--rw-r--r--   0        0        0     7373 2024-05-02 07:53:42.673922 django_herobiz_ds-2.3.0/django_herobiz_ds/views.py
--rw-r--r--   0        0        0      969 2024-05-07 00:57:37.579961 django_herobiz_ds-2.3.0/pyproject.toml
--rw-r--r--   0        0        0     5757 1970-01-01 00:00:00.000000 django_herobiz_ds-2.3.0/PKG-INFO
+-rw-r--r--   0        0        0    10244 2024-05-18 19:52:14.060654 django_herobiz_ds-3.0.0/.DS_Store
+-rw-r--r--   0        0        0       66 2024-03-20 23:56:06.731106 django_herobiz_ds-3.0.0/.gitattributes
+-rw-r--r--   0        0        0      145 2024-05-18 20:39:30.977910 django_herobiz_ds-3.0.0/.gitignore
+-rw-r--r--   0        0        0       52 2024-03-20 23:57:31.872658 django_herobiz_ds-3.0.0/.idea/.gitignore
+-rw-r--r--   0        0        0      407 2024-03-20 23:57:31.821245 django_herobiz_ds-3.0.0/.idea/django-herobiz-ds.iml
+-rw-r--r--   0        0        0      174 2024-03-20 23:57:31.832580 django_herobiz_ds-3.0.0/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      425 2024-03-21 00:02:45.749953 django_herobiz_ds-3.0.0/.idea/misc.xml
+-rw-r--r--   0        0        0      286 2024-03-20 23:57:31.826587 django_herobiz_ds-3.0.0/.idea/modules.xml
+-rw-r--r--   0        0        0      167 2024-03-20 23:57:31.834402 django_herobiz_ds-3.0.0/.idea/vcs.xml
+-rw-r--r--   0        0        0     1079 2024-03-19 03:45:10.033383 django_herobiz_ds-3.0.0/LICENSE
+-rw-r--r--   0        0        0     5021 2024-05-23 02:16:58.219368 django_herobiz_ds-3.0.0/README.md
+-rw-r--r--   0        0        0     8196 2024-05-18 19:51:53.308139 django_herobiz_ds-3.0.0/django_herobiz_ds/.DS_Store
+-rw-r--r--   0        0        0        0 2024-03-28 01:56:00.401301 django_herobiz_ds-3.0.0/django_herobiz_ds/__init__.py
+-rw-r--r--   0        0        0      612 2024-04-20 01:31:00.212458 django_herobiz_ds-3.0.0/django_herobiz_ds/admin.py
+-rw-r--r--   0        0        0      164 2024-03-28 01:56:00.402678 django_herobiz_ds-3.0.0/django_herobiz_ds/apps.py
+-rw-r--r--   0        0        0     1201 2024-04-20 02:08:26.881448 django_herobiz_ds-3.0.0/django_herobiz_ds/forms.py
+-rw-r--r--   0        0        0     1988 2024-04-05 02:30:48.031309 django_herobiz_ds-3.0.0/django_herobiz_ds/migrations/0001_initial.py
+-rw-r--r--   0        0        0      421 2024-04-05 03:09:43.264596 django_herobiz_ds-3.0.0/django_herobiz_ds/migrations/0002_portfolio_client.py
+-rw-r--r--   0        0        0     2353 2024-04-19 06:58:00.234598 django_herobiz_ds-3.0.0/django_herobiz_ds/migrations/0003_post_profile.py
+-rw-r--r--   0        0        0        0 2024-03-28 01:56:00.403238 django_herobiz_ds-3.0.0/django_herobiz_ds/migrations/__init__.py
+-rw-r--r--   0        0        0     3203 2024-05-23 02:16:58.212227 django_herobiz_ds-3.0.0/django_herobiz_ds/models.py
+-rw-r--r--   0        0        0      647 2024-05-23 02:16:58.208568 django_herobiz_ds-3.0.0/django_herobiz_ds/sitemaps.py
+-rwxr-xr-x   0        0        0    60252 2024-03-29 01:14:08.439726 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/css/main.css
+-rwxr-xr-x   0        0        0     7992 2024-04-03 08:26:33.002126 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/css/variables-blue.css
+-rwxr-xr-x   0        0        0     7989 2024-04-03 08:32:44.614276 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/css/variables-green.css
+-rwxr-xr-x   0        0        0     7992 2024-04-03 08:32:44.619981 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/css/variables-orange.css
+-rwxr-xr-x   0        0        0     7994 2024-04-03 08:32:44.616432 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/css/variables-pink.css
+-rwxr-xr-x   0        0        0     7992 2024-04-03 08:32:44.612088 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/css/variables-purple.css
+-rwxr-xr-x   0        0        0     7986 2024-04-03 08:32:44.607824 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/css/variables-red.css
+-rwxr-xr-x   0        0        0     7985 2024-04-03 08:32:44.618152 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/css/variables.css
+-rwxr-xr-x   0        0        0      766 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/img/about-bg.png
+-rwxr-xr-x   0        0        0    95604 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/img/faq.jpg
+-rwxr-xr-x   0        0        0    13287 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/img/hero-bg.png
+-rwxr-xr-x   0        0        0    13081 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/img/onfocus-content-bg.jpg
+-rwxr-xr-x   0        0        0    61855 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/img/pricing-bg.jpg
+-rwxr-xr-x   0        0        0     8186 2024-03-17 05:37:08.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/js/main.js
+-rwxr-xr-x   0        0        0      281 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/scss/_blog.scss
+-rwxr-xr-x   0        0        0     3649 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/scss/_footer.scss
+-rwxr-xr-x   0        0        0     3770 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/scss/_general.scss
+-rwxr-xr-x   0        0        0     1118 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/scss/_header.scss
+-rwxr-xr-x   0        0        0      643 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/scss/_index.scss
+-rwxr-xr-x   0        0        0     5712 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/scss/_nav.scss
+-rwxr-xr-x   0        0        0     1320 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/scss/_portfolio-details.scss
+-rwxr-xr-x   0        0        0     2172 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/scss/blog/_comments.scss
+-rwxr-xr-x   0        0        0     3738 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/scss/blog/_details.scss
+-rwxr-xr-x   0        0        0      758 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/scss/blog/_pagination.scss
+-rwxr-xr-x   0        0        0     1813 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/scss/blog/_posts-list.scss
+-rwxr-xr-x   0        0        0     3480 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/scss/blog/_sidebar.scss
+-rwxr-xr-x   0        0        0     1676 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/scss/index/_about.scss
+-rwxr-xr-x   0        0        0      377 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/scss/index/_clients.scss
+-rwxr-xr-x   0        0        0     3086 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/scss/index/_contact.scss
+-rwxr-xr-x   0        0        0     1882 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/scss/index/_cta.scss
+-rwxr-xr-x   0        0        0     1674 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/scss/index/_faq.scss
+-rwxr-xr-x   0        0        0      981 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/scss/index/_featured-services.scss
+-rwxr-xr-x   0        0        0     1762 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/scss/index/_features.scss
+-rwxr-xr-x   0        0        0     2205 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/scss/index/_hero-animated.scss
+-rwxr-xr-x   0        0        0     1990 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/scss/index/_hero-fullscreen.scss
+-rwxr-xr-x   0        0        0     1764 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/scss/index/_hero-static.scss
+-rwxr-xr-x   0        0        0     3481 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/scss/index/_hero.scss
+-rwxr-xr-x   0        0        0     3798 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/scss/index/_onfocus.scss
+-rwxr-xr-x   0        0        0     2264 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/scss/index/_portfolio.scss
+-rwxr-xr-x   0        0        0     2551 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/scss/index/_pricing.scss
+-rwxr-xr-x   0        0        0     1512 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/scss/index/_recent-blog-posts.scss
+-rwxr-xr-x   0        0        0     1718 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/scss/index/_services.scss
+-rwxr-xr-x   0        0        0     1922 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/scss/index/_team.scss
+-rwxr-xr-x   0        0        0     2203 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/scss/index/_testimonials.scss
+-rwxr-xr-x   0        0        0      253 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/scss/main.scss
+-rwxr-xr-x   0        0        0     7960 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/scss/variables-blue.css
+-rwxr-xr-x   0        0        0     7957 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/scss/variables-green.css
+-rwxr-xr-x   0        0        0     7960 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/scss/variables-orange.css
+-rwxr-xr-x   0        0        0     7962 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/scss/variables-pink.css
+-rwxr-xr-x   0        0        0     7960 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/scss/variables-purple.css
+-rwxr-xr-x   0        0        0     7954 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/scss/variables-red.css
+-rwxr-xr-x   0        0        0     7985 2024-05-21 00:42:18.466434 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/scss/variables.css
+-rw-r--r--   0        0        0    19941 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/aos/aos.cjs.js
+-rw-r--r--   0        0        0    28765 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/aos/aos.css
+-rw-r--r--   0        0        0    19768 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/aos/aos.esm.js
+-rw-r--r--   0        0        0    13800 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/aos/aos.js
+-rw-r--r--   0        0        0    56459 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/aos/aos.js.map
+-rw-r--r--   0        0        0    98255 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/bootstrap-icons/bootstrap-icons.css
+-rw-r--r--   0        0        0    52358 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/bootstrap-icons/bootstrap-icons.json
+-rw-r--r--   0        0        0    85875 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/bootstrap-icons/bootstrap-icons.min.css
+-rw-r--r--   0        0        0    57755 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/bootstrap-icons/bootstrap-icons.scss
+-rw-r--r--   0        0        0   176032 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/bootstrap-icons/fonts/bootstrap-icons.woff
+-rw-r--r--   0        0        0   130396 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/bootstrap-icons/fonts/bootstrap-icons.woff2
+-rw-r--r--   0        0        0    70329 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-grid.css
+-rw-r--r--   0        0        0   203221 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-grid.css.map
+-rw-r--r--   0        0        0    51795 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-grid.min.css
+-rw-r--r--   0        0        0   115986 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-grid.min.css.map
+-rw-r--r--   0        0        0    70403 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-grid.rtl.css
+-rw-r--r--   0        0        0   203225 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-grid.rtl.css.map
+-rw-r--r--   0        0        0    51870 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-grid.rtl.min.css
+-rw-r--r--   0        0        0   116063 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-grid.rtl.min.css.map
+-rw-r--r--   0        0        0    12065 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-reboot.css
+-rw-r--r--   0        0        0   129371 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-reboot.css.map
+-rw-r--r--   0        0        0    10126 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-reboot.min.css
+-rw-r--r--   0        0        0    51369 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-reboot.min.css.map
+-rw-r--r--   0        0        0    12058 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-reboot.rtl.css
+-rw-r--r--   0        0        0   129386 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-reboot.rtl.css.map
+-rw-r--r--   0        0        0    10198 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css
+-rw-r--r--   0        0        0    63943 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css.map
+-rw-r--r--   0        0        0   107823 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-utilities.css
+-rw-r--r--   0        0        0   267535 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-utilities.css.map
+-rw-r--r--   0        0        0    85352 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-utilities.min.css
+-rw-r--r--   0        0        0   180381 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-utilities.min.css.map
+-rw-r--r--   0        0        0   107691 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-utilities.rtl.css
+-rw-r--r--   0        0        0   267476 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-utilities.rtl.css.map
+-rw-r--r--   0        0        0    85281 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css
+-rw-r--r--   0        0        0   180217 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css.map
+-rw-r--r--   0        0        0   281046 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap.css
+-rw-r--r--   0        0        0   679755 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap.css.map
+-rw-r--r--   0        0        0   232803 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap.min.css
+-rw-r--r--   0        0        0   589892 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap.min.css.map
+-rw-r--r--   0        0        0   280259 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap.rtl.css
+-rw-r--r--   0        0        0   679615 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap.rtl.css.map
+-rw-r--r--   0        0        0   232911 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap.rtl.min.css
+-rw-r--r--   0        0        0   589087 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap.rtl.min.css.map
+-rw-r--r--   0        0        0   207819 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/js/bootstrap.bundle.js
+-rw-r--r--   0        0        0   444579 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/js/bootstrap.bundle.js.map
+-rw-r--r--   0        0        0    80721 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/js/bootstrap.bundle.min.js
+-rw-r--r--   0        0        0   332090 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/js/bootstrap.bundle.min.js.map
+-rw-r--r--   0        0        0   135829 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/js/bootstrap.esm.js
+-rw-r--r--   0        0        0   305438 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/js/bootstrap.esm.js.map
+-rw-r--r--   0        0        0    73935 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/js/bootstrap.esm.min.js
+-rw-r--r--   0        0        0   222455 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/js/bootstrap.esm.min.js.map
+-rw-r--r--   0        0        0   145401 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/js/bootstrap.js
+-rw-r--r--   0        0        0   306606 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/js/bootstrap.js.map
+-rw-r--r--   0        0        0    60635 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/js/bootstrap.min.js
+-rw-r--r--   0        0        0   220561 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/js/bootstrap.min.js.map
+-rw-r--r--   0        0        0    17372 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/glightbox/css/glightbox.css
+-rw-r--r--   0        0        0    13749 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/glightbox/css/glightbox.min.css
+-rw-r--r--   0        0        0    52561 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/glightbox/css/plyr.css
+-rw-r--r--   0        0        0    45081 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/glightbox/css/plyr.min.css
+-rw-r--r--   0        0        0   109391 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/glightbox/js/glightbox.js
+-rw-r--r--   0        0        0    55880 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/glightbox/js/glightbox.min.js
+-rw-r--r--   0        0        0    91398 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/isotope-layout/isotope.pkgd.js
+-rw-r--r--   0        0        0    35445 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/isotope-layout/isotope.pkgd.min.js
+-rwxr-xr-x   0        0        0   238381 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/php-email-form/php-email-form.php
+-rwxr-xr-x   0        0        0     2734 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/php-email-form/validate.js
+-rw-r--r--   0        0        0    18436 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/swiper/swiper-bundle.min.css
+-rw-r--r--   0        0        0   149147 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/swiper/swiper-bundle.min.js
+-rw-r--r--   0        0        0   201656 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/swiper/swiper-bundle.min.js.map
+-rw-r--r--   0        0        0     2113 2024-05-23 02:24:17.730402 django_herobiz_ds-3.0.0/django_herobiz_ds/templates/herobizds/_about.html
+-rw-r--r--   0        0        0      446 2024-05-23 02:22:55.415360 django_herobiz_ds-3.0.0/django_herobiz_ds/templates/herobizds/_clients.html
+-rw-r--r--   0        0        0     2992 2024-05-23 02:22:55.420183 django_herobiz_ds-3.0.0/django_herobiz_ds/templates/herobizds/_contact.html
+-rw-r--r--   0        0        0     1165 2024-05-23 02:20:52.803249 django_herobiz_ds-3.0.0/django_herobiz_ds/templates/herobizds/_cta.html
+-rw-r--r--   0        0        0     1604 2024-05-23 02:20:52.807953 django_herobiz_ds-3.0.0/django_herobiz_ds/templates/herobizds/_faq.html
+-rw-r--r--   0        0        0      794 2024-03-29 06:50:25.784512 django_herobiz_ds-3.0.0/django_herobiz_ds/templates/herobizds/_featured-services.html
+-rw-r--r--   0        0        0     2051 2024-05-23 02:20:52.797770 django_herobiz_ds-3.0.0/django_herobiz_ds/templates/herobizds/_features.html
+-rw-r--r--   0        0        0      988 2024-05-23 02:20:52.805759 django_herobiz_ds-3.0.0/django_herobiz_ds/templates/herobizds/_hero-animated.html
+-rw-r--r--   0        0        0     1844 2024-05-23 02:20:52.812548 django_herobiz_ds-3.0.0/django_herobiz_ds/templates/herobizds/_hero-carousel.html
+-rw-r--r--   0        0        0      873 2024-05-23 02:20:52.810483 django_herobiz_ds-3.0.0/django_herobiz_ds/templates/herobizds/_hero-fullscreen.html
+-rw-r--r--   0        0        0      876 2024-05-23 02:20:52.814251 django_herobiz_ds-3.0.0/django_herobiz_ds/templates/herobizds/_hero-static.html
+-rw-r--r--   0        0        0     1905 2024-05-23 02:16:58.193751 django_herobiz_ds-3.0.0/django_herobiz_ds/templates/herobizds/_onfocus.html
+-rw-r--r--   0        0        0     1491 2024-05-23 02:16:58.192016 django_herobiz_ds-3.0.0/django_herobiz_ds/templates/herobizds/_portfolio.html
+-rw-r--r--   0        0        0     1467 2024-05-23 02:16:58.213862 django_herobiz_ds-3.0.0/django_herobiz_ds/templates/herobizds/_pricing.html
+-rw-r--r--   0        0        0     1181 2024-05-23 02:16:58.220384 django_herobiz_ds-3.0.0/django_herobiz_ds/templates/herobizds/_recent-blog-posts.html
+-rw-r--r--   0        0        0      972 2024-05-23 02:16:58.154764 django_herobiz_ds-3.0.0/django_herobiz_ds/templates/herobizds/_services.html
+-rw-r--r--   0        0        0     1696 2024-05-23 02:16:58.217275 django_herobiz_ds-3.0.0/django_herobiz_ds/templates/herobizds/_sidebar.html
+-rw-r--r--   0        0        0     1501 2024-05-23 02:16:58.181493 django_herobiz_ds-3.0.0/django_herobiz_ds/templates/herobizds/_team.html
+-rw-r--r--   0        0        0     1357 2024-05-23 02:16:58.199415 django_herobiz_ds-3.0.0/django_herobiz_ds/templates/herobizds/_testimonials.html
+-rwxr-xr-x   0        0        0    10336 2024-05-23 02:16:58.187055 django_herobiz_ds-3.0.0/django_herobiz_ds/templates/herobizds/blog-details.html
+-rwxr-xr-x   0        0        0     3000 2024-05-23 02:16:58.183519 django_herobiz_ds-3.0.0/django_herobiz_ds/templates/herobizds/blog.html
+-rw-r--r--   0        0        0      351 2024-05-23 02:16:58.210456 django_herobiz_ds-3.0.0/django_herobiz_ds/templates/herobizds/breadcrumb.html
+-rw-r--r--   0        0        0     3934 2024-04-04 04:44:18.713512 django_herobiz_ds-3.0.0/django_herobiz_ds/templates/herobizds/footer.html
+-rwxr-xr-x   0        0        0     1341 2024-03-12 00:49:58.000000 django_herobiz_ds-3.0.0/django_herobiz_ds/templates/herobizds/forms/contact.php
+-rw-r--r--   0        0        0     1400 2024-05-23 02:16:58.164076 django_herobiz_ds-3.0.0/django_herobiz_ds/templates/herobizds/header.html
+-rwxr-xr-x   0        0        0     5189 2024-05-23 02:16:58.195800 django_herobiz_ds-3.0.0/django_herobiz_ds/templates/herobizds/index.html
+-rwxr-xr-x   0        0        0     2550 2024-05-23 02:16:58.166511 django_herobiz_ds-3.0.0/django_herobiz_ds/templates/herobizds/portfolio-details.html
+-rwxr-xr-x   0        0        0    16287 2024-05-23 02:16:58.175186 django_herobiz_ds-3.0.0/django_herobiz_ds/templates/herobizds/privacy.html
+-rw-r--r--   0        0        0     2076 2024-05-23 02:16:58.160314 django_herobiz_ds-3.0.0/django_herobiz_ds/templates/herobizds/seo.html
+-rwxr-xr-x   0        0        0    16327 2024-05-23 02:16:58.223117 django_herobiz_ds-3.0.0/django_herobiz_ds/templates/herobizds/terms.html
+-rw-r--r--   0        0        0        0 2023-03-21 07:32:09.033136 django_herobiz_ds-3.0.0/django_herobiz_ds/templatetags/__init__.py
+-rw-r--r--   0        0        0     5735 2024-05-23 02:16:58.170523 django_herobiz_ds-3.0.0/django_herobiz_ds/templatetags/herobizds_tags.py
+-rw-r--r--   0        0        0       60 2024-03-28 01:56:00.403087 django_herobiz_ds-3.0.0/django_herobiz_ds/tests.py
+-rw-r--r--   0        0        0     1165 2024-05-23 02:16:58.198088 django_herobiz_ds-3.0.0/django_herobiz_ds/urls.py
+-rw-r--r--   0        0        0     7332 2024-05-23 02:16:58.215830 django_herobiz_ds-3.0.0/django_herobiz_ds/views.py
+-rw-r--r--   0        0        0      969 2024-05-23 02:16:58.146959 django_herobiz_ds-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0     5757 1970-01-01 00:00:00.000000 django_herobiz_ds-3.0.0/PKG-INFO
```

### Comparing `django_herobiz_ds-2.3.0/.DS_Store` & `django_herobiz_ds-3.0.0/.DS_Store`

 * *Files 6% similar despite different names*

```diff
@@ -252,157 +252,157 @@
 00000fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001000: 0000 0000 0000 0000 0000 002c 0000 0004  ...........,....
 00001010: 002e 0067 0069 0074 6c67 3153 636f 6d70  ...g.i.tlg1Scomp
-00001020: 0000 0000 02d1 1501 0000 0004 002e 0067  ...............g
+00001020: 0000 0000 02d1 efdf 0000 0004 002e 0067  ...............g
 00001030: 0069 0074 6d6f 4444 626c 6f62 0000 0008  .i.tmoDDblob....
-00001040: 8353 b64a 65f2 c541 0000 0004 002e 0067  .S.Je..A.......g
+00001040: f8ed 5338 53f6 c541 0000 0004 002e 0067  ..S8S..A.......g
 00001050: 0069 0074 6d6f 6444 626c 6f62 0000 0008  .i.tmodDblob....
-00001060: 8353 b64a 65f2 c541 0000 0004 002e 0067  .S.Je..A.......g
+00001060: f8ed 5338 53f6 c541 0000 0004 002e 0067  ..S8S..A.......g
 00001070: 0069 0074 7068 3153 636f 6d70 0000 0000  .i.tph1Scomp....
-00001080: 02f2 1000 0000 0005 002e 0069 0064 0065  ...........i.d.e
+00001080: 02f5 1000 0000 0005 002e 0069 0064 0065  ...........i.d.e
 00001090: 0061 6c67 3153 636f 6d70 0000 0000 0000  .alg1Scomp......
-000010a0: 1844 0000 0005 002e 0069 0064 0065 0061  .D.......i.d.e.a
-000010b0: 6d6f 4444 626c 6f62 0000 0008 4dbd b8a9  moDDblob....M...
-000010c0: 64f2 c541 0000 0005 002e 0069 0064 0065  d..A.......i.d.e
-000010d0: 0061 6d6f 6444 626c 6f62 0000 0008 4dbd  .amodDblob....M.
-000010e0: b8a9 64f2 c541 0000 0005 002e 0069 0064  ..d..A.......i.d
+000010a0: 17c1 0000 0005 002e 0069 0064 0065 0061  .........i.d.e.a
+000010b0: 6d6f 4444 626c 6f62 0000 0008 915a 24b7  moDDblob.....Z$.
+000010c0: 25f6 c541 0000 0005 002e 0069 0064 0065  %..A.......i.d.e
+000010d0: 0061 6d6f 6444 626c 6f62 0000 0008 915a  .amodDblob.....Z
+000010e0: 24b7 25f6 c541 0000 0005 002e 0069 0064  $.%..A.......i.d
 000010f0: 0065 0061 7068 3153 636f 6d70 0000 0000  .e.aph1Scomp....
 00001100: 0000 8000 0000 0005 002e 0076 0065 006e  ...........v.e.n
 00001110: 0076 6c67 3153 636f 6d70 0000 0000 0661  .vlg1Scomp.....a
 00001120: 9a7d 0000 0005 002e 0076 0065 006e 0076  .}.......v.e.n.v
 00001130: 6d6f 4444 626c 6f62 0000 0008 e6e8 12b2  moDDblob........
 00001140: d7d5 c541 0000 0005 002e 0076 0065 006e  ...A.......v.e.n
 00001150: 0076 6d6f 6444 626c 6f62 0000 0008 e6e8  .vmodDblob......
 00001160: 12b2 d7d5 c541 0000 0005 002e 0076 0065  .....A.......v.e
 00001170: 006e 0076 7068 3153 636f 6d70 0000 0000  .n.vph1Scomp....
 00001180: 079b 7000 0000 0005 005f 0064 0061 0074  ..p......_.d.a.t
-00001190: 0061 6277 7370 626c 6f62 0000 00b9 6270  .abwspblob....bp
+00001190: 0061 6277 7370 626c 6f62 0000 00b8 6270  .abwspblob....bp
 000011a0: 6c69 7374 3030 d601 0203 0405 0607 0807  list00..........
 000011b0: 080b 085d 5368 6f77 5374 6174 7573 4261  ...]ShowStatusBa
 000011c0: 725b 5368 6f77 546f 6f6c 6261 725b 5368  r[ShowToolbar[Sh
 000011d0: 6f77 5461 6256 6965 775f 1014 436f 6e74  owTabView_..Cont
 000011e0: 6169 6e65 7253 686f 7753 6964 6562 6172  ainerShowSidebar
 000011f0: 5c57 696e 646f 7742 6f75 6e64 735b 5368  \WindowBounds[Sh
-00001200: 6f77 5369 6465 6261 7208 0908 095f 1019  owSidebar...._..
-00001210: 7b7b 3138 382c 2033 3236 7d2c 207b 3132  {{188, 326}, {12
-00001220: 3332 2c20 3638 377d 7d09 0815 232f 3b52  32, 687}}...#/;R
-00001230: 5f6b 6c6d 6e6f 8b00 0000 0000 0001 0100  _klmno..........
-00001240: 0000 0000 0000 0d00 0000 0000 0000 0000  ................
-00001250: 0000 0000 0000 8c00 0000 0500 5f00 6400  ............_.d.
-00001260: 6100 7400 616c 6731 5363 6f6d 7000 0000  a.t.alg1Scomp...
-00001270: 0000 00b0 6900 0000 0500 5f00 6400 6100  ....i....._.d.a.
-00001280: 7400 616d 6f44 4462 6c6f 6200 0000 08cb  t.amoDDblob.....
-00001290: 62b8 dc65 eac5 4100 0000 0500 5f00 6400  b..e..A....._.d.
-000012a0: 6100 7400 616d 6f64 4462 6c6f 6200 0000  a.t.amodDblob...
-000012b0: 08cb 62b8 dc65 eac5 4100 0000 0500 5f00  ..b..e..A....._.
-000012c0: 6400 6100 7400 6170 6831 5363 6f6d 7000  d.a.t.aph1Scomp.
-000012d0: 0000 0000 00e0 0000 0000 0500 5f00 6400  ............_.d.
-000012e0: 6100 7400 6176 5372 6e6c 6f6e 6700 0000  a.t.avSrnlong...
-000012f0: 0100 0000 0900 5f00 6d00 7900 7400 6500  ......_.m.y.t.e.
-00001300: 7300 7400 6500 7262 7773 7062 6c6f 6200  s.t.e.rbwspblob.
-00001310: 0000 b862 706c 6973 7430 30d6 0102 0304  ...bplist00.....
-00001320: 0506 0708 0708 0b08 5d53 686f 7753 7461  ........]ShowSta
-00001330: 7475 7342 6172 5b53 686f 7754 6f6f 6c62  tusBar[ShowToolb
-00001340: 6172 5b53 686f 7754 6162 5669 6577 5f10  ar[ShowTabView_.
-00001350: 1443 6f6e 7461 696e 6572 5368 6f77 5369  .ContainerShowSi
-00001360: 6465 6261 725c 5769 6e64 6f77 426f 756e  debar\WindowBoun
-00001370: 6473 5b53 686f 7753 6964 6562 6172 0809  ds[ShowSidebar..
-00001380: 0809 5f10 187b 7b38 3239 2c20 3533 317d  .._..{{829, 531}
-00001390: 2c20 7b39 3230 2c20 3433 367d 7d09 0815  , {920, 436}}...
-000013a0: 232f 3b52 5f6b 6c6d 6e6f 8a00 0000 0000  #/;R_klmno......
-000013b0: 0001 0100 0000 0000 0000 0d00 0000 0000  ................
-000013c0: 0000 0000 0000 0000 0000 8b00 0000 0900  ................
-000013d0: 5f00 6d00 7900 7400 6500 7300 7400 6500  _.m.y.t.e.s.t.e.
-000013e0: 726c 6731 5363 6f6d 7000 0000 0000 0031  rlg1Scomp......1
-000013f0: 0f00 0000 0900 5f00 6d00 7900 7400 6500  ......_.m.y.t.e.
-00001400: 7300 7400 6500 726d 6f44 4462 6c6f 6200  s.t.e.rmoDDblob.
-00001410: 0000 0850 db50 8925 e9c5 4100 0000 0900  ...P.P.%..A.....
-00001420: 5f00 6d00 7900 7400 6500 7300 7400 6500  _.m.y.t.e.s.t.e.
-00001430: 726d 6f64 4462 6c6f 6200 0000 0850 db50  rmodDblob....P.P
-00001440: 8925 e9c5 4100 0000 0900 5f00 6d00 7900  .%..A....._.m.y.
-00001450: 7400 6500 7300 7400 6500 7270 6831 5363  t.e.s.t.e.rph1Sc
-00001460: 6f6d 7000 0000 0000 0090 0000 0000 0900  omp.............
-00001470: 5f00 6d00 7900 7400 6500 7300 7400 6500  _.m.y.t.e.s.t.e.
-00001480: 7276 5372 6e6c 6f6e 6700 0000 0100 0000  rvSrnlong.......
-00001490: 0700 5f00 7300 7400 6100 7400 6900 6362  .._.s.t.a.t.i.cb
-000014a0: 7773 7062 6c6f 6200 0000 b862 706c 6973  wspblob....bplis
-000014b0: 7430 30d6 0102 0304 0506 0708 0708 0b08  t00.............
-000014c0: 5d53 686f 7753 7461 7475 7342 6172 5b53  ]ShowStatusBar[S
-000014d0: 686f 7754 6f6f 6c62 6172 5b53 686f 7754  howToolbar[ShowT
-000014e0: 6162 5669 6577 5f10 1443 6f6e 7461 696e  abView_..Contain
-000014f0: 6572 5368 6f77 5369 6465 6261 725c 5769  erShowSidebar\Wi
-00001500: 6e64 6f77 426f 756e 6473 5b53 686f 7753  ndowBounds[ShowS
-00001510: 6964 6562 6172 0809 0809 5f10 187b 7b36  idebar...._..{{6
-00001520: 3231 2c20 3331 367d 2c20 7b39 3230 2c20  21, 316}, {920, 
-00001530: 3433 367d 7d09 0815 232f 3b52 5f6b 6c6d  436}}...#/;R_klm
-00001540: 6e6f 8a00 0000 0000 0001 0100 0000 0000  no..............
-00001550: 0000 0d00 0000 0000 0000 0000 0000 0000  ................
-00001560: 0000 8b00 0000 0700 5f00 7300 7400 6100  ........_.s.t.a.
-00001570: 7400 6900 636c 6731 5363 6f6d 7000 0000  t.i.clg1Scomp...
-00001580: 0000 27ff e300 0000 0700 5f00 7300 7400  ..'......._.s.t.
-00001590: 6100 7400 6900 636d 6f44 4462 6c6f 6200  a.t.i.cmoDDblob.
-000015a0: 0000 086f 5396 6f8d dac5 4100 0000 0700  ...oS.o...A.....
-000015b0: 5f00 7300 7400 6100 7400 6900 636d 6f64  _.s.t.a.t.i.cmod
-000015c0: 4462 6c6f 6200 0000 086f 5396 6f8d dac5  Dblob....oS.o...
-000015d0: 4100 0000 0700 5f00 7300 7400 6100 7400  A....._.s.t.a.t.
-000015e0: 6900 6370 6831 5363 6f6d 7000 0000 0000  i.cph1Scomp.....
-000015f0: 29d0 0000 0000 0700 5f00 7300 7400 6100  )......._.s.t.a.
-00001600: 7400 6900 6376 5372 6e6c 6f6e 6700 0000  t.i.cvSrnlong...
-00001610: 0100 0000 0400 6400 6900 7300 746c 6731  ......d.i.s.tlg1
-00001620: 5363 6f6d 7000 0000 0002 0ba6 c000 0000  Scomp...........
-00001630: 0400 6400 6900 7300 746d 6f44 4462 6c6f  ..d.i.s.tmoDDblo
-00001640: 6200 0000 0817 7412 a364 f2c5 4100 0000  b.....t..d..A...
-00001650: 0400 6400 6900 7300 746d 6f64 4462 6c6f  ..d.i.s.tmodDblo
-00001660: 6200 0000 0817 7412 a364 f2c5 4100 0000  b.....t..d..A...
-00001670: 0400 6400 6900 7300 7470 6831 5363 6f6d  ..d.i.s.tph1Scom
-00001680: 7000 0000 0002 0bd0 0000 0000 1100 6400  p.............d.
-00001690: 6a00 6100 6e00 6700 6f00 5f00 6800 6500  j.a.n.g.o._.h.e.
-000016a0: 7200 6f00 6200 6900 7a00 5f00 6400 7362  r.o.b.i.z._.d.sb
-000016b0: 7773 7062 6c6f 6200 0000 b862 706c 6973  wspblob....bplis
-000016c0: 7430 30d6 0102 0304 0506 0708 0708 0b08  t00.............
-000016d0: 5d53 686f 7753 7461 7475 7342 6172 5b53  ]ShowStatusBar[S
-000016e0: 686f 7754 6f6f 6c62 6172 5b53 686f 7754  howToolbar[ShowT
-000016f0: 6162 5669 6577 5f10 1443 6f6e 7461 696e  abView_..Contain
-00001700: 6572 5368 6f77 5369 6465 6261 725c 5769  erShowSidebar\Wi
-00001710: 6e64 6f77 426f 756e 6473 5b53 686f 7753  ndowBounds[ShowS
-00001720: 6964 6562 6172 0809 0809 5f10 187b 7b33  idebar...._..{{3
-00001730: 3831 2c20 3533 397d 2c20 7b39 3230 2c20  81, 539}, {920, 
-00001740: 3433 367d 7d09 0815 232f 3b52 5f6b 6c6d  436}}...#/;R_klm
-00001750: 6e6f 8a00 0000 0000 0001 0100 0000 0000  no..............
-00001760: 0000 0d00 0000 0000 0000 0000 0000 0000  ................
-00001770: 0000 8b00 0000 1100 6400 6a00 6100 6e00  ........d.j.a.n.
-00001780: 6700 6f00 5f00 6800 6500 7200 6f00 6200  g.o._.h.e.r.o.b.
-00001790: 6900 7a00 5f00 6400 736c 6731 5363 6f6d  i.z._.d.slg1Scom
-000017a0: 7000 0000 0000 a913 d400 0000 1100 6400  p.............d.
-000017b0: 6a00 6100 6e00 6700 6f00 5f00 6800 6500  j.a.n.g.o._.h.e.
-000017c0: 7200 6f00 6200 6900 7a00 5f00 6400 736d  r.o.b.i.z._.d.sm
-000017d0: 6f44 4462 6c6f 6200 0000 08c0 ccc5 9e64  oDDblob........d
-000017e0: f2c5 4100 0000 1100 6400 6a00 6100 6e00  ..A.....d.j.a.n.
-000017f0: 6700 6f00 5f00 6800 6500 7200 6f00 6200  g.o._.h.e.r.o.b.
-00001800: 6900 7a00 5f00 6400 736d 6f64 4462 6c6f  i.z._.d.smodDblo
-00001810: 6200 0000 08c0 ccc5 9e64 f2c5 4100 0000  b........d..A...
-00001820: 1100 6400 6a00 6100 6e00 6700 6f00 5f00  ..d.j.a.n.g.o._.
-00001830: 6800 6500 7200 6f00 6200 6900 7a00 5f00  h.e.r.o.b.i.z._.
-00001840: 6400 7370 6831 5363 6f6d 7000 0000 0000  d.sph1Scomp.....
-00001850: aeb0 0000 0000 1100 6400 6a00 6100 6e00  ........d.j.a.n.
-00001860: 6700 6f00 5f00 6800 6500 7200 6f00 6200  g.o._.h.e.r.o.b.
-00001870: 6900 7a00 5f00 6400 7376 5372 6e6c 6f6e  i.z._.d.svSrnlon
-00001880: 6700 0000 0100 0000 0500 6d00 6500 6400  g.........m.e.d.
-00001890: 6900 616c 6731 5363 6f6d 7000 0000 0001  i.alg1Scomp.....
-000018a0: 6dc0 ab00 0000 0500 6d00 6500 6400 6900  m.......m.e.d.i.
-000018b0: 616d 6f44 4462 6c6f 6200 0000 0830 3b54  amoDDblob....0;T
-000018c0: b6a8 e9c5 4100 0000 0500 6d00 6500 6400  ....A.....m.e.d.
-000018d0: 6900 616d 6f64 4462 6c6f 6200 0000 0830  i.amodDblob....0
-000018e0: 3b54 b6a8 e9c5 4100 0000 0500 6d00 6500  ;T....A.....m.e.
-000018f0: 6400 6900 6170 6831 5363 6f6d 7000 0000  d.i.aph1Scomp...
-00001900: 0001 6df0 0000 0000 0000 0000 0000 0000  ..m.............
+00001200: 6f77 5369 6465 6261 7208 0908 095f 1018  owSidebar...._..
+00001210: 7b7b 3331 322c 2032 3335 7d2c 207b 3932  {{312, 235}, {92
+00001220: 302c 2034 3336 7d7d 0908 1523 2f3b 525f  0, 436}}...#/;R_
+00001230: 6b6c 6d6e 6f8a 0000 0000 0000 0101 0000  klmno...........
+00001240: 0000 0000 000d 0000 0000 0000 0000 0000  ................
+00001250: 0000 0000 008b 0000 0005 005f 0064 0061  ..........._.d.a
+00001260: 0074 0061 6c67 3153 636f 6d70 0000 0000  .t.alg1Scomp....
+00001270: 0000 affd 0000 0005 005f 0064 0061 0074  ........._.d.a.t
+00001280: 0061 6d6f 4444 626c 6f62 0000 0008 0573  .amoDDblob.....s
+00001290: 016d d9f4 c541 0000 0005 005f 0064 0061  .m...A....._.d.a
+000012a0: 0074 0061 6d6f 6444 626c 6f62 0000 0008  .t.amodDblob....
+000012b0: 0573 016d d9f4 c541 0000 0005 005f 0064  .s.m...A....._.d
+000012c0: 0061 0074 0061 7068 3153 636f 6d70 0000  .a.t.aph1Scomp..
+000012d0: 0000 0000 e000 0000 0005 005f 0064 0061  ..........._.d.a
+000012e0: 0074 0061 7653 726e 6c6f 6e67 0000 0001  .t.avSrnlong....
+000012f0: 0000 0009 005f 006d 0079 0074 0065 0073  ....._.m.y.t.e.s
+00001300: 0074 0065 0072 6277 7370 626c 6f62 0000  .t.e.rbwspblob..
+00001310: 00b8 6270 6c69 7374 3030 d601 0203 0405  ..bplist00......
+00001320: 0607 0807 080b 085d 5368 6f77 5374 6174  .......]ShowStat
+00001330: 7573 4261 725b 5368 6f77 546f 6f6c 6261  usBar[ShowToolba
+00001340: 725b 5368 6f77 5461 6256 6965 775f 1014  r[ShowTabView_..
+00001350: 436f 6e74 6169 6e65 7253 686f 7753 6964  ContainerShowSid
+00001360: 6562 6172 5c57 696e 646f 7742 6f75 6e64  ebar\WindowBound
+00001370: 735b 5368 6f77 5369 6465 6261 7208 0908  s[ShowSidebar...
+00001380: 095f 1018 7b7b 3832 392c 2035 3331 7d2c  ._..{{829, 531},
+00001390: 207b 3932 302c 2034 3336 7d7d 0908 1523   {920, 436}}...#
+000013a0: 2f3b 525f 6b6c 6d6e 6f8a 0000 0000 0000  /;R_klmno.......
+000013b0: 0101 0000 0000 0000 000d 0000 0000 0000  ................
+000013c0: 0000 0000 0000 0000 008b 0000 0009 005f  ..............._
+000013d0: 006d 0079 0074 0065 0073 0074 0065 0072  .m.y.t.e.s.t.e.r
+000013e0: 6c67 3153 636f 6d70 0000 0000 0000 310f  lg1Scomp......1.
+000013f0: 0000 0009 005f 006d 0079 0074 0065 0073  ....._.m.y.t.e.s
+00001400: 0074 0065 0072 6d6f 4444 626c 6f62 0000  .t.e.rmoDDblob..
+00001410: 0008 50db 5089 25e9 c541 0000 0009 005f  ..P.P.%..A....._
+00001420: 006d 0079 0074 0065 0073 0074 0065 0072  .m.y.t.e.s.t.e.r
+00001430: 6d6f 6444 626c 6f62 0000 0008 50db 5089  modDblob....P.P.
+00001440: 25e9 c541 0000 0009 005f 006d 0079 0074  %..A....._.m.y.t
+00001450: 0065 0073 0074 0065 0072 7068 3153 636f  .e.s.t.e.rph1Sco
+00001460: 6d70 0000 0000 0000 9000 0000 0009 005f  mp............._
+00001470: 006d 0079 0074 0065 0073 0074 0065 0072  .m.y.t.e.s.t.e.r
+00001480: 7653 726e 6c6f 6e67 0000 0001 0000 0007  vSrnlong........
+00001490: 005f 0073 0074 0061 0074 0069 0063 6277  ._.s.t.a.t.i.cbw
+000014a0: 7370 626c 6f62 0000 00b8 6270 6c69 7374  spblob....bplist
+000014b0: 3030 d601 0203 0405 0607 0807 080b 085d  00.............]
+000014c0: 5368 6f77 5374 6174 7573 4261 725b 5368  ShowStatusBar[Sh
+000014d0: 6f77 546f 6f6c 6261 725b 5368 6f77 5461  owToolbar[ShowTa
+000014e0: 6256 6965 775f 1014 436f 6e74 6169 6e65  bView_..Containe
+000014f0: 7253 686f 7753 6964 6562 6172 5c57 696e  rShowSidebar\Win
+00001500: 646f 7742 6f75 6e64 735b 5368 6f77 5369  dowBounds[ShowSi
+00001510: 6465 6261 7208 0908 095f 1018 7b7b 3632  debar...._..{{62
+00001520: 312c 2033 3136 7d2c 207b 3932 302c 2034  1, 316}, {920, 4
+00001530: 3336 7d7d 0908 1523 2f3b 525f 6b6c 6d6e  36}}...#/;R_klmn
+00001540: 6f8a 0000 0000 0000 0101 0000 0000 0000  o...............
+00001550: 000d 0000 0000 0000 0000 0000 0000 0000  ................
+00001560: 008b 0000 0007 005f 0073 0074 0061 0074  ......._.s.t.a.t
+00001570: 0069 0063 6c67 3153 636f 6d70 0000 0000  .i.clg1Scomp....
+00001580: 0027 ffe3 0000 0007 005f 0073 0074 0061  .'......._.s.t.a
+00001590: 0074 0069 0063 6d6f 4444 626c 6f62 0000  .t.i.cmoDDblob..
+000015a0: 0008 6f53 966f 8dda c541 0000 0007 005f  ..oS.o...A....._
+000015b0: 0073 0074 0061 0074 0069 0063 6d6f 6444  .s.t.a.t.i.cmodD
+000015c0: 626c 6f62 0000 0008 6f53 966f 8dda c541  blob....oS.o...A
+000015d0: 0000 0007 005f 0073 0074 0061 0074 0069  ....._.s.t.a.t.i
+000015e0: 0063 7068 3153 636f 6d70 0000 0000 0029  .cph1Scomp.....)
+000015f0: d000 0000 0007 005f 0073 0074 0061 0074  ......._.s.t.a.t
+00001600: 0069 0063 7653 726e 6c6f 6e67 0000 0001  .i.cvSrnlong....
+00001610: 0000 0004 0064 0069 0073 0074 6c67 3153  .....d.i.s.tlg1S
+00001620: 636f 6d70 0000 0000 0256 1378 0000 0004  comp.....V.x....
+00001630: 0064 0069 0073 0074 6d6f 4444 626c 6f62  .d.i.s.tmoDDblob
+00001640: 0000 0008 d9a5 7a04 daf4 c541 0000 0004  ......z....A....
+00001650: 0064 0069 0073 0074 6d6f 6444 626c 6f62  .d.i.s.tmodDblob
+00001660: 0000 0008 d9a5 7a04 daf4 c541 0000 0004  ......z....A....
+00001670: 0064 0069 0073 0074 7068 3153 636f 6d70  .d.i.s.tph1Scomp
+00001680: 0000 0000 0256 4000 0000 0011 0064 006a  .....V@......d.j
+00001690: 0061 006e 0067 006f 005f 0068 0065 0072  .a.n.g.o._.h.e.r
+000016a0: 006f 0062 0069 007a 005f 0064 0073 6277  .o.b.i.z._.d.sbw
+000016b0: 7370 626c 6f62 0000 00b8 6270 6c69 7374  spblob....bplist
+000016c0: 3030 d601 0203 0405 0607 0807 080b 085d  00.............]
+000016d0: 5368 6f77 5374 6174 7573 4261 725b 5368  ShowStatusBar[Sh
+000016e0: 6f77 546f 6f6c 6261 725b 5368 6f77 5461  owToolbar[ShowTa
+000016f0: 6256 6965 775f 1014 436f 6e74 6169 6e65  bView_..Containe
+00001700: 7253 686f 7753 6964 6562 6172 5c57 696e  rShowSidebar\Win
+00001710: 646f 7742 6f75 6e64 735b 5368 6f77 5369  dowBounds[ShowSi
+00001720: 6465 6261 7208 0908 095f 1018 7b7b 3331  debar...._..{{31
+00001730: 322c 2032 3335 7d2c 207b 3932 302c 2034  2, 235}, {920, 4
+00001740: 3336 7d7d 0908 1523 2f3b 525f 6b6c 6d6e  36}}...#/;R_klmn
+00001750: 6f8a 0000 0000 0000 0101 0000 0000 0000  o...............
+00001760: 000d 0000 0000 0000 0000 0000 0000 0000  ................
+00001770: 008b 0000 0011 0064 006a 0061 006e 0067  .......d.j.a.n.g
+00001780: 006f 005f 0068 0065 0072 006f 0062 0069  .o._.h.e.r.o.b.i
+00001790: 007a 005f 0064 0073 6c67 3153 636f 6d70  .z._.d.slg1Scomp
+000017a0: 0000 0000 00a9 1419 0000 0011 0064 006a  .............d.j
+000017b0: 0061 006e 0067 006f 005f 0068 0065 0072  .a.n.g.o._.h.e.r
+000017c0: 006f 0062 0069 007a 005f 0064 0073 6d6f  .o.b.i.z._.d.smo
+000017d0: 4444 626c 6f62 0000 0008 0270 c86d 9ff5  DDblob.....p.m..
+000017e0: c541 0000 0011 0064 006a 0061 006e 0067  .A.....d.j.a.n.g
+000017f0: 006f 005f 0068 0065 0072 006f 0062 0069  .o._.h.e.r.o.b.i
+00001800: 007a 005f 0064 0073 6d6f 6444 626c 6f62  .z._.d.smodDblob
+00001810: 0000 0008 0270 c86d 9ff5 c541 0000 0011  .....p.m...A....
+00001820: 0064 006a 0061 006e 0067 006f 005f 0068  .d.j.a.n.g.o._.h
+00001830: 0065 0072 006f 0062 0069 007a 005f 0064  .e.r.o.b.i.z._.d
+00001840: 0073 7068 3153 636f 6d70 0000 0000 00ae  .sph1Scomp......
+00001850: b000 0000 0011 0064 006a 0061 006e 0067  .......d.j.a.n.g
+00001860: 006f 005f 0068 0065 0072 006f 0062 0069  .o._.h.e.r.o.b.i
+00001870: 007a 005f 0064 0073 7653 726e 6c6f 6e67  .z._.d.svSrnlong
+00001880: 0000 0001 0000 0005 006d 0065 0064 0069  .........m.e.d.i
+00001890: 0061 6c67 3153 636f 6d70 0000 0000 016d  .alg1Scomp.....m
+000018a0: c0ab 0000 0005 006d 0065 0064 0069 0061  .......m.e.d.i.a
+000018b0: 6d6f 4444 626c 6f62 0000 0008 303b 54b6  moDDblob....0;T.
+000018c0: a8e9 c541 0000 0005 006d 0065 0064 0069  ...A.....m.e.d.i
+000018d0: 0061 6d6f 6444 626c 6f62 0000 0008 303b  .amodDblob....0;
+000018e0: 54b6 a8e9 c541 0000 0005 006d 0065 0064  T....A.....m.e.d
+000018f0: 0069 0061 7068 3153 636f 6d70 0000 0000  .i.aph1Scomp....
+00001900: 016d f000 0000 0000 0000 0000 0000 0000  .m..............
 00001910: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001920: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001930: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001940: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001950: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001960: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001970: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -586,56 +586,56 @@
 00002490: 0100 0200 0000 0000 0100 0400 0000 0000  ................
 000024a0: 0100 0800 0000 0000 0100 1000 0000 0000  ................
 000024b0: 0100 2000 0000 0000 0100 4000 0000 0000  .. .......@.....
 000024c0: 0100 8000 0000 0000 0101 0000 0000 0000  ................
 000024d0: 0102 0000 0000 0000 0104 0000 0000 0000  ................
 000024e0: 0108 0000 0000 0000 0110 0000 0000 0000  ................
 000024f0: 0120 0000 0000 0000 0140 0000 0000 0000  . .......@......
-00002500: 0064 6f77 426f 756e 6473 5b53 686f 7753  .dowBounds[ShowS
-00002510: 6964 6562 6172 0809 0809 5f10 187b 7b36  idebar...._..{{6
-00002520: 3231 2c20 3331 367d 2c20 7b39 3230 2c20  21, 316}, {920, 
-00002530: 3433 367d 7d09 0815 232f 3b52 5f6b 6c6d  436}}...#/;R_klm
-00002540: 6e6f 8a00 0000 0000 0001 0100 0000 0000  no..............
-00002550: 0000 0d00 0000 0000 0000 0000 0000 0000  ................
-00002560: 0000 8b00 0000 0700 5f00 7300 7400 6100  ........_.s.t.a.
-00002570: 7400 6900 636c 6731 5363 6f6d 7000 0000  t.i.clg1Scomp...
-00002580: 0000 27ff e300 0000 0700 5f00 7300 7400  ..'......._.s.t.
-00002590: 6100 7400 6900 636d 6f44 4462 6c6f 6200  a.t.i.cmoDDblob.
-000025a0: 0000 086f 5396 6f8d dac5 4100 0000 0700  ...oS.o...A.....
-000025b0: 5f00 7300 7400 6100 7400 6900 636d 6f64  _.s.t.a.t.i.cmod
-000025c0: 4462 6c6f 6200 0000 086f 5396 6f8d dac5  Dblob....oS.o...
-000025d0: 4100 0000 0700 5f00 7300 7400 6100 7400  A....._.s.t.a.t.
-000025e0: 6900 6370 6831 5363 6f6d 7000 0000 0000  i.cph1Scomp.....
-000025f0: 29d0 0000 0000 0700 5f00 7300 7400 6100  )......._.s.t.a.
-00002600: 7400 6900 6376 5372 6e6c 6f6e 6700 0000  t.i.cvSrnlong...
-00002610: 0100 0000 0400 6400 6900 7300 746c 6731  ......d.i.s.tlg1
-00002620: 5363 6f6d 7000 0000 0002 0ba6 c000 0000  Scomp...........
-00002630: 0400 6400 6900 7300 746d 6f44 4462 6c6f  ..d.i.s.tmoDDblo
-00002640: 6200 0000 0817 7412 a364 f2c5 4100 0000  b.....t..d..A...
-00002650: 0400 6400 6900 7300 746d 6f64 4462 6c6f  ..d.i.s.tmodDblo
-00002660: 6200 0000 0817 7412 a364 f2c5 4100 0000  b.....t..d..A...
-00002670: 0400 6400 6900 7300 7470 6831 5363 6f6d  ..d.i.s.tph1Scom
-00002680: 7000 0000 0002 0bd0 0000 0000 1100 6400  p.............d.
-00002690: 6a00 6100 6e00 6700 6f00 5f00 6800 6500  j.a.n.g.o._.h.e.
-000026a0: 7200 6f00 6200 6900 7a00 5f00 6400 7362  r.o.b.i.z._.d.sb
-000026b0: 7773 7062 6c6f 6200 0000 b862 706c 6973  wspblob....bplis
-000026c0: 7430 30d6 0102 0304 0506 0708 0708 0b08  t00.............
-000026d0: 5d53 686f 7753 7461 7475 7342 6172 5b53  ]ShowStatusBar[S
-000026e0: 686f 7754 6f6f 6c62 6172 5b53 686f 7754  howToolbar[ShowT
-000026f0: 6162 5669 6577 5f10 1443 6f6e 7461 696e  abView_..Contain
-00002700: 6572 5368 6f77 5369 6465 6261 725c 5769  erShowSidebar\Wi
-00002710: 6e64 6f77 426f 756e 6473 5b53 686f 7753  ndowBounds[ShowS
-00002720: 6964 6562 6172 0809 0809 5f10 187b 7b33  idebar...._..{{3
-00002730: 3831 2c20 3533 397d 2c20 7b39 3230 2c20  81, 539}, {920, 
-00002740: 3433 367d 7d09 0815 232f 3b52 5f6b 6c6d  436}}...#/;R_klm
-00002750: 6e6f 8a00 0000 0000 0001 0100 0000 0000  no..............
-00002760: 0000 0d00 0000 0000 0000 0000 0000 0000  ................
-00002770: 0000 8b00 0000 1100 6400 6a00 6100 6e00  ........d.j.a.n.
-00002780: 6700 6f00 5f00 6800 6500 7200 6f00 6200  g.o._.h.e.r.o.b.
-00002790: 6900 7a00 5f00 6400 736c 6731 5363 6f6d  i.z._.d.slg1Scom
-000027a0: 7000 0000 0000 a913 d400 0000 1100 6400  p.............d.
-000027b0: 6a00 6100 6e00 6700 6f00 5f00 6800 6500  j.a.n.g.o._.h.e.
-000027c0: 7200 6f00 6200 6900 7a00 5f00 6400 736d  r.o.b.i.z._.d.sm
-000027d0: 6f44 4462 6c6f 6200 0000 08c0 ccc5 9e64  oDDblob........d
-000027e0: f2c5 4100 0000 1100 6400 6a00 6100 6e00  ..A.....d.j.a.n.
-000027f0: 6700 6f00 5f00 6800 6500 7200 6f00 6200  g.o._.h.e.r.o.b.
-00002800: 6900 7a00                                i.z.
+00002500: 006f 7742 6f75 6e64 735b 5368 6f77 5369  .owBounds[ShowSi
+00002510: 6465 6261 7208 0908 095f 1018 7b7b 3632  debar...._..{{62
+00002520: 312c 2033 3136 7d2c 207b 3932 302c 2034  1, 316}, {920, 4
+00002530: 3336 7d7d 0908 1523 2f3b 525f 6b6c 6d6e  36}}...#/;R_klmn
+00002540: 6f8a 0000 0000 0000 0101 0000 0000 0000  o...............
+00002550: 000d 0000 0000 0000 0000 0000 0000 0000  ................
+00002560: 008b 0000 0007 005f 0073 0074 0061 0074  ......._.s.t.a.t
+00002570: 0069 0063 6c67 3153 636f 6d70 0000 0000  .i.clg1Scomp....
+00002580: 0027 ffe3 0000 0007 005f 0073 0074 0061  .'......._.s.t.a
+00002590: 0074 0069 0063 6d6f 4444 626c 6f62 0000  .t.i.cmoDDblob..
+000025a0: 0008 6f53 966f 8dda c541 0000 0007 005f  ..oS.o...A....._
+000025b0: 0073 0074 0061 0074 0069 0063 6d6f 6444  .s.t.a.t.i.cmodD
+000025c0: 626c 6f62 0000 0008 6f53 966f 8dda c541  blob....oS.o...A
+000025d0: 0000 0007 005f 0073 0074 0061 0074 0069  ....._.s.t.a.t.i
+000025e0: 0063 7068 3153 636f 6d70 0000 0000 0029  .cph1Scomp.....)
+000025f0: d000 0000 0007 005f 0073 0074 0061 0074  ......._.s.t.a.t
+00002600: 0069 0063 7653 726e 6c6f 6e67 0000 0001  .i.cvSrnlong....
+00002610: 0000 0004 0064 0069 0073 0074 6c67 3153  .....d.i.s.tlg1S
+00002620: 636f 6d70 0000 0000 0256 1378 0000 0004  comp.....V.x....
+00002630: 0064 0069 0073 0074 6d6f 4444 626c 6f62  .d.i.s.tmoDDblob
+00002640: 0000 0008 d9a5 7a04 daf4 c541 0000 0004  ......z....A....
+00002650: 0064 0069 0073 0074 6d6f 6444 626c 6f62  .d.i.s.tmodDblob
+00002660: 0000 0008 d9a5 7a04 daf4 c541 0000 0004  ......z....A....
+00002670: 0064 0069 0073 0074 7068 3153 636f 6d70  .d.i.s.tph1Scomp
+00002680: 0000 0000 0256 4000 0000 0011 0064 006a  .....V@......d.j
+00002690: 0061 006e 0067 006f 005f 0068 0065 0072  .a.n.g.o._.h.e.r
+000026a0: 006f 0062 0069 007a 005f 0064 0073 6277  .o.b.i.z._.d.sbw
+000026b0: 7370 626c 6f62 0000 00b8 6270 6c69 7374  spblob....bplist
+000026c0: 3030 d601 0203 0405 0607 0807 080b 085d  00.............]
+000026d0: 5368 6f77 5374 6174 7573 4261 725b 5368  ShowStatusBar[Sh
+000026e0: 6f77 546f 6f6c 6261 725b 5368 6f77 5461  owToolbar[ShowTa
+000026f0: 6256 6965 775f 1014 436f 6e74 6169 6e65  bView_..Containe
+00002700: 7253 686f 7753 6964 6562 6172 5c57 696e  rShowSidebar\Win
+00002710: 646f 7742 6f75 6e64 735b 5368 6f77 5369  dowBounds[ShowSi
+00002720: 6465 6261 7208 0908 095f 1018 7b7b 3331  debar...._..{{31
+00002730: 322c 2032 3335 7d2c 207b 3932 302c 2034  2, 235}, {920, 4
+00002740: 3336 7d7d 0908 1523 2f3b 525f 6b6c 6d6e  36}}...#/;R_klmn
+00002750: 6f8a 0000 0000 0000 0101 0000 0000 0000  o...............
+00002760: 000d 0000 0000 0000 0000 0000 0000 0000  ................
+00002770: 008b 0000 0011 0064 006a 0061 006e 0067  .......d.j.a.n.g
+00002780: 006f 005f 0068 0065 0072 006f 0062 0069  .o._.h.e.r.o.b.i
+00002790: 007a 005f 0064 0073 6c67 3153 636f 6d70  .z._.d.slg1Scomp
+000027a0: 0000 0000 00a9 1419 0000 0011 0064 006a  .............d.j
+000027b0: 0061 006e 0067 006f 005f 0068 0065 0072  .a.n.g.o._.h.e.r
+000027c0: 006f 0062 0069 007a 005f 0064 0073 6d6f  .o.b.i.z._.d.smo
+000027d0: 4444 626c 6f62 0000 0008 0270 c86d 9ff5  DDblob.....p.m..
+000027e0: c541 0000 0011 0064 006a 0061 006e 0067  .A.....d.j.a.n.g
+000027f0: 006f 005f 0068 0065 0072 006f 0062 0069  .o._.h.e.r.o.b.i
+00002800: 007a 005f                                .z._
```

### Comparing `django_herobiz_ds-2.3.0/LICENSE` & `django_herobiz_ds-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/README.md` & `django_herobiz_ds-3.0.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 #### Requirements
 
 Django >= 4.2.11
 libsass>=0.23.0
 django-analyticsds >= 0.3.1
 django-calendards >= 0.4.0
 django-modalds >= 0.1.0
-django-utilsds >= 0.4.0
+django-utilsds >= 0.6.0
 django-mdeditor >= 0.1.20
 django-hitcount >= 1.3.5
 django-taggit >= 5.0.1
 django-markdownify >= 0.9.3
 django-light >= 0.1.0   # 밝은 admin 화면
 pillow >= 10.3.0    # 데이터베이스에서 이미지 사용하기위해
```

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/.DS_Store` & `django_herobiz_ds-3.0.0/django_herobiz_ds/.DS_Store`

 * *Files 8% similar despite different names*

```diff
@@ -259,16 +259,16 @@
 00001020: 626c 6f62 0000 00b8 6270 6c69 7374 3030  blob....bplist00
 00001030: d601 0203 0405 0607 0807 080b 085d 5368  .............]Sh
 00001040: 6f77 5374 6174 7573 4261 725b 5368 6f77  owStatusBar[Show
 00001050: 546f 6f6c 6261 725b 5368 6f77 5461 6256  Toolbar[ShowTabV
 00001060: 6965 775f 1014 436f 6e74 6169 6e65 7253  iew_..ContainerS
 00001070: 686f 7753 6964 6562 6172 5c57 696e 646f  howSidebar\Windo
 00001080: 7742 6f75 6e64 735b 5368 6f77 5369 6465  wBounds[ShowSide
-00001090: 6261 7208 0908 095f 1018 7b7b 3137 312c  bar...._..{{171,
-000010a0: 2036 3337 7d2c 207b 3932 302c 2034 3336   637}, {920, 436
+00001090: 6261 7208 0908 095f 1018 7b7b 3331 322c  bar...._..{{312,
+000010a0: 2032 3335 7d2c 207b 3932 302c 2034 3336   235}, {920, 436
 000010b0: 7d7d 0908 1523 2f3b 525f 6b6c 6d6e 6f8a  }}...#/;R_klmno.
 000010c0: 0000 0000 0000 0101 0000 0000 0000 000d  ................
 000010d0: 0000 0000 0000 0000 0000 0000 0000 008b  ................
 000010e0: 0000 0006 0073 0074 0061 0074 0069 0063  .....s.t.a.t.i.c
 000010f0: 6c67 3153 636f 6d70 0000 0000 0000 0000  lg1Scomp........
 00001100: 0000 0006 0073 0074 0061 0074 0069 0063  .....s.t.a.t.i.c
 00001110: 6d6f 4444 626c 6f62 0000 0008 3dd0 ec70  moDDblob....=..p
@@ -283,16 +283,16 @@
 000011a0: 6f62 0000 00b8 6270 6c69 7374 3030 d601  ob....bplist00..
 000011b0: 0203 0405 0607 0807 080b 085d 5368 6f77  ...........]Show
 000011c0: 5374 6174 7573 4261 725b 5368 6f77 546f  StatusBar[ShowTo
 000011d0: 6f6c 6261 725b 5368 6f77 5461 6256 6965  olbar[ShowTabVie
 000011e0: 775f 1014 436f 6e74 6169 6e65 7253 686f  w_..ContainerSho
 000011f0: 7753 6964 6562 6172 5c57 696e 646f 7742  wSidebar\WindowB
 00001200: 6f75 6e64 735b 5368 6f77 5369 6465 6261  ounds[ShowSideba
-00001210: 7208 0908 095f 1018 7b7b 3137 312c 2036  r...._..{{171, 6
-00001220: 3337 7d2c 207b 3932 302c 2034 3336 7d7d  37}, {920, 436}}
+00001210: 7208 0908 095f 1018 7b7b 3331 322c 2032  r...._..{{312, 2
+00001220: 3335 7d2c 207b 3932 302c 2034 3336 7d7d  35}, {920, 436}}
 00001230: 0908 1523 2f3b 525f 6b6c 6d6e 6f8a 0000  ...#/;R_klmno...
 00001240: 0000 0000 0101 0000 0000 0000 000d 0000  ................
 00001250: 0000 0000 0000 0000 0000 0000 008b 0000  ................
 00001260: 0009 0074 0065 006d 0070 006c 0061 0074  ...t.e.m.p.l.a.t
 00001270: 0065 0073 6c67 3153 636f 6d70 0000 0000  .e.slg1Scomp....
 00001280: 0000 0000 0000 0009 0074 0065 006d 0070  .........t.e.m.p
 00001290: 006c 0061 0074 0065 0073 6d6f 4444 626c  .l.a.t.e.smoDDbl
@@ -309,16 +309,16 @@
 00001340: 626c 6f62 0000 00b8 6270 6c69 7374 3030  blob....bplist00
 00001350: d601 0203 0405 0607 0807 080b 085d 5368  .............]Sh
 00001360: 6f77 5374 6174 7573 4261 725b 5368 6f77  owStatusBar[Show
 00001370: 546f 6f6c 6261 725b 5368 6f77 5461 6256  Toolbar[ShowTabV
 00001380: 6965 775f 1014 436f 6e74 6169 6e65 7253  iew_..ContainerS
 00001390: 686f 7753 6964 6562 6172 5c57 696e 646f  howSidebar\Windo
 000013a0: 7742 6f75 6e64 735b 5368 6f77 5369 6465  wBounds[ShowSide
-000013b0: 6261 7208 0908 095f 1018 7b7b 3137 312c  bar...._..{{171,
-000013c0: 2036 3337 7d2c 207b 3932 302c 2034 3336   637}, {920, 436
+000013b0: 6261 7208 0908 095f 1018 7b7b 3331 322c  bar...._..{{312,
+000013c0: 2032 3335 7d2c 207b 3932 302c 2034 3336   235}, {920, 436
 000013d0: 7d7d 0908 1523 2f3b 525f 6b6c 6d6e 6f8a  }}...#/;R_klmno.
 000013e0: 0000 0000 0000 0101 0000 0000 0000 000d  ................
 000013f0: 0000 0000 0000 0000 0000 0000 0000 008b  ................
 00001400: 0000 000c 0074 0065 006d 0070 006c 0061  .....t.e.m.p.l.a
 00001410: 0074 0065 0074 0061 0067 0073 6c67 3153  .t.e.t.a.g.slg1S
 00001420: 636f 6d70 0000 0000 0000 0000 0000 000c  comp............
 00001430: 0074 0065 006d 0070 006c 0061 0074 0065  .t.e.m.p.l.a.t.e
```

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/admin.py` & `django_herobiz_ds-3.0.0/django_herobiz_ds/admin.py`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/forms.py` & `django_herobiz_ds-3.0.0/django_herobiz_ds/forms.py`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/migrations/0001_initial.py` & `django_herobiz_ds-3.0.0/django_herobiz_ds/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/migrations/0003_post_profile.py` & `django_herobiz_ds-3.0.0/django_herobiz_ds/migrations/0003_post_profile.py`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/models.py` & `django_herobiz_ds-3.0.0/django_herobiz_ds/models.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 from django.db import models
 from mdeditor.fields import MDTextField
 from _data.herobizds import CATEGORY
+from _data import herobizds
 from taggit.managers import TaggableManager
 from django.contrib.auth.models import User
 from hitcount.models import HitCount
 from django.contrib.contenttypes.fields import GenericRelation
 
+template_name = herobizds.context['template_name']
+
 
 class Portfolio(models.Model):
     title = models.CharField('제목', max_length=20)
     subtitle = models.CharField('부제목', max_length=40)
     filter = models.ForeignKey(
         'Category',
         related_name='category',
@@ -63,15 +66,15 @@
 
     def __str__(self):
         return self.title
 
     def get_absolute_url(self):
         from django.urls import reverse
 
-        return reverse("herobizds:post_detail", kwargs={"slug": str(self.slug)})
+        return reverse(template_name + ':post_detail', kwargs={"slug": str(self.slug)})
 
 
 class Profile(models.Model):
     user = models.OneToOneField(User, on_delete=models.CASCADE)     # Delete profile when user is deleted
     image = models.ImageField(default='default_profile.jpg', upload_to='profile_pics')
 
     def __str__(self):
```

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/sitemaps.py` & `django_herobiz_ds-3.0.0/django_herobiz_ds/sitemaps.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 from django.contrib.sitemaps import Sitemap
 from .models import Post
 from django.urls import reverse
+from _data import herobizds
+
+
+template_name = herobizds.context['template_name']
 
 
 class PostSitemap(Sitemap):
     changefreq = "weekly"
     priority = 0.8
 
     def items(self):
@@ -16,12 +20,12 @@
 
 class StaticViewSitemap(Sitemap):
     priority = 0.5
     changefreq = 'weekly'
 
     def items(self):
         return [
-            'herobizds:home',
+            template_name + ':home',
         ]
 
     def location(self, item):
         return reverse(item)
```

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/css/main.css` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/css/main.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/css/variables-blue.css` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/css/variables-blue.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/css/variables-green.css` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/css/variables-green.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/css/variables-orange.css` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/css/variables-orange.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/css/variables-pink.css` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/css/variables-pink.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/css/variables-purple.css` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/css/variables-purple.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/css/variables-red.css` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/css/variables-red.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/css/variables.css` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/css/variables.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/img/about-bg.png` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/img/about-bg.png`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/img/faq.jpg` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/img/faq.jpg`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/img/hero-bg.png` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/img/hero-bg.png`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/img/onfocus-content-bg.jpg` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/img/onfocus-content-bg.jpg`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/img/pricing-bg.jpg` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/img/pricing-bg.jpg`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/js/main.js` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/js/main.js`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/_footer.scss` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/scss/_footer.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/_general.scss` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/scss/_general.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/_header.scss` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/scss/_header.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/_index.scss` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/scss/_index.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/_nav.scss` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/scss/_nav.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/_portfolio-details.scss` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/scss/_portfolio-details.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/blog/_comments.scss` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/scss/blog/_comments.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/blog/_details.scss` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/scss/blog/_details.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/blog/_pagination.scss` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/scss/blog/_pagination.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/blog/_posts-list.scss` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/scss/blog/_posts-list.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/blog/_sidebar.scss` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/scss/blog/_sidebar.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/index/_about.scss` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/scss/index/_about.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/index/_contact.scss` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/scss/index/_contact.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/index/_cta.scss` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/scss/index/_cta.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/index/_faq.scss` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/scss/index/_faq.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/index/_featured-services.scss` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/scss/index/_featured-services.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/index/_features.scss` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/scss/index/_features.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/index/_hero-animated.scss` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/scss/index/_hero-animated.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/index/_hero-fullscreen.scss` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/scss/index/_hero-fullscreen.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/index/_hero-static.scss` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/scss/index/_hero-static.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/index/_hero.scss` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/scss/index/_hero.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/index/_onfocus.scss` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/scss/index/_onfocus.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/index/_portfolio.scss` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/scss/index/_portfolio.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/index/_pricing.scss` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/scss/index/_pricing.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/index/_recent-blog-posts.scss` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/scss/index/_recent-blog-posts.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/index/_services.scss` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/scss/index/_services.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/index/_team.scss` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/scss/index/_team.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/index/_testimonials.scss` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/scss/index/_testimonials.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/variables-blue.css` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/scss/variables-blue.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/variables-green.css` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/scss/variables-green.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/variables-orange.css` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/scss/variables-orange.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/variables-pink.css` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/scss/variables-pink.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/variables-purple.css` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/scss/variables-purple.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/variables-red.css` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/scss/variables-red.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/scss/variables.css` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/scss/variables.css`

 * *Files 1% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 
 /*--------------------------------------------------------------
 # 1. HeroBiz template variables 
 --------------------------------------------------------------*/
 :root {
 
   /* Fonts */
-  --font-default: 'Open Sans', system-ui, -apple-system, "Segoe UI", Roboto, "Helvetica Neue", Arial, "Noto Sans", "Liberation Sans", sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol", "Noto Color Emoji";
-  --font-primary: 'Source Sans Pro', sans-serif;
+  --font-default: 'Noto Sans KR', 'Open Sans', system-ui, -apple-system, "Segoe UI", Roboto, "Helvetica Neue", Arial, "Noto Sans", "Liberation Sans", sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol", "Noto Color Emoji";
+  --font-primary: 'Noto Sans KR', 'Source Sans Pro', sans-serif;
   --font-secondary: 'Poppins', sans-serif;
 
   /* Colors */
   /* The *-rgb color names are simply the RGB converted value of the corresponding color for use in the rgba() function */
 
   /* Default text color */
   --color-default: #1a1f24;
```

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/aos/aos.cjs.js` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/aos/aos.cjs.js`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/aos/aos.css` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/aos/aos.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/aos/aos.esm.js` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/aos/aos.esm.js`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/aos/aos.js` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/aos/aos.js`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/aos/aos.js.map` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/aos/aos.js.map`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap-icons/bootstrap-icons.css` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/bootstrap-icons/bootstrap-icons.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap-icons/bootstrap-icons.json` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/bootstrap-icons/bootstrap-icons.json`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap-icons/bootstrap-icons.min.css` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/bootstrap-icons/bootstrap-icons.min.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap-icons/bootstrap-icons.scss` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/bootstrap-icons/bootstrap-icons.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap-icons/fonts/bootstrap-icons.woff` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/bootstrap-icons/fonts/bootstrap-icons.woff`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap-icons/fonts/bootstrap-icons.woff2` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/bootstrap-icons/fonts/bootstrap-icons.woff2`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-grid.css` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-grid.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-grid.css.map` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-grid.css.map`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-grid.min.css` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-grid.min.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-grid.min.css.map` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-grid.min.css.map`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-grid.rtl.css` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-grid.rtl.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-grid.rtl.css.map` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-grid.rtl.css.map`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-grid.rtl.min.css` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-grid.rtl.min.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-grid.rtl.min.css.map` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-grid.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-reboot.css` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-reboot.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-reboot.css.map` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-reboot.css.map`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-reboot.min.css` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-reboot.min.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-reboot.min.css.map` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-reboot.min.css.map`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-reboot.rtl.css` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-reboot.rtl.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-reboot.rtl.css.map` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-reboot.rtl.css.map`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css.map` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-utilities.css` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-utilities.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-utilities.css.map` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-utilities.css.map`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-utilities.min.css` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-utilities.min.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-utilities.min.css.map` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-utilities.min.css.map`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-utilities.rtl.css` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-utilities.rtl.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-utilities.rtl.css.map` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-utilities.rtl.css.map`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css.map` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap.css` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap.css.map` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap.min.css` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap.min.css.map` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap.rtl.css` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap.rtl.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap.rtl.css.map` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap.rtl.css.map`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap.rtl.min.css` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap.rtl.min.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap.rtl.min.css.map` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/css/bootstrap.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/js/bootstrap.bundle.js` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/js/bootstrap.bundle.js`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/js/bootstrap.bundle.js.map` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/js/bootstrap.bundle.js.map`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/js/bootstrap.bundle.min.js` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/js/bootstrap.bundle.min.js.map` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/js/bootstrap.bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/js/bootstrap.esm.js` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/js/bootstrap.esm.js`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/js/bootstrap.esm.js.map` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/js/bootstrap.esm.js.map`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/js/bootstrap.esm.min.js` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/js/bootstrap.esm.min.js`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/js/bootstrap.esm.min.js.map` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/js/bootstrap.esm.min.js.map`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/js/bootstrap.js` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/js/bootstrap.js.map` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/js/bootstrap.js.map`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/js/bootstrap.min.js` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/js/bootstrap.min.js.map` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/bootstrap/js/bootstrap.min.js.map`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/glightbox/css/glightbox.css` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/glightbox/css/glightbox.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/glightbox/css/glightbox.min.css` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/glightbox/css/glightbox.min.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/glightbox/css/plyr.css` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/glightbox/css/plyr.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/glightbox/css/plyr.min.css` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/glightbox/css/plyr.min.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/glightbox/js/glightbox.js` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/glightbox/js/glightbox.js`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/glightbox/js/glightbox.min.js` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/glightbox/js/glightbox.min.js`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/isotope-layout/isotope.pkgd.js` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/isotope-layout/isotope.pkgd.js`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/isotope-layout/isotope.pkgd.min.js` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/isotope-layout/isotope.pkgd.min.js`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/php-email-form/php-email-form.php` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/php-email-form/php-email-form.php`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/php-email-form/validate.js` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/php-email-form/validate.js`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/swiper/swiper-bundle.min.css` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/swiper/swiper-bundle.min.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/swiper/swiper-bundle.min.js` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/swiper/swiper-bundle.min.js`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/static/herobizds/vendor/swiper/swiper-bundle.min.js.map` & `django_herobiz_ds-3.0.0/django_herobiz_ds/static/herobizds/vendor/swiper/swiper-bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/_about.html` & `django_herobiz_ds-3.0.0/django_herobiz_ds/templates/herobizds/_features.html`

 * *Files 19% similar despite different names*

```diff
@@ -1,131 +1,129 @@
 00000000: 7b25 206c 6f61 6420 7374 6174 6963 2025  {% load static %
-00000010: 7d0a 0a3c 7374 796c 653e 0a20 202e 6162  }..<style>.  .ab
-00000020: 6f75 7420 2e61 626f 7574 2d69 6d67 3a62  out .about-img:b
-00000030: 6566 6f72 6520 7b0a 2020 706f 7369 7469  efore {.  positi
-00000040: 6f6e 3a20 6162 736f 6c75 7465 3b0a 2020  on: absolute;.  
-00000050: 696e 7365 743a 202d 3630 7078 2030 2030  inset: -60px 0 0
-00000060: 202d 3630 7078 3b0a 2020 7a2d 696e 6465   -60px;.  z-inde
-00000070: 783a 202d 313b 0a20 2063 6f6e 7465 6e74  x: -1;.  content
-00000080: 3a20 2222 3b0a 2020 6261 636b 6772 6f75  : "";.  backgrou
-00000090: 6e64 3a20 7572 6c28 227b 2520 7374 6174  nd: url("{% stat
-000000a0: 6963 2027 6865 726f 6269 7a64 732f 696d  ic 'herobizds/im
-000000b0: 672f 6162 6f75 742d 6267 2e70 6e67 2720  g/about-bg.png' 
-000000c0: 257d 2229 2074 6f70 206c 6566 743b 0a20  %}") top left;. 
-000000d0: 2062 6163 6b67 726f 756e 642d 7265 7065   background-repe
-000000e0: 6174 3a20 6e6f 2d72 6570 6561 743b 0a7d  at: no-repeat;.}
-000000f0: 0a3c 2f73 7479 6c65 3e0a 0a3c 7365 6374  .</style>..<sect
-00000100: 696f 6e20 6964 3d22 6162 6f75 7422 2063  ion id="about" c
-00000110: 6c61 7373 3d22 6162 6f75 7422 3e0a 2020  lass="about">.  
-00000120: 3c64 6976 2063 6c61 7373 3d22 636f 6e74  <div class="cont
-00000130: 6169 6e65 7222 2064 6174 612d 616f 733d  ainer" data-aos=
-00000140: 2266 6164 652d 7570 223e 0a0a 2020 2020  "fade-up">..    
-00000150: 3c64 6976 2063 6c61 7373 3d22 7365 6374  <div class="sect
-00000160: 696f 6e2d 6865 6164 6572 223e 0a20 2020  ion-header">.   
-00000170: 2020 203c 6832 3e41 626f 7574 2055 733c     <h2>About Us<
-00000180: 2f68 323e 0a20 2020 2020 203c 703e 7b7b  /h2>.      <p>{{
-00000190: 2061 626f 7574 5f70 207d 7d3c 2f70 3e0a   about_p }}</p>.
-000001a0: 2020 2020 3c2f 6469 763e 0a0a 2020 2020      </div>..    
-000001b0: 3c64 6976 2063 6c61 7373 3d22 726f 7720  <div class="row 
-000001c0: 672d 3420 672d 6c67 2d35 2220 6461 7461  g-4 g-lg-5" data
-000001d0: 2d61 6f73 3d22 6661 6465 2d75 7022 2064  -aos="fade-up" d
-000001e0: 6174 612d 616f 732d 6465 6c61 793d 2232  ata-aos-delay="2
-000001f0: 3030 223e 0a0a 2020 2020 2020 3c64 6976  00">..      <div
-00000200: 2063 6c61 7373 3d22 636f 6c2d 6c67 2d35   class="col-lg-5
-00000210: 223e 0a20 2020 2020 2020 203c 6469 7620  ">.        <div 
-00000220: 636c 6173 733d 2261 626f 7574 2d69 6d67  class="about-img
-00000230: 223e 0a20 2020 2020 2020 2020 203c 696d  ">.          <im
-00000240: 6720 7372 633d 227b 2520 7374 6174 6963  g src="{% static
-00000250: 2027 696d 672f 6865 726f 6269 7a64 732f   'img/herobizds/
-00000260: 277c 6164 643a 6162 6f75 745f 696d 6167  '|add:about_imag
-00000270: 6527 2025 7d22 2063 6c61 7373 3d22 696d  e' %}" class="im
-00000280: 672d 666c 7569 6422 2061 6c74 3d22 223e  g-fluid" alt="">
-00000290: 0a20 2020 2020 2020 203c 2f64 6976 3e0a  .        </div>.
-000002a0: 2020 2020 2020 3c2f 6469 763e 0a0a 2020        </div>..  
-000002b0: 2020 2020 3c64 6976 2063 6c61 7373 3d22      <div class="
-000002c0: 636f 6c2d 6c67 2d37 223e 0a20 2020 2020  col-lg-7">.     
-000002d0: 2020 207b 2520 6175 746f 6573 6361 7065     {% autoescape
-000002e0: 206f 6666 2025 7d0a 2020 2020 2020 2020   off %}.        
-000002f0: 3c68 3320 636c 6173 733d 2270 742d 3020  <h3 class="pt-0 
-00000300: 7074 2d6c 672d 3522 3e7b 7b20 6162 6f75  pt-lg-5">{{ abou
-00000310: 745f 6833 207d 7d3c 2f68 333e 0a0a 2020  t_h3 }}</h3>..  
-00000320: 2020 2020 2020 3c21 2d2d 2054 6162 7320        <!-- Tabs 
-00000330: 2d2d 3e0a 2020 2020 2020 2020 3c75 6c20  -->.        <ul 
-00000340: 636c 6173 733d 226e 6176 206e 6176 2d70  class="nav nav-p
-00000350: 696c 6c73 206d 622d 3322 3e0a 2020 2020  ills mb-3">.    
-00000360: 2020 2020 2020 7b25 2066 6f72 2069 7465        {% for ite
-00000370: 6d20 696e 2061 626f 7574 2025 7d0a 2020  m in about %}.  
-00000380: 2020 2020 2020 2020 3c6c 693e 3c61 2063          <li><a c
-00000390: 6c61 7373 3d22 6e61 762d 6c69 6e6b 0a20  lass="nav-link. 
-000003a0: 2020 2020 2020 2020 207b 2520 6966 2066           {% if f
-000003b0: 6f72 6c6f 6f70 2e66 6972 7374 2025 7d20  orloop.first %} 
-000003c0: 6163 7469 7665 7b25 2065 6e64 6966 2025  active{% endif %
-000003d0: 7d0a 2020 2020 2020 2020 2020 2220 6461  }.          " da
-000003e0: 7461 2d62 732d 746f 6767 6c65 3d22 7069  ta-bs-toggle="pi
-000003f0: 6c6c 2220 6872 6566 3d22 2374 6162 7b25  ll" href="#tab{%
-00000400: 2063 7963 6c65 2027 3127 2027 3227 2027   cycle '1' '2' '
-00000410: 3327 2027 3427 2027 3527 2025 7d22 3e7b  3' '4' '5' %}">{
-00000420: 7b20 6974 656d 2e74 6974 6c65 207d 7d3c  { item.title }}<
-00000430: 2f61 3e3c 2f6c 693e 0a20 2020 2020 2020  /a></li>.       
-00000440: 2020 207b 2520 656e 6466 6f72 2025 7d0a     {% endfor %}.
-00000450: 2020 2020 2020 2020 3c2f 756c 3e3c 212d          </ul><!-
-00000460: 2d20 456e 6420 5461 6273 202d 2d3e 0a0a  - End Tabs -->..
-00000470: 2020 2020 2020 2020 3c21 2d2d 2054 6162          <!-- Tab
-00000480: 2043 6f6e 7465 6e74 202d 2d3e 0a20 2020   Content -->.   
-00000490: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
-000004a0: 2274 6162 2d63 6f6e 7465 6e74 223e 0a20  "tab-content">. 
-000004b0: 2020 2020 2020 2020 207b 2520 666f 7220           {% for 
-000004c0: 6974 656d 2069 6e20 6162 6f75 7420 257d  item in about %}
-000004d0: 0a20 2020 2020 2020 2020 207b 2520 6966  .          {% if
-000004e0: 2066 6f72 6c6f 6f70 2e66 6972 7374 2025   forloop.first %
-000004f0: 7d0a 2020 2020 2020 2020 2020 3c64 6976  }.          <div
-00000500: 2063 6c61 7373 3d22 7461 622d 7061 6e65   class="tab-pane
-00000510: 2066 6164 6520 7368 6f77 2061 6374 6976   fade show activ
-00000520: 6522 2069 643d 2274 6162 3122 3e0a 2020  e" id="tab1">.  
-00000530: 2020 2020 2020 2020 7b25 2065 6c73 6520          {% else 
-00000540: 257d 0a20 2020 2020 2020 2020 203c 6469  %}.          <di
-00000550: 7620 636c 6173 733d 2274 6162 2d70 616e  v class="tab-pan
-00000560: 6520 6661 6465 2073 686f 7722 2069 643d  e fade show" id=
-00000570: 2274 6162 7b25 2063 7963 6c65 2027 3227  "tab{% cycle '2'
-00000580: 2027 3327 2027 3427 2027 3527 2025 7d22   '3' '4' '5' %}"
-00000590: 3e0a 2020 2020 2020 2020 2020 7b25 2065  >.          {% e
-000005a0: 6e64 6966 2025 7d0a 2020 2020 2020 2020  ndif %}.        
-000005b0: 2020 2020 7b25 2069 6620 6974 656d 2e70      {% if item.p
-000005c0: 5f69 7461 6c69 6320 257d 0a20 2020 2020  _italic %}.     
-000005d0: 2020 2020 2020 203c 7020 636c 6173 733d         <p class=
-000005e0: 2266 7374 2d69 7461 6c69 6322 3e7b 7b20  "fst-italic">{{ 
-000005f0: 6974 656d 2e70 5f69 7461 6c69 6320 7d7d  item.p_italic }}
-00000600: 3c2f 703e 0a20 2020 2020 2020 2020 2020  </p>.           
-00000610: 207b 2520 656e 6469 6620 257d 0a20 2020   {% endif %}.   
-00000620: 2020 2020 2020 2020 207b 2520 666f 7220           {% for 
-00000630: 6368 6b5f 6974 656d 2069 6e20 6974 656d  chk_item in item
-00000640: 2e63 6865 636b 2025 7d0a 2020 2020 2020  .check %}.      
-00000650: 2020 2020 2020 2020 7b25 2069 6620 6368          {% if ch
-00000660: 6b5f 6974 656d 2e68 3420 257d 0a20 2020  k_item.h4 %}.   
-00000670: 2020 2020 2020 2020 2020 203c 6469 7620             <div 
-00000680: 636c 6173 733d 2264 2d66 6c65 7820 616c  class="d-flex al
-00000690: 6967 6e2d 6974 656d 732d 6365 6e74 6572  ign-items-center
-000006a0: 206d 742d 3422 3e0a 2020 2020 2020 2020   mt-4">.        
-000006b0: 2020 2020 2020 2020 3c69 2063 6c61 7373          <i class
-000006c0: 3d22 6269 2062 692d 6368 6563 6b32 223e  ="bi bi-check2">
-000006d0: 3c2f 693e 0a20 2020 2020 2020 2020 2020  </i>.           
-000006e0: 2020 2020 203c 6834 3e7b 7b20 6368 6b5f       <h4>{{ chk_
-000006f0: 6974 656d 2e68 3420 7d7d 3c2f 6834 3e0a  item.h4 }}</h4>.
-00000700: 2020 2020 2020 2020 2020 2020 2020 3c2f                </
-00000710: 6469 763e 0a20 2020 2020 2020 2020 2020  div>.           
-00000720: 2020 207b 2520 656e 6469 6620 257d 0a20     {% endif %}. 
-00000730: 2020 2020 2020 2020 2020 2020 207b 2520               {% 
-00000740: 6966 2063 686b 5f69 7465 6d2e 7020 257d  if chk_item.p %}
-00000750: 0a20 2020 2020 2020 2020 2020 2020 203c  .              <
-00000760: 703e 7b7b 2063 686b 5f69 7465 6d2e 7020  p>{{ chk_item.p 
-00000770: 7d7d 3c2f 703e 0a20 2020 2020 2020 2020  }}</p>.         
-00000780: 2020 2020 207b 2520 656e 6469 6620 257d       {% endif %}
-00000790: 0a20 2020 2020 2020 2020 2020 207b 2520  .            {% 
-000007a0: 656e 6466 6f72 2025 7d0a 2020 2020 2020  endfor %}.      
-000007b0: 2020 2020 3c2f 6469 763e 0a20 2020 2020      </div>.     
-000007c0: 2020 2020 207b 2520 656e 6466 6f72 2025       {% endfor %
-000007d0: 7d0a 2020 2020 2020 2020 3c2f 6469 763e  }.        </div>
-000007e0: 0a20 2020 2020 2020 207b 2520 656e 6461  .        {% enda
-000007f0: 7574 6f65 7363 6170 6520 257d 0a20 2020  utoescape %}.   
-00000800: 2020 203c 2f64 6976 3e0a 2020 2020 3c2f     </div>.    </
-00000810: 6469 763e 0a20 203c 2f64 6976 3e0a 3c2f  div>.  </div>.</
-00000820: 7365 6374 696f 6e3e                      section>
+00000010: 7d0a 0a3c 7365 6374 696f 6e20 6964 3d22  }..<section id="
+00000020: 6665 6174 7572 6573 2220 636c 6173 733d  features" class=
+00000030: 2266 6561 7475 7265 7322 3e0a 2020 3c64  "features">.  <d
+00000040: 6976 2063 6c61 7373 3d22 636f 6e74 6169  iv class="contai
+00000050: 6e65 7222 2064 6174 612d 616f 733d 2266  ner" data-aos="f
+00000060: 6164 652d 7570 223e 0a0a 2020 2020 3c75  ade-up">..    <u
+00000070: 6c20 636c 6173 733d 226e 6176 206e 6176  l class="nav nav
+00000080: 2d74 6162 7320 726f 7720 6779 2d34 2064  -tabs row gy-4 d
+00000090: 2d66 6c65 7822 3e0a 2020 2020 2020 7b25  -flex">.      {%
+000000a0: 2066 6f72 2069 7465 6d20 696e 2066 6561   for item in fea
+000000b0: 7475 7265 7320 257d 0a20 2020 2020 203c  tures %}.      <
+000000c0: 6c69 2063 6c61 7373 3d22 6e61 762d 6974  li class="nav-it
+000000d0: 656d 2063 6f6c 2d36 2063 6f6c 2d6d 642d  em col-6 col-md-
+000000e0: 3420 636f 6c2d 6c67 2d32 223e 0a20 2020  4 col-lg-2">.   
+000000f0: 2020 2020 207b 2520 6966 2066 6f72 6c6f       {% if forlo
+00000100: 6f70 2e66 6972 7374 2025 7d0a 2020 2020  op.first %}.    
+00000110: 2020 2020 3c61 2063 6c61 7373 3d22 6e61      <a class="na
+00000120: 762d 6c69 6e6b 2061 6374 6976 6520 7368  v-link active sh
+00000130: 6f77 2220 6461 7461 2d62 732d 746f 6767  ow" data-bs-togg
+00000140: 6c65 3d22 7461 6222 2064 6174 612d 6273  le="tab" data-bs
+00000150: 2d74 6172 6765 743d 2223 7461 622d 3122  -target="#tab-1"
+00000160: 3e0a 2020 2020 2020 2020 7b25 2065 6c73  >.        {% els
+00000170: 6520 257d 0a20 2020 2020 2020 203c 6120  e %}.        <a 
+00000180: 636c 6173 733d 226e 6176 2d6c 696e 6b22  class="nav-link"
+00000190: 2064 6174 612d 6273 2d74 6f67 676c 653d   data-bs-toggle=
+000001a0: 2274 6162 2220 6461 7461 2d62 732d 7461  "tab" data-bs-ta
+000001b0: 7267 6574 3d22 2374 6162 2d7b 2520 6379  rget="#tab-{% cy
+000001c0: 636c 6520 2732 2720 2733 2720 2734 2720  cle '2' '3' '4' 
+000001d0: 2735 2720 2736 2720 257d 223e 0a20 2020  '5' '6' %}">.   
+000001e0: 2020 2020 207b 2520 656e 6469 6620 257d       {% endif %}
+000001f0: 0a20 2020 2020 2020 2020 203c 6920 636c  .          <i cl
+00000200: 6173 733d 2262 6920 7b7b 2069 7465 6d2e  ass="bi {{ item.
+00000210: 6963 6f6e 207d 7d20 636f 6c6f 722d 7b25  icon }} color-{%
+00000220: 2063 7963 6c65 2027 6379 616e 2720 2769   cycle 'cyan' 'i
+00000230: 6e64 6967 6f27 2027 7465 616c 2720 2772  ndigo' 'teal' 'r
+00000240: 6564 2720 2762 6c75 6527 2027 6f72 616e  ed' 'blue' 'oran
+00000250: 6765 2720 257d 223e 3c2f 693e 0a20 2020  ge' %}"></i>.   
+00000260: 2020 2020 2020 203c 6834 3e7b 7b20 6974         <h4>{{ it
+00000270: 656d 2e74 6974 6c65 207d 7d3c 2f68 343e  em.title }}</h4>
+00000280: 0a20 2020 2020 2020 203c 2f61 3e0a 2020  .        </a>.  
+00000290: 2020 2020 3c2f 6c69 3e0a 2020 2020 2020      </li>.      
+000002a0: 7b25 2065 6e64 666f 7220 257d 0a0a 2020  {% endfor %}..  
+000002b0: 2020 3c2f 756c 3e0a 0a20 2020 203c 6469    </ul>..    <di
+000002c0: 7620 636c 6173 733d 2274 6162 2d63 6f6e  v class="tab-con
+000002d0: 7465 6e74 223e 0a20 2020 2020 207b 2520  tent">.      {% 
+000002e0: 666f 7220 6974 656d 2069 6e20 6665 6174  for item in feat
+000002f0: 7572 6573 2025 7d0a 2020 2020 2020 7b25  ures %}.      {%
+00000300: 2069 6620 666f 726c 6f6f 702e 6669 7273   if forloop.firs
+00000310: 7420 257d 0a20 2020 2020 203c 6469 7620  t %}.      <div 
+00000320: 636c 6173 733d 2274 6162 2d70 616e 6520  class="tab-pane 
+00000330: 6163 7469 7665 2073 686f 7722 2069 643d  active show" id=
+00000340: 2274 6162 2d31 223e 0a20 2020 2020 207b  "tab-1">.      {
+00000350: 2520 656c 7365 2025 7d0a 2020 2020 2020  % else %}.      
+00000360: 3c64 6976 2063 6c61 7373 3d22 7461 622d  <div class="tab-
+00000370: 7061 6e65 2220 6964 3d22 7461 622d 7b25  pane" id="tab-{%
+00000380: 2063 7963 6c65 2027 3227 2027 3327 2027   cycle '2' '3' '
+00000390: 3427 2027 3527 2027 3627 2025 7d22 3e0a  4' '5' '6' %}">.
+000003a0: 2020 2020 2020 7b25 2065 6e64 6966 2025        {% endif %
+000003b0: 7d0a 2020 2020 2020 2020 3c64 6976 2063  }.        <div c
+000003c0: 6c61 7373 3d22 726f 7720 6779 2d34 223e  lass="row gy-4">
+000003d0: 0a20 2020 2020 2020 2020 207b 2520 6966  .          {% if
+000003e0: 2066 6f72 6c6f 6f70 2e66 6972 7374 2025   forloop.first %
+000003f0: 7d0a 2020 2020 2020 2020 2020 3c64 6976  }.          <div
+00000400: 2063 6c61 7373 3d22 636f 6c2d 6c67 2d38   class="col-lg-8
+00000410: 206f 7264 6572 2d32 206f 7264 6572 2d6c   order-2 order-l
+00000420: 672d 3122 2064 6174 612d 616f 733d 2266  g-1" data-aos="f
+00000430: 6164 652d 7570 2220 6461 7461 2d61 6f73  ade-up" data-aos
+00000440: 2d64 656c 6179 3d22 3130 3022 3e0a 2020  -delay="100">.  
+00000450: 2020 2020 2020 2020 7b25 2065 6c73 6520          {% else 
+00000460: 257d 0a20 2020 2020 2020 2020 203c 6469  %}.          <di
+00000470: 7620 636c 6173 733d 2263 6f6c 2d6c 672d  v class="col-lg-
+00000480: 3820 6f72 6465 722d 3220 6f72 6465 722d  8 order-2 order-
+00000490: 6c67 2d31 223e 0a20 2020 2020 2020 2020  lg-1">.         
+000004a0: 207b 2520 656e 6469 6620 257d 0a20 2020   {% endif %}.   
+000004b0: 2020 2020 2020 2020 203c 6833 3e7b 7b20           <h3>{{ 
+000004c0: 6974 656d 2e74 6974 6c65 207d 7d3c 2f68  item.title }}</h
+000004d0: 333e 0a20 2020 2020 2020 2020 2020 203c  3>.            <
+000004e0: 7020 636c 6173 733d 2266 7374 2d69 7461  p class="fst-ita
+000004f0: 6c69 6322 3e0a 2020 2020 2020 2020 2020  lic">.          
+00000500: 2020 2020 7b7b 2069 7465 6d2e 705f 7570      {{ item.p_up
+00000510: 7065 7220 7d7d 0a20 2020 2020 2020 2020  per }}.         
+00000520: 2020 203c 2f70 3e0a 2020 2020 2020 2020     </p>.        
+00000530: 2020 2020 3c75 6c3e 0a20 2020 2020 2020      <ul>.       
+00000540: 2020 2020 2020 207b 2520 666f 7220 6c69         {% for li
+00000550: 2069 6e20 6974 656d 2e6c 6920 257d 0a20   in item.li %}. 
+00000560: 2020 2020 2020 2020 2020 2020 203c 6c69               <li
+00000570: 3e3c 6920 636c 6173 733d 2262 6920 6269  ><i class="bi bi
+00000580: 2d63 6865 636b 2d63 6972 636c 652d 6669  -check-circle-fi
+00000590: 6c6c 223e 3c2f 693e 207b 7b20 6c69 207d  ll"></i> {{ li }
+000005a0: 7d3c 2f6c 693e 0a20 2020 2020 2020 2020  }</li>.         
+000005b0: 2020 2020 207b 2520 656e 6466 6f72 2025       {% endfor %
+000005c0: 7d0a 2020 2020 2020 2020 2020 2020 3c2f  }.            </
+000005d0: 756c 3e0a 2020 2020 2020 2020 2020 2020  ul>.            
+000005e0: 3c70 2063 6c61 7373 3d22 6673 742d 6974  <p class="fst-it
+000005f0: 616c 6963 223e 0a20 2020 2020 2020 2020  alic">.         
+00000600: 2020 2020 207b 7b20 6974 656d 2e70 5f6c       {{ item.p_l
+00000610: 6f77 6572 207d 7d0a 2020 2020 2020 2020  ower }}.        
+00000620: 2020 2020 3c2f 703e 0a20 2020 2020 2020      </p>.       
+00000630: 2020 203c 2f64 6976 3e0a 2020 2020 2020     </div>.      
+00000640: 2020 2020 7b25 2069 6620 666f 726c 6f6f      {% if forloo
+00000650: 702e 6669 7273 7420 257d 0a20 2020 2020  p.first %}.     
+00000660: 2020 2020 203c 6469 7620 636c 6173 733d       <div class=
+00000670: 2263 6f6c 2d6c 672d 3420 6f72 6465 722d  "col-lg-4 order-
+00000680: 3120 6f72 6465 722d 6c67 2d32 2074 6578  1 order-lg-2 tex
+00000690: 742d 6365 6e74 6572 2220 6461 7461 2d61  t-center" data-a
+000006a0: 6f73 3d22 6661 6465 2d75 7022 2064 6174  os="fade-up" dat
+000006b0: 612d 616f 732d 6465 6c61 793d 2232 3030  a-aos-delay="200
+000006c0: 223e 0a20 2020 2020 2020 2020 207b 2520  ">.          {% 
+000006d0: 656c 7365 2025 7d0a 2020 2020 2020 2020  else %}.        
+000006e0: 2020 3c64 6976 2063 6c61 7373 3d22 636f    <div class="co
+000006f0: 6c2d 6c67 2d34 206f 7264 6572 2d31 206f  l-lg-4 order-1 o
+00000700: 7264 6572 2d6c 672d 3220 7465 7874 2d63  rder-lg-2 text-c
+00000710: 656e 7465 7222 3e0a 2020 2020 2020 2020  enter">.        
+00000720: 2020 7b25 2065 6e64 6966 2025 7d0a 2020    {% endif %}.  
+00000730: 2020 2020 2020 2020 2020 3c69 6d67 2073            <img s
+00000740: 7263 3d22 7b25 2073 7461 7469 6320 2769  rc="{% static 'i
+00000750: 6d67 2f27 7c61 6464 3a74 656d 706c 6174  mg/'|add:templat
+00000760: 655f 6e61 6d65 7c61 6464 3a27 2f66 6561  e_name|add:'/fea
+00000770: 7475 7265 732f 277c 6164 643a 6974 656d  tures/'|add:item
+00000780: 2e69 6d61 6765 2025 7d22 2061 6c74 3d22  .image %}" alt="
+00000790: 2220 636c 6173 733d 2269 6d67 2d66 6c75  " class="img-flu
+000007a0: 6964 223e 0a20 2020 2020 2020 2020 203c  id">.          <
+000007b0: 2f64 6976 3e0a 2020 2020 2020 2020 3c2f  /div>.        </
+000007c0: 6469 763e 0a20 2020 2020 203c 2f64 6976  div>.      </div
+000007d0: 3e0a 2020 2020 2020 7b25 2065 6e64 666f  >.      {% endfo
+000007e0: 7220 257d 0a20 2020 203c 2f64 6976 3e0a  r %}.    </div>.
+000007f0: 2020 3c2f 6469 763e 0a3c 2f73 6563 7469    </div>.</secti
+00000800: 6f6e 3e                                  on>
```

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/_contact.html` & `django_herobiz_ds-3.0.0/django_herobiz_ds/templates/herobizds/_contact.html`

 * *Files 4% similar despite different names*

```diff
@@ -53,15 +53,15 @@
               </div><!-- End Info Item -->
 
             </div>
 
           </div>
 
           <div class="col-lg-8">
-            <form action="{% url 'herobizds:home' %}#contact" method="POST" role="form" class="php-email-form  w-100" data-aos="fade-up">
+            <form action="{% url template_name|add:':home' %}#contact" method="POST" role="form" class="php-email-form  w-100" data-aos="fade-up">
               {% csrf_token %}
               <div class="row">
                 <div class="col-md-6 form-group">
                   {{ form.name }}
                 </div>
                 <div class="col-md-6 form-group mt-3 mt-md-0">
                   {{ form.email }}
```

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/_cta.html` & `django_herobiz_ds-3.0.0/django_herobiz_ds/templates/herobizds/_cta.html`

 * *Files 10% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         </div>
         </div>
         {% endautoescape %}
       </div>
 
       <div class="col-lg-4 col-md-6 order-first order-md-last d-flex align-items-center">
         <div class="img">
-          <img src="{% static 'img/herobizds/'|add:cta_image %}" alt="" class="img-fluid">
+          <img src="{% static 'img/'|add:template_name|add:'/'|add:cta_image %}" alt="" class="img-fluid">
         </div>
       </div>
 
     </div>
 
   </div>
 </section>
```

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/_faq.html` & `django_herobiz_ds-3.0.0/django_herobiz_ds/templates/herobizds/_faq.html`

 * *Files 2% similar despite different names*

```diff
@@ -31,11 +31,11 @@
                 {% endautoescape %}
               </div>
             </div>
           </div>
           {% endfor %}
         </div>
       </div>
-      <div class="col-lg-5 align-items-stretch order-1 order-lg-2 img" style='background-image: url("{% static 'herobizds/img/faq.jpg' %}");'>&nbsp;</div>
+      <div class="col-lg-5 align-items-stretch order-1 order-lg-2 img" style='background-image: url("{% static template_name|add:'/img/faq.jpg' %}");'>&nbsp;</div>
     </div>
   </div>
 </section>
```

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/_featured-services.html` & `django_herobiz_ds-3.0.0/django_herobiz_ds/templates/herobizds/_featured-services.html`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/_hero-animated.html` & `django_herobiz_ds-3.0.0/django_herobiz_ds/templates/herobizds/_hero-animated.html`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 {% load static %}
 <style>
   .hero-animated {
   width: 100%;
   min-height: 50vh;
-  background: url("{% static 'herobizds/img/hero-bg.png' %}") center center;
+  background: url("{% static template_name|add:'/img/hero-bg.png' %}") center center;
   background-size: cover;
   position: relative;
   padding: 120px 0 60px;
 }
 
 </style>
 <section id="hero-animated" class="hero-animated d-flex align-items-center">
   <div class="container d-flex flex-column justify-content-center align-items-center text-center position-relative" data-aos="zoom-out">
-    <img src="{% static 'img/herobizds/hero-animated.svg' %}" class="img-fluid animated">
+    <img src="{% static 'img/'|add:template_name|add:'/hero-animated.svg' %}" class="img-fluid animated">
     {% autoescape off %}
     <h2>{{ hero.title }}</h2>
     <p>{{ hero.slogan }}</p>
     {% endautoescape %}
     <div class="d-flex">
       <a href="{{ hero.btn.link }}" class="btn-get-started scrollto">{{ hero.btn.title }}</a>
       <a href="{{ hero.video_link }}" class="glightbox btn-watch-video d-flex align-items-center"><i class="bi bi-play-circle"></i><span>Watch Video</span></a>
```

#### html2text {}

```diff
@@ -1,7 +1,8 @@
 {% load static %}
-[{% static 'img/herobizds/hero-animated.svg' %}]{% autoescape off %}
+[{% static 'img/'|add:template_name|add:'/hero-animated.svg' %}]{% autoescape
+off %}
 ********** {{{{ hheerroo..ttiittllee }}}} **********
 {{ hero.slogan }}
 {% endautoescape %}
 _{_{_ _h_e_r_o_._b_t_n_._t_i_t_l_e_ _}_}
 _W_a_t_c_h_ _V_i_d_e_o
```

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/_hero-carousel.html` & `django_herobiz_ds-3.0.0/django_herobiz_ds/templates/herobizds/_hero-carousel.html`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 {% load static %}
 
 <style>
   .hero {
   width: 100%;
   padding: 0;
   background: #000000;
-  background: url("{% static 'herobizds/img/hero-bg.png' %}") center center;
+  background: url("{% static template_name|add:'/img/hero-bg.png' %}") center center;
   background-size: cover;
   background-position: center;
   background-repeat: no-repeat;
   position: relative;
   display: flex;
   flex-direction: column;
   justify-content: center;
@@ -26,15 +26,15 @@
       {% else %}
       <div class="carousel-item">
       {% endif %}
 
         <div class="container">
           <div class="row justify-content-center gy-6">
             <div class="col-lg-5 col-md-8">
-              <img src="{% static 'img/herobizds/hero-carousel/'|add:item.image' %}" alt="" class="img-fluid img">
+              <img src="{% static 'img/'|add:template_name|add:'/hero-carousel/'|add:item.image' %}" alt="" class="img-fluid img">
             </div>
 
             <div class="col-lg-9 text-center">
               {% autoescape off %}
               <h2>{{ item.title }}</h2>
               <p>{{ item.slogan }}</p>
               {% endautoescape %}
```

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/_hero-fullscreen.html` & `django_herobiz_ds-3.0.0/django_herobiz_ds/templates/herobizds/_hero-fullscreen.html`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 {% load static %}
 
 <style>
   .hero-fullscreen {
   width: 100%;
   min-height: 100vh;
-  background: url("{% static 'img/herobizds/hero-fullscreen-bg.jpg' %}") center center;
+  background: url("{% static 'img/'|add:template_name|add:'/hero-fullscreen-bg.jpg' %}") center center;
   background-size: cover;
   position: relative;
   padding: 120px 0 60px;
 }
 </style>
 
 <section id="hero-fullscreen" class="hero-fullscreen d-flex align-items-center">
```

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/_hero-static.html` & `django_herobiz_ds-3.0.0/django_herobiz_ds/templates/herobizds/_hero-static.html`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 {% load static %}
 <style>
   .hero-static {
   width: 100%;
   min-height: 50vh;
-  background: url("{% static 'herobizds/img/hero-bg.png' %}") center center;
+  background: url("{% static template_name|add:'/img/hero-bg.png' %}") center center;
   background-size: cover;
   position: relative;
   padding: 120px 0 60px;
 }
 </style>
 
 <section id="hero-static" class="hero-static d-flex align-items-center">
```

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/_onfocus.html` & `django_herobiz_ds-3.0.0/django_herobiz_ds/templates/herobizds/_onfocus.html`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 {% load static %}
 <style>
 .onfocus .video-play {
   min-height: 400px;
-  background: linear-gradient(rgba(0, 0, 0, 0.4), rgba(0, 0, 0, 0.7)), url("{% static 'img/herobizds/onfocus-video-bg.jpg' %}") center center;
+  background: linear-gradient(rgba(0, 0, 0, 0.4), rgba(0, 0, 0, 0.7)), url("{% static 'img/'|add:template_name|add:'/onfocus-video-bg.jpg' %}") center center;
   background-size: cover;
 }
 
 .onfocus .content {
-  background: linear-gradient(rgba(72, 86, 100, 0.5), rgba(72, 86, 100, 0.8)), url("{% static 'herobizds/img/onfocus-content-bg.jpg' %}") center center;
+  background: linear-gradient(rgba(72, 86, 100, 0.5), rgba(72, 86, 100, 0.8)), url("{% static ''|add:template_name|add:'/img/onfocus-content-bg.jpg' %}") center center;
   background-size: cover;
   color: rgba(255, 255, 255, 0.8);
   padding: 40px;
 }
 
 </style>
 <section id="onfocus" class="onfocus">
```

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/_portfolio.html` & `django_herobiz_ds-3.0.0/django_herobiz_ds/templates/herobizds/_portfolio.html`

 * *Files 5% similar despite different names*

```diff
@@ -25,15 +25,15 @@
       <div class="row g-0 portfolio-container">
         {% for item in items.all %}
         <div class="col-xl-3 col-lg-4 col-md-6 portfolio-item filter-{{ item.filter }}">
           <img src="{{ item.image1.url }}" class="img-fluid" alt="">
           <div class="portfolio-info">
             <h4>{{ item.title }}</h4>
             <a href="{{ item.image1.url }}" title="{{ item.title }}" data-gallery="portfolio-gallery" class="glightbox preview-link"><i class="bi bi-zoom-in"></i></a>
-            <a href="{% url 'herobizds:details' item.id %}" title="More Details" class="details-link" target="_blank"><i class="bi bi-link-45deg"></i></a>
+            <a href="{% url template_name|add:':details' item.id %}" title="More Details" class="details-link" target="_blank"><i class="bi bi-link-45deg"></i></a>
           </div>
         </div>
         {% endfor %}
       </div><!-- End Portfolio Container -->
     </div>
   </div>
 </section>
```

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/_pricing.html` & `django_herobiz_ds-3.0.0/django_herobiz_ds/templates/herobizds/_pricing.html`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 {% load static %}
 
 <style>
 .pricing .pricing-header {
-  background: linear-gradient(rgba(72, 86, 100, 0.9), rgba(72, 86, 100, 0.9)), url("{% static 'herobizds/img/pricing-bg.jpg' %}") center center;
+  background: linear-gradient(rgba(72, 86, 100, 0.9), rgba(72, 86, 100, 0.9)), url("{% static template_name|add:'/img/pricing-bg.jpg' %}") center center;
   background-size: cover;
   text-align: center;
   padding: 40px;
   margin: -60px -40px 0;
 }
 </style>
 
@@ -17,19 +17,15 @@
       <h2>{{ pricing_title }}</h2>
       <p>{{ pricing_subtitle }}</p>
     </div>
 
     <div class="row gy-4">
       {% for item in pricing %}
       <div class="col-lg-4" data-aos="zoom-in" data-aos-delay="{% cycle '200' '400' '600' %}">
-        {% if item.featured %}
-        <div class="pricing-item featured">
-        {% else %}
-        <div class="pricing-item">
-        {% endif %}
+        <div class="pricing-item {% if item.featured %}featured{% endif %}">
           <div class="pricing-header">
             <h3>{{ item.title }}</h3>
             <h4><sup>₩</sup>{{ item.price }}<span> / month</span></h4>
           </div>
           <ul>
             {% for pcontent in item.pcontents %}
             <li><i class="bi bi-dot"></i> <span>{{ pcontent }}</span></li>
```

#### html2text {}

```diff
@@ -1,14 +1,11 @@
 {% load static %}
 ********** {{{{ pprriicciinngg__ttiittllee }}}} **********
 {{ pricing_subtitle }}
 {% for item in pricing %}
-{% if item.featured %}
-{% else %}
-{% endif %}
 ******** {{{{ iitteemm..ttiittllee }}}} ********
 ****** ?â??©{{{{ iitteemm..pprriiccee }}}} // mmoonntthh ******
     * {% for pcontent in item.pcontents %}
     * {{ pcontent }}
     * {% endfor %} {% for ncontent in item.ncontents %}
     * {{ ncontent }}
     * {% endfor %}
```

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/_recent-blog-posts.html` & `django_herobiz_ds-3.0.0/django_herobiz_ds/templates/herobizds/_recent-blog-posts.html`

 * *Files 14% similar despite different names*

```diff
@@ -7,21 +7,25 @@
       <p>{{ blog_subtitle }}</p>
     </div>
 
     <div class="row">
       {% for item in top3 %}
       <div class="col-lg-4" data-aos="fade-up" data-aos-delay="{% cycle '200' '400' '600' %}">
         <div class="post-box">
-          <div class="post-img"><img src="{{ item.thumbnail.url }}" class="img-fluid" alt=""></div>
+          <div class="post-img">
+            <div class="ratio ratio-4x3">
+              <img src="{{ item.thumbnail.url }}" class="img-fluid" alt="">
+            </div>
+          </div>
           <div class="meta">
             <span class="post-date">{{ item.updated_on | date:"D, F d"}}</span>
             <span class="post-author"> / {{ item.author.last_name}} {{ item.author.first_name }}</span>
           </div>
           <h3 class="post-title">{{ item.title }}</h3>
           <p>{{ item.content | truncatechars:200 }}</p>
-          <a href="{% url 'herobizds:post_detail' item.slug  %}" class="readmore stretched-link"><span>Read More</span><i class="bi bi-arrow-right"></i></a>
+          <a href="{% url template_name|add:':post_detail' item.slug  %}" class="readmore stretched-link"><span>Read More</span><i class="bi bi-arrow-right"></i></a>
         </div>
       </div>
       {% endfor %}
     </div>
   </div>
 </section>
```

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/_services.html` & `django_herobiz_ds-3.0.0/django_herobiz_ds/templates/herobizds/_services.html`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     </div>
 
     <div class="row gy-5">
       {% for item in services %}
       <div class="col-xl-4 col-md-6" data-aos="zoom-in" data-aos-delay="{% cycle '200' '300' '400' '500' '600' '700' %}">
         <div class="service-item">
           <div class="img">
-            <img src="{% static 'img/herobizds/services/'|add:item.image %}" class="img-fluid" alt="">
+            <img src="{% static 'img/'|add:template_name|add:'/services/'|add:item.image %}" class="img-fluid" alt="">
           </div>
           <div class="details position-relative">
             <div class="icon">
               <i class="bi {{ item.icon }}"></i>
             </div>
             <a href="#" class="stretched-link">
               <h3>{{ item.h3 }}</h3>
```

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/_sidebar.html` & `django_herobiz_ds-3.0.0/django_herobiz_ds/templates/herobizds/_sidebar.html`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 {% load herobizds_tags %}
 {% load static %}
 
 <div class="sidebar">
 
   <div class="sidebar-item search-form">
     <h3 class="sidebar-title">Search</h3>
-    <form action="{% url 'herobizds:search_result' %}" class="mt-3" method="get">
+    <form action="{% url template_name|add:':search_result' %}" class="mt-3" method="get">
       {{ form.q }}
       <button type="submit"><i class="bi bi-search"></i></button>
     </form>
   </div><!-- End sidebar search formn-->
 
   <div class="sidebar-item categories">
     <h3 class="sidebar-title">Categories</h3>
     <ul class="mt-3">
       {% for category_int, name, count in category %}
-      <li><a href="{% url 'herobizds:category' category_int %}">{{ name }} <span>({{ count }})</span></a></li>
+      <li><a href="{% url template_name|add:':category' category_int %}">{{ name }} <span>({{ count }})</span></a></li>
       {% endfor %}
     </ul>
   </div><!-- End sidebar categories-->
 
   <div class="sidebar-item recent-posts">
     <h3 class="sidebar-title">Recent Posts</h3>
 
@@ -28,26 +28,26 @@
       {% if forloop.first %}
       <div class="post-item mt-3">
       {% else %}
       <div class="post-item">
       {% endif%}
         <img src="{{ l.thumbnail.url }}" alt="" class="flex-shrink-0">
         <div>
-          <h4><a href="{% url 'herobizds:post_detail' l.slug %}">{{ l.title }}</a></h4>
+          <h4><a href="{% url template_name|add:':post_detail' l.slug %}">{{ l.title }}</a></h4>
           <time datetime="{{ l.updated_on | date:'Y-m-d'}}">{{ l.updated_on | date:"M d, Y"}}</time>
         </div>
       </div><!-- End recent post item-->
       {% endfor %}
     </div>
 
   </div><!-- End sidebar recent posts-->
 
   <div class="sidebar-item tags">
     <h3 class="sidebar-title">Tags</h3>
     <ul class="mt-3">
       {% for tag in all_tags %}
-      <li><a href="{% url 'herobizds:search_tag' tag %}">{{ tag }}</a></li>
+      <li><a href="{% url template_name|add:':search_tag' tag %}">{{ tag }}</a></li>
       {% endfor %}
     </ul>
   </div><!-- End sidebar tags-->
 
 </div>
```

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/_team.html` & `django_herobiz_ds-3.0.0/django_herobiz_ds/templates/herobizds/_team.html`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
     <div class="row gy-5">
       {% for member in team %}
       <div class="col-xl-4 col-md-6 d-flex" data-aos="zoom-in" data-aos-delay="{% cycle '200' '400' '600' '800' %}">
         <div class="team-member">
           <div class="member-img">
             {% cycle 'member1' 'member2' 'member3' 'member4' 'member5' 'member6' as member_dir silent %}
-            <img src="{% static 'img/herobizds/team/'|add:member_dir|add:'/profile.jpg' %}" class="img-fluid" alt="">
+            <img src="{% static 'img/'|add:template_name|add:'/team/'|add:member_dir|add:'/profile.jpg' %}" class="img-fluid" alt="">
           </div>
           <div class="member-info">
             <div class="social">
               {% if member.social.twitter %}
               <a href=""><i class="bi bi-twitter"></i></a>
               {% endif %}
               {% if member.social.facebook %}
```

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/_testimonials.html` & `django_herobiz_ds-3.0.0/django_herobiz_ds/templates/herobizds/_testimonials.html`

 * *Files 5% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 {% load static %}
 <style>
   .testimonials {
   padding: 80px 0;
-  background: url("{% static 'img/herobizds/testimonials-bg.jpg' %}") no-repeat;
+  background: url("{% static 'img/'|add:template_name|add:'/testimonials-bg.jpg' %}") no-repeat;
   background-position: center center;
   background-size: cover;
   position: relative;
 }
 </style>
 
 <section id="testimonials" class="testimonials">
   <div class="container" data-aos="fade-up">
 
     <div class="testimonials-slider swiper">
       <div class="swiper-wrapper">
         {% for item in testimonials %}
         <div class="swiper-slide">
           <div class="testimonial-item">
-            <img src="{% static 'img/herobizds/testimonials/'|add:item.photo %}" class="testimonial-img" alt="">
+            <img src="{% static 'img/'|add:template_name|add:'/testimonials/'|add:item.photo %}" class="testimonial-img" alt="">
             <h3>{{ item.name }}</h3>
             {% autoescape off %}
             <h4>{{ item.job }}</h4>
             {% endautoescape %}
             <div class="stars">
               <i class="bi bi-star-fill"></i><i class="bi bi-star-fill"></i><i class="bi bi-star-fill"></i><i class="bi bi-star-fill"></i><i class="bi bi-star-fill"></i>
             </div>
```

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/blog-details.html` & `django_herobiz_ds-3.0.0/django_herobiz_ds/templates/herobizds/blog-details.html`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-{% extends "herobizds/index.html" %}
+{% extends template_name|add:'/index.html' %}
 {% load static %}
 {% load herobizds_tags %}
 {% load markdownify %}
 
 {% block content %}
   <main id="main">
-    <!-- ======= Breadcrumbs ======= -->{% include 'herobizds/breadcrumb.html' %}<!-- End Breadcrumbs -->
+    <!-- ======= Breadcrumbs ======= -->{% include template_name|add:'/breadcrumb.html' %}<!-- End Breadcrumbs -->
 
     <!-- ======= Blog Details Section ======= -->
     <section id="blog" class="blog">
       <div class="container" data-aos="fade-up">
         <div class="row g-5">
           <div class="col-lg-8">
             <article class="blog-details">
@@ -17,42 +17,42 @@
                 <img src="{{ object.thumbnail.url }}" alt="" class="img-fluid">
               </div>
 
               <h2 class="title">{{ object.title }}</h2>
 
               <div class="meta-top">
                 <ul>
-                  <li class="d-flex align-items-center"><i class="bi bi-person"></i> <a href="{% url 'herobizds:post_detail' object.slug %}">{{ object.author.last_name }} {{ object.author.first_name }}</a></li>
-                  <li class="d-flex align-items-center"><i class="bi bi-clock"></i> <a href="{% url 'herobizds:post_detail' object.slug %}"><time datetime="{{ object.updated_on | date:'Y-m-d' }}">{{ object.updated_on | date:"M d, Y" }}</time></a></li>
-                  <!-- <li class="d-flex align-items-center"><i class="bi bi-chat-dots"></i> <a href="{% url 'herobizds:post_detail' object.slug %}">12 Comments</a></li> -->
+                  <li class="d-flex align-items-center"><i class="bi bi-person"></i> <a href="{% url template_name|add:':post_detail' object.slug %}">{{ object.author.last_name }} {{ object.author.first_name }}</a></li>
+                  <li class="d-flex align-items-center"><i class="bi bi-clock"></i> <a href="{% url template_name|add:':post_detail' object.slug %}"><time datetime="{{ object.updated_on | date:'Y-m-d' }}">{{ object.updated_on | date:"M d, Y" }}</time></a></li>
+                  <!-- <li class="d-flex align-items-center"><i class="bi bi-chat-dots"></i> <a href="{% url template_name|add:':post_detail' object.slug %}">12 Comments</a></li> -->
                 </ul>
               </div><!-- End meta top -->
 
               <div class="content">
                 {{ object.content | markdownify }}
               </div><!-- End post content -->
 
               <div class="meta-bottom">
                 <i class="bi bi-folder"></i>
                 <ul class="cats">
-                  <li><a href="{% url 'herobizds:category' object.category %}">{{ category_name }}</a></li>
+                  <li><a href="{% url template_name|add:':category' object.category %}">{{ category_name }}</a></li>
                 </ul>
 
                 <i class="bi bi-tags"></i>
                 <ul class="tags">
                   {% for tag in object.tags.all %}
-                  <li><a href="{% url 'herobizds:search_tag' tag %}">{{ tag }}</a></li>
+                  <li><a href="{% url template_name|add:':search_tag' tag %}">{{ tag }}</a></li>
                   {% endfor %}
                 </ul>
               </div><!-- End meta bottom -->
 
             </article><!-- End blog post -->
 
             <div class="post-author d-flex align-items-center">
-              <img src="{% static 'img/herobizds/blog-author.jpg' %}" class="rounded-circle flex-shrink-0" alt="">
+              <img src="{% static 'img/'|add:template_name|add:'/blog-author.jpg' %}" class="rounded-circle flex-shrink-0" alt="">
               <div>
                 <h4>{{ author.name }}</h4>
                 <div class="social-links">
                   {% if author.social.twitter %}
                   <a href="{{ author.social.twitter }}"><i class="bi bi-twitter"></i></a>
                   {% endif %}
                   {% if author.social.facebook %}
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-{% extends "herobizds/index.html" %} {% load static %} {% load herobizds_tags
-%} {% load markdownify %} {% block content %} {% include 'herobizds/
-breadcrumb.html' %}
+{% extends template_name|add:'/index.html' %} {% load static %} {% load
+herobizds_tags %} {% load markdownify %} {% block content %} {% include
+template_name|add:'/breadcrumb.html' %}
 ********** {{{{ oobbjjeecctt..ttiittllee }}}} **********
     * _{_{_ _o_b_j_e_c_t_._a_u_t_h_o_r_._l_a_s_t___n_a_m_e_ _}_}_ _{_{_ _o_b_j_e_c_t_._a_u_t_h_o_r_._f_i_r_s_t___n_a_m_e_ _}_}
     * _{_{_ _o_b_j_e_c_t_._u_p_d_a_t_e_d___o_n_ _|_ _d_a_t_e_:_"_M_ _d_,_ _Y_"_ _}_}
 {{ object.content | markdownify }}
     * _{_{_ _c_a_t_e_g_o_r_y___n_a_m_e_ _}_}
     * {% for tag in object.tags.all %}
     * _{_{_ _t_a_g_ _}_}
```

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/blog.html` & `django_herobiz_ds-3.0.0/django_herobiz_ds/templates/herobizds/blog.html`

 * *Files 17% similar despite different names*

```diff
@@ -1,45 +1,47 @@
-{% extends "herobizds/index.html" %}
+{% extends template_name|add:'/index.html' %}
 {% load static %}
 {% load herobizds_tags %}
 {% load markdownify %}
 
 {% block content %}
 <main id="main">
-  <!-- ======= Breadcrumbs ======= -->{% include 'herobizds/breadcrumb.html' %}<!-- End Breadcrumbs -->
+  <!-- ======= Breadcrumbs ======= -->{% include template_name|add:'/breadcrumb.html' %}<!-- End Breadcrumbs -->
 
   <!-- ======= Blog Section ======= -->
   <section id="blog" class="blog">
     <div class="container" data-aos="fade-up">
       <div class="row g-5">
         <div class="col-lg-8">
           <div class="row gy-4 posts-list">
             {% for item in page_obj %}
             <div class="col-lg-6">
               <article class="d-flex flex-column">
                 <div class="post-img">
-                  <img src="{{ item.thumbnail.url }}" alt="" class="img-fluid">
+                  <div class="ratio ratio-16x9">
+                    <img src="{{ item.thumbnail.url }}" alt="" class="img-fluid">
+                  </div>
                 </div>
                 <h2 class="title">
-                  <a href="{% url 'herobizds:post_detail' item.slug %}">{{ item.title }}</a>
+                  <a href="{% url template_name|add:':post_detail' item.slug %}">{{ item.title }}</a>
                 </h2>
                 <div class="meta-top">
                   <ul>
-                    <li class="d-flex align-items-center"><i class="bi bi-person"></i> <a href="{% url 'herobizds:post_detail' item.slug %}">{{ item.author.last_name }} {{ item.author.first_name }}</a></li>
-                    <li class="d-flex align-items-center"><i class="bi bi-clock"></i> <a href="{% url 'herobizds:post_detail' item.slug %}"><time datetime="{{ item.updated_on | date:'Y-m-d' }}">{{ item.updated_on | date:"M d, Y" }}</time></a></li>
-                    <!-- <li class="d-flex align-items-center"><i class="bi bi-chat-dots"></i> <a href="{% url 'herobizds:post_detail' item.slug %}">12 Comments</a></li> -->
+                    <li class="d-flex align-items-center"><i class="bi bi-person"></i> <a href="{% url template_name|add:':post_detail' item.slug %}">{{ item.author.last_name }} {{ item.author.first_name }}</a></li>
+                    <li class="d-flex align-items-center"><i class="bi bi-clock"></i> <a href="{% url template_name|add:':post_detail' item.slug %}"><time datetime="{{ item.updated_on | date:'Y-m-d' }}">{{ item.updated_on | date:"M d, Y" }}</time></a></li>
+                    <!-- <li class="d-flex align-items-center"><i class="bi bi-chat-dots"></i> <a href="{% url template_name|add:':post_detail' item.slug %}">12 Comments</a></li> -->
                   </ul>
                 </div>
                 <div class="content">
                   <p>
                     {{ item.content | markdownify | striptags | truncatechars:100 }}
                   </p>
                 </div>
                 <div class="read-more mt-auto align-self-end">
-                  <a href="{% url 'herobizds:post_detail' item.slug %}">Read More</a>
+                  <a href="{% url template_name|add:':post_detail' item.slug %}">Read More</a>
                 </div>
               </article>
             </div><!-- End post list item -->
             {% endfor %}
           </div><!-- End blog posts list -->
 
           {% if is_paginated %}
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-{% extends "herobizds/index.html" %} {% load static %} {% load herobizds_tags
-%} {% load markdownify %} {% block content %} {% include 'herobizds/
-breadcrumb.html' %}
+{% extends template_name|add:'/index.html' %} {% load static %} {% load
+herobizds_tags %} {% load markdownify %} {% block content %} {% include
+template_name|add:'/breadcrumb.html' %}
 {% for item in page_obj %}
 ********** _{{_{{_ _ii_tt_ee_mm_.._tt_ii_tt_ll_ee_ _}}_}} **********
     * _{_{_ _i_t_e_m_._a_u_t_h_o_r_._l_a_s_t___n_a_m_e_ _}_}_ _{_{_ _i_t_e_m_._a_u_t_h_o_r_._f_i_r_s_t___n_a_m_e_ _}_}
     * _{_{_ _i_t_e_m_._u_p_d_a_t_e_d___o_n_ _|_ _d_a_t_e_:_"_M_ _d_,_ _Y_"_ _}_}
 {{ item.content | markdownify | striptags | truncatechars:100 }}
 _R_e_a_d_ _M_o_r_e
 {% endfor %}
```

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/footer.html` & `django_herobiz_ds-3.0.0/django_herobiz_ds/templates/herobizds/footer.html`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/forms/contact.php` & `django_herobiz_ds-3.0.0/django_herobiz_ds/templates/herobizds/forms/contact.php`

 * *Files identical despite different names*

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/header.html` & `django_herobiz_ds-3.0.0/django_herobiz_ds/templates/herobizds/header.html`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 {% load static %}
 {% load django_utilsds_tags %}
 
 <header id="header" class="header fixed-top" data-scrollto-offset="0">
   <div class="container-fluid d-flex align-items-center justify-content-between">
-    <a href="{% url 'herobizds:home' %}" class="logo d-flex align-items-center scrollto me-auto me-lg-0">
+    <a href="{% url template_name|add:':home' %}" class="logo d-flex align-items-center scrollto me-auto me-lg-0">
       {% if use_logo %}
-      <img src="{% static 'img/herobizds/logo.png' %}" alt="">
+      <img src="{% static 'img/'|add:template_name|add:'/logo.png' %}" alt="">
       {% else %}
       <h1>{{ logo_text }}<span>.</span></h1>
       {% endif %}
     </a>
 
     <nav id="navbar" class="navbar">
       <ul>
         <!-- 메뉴 -->
         {% for component, etc, title, is_show in components %}
           {% if is_show %}
             {% if component == 'direct_link' %}
               <li><a class="nav-link scrollto" href="{{ etc }}">{{ title }}</a></li>
             {% else %}
-              <li><a class="nav-link scrollto" href="{% url 'herobizds:home' %}#{{ component | underscore_to_hyphen }}">{{ title }}</a></li>
+              <li><a class="nav-link scrollto" href="{% url template_name|add:':home' %}#{{ component | underscore_to_hyphen }}">{{ title }}</a></li>
             {% endif %}
           {% endif %}
         {% endfor %}
       </ul>
       <i class="bi bi-list mobile-nav-toggle d-none"></i>
     </nav><!-- .navbar -->
     {% for component, is_use, _, _ in components %}
```

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/index.html` & `django_herobiz_ds-3.0.0/django_herobiz_ds/templates/herobizds/index.html`

 * *Files 14% similar despite different names*

```diff
@@ -4,40 +4,39 @@
 {% load django_modalds_tags %}
 {% load django_analyticsds_tags %}
 
 <!DOCTYPE html>
 <html lang="en">
 
 <head>
-  <!-- ======= SEO ======= -->{% include 'herobizds/seo.html' %}<!-- End SEO -->
+  <!-- ======= SEO ======= -->{% seo %}<!-- End SEO -->
 
   <!-- Vendor CSS Files -->
   <link rel="stylesheet"
-        href="{% static 'herobizds/vendor/bootstrap/css/bootstrap.min.css' %}" crossorigin="anonymous">
-  <link rel="stylesheet" href="{% static 'herobizds/vendor/bootstrap-icons/bootstrap-icons.min.css' %}">
-  <link href="{% static 'herobizds/vendor/aos/aos.css' %}" rel="stylesheet">
-  <link href="{% static 'herobizds/vendor/glightbox/css/glightbox.min.css' %}" rel="stylesheet">
-  <link href="{% static 'herobizds/vendor/swiper/swiper-bundle.min.css' %}" rel="stylesheet">
+        href="{% static template_name|add:'/vendor/bootstrap/css/bootstrap.min.css' %}" crossorigin="anonymous">
+  <link rel="stylesheet" href="{% static template_name|add:'/vendor/bootstrap-icons/bootstrap-icons.min.css' %}">
+  <link href="{% static template_name|add:'/vendor/aos/aos.css' %}" rel="stylesheet">
+  <link href="{% static template_name|add:'/vendor/glightbox/css/glightbox.min.css' %}" rel="stylesheet">
+  <link href="{% static template_name|add:'/vendor/swiper/swiper-bundle.min.css' %}" rel="stylesheet">
 
   <!-- Variables CSS Files. Uncomment your preferred color scheme -->
-  <link href="{% static 'herobizds/css/variables'|add:color|add:'.css' %}" rel="stylesheet">
-  <!-- <link href="{% static 'herobizds/css/variables-blue.css' %}" rel="stylesheet"> -->
-  <!-- <link href="{% static 'herobizds/css/variables-green.css' %}" rel="stylesheet"> -->
-  <!-- <link href="{% static 'herobizds/css/variables-orange.css' %}" rel="stylesheet"> -->
-  <!-- <link href="{% static 'herobizds/css/variables-purple.css' %}" rel="stylesheet"> -->
-  <!-- <link href="{% static 'herobizds/css/variables-red.css' %}" rel="stylesheet"> -->
-  <!-- <link href="{% static 'herobizds/css/variables-pink.css' %}" rel="stylesheet"> -->
+  <link href="{% static template_name|add:'/css/variables'|add:color|add:'.css' %}" rel="stylesheet">
+  <!-- <link href="{% static template_name|add:'/css/variables-blue.css' %}" rel="stylesheet"> -->
+  <!-- <link href="{% static template_name|add:'/css/variables-green.css' %}" rel="stylesheet"> -->
+  <!-- <link href="{% static template_name|add:'/css/variables-orange.css' %}" rel="stylesheet"> -->
+  <!-- <link href="{% static template_name|add:'/css/variables-purple.css' %}" rel="stylesheet"> -->
+  <!-- <link href="{% static template_name|add:'/css/variables-red.css' %}" rel="stylesheet"> -->
+  <!-- <link href="{% static template_name|add:'/css/variables-pink.css' %}" rel="stylesheet"> -->
 
   <!-- Template Main CSS File -->
-  <link href="{% static 'herobizds/css/main.css' %}" rel="stylesheet">
-
+  <link href="{% static template_name|add:'/css/main.css' %}" rel="stylesheet">
 </head>
 
 <body>
-  <!-- ======= Header ======= -->{% include 'herobizds/header.html' %}<!-- End Header -->
+  <!-- ======= Header ======= -->{% header %}<!-- End Header -->
   {% block content %}
   <!-- ======= Hero Section ======= -->{% hero %}<!-- End Hero -->
   <main id="main">
     {% show_calendar %}
     {% show_modal %}
     {% make_analytics %}
 
@@ -73,26 +72,26 @@
           <!-- ======= Contact Section ======= -->{% contact %}<!-- End Contact Section -->
         {% endif %}
       {% endif %}
     {% endfor %}
   </main><!-- End #main -->
   {% endblock content %}
 
-  <!-- ======= Footer ======= -->{% include 'herobizds/footer.html' %}<!-- End Footer -->
+  <!-- ======= Footer ======= -->{% footer %}<!-- End Footer -->
 
   <a href="#" class="scroll-top d-flex align-items-center justify-content-center"><i class="bi bi-arrow-up-short"></i></a>
 
   <div id="preloader"></div>
 
   <!-- Vendor JS Files -->
-  <script src="{% static 'herobizds/vendor/bootstrap/js/bootstrap.bundle.min.js' %}"
+  <script src="{% static template_name|add:'/vendor/bootstrap/js/bootstrap.bundle.min.js' %}"
           crossorigin="anonymous"></script>
-  <script src="{% static 'herobizds/vendor/aos/aos.js' %}"></script>
-  <script src="{% static 'herobizds/vendor/glightbox/js/glightbox.min.js' %}"></script>
-  <script src="{% static 'herobizds/vendor/isotope-layout/isotope.pkgd.min.js' %}"></script>
-  <script src="{% static 'herobizds/vendor/swiper/swiper-bundle.min.js' %}"></script>
-  <!-- <script src="{% static 'herobizds/vendor/php-email-form/validate.js' %}"></script> -->
+  <script src="{% static template_name|add:'/vendor/aos/aos.js' %}"></script>
+  <script src="{% static template_name|add:'/vendor/glightbox/js/glightbox.min.js' %}"></script>
+  <script src="{% static template_name|add:'/vendor/isotope-layout/isotope.pkgd.min.js' %}"></script>
+  <script src="{% static template_name|add:'/vendor/swiper/swiper-bundle.min.js' %}"></script>
+  <!-- <script src="{% static template_name|add:'/vendor/php-email-form/validate.js' %}"></script> -->
 
   <!-- Template Main JS File -->
-  <script src="{% static 'herobizds/js/main.js' %}"></script>
+  <script src="{% static template_name|add:'/js/main.js' %}"></script>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
 {% load static %} {% load herobizds_tags %} {% load django_calendards_tags %}
 {% load django_modalds_tags %} {% load django_analyticsds_tags %}
-{% include 'herobizds/seo.html' %}
-{% include 'herobizds/header.html' %} {% block content %} {% hero %} {%
-show_calendar %} {% show_modal %} {% make_analytics %} {% for component,
-is_use, _, _ in components %} {% if is_use %} {% if component ==
-'featured_services' %} {% featured_services %} {% elif component == 'about' %}
-{% about %} {% elif component == 'clients' %} {% clients %} {% elif component
-== 'cta' %} {% cta %} {% elif component == 'onfocus' %} {% onfocus %} {% elif
-component == 'features' %} {% features %} {% elif component == 'services' %} {%
-services %} {% elif component == 'testimonials' %} {% testimonials %} {% elif
-component == 'pricing' %} {% pricing %} {% elif component == 'faq' %} {% faq %}
-{% elif component == 'portfolio' %} {% portfolio %} {% elif component == 'team'
-%} {% team %} {% elif component == 'recent_blog_posts' %} {% recent_blog_posts
-%} {% elif component == 'contact' %} {% contact %} {% endif %} {% endif %} {%
-endfor %} {% endblock content %} {% include 'herobizds/footer.html' %}
+{% seo %}
+{% header %} {% block content %} {% hero %} {% show_calendar %} {% show_modal
+%} {% make_analytics %} {% for component, is_use, _, _ in components %} {% if
+is_use %} {% if component == 'featured_services' %} {% featured_services %} {%
+elif component == 'about' %} {% about %} {% elif component == 'clients' %} {%
+clients %} {% elif component == 'cta' %} {% cta %} {% elif component ==
+'onfocus' %} {% onfocus %} {% elif component == 'features' %} {% features %} {%
+elif component == 'services' %} {% services %} {% elif component ==
+'testimonials' %} {% testimonials %} {% elif component == 'pricing' %} {%
+pricing %} {% elif component == 'faq' %} {% faq %} {% elif component ==
+'portfolio' %} {% portfolio %} {% elif component == 'team' %} {% team %} {%
+elif component == 'recent_blog_posts' %} {% recent_blog_posts %} {% elif
+component == 'contact' %} {% contact %} {% endif %} {% endif %} {% endfor %} {%
+endblock content %} {% footer %}
```

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/portfolio-details.html` & `django_herobiz_ds-3.0.0/django_herobiz_ds/templates/herobizds/portfolio-details.html`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-{% extends "herobizds/index.html" %}
+{% extends template_name|add:'/index.html' %}
 {% load static %}
 
 {% block content %}
   <main id="main">
-    <!-- ======= Breadcrumbs ======= -->{% include 'herobizds/breadcrumb.html' %}<!-- End Breadcrumbs -->
+    <!-- ======= Breadcrumbs ======= -->{% include template_name|add:'/breadcrumb.html' %}<!-- End Breadcrumbs -->
 
     <!-- ======= Portfolio Details Section ======= -->
     <section id="portfolio-details" class="portfolio-details">
       <div class="container" data-aos="fade-up">
 
         <div class="row gy-4">
```

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/privacy.html` & `django_herobiz_ds-3.0.0/django_herobiz_ds/templates/herobizds/privacy.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-{% extends "herobizds/index.html" %}
+{% extends template_name|add:'/index.html' %}
 {% load static %}
 
 {% block content %}
 <main id="main">
-  <!-- ======= Breadcrumbs ======= -->{% include 'herobizds/breadcrumb.html' %}<!-- End Breadcrumbs -->
+  <!-- ======= Breadcrumbs ======= -->{% include template_name|add:'/breadcrumb.html' %}<!-- End Breadcrumbs -->
 
   <!-- ======= Blog Section ======= -->
   <section class="inner-page">
     <div class="container" data-aos="fade-up">
 
       <div class="section-header">
         <h2>개인정보처리방침</h2>
```

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/seo.html` & `django_herobiz_ds-3.0.0/django_herobiz_ds/templates/herobizds/seo.html`

 * *Files 9% similar despite different names*

```diff
@@ -5,30 +5,30 @@
 <meta content="width=device-width, initial-scale=1.0" name="viewport">
 
 <title>{{ seo.company_name }} | {{ seo.small_title }}</title>
 <meta name="description" content="{{ seo.desc }}">
 <meta name="keywords" content="{{ seo.keywords }}">
 
 <meta property="og:url" content="https://{{ seo.url }}">
-<meta property="og:image" itemprop="image primaryImageOfPage" content="{% static 'img/herobizds/favicon.png' %}">
+<meta property="og:image" itemprop="image primaryImageOfPage" content="{% static 'img/'|add:template_name|add:'/favicon.png' %}">
 
 <meta name="twitter:description" property="og:description" itemprop="description" content="{{ seo.desc }}">
 <meta name="twitter:title" property="og:title" itemprop="name" content="{{ seo.company_name }} | {{ seo.small_title }}">
 
 {% cache 86400 base_header %}
 <meta property="og:type" content="website">
 <meta property="og:site_name" content="{{ seo.url }}">
 <meta name="twitter:card" content="summary">
 <meta name="twitter:domain" content="{{ seo.url }}">
 {% endcache %}
 
 <!-- Favicons -->
-<link rel="icon" type="image/png" sizes="32x32" href="{% static 'img/herobizds/favicon.png' %}">
-<link rel="shortcut icon" sizes="16x16 24x24 32x32 48x48" href="{% static 'img/herobizds/favicon.ico' %}">
-<link rel="apple-touch-icon" sizes="180x180" href="{% static 'img/herobizds/apple-touch-icon.png' %}">
+<link rel="icon" type="image/png" sizes="32x32" href="{% static 'img/'|add:template_name|add:'/favicon.png' %}">
+<link rel="shortcut icon" sizes="16x16 24x24 32x32 48x48" href="{% static 'img/'|add:template_name|add:'/favicon.ico' %}">
+<link rel="apple-touch-icon" sizes="180x180" href="{% static 'img/'|add:template_name|add:'/apple-touch-icon.png' %}">
 
 <!-- Google Fonts -->
 <!-- 템플릿 기본 폰트 -->
 <link href="https://fonts.googleapis.com/css2
 ?family=Open+Sans:ital,wght@0,300;0,400;0,500;0,600;0,700;1,300;1,400;1,500;1,600;1,700
 &family=Poppins:ital,wght@0,300;0,400;0,500;0,600;0,700;1,300;1,400;1,500;1,600;1,700
 &family=Source+Sans+Pro:ital,wght@0,300;0,400;0,600;0,700;1,300;1,400;1,600;1,700&display=swap" rel="stylesheet">
```

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/templates/herobizds/terms.html` & `django_herobiz_ds-3.0.0/django_herobiz_ds/templates/herobizds/terms.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-{% extends "herobizds/index.html" %}
+{% extends template_name|add:'/index.html' %}
 {% load static %}
 
 {% block content %}
 <main id="main">
-  <!-- ======= Breadcrumbs ======= -->{% include 'herobizds/breadcrumb.html' %}<!-- End Breadcrumbs -->
+  <!-- ======= Breadcrumbs ======= -->{% include template_name|add:'/breadcrumb.html' %}<!-- End Breadcrumbs -->
 
   <!-- ======= Blog Section ======= -->
   <section class="inner-page">
     <div class="container" data-aos="fade-up">
 
       <div class="section-header">
         <h2>이용약관</h2>
```

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/templatetags/herobizds_tags.py` & `django_herobiz_ds-3.0.0/django_herobiz_ds/templatetags/herobizds_tags.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from django.template import Library, loader
 from ..models import Post
 from ..models import Portfolio, Category
 from taggit.models import Tag
 from _data.herobizds import CATEGORY
 from ..forms import SearchForm
+from _data import herobizds
+
 
 import logging
 logger = logging.getLogger(__name__)
 formatter = logging.Formatter('%(levelname)s: [%(name)s] %(message)s')
 ch = logging.StreamHandler()
 ch.setFormatter(formatter)
 logger.addHandler(ch)
@@ -15,174 +17,207 @@
 
 
 register = Library()
 
 # https://localcoder.org/django-inclusion-tag-with-configurable-template
 
 
+template_name = herobizds.context['template_name']
+
+
+@register.simple_tag(takes_context=True)
+def seo(context):
+    t = loader.get_template(template_name + "/seo.html")
+    context.update({
+        'template_name': template_name,
+    })
+    logger.info(context)
+    return t.render(context.flatten())
+
+
+@register.simple_tag(takes_context=True)
+def header(context):
+    t = loader.get_template(template_name + "/header.html")
+    context.update({
+        'template_name': template_name,
+    })
+    logger.info(context)
+    return t.render(context.flatten())
+
+
 @register.simple_tag(takes_context=True)
 def hero(context):
-    t = loader.get_template(f"herobizds/_hero-{context['hero_type']}.html")
+    t = loader.get_template(template_name + f"/_hero-{context['hero_type']}.html")
     context.update({
 
     })
     logger.info(context)
     return t.render(context.flatten())
 
 
 @register.simple_tag(takes_context=True)
 def featured_services(context):
-    t = loader.get_template("herobizds/_featured-services.html")
+    t = loader.get_template(template_name + "/_featured-services.html")
     context.update({
 
     })
     logger.info(context)
     return t.render(context.flatten())
 
 
 @register.simple_tag(takes_context=True)
 def about(context):
-    t = loader.get_template("herobizds/_about.html")
+    t = loader.get_template(template_name + "/_about.html")
     context.update({
 
     })
     logger.info(context)
     return t.render(context.flatten())
 
 
 @register.simple_tag(takes_context=True)
 def clients(context):
-    t = loader.get_template("herobizds/_clients.html")
+    t = loader.get_template(template_name + "/_clients.html")
     context.update({
 
     })
     logger.info(context)
     return t.render(context.flatten())
 
 
 @register.simple_tag(takes_context=True)
 def cta(context):
-    t = loader.get_template("herobizds/_cta.html")
+    t = loader.get_template(template_name + "/_cta.html")
     context.update({
 
     })
     logger.info(context)
     return t.render(context.flatten())
 
 
 @register.simple_tag(takes_context=True)
 def onfocus(context):
-    t = loader.get_template("herobizds/_onfocus.html")
+    t = loader.get_template(template_name + "/_onfocus.html")
     context.update({
 
     })
     logger.info(context)
     return t.render(context.flatten())
 
 
 @register.simple_tag(takes_context=True)
 def features(context):
-    t = loader.get_template("herobizds/_features.html")
+    t = loader.get_template(template_name + "/_features.html")
     context.update({
 
     })
     logger.info(context)
     return t.render(context.flatten())
 
 
 @register.simple_tag(takes_context=True)
 def services(context):
-    t = loader.get_template("herobizds/_services.html")
+    t = loader.get_template(template_name + "/_services.html")
     context.update({
 
     })
     logger.info(context)
     return t.render(context.flatten())
 
 
 @register.simple_tag(takes_context=True)
 def testimonials(context):
-    t = loader.get_template("herobizds/_testimonials.html")
+    t = loader.get_template(template_name + "/_testimonials.html")
     context.update({
 
     })
     logger.info(context)
     return t.render(context.flatten())
 
 
 @register.simple_tag(takes_context=True)
 def pricing(context):
-    t = loader.get_template("herobizds/_pricing.html")
+    t = loader.get_template(template_name + "/_pricing.html")
     context.update({
 
     })
     logger.info(context)
     return t.render(context.flatten())
 
 
 @register.simple_tag(takes_context=True)
 def faq(context):
-    t = loader.get_template("herobizds/_faq.html")
+    t = loader.get_template(template_name + "/_faq.html")
     context.update({
 
     })
     logger.info(context)
     return t.render(context.flatten())
 
 
 @register.simple_tag(takes_context=True)
 def portfolio(context):
-    t = loader.get_template("herobizds/_portfolio.html")
+    t = loader.get_template(template_name + "/_portfolio.html")
     context.update({
         'categories': Category.objects,
         'items': Portfolio.objects,
     })
     logger.info(context)
     return t.render(context.flatten())
 
 
 @register.simple_tag(takes_context=True)
 def team(context):
-    t = loader.get_template("herobizds/_team.html")
+    t = loader.get_template(template_name + "/_team.html")
     context.update({
 
     })
     logger.info(context)
     return t.render(context.flatten())
 
 
 @register.simple_tag(takes_context=True)
 def recent_blog_posts(context):
-    t = loader.get_template("herobizds/_recent-blog-posts.html")
+    t = loader.get_template(template_name + "/_recent-blog-posts.html")
     objects = Post.objects.filter(status=1).filter(remarkable=True).order_by('-updated_on')
     context.update({
         'top3': objects[:3],
     })
     logger.info(context)
     return t.render(context.flatten())
 
 
 @register.simple_tag(takes_context=True)
 def contact(context):
-    t = loader.get_template("herobizds/_contact.html")
+    t = loader.get_template(template_name + "/_contact.html")
     context.update({
 
     })
     logger.info(context)
     return t.render(context.flatten())
 
 
 @register.simple_tag(takes_context=True)
 def sidebar(context):
-    t = loader.get_template(f"herobizds/_sidebar.html")
+    t = loader.get_template(template_name + "/_sidebar.html")
     tags = Tag.objects.all()
     category = []
     for category_int, name in CATEGORY:
         category.append([category_int, name, Post.objects.filter(status=1).filter(category=category_int).count()])
     context.update({
         'form': SearchForm(),
         'category': category,
         'all_tags': tags,
         'latest': Post.objects.filter(status=1).order_by('-updated_on')[:6],
     })
     logger.info(context)
     return t.render(context.flatten())
+
+
+@register.simple_tag(takes_context=True)
+def footer(context):
+    t = loader.get_template(template_name + "/footer.html")
+    context.update({
+        'template_name': template_name,
+    })
+    logger.info(context)
+    return t.render(context.flatten())
```

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/urls.py` & `django_herobiz_ds-3.0.0/django_herobiz_ds/urls.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from django.urls import path, include
 from django.contrib.sitemaps.views import sitemap
 from . import views
 from .sitemaps import PostSitemap, StaticViewSitemap
+from _data import herobizds
+
+app_name = herobizds.context['template_name']
 
-app_name = 'herobizds'
 
 sitemaps = {
     "posts": PostSitemap,
     'static': StaticViewSitemap,
 }
 
 urlpatterns = [
```

### Comparing `django_herobiz_ds-2.3.0/django_herobiz_ds/views.py` & `django_herobiz_ds-3.0.0/django_herobiz_ds/views.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from django.shortcuts import render, get_object_or_404
 from django_utilsds import utils
 from .forms import AppointmentForm
 from _data import herobizds
+
 from .models import Portfolio
 from hitcount.views import HitCountDetailView
 from .models import Post, CATEGORY
 from django.views import generic
 from .forms import SearchForm
 
 import logging
@@ -14,14 +15,17 @@
 ch = logging.StreamHandler()
 ch.setFormatter(formatter)
 logger.addHandler(ch)
 logger.setLevel(logging.ERROR)
 
 num_pagination = 6
 
+template_name = herobizds.context['template_name']
+c = herobizds.context
+
 
 def make_page_bundle(page_range, n=5):
     # 전체 페이지를 n 개수의 묶음으로 만든다.
     # pagination에 사용
     l = [i for i in page_range]
     return [l[i:i + n] for i in range(0, len(l), n)]
 
@@ -29,24 +33,22 @@
 def robots(request):
     from django.shortcuts import HttpResponse
     file_content = utils.make_robots()
     return HttpResponse(file_content, content_type="text/plain")
 
 
 def home(request):
-    c = herobizds.context
-
     logger.info(c)
     if request.method == 'GET':
         c.update({'form': AppointmentForm()})
         c['post_message'] = None
-        return render(request, 'herobizds/index.html', c)
+        return render(request, template_name + '/index.html', c)
     elif request.method == "POST":
         c.update(make_post_context(request.POST, c['basic_info']['consult_email']))
-        return render(request, 'herobizds/index.html', c)
+        return render(request, template_name + '/index.html', c)
 
 
 def make_post_context(request_post, consult_mail):
     logger.info(request_post)
     context = {}
     # appointment 앱에서 post 요청을 처리함.
     logger.info(f'request.POST : {request_post}')
@@ -58,40 +60,38 @@
         subject = form.cleaned_data['subject']
         message = form.cleaned_data['message']
         logger.info(f'Pass validation test -  {name} {email} {subject} {message}')
         is_sendmail = utils.mail_to(title=f'{name} 고객 상담 문의',
                                     text=f'이름: {name}\n메일: {email}\n제목: {subject}\n메시지: {message}',
                                     mail_addr=consult_mail)
         if is_sendmail:
-            context['post_message'] = '담당자에게 예약 신청이 전달되었습니다. 확인 후 바로 연락 드리겠습니다. 감사합니다.'
+            context['post_message'] = '담당자에게 내용이 전달되었습니다. 확인 후 바로 연락 드리겠습니다. 감사합니다.'
         else:
             context['post_message'] = '메일 전송에서 오류가 발생하였습니다. 카카오톡이나 전화로 문의주시면 감사하겠습니다. 죄송합니다.'
         return context
     else:
         logger.error('Fail form validation test')
         context['post_message'] = '입력 항목이 유효하지 않습니다. 다시 입력해 주십시요.'
         return context
 
 
 def details(request, id: int):
-    c = herobizds.context
     c.update(
         {
             "breadcrumb": {
                 "title": c['portfolio']['title'],
             },
             "obj": get_object_or_404(Portfolio, pk=id),
         }
     )
     logger.debug(c)
     return render(request, "herobizds/portfolio-details.html", c)
 
 
 def terms(request):
-    c = herobizds.context
     c.update(
         {
             "breadcrumb": {
                 "title": "Terms of Use",
             },
             "terms": {
                 "company_name": c['basic_info']['company_name'],
@@ -99,15 +99,14 @@
             },
         }
     )
     return render(request, "herobizds/terms.html", c)
 
 
 def privacy(request):
-    c = herobizds.context
     c.update(
         {
             "breadcrumb": {
                 "title": "Privacy Policy",
             },
             "privacy": {
                 "company_name": c['basic_info']['company_name'],
@@ -121,41 +120,41 @@
         }
     )
     return render(request, "herobizds/privacy.html", c)
 
 
 class PostDetailView(HitCountDetailView):
     model = Post
-    template_name = 'herobizds/blog-details.html'
+    template_name = template_name + '/blog-details.html'
     context_object_name = 'object'
     slug_field = 'slug'
     count_hit = True
 
     def get_context_data(self, **kwargs):
         context = super().get_context_data(**kwargs)
 
         for i, name in CATEGORY:
             if self.get_object().category == i:
                 category_name = name
                 break
 
-        context.update(herobizds.context)
+        context.update(c)
         context.update(
             {
                 'breadcrumb': {
                     'title': 'Blog Detail'
                 },
                 'category_name': category_name
             }
         )
         return context
 
 
 class SearchResult(generic.ListView):
-    template_name = 'herobizds/blog.html'
+    template_name = template_name + '/blog.html'
     paginate_by = num_pagination
 
     def get_queryset(self):
         form = SearchForm(self.request.GET)
         if form.is_valid():
             q = form.cleaned_data['q']
         else:
@@ -169,15 +168,15 @@
         pages_devided = make_page_bundle(context['paginator'].page_range)
 
         # 현재 페이지에 해당하는 묶음을 page_bundle로 전달한다.
         for page_bundle in pages_devided:
             if context['page_obj'].number in page_bundle:
                 context['page_bundle'] = page_bundle
 
-        context.update(herobizds.context)
+        context.update(c)
         return context
 
 
 class Blog(SearchResult):
     # 홈페이지에서 다이렉트 링크로 연결하기 위해서 필요하다.
     def get_queryset(self):
         # https://stackoverflow.com/questions/56067365/how-to-filter-posts-by-tags-using-django-taggit-in-django
```

### Comparing `django_herobiz_ds-2.3.0/pyproject.toml` & `django_herobiz_ds-3.0.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "django_herobiz_ds"
-version = "2.3.0"
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
-    "django-utilsds >= 0.5.0",
+    "django-utilsds >= 0.6.0",
     "django-mdeditor >= 0.1.20",
     "django-hitcount >= 1.3.5",
     "django-taggit >= 5.0.1",
     "django-markdownify >= 0.9.3",
     "django-light >= 0.1.0",
     "pillow >= 10.3.0",
 ]
```

### Comparing `django_herobiz_ds-2.3.0/PKG-INFO` & `django_herobiz_ds-3.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: django_herobiz_ds
-Version: 2.3.0
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
-Requires-Dist: django-utilsds >= 0.5.0
+Requires-Dist: django-utilsds >= 0.6.0
 Requires-Dist: django-mdeditor >= 0.1.20
 Requires-Dist: django-hitcount >= 1.3.5
 Requires-Dist: django-taggit >= 5.0.1
 Requires-Dist: django-markdownify >= 0.9.3
 Requires-Dist: django-light >= 0.1.0
 Requires-Dist: pillow >= 10.3.0
 Project-URL: Home, https://www.demiansoft.com
@@ -31,15 +31,15 @@
 #### Requirements
 
 Django >= 4.2.11
 libsass>=0.23.0
 django-analyticsds >= 0.3.1
 django-calendards >= 0.4.0
 django-modalds >= 0.1.0
-django-utilsds >= 0.4.0
+django-utilsds >= 0.6.0
 django-mdeditor >= 0.1.20
 django-hitcount >= 1.3.5
 django-taggit >= 5.0.1
 django-markdownify >= 0.9.3
 django-light >= 0.1.0   # 밝은 admin 화면
 pillow >= 10.3.0    # 데이터베이스에서 이미지 사용하기위해
```

