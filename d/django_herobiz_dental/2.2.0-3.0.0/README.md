# Comparing `tmp/django_herobiz_dental-2.2.0.tar.gz` & `tmp/django_herobiz_dental-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_herobiz_dental-2.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "django_herobiz_dental-3.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `django_herobiz_dental-2.2.0.tar` & `django_herobiz_dental-3.0.0.tar`

### file list

```diff
@@ -1,178 +1,178 @@
--rw-r--r--   0        0        0    10244 2024-05-17 05:37:55.112002 django_herobiz_dental-2.2.0/.DS_Store
--rw-r--r--   0        0        0       66 2024-04-05 05:27:06.902059 django_herobiz_dental-2.2.0/.gitattributes
--rw-r--r--   0        0        0       55 2024-05-18 01:48:26.698611 django_herobiz_dental-2.2.0/.gitignore
--rw-r--r--   0        0        0       52 2024-04-05 05:27:59.025754 django_herobiz_dental-2.2.0/.idea/.gitignore
--rw-r--r--   0        0        0      411 2024-04-05 05:27:58.943620 django_herobiz_dental-2.2.0/.idea/django-herobiz-dental.iml
--rw-r--r--   0        0        0      174 2024-04-05 05:27:58.956024 django_herobiz_dental-2.2.0/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      433 2024-04-05 06:12:30.213755 django_herobiz_dental-2.2.0/.idea/misc.xml
--rw-r--r--   0        0        0      294 2024-04-05 05:27:58.950052 django_herobiz_dental-2.2.0/.idea/modules.xml
--rw-r--r--   0        0        0      167 2024-04-05 05:27:58.958164 django_herobiz_dental-2.2.0/.idea/vcs.xml
--rw-r--r--   0        0        0     1079 2024-03-19 03:45:10.033383 django_herobiz_dental-2.2.0/LICENSE
--rw-r--r--   0        0        0     5042 2024-05-18 19:44:22.970154 django_herobiz_dental-2.2.0/README.md
--rw-r--r--   0        0        0        0 2024-04-05 06:12:24.810066 django_herobiz_dental-2.2.0/django_herobiz_dental/__init__.py
--rw-r--r--   0        0        0      612 2024-04-21 04:03:56.019184 django_herobiz_dental-2.2.0/django_herobiz_dental/admin.py
--rw-r--r--   0        0        0      172 2024-04-05 06:12:24.811671 django_herobiz_dental-2.2.0/django_herobiz_dental/apps.py
--rw-r--r--   0        0        0     1201 2024-04-21 04:03:56.010074 django_herobiz_dental-2.2.0/django_herobiz_dental/forms.py
--rw-r--r--   0        0        0     2088 2024-04-05 06:31:38.858042 django_herobiz_dental-2.2.0/django_herobiz_dental/migrations/0001_initial.py
--rw-r--r--   0        0        0      334 2024-04-11 05:20:55.981354 django_herobiz_dental-2.2.0/django_herobiz_dental/migrations/0002_remove_portfolio_client.py
--rw-r--r--   0        0        0     2553 2024-04-21 04:08:50.044472 django_herobiz_dental-2.2.0/django_herobiz_dental/migrations/0003_portfolio_client_post_profile.py
--rw-r--r--   0        0        0        0 2024-04-05 06:12:24.812107 django_herobiz_dental-2.2.0/django_herobiz_dental/migrations/__init__.py
--rw-r--r--   0        0        0     3149 2024-05-16 05:59:24.869835 django_herobiz_dental-2.2.0/django_herobiz_dental/models.py
--rw-r--r--   0        0        0      559 2024-04-21 04:03:56.001901 django_herobiz_dental-2.2.0/django_herobiz_dental/sitemaps.py
--rwxr-xr-x   0        0        0    60252 2024-03-29 01:14:08.439726 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/css/main.css
--rwxr-xr-x   0        0        0     7992 2024-04-03 08:26:33.002126 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/css/variables-blue.css
--rwxr-xr-x   0        0        0     7989 2024-04-03 08:32:44.614276 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/css/variables-green.css
--rwxr-xr-x   0        0        0     7992 2024-04-03 08:32:44.619981 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/css/variables-orange.css
--rwxr-xr-x   0        0        0     7994 2024-04-03 08:32:44.616432 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/css/variables-pink.css
--rwxr-xr-x   0        0        0     7992 2024-04-03 08:32:44.612088 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/css/variables-purple.css
--rwxr-xr-x   0        0        0     7986 2024-04-03 08:32:44.607824 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/css/variables-red.css
--rwxr-xr-x   0        0        0     7985 2024-04-03 08:32:44.618152 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/css/variables.css
--rwxr-xr-x   0        0        0      766 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/img/about-bg.png
--rwxr-xr-x   0        0        0    95604 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/img/faq.jpg
--rwxr-xr-x   0        0        0    13287 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/img/hero-bg.png
--rwxr-xr-x   0        0        0    13081 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/img/onfocus-content-bg.jpg
--rwxr-xr-x   0        0        0    61855 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/img/pricing-bg.jpg
--rwxr-xr-x   0        0        0     8186 2024-03-17 05:37:08.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/js/main.js
--rwxr-xr-x   0        0        0      281 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/scss/_blog.scss
--rwxr-xr-x   0        0        0     3649 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/scss/_footer.scss
--rwxr-xr-x   0        0        0     3770 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/scss/_general.scss
--rwxr-xr-x   0        0        0     1118 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/scss/_header.scss
--rwxr-xr-x   0        0        0      643 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/scss/_index.scss
--rwxr-xr-x   0        0        0     5712 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/scss/_nav.scss
--rwxr-xr-x   0        0        0     1320 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/scss/_portfolio-details.scss
--rwxr-xr-x   0        0        0     2172 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/scss/blog/_comments.scss
--rwxr-xr-x   0        0        0     3738 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/scss/blog/_details.scss
--rwxr-xr-x   0        0        0      758 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/scss/blog/_pagination.scss
--rwxr-xr-x   0        0        0     1813 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/scss/blog/_posts-list.scss
--rwxr-xr-x   0        0        0     3480 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/scss/blog/_sidebar.scss
--rwxr-xr-x   0        0        0     1676 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/scss/index/_about.scss
--rwxr-xr-x   0        0        0      377 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/scss/index/_clients.scss
--rwxr-xr-x   0        0        0     3086 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/scss/index/_contact.scss
--rwxr-xr-x   0        0        0     1882 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/scss/index/_cta.scss
--rwxr-xr-x   0        0        0     1674 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/scss/index/_faq.scss
--rwxr-xr-x   0        0        0      981 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/scss/index/_featured-services.scss
--rwxr-xr-x   0        0        0     1762 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/scss/index/_features.scss
--rwxr-xr-x   0        0        0     2205 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/scss/index/_hero-animated.scss
--rwxr-xr-x   0        0        0     1990 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/scss/index/_hero-fullscreen.scss
--rwxr-xr-x   0        0        0     1764 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/scss/index/_hero-static.scss
--rwxr-xr-x   0        0        0     3481 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/scss/index/_hero.scss
--rwxr-xr-x   0        0        0     3798 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/scss/index/_onfocus.scss
--rwxr-xr-x   0        0        0     2264 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/scss/index/_portfolio.scss
--rwxr-xr-x   0        0        0     2551 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/scss/index/_pricing.scss
--rwxr-xr-x   0        0        0     1512 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/scss/index/_recent-blog-posts.scss
--rwxr-xr-x   0        0        0     1718 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/scss/index/_services.scss
--rwxr-xr-x   0        0        0     1922 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/scss/index/_team.scss
--rwxr-xr-x   0        0        0     2203 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/scss/index/_testimonials.scss
--rwxr-xr-x   0        0        0      253 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/scss/main.scss
--rwxr-xr-x   0        0        0     7960 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/scss/variables-blue.css
--rwxr-xr-x   0        0        0     7957 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/scss/variables-green.css
--rwxr-xr-x   0        0        0     7960 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/scss/variables-orange.css
--rwxr-xr-x   0        0        0     7962 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/scss/variables-pink.css
--rwxr-xr-x   0        0        0     7960 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/scss/variables-purple.css
--rwxr-xr-x   0        0        0     7954 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/scss/variables-red.css
--rwxr-xr-x   0        0        0     7953 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/scss/variables.css
--rw-r--r--   0        0        0    19941 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/aos/aos.cjs.js
--rw-r--r--   0        0        0    28765 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/aos/aos.css
--rw-r--r--   0        0        0    19768 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/aos/aos.esm.js
--rw-r--r--   0        0        0    13800 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/aos/aos.js
--rw-r--r--   0        0        0    56459 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/aos/aos.js.map
--rw-r--r--   0        0        0    98255 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap-icons/bootstrap-icons.css
--rw-r--r--   0        0        0    52358 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap-icons/bootstrap-icons.json
--rw-r--r--   0        0        0    85875 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap-icons/bootstrap-icons.min.css
--rw-r--r--   0        0        0    57755 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap-icons/bootstrap-icons.scss
--rw-r--r--   0        0        0   176032 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap-icons/fonts/bootstrap-icons.woff
--rw-r--r--   0        0        0   130396 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap-icons/fonts/bootstrap-icons.woff2
--rw-r--r--   0        0        0    70329 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-grid.css
--rw-r--r--   0        0        0   203221 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-grid.css.map
--rw-r--r--   0        0        0    51795 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-grid.min.css
--rw-r--r--   0        0        0   115986 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-grid.min.css.map
--rw-r--r--   0        0        0    70403 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-grid.rtl.css
--rw-r--r--   0        0        0   203225 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-grid.rtl.css.map
--rw-r--r--   0        0        0    51870 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-grid.rtl.min.css
--rw-r--r--   0        0        0   116063 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-grid.rtl.min.css.map
--rw-r--r--   0        0        0    12065 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-reboot.css
--rw-r--r--   0        0        0   129371 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-reboot.css.map
--rw-r--r--   0        0        0    10126 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-reboot.min.css
--rw-r--r--   0        0        0    51369 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-reboot.min.css.map
--rw-r--r--   0        0        0    12058 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-reboot.rtl.css
--rw-r--r--   0        0        0   129386 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-reboot.rtl.css.map
--rw-r--r--   0        0        0    10198 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css
--rw-r--r--   0        0        0    63943 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css.map
--rw-r--r--   0        0        0   107823 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-utilities.css
--rw-r--r--   0        0        0   267535 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-utilities.css.map
--rw-r--r--   0        0        0    85352 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-utilities.min.css
--rw-r--r--   0        0        0   180381 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-utilities.min.css.map
--rw-r--r--   0        0        0   107691 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-utilities.rtl.css
--rw-r--r--   0        0        0   267476 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-utilities.rtl.css.map
--rw-r--r--   0        0        0    85281 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css
--rw-r--r--   0        0        0   180217 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css.map
--rw-r--r--   0        0        0   281046 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap.css
--rw-r--r--   0        0        0   679755 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap.css.map
--rw-r--r--   0        0        0   232803 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap.min.css
--rw-r--r--   0        0        0   589892 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap.min.css.map
--rw-r--r--   0        0        0   280259 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap.rtl.css
--rw-r--r--   0        0        0   679615 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap.rtl.css.map
--rw-r--r--   0        0        0   232911 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap.rtl.min.css
--rw-r--r--   0        0        0   589087 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap.rtl.min.css.map
--rw-r--r--   0        0        0   207819 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/js/bootstrap.bundle.js
--rw-r--r--   0        0        0   444579 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/js/bootstrap.bundle.js.map
--rw-r--r--   0        0        0    80721 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/js/bootstrap.bundle.min.js
--rw-r--r--   0        0        0   332090 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/js/bootstrap.bundle.min.js.map
--rw-r--r--   0        0        0   135829 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/js/bootstrap.esm.js
--rw-r--r--   0        0        0   305438 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/js/bootstrap.esm.js.map
--rw-r--r--   0        0        0    73935 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/js/bootstrap.esm.min.js
--rw-r--r--   0        0        0   222455 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/js/bootstrap.esm.min.js.map
--rw-r--r--   0        0        0   145401 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/js/bootstrap.js
--rw-r--r--   0        0        0   306606 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/js/bootstrap.js.map
--rw-r--r--   0        0        0    60635 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/js/bootstrap.min.js
--rw-r--r--   0        0        0   220561 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/js/bootstrap.min.js.map
--rw-r--r--   0        0        0    17372 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/glightbox/css/glightbox.css
--rw-r--r--   0        0        0    13749 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/glightbox/css/glightbox.min.css
--rw-r--r--   0        0        0    52561 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/glightbox/css/plyr.css
--rw-r--r--   0        0        0    45081 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/glightbox/css/plyr.min.css
--rw-r--r--   0        0        0   109391 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/glightbox/js/glightbox.js
--rw-r--r--   0        0        0    55880 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/glightbox/js/glightbox.min.js
--rw-r--r--   0        0        0    91398 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/isotope-layout/isotope.pkgd.js
--rw-r--r--   0        0        0    35445 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/isotope-layout/isotope.pkgd.min.js
--rwxr-xr-x   0        0        0   238381 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/php-email-form/php-email-form.php
--rwxr-xr-x   0        0        0     2734 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/php-email-form/validate.js
--rw-r--r--   0        0        0    18436 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/swiper/swiper-bundle.min.css
--rw-r--r--   0        0        0   149147 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/swiper/swiper-bundle.min.js
--rw-r--r--   0        0        0   201656 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/swiper/swiper-bundle.min.js.map
--rw-r--r--   0        0        0     2102 2024-04-09 00:04:07.573124 django_herobiz_dental-2.2.0/django_herobiz_dental/templates/herobizdental/_about.html
--rw-r--r--   0        0        0      434 2024-04-05 06:31:15.204362 django_herobiz_dental-2.2.0/django_herobiz_dental/templates/herobizdental/_clients.html
--rw-r--r--   0        0        0     2846 2024-04-12 02:19:51.757891 django_herobiz_dental-2.2.0/django_herobiz_dental/templates/herobizdental/_contact.html
--rw-r--r--   0        0        0     1175 2024-05-04 00:59:47.337426 django_herobiz_dental-2.2.0/django_herobiz_dental/templates/herobizdental/_cta.html
--rw-r--r--   0        0        0     1599 2024-04-05 06:31:15.205949 django_herobiz_dental-2.2.0/django_herobiz_dental/templates/herobizdental/_faq.html
--rw-r--r--   0        0        0      794 2024-03-29 06:50:25.784512 django_herobiz_dental-2.2.0/django_herobiz_dental/templates/herobizdental/_featured-services.html
--rw-r--r--   0        0        0     2039 2024-04-05 06:31:15.185290 django_herobiz_dental-2.2.0/django_herobiz_dental/templates/herobizdental/_features.html
--rw-r--r--   0        0        0      976 2024-04-05 08:05:20.508185 django_herobiz_dental-2.2.0/django_herobiz_dental/templates/herobizdental/_hero-animated.html
--rw-r--r--   0        0        0     1827 2024-04-09 00:03:36.818036 django_herobiz_dental-2.2.0/django_herobiz_dental/templates/herobizdental/_hero-carousel.html
--rw-r--r--   0        0        0      866 2024-04-05 07:58:17.230132 django_herobiz_dental-2.2.0/django_herobiz_dental/templates/herobizdental/_hero-fullscreen.html
--rw-r--r--   0        0        0      871 2024-04-05 06:31:15.195476 django_herobiz_dental-2.2.0/django_herobiz_dental/templates/herobizdental/_hero-static.html
--rw-r--r--   0        0        0     2039 2024-05-04 01:19:12.465694 django_herobiz_dental-2.2.0/django_herobiz_dental/templates/herobizdental/_onfocus.html
--rw-r--r--   0        0        0     1486 2024-04-05 06:31:15.182443 django_herobiz_dental-2.2.0/django_herobiz_dental/templates/herobizdental/_portfolio.html
--rw-r--r--   0        0        0     1462 2024-05-09 00:00:35.838293 django_herobiz_dental-2.2.0/django_herobiz_dental/templates/herobizdental/_pricing.html
--rw-r--r--   0        0        0     1176 2024-05-21 23:49:52.792752 django_herobiz_dental-2.2.0/django_herobiz_dental/templates/herobizdental/_recent-blog-posts.html
--rw-r--r--   0        0        0      990 2024-05-17 04:40:54.995837 django_herobiz_dental-2.2.0/django_herobiz_dental/templates/herobizdental/_services.html
--rw-r--r--   0        0        0     1699 2024-05-16 05:16:41.130030 django_herobiz_dental-2.2.0/django_herobiz_dental/templates/herobizdental/_sidebar.html
--rw-r--r--   0        0        0     1676 2024-04-11 00:36:54.545452 django_herobiz_dental-2.2.0/django_herobiz_dental/templates/herobizdental/_team.html
--rw-r--r--   0        0        0     1333 2024-04-05 06:31:15.202919 django_herobiz_dental-2.2.0/django_herobiz_dental/templates/herobizdental/_testimonials.html
--rwxr-xr-x   0        0        0    10531 2024-04-30 05:50:18.836953 django_herobiz_dental-2.2.0/django_herobiz_dental/templates/herobizdental/blog-details.html
--rwxr-xr-x   0        0        0     2969 2024-05-21 23:49:19.877790 django_herobiz_dental-2.2.0/django_herobiz_dental/templates/herobizdental/blog.html
--rw-r--r--   0        0        0      346 2024-04-05 06:31:15.198382 django_herobiz_dental-2.2.0/django_herobiz_dental/templates/herobizdental/breadcrumb.html
--rw-r--r--   0        0        0     2215 2024-04-11 03:29:47.000571 django_herobiz_dental-2.2.0/django_herobiz_dental/templates/herobizdental/footer.html
--rwxr-xr-x   0        0        0     1341 2024-03-12 00:49:58.000000 django_herobiz_dental-2.2.0/django_herobiz_dental/templates/herobizdental/forms/contact.php
--rw-r--r--   0        0        0     1430 2024-05-16 04:59:12.184906 django_herobiz_dental-2.2.0/django_herobiz_dental/templates/herobizdental/header.html
--rwxr-xr-x   0        0        0     5184 2024-05-02 04:54:51.026951 django_herobiz_dental-2.2.0/django_herobiz_dental/templates/herobizdental/index.html
--rwxr-xr-x   0        0        0     4995 2024-04-11 05:42:55.439634 django_herobiz_dental-2.2.0/django_herobiz_dental/templates/herobizdental/portfolio-details.html
--rwxr-xr-x   0        0        0    16277 2024-04-21 04:03:55.997732 django_herobiz_dental-2.2.0/django_herobiz_dental/templates/herobizdental/privacy.html
--rw-r--r--   0        0        0     2028 2024-04-05 06:31:15.187765 django_herobiz_dental-2.2.0/django_herobiz_dental/templates/herobizdental/seo.html
--rwxr-xr-x   0        0        0    16317 2024-04-21 04:03:56.020846 django_herobiz_dental-2.2.0/django_herobiz_dental/templates/herobizdental/terms.html
--rw-r--r--   0        0        0        0 2023-03-21 07:32:09.033136 django_herobiz_dental-2.2.0/django_herobiz_dental/templatetags/__init__.py
--rw-r--r--   0        0        0     4813 2024-05-03 01:08:11.844770 django_herobiz_dental-2.2.0/django_herobiz_dental/templatetags/herobizdental_tags.py
--rw-r--r--   0        0        0       60 2024-04-05 06:12:24.811958 django_herobiz_dental-2.2.0/django_herobiz_dental/tests.py
--rw-r--r--   0        0        0     1115 2024-04-21 04:03:56.022033 django_herobiz_dental-2.2.0/django_herobiz_dental/urls.py
--rw-r--r--   0        0        0     7429 2024-05-02 07:51:11.143076 django_herobiz_dental-2.2.0/django_herobiz_dental/views.py
--rw-r--r--   0        0        0      972 2024-05-21 23:52:04.917332 django_herobiz_dental-2.2.0/pyproject.toml
--rw-r--r--   0        0        0     5782 1970-01-01 00:00:00.000000 django_herobiz_dental-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0    10244 2024-05-17 05:37:55.112002 django_herobiz_dental-3.0.0/.DS_Store
+-rw-r--r--   0        0        0       66 2024-04-05 05:27:06.902059 django_herobiz_dental-3.0.0/.gitattributes
+-rw-r--r--   0        0        0       55 2024-05-18 01:48:26.698611 django_herobiz_dental-3.0.0/.gitignore
+-rw-r--r--   0        0        0       52 2024-04-05 05:27:59.025754 django_herobiz_dental-3.0.0/.idea/.gitignore
+-rw-r--r--   0        0        0      411 2024-04-05 05:27:58.943620 django_herobiz_dental-3.0.0/.idea/django-herobiz-dental.iml
+-rw-r--r--   0        0        0      174 2024-04-05 05:27:58.956024 django_herobiz_dental-3.0.0/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      433 2024-04-05 06:12:30.213755 django_herobiz_dental-3.0.0/.idea/misc.xml
+-rw-r--r--   0        0        0      294 2024-04-05 05:27:58.950052 django_herobiz_dental-3.0.0/.idea/modules.xml
+-rw-r--r--   0        0        0      167 2024-04-05 05:27:58.958164 django_herobiz_dental-3.0.0/.idea/vcs.xml
+-rw-r--r--   0        0        0     1079 2024-03-19 03:45:10.033383 django_herobiz_dental-3.0.0/LICENSE
+-rw-r--r--   0        0        0     5042 2024-05-22 23:59:16.810438 django_herobiz_dental-3.0.0/README.md
+-rw-r--r--   0        0        0        0 2024-04-05 06:12:24.810066 django_herobiz_dental-3.0.0/django_herobiz_dental/__init__.py
+-rw-r--r--   0        0        0      612 2024-04-21 04:03:56.019184 django_herobiz_dental-3.0.0/django_herobiz_dental/admin.py
+-rw-r--r--   0        0        0      172 2024-04-05 06:12:24.811671 django_herobiz_dental-3.0.0/django_herobiz_dental/apps.py
+-rw-r--r--   0        0        0     1201 2024-04-21 04:03:56.010074 django_herobiz_dental-3.0.0/django_herobiz_dental/forms.py
+-rw-r--r--   0        0        0     2088 2024-04-05 06:31:38.858042 django_herobiz_dental-3.0.0/django_herobiz_dental/migrations/0001_initial.py
+-rw-r--r--   0        0        0      334 2024-04-11 05:20:55.981354 django_herobiz_dental-3.0.0/django_herobiz_dental/migrations/0002_remove_portfolio_client.py
+-rw-r--r--   0        0        0     2553 2024-04-21 04:08:50.044472 django_herobiz_dental-3.0.0/django_herobiz_dental/migrations/0003_portfolio_client_post_profile.py
+-rw-r--r--   0        0        0        0 2024-04-05 06:12:24.812107 django_herobiz_dental-3.0.0/django_herobiz_dental/migrations/__init__.py
+-rw-r--r--   0        0        0     3240 2024-05-23 00:20:12.264914 django_herobiz_dental-3.0.0/django_herobiz_dental/models.py
+-rw-r--r--   0        0        0      655 2024-05-23 00:20:12.261585 django_herobiz_dental-3.0.0/django_herobiz_dental/sitemaps.py
+-rwxr-xr-x   0        0        0    60252 2024-03-29 01:14:08.439726 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/css/main.css
+-rwxr-xr-x   0        0        0     7992 2024-04-03 08:26:33.002126 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/css/variables-blue.css
+-rwxr-xr-x   0        0        0     7989 2024-04-03 08:32:44.614276 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/css/variables-green.css
+-rwxr-xr-x   0        0        0     7992 2024-04-03 08:32:44.619981 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/css/variables-orange.css
+-rwxr-xr-x   0        0        0     7994 2024-04-03 08:32:44.616432 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/css/variables-pink.css
+-rwxr-xr-x   0        0        0     7992 2024-04-03 08:32:44.612088 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/css/variables-purple.css
+-rwxr-xr-x   0        0        0     7986 2024-04-03 08:32:44.607824 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/css/variables-red.css
+-rwxr-xr-x   0        0        0     7985 2024-04-03 08:32:44.618152 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/css/variables.css
+-rwxr-xr-x   0        0        0      766 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/img/about-bg.png
+-rwxr-xr-x   0        0        0    95604 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/img/faq.jpg
+-rwxr-xr-x   0        0        0    13287 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/img/hero-bg.png
+-rwxr-xr-x   0        0        0    13081 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/img/onfocus-content-bg.jpg
+-rwxr-xr-x   0        0        0    61855 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/img/pricing-bg.jpg
+-rwxr-xr-x   0        0        0     8186 2024-03-17 05:37:08.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/js/main.js
+-rwxr-xr-x   0        0        0      281 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/scss/_blog.scss
+-rwxr-xr-x   0        0        0     3649 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/scss/_footer.scss
+-rwxr-xr-x   0        0        0     3770 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/scss/_general.scss
+-rwxr-xr-x   0        0        0     1118 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/scss/_header.scss
+-rwxr-xr-x   0        0        0      643 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/scss/_index.scss
+-rwxr-xr-x   0        0        0     5712 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/scss/_nav.scss
+-rwxr-xr-x   0        0        0     1320 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/scss/_portfolio-details.scss
+-rwxr-xr-x   0        0        0     2172 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/scss/blog/_comments.scss
+-rwxr-xr-x   0        0        0     3738 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/scss/blog/_details.scss
+-rwxr-xr-x   0        0        0      758 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/scss/blog/_pagination.scss
+-rwxr-xr-x   0        0        0     1813 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/scss/blog/_posts-list.scss
+-rwxr-xr-x   0        0        0     3480 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/scss/blog/_sidebar.scss
+-rwxr-xr-x   0        0        0     1676 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/scss/index/_about.scss
+-rwxr-xr-x   0        0        0      377 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/scss/index/_clients.scss
+-rwxr-xr-x   0        0        0     3086 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/scss/index/_contact.scss
+-rwxr-xr-x   0        0        0     1882 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/scss/index/_cta.scss
+-rwxr-xr-x   0        0        0     1674 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/scss/index/_faq.scss
+-rwxr-xr-x   0        0        0      981 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/scss/index/_featured-services.scss
+-rwxr-xr-x   0        0        0     1762 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/scss/index/_features.scss
+-rwxr-xr-x   0        0        0     2205 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/scss/index/_hero-animated.scss
+-rwxr-xr-x   0        0        0     1990 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/scss/index/_hero-fullscreen.scss
+-rwxr-xr-x   0        0        0     1764 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/scss/index/_hero-static.scss
+-rwxr-xr-x   0        0        0     3481 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/scss/index/_hero.scss
+-rwxr-xr-x   0        0        0     3798 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/scss/index/_onfocus.scss
+-rwxr-xr-x   0        0        0     2264 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/scss/index/_portfolio.scss
+-rwxr-xr-x   0        0        0     2551 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/scss/index/_pricing.scss
+-rwxr-xr-x   0        0        0     1512 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/scss/index/_recent-blog-posts.scss
+-rwxr-xr-x   0        0        0     1718 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/scss/index/_services.scss
+-rwxr-xr-x   0        0        0     1922 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/scss/index/_team.scss
+-rwxr-xr-x   0        0        0     2203 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/scss/index/_testimonials.scss
+-rwxr-xr-x   0        0        0      253 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/scss/main.scss
+-rwxr-xr-x   0        0        0     7960 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/scss/variables-blue.css
+-rwxr-xr-x   0        0        0     7957 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/scss/variables-green.css
+-rwxr-xr-x   0        0        0     7960 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/scss/variables-orange.css
+-rwxr-xr-x   0        0        0     7962 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/scss/variables-pink.css
+-rwxr-xr-x   0        0        0     7960 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/scss/variables-purple.css
+-rwxr-xr-x   0        0        0     7954 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/scss/variables-red.css
+-rwxr-xr-x   0        0        0     7953 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/scss/variables.css
+-rw-r--r--   0        0        0    19941 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/aos/aos.cjs.js
+-rw-r--r--   0        0        0    28765 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/aos/aos.css
+-rw-r--r--   0        0        0    19768 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/aos/aos.esm.js
+-rw-r--r--   0        0        0    13800 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/aos/aos.js
+-rw-r--r--   0        0        0    56459 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/aos/aos.js.map
+-rw-r--r--   0        0        0    98255 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap-icons/bootstrap-icons.css
+-rw-r--r--   0        0        0    52358 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap-icons/bootstrap-icons.json
+-rw-r--r--   0        0        0    85875 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap-icons/bootstrap-icons.min.css
+-rw-r--r--   0        0        0    57755 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap-icons/bootstrap-icons.scss
+-rw-r--r--   0        0        0   176032 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap-icons/fonts/bootstrap-icons.woff
+-rw-r--r--   0        0        0   130396 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap-icons/fonts/bootstrap-icons.woff2
+-rw-r--r--   0        0        0    70329 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-grid.css
+-rw-r--r--   0        0        0   203221 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-grid.css.map
+-rw-r--r--   0        0        0    51795 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-grid.min.css
+-rw-r--r--   0        0        0   115986 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-grid.min.css.map
+-rw-r--r--   0        0        0    70403 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-grid.rtl.css
+-rw-r--r--   0        0        0   203225 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-grid.rtl.css.map
+-rw-r--r--   0        0        0    51870 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-grid.rtl.min.css
+-rw-r--r--   0        0        0   116063 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-grid.rtl.min.css.map
+-rw-r--r--   0        0        0    12065 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-reboot.css
+-rw-r--r--   0        0        0   129371 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-reboot.css.map
+-rw-r--r--   0        0        0    10126 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-reboot.min.css
+-rw-r--r--   0        0        0    51369 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-reboot.min.css.map
+-rw-r--r--   0        0        0    12058 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-reboot.rtl.css
+-rw-r--r--   0        0        0   129386 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-reboot.rtl.css.map
+-rw-r--r--   0        0        0    10198 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css
+-rw-r--r--   0        0        0    63943 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css.map
+-rw-r--r--   0        0        0   107823 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-utilities.css
+-rw-r--r--   0        0        0   267535 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-utilities.css.map
+-rw-r--r--   0        0        0    85352 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-utilities.min.css
+-rw-r--r--   0        0        0   180381 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-utilities.min.css.map
+-rw-r--r--   0        0        0   107691 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-utilities.rtl.css
+-rw-r--r--   0        0        0   267476 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-utilities.rtl.css.map
+-rw-r--r--   0        0        0    85281 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css
+-rw-r--r--   0        0        0   180217 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css.map
+-rw-r--r--   0        0        0   281046 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap.css
+-rw-r--r--   0        0        0   679755 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap.css.map
+-rw-r--r--   0        0        0   232803 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap.min.css
+-rw-r--r--   0        0        0   589892 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap.min.css.map
+-rw-r--r--   0        0        0   280259 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap.rtl.css
+-rw-r--r--   0        0        0   679615 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap.rtl.css.map
+-rw-r--r--   0        0        0   232911 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap.rtl.min.css
+-rw-r--r--   0        0        0   589087 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap.rtl.min.css.map
+-rw-r--r--   0        0        0   207819 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/js/bootstrap.bundle.js
+-rw-r--r--   0        0        0   444579 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/js/bootstrap.bundle.js.map
+-rw-r--r--   0        0        0    80721 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/js/bootstrap.bundle.min.js
+-rw-r--r--   0        0        0   332090 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/js/bootstrap.bundle.min.js.map
+-rw-r--r--   0        0        0   135829 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/js/bootstrap.esm.js
+-rw-r--r--   0        0        0   305438 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/js/bootstrap.esm.js.map
+-rw-r--r--   0        0        0    73935 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/js/bootstrap.esm.min.js
+-rw-r--r--   0        0        0   222455 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/js/bootstrap.esm.min.js.map
+-rw-r--r--   0        0        0   145401 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/js/bootstrap.js
+-rw-r--r--   0        0        0   306606 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/js/bootstrap.js.map
+-rw-r--r--   0        0        0    60635 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/js/bootstrap.min.js
+-rw-r--r--   0        0        0   220561 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/js/bootstrap.min.js.map
+-rw-r--r--   0        0        0    17372 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/glightbox/css/glightbox.css
+-rw-r--r--   0        0        0    13749 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/glightbox/css/glightbox.min.css
+-rw-r--r--   0        0        0    52561 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/glightbox/css/plyr.css
+-rw-r--r--   0        0        0    45081 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/glightbox/css/plyr.min.css
+-rw-r--r--   0        0        0   109391 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/glightbox/js/glightbox.js
+-rw-r--r--   0        0        0    55880 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/glightbox/js/glightbox.min.js
+-rw-r--r--   0        0        0    91398 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/isotope-layout/isotope.pkgd.js
+-rw-r--r--   0        0        0    35445 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/isotope-layout/isotope.pkgd.min.js
+-rwxr-xr-x   0        0        0   238381 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/php-email-form/php-email-form.php
+-rwxr-xr-x   0        0        0     2734 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/php-email-form/validate.js
+-rw-r--r--   0        0        0    18436 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/swiper/swiper-bundle.min.css
+-rw-r--r--   0        0        0   149147 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/swiper/swiper-bundle.min.js
+-rw-r--r--   0        0        0   201656 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/swiper/swiper-bundle.min.js.map
+-rw-r--r--   0        0        0     2119 2024-05-23 01:03:12.820571 django_herobiz_dental-3.0.0/django_herobiz_dental/templates/herobizdental/_about.html
+-rw-r--r--   0        0        0      446 2024-05-23 01:03:12.832496 django_herobiz_dental-3.0.0/django_herobiz_dental/templates/herobizdental/_clients.html
+-rw-r--r--   0        0        0     2846 2024-04-12 02:19:51.757891 django_herobiz_dental-3.0.0/django_herobiz_dental/templates/herobizdental/_contact.html
+-rw-r--r--   0        0        0     1187 2024-05-23 01:03:12.808322 django_herobiz_dental-3.0.0/django_herobiz_dental/templates/herobizdental/_cta.html
+-rw-r--r--   0        0        0     1604 2024-05-23 01:03:12.794389 django_herobiz_dental-3.0.0/django_herobiz_dental/templates/herobizdental/_faq.html
+-rw-r--r--   0        0        0      794 2024-03-29 06:50:25.784512 django_herobiz_dental-3.0.0/django_herobiz_dental/templates/herobizdental/_featured-services.html
+-rw-r--r--   0        0        0     2051 2024-05-23 01:03:12.811227 django_herobiz_dental-3.0.0/django_herobiz_dental/templates/herobizdental/_features.html
+-rw-r--r--   0        0        0      993 2024-05-23 01:03:12.818117 django_herobiz_dental-3.0.0/django_herobiz_dental/templates/herobizdental/_hero-animated.html
+-rw-r--r--   0        0        0     1844 2024-05-23 01:03:12.824279 django_herobiz_dental-3.0.0/django_herobiz_dental/templates/herobizdental/_hero-carousel.html
+-rw-r--r--   0        0        0      878 2024-05-23 01:03:12.829507 django_herobiz_dental-3.0.0/django_herobiz_dental/templates/herobizdental/_hero-fullscreen.html
+-rw-r--r--   0        0        0      876 2024-05-23 01:03:12.805247 django_herobiz_dental-3.0.0/django_herobiz_dental/templates/herobizdental/_hero-static.html
+-rw-r--r--   0        0        0     2056 2024-05-23 01:03:12.816254 django_herobiz_dental-3.0.0/django_herobiz_dental/templates/herobizdental/_onfocus.html
+-rw-r--r--   0        0        0     1491 2024-05-23 01:03:12.826079 django_herobiz_dental-3.0.0/django_herobiz_dental/templates/herobizdental/_portfolio.html
+-rw-r--r--   0        0        0     1467 2024-05-23 01:03:12.827942 django_herobiz_dental-3.0.0/django_herobiz_dental/templates/herobizdental/_pricing.html
+-rw-r--r--   0        0        0     1181 2024-05-23 01:03:12.813800 django_herobiz_dental-3.0.0/django_herobiz_dental/templates/herobizdental/_recent-blog-posts.html
+-rw-r--r--   0        0        0     1002 2024-05-23 01:03:12.822567 django_herobiz_dental-3.0.0/django_herobiz_dental/templates/herobizdental/_services.html
+-rw-r--r--   0        0        0     1719 2024-05-23 01:03:12.800372 django_herobiz_dental-3.0.0/django_herobiz_dental/templates/herobizdental/_sidebar.html
+-rw-r--r--   0        0        0     1700 2024-05-23 01:03:12.831145 django_herobiz_dental-3.0.0/django_herobiz_dental/templates/herobizdental/_team.html
+-rw-r--r--   0        0        0     1357 2024-05-23 01:03:12.834219 django_herobiz_dental-3.0.0/django_herobiz_dental/templates/herobizdental/_testimonials.html
+-rwxr-xr-x   0        0        0    10578 2024-05-23 00:55:55.346226 django_herobiz_dental-3.0.0/django_herobiz_dental/templates/herobizdental/blog-details.html
+-rwxr-xr-x   0        0        0     2969 2024-05-21 23:49:19.877790 django_herobiz_dental-3.0.0/django_herobiz_dental/templates/herobizdental/blog.html
+-rw-r--r--   0        0        0      351 2024-05-23 00:36:35.194584 django_herobiz_dental-3.0.0/django_herobiz_dental/templates/herobizdental/breadcrumb.html
+-rw-r--r--   0        0        0     2225 2024-05-23 00:36:35.187021 django_herobiz_dental-3.0.0/django_herobiz_dental/templates/herobizdental/footer.html
+-rwxr-xr-x   0        0        0     1341 2024-03-12 00:49:58.000000 django_herobiz_dental-3.0.0/django_herobiz_dental/templates/herobizdental/forms/contact.php
+-rw-r--r--   0        0        0     1457 2024-05-23 00:36:35.199097 django_herobiz_dental-3.0.0/django_herobiz_dental/templates/herobizdental/header.html
+-rwxr-xr-x   0        0        0     5197 2024-05-23 00:36:35.183308 django_herobiz_dental-3.0.0/django_herobiz_dental/templates/herobizdental/index.html
+-rwxr-xr-x   0        0        0     2285 2024-05-23 00:55:55.340269 django_herobiz_dental-3.0.0/django_herobiz_dental/templates/herobizdental/portfolio-details.html
+-rwxr-xr-x   0        0        0    16287 2024-05-23 00:41:03.802323 django_herobiz_dental-3.0.0/django_herobiz_dental/templates/herobizdental/privacy.html
+-rw-r--r--   0        0        0     2076 2024-05-23 00:36:35.197131 django_herobiz_dental-3.0.0/django_herobiz_dental/templates/herobizdental/seo.html
+-rwxr-xr-x   0        0        0    16327 2024-05-23 00:41:03.806327 django_herobiz_dental-3.0.0/django_herobiz_dental/templates/herobizdental/terms.html
+-rw-r--r--   0        0        0        0 2023-03-21 07:32:09.033136 django_herobiz_dental-3.0.0/django_herobiz_dental/templatetags/__init__.py
+-rw-r--r--   0        0        0     6375 2024-05-23 00:36:35.176697 django_herobiz_dental-3.0.0/django_herobiz_dental/templatetags/herobizdental_tags.py
+-rw-r--r--   0        0        0       60 2024-04-05 06:12:24.811958 django_herobiz_dental-3.0.0/django_herobiz_dental/tests.py
+-rw-r--r--   0        0        0     1171 2024-05-23 00:20:12.258324 django_herobiz_dental-3.0.0/django_herobiz_dental/urls.py
+-rw-r--r--   0        0        0     7372 2024-05-22 23:59:16.806472 django_herobiz_dental-3.0.0/django_herobiz_dental/views.py
+-rw-r--r--   0        0        0      972 2024-05-22 23:59:16.813056 django_herobiz_dental-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0     5782 1970-01-01 00:00:00.000000 django_herobiz_dental-3.0.0/PKG-INFO
```

