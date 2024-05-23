# Comparing `tmp/django_env_robots-0.0.1.tar.gz` & `tmp/django_env_robots-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_env_robots-0.0.1.tar", last modified: Thu May 23 11:42:41 2024, max compression
+gzip compressed data, was "django_env_robots-0.0.2.tar", last modified: Thu May 23 14:10:56 2024, max compression
```

## Comparing `django_env_robots-0.0.1.tar` & `django_env_robots-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 patsmith   (501) staff       (20)        0 2024-05-23 11:42:41.569227 django_env_robots-0.0.1/
--rw-r--r--   0 patsmith   (501) staff       (20)     1064 2024-05-22 15:42:15.000000 django_env_robots-0.0.1/LICENSE
--rw-r--r--   0 patsmith   (501) staff       (20)        0 2024-05-23 11:37:41.000000 django_env_robots-0.0.1/MANIFEST.in
--rw-r--r--   0 patsmith   (501) staff       (20)     2728 2024-05-23 11:42:41.568673 django_env_robots-0.0.1/PKG-INFO
--rw-r--r--   0 patsmith   (501) staff       (20)      930 2024-05-23 09:35:52.000000 django_env_robots-0.0.1/README.md
-drwxr-xr-x   0 patsmith   (501) staff       (20)        0 2024-05-23 11:42:41.565838 django_env_robots-0.0.1/django_env_robots/
--rw-r--r--   0 patsmith   (501) staff       (20)       21 2024-05-22 15:58:37.000000 django_env_robots-0.0.1/django_env_robots/__init__.py
--rw-r--r--   0 patsmith   (501) staff       (20)      155 2024-05-22 15:56:56.000000 django_env_robots-0.0.1/django_env_robots/apps.py
--rw-r--r--   0 patsmith   (501) staff       (20)       57 2024-05-22 15:23:46.000000 django_env_robots-0.0.1/django_env_robots/models.py
--rw-r--r--   0 patsmith   (501) staff       (20)       60 2024-05-22 15:23:46.000000 django_env_robots-0.0.1/django_env_robots/tests.py
--rw-r--r--   0 patsmith   (501) staff       (20)      115 2024-05-22 16:16:15.000000 django_env_robots-0.0.1/django_env_robots/urls.py
--rw-r--r--   0 patsmith   (501) staff       (20)     1121 2024-05-22 16:24:08.000000 django_env_robots-0.0.1/django_env_robots/views.py
-drwxr-xr-x   0 patsmith   (501) staff       (20)        0 2024-05-23 11:42:41.568005 django_env_robots-0.0.1/django_env_robots.egg-info/
--rw-r--r--   0 patsmith   (501) staff       (20)     2728 2024-05-23 11:42:41.000000 django_env_robots-0.0.1/django_env_robots.egg-info/PKG-INFO
--rw-r--r--   0 patsmith   (501) staff       (20)      412 2024-05-23 11:42:41.000000 django_env_robots-0.0.1/django_env_robots.egg-info/SOURCES.txt
--rw-r--r--   0 patsmith   (501) staff       (20)        1 2024-05-23 11:42:41.000000 django_env_robots-0.0.1/django_env_robots.egg-info/dependency_links.txt
--rw-r--r--   0 patsmith   (501) staff       (20)       12 2024-05-23 11:42:41.000000 django_env_robots-0.0.1/django_env_robots.egg-info/requires.txt
--rw-r--r--   0 patsmith   (501) staff       (20)       18 2024-05-23 11:42:41.000000 django_env_robots-0.0.1/django_env_robots.egg-info/top_level.txt
--rw-r--r--   0 patsmith   (501) staff       (20)      820 2024-05-23 11:22:35.000000 django_env_robots-0.0.1/pyproject.toml
--rw-r--r--   0 patsmith   (501) staff       (20)       38 2024-05-23 11:42:41.569383 django_env_robots-0.0.1/setup.cfg
+drwxr-xr-x   0 patsmith   (501) staff       (20)        0 2024-05-23 14:10:56.354541 django_env_robots-0.0.2/
+-rw-r--r--   0 patsmith   (501) staff       (20)     1064 2024-05-22 15:42:15.000000 django_env_robots-0.0.2/LICENSE
+-rw-r--r--   0 patsmith   (501) staff       (20)        0 2024-05-23 11:37:41.000000 django_env_robots-0.0.2/MANIFEST.in
+-rw-r--r--   0 patsmith   (501) staff       (20)     3319 2024-05-23 14:10:56.353827 django_env_robots-0.0.2/PKG-INFO
+-rw-r--r--   0 patsmith   (501) staff       (20)     1521 2024-05-23 14:09:35.000000 django_env_robots-0.0.2/README.md
+drwxr-xr-x   0 patsmith   (501) staff       (20)        0 2024-05-23 14:10:56.349673 django_env_robots-0.0.2/django_env_robots/
+-rw-r--r--   0 patsmith   (501) staff       (20)       21 2024-05-22 15:58:37.000000 django_env_robots-0.0.2/django_env_robots/__init__.py
+-rw-r--r--   0 patsmith   (501) staff       (20)      155 2024-05-22 15:56:56.000000 django_env_robots-0.0.2/django_env_robots/apps.py
+-rw-r--r--   0 patsmith   (501) staff       (20)       57 2024-05-22 15:23:46.000000 django_env_robots-0.0.2/django_env_robots/models.py
+-rw-r--r--   0 patsmith   (501) staff       (20)       60 2024-05-22 15:23:46.000000 django_env_robots-0.0.2/django_env_robots/tests.py
+-rw-r--r--   0 patsmith   (501) staff       (20)      115 2024-05-23 13:41:24.000000 django_env_robots-0.0.2/django_env_robots/urls.py
+-rw-r--r--   0 patsmith   (501) staff       (20)      784 2024-05-23 13:50:02.000000 django_env_robots-0.0.2/django_env_robots/views.py
+drwxr-xr-x   0 patsmith   (501) staff       (20)        0 2024-05-23 14:10:56.352994 django_env_robots-0.0.2/django_env_robots.egg-info/
+-rw-r--r--   0 patsmith   (501) staff       (20)     3319 2024-05-23 14:10:56.000000 django_env_robots-0.0.2/django_env_robots.egg-info/PKG-INFO
+-rw-r--r--   0 patsmith   (501) staff       (20)      412 2024-05-23 14:10:56.000000 django_env_robots-0.0.2/django_env_robots.egg-info/SOURCES.txt
+-rw-r--r--   0 patsmith   (501) staff       (20)        1 2024-05-23 14:10:56.000000 django_env_robots-0.0.2/django_env_robots.egg-info/dependency_links.txt
+-rw-r--r--   0 patsmith   (501) staff       (20)       12 2024-05-23 14:10:56.000000 django_env_robots-0.0.2/django_env_robots.egg-info/requires.txt
+-rw-r--r--   0 patsmith   (501) staff       (20)       18 2024-05-23 14:10:56.000000 django_env_robots-0.0.2/django_env_robots.egg-info/top_level.txt
+-rw-r--r--   0 patsmith   (501) staff       (20)      820 2024-05-23 13:54:45.000000 django_env_robots-0.0.2/pyproject.toml
+-rw-r--r--   0 patsmith   (501) staff       (20)       38 2024-05-23 14:10:56.354680 django_env_robots-0.0.2/setup.cfg
```

### Comparing `django_env_robots-0.0.1/LICENSE` & `django_env_robots-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django_env_robots-0.0.1/PKG-INFO` & `django_env_robots-0.0.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-env-robots
-Version: 0.0.1
+Version: 0.0.2
 Summary: Control robots.txt files from environment variables and templates.
 Author-email: Pat Smith <pat.smith@cursive.works>
 License: MIT License
         
         Copyright (c) 2024 Cursive
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -34,14 +34,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: django>=3.2
 
 # Django Env Robots (.txt)
 
 Serve different robots.txt from your production | stage | etc servers by setting environment variables. Rules are managed via templates.