### Comparing `django_herobiz_dental-2.2.0/.DS_Store` & `django_herobiz_dental-3.0.0/.DS_Store`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/LICENSE` & `django_herobiz_dental-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/README.md` & `django_herobiz_dental-3.0.0/README.md`

 * *Files 1% similar despite different names*

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

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/admin.py` & `django_herobiz_dental-3.0.0/django_herobiz_dental/admin.py`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/forms.py` & `django_herobiz_dental-3.0.0/django_herobiz_dental/forms.py`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/migrations/0001_initial.py` & `django_herobiz_dental-3.0.0/django_herobiz_dental/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/migrations/0003_portfolio_client_post_profile.py` & `django_herobiz_dental-3.0.0/django_herobiz_dental/migrations/0003_portfolio_client_post_profile.py`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/models.py` & `django_herobiz_dental-3.0.0/django_herobiz_dental/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 from django.db import models
 from mdeditor.fields import MDTextField
 from _data.herobizdental import CATEGORY
+from _data import herobizdental
 from taggit.managers import TaggableManager
 from django.contrib.auth.models import User
 from hitcount.models import HitCount
 from django.contrib.contenttypes.fields import GenericRelation
 
+template_name = herobizdental.context['template_name']
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
 
-        return reverse("herobizdental:post_detail", kwargs={"slug": str(self.slug)})
+        return reverse(template_name + ':post_detail', kwargs={"slug": str(self.slug)})
 
 
 class Profile(models.Model):
     user = models.OneToOneField(User, on_delete=models.CASCADE)     # Delete profile when user is deleted
     image = models.ImageField(default='default_profile.jpg', upload_to='profile_pics')
 
     def __str__(self):
```

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/sitemaps.py` & `django_herobiz_dental-3.0.0/django_herobiz_dental/sitemaps.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 from django.contrib.sitemaps import Sitemap
 from .models import Post
 from django.urls import reverse
+from _data import herobizdental
+
+
+template_name = herobizdental.context['template_name']
 
 
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
-            'herobizdental:home',
+            template_name + ':home',
         ]
 
     def location(self, item):
         return reverse(item)
```

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/css/main.css` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/css/main.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/css/variables-blue.css` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/css/variables-blue.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/css/variables-green.css` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/css/variables-green.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/css/variables-orange.css` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/css/variables-orange.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/css/variables-pink.css` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/css/variables-pink.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/css/variables-purple.css` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/css/variables-purple.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/css/variables-red.css` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/css/variables-red.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/css/variables.css` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/css/variables.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/img/about-bg.png` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/img/about-bg.png`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/img/faq.jpg` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/img/faq.jpg`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/img/hero-bg.png` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/img/hero-bg.png`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/img/onfocus-content-bg.jpg` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/img/onfocus-content-bg.jpg`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/img/pricing-bg.jpg` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/img/pricing-bg.jpg`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/js/main.js` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/js/main.js`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/scss/_footer.scss` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/scss/_footer.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/scss/_general.scss` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/scss/_general.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/scss/_header.scss` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/scss/_header.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/scss/_index.scss` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/scss/_index.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/scss/_nav.scss` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/scss/_nav.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/scss/_portfolio-details.scss` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/scss/_portfolio-details.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/scss/blog/_comments.scss` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/scss/blog/_comments.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/scss/blog/_details.scss` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/scss/blog/_details.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/scss/blog/_pagination.scss` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/scss/blog/_pagination.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/scss/blog/_posts-list.scss` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/scss/blog/_posts-list.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/scss/blog/_sidebar.scss` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/scss/blog/_sidebar.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/scss/index/_about.scss` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/scss/index/_about.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/scss/index/_contact.scss` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/scss/index/_contact.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/scss/index/_cta.scss` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/scss/index/_cta.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/scss/index/_faq.scss` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/scss/index/_faq.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/scss/index/_featured-services.scss` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/scss/index/_featured-services.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/scss/index/_features.scss` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/scss/index/_features.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/scss/index/_hero-animated.scss` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/scss/index/_hero-animated.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/scss/index/_hero-fullscreen.scss` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/scss/index/_hero-fullscreen.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/scss/index/_hero-static.scss` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/scss/index/_hero-static.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/scss/index/_hero.scss` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/scss/index/_hero.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/scss/index/_onfocus.scss` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/scss/index/_onfocus.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/scss/index/_portfolio.scss` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/scss/index/_portfolio.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/scss/index/_pricing.scss` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/scss/index/_pricing.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/scss/index/_recent-blog-posts.scss` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/scss/index/_recent-blog-posts.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/scss/index/_services.scss` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/scss/index/_services.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/scss/index/_team.scss` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/scss/index/_team.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/scss/index/_testimonials.scss` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/scss/index/_testimonials.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/scss/variables-blue.css` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/scss/variables-blue.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/scss/variables-green.css` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/scss/variables-green.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/scss/variables-orange.css` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/scss/variables-orange.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/scss/variables-pink.css` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/scss/variables-pink.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/scss/variables-purple.css` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/scss/variables-purple.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/scss/variables-red.css` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/scss/variables-red.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/scss/variables.css` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/scss/variables.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/aos/aos.cjs.js` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/aos/aos.cjs.js`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/aos/aos.css` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/aos/aos.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/aos/aos.esm.js` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/aos/aos.esm.js`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/aos/aos.js` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/aos/aos.js`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/aos/aos.js.map` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/aos/aos.js.map`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap-icons/bootstrap-icons.css` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap-icons/bootstrap-icons.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap-icons/bootstrap-icons.json` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap-icons/bootstrap-icons.json`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap-icons/bootstrap-icons.min.css` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap-icons/bootstrap-icons.min.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap-icons/bootstrap-icons.scss` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap-icons/bootstrap-icons.scss`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap-icons/fonts/bootstrap-icons.woff` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap-icons/fonts/bootstrap-icons.woff`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap-icons/fonts/bootstrap-icons.woff2` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap-icons/fonts/bootstrap-icons.woff2`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-grid.css` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-grid.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-grid.css.map` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-grid.css.map`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-grid.min.css` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-grid.min.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-grid.min.css.map` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-grid.min.css.map`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-grid.rtl.css` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-grid.rtl.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-grid.rtl.css.map` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-grid.rtl.css.map`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-grid.rtl.min.css` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-grid.rtl.min.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-grid.rtl.min.css.map` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-grid.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-reboot.css` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-reboot.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-reboot.css.map` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-reboot.css.map`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-reboot.min.css` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-reboot.min.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-reboot.min.css.map` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-reboot.min.css.map`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-reboot.rtl.css` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-reboot.rtl.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-reboot.rtl.css.map` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-reboot.rtl.css.map`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css.map` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-reboot.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-utilities.css` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-utilities.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-utilities.css.map` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-utilities.css.map`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-utilities.min.css` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-utilities.min.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-utilities.min.css.map` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-utilities.min.css.map`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-utilities.rtl.css` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-utilities.rtl.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-utilities.rtl.css.map` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-utilities.rtl.css.map`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css.map` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap-utilities.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap.css` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap.css.map` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap.min.css` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap.min.css.map` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap.rtl.css` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap.rtl.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap.rtl.css.map` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap.rtl.css.map`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap.rtl.min.css` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap.rtl.min.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap.rtl.min.css.map` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/css/bootstrap.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/js/bootstrap.bundle.js` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/js/bootstrap.bundle.js`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/js/bootstrap.bundle.js.map` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/js/bootstrap.bundle.js.map`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/js/bootstrap.bundle.min.js` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/js/bootstrap.bundle.min.js.map` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/js/bootstrap.bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/js/bootstrap.esm.js` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/js/bootstrap.esm.js`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/js/bootstrap.esm.js.map` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/js/bootstrap.esm.js.map`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/js/bootstrap.esm.min.js` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/js/bootstrap.esm.min.js`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/js/bootstrap.esm.min.js.map` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/js/bootstrap.esm.min.js.map`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/js/bootstrap.js` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/js/bootstrap.js.map` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/js/bootstrap.js.map`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/js/bootstrap.min.js` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/js/bootstrap.min.js.map` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/bootstrap/js/bootstrap.min.js.map`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/glightbox/css/glightbox.css` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/glightbox/css/glightbox.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/glightbox/css/glightbox.min.css` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/glightbox/css/glightbox.min.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/glightbox/css/plyr.css` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/glightbox/css/plyr.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/glightbox/css/plyr.min.css` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/glightbox/css/plyr.min.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/glightbox/js/glightbox.js` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/glightbox/js/glightbox.js`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/glightbox/js/glightbox.min.js` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/glightbox/js/glightbox.min.js`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/isotope-layout/isotope.pkgd.js` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/isotope-layout/isotope.pkgd.js`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/isotope-layout/isotope.pkgd.min.js` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/isotope-layout/isotope.pkgd.min.js`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/php-email-form/php-email-form.php` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/php-email-form/php-email-form.php`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/php-email-form/validate.js` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/php-email-form/validate.js`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/swiper/swiper-bundle.min.css` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/swiper/swiper-bundle.min.css`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/swiper/swiper-bundle.min.js` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/swiper/swiper-bundle.min.js`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/static/herobizdental/vendor/swiper/swiper-bundle.min.js.map` & `django_herobiz_dental-3.0.0/django_herobiz_dental/static/herobizdental/vendor/swiper/swiper-bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/templates/herobizdental/_about.html` & `django_herobiz_dental-3.0.0/django_herobiz_dental/templates/herobizdental/_about.html`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 <style>
   .about .about-img:before {
   position: absolute;
   inset: -60px 0 0 -60px;
   z-index: -1;
   content: "";
-  background: url("{% static 'herobizdental/img/about-bg.png' %}") top left;
+  background: url("{% static template_name|add:'/img/about-bg.png' %}") top left;
   background-repeat: no-repeat;
 }
 </style>
 
 <section id="about" class="about">
   <div class="container" data-aos="fade-up">
 