+By default it excludes robots entirely.
 
 
 ## Installation
 
 Install from [PyPI](https://pypi.org/project/django-env-robots/):
 
 ```
@@ -53,25 +54,46 @@
 ```
 'django_env_robots',
 ```
 
 ## Usage
 
 ### settings.py
+Set the following:
+ - `SERVER_ENV` identifies the nature of the server and thus the robots.txt template that will be used.
+ - `ROBOT_SITEMAP_URLS` a list of relative urls to your sitemap(s).
+
+E.g:
 ```
-# robots
-SERVER_ENV = Env.get('SERVER_ENV', 'production')
-ROBOTS_ROOT = os.path.join(BASE_DIR, 'robots')
-ROBOTS_SITEMAP_URLS = Env.list('ROBOTS_SITEMAP_URLS', '/sitemap.xml')
+SERVER_ENV = 'production'
+ROBOTS_SITEMAP_URLS = ['/sitemap.xml', '/other_sitemap.xml']
 ```
 
 ### urls.py
 ```
 from django_env_robots import urls as robots_urls
 ...
 urlpatterns = [
     path("robots.txt", include(robots_urls)),
 ]
 ```
+
+### robots templates
+Create corresponding template files for each SERVER_ENV you will be using.
+These live in your projects `templates` directory in a `robots` subfolder.
+
+For example, if `SERVER_ENV` can be `production` or `stage`, then create:
+ - `templates/robots/production.txt`
+ - `templates/robots/stage.txt`
+
+e.g:
+```
+User-agent: *
+Disallow: /admin/*
+
+{% for sitemap_url in sitemap_urls %}Sitemap: {{ sitemap_url }}
+{% endfor %}
+```
+
 ### Other considertions
 
 A robots.txt being served from a Whitenose public directory will win over this app. That is because of whitenoise's middleware behaviour - quite correct but watch out for that.
```

### Comparing `django_env_robots-0.0.1/django_env_robots.egg-info/PKG-INFO` & `django_env_robots-0.0.2/django_env_robots.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-env-robots
-Version: 0.0.1
+Version: 0.0.2
 Summary: Control robots.txt files from environment variables and templates.
 Author-email: Pat Smith <pat.smith@cursive.works>
 License: MIT License
         
         Copyright (c) 2024 Cursive
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -34,14 +34,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: django>=3.2
 
 # Django Env Robots (.txt)
 
 Serve different robots.txt from your production | stage | etc servers by setting environment variables. Rules are managed via templates.
+By default it excludes robots entirely.
 
 
 ## Installation
 
 Install from [PyPI](https://pypi.org/project/django-env-robots/):
 
 ```
@@ -53,25 +54,46 @@
 ```
 'django_env_robots',
 ```
 
 ## Usage
 
 ### settings.py
+Set the following:
+ - `SERVER_ENV` identifies the nature of the server and thus the robots.txt template that will be used.
+ - `ROBOT_SITEMAP_URLS` a list of relative urls to your sitemap(s).
+
+E.g:
 ```
-# robots
-SERVER_ENV = Env.get('SERVER_ENV', 'production')
-ROBOTS_ROOT = os.path.join(BASE_DIR, 'robots')
-ROBOTS_SITEMAP_URLS = Env.list('ROBOTS_SITEMAP_URLS', '/sitemap.xml')
+SERVER_ENV = 'production'
+ROBOTS_SITEMAP_URLS = ['/sitemap.xml', '/other_sitemap.xml']
 ```
 
 ### urls.py
 ```
 from django_env_robots import urls as robots_urls
 ...
 urlpatterns = [
     path("robots.txt", include(robots_urls)),
 ]
 ```
+
+### robots templates
+Create corresponding template files for each SERVER_ENV you will be using.
+These live in your projects `templates` directory in a `robots` subfolder.
+
+For example, if `SERVER_ENV` can be `production` or `stage`, then create:
+ - `templates/robots/production.txt`
+ - `templates/robots/stage.txt`
+
+e.g:
+```
+User-agent: *
+Disallow: /admin/*
+
+{% for sitemap_url in sitemap_urls %}Sitemap: {{ sitemap_url }}
+{% endfor %}
+```
+
 ### Other considertions
 
 A robots.txt being served from a Whitenose public directory will win over this app. That is because of whitenoise's middleware behaviour - quite correct but watch out for that.
```

### Comparing `django_env_robots-0.0.1/pyproject.toml` & `django_env_robots-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "django-env-robots"
-version = "0.0.1"
+version = "0.0.2"
 description = "Control robots.txt files from environment variables and templates."
 readme = "README.md"
 authors = [{ name = "Pat Smith", email = "pat.smith@cursive.works" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