@@ -19,15 +19,15 @@
       <p>{{ about_p }}</p>
     </div>
 
     <div class="row g-4 g-lg-5" data-aos="fade-up" data-aos-delay="200">
 
       <div class="col-lg-5">
         <div class="about-img">
-          <img src="{% static 'img/herobizdental/about/'|add:about_image' %}" class="img-fluid" alt="">
+          <img src="{% static 'img/'|add:template_name|add:'/about/'|add:about_image' %}" class="img-fluid" alt="">
         </div>
       </div>
 
       <div class="col-lg-7">
         {% autoescape off %}
         <h3 class="pt-0 pt-lg-5">{{ about_h3 }}</h3>
```

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/templates/herobizdental/_contact.html` & `django_herobiz_dental-3.0.0/django_herobiz_dental/templates/herobizdental/_contact.html`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/templates/herobizdental/_cta.html` & `django_herobiz_dental-3.0.0/django_herobiz_dental/templates/herobizdental/_cta.html`

 * *Files 9% similar despite different names*

```diff
@@ -20,15 +20,15 @@
           </div>
         </div>
         {% endautoescape %}
       </div>
 
       <div class="col-lg-4 col-md-6 order-first order-md-last d-flex align-items-center">
         <div class="img">
-          <img src="{% static 'img/herobizdental/cta/'|add:cta_image %}" alt="" class="img-fluid">
+          <img src="{% static 'img/'|add:template_name|add:'/cta/'|add:cta_image %}" alt="" class="img-fluid">
         </div>
       </div>
 
     </div>
 
   </div>
 </section>
```

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/templates/herobizdental/_faq.html` & `django_herobiz_dental-3.0.0/django_herobiz_dental/templates/herobizdental/_faq.html`

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
-      <div class="col-lg-5 align-items-stretch order-1 order-lg-2 img" style='background-image: url("{% static 'herobizdental/img/faq.jpg' %}");'>&nbsp;</div>
+      <div class="col-lg-5 align-items-stretch order-1 order-lg-2 img" style='background-image: url("{% static template_name|add:'/img/faq.jpg' %}");'>&nbsp;</div>
     </div>
   </div>
 </section>
```

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/templates/herobizdental/_featured-services.html` & `django_herobiz_dental-3.0.0/django_herobiz_dental/templates/herobizdental/_featured-services.html`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/templates/herobizdental/_features.html` & `django_herobiz_dental-3.0.0/django_herobiz_dental/templates/herobizdental/_features.html`

 * *Files 4% similar despite different names*

```diff
@@ -46,15 +46,15 @@
             </p>
           </div>
           {% if forloop.first %}
           <div class="col-lg-4 order-1 order-lg-2 text-center" data-aos="fade-up" data-aos-delay="200">
           {% else %}
           <div class="col-lg-4 order-1 order-lg-2 text-center">
           {% endif %}
-            <img src="{% static 'img/herobizdental/features/'|add:item.image %}" alt="" class="img-fluid">
+            <img src="{% static 'img/'|add:template_name|add:'/features/'|add:item.image %}" alt="" class="img-fluid">
           </div>
         </div>
       </div>
       {% endfor %}
     </div>
   </div>
 </section>
```

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/templates/herobizdental/_hero-animated.html` & `django_herobiz_dental-3.0.0/django_herobiz_dental/templates/herobizdental/_hero-animated.html`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 {% load static %}
 <style>
   .hero-animated {
   width: 100%;
   min-height: 50vh;
-  background: url("{% static 'herobizdental/img/hero-bg.png' %}") center center;
+  background: url("{% static template_name|add:'/img/hero-bg.png' %}") center center;
   background-size: cover;
   position: relative;
   padding: 120px 0 60px;
 }
 
 </style>
 <section id="hero-animated" class="hero-animated d-flex align-items-center">
   <div class="container d-flex flex-column justify-content-center align-items-center text-center position-relative" data-aos="zoom-out">
-    <img src="{% static 'img/herobizdental/hero/hero-animated.svg' %}" class="img-fluid animated">
+    <img src="{% static 'img/'|add:template_name|add:'/hero/hero-animated.svg' %}" class="img-fluid animated">
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
-[{% static 'img/herobizdental/hero/hero-animated.svg' %}]{% autoescape off %}
+[{% static 'img/'|add:template_name|add:'/hero/hero-animated.svg' %}]{%
+autoescape off %}
 ********** {{{{ hheerroo..ttiittllee }}}} **********
 {{ hero.slogan }}
 {% endautoescape %}
 _{_{_ _h_e_r_o_._b_t_n_._t_i_t_l_e_ _}_}
 _W_a_t_c_h_ _V_i_d_e_o
```

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/templates/herobizdental/_hero-carousel.html` & `django_herobiz_dental-3.0.0/django_herobiz_dental/templates/herobizdental/_hero-carousel.html`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 {% load static %}
 
 <style>
   .hero {
   width: 100%;
   padding: 0;
   background: #000000;
-  background: url("{% static 'herobizdental/img/hero-bg.png' %}") center center;
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
-              <img src="{% static 'img/herobizdental/hero-carousel/'|add:item.image' %}" alt="" class="img-fluid img">
+              <img src="{% static 'img/'|add:template_name|add:'/hero-carousel/'|add:item.image' %}" alt="" class="img-fluid img">
             </div>
 
             <div class="col-lg-9 text-center">
               {% autoescape off %}
               <h2>{{ item.title }}</h2>
               <p>{{ item.slogan }}</p>
               {% endautoescape %}
```

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/templates/herobizdental/_hero-fullscreen.html` & `django_herobiz_dental-3.0.0/django_herobiz_dental/templates/herobizdental/_hero-fullscreen.html`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 {% load static %}
 
 <style>
   .hero-fullscreen {
   width: 100%;
   min-height: 100vh;
-  background: url("{% static 'img/herobizdental/hero/hero-fullscreen-bg.jpg' %}") center center;
+  background: url("{% static 'img/'|add:template_name|add:'/hero/hero-fullscreen-bg.jpg' %}") center center;
   background-size: cover;
   position: relative;
   padding: 120px 0 60px;
 }
 </style>
 
 <section id="hero-fullscreen" class="hero-fullscreen d-flex align-items-center">
```

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/templates/herobizdental/_hero-static.html` & `django_herobiz_dental-3.0.0/django_herobiz_dental/templates/herobizdental/_hero-static.html`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 {% load static %}
 <style>
   .hero-static {
   width: 100%;
   min-height: 50vh;
-  background: url("{% static 'herobizdental/img/hero-bg.png' %}") center center;
+  background: url("{% static template_name|add:'/img/hero-bg.png' %}") center center;
   background-size: cover;
   position: relative;
   padding: 120px 0 60px;
 }
 </style>
 
 <section id="hero-static" class="hero-static d-flex align-items-center">
```

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/templates/herobizdental/_onfocus.html` & `django_herobiz_dental-3.0.0/django_herobiz_dental/templates/herobizdental/_onfocus.html`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 {% load static %}
 <style>
 .onfocus .video-play {
   min-height: 400px;
-  background: linear-gradient(rgba(0, 0, 0, 0.4), rgba(0, 0, 0, 0.7)), url("{% static 'img/herobizdental/onfocus/'|add:onfocus_image %}") center center;
+  background: linear-gradient(rgba(0, 0, 0, 0.4), rgba(0, 0, 0, 0.7)), url("{% static 'img/'|add:template_name|add:'/onfocus/'|add:onfocus_image %}") center center;
   background-size: cover;
 }
 
 .onfocus .content {
-  background: linear-gradient(rgba(72, 86, 100, 0.5), rgba(72, 86, 100, 0.8)), url("{% static 'herobizdental/img/onfocus-content-bg.jpg' %}") center center;
+  background: linear-gradient(rgba(72, 86, 100, 0.5), rgba(72, 86, 100, 0.8)), url("{% static template_name|add:'/img/onfocus-content-bg.jpg' %}") center center;
   background-size: cover;
   color: rgba(255, 255, 255, 0.8);
   padding: 40px;
 }
 
 </style>
 <section id="onfocus" class="onfocus">
```

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/templates/herobizdental/_portfolio.html` & `django_herobiz_dental-3.0.0/django_herobiz_dental/templates/herobizdental/_portfolio.html`

 * *Files 11% similar despite different names*

```diff
@@ -25,15 +25,15 @@
       <div class="row g-0 portfolio-container">
         {% for item in items.all %}
         <div class="col-xl-3 col-lg-4 col-md-6 portfolio-item filter-{{ item.filter }}">
           <img src="{{ item.image1.url }}" class="img-fluid" alt="">
           <div class="portfolio-info">
             <h4>{{ item.title }}</h4>
             <a href="{{ item.image1.url }}" title="{{ item.title }}" data-gallery="portfolio-gallery" class="glightbox preview-link"><i class="bi bi-zoom-in"></i></a>
-            <a href="{% url 'herobizdental:details' item.id %}" title="More Details" class="details-link" target="_blank"><i class="bi bi-link-45deg"></i></a>
+            <a href="{% url template_name|add:':details' item.id %}" title="More Details" class="details-link" target="_blank"><i class="bi bi-link-45deg"></i></a>
           </div>
         </div>
         {% endfor %}
       </div><!-- End Portfolio Container -->
     </div>
   </div>
 </section>
```

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/templates/herobizdental/_pricing.html` & `django_herobiz_dental-3.0.0/django_herobiz_dental/templates/herobizdental/_pricing.html`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 {% load static %}
 
 <style>
 .pricing .pricing-header {
-  background: linear-gradient(rgba(72, 86, 100, 0.9), rgba(72, 86, 100, 0.9)), url("{% static 'herobizdental/img/pricing-bg.jpg' %}") center center;
+  background: linear-gradient(rgba(72, 86, 100, 0.9), rgba(72, 86, 100, 0.9)), url("{% static template_name|add:'/img/pricing-bg.jpg' %}") center center;
   background-size: cover;
   text-align: center;
   padding: 40px;
   margin: -60px -40px 0;
 }
 </style>
```

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/templates/herobizdental/_recent-blog-posts.html` & `django_herobiz_dental-3.0.0/django_herobiz_dental/templates/herobizdental/_recent-blog-posts.html`

 * *Files 8% similar despite different names*

```diff
@@ -18,14 +18,14 @@
           </div>
           <div class="meta">
             <span class="post-date">{{ item.updated_on | date:"D, F d"}}</span>
             <span class="post-author"> / {{ item.author.last_name}} {{ item.author.first_name }}</span>
           </div>
           <h3 class="post-title">{{ item.title }}</h3>
           <p>{{ item.content | truncatechars:200 }}</p>
-          <a href="{% url 'herobizdental:post_detail' item.slug  %}" class="readmore stretched-link"><span>Read More</span><i class="bi bi-arrow-right"></i></a>
+          <a href="{% url template_name|add:':post_detail' item.slug  %}" class="readmore stretched-link"><span>Read More</span><i class="bi bi-arrow-right"></i></a>
         </div>
       </div>
       {% endfor %}
     </div>
   </div>
 </section>
```

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/templates/herobizdental/_services.html` & `django_herobiz_dental-3.0.0/django_herobiz_dental/templates/herobizdental/_services.html`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     </div>
 
     <div class="row gy-5">
       {% for item in services %}
       <div class="col-xl-4 col-md-6" data-aos="zoom-in" data-aos-delay="{% cycle '200' '300' '400' '500' '600' '700' %}">
         <div class="service-item">
           <div class="img">
-            <img src="{% static 'img/herobizdental/services/'|add:item.image %}" class="img-fluid" alt="">
+            <img src="{% static 'img/'|add:template_name|add:'/services/'|add:item.image %}" class="img-fluid" alt="">
           </div>
           <div class="details position-relative">
             <div class="icon">
               <i class="bi {{ item.icon }}"></i>
             </div>
             <a href="{{ item.link }}" class="stretched-link" target="_blank">
               <h3>{{ item.h3 }}</h3>
```

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/templates/herobizdental/_sidebar.html` & `django_herobiz_dental-3.0.0/django_herobiz_dental/templates/herobizdental/_sidebar.html`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 {% load herobizdental_tags %}
 {% load static %}
 
 <div class="sidebar">
 
   <div class="sidebar-item search-form">
     <h3 class="sidebar-title">Search</h3>
-    <form action="{% url 'herobizdental:search_result' %}" class="mt-3" method="get">
+    <form action="{% url template_name|add:':search_result' %}" class="mt-3" method="get">
       {{ form.q }}
       <button type="submit"><i class="bi bi-search"></i></button>
     </form>
   </div><!-- End sidebar search formn-->
 
   <div class="sidebar-item categories">
     <h3 class="sidebar-title">Categories</h3>
     <ul class="mt-3">
       {% for category_int, name, count in category %}
-      <li><a href="{% url 'herobizdental:category' category_int %}">{{ name }} <span>({{ count }})</span></a></li>
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
-          <h4><a href="{% url 'herobizdental:post_detail' l.slug %}">{{ l.title | truncatechars:30 }}</a></h4>
+          <h4><a href="{% url template_name|add:':post_detail' l.slug %}">{{ l.title | truncatechars:30 }}</a></h4>
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
-      <li><a href="{% url 'herobizdental:search_tag' tag %}">{{ tag }}</a></li>
+      <li><a href="{% url template_name|add:':search_tag' tag %}">{{ tag }}</a></li>
       {% endfor %}
     </ul>
   </div><!-- End sidebar tags-->
 
 </div>
```

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/templates/herobizdental/_team.html` & `django_herobiz_dental-3.0.0/django_herobiz_dental/templates/herobizdental/_team.html`

 * *Files 11% similar despite different names*

```diff
@@ -15,20 +15,20 @@
       <div class="col-xl-6 col-md-6 d-flex" data-aos="zoom-in" data-aos-delay="{% cycle '200' '400'%}">
       {% else %}
       <div class="col-xl-4 col-md-6 d-flex" data-aos="zoom-in" data-aos-delay="{% cycle '200' '400' '600' '800' '1000' '1200' %}">
       {% endif %}
         <div class="team-member">
           <div class="member-img">
             {% cycle 'member1' 'member2' 'member3' 'member4' 'member5' 'member6' as member_dir silent %}
-            <img src="{% static 'img/herobizdental/team/'|add:member_dir|add:'/profile.jpg' %}" class="img-fluid" alt="">
+            <img src="{% static 'img/'|add:template_name|add:'/team/'|add:member_dir|add:'/profile.jpg' %}" class="img-fluid" alt="">
           </div>
           <div class="member-info">
             <div class="social">
               {% for title, filename in member.certs %}
-              <a href="{% static 'img/herobizdental/team/'|add:member_dir|add:'/'|add:filename %}"
+              <a href="{% static 'img/'|add:template_name|add:'/team/'|add:member_dir|add:'/'|add:filename %}"
                  data-bs-toggle="tooltip" title="{{ title }}" class="glightbox">
               <i class="bi {% cycle 'bi-award' 'bi-hand-thumbs-up' 'bi-star' 'bi-tags' 'bi-magic' %}"></i>
               </a>
               {% endfor %}
             </div>
             <h4>{{ member.name }}</h4>
             <span>{{ member.title }}</span>
```

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/templates/herobizdental/_testimonials.html` & `django_herobiz_dental-3.0.0/django_herobiz_dental/templates/herobizdental/_testimonials.html`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 {% load static %}
 <style>
   .testimonials {
   padding: 80px 0;
-  background: url("{% static 'img/herobizdental/testimonials-bg.jpg' %}") no-repeat;
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
-            <img src="{% static 'img/herobizdental/testimonials/'|add:item.photo %}" class="testimonial-img" alt="">
+            <img src="{% static 'img/'|add:template_name|add:'/testimonials/'|add:item.photo %}" class="testimonial-img" alt="">
             <h3>{{ item.name }}</h3>
             {% autoescape off %}
             <h4>{{ item.job }}</h4>
             {% endautoescape %}
             <div class="stars">
               <i class="bi bi-star-fill"></i><i class="bi bi-star-fill"></i><i class="bi bi-star-fill"></i><i class="bi bi-star-fill"></i><i class="bi bi-star-fill"></i>
             </div>
```

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/templates/herobizdental/blog-details.html` & `django_herobiz_dental-3.0.0/django_herobiz_dental/templates/herobizdental/blog-details.html`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-{% extends "herobizdental/index.html" %}
+{% extends template_name|add:'/index.html' %}
 {% load static %}
 {% load herobizdental_tags %}
 {% load markdownify %}
 
 {% block content %}
   <main id="main">
-    <!-- ======= Breadcrumbs ======= -->{% include 'herobizdental/breadcrumb.html' %}<!-- End Breadcrumbs -->
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
-                  <li class="d-flex align-items-center"><i class="bi bi-person"></i> <a href="{% url 'herobizdental:post_detail' object.slug %}">{{ object.author.last_name }} {{ object.author.first_name }}</a></li>
-                  <li class="d-flex align-items-center"><i class="bi bi-clock"></i> <a href="{% url 'herobizdental:post_detail' object.slug %}"><time datetime="{{ object.updated_on | date:'Y-m-d' }}">{{ object.updated_on | date:"M d, Y" }}</time></a></li>
-                  <!-- <li class="d-flex align-items-center"><i class="bi bi-chat-dots"></i> <a href="{% url 'herobizdental:post_detail' object.slug %}">12 Comments</a></li> -->
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
-                  <li><a href="{% url 'herobizdental:category' object.category %}">{{ category_name }}</a></li>
+                  <li><a href="{% url template_name|add:':category' object.category %}">{{ category_name }}</a></li>
                 </ul>
 
                 <i class="bi bi-tags"></i>
                 <ul class="tags">
                   {% for tag in object.tags.all %}
-                  <li><a href="{% url 'herobizdental:search_tag' tag %}">{{ tag }}</a></li>
+                  <li><a href="{% url template_name|add:':search_tag' tag %}">{{ tag }}</a></li>
                   {% endfor %}
                 </ul>
               </div><!-- End meta bottom -->
 
             </article><!-- End blog post -->
 
             <div class="post-author d-flex align-items-center">
-              <img src="{% static 'img/herobizdental/blog-author.jpg' %}" class="rounded-circle flex-shrink-0" alt="">
+              <img src="{% static 'img/'|add:template_name|add:'/blog-author.jpg' %}" class="rounded-circle flex-shrink-0" alt="">
               <div>
                 <h4>{{ author.name }}</h4>
                 <div class="social-links">
                   {% if author.social.twitter %}
                   <a href="{{ author.social.twitter }}" target="_blank"><i class="bi bi-twitter"></i></a>
                   {% endif %}
                   {% if author.social.facebook %}
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
-{% extends "herobizdental/index.html" %} {% load static %} {% load
+{% extends template_name|add:'/index.html' %} {% load static %} {% load
 herobizdental_tags %} {% load markdownify %} {% block content %} {% include
-'herobizdental/breadcrumb.html' %}
+template_name|add:'/breadcrumb.html' %}
 ********** {{{{ oobbjjeecctt..ttiittllee }}}} **********
     * _{_{_ _o_b_j_e_c_t_._a_u_t_h_o_r_._l_a_s_t___n_a_m_e_ _}_}_ _{_{_ _o_b_j_e_c_t_._a_u_t_h_o_r_._f_i_r_s_t___n_a_m_e_ _}_}
     * _{_{_ _o_b_j_e_c_t_._u_p_d_a_t_e_d___o_n_ _|_ _d_a_t_e_:_"_M_ _d_,_ _Y_"_ _}_}
 {{ object.content | markdownify }}
     * _{_{_ _c_a_t_e_g_o_r_y___n_a_m_e_ _}_}
     * {% for tag in object.tags.all %}
     * _{_{_ _t_a_g_ _}_}
```

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/templates/herobizdental/blog.html` & `django_herobiz_dental-3.0.0/django_herobiz_dental/templates/herobizdental/blog.html`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/templates/herobizdental/footer.html` & `django_herobiz_dental-3.0.0/django_herobiz_dental/templates/herobizdental/footer.html`

 * *Files 4% similar despite different names*

```diff
@@ -4,16 +4,16 @@
     <div class="footer-legal text-center">
       <div class="container d-flex flex-column flex-lg-row justify-content-center justify-content-lg-between align-items-center">
 
         <div class="d-flex flex-column align-items-center align-items-lg-start">
           <div class="copyright">
           &copy; Copyright <a href="https://demiansoft.com" target="_blank"><strong><span>Demiansoft</span></strong></a>
             <a href="https://map.naver.com/v5/entry/place/13289684?c=15,0,0,0,dh" target="_blank">.</a> All Rights Reserved |
-            <a href="{% url 'herobizdental:terms' %}"> 이용약관</a> |
-            <a href="{% url 'herobizdental:privacy' %}"> 개인정보처리방침</a>
+            <a href="{% url template_name|add:':terms' %}"> 이용약관</a> |
+            <a href="{% url template_name|add:':privacy' %}"> 개인정보처리방침</a>
         </div>
         <div class="credits">
           {{ basic_info.company_name }} | {{ basic_info.owner}} | {{ basic_info.addr }} | 사업자등록번호: {{ basic_info.business_reg_number }}
         </div>
 
         </div>
```

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/templates/herobizdental/forms/contact.php` & `django_herobiz_dental-3.0.0/django_herobiz_dental/templates/herobizdental/forms/contact.php`

 * *Files identical despite different names*

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/templates/herobizdental/header.html` & `django_herobiz_dental-3.0.0/django_herobiz_dental/templates/herobizdental/header.html`

 * *Files 23% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 {% load static %}
 {% load django_utilsds_tags %}
 
 <header id="header" class="header fixed-top" data-scrollto-offset="0">
   <div class="container-fluid d-flex align-items-center justify-content-between">
-    <a href="{% url 'herobizdental:home' %}" class="logo d-flex align-items-center scrollto me-auto me-lg-0">
+    <a href="{% url template_name|add:':home' %}" class="logo d-flex align-items-center scrollto me-auto me-lg-0">
       {% if use_logo %}
-      <img src="{% static 'img/herobizdental/logo/'|add:logo_text|add:'.png' %}" alt="">
+      <img src="{% static 'img/'|add:template_name|add:'/logo/'|add:logo_text|add:'.png' %}" alt="">
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
-              <li><a class="nav-link scrollto" href="{% url 'herobizdental:home' %}#{{ component | underscore_to_hyphen }}">{{ title }}</a></li>
+              <li><a class="nav-link scrollto" href="{% url template_name|add:':home' %}#{{ component | underscore_to_hyphen }}">{{ title }}</a></li>
             {% endif %}
           {% endif %}
         {% endfor %}
       </ul>
       <i class="bi bi-list mobile-nav-toggle d-none"></i>
     </nav><!-- .navbar -->
     {% for component, is_use, _, _ in components %}
     {% if component == menu_btn.component and is_use %}
-    <a class="btn-getstarted scrollto" href="{% url 'herobizdental:home' %}#{{ menu_btn.component }}">{{ menu_btn.title }}</a>
+    <a class="btn-getstarted scrollto" href="{% url template_name|add:':home' %}#{{ menu_btn.component }}">{{ menu_btn.title }}</a>
     {% endif %}
     {% endfor %}
   </div>
 </header>
```

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/templates/herobizdental/index.html` & `django_herobiz_dental-3.0.0/django_herobiz_dental/templates/herobizdental/index.html`

 * *Files 14% similar despite different names*

```diff
@@ -4,40 +4,40 @@
 {% load django_modalds_tags %}
 {% load django_analyticsds_tags %}
 
 <!DOCTYPE html>
 <html lang="en">
 
 <head>
-  <!-- ======= SEO ======= -->{% include 'herobizdental/seo.html' %}<!-- End SEO -->
+  <!-- ======= SEO ======= -->{% seo %}<!-- End SEO -->
 
   <!-- Vendor CSS Files -->
   <link rel="stylesheet"
-        href="{% static 'herobizdental/vendor/bootstrap/css/bootstrap.min.css' %}" crossorigin="anonymous">
-  <link rel="stylesheet" href="{% static 'herobizdental/vendor/bootstrap-icons/bootstrap-icons.min.css' %}">
-  <link href="{% static 'herobizdental/vendor/aos/aos.css' %}" rel="stylesheet">
-  <link href="{% static 'herobizdental/vendor/glightbox/css/glightbox.min.css' %}" rel="stylesheet">
-  <link href="{% static 'herobizdental/vendor/swiper/swiper-bundle.min.css' %}" rel="stylesheet">
+        href="{% static template_name|add:'/vendor/bootstrap/css/bootstrap.min.css' %}" crossorigin="anonymous">
+  <link rel="stylesheet" href="{% static template_name|add:'/vendor/bootstrap-icons/bootstrap-icons.min.css' %}">
+  <link href="{% static template_name|add:'/vendor/aos/aos.css' %}" rel="stylesheet">
+  <link href="{% static template_name|add:'/vendor/glightbox/css/glightbox.min.css' %}" rel="stylesheet">
+  <link href="{% static template_name|add:'/vendor/swiper/swiper-bundle.min.css' %}" rel="stylesheet">
 
   <!-- Variables CSS Files. Uncomment your preferred color scheme -->
-  <link href="{% static 'herobizdental/css/variables'|add:color|add:'.css' %}" rel="stylesheet">
-  <!-- <link href="{% static 'herobizdental/css/variables-blue.css' %}" rel="stylesheet"> -->
-  <!-- <link href="{% static 'herobizdental/css/variables-green.css' %}" rel="stylesheet"> -->
-  <!-- <link href="{% static 'herobizdental/css/variables-orange.css' %}" rel="stylesheet"> -->
-  <!-- <link href="{% static 'herobizdental/css/variables-purple.css' %}" rel="stylesheet"> -->
-  <!-- <link href="{% static 'herobizdental/css/variables-red.css' %}" rel="stylesheet"> -->
-  <!-- <link href="{% static 'herobizdental/css/variables-pink.css' %}" rel="stylesheet"> -->
+  <link href="{% static template_name|add:'/css/variables'|add:color|add:'.css' %}" rel="stylesheet">
+  <!-- <link href="{% static template_name|add:'/css/variables-blue.css' %}" rel="stylesheet"> -->
+  <!-- <link href="{% static template_name|add:'/css/variables-green.css' %}" rel="stylesheet"> -->
+  <!-- <link href="{% static template_name|add:'/css/variables-orange.css' %}" rel="stylesheet"> -->
+  <!-- <link href="{% static template_name|add:'/css/variables-purple.css' %}" rel="stylesheet"> -->
+  <!-- <link href="{% static template_name|add:'/css/variables-red.css' %}" rel="stylesheet"> -->
+  <!-- <link href="{% static template_name|add:'/css/variables-pink.css' %}" rel="stylesheet"> -->
 
   <!-- Template Main CSS File -->
-  <link href="{% static 'herobizdental/css/main.css' %}" rel="stylesheet">
+  <link href="{% static template_name|add:'/css/main.css' %}" rel="stylesheet">
 
 </head>
 
 <body>
-  <!-- ======= Header ======= -->{% include 'herobizdental/header.html' %}<!-- End Header -->
+  <!-- ======= Header ======= -->{% header %}<!-- End Header -->
   {% block content %}
   <!-- ======= Hero Section ======= -->{% hero %}<!-- End Hero -->
 
   <main id="main">
     {% show_calendar %}
     {% show_modal %}
     {% make_analytics %}
@@ -74,26 +74,26 @@
           <!-- ======= Contact Section ======= -->{% contact %}<!-- End Contact Section -->
         {% endif %}
       {% endif %}
     {% endfor %}
   </main><!-- End #main -->
   {% endblock content %}
 
-  <!-- ======= Footer ======= -->{% include 'herobizdental/footer.html' %}<!-- End Footer -->
+  <!-- ======= Footer ======= -->{% footer %}<!-- End Footer -->
 
   <a href="#" class="scroll-top d-flex align-items-center justify-content-center"><i class="bi bi-arrow-up-short"></i></a>
 
   <div id="preloader"></div>
 
   <!-- Vendor JS Files -->
-  <script src="{% static 'herobizdental/vendor/bootstrap/js/bootstrap.bundle.min.js' %}"
+  <script src="{% static template_name|add:'/vendor/bootstrap/js/bootstrap.bundle.min.js' %}"
           crossorigin="anonymous"></script>
-  <script src="{% static 'herobizdental/vendor/aos/aos.js' %}"></script>
-  <script src="{% static 'herobizdental/vendor/glightbox/js/glightbox.min.js' %}"></script>
-  <script src="{% static 'herobizdental/vendor/isotope-layout/isotope.pkgd.min.js' %}"></script>
-  <script src="{% static 'herobizdental/vendor/swiper/swiper-bundle.min.js' %}"></script>
-  <!-- <script src="{% static 'herobizdental/vendor/php-email-form/validate.js' %}"></script> -->
+  <script src="{% static template_name|add:'/vendor/aos/aos.js' %}"></script>
+  <script src="{% static template_name|add:'/vendor/glightbox/js/glightbox.min.js' %}"></script>
+  <script src="{% static template_name|add:'/vendor/isotope-layout/isotope.pkgd.min.js' %}"></script>
+  <script src="{% static template_name|add:'/vendor/swiper/swiper-bundle.min.js' %}"></script>
+  <!-- <script src="{% static template_name|add:'/vendor/php-email-form/validate.js' %}"></script> -->
 
   <!-- Template Main JS File -->
-  <script src="{% static 'herobizdental/js/main.js' %}"></script>
+  <script src="{% static template_name|add:'/js/main.js' %}"></script>
 </body>
 </html>
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
 {% load static %} {% load herobizdental_tags %} {% load django_calendards_tags
 %} {% load django_modalds_tags %} {% load django_analyticsds_tags %}
-{% include 'herobizdental/seo.html' %}
-{% include 'herobizdental/header.html' %} {% block content %} {% hero %} {%
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
-endfor %} {% endblock content %} {% include 'herobizdental/footer.html' %}
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

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/templates/herobizdental/privacy.html` & `django_herobiz_dental-3.0.0/django_herobiz_dental/templates/herobizdental/privacy.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-{% extends "herobizdental/index.html" %}
+{% extends template_name|add:'/index.html' %}
 {% load static %}
 
 {% block content %}
 <main id="main">
-  <!-- ======= Breadcrumbs ======= -->{% include 'herobizdental/breadcrumb.html' %}<!-- End Breadcrumbs -->
+  <!-- ======= Breadcrumbs ======= -->{% include template_name|add:'/breadcrumb.html' %}<!-- End Breadcrumbs -->
 
   <!-- ======= Blog Section ======= -->
   <section class="inner-page">
     <div class="container" data-aos="fade-up">
 
       <div class="section-header">
         <h2>개인정보처리방침</h2>
```

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/templates/herobizdental/seo.html` & `django_herobiz_dental-3.0.0/django_herobiz_dental/templates/herobizdental/seo.html`

 * *Files 14% similar despite different names*

```diff
@@ -5,30 +5,30 @@
 <meta content="width=device-width, initial-scale=1.0" name="viewport">
 
 <title>{{ seo.company_name }} | {{ seo.small_title }}</title>
 <meta name="description" content="{{ seo.desc }}">
 <meta name="keywords" content="{{ seo.keywords }}">
 
 <meta property="og:url" content="https://{{ seo.url }}">
-<meta property="og:image" itemprop="image primaryImageOfPage" content="{% static 'img/herobizdental/favicon.png' %}">
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
-<link rel="icon" type="image/png" sizes="32x32" href="{% static 'img/herobizdental/favicon.png' %}">
-<link rel="shortcut icon" sizes="16x16 24x24 32x32 48x48" href="{% static 'img/herobizdental/favicon.ico' %}">
-<link rel="apple-touch-icon" sizes="180x180" href="{% static 'img/herobizdental/apple-touch-icon.png' %}">
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

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/templates/herobizdental/terms.html` & `django_herobiz_dental-3.0.0/django_herobiz_dental/templates/herobizdental/terms.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-{% extends "herobizdental/index.html" %}
+{% extends template_name|add:'/index.html' %}
 {% load static %}
 
 {% block content %}
 <main id="main">
-  <!-- ======= Breadcrumbs ======= -->{% include 'herobizdental/breadcrumb.html' %}<!-- End Breadcrumbs -->
+  <!-- ======= Breadcrumbs ======= -->{% include template_name|add:'/breadcrumb.html' %}<!-- End Breadcrumbs -->
 
   <!-- ======= Blog Section ======= -->
   <section class="inner-page">
     <div class="container" data-aos="fade-up">
 
       <div class="section-header">
         <h2>이용약관</h2>
```

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/templatetags/herobizdental_tags.py` & `django_herobiz_dental-3.0.0/django_herobiz_dental/templatetags/herobizdental_tags.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from django.template import Library, loader
 from ..models import Post
 from ..models import Portfolio, Category
 from taggit.models import Tag
 from _data.herobizdental import CATEGORY
 from ..forms import SearchForm
+from _data import herobizdental
+
 
 import logging
 logger = logging.getLogger(__name__)
 formatter = logging.Formatter('%(levelname)s: [%(name)s] %(message)s')
 ch = logging.StreamHandler()
 ch.setFormatter(formatter)
 logger.addHandler(ch)
@@ -15,174 +17,210 @@
 
 
 register = Library()
 
 # https://localcoder.org/django-inclusion-tag-with-configurable-template
 
 
+template_name = herobizdental.context['template_name']
+
+
 @register.simple_tag(takes_context=True)
-def hero(context):
-    t = loader.get_template(f"herobizdental/_hero-{context['hero_type']}.html")
+def seo(context):
+    t = loader.get_template(template_name + "/seo.html")
     context.update({
+        'template_name': template_name,
+    })
+    logger.info(context)
+    return t.render(context.flatten())
 
+
+@register.simple_tag(takes_context=True)
+def header(context):
+    t = loader.get_template(template_name + "/header.html")
+    context.update({
+        'template_name': template_name,
     })
     logger.info(context)
     return t.render(context.flatten())
 
 
 @register.simple_tag(takes_context=True)
-def featured_services(context):
-    t = loader.get_template("herobizdental/_featured-services.html")
+def hero(context):
+    t = loader.get_template(template_name + f"/_hero-{context['hero_type']}.html")
     context.update({
+        'template_name': template_name,
+    })
+    logger.info(context)
+    return t.render(context.flatten())
+
 
+@register.simple_tag(takes_context=True)
+def featured_services(context):
+    t = loader.get_template(template_name + "/_featured-services.html")
+    context.update({
+        'template_name': template_name,
     })
     logger.info(context)
     return t.render(context.flatten())
 
 
 @register.simple_tag(takes_context=True)
 def about(context):
-    t = loader.get_template("herobizdental/_about.html")
+    t = loader.get_template(template_name + "/_about.html")
     context.update({
-
+        'template_name': template_name,
     })
     logger.info(context)
     return t.render(context.flatten())
 
 
 @register.simple_tag(takes_context=True)
 def clients(context):
-    t = loader.get_template("herobizdental/_clients.html")
+    t = loader.get_template(template_name + "/_clients.html")
     context.update({
-
+        'template_name': template_name,
     })
     logger.info(context)
     return t.render(context.flatten())
 
 
 @register.simple_tag(takes_context=True)
 def cta(context):
-    t = loader.get_template("herobizdental/_cta.html")
+    t = loader.get_template(template_name + "/_cta.html")
     context.update({
-
+        'template_name': template_name,
     })
     logger.info(context)
     return t.render(context.flatten())
 
 
 @register.simple_tag(takes_context=True)
 def onfocus(context):
-    t = loader.get_template("herobizdental/_onfocus.html")
+    t = loader.get_template(template_name + "/_onfocus.html")
     context.update({
-
+        'template_name': template_name,
     })
     logger.info(context)
     return t.render(context.flatten())
 
 
 @register.simple_tag(takes_context=True)
 def features(context):
-    t = loader.get_template("herobizdental/_features.html")
+    t = loader.get_template(template_name + "/_features.html")
     context.update({
-
+        'template_name': template_name,
     })
     logger.info(context)
     return t.render(context.flatten())
 
 
 @register.simple_tag(takes_context=True)
 def services(context):
-    t = loader.get_template("herobizdental/_services.html")
+    t = loader.get_template(template_name + "/_services.html")
     context.update({
-
+        'template_name': template_name,
     })
     logger.info(context)
     return t.render(context.flatten())
 
 
 @register.simple_tag(takes_context=True)
 def testimonials(context):
-    t = loader.get_template("herobizdental/_testimonials.html")
+    t = loader.get_template(template_name + "/_testimonials.html")
     context.update({
-
+        'template_name': template_name,
     })
     logger.info(context)
     return t.render(context.flatten())
 
 
 @register.simple_tag(takes_context=True)
 def pricing(context):
-    t = loader.get_template("herobizdental/_pricing.html")
+    t = loader.get_template(template_name + "/_pricing.html")
     context.update({
-
+        'template_name': template_name,
     })
     logger.info(context)
     return t.render(context.flatten())
 
 
 @register.simple_tag(takes_context=True)
 def faq(context):
-    t = loader.get_template("herobizdental/_faq.html")
+    t = loader.get_template(template_name + "/_faq.html")
     context.update({
-
+        'template_name': template_name,
     })
     logger.info(context)
     return t.render(context.flatten())
 
 
 @register.simple_tag(takes_context=True)
 def portfolio(context):
-    t = loader.get_template("herobizdental/_portfolio.html")
+    t = loader.get_template(template_name + "/_portfolio.html")
     context.update({
+        'template_name': template_name,
         'categories': Category.objects,
         'items': Portfolio.objects,
     })
     logger.info(context)
     return t.render(context.flatten())
 
 
 @register.simple_tag(takes_context=True)
 def team(context):
-    t = loader.get_template("herobizdental/_team.html")
+    t = loader.get_template(template_name + "/_team.html")
     context.update({
-
+        'template_name': template_name,
     })
     logger.info(context)
     return t.render(context.flatten())
 
 
 @register.simple_tag(takes_context=True)
 def recent_blog_posts(context):
-    t = loader.get_template("herobizdental/_recent-blog-posts.html")
+    t = loader.get_template(template_name + "/_recent-blog-posts.html")
     objects = Post.objects.filter(status=1).filter(remarkable=True).order_by('-updated_on')
     context.update({
+        'template_name': template_name,
         'top3': objects[:3],
     })
     logger.info(context)
     return t.render(context.flatten())
 
 
 @register.simple_tag(takes_context=True)
 def contact(context):
-    t = loader.get_template("herobizdental/_contact.html")
+    t = loader.get_template(template_name + "/_contact.html")
     context.update({
-
+        'template_name': template_name,
     })
     logger.info(context)
     return t.render(context.flatten())
 
 
 @register.simple_tag(takes_context=True)
 def sidebar(context):
-    t = loader.get_template(f"herobizdental/_sidebar.html")
+    t = loader.get_template(template_name + "/_sidebar.html")
     tags = Tag.objects.all()
     category = []
     for category_int, name in CATEGORY:
         category.append([category_int, name, Post.objects.filter(status=1).filter(category=category_int).count()])
     context.update({
+        'template_name': template_name,
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

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/urls.py` & `django_herobiz_dental-3.0.0/django_herobiz_dental/urls.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from django.urls import path, include
 from django.contrib.sitemaps.views import sitemap
 from . import views
 from .sitemaps import PostSitemap, StaticViewSitemap
+from _data import herobizdental
 
-app_name = 'herobizdental'
+app_name = herobizdental.context['template_name']
 
 sitemaps = {
     "posts": PostSitemap,
     'static': StaticViewSitemap,
 }
 
 urlpatterns = [
```

### Comparing `django_herobiz_dental-2.2.0/django_herobiz_dental/views.py` & `django_herobiz_dental-3.0.0/django_herobiz_dental/views.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from django.shortcuts import render, get_object_or_404
 from django_utilsds import utils
 from .forms import AppointmentForm
 from _data import herobizdental
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
 
+template_name = herobizdental.context['template_name']
+c = herobizdental.context
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
-    c = herobizdental.context
-
     logger.info(c)
     if request.method == 'GET':
         c.update({'form': AppointmentForm()})
         c['post_message'] = None
-        return render(request, 'herobizdental/index.html', c)
+        return render(request, template_name + '/index.html', c)
     elif request.method == "POST":
         c.update(make_post_context(request.POST, c['basic_info']['consult_email']))
-        return render(request, 'herobizdental/index.html', c)
+        return render(request, template_name + '/index.html', c)
 
 
 def make_post_context(request_post, consult_mail):
     logger.info(request_post)
     context = {}
     # appointment 앱에서 post 요청을 처리함.
     logger.info(f'request.POST : {request_post}')
@@ -69,45 +71,42 @@
     else:
         logger.error('Fail form validation test')
         context['post_message'] = '입력 항목이 유효하지 않습니다. 다시 입력해 주십시요.'
         return context
 
 
 def details(request, id: int):
-    c = herobizdental.context
     c.update(
         {
             "obj": get_object_or_404(Portfolio, pk=id),
             "breadcrumb": {
                 "title": c['portfolio']['title'],
             },
         }
     )
     logger.debug(c)
-    return render(request, "herobizdental/portfolio-details.html", c)
+    return render(request, template_name + '/portfolio-details.html', c)
 
 
 def terms(request):
-    c = herobizdental.context
     c.update(
         {
             "breadcrumb": {
                 "title": "Terms of Use",
             },
             "terms": {
                 "company_name": c['basic_info']['company_name'],
                 "sdate": c['basic_info']['sdate'],
             },
         }
     )
-    return render(request, "herobizdental/terms.html", c)
+    return render(request, template_name + '/terms.html', c)
 
 
 def privacy(request):
-    c = herobizdental.context
     c.update(
         {
             "breadcrumb": {
                 "title": "Privacy Policy",
             },
             "privacy": {
                 "company_name": c['basic_info']['company_name'],
@@ -116,46 +115,46 @@
                 "position": "담당자",
                 "phone": c['basic_info']['phone'],
                 "email": c['basic_info']['owner_email'],
                 "sdate": c['basic_info']['sdate'],
             },
         }
     )
-    return render(request, "herobizdental/privacy.html", c)
+    return render(request, template_name + '/privacy.html', c)
 
 
 class PostDetailView(HitCountDetailView):
     model = Post
-    template_name = 'herobizdental/blog-details.html'
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
 
-        context.update(herobizdental.context)
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
-    template_name = 'herobizdental/blog.html'
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
 
-        context.update(herobizdental.context)
+        context.update(c)
         return context
 
 
 class Blog(SearchResult):
     # 홈페이지에서 다이렉트 링크로 연결하기 위해서 필요하다.
     def get_queryset(self):
         # https://stackoverflow.com/questions/56067365/how-to-filter-posts-by-tags-using-django-taggit-in-django
```

### Comparing `django_herobiz_dental-2.2.0/pyproject.toml` & `django_herobiz_dental-3.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "django_herobiz_dental"
-version = "2.2.0"
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
     "django-mdeditor >= 0.1.20",
     "django-hitcount >= 1.3.5",
     "django-taggit >= 5.0.1",
     "django-markdownify >= 0.9.3",
     "django-light >= 0.1.0",
     "pillow >= 10.3.0",
 ]
```

### Comparing `django_herobiz_dental-2.2.0/PKG-INFO` & `django_herobiz_dental-3.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: django_herobiz_dental
-Version: 2.2.0
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

