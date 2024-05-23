# Comparing `tmp/launchflow-0.3.9.dev8.tar.gz` & `tmp/launchflow-0.4.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "launchflow-0.3.9.dev8.tar", last modified: Tue Apr  9 01:37:07 2024, max compression
+gzip compressed data, was "launchflow-0.4.0.dev0.tar", last modified: Thu May 23 02:12:36 2024, max compression
```

## Comparing `launchflow-0.3.9.dev8.tar` & `launchflow-0.4.0.dev0.tar`

### file list

```diff
@@ -1,198 +1,284 @@
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-09 01:37:07.491743 launchflow-0.3.9.dev8/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      118 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev8/MANIFEST.in
--rw-r--r--   0 tanke     (1000) tanke     (1000)     3423 2024-04-09 01:37:07.491743 launchflow-0.3.9.dev8/PKG-INFO
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     1996 2024-03-13 23:12:43.000000 launchflow-0.3.9.dev8/README.md
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-09 01:37:07.467743 launchflow-0.3.9.dev8/launchflow/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      528 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev8/launchflow/__init__.py
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-09 01:37:07.467743 launchflow-0.3.9.dev8/launchflow/aws/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)       67 2024-03-20 15:00:34.000000 launchflow-0.3.9.dev8/launchflow/aws/__init__.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     4480 2024-04-04 22:30:13.000000 launchflow-0.3.9.dev8/launchflow/aws/rds.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     3512 2024-04-02 20:56:37.000000 launchflow-0.3.9.dev8/launchflow/aws/s3.py
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-09 01:37:07.467743 launchflow-0.3.9.dev8/launchflow/cache/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)       95 2024-03-11 17:20:31.000000 launchflow-0.3.9.dev8/launchflow/cache/__init__.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     4980 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev8/launchflow/cache/launchflow_tmp.py
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-09 01:37:07.471743 launchflow-0.3.9.dev8/launchflow/cli/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-01-25 20:38:50.000000 launchflow-0.3.9.dev8/launchflow/cli/__init__.py
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-09 01:37:07.471743 launchflow-0.3.9.dev8/launchflow/cli/accounts/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-03-11 02:43:04.000000 launchflow-0.3.9.dev8/launchflow/cli/accounts/__init__.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     1250 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev8/launchflow/cli/accounts/account_commands.py
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-09 01:37:07.471743 launchflow-0.3.9.dev8/launchflow/cli/config/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-03-11 02:43:04.000000 launchflow-0.3.9.dev8/launchflow/cli/config/__init__.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     1026 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev8/launchflow/cli/config/config_commands.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      566 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev8/launchflow/cli/constants.py
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-09 01:37:07.471743 launchflow-0.3.9.dev8/launchflow/cli/environments/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-03-11 02:43:04.000000 launchflow-0.3.9.dev8/launchflow/cli/environments/__init__.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     2535 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev8/launchflow/cli/environments/environment_commands.py
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-09 01:37:07.471743 launchflow-0.3.9.dev8/launchflow/cli/gen/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev8/launchflow/cli/gen/__init__.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     2692 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev8/launchflow/cli/gen/template.py
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-09 01:37:07.471743 launchflow-0.3.9.dev8/launchflow/cli/gen/templates/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev8/launchflow/cli/gen/templates/__init__.py
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-09 01:37:07.471743 launchflow-0.3.9.dev8/launchflow/cli/gen/templates/__pycache__/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      209 2024-04-02 23:44:00.000000 launchflow-0.3.9.dev8/launchflow/cli/gen/templates/__pycache__/__init__.cpython-311.pyc
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-09 01:37:07.471743 launchflow-0.3.9.dev8/launchflow/cli/gen/templates/django/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev8/launchflow/cli/gen/templates/django/__init__.py
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-09 01:37:07.471743 launchflow-0.3.9.dev8/launchflow/cli/gen/templates/django/__pycache__/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      216 2024-04-03 19:22:56.000000 launchflow-0.3.9.dev8/launchflow/cli/gen/templates/django/__pycache__/__init__.cpython-311.pyc
--rw-rw-r--   0 tanke     (1000) tanke     (1000)    15518 2024-04-05 00:17:48.000000 launchflow-0.3.9.dev8/launchflow/cli/gen/templates/django/__pycache__/django_template.cpython-311.pyc
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-09 01:37:07.471743 launchflow-0.3.9.dev8/launchflow/cli/gen/templates/django/_postgres_template/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     2015 2024-04-03 20:53:05.000000 launchflow-0.3.9.dev8/launchflow/cli/gen/templates/django/_postgres_template/Dockerfile.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      162 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev8/launchflow/cli/gen/templates/django/_postgres_template/Makefile.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     3216 2024-04-04 16:43:35.000000 launchflow-0.3.9.dev8/launchflow/cli/gen/templates/django/_postgres_template/README.md.jinja
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-09 01:37:07.475743 launchflow-0.3.9.dev8/launchflow/cli/gen/templates/django/_postgres_template/app/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev8/launchflow/cli/gen/templates/django/_postgres_template/app/__init__.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      100 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev8/launchflow/cli/gen/templates/django/_postgres_template/app/admin.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)       81 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev8/launchflow/cli/gen/templates/django/_postgres_template/app/apps.py.jinja
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-09 01:37:07.475743 launchflow-0.3.9.dev8/launchflow/cli/gen/templates/django/_postgres_template/app/migrations/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      748 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev8/launchflow/cli/gen/templates/django/_postgres_template/app/migrations/0001_initial.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev8/launchflow/cli/gen/templates/django/_postgres_template/app/migrations/__init__.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      151 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev8/launchflow/cli/gen/templates/django/_postgres_template/app/models.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      487 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev8/launchflow/cli/gen/templates/django/_postgres_template/app/serializers.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      264 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev8/launchflow/cli/gen/templates/django/_postgres_template/app/urls.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     2021 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev8/launchflow/cli/gen/templates/django/_postgres_template/app/views.py.jinja
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-09 01:37:07.475743 launchflow-0.3.9.dev8/launchflow/cli/gen/templates/django/_postgres_template/django_app/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev8/launchflow/cli/gen/templates/django/_postgres_template/django_app/__init__.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      171 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev8/launchflow/cli/gen/templates/django/_postgres_template/django_app/asgi.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)       19 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev8/launchflow/cli/gen/templates/django/_postgres_template/django_app/infra.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     2157 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev8/launchflow/cli/gen/templates/django/_postgres_template/django_app/settings.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      166 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev8/launchflow/cli/gen/templates/django/_postgres_template/django_app/urls.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      171 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev8/launchflow/cli/gen/templates/django/_postgres_template/django_app/wsgi.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      182 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev8/launchflow/cli/gen/templates/django/_postgres_template/launchflow.yaml.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      542 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev8/launchflow/cli/gen/templates/django/_postgres_template/manage.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)       99 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev8/launchflow/cli/gen/templates/django/_postgres_template/requirements.txt.jinja
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-09 01:37:07.475743 launchflow-0.3.9.dev8/launchflow/cli/gen/templates/django/_simple_template/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     2015 2024-04-03 20:52:02.000000 launchflow-0.3.9.dev8/launchflow/cli/gen/templates/django/_simple_template/Dockerfile.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)       91 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev8/launchflow/cli/gen/templates/django/_simple_template/Makefile.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     3216 2024-04-04 16:43:35.000000 launchflow-0.3.9.dev8/launchflow/cli/gen/templates/django/_simple_template/README.md.jinja
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-09 01:37:07.475743 launchflow-0.3.9.dev8/launchflow/cli/gen/templates/django/_simple_template/app/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev8/launchflow/cli/gen/templates/django/_simple_template/app/__init__.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)       81 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev8/launchflow/cli/gen/templates/django/_simple_template/app/apps.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      164 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev8/launchflow/cli/gen/templates/django/_simple_template/app/urls.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      326 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev8/launchflow/cli/gen/templates/django/_simple_template/app/views.py.jinja
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-09 01:37:07.479743 launchflow-0.3.9.dev8/launchflow/cli/gen/templates/django/_simple_template/django_app/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev8/launchflow/cli/gen/templates/django/_simple_template/django_app/__init__.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      171 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev8/launchflow/cli/gen/templates/django/_simple_template/django_app/asgi.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)       19 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev8/launchflow/cli/gen/templates/django/_simple_template/django_app/infra.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     2157 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev8/launchflow/cli/gen/templates/django/_simple_template/django_app/settings.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      166 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev8/launchflow/cli/gen/templates/django/_simple_template/django_app/urls.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      171 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev8/launchflow/cli/gen/templates/django/_simple_template/django_app/wsgi.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      182 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev8/launchflow/cli/gen/templates/django/_simple_template/launchflow.yaml.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      542 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev8/launchflow/cli/gen/templates/django/_simple_template/manage.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)       99 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev8/launchflow/cli/gen/templates/django/_simple_template/requirements.txt.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)    14570 2024-04-05 00:17:09.000000 launchflow-0.3.9.dev8/launchflow/cli/gen/templates/django/django_template.py
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-09 01:37:07.479743 launchflow-0.3.9.dev8/launchflow/cli/gen/templates/fastapi/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev8/launchflow/cli/gen/templates/fastapi/__init__.py
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-09 01:37:07.479743 launchflow-0.3.9.dev8/launchflow/cli/gen/templates/fastapi/__pycache__/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      217 2024-04-02 23:47:30.000000 launchflow-0.3.9.dev8/launchflow/cli/gen/templates/fastapi/__pycache__/__init__.cpython-311.pyc
--rw-rw-r--   0 tanke     (1000) tanke     (1000)    17805 2024-04-05 00:17:48.000000 launchflow-0.3.9.dev8/launchflow/cli/gen/templates/fastapi/__pycache__/fastapi_template.cpython-311.pyc
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-09 01:37:07.479743 launchflow-0.3.9.dev8/launchflow/cli/gen/templates/fastapi/_postgres_template/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     1849 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev8/launchflow/cli/gen/templates/fastapi/_postgres_template/Dockerfile.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     2664 2024-04-04 16:43:35.000000 launchflow-0.3.9.dev8/launchflow/cli/gen/templates/fastapi/_postgres_template/README.md.jinja
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-09 01:37:07.479743 launchflow-0.3.9.dev8/launchflow/cli/gen/templates/fastapi/_postgres_template/app/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev8/launchflow/cli/gen/templates/fastapi/_postgres_template/app/__init__.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)       19 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev8/launchflow/cli/gen/templates/fastapi/_postgres_template/app/infra.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      576 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev8/launchflow/cli/gen/templates/fastapi/_postgres_template/app/main.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      371 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev8/launchflow/cli/gen/templates/fastapi/_postgres_template/app/models.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      559 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev8/launchflow/cli/gen/templates/fastapi/_postgres_template/app/schemas.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      182 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev8/launchflow/cli/gen/templates/fastapi/_postgres_template/launchflow.yaml.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)       79 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev8/launchflow/cli/gen/templates/fastapi/_postgres_template/requirements.txt.jinja
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-09 01:37:07.479743 launchflow-0.3.9.dev8/launchflow/cli/gen/templates/fastapi/_simple_template/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     1849 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev8/launchflow/cli/gen/templates/fastapi/_simple_template/Dockerfile.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     2664 2024-04-04 16:43:35.000000 launchflow-0.3.9.dev8/launchflow/cli/gen/templates/fastapi/_simple_template/README.md.jinja
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-09 01:37:07.479743 launchflow-0.3.9.dev8/launchflow/cli/gen/templates/fastapi/_simple_template/app/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev8/launchflow/cli/gen/templates/fastapi/_simple_template/app/__init__.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)       19 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev8/launchflow/cli/gen/templates/fastapi/_simple_template/app/infra.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      573 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev8/launchflow/cli/gen/templates/fastapi/_simple_template/app/main.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      182 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev8/launchflow/cli/gen/templates/fastapi/_simple_template/launchflow.yaml.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)       79 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev8/launchflow/cli/gen/templates/fastapi/_simple_template/requirements.txt.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)    18560 2024-04-05 00:17:11.000000 launchflow-0.3.9.dev8/launchflow/cli/gen/templates/fastapi/fastapi_template.py
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-09 01:37:07.483743 launchflow-0.3.9.dev8/launchflow/cli/gen/templates/flask/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev8/launchflow/cli/gen/templates/flask/__init__.py
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-09 01:37:07.483743 launchflow-0.3.9.dev8/launchflow/cli/gen/templates/flask/__pycache__/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      215 2024-04-03 19:22:56.000000 launchflow-0.3.9.dev8/launchflow/cli/gen/templates/flask/__pycache__/__init__.cpython-311.pyc
--rw-rw-r--   0 tanke     (1000) tanke     (1000)    17114 2024-04-05 00:17:48.000000 launchflow-0.3.9.dev8/launchflow/cli/gen/templates/flask/__pycache__/flask_template.cpython-311.pyc
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-09 01:37:07.483743 launchflow-0.3.9.dev8/launchflow/cli/gen/templates/flask/_postgres_template/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     1877 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev8/launchflow/cli/gen/templates/flask/_postgres_template/Dockerfile.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     2750 2024-04-04 16:43:35.000000 launchflow-0.3.9.dev8/launchflow/cli/gen/templates/flask/_postgres_template/README.md.jinja
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-09 01:37:07.483743 launchflow-0.3.9.dev8/launchflow/cli/gen/templates/flask/_postgres_template/app/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev8/launchflow/cli/gen/templates/flask/_postgres_template/app/__init__.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)       19 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev8/launchflow/cli/gen/templates/flask/_postgres_template/app/infra.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      297 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev8/launchflow/cli/gen/templates/flask/_postgres_template/app/main.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      371 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev8/launchflow/cli/gen/templates/flask/_postgres_template/app/models.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      559 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev8/launchflow/cli/gen/templates/flask/_postgres_template/app/schemas.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      182 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev8/launchflow/cli/gen/templates/flask/_postgres_template/launchflow.yaml.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)       78 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev8/launchflow/cli/gen/templates/flask/_postgres_template/requirements.txt.jinja
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-09 01:37:07.483743 launchflow-0.3.9.dev8/launchflow/cli/gen/templates/flask/_simple_template/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     1877 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev8/launchflow/cli/gen/templates/flask/_simple_template/Dockerfile.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     2750 2024-04-04 16:43:33.000000 launchflow-0.3.9.dev8/launchflow/cli/gen/templates/flask/_simple_template/README.md.jinja
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-09 01:37:07.483743 launchflow-0.3.9.dev8/launchflow/cli/gen/templates/flask/_simple_template/app/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev8/launchflow/cli/gen/templates/flask/_simple_template/app/__init__.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)       19 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev8/launchflow/cli/gen/templates/flask/_simple_template/app/infra.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      324 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev8/launchflow/cli/gen/templates/flask/_simple_template/app/main.py.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      182 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev8/launchflow/cli/gen/templates/flask/_simple_template/launchflow.yaml.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)       78 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev8/launchflow/cli/gen/templates/flask/_simple_template/requirements.txt.jinja
--rw-rw-r--   0 tanke     (1000) tanke     (1000)    17509 2024-04-05 00:17:00.000000 launchflow-0.3.9.dev8/launchflow/cli/gen/templates/flask/flask_template.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)    19278 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev8/launchflow/cli/main.py
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-09 01:37:07.483743 launchflow-0.3.9.dev8/launchflow/cli/project/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-01-30 20:01:40.000000 launchflow-0.3.9.dev8/launchflow/cli/project/__init__.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     1702 2024-03-11 17:23:46.000000 launchflow-0.3.9.dev8/launchflow/cli/project/project_commands.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     3067 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev8/launchflow/cli/project_gen.py
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-09 01:37:07.483743 launchflow-0.3.9.dev8/launchflow/cli/resources/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-03-11 02:43:04.000000 launchflow-0.3.9.dev8/launchflow/cli/resources/__init__.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     4436 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev8/launchflow/cli/resources/resource_commands.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     5382 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev8/launchflow/cli/resources_ast.py
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-09 01:37:07.483743 launchflow-0.3.9.dev8/launchflow/cli/services/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)        0 2024-03-21 18:34:33.000000 launchflow-0.3.9.dev8/launchflow/cli/services/__init__.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     4413 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev8/launchflow/cli/services/service_commands.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     3501 2024-03-11 17:20:31.000000 launchflow-0.3.9.dev8/launchflow/cli/utils.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      482 2024-03-11 17:23:46.000000 launchflow-0.3.9.dev8/launchflow/cli/utyper.py
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-09 01:37:07.487743 launchflow-0.3.9.dev8/launchflow/clients/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      296 2024-03-11 17:23:46.000000 launchflow-0.3.9.dev8/launchflow/clients/__init__.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     1155 2024-03-11 17:23:46.000000 launchflow-0.3.9.dev8/launchflow/clients/accounts_client.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     1137 2024-03-29 14:50:29.000000 launchflow-0.3.9.dev8/launchflow/clients/client.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     1832 2024-03-11 17:23:46.000000 launchflow-0.3.9.dev8/launchflow/clients/connect_client.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     4806 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev8/launchflow/clients/environments_client.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     1911 2024-03-21 18:34:33.000000 launchflow-0.3.9.dev8/launchflow/clients/operations_client.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     1820 2024-03-11 17:23:46.000000 launchflow-0.3.9.dev8/launchflow/clients/projects_client.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     5117 2024-03-21 18:34:33.000000 launchflow-0.3.9.dev8/launchflow/clients/resources_client.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     3767 2024-03-21 18:34:33.000000 launchflow-0.3.9.dev8/launchflow/clients/response_schemas.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     3477 2024-03-21 18:34:33.000000 launchflow-0.3.9.dev8/launchflow/clients/services_client.py
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-09 01:37:07.487743 launchflow-0.3.9.dev8/launchflow/config/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)       99 2024-03-11 17:20:31.000000 launchflow-0.3.9.dev8/launchflow/config/__init__.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     4412 2024-03-11 17:20:31.000000 launchflow-0.3.9.dev8/launchflow/config/launchflow_config.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     1361 2024-04-03 22:09:55.000000 launchflow-0.3.9.dev8/launchflow/config/launchflow_env.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     5144 2024-03-14 16:50:08.000000 launchflow-0.3.9.dev8/launchflow/config/launchflow_yaml.py
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-09 01:37:07.487743 launchflow-0.3.9.dev8/launchflow/context/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)       91 2024-03-13 17:41:44.000000 launchflow-0.3.9.dev8/launchflow/context/__init__.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)    16535 2024-04-03 22:10:20.000000 launchflow-0.3.9.dev8/launchflow/context/launchflow_ctx.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     4030 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev8/launchflow/exceptions.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     5180 2024-03-22 06:06:27.000000 launchflow-0.3.9.dev8/launchflow/fastapi.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)       52 2024-03-27 23:08:23.000000 launchflow-0.3.9.dev8/launchflow/flask.py
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-09 01:37:07.487743 launchflow-0.3.9.dev8/launchflow/flows/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      129 2024-03-11 02:43:04.000000 launchflow-0.3.9.dev8/launchflow/flows/__init__.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     1236 2024-03-11 17:23:46.000000 launchflow-0.3.9.dev8/launchflow/flows/account_id.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     3746 2024-03-21 18:34:33.000000 launchflow-0.3.9.dev8/launchflow/flows/auth.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)    31351 2024-04-09 01:36:50.000000 launchflow-0.3.9.dev8/launchflow/flows/cloud_provider.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     7171 2024-03-22 06:06:27.000000 launchflow-0.3.9.dev8/launchflow/flows/environments_flows.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     4030 2024-03-22 06:06:27.000000 launchflow-0.3.9.dev8/launchflow/flows/project_flows.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)    18602 2024-03-21 18:34:33.000000 launchflow-0.3.9.dev8/launchflow/flows/resource_flows.py
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-09 01:37:07.491743 launchflow-0.3.9.dev8/launchflow/gcp/
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      219 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev8/launchflow/gcp/__init__.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     7762 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev8/launchflow/gcp/cloudsql.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     2978 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev8/launchflow/gcp/compute_engine.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     3523 2024-04-02 20:56:22.000000 launchflow-0.3.9.dev8/launchflow/gcp/gcs.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     2755 2024-04-03 18:40:41.000000 launchflow-0.3.9.dev8/launchflow/gcp/memorystore.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     2578 2024-04-05 21:08:46.000000 launchflow-0.3.9.dev8/launchflow/gcp/utils.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     2059 2024-03-11 17:23:46.000000 launchflow-0.3.9.dev8/launchflow/operations.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     2288 2024-04-02 21:12:53.000000 launchflow-0.3.9.dev8/launchflow/resource.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)       50 2024-03-11 17:20:31.000000 launchflow-0.3.9.dev8/launchflow/service.py
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      789 2024-03-28 23:07:50.000000 launchflow-0.3.9.dev8/launchflow/utils.py
-drwxrwxr-x   0 tanke     (1000) tanke     (1000)        0 2024-04-09 01:37:07.491743 launchflow-0.3.9.dev8/launchflow.egg-info/
--rw-r--r--   0 tanke     (1000) tanke     (1000)     3423 2024-04-09 01:37:07.000000 launchflow-0.3.9.dev8/launchflow.egg-info/PKG-INFO
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     8331 2024-04-09 01:37:07.000000 launchflow-0.3.9.dev8/launchflow.egg-info/SOURCES.txt
--rw-rw-r--   0 tanke     (1000) tanke     (1000)        1 2024-04-09 01:37:07.000000 launchflow-0.3.9.dev8/launchflow.egg-info/dependency_links.txt
--rw-rw-r--   0 tanke     (1000) tanke     (1000)       84 2024-04-09 01:37:07.000000 launchflow-0.3.9.dev8/launchflow.egg-info/entry_points.txt
--rw-rw-r--   0 tanke     (1000) tanke     (1000)      309 2024-04-09 01:37:07.000000 launchflow-0.3.9.dev8/launchflow.egg-info/requires.txt
--rw-rw-r--   0 tanke     (1000) tanke     (1000)       11 2024-04-09 01:37:07.000000 launchflow-0.3.9.dev8/launchflow.egg-info/top_level.txt
--rw-rw-r--   0 tanke     (1000) tanke     (1000)     1421 2024-04-09 01:36:54.000000 launchflow-0.3.9.dev8/pyproject.toml
--rw-rw-r--   0 tanke     (1000) tanke     (1000)       38 2024-04-09 01:37:07.491743 launchflow-0.3.9.dev8/setup.cfg
+drwxr-xr-x   0 calebvandyke   (501) staff       (20)        0 2024-05-23 02:12:36.947342 launchflow-0.4.0.dev0/
+-rw-r--r--   0 calebvandyke   (501) staff       (20)      161 2024-05-14 17:27:57.000000 launchflow-0.4.0.dev0/MANIFEST.in
+-rw-r--r--   0 calebvandyke   (501) staff       (20)     3890 2024-05-23 02:12:36.947130 launchflow-0.4.0.dev0/PKG-INFO
+-rw-r--r--   0 calebvandyke   (501) staff       (20)     1996 2024-05-14 13:09:20.000000 launchflow-0.4.0.dev0/README.md
+drwxr-xr-x   0 calebvandyke   (501) staff       (20)        0 2024-05-23 02:12:36.910912 launchflow-0.4.0.dev0/launchflow/
+-rw-r--r--   0 calebvandyke   (501) staff       (20)      735 2024-05-22 19:01:25.000000 launchflow-0.4.0.dev0/launchflow/__init__.py
+drwxr-xr-x   0 calebvandyke   (501) staff       (20)        0 2024-05-23 02:12:36.913479 launchflow-0.4.0.dev0/launchflow/aws/
+-rw-r--r--   0 calebvandyke   (501) staff       (20)      234 2024-05-14 13:08:59.000000 launchflow-0.4.0.dev0/launchflow/aws/__init__.py
+-rw-r--r--   0 calebvandyke   (501) staff       (20)    14019 2024-05-16 16:00:23.000000 launchflow-0.4.0.dev0/launchflow/aws/ec2.py
+-rw-r--r--   0 calebvandyke   (501) staff       (20)     1786 2024-05-14 13:08:59.000000 launchflow-0.4.0.dev0/launchflow/aws/ecs_fargate.py
+-rw-r--r--   0 calebvandyke   (501) staff       (20)     3663 2024-05-16 16:00:23.000000 launchflow-0.4.0.dev0/launchflow/aws/elasticache.py
+-rw-r--r--   0 calebvandyke   (501) staff       (20)     5832 2024-05-16 16:00:23.000000 launchflow-0.4.0.dev0/launchflow/aws/rds.py
+-rw-r--r--   0 calebvandyke   (501) staff       (20)      254 2024-05-14 13:08:59.000000 launchflow-0.4.0.dev0/launchflow/aws/resource.py
+-rw-r--r--   0 calebvandyke   (501) staff       (20)     3850 2024-05-16 16:00:23.000000 launchflow-0.4.0.dev0/launchflow/aws/s3.py
+-rw-r--r--   0 calebvandyke   (501) staff       (20)     2872 2024-05-17 14:07:04.000000 launchflow-0.4.0.dev0/launchflow/aws/secrets_manager.py
+drwxr-xr-x   0 calebvandyke   (501) staff       (20)        0 2024-05-23 02:12:36.913896 launchflow-0.4.0.dev0/launchflow/cache/
+-rw-r--r--   0 calebvandyke   (501) staff       (20)       95 2024-05-14 13:08:59.000000 launchflow-0.4.0.dev0/launchflow/cache/__init__.py
+-rw-r--r--   0 calebvandyke   (501) staff       (20)     4980 2024-05-14 13:08:59.000000 launchflow-0.4.0.dev0/launchflow/cache/launchflow_tmp.py
+drwxr-xr-x   0 calebvandyke   (501) staff       (20)        0 2024-05-23 02:12:36.915382 launchflow-0.4.0.dev0/launchflow/cli/
+-rw-r--r--   0 calebvandyke   (501) staff       (20)        0 2024-05-14 13:08:59.000000 launchflow-0.4.0.dev0/launchflow/cli/__init__.py
+drwxr-xr-x   0 calebvandyke   (501) staff       (20)        0 2024-05-23 02:12:36.915610 launchflow-0.4.0.dev0/launchflow/cli/accounts/
+-rw-r--r--   0 calebvandyke   (501) staff       (20)        0 2024-05-14 13:08:59.000000 launchflow-0.4.0.dev0/launchflow/cli/accounts/__init__.py
+-rw-r--r--   0 calebvandyke   (501) staff       (20)     1250 2024-05-16 16:00:23.000000 launchflow-0.4.0.dev0/launchflow/cli/accounts/account_commands.py
+-rw-r--r--   0 calebvandyke   (501) staff       (20)     6890 2024-05-14 13:08:59.000000 launchflow-0.4.0.dev0/launchflow/cli/ast_search.py
+drwxr-xr-x   0 calebvandyke   (501) staff       (20)        0 2024-05-23 02:12:36.915872 launchflow-0.4.0.dev0/launchflow/cli/config/
+-rw-r--r--   0 calebvandyke   (501) staff       (20)        0 2024-05-14 13:08:59.000000 launchflow-0.4.0.dev0/launchflow/cli/config/__init__.py
+-rw-r--r--   0 calebvandyke   (501) staff       (20)     1026 2024-05-16 16:00:23.000000 launchflow-0.4.0.dev0/launchflow/cli/config/config_commands.py
+-rw-r--r--   0 calebvandyke   (501) staff       (20)      814 2024-05-14 13:08:59.000000 launchflow-0.4.0.dev0/launchflow/cli/constants.py
+drwxr-xr-x   0 calebvandyke   (501) staff       (20)        0 2024-05-23 02:12:36.916122 launchflow-0.4.0.dev0/launchflow/cli/environments/
+-rw-r--r--   0 calebvandyke   (501) staff       (20)        0 2024-05-14 13:08:59.000000 launchflow-0.4.0.dev0/launchflow/cli/environments/__init__.py
+-rw-r--r--   0 calebvandyke   (501) staff       (20)     4248 2024-05-21 20:59:12.000000 launchflow-0.4.0.dev0/launchflow/cli/environments/environment_commands.py
+drwxr-xr-x   0 calebvandyke   (501) staff       (20)        0 2024-05-23 02:12:36.916338 launchflow-0.4.0.dev0/launchflow/cli/gen/
+-rw-r--r--   0 calebvandyke   (501) staff       (20)        0 2024-05-14 13:08:59.000000 launchflow-0.4.0.dev0/launchflow/cli/gen/__init__.py
+-rw-r--r--   0 calebvandyke   (501) staff       (20)     2854 2024-05-14 13:08:59.000000 launchflow-0.4.0.dev0/launchflow/cli/gen/template.py
+drwxr-xr-x   0 calebvandyke   (501) staff       (20)        0 2024-05-23 02:12:36.916523 launchflow-0.4.0.dev0/launchflow/cli/gen/templates/
+-rw-r--r--   0 calebvandyke   (501) staff       (20)        0 2024-05-14 13:08:59.000000 launchflow-0.4.0.dev0/launchflow/cli/gen/templates/__init__.py
+drwxr-xr-x   0 calebvandyke   (501) staff       (20)        0 2024-05-23 02:12:36.916647 launchflow-0.4.0.dev0/launchflow/cli/gen/templates/__pycache__/
+-rw-r--r--   0 calebvandyke   (501) staff       (20)      189 2024-05-14 13:47:29.000000 launchflow-0.4.0.dev0/launchflow/cli/gen/templates/__pycache__/__init__.cpython-311.pyc
+drwxr-xr-x   0 calebvandyke   (501) staff       (20)        0 2024-05-23 02:12:36.917092 launchflow-0.4.0.dev0/launchflow/cli/gen/templates/django/
+-rw-r--r--   0 calebvandyke   (501) staff       (20)        0 2024-05-14 13:08:59.000000 launchflow-0.4.0.dev0/launchflow/cli/gen/templates/django/__init__.py
+drwxr-xr-x   0 calebvandyke   (501) staff       (20)        0 2024-05-23 02:12:36.917478 launchflow-0.4.0.dev0/launchflow/cli/gen/templates/django/__pycache__/
+-rw-r--r--   0 calebvandyke   (501) staff       (20)      196 2024-05-14 13:47:29.000000 launchflow-0.4.0.dev0/launchflow/cli/gen/templates/django/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 calebvandyke   (501) staff       (20)    16097 2024-05-16 16:02:46.000000 launchflow-0.4.0.dev0/launchflow/cli/gen/templates/django/__pycache__/django_template.cpython-311.pyc
+drwxr-xr-x   0 calebvandyke   (501) staff       (20)        0 2024-05-23 02:12:36.918476 launchflow-0.4.0.dev0/launchflow/cli/gen/templates/django/_postgres_template/
+-rw-r--r--   0 calebvandyke   (501) staff       (20)     1946 2024-05-14 13:08:59.000000 launchflow-0.4.0.dev0/launchflow/cli/gen/templates/django/_postgres_template/Dockerfile.jinja
+-rw-r--r--   0 calebvandyke   (501) staff       (20)      164 2024-05-14 13:08:59.000000 launchflow-0.4.0.dev0/launchflow/cli/gen/templates/django/_postgres_template/Makefile.jinja
+-rw-r--r--   0 calebvandyke   (501) staff       (20)     3219 2024-05-14 13:08:59.000000 launchflow-0.4.0.dev0/launchflow/cli/gen/templates/django/_postgres_template/README.md.jinja
+drwxr-xr-x   0 calebvandyke   (501) staff       (20)        0 2024-05-23 02:12:36.919521 launchflow-0.4.0.dev0/launchflow/cli/gen/templates/django/_postgres_template/app/
+-rw-r--r--   0 calebvandyke   (501) staff       (20)        0 2024-05-14 13:08:59.000000 launchflow-0.4.0.dev0/launchflow/cli/gen/templates/django/_postgres_template/app/__init__.py.jinja
+-rw-r--r--   0 calebvandyke   (501) staff       (20)      100 2024-05-14 13:08:59.000000 launchflow-0.4.0.dev0/launchflow/cli/gen/templates/django/_postgres_template/app/admin.py.jinja
+-rw-r--r--   0 calebvandyke   (501) staff       (20)       81 2024-05-14 13:08:59.000000 launchflow-0.4.0.dev0/launchflow/cli/gen/templates/django/_postgres_template/app/apps.py.jinja
+drwxr-xr-x   0 calebvandyke   (501) staff       (20)        0 2024-05-23 02:12:36.919792 launchflow-0.4.0.dev0/launchflow/cli/gen/templates/django/_postgres_template/app/migrations/
+-rw-r--r--   0 calebvandyke   (501) staff       (20)      748 2024-05-14 13:08:59.000000 launchflow-0.4.0.dev0/launchflow/cli/gen/templates/django/_postgres_template/app/migrations/0001_initial.py.jinja
+-rw-r--r--   0 calebvandyke   (501) staff       (20)        0 2024-05-14 13:08:59.000000 launchflow-0.4.0.dev0/launchflow/cli/gen/templates/django/_postgres_template/app/migrations/__init__.py.jinja
+-rw-r--r--   0 calebvandyke   (501) staff       (20)      151 2024-05-14 13:08:59.000000 launchflow-0.4.0.dev0/launchflow/cli/gen/templates/django/_postgres_template/app/models.py.jinja
+-rw-r--r--   0 calebvandyke   (501) staff       (20)      487 2024-05-14 13:08:59.000000 launchflow-0.4.0.dev0/launchflow/cli/gen/templates/django/_postgres_template/app/serializers.py.jinja
+-rw-r--r--   0 calebvandyke   (501) staff       (20)      264 2024-05-14 13:08:59.000000 launchflow-0.4.0.dev0/launchflow/cli/gen/templates/django/_postgres_template/app/urls.py.jinja
+-rw-r--r--   0 calebvandyke   (501) staff       (20)     2021 2024-05-14 13:08:59.000000 launchflow-0.4.0.dev0/launchflow/cli/gen/templates/django/_postgres_template/app/views.py.jinja
+drwxr-xr-x   0 calebvandyke   (501) staff       (20)        0 2024-05-23 02:12:36.920730 launchflow-0.4.0.dev0/launchflow/cli/gen/templates/django/_postgres_template/django_app/
+-rw-r--r--   0 calebvandyke   (501) staff       (20)        0 2024-05-14 13:08:59.000000 launchflow-0.4.0.dev0/launchflow/cli/gen/templates/django/_postgres_template/django_app/__init__.py.jinja
+-rw-r--r--   0 calebvandyke   (501) staff       (20)      171 2024-05-14 13:08:59.000000 launchflow-0.4.0.dev0/launchflow/cli/gen/templates/django/_postgres_template/django_app/asgi.py.jinja
+-rw-r--r--   0 calebvandyke   (501) staff       (20)       19 2024-05-14 13:08:59.000000 launchflow-0.4.0.dev0/launchflow/cli/gen/templates/django/_postgres_template/django_app/infra.py.jinja
+-rw-r--r--   0 calebvandyke   (501) staff       (20)      293 2024-05-14 13:08:59.000000 launchflow-0.4.0.dev0/launchflow/cli/gen/templates/django/_postgres_template/django_app/middleware.py.jinja
+-rw-r--r--   0 calebvandyke   (501) staff       (20)     2229 2024-05-14 13:08:59.000000 launchflow-0.4.0.dev0/launchflow/cli/gen/templates/django/_postgres_template/django_app/settings.py.jinja
+-rw-r--r--   0 calebvandyke   (501) staff       (20)      166 2024-05-14 13:08:59.000000 launchflow-0.4.0.dev0/launchflow/cli/gen/templates/django/_postgres_template/django_app/urls.py.jinja
+-rw-r--r--   0 calebvandyke   (501) staff       (20)      171 2024-05-14 13:08:59.000000 launchflow-0.4.0.dev0/launchflow/cli/gen/templates/django/_postgres_template/django_app/wsgi.py.jinja
+-rw-r--r--   0 calebvandyke   (501) staff       (20)      182 2024-05-14 13:08:59.000000 launchflow-0.4.0.dev0/launchflow/cli/gen/templates/django/_postgres_template/launchflow.yaml.jinja
+-rw-r--r--   0 calebvandyke   (501) staff       (20)      542 2024-05-14 13:08:59.000000 launchflow-0.4.0.dev0/launchflow/cli/gen/templates/django/_postgres_template/manage.py.jinja
+-rw-r--r--   0 calebvandyke   (501) staff       (20)       99 2024-05-14 13:08:59.000000 launchflow-0.4.0.dev0/launchflow/cli/gen/templates/django/_postgres_template/requirements.txt.jinja
+drwxr-xr-x   0 calebvandyke   (501) staff       (20)        0 2024-05-23 02:12:36.921604 launchflow-0.4.0.dev0/launchflow/cli/gen/templates/django/_simple_template/
+-rw-r--r--   0 calebvandyke   (501) staff       (20)     1946 2024-05-14 13:08:59.000000 launchflow-0.4.0.dev0/launchflow/cli/gen/templates/django/_simple_template/Dockerfile.jinja
+-rw-r--r--   0 calebvandyke   (501) staff       (20)       93 2024-05-14 13:08:59.000000 launchflow-0.4.0.dev0/launchflow/cli/gen/templates/django/_simple_template/Makefile.jinja
+-rw-r--r--   0 calebvandyke   (501) staff       (20)     3219 2024-05-14 13:08:59.000000 launchflow-0.4.0.dev0/launchflow/cli/gen/templates/django/_simple_template/README.md.jinja
+drwxr-xr-x   0 calebvandyke   (501) staff       (20)        0 2024-05-23 02:12:36.922141 launchflow-0.4.0.dev0/launchflow/cli/gen/templates/django/_simple_template/app/
+-rw-r--r--   0 calebvandyke   (501) staff       (20)        0 2024-05-14 13:08:59.000000 launchflow-0.4.0.dev0/launchflow/cli/gen/templates/django/_simple_template/app/__init__.py.jinja
+-rw-r--r--   0 calebvandyke   (501) staff       (20)       81 2024-05-14 13:08:59.000000 launchflow-0.4.0.dev0/launchflow/cli/gen/templates/django/_simple_template/app/apps.py.jinja
+-rw-r--r--   0 calebvandyke   (501) staff       (20)      164 2024-05-14 13:08:59.000000 launchflow-0.4.0.dev0/launchflow/cli/gen/templates/django/_simple_template/app/urls.py.jinja
+-rw-r--r--   0 calebvandyke   (501) staff       (20)      326 2024-05-14 13:08:59.000000 launchflow-0.4.0.dev0/launchflow/cli/gen/templates/django/_simple_template/app/views.py.jinja
+drwxr-xr-x   0 calebvandyke   (501) staff       (20)        0 2024-05-23 02:12:36.923363 launchflow-0.4.0.dev0/launchflow/cli/gen/templates/django/_simple_template/django_app/
+-rw-r--r--   0 calebvandyke   (501) staff       (20)        0 2024-05-14 13:08:59.000000 launchflow-0.4.0.dev0/launchflow/cli/gen/templates/django/_simple_template/django_app/__init__.py.jinja
+-rw-r--r--   0 calebvandyke   (501) staff       (20)      171 2024-05-14 13:08:59.000000 launchflow-0.4.0.dev0/launchflow/cli/gen/templates/django/_simple_template/django_app/asgi.py.jinja
+-rw-r--r--   0 calebvandyke   (501) staff       (20)       19 2024-05-14 13:08:59.000000 launchflow-0.4.0.dev0/launchflow/cli/gen/templates/django/_simple_template/django_app/infra.py.jinja
+-rw-r--r--   0 calebvandyke   (501) staff       (20)      293 2024-05-14 13:08:59.000000 launchflow-0.4.0.dev0/launchflow/cli/gen/templates/django/_simple_template/django_app/middleware.py.jinja
+-rw-r--r--   0 calebvandyke   (501) staff       (20)     2229 2024-05-14 13:08:59.000000 launchflow-0.4.0.dev0/launchflow/cli/gen/templates/django/_simple_template/django_app/settings.py.jinja
+-rw-r--r--   0 calebvandyke   (501) staff       (20)      166 2024-05-14 13:08:59.000000 launchflow-0.4.0.dev0/launchflow/cli/gen/templates/django/_simple_template/django_app/urls.py.jinja
+-rw-r--r--   0 calebvandyke   (501) staff       (20)      171 2024-05-14 13:08:59.000000 launchflow-0.4.0.dev0/launchflow/cli/gen/templates/django/_simple_template/django_app/wsgi.py.jinja
+-rw-r--r--   0 calebvandyke   (501) staff       (20)      182 2024-05-14 13:08:59.000000 launchflow-0.4.0.dev0/launchflow/cli/gen/templates/django/_simple_template/launchflow.yaml.jinja
+-rw-r--r--   0 calebvandyke   (501) staff       (20)      542 2024-05-14 13:08:59.000000 launchflow-0.4.0.dev0/launchflow/cli/gen/templates/django/_simple_template/manage.py.jinja
+-rw-r--r--   0 calebvandyke   (501) staff       (20)       99 2024-05-14 13:08:59.000000 launchflow-0.4.0.dev0/launchflow/cli/gen/templates/django/_simple_template/requirements.txt.jinja
+-rw-r--r--   0 calebvandyke   (501) staff       (20)    16928 2024-05-16 16:00:23.000000 launchflow-0.4.0.dev0/launchflow/cli/gen/templates/django/django_template.py
+drwxr-xr-x   0 calebvandyke   (501) staff       (20)        0 2024-05-23 02:12:36.923643 launchflow-0.4.0.dev0/launchflow/cli/gen/templates/fastapi/
+-rw-r--r--   0 calebvandyke   (501) staff       (20)        0 2024-05-14 13:08:59.000000 launchflow-0.4.0.dev0/launchflow/cli/gen/templates/fastapi/__init__.py
+drwxr-xr-x   0 calebvandyke   (501) staff       (20)        0 2024-05-23 02:12:36.923952 launchflow-0.4.0.dev0/launchflow/cli/gen/templates/fastapi/__pycache__/
+-rw-r--r--   0 calebvandyke   (501) staff       (20)      197 2024-05-14 13:47:29.000000 launchflow-0.4.0.dev0/launchflow/cli/gen/templates/fastapi/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 calebvandyke   (501) staff       (20)    18192 2024-05-16 16:02:46.000000 launchflow-0.4.0.dev0/launchflow/cli/gen/templates/fastapi/__pycache__/fastapi_template.cpython-311.pyc
+drwxr-xr-x   0 calebvandyke   (501) staff       (20)        0 2024-05-23 02:12:36.924567 launchflow-0.4.0.dev0/launchflow/cli/gen/templates/fastapi/_postgres_template/
+-rw-r--r--   0 calebvandyke   (501) staff       (20)     1780 2024-05-14 13:08:59.000000 launchflow-0.4.0.dev0/launchflow/cli/gen/templates/fastapi/_postgres_template/Dockerfile.jinja
+-rw-r--r--   0 calebvandyke   (501) staff       (20)     2665 2024-05-14 13:08:59.000000 launchflow-0.4.0.dev0/launchflow/cli/gen/templates/fastapi/_postgres_template/README.md.jinja
+drwxr-xr-x   0 calebvandyke   (501) staff       (20)        0 2024-05-23 02:12:36.925189 launchflow-0.4.0.dev0/launchflow/cli/gen/templates/fastapi/_postgres_template/app/
+-rw-r--r--   0 calebvandyke   (501) staff       (20)        0 2024-05-14 13:08:59.000000 launchflow-0.4.0.dev0/launchflow/cli/gen/templates/fastapi/_postgres_template/app/__init__.py.jinja
+-rw-r--r--   0 calebvandyke   (501) staff       (20)       19 2024-05-14 13:08:59.000000 launchflow-0.4.0.dev0/launchflow/cli/gen/templates/fastapi/_postgres_template/app/infra.py.jinja
+-rw-r--r--   0 calebvandyke   (501) staff       (20)      576 2024-05-14 13:08:59.000000 launchflow-0.4.0.dev0/launchflow/cli/gen/templates/fastapi/_postgres_template/app/main.py.jinja
+-rw-r--r--   0 calebvandyke   (501) staff       (20)      371 2024-05-14 13:08:59.000000 launchflow-0.4.0.dev0/launchflow/cli/gen/templates/fastapi/_postgres_template/app/models.py.jinja
+-rw-r--r--   0 calebvandyke   (501) staff       (20)      559 2024-05-14 13:08:59.000000 launchflow-0.4.0.dev0/launchflow/cli/gen/templates/fastapi/_postgres_template/app/schemas.py.jinja
+-rw-r--r--   0 calebvandyke   (501) staff       (20)      182 2024-05-14 13:08:59.000000 launchflow-0.4.0.dev0/launchflow/cli/gen/templates/fastapi/_postgres_template/launchflow.yaml.jinja
+-rw-r--r--   0 calebvandyke   (501) staff       (20)       79 2024-05-14 13:08:59.000000 launchflow-0.4.0.dev0/launchflow/cli/gen/templates/fastapi/_postgres_template/requirements.txt.jinja
+drwxr-xr-x   0 calebvandyke   (501) staff       (20)        0 2024-05-23 02:12:36.925777 launchflow-0.4.0.dev0/launchflow/cli/gen/templates/fastapi/_simple_template/
+-rw-r--r--   0 calebvandyke   (501) staff       (20)     1780 2024-05-14 13:08:59.000000 launchflow-0.4.0.dev0/launchflow/cli/gen/templates/fastapi/_simple_template/Dockerfile.jinja
+-rw-r--r--   0 calebvandyke   (501) staff       (20)     2665 2024-05-14 13:08:59.000000 launchflow-0.4.0.dev0/launchflow/cli/gen/templates/fastapi/_simple_template/README.md.jinja
+drwxr-xr-x   0 calebvandyke   (501) staff       (20)        0 2024-05-23 02:12:36.926129 launchflow-0.4.0.dev0/launchflow/cli/gen/templates/fastapi/_simple_template/app/
+-rw-r--r--   0 calebvandyke   (501) staff       (20)        0 2024-05-14 13:08:59.000000 launchflow-0.4.0.dev0/launchflow/cli/gen/templates/fastapi/_simple_template/app/__init__.py.jinja
+-rw-r--r--   0 calebvandyke   (501) staff       (20)       19 2024-05-14 13:08:59.000000 launchflow-0.4.0.dev0/launchflow/cli/gen/templates/fastapi/_simple_template/app/infra.py.jinja
+-rw-r--r--   0 calebvandyke   (501) staff       (20)      573 2024-05-14 13:08:59.000000 launchflow-0.4.0.dev0/launchflow/cli/gen/templates/fastapi/_simple_template/app/main.py.jinja
+-rw-r--r--   0 calebvandyke   (501) staff       (20)      182 2024-05-14 13:08:59.000000 launchflow-0.4.0.dev0/launchflow/cli/gen/templates/fastapi/_simple_template/launchflow.yaml.jinja
+-rw-r--r--   0 calebvandyke   (501) staff       (20)       79 2024-05-14 13:08:59.000000 launchflow-0.4.0.dev0/launchflow/cli/gen/templates/fastapi/_simple_template/requirements.txt.jinja
+-rw-r--r--   0 calebvandyke   (501) staff       (20)    19725 2024-05-16 16:00:23.000000 launchflow-0.4.0.dev0/launchflow/cli/gen/templates/fastapi/fastapi_template.py
+drwxr-xr-x   0 calebvandyke   (501) staff       (20)        0 2024-05-23 02:12:36.926359 launchflow-0.4.0.dev0/launchflow/cli/gen/templates/flask/
+-rw-r--r--   0 calebvandyke   (501) staff       (20)        0 2024-05-14 13:08:59.000000 launchflow-0.4.0.dev0/launchflow/cli/gen/templates/flask/__init__.py
+drwxr-xr-x   0 calebvandyke   (501) staff       (20)        0 2024-05-23 02:12:36.926739 launchflow-0.4.0.dev0/launchflow/cli/gen/templates/flask/__pycache__/
+-rw-r--r--   0 calebvandyke   (501) staff       (20)      195 2024-05-14 13:47:29.000000 launchflow-0.4.0.dev0/launchflow/cli/gen/templates/flask/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 calebvandyke   (501) staff       (20)    17192 2024-05-16 16:02:46.000000 launchflow-0.4.0.dev0/launchflow/cli/gen/templates/flask/__pycache__/flask_template.cpython-311.pyc
+drwxr-xr-x   0 calebvandyke   (501) staff       (20)        0 2024-05-23 02:12:36.927323 launchflow-0.4.0.dev0/launchflow/cli/gen/templates/flask/_postgres_template/
+-rw-r--r--   0 calebvandyke   (501) staff       (20)     1808 2024-05-14 13:08:59.000000 launchflow-0.4.0.dev0/launchflow/cli/gen/templates/flask/_postgres_template/Dockerfile.jinja
+-rw-r--r--   0 calebvandyke   (501) staff       (20)     2751 2024-05-14 13:08:59.000000 launchflow-0.4.0.dev0/launchflow/cli/gen/templates/flask/_postgres_template/README.md.jinja
+drwxr-xr-x   0 calebvandyke   (501) staff       (20)        0 2024-05-23 02:12:36.927995 launchflow-0.4.0.dev0/launchflow/cli/gen/templates/flask/_postgres_template/app/
+-rw-r--r--   0 calebvandyke   (501) staff       (20)        0 2024-05-14 13:08:59.000000 launchflow-0.4.0.dev0/launchflow/cli/gen/templates/flask/_postgres_template/app/__init__.py.jinja
+-rw-r--r--   0 calebvandyke   (501) staff       (20)       19 2024-05-14 13:08:59.000000 launchflow-0.4.0.dev0/launchflow/cli/gen/templates/flask/_postgres_template/app/infra.py.jinja
+-rw-r--r--   0 calebvandyke   (501) staff       (20)      297 2024-05-14 13:08:59.000000 launchflow-0.4.0.dev0/launchflow/cli/gen/templates/flask/_postgres_template/app/main.py.jinja
+-rw-r--r--   0 calebvandyke   (501) staff       (20)      371 2024-05-14 13:08:59.000000 launchflow-0.4.0.dev0/launchflow/cli/gen/templates/flask/_postgres_template/app/models.py.jinja
+-rw-r--r--   0 calebvandyke   (501) staff       (20)      559 2024-05-14 13:08:59.000000 launchflow-0.4.0.dev0/launchflow/cli/gen/templates/flask/_postgres_template/app/schemas.py.jinja
+-rw-r--r--   0 calebvandyke   (501) staff       (20)      182 2024-05-14 13:08:59.000000 launchflow-0.4.0.dev0/launchflow/cli/gen/templates/flask/_postgres_template/launchflow.yaml.jinja
+-rw-r--r--   0 calebvandyke   (501) staff       (20)       78 2024-05-14 13:08:59.000000 launchflow-0.4.0.dev0/launchflow/cli/gen/templates/flask/_postgres_template/requirements.txt.jinja
+drwxr-xr-x   0 calebvandyke   (501) staff       (20)        0 2024-05-23 02:12:36.928563 launchflow-0.4.0.dev0/launchflow/cli/gen/templates/flask/_simple_template/
+-rw-r--r--   0 calebvandyke   (501) staff       (20)     1808 2024-05-14 13:08:59.000000 launchflow-0.4.0.dev0/launchflow/cli/gen/templates/flask/_simple_template/Dockerfile.jinja
+-rw-r--r--   0 calebvandyke   (501) staff       (20)     2751 2024-05-14 13:08:59.000000 launchflow-0.4.0.dev0/launchflow/cli/gen/templates/flask/_simple_template/README.md.jinja
+drwxr-xr-x   0 calebvandyke   (501) staff       (20)        0 2024-05-23 02:12:36.928988 launchflow-0.4.0.dev0/launchflow/cli/gen/templates/flask/_simple_template/app/
+-rw-r--r--   0 calebvandyke   (501) staff       (20)        0 2024-05-14 13:08:59.000000 launchflow-0.4.0.dev0/launchflow/cli/gen/templates/flask/_simple_template/app/__init__.py.jinja
+-rw-r--r--   0 calebvandyke   (501) staff       (20)       19 2024-05-14 13:08:59.000000 launchflow-0.4.0.dev0/launchflow/cli/gen/templates/flask/_simple_template/app/infra.py.jinja
+-rw-r--r--   0 calebvandyke   (501) staff       (20)      324 2024-05-14 13:08:59.000000 launchflow-0.4.0.dev0/launchflow/cli/gen/templates/flask/_simple_template/app/main.py.jinja
+-rw-r--r--   0 calebvandyke   (501) staff       (20)      182 2024-05-14 13:08:59.000000 launchflow-0.4.0.dev0/launchflow/cli/gen/templates/flask/_simple_template/launchflow.yaml.jinja
+-rw-r--r--   0 calebvandyke   (501) staff       (20)       78 2024-05-14 13:08:59.000000 launchflow-0.4.0.dev0/launchflow/cli/gen/templates/flask/_simple_template/requirements.txt.jinja
+-rw-r--r--   0 calebvandyke   (501) staff       (20)    18651 2024-05-16 16:00:23.000000 launchflow-0.4.0.dev0/launchflow/cli/gen/templates/flask/flask_template.py
+-rw-r--r--   0 calebvandyke   (501) staff       (20)    33357 2024-05-23 00:43:11.000000 launchflow-0.4.0.dev0/launchflow/cli/main.py
+drwxr-xr-x   0 calebvandyke   (501) staff       (20)        0 2024-05-23 02:12:36.929255 launchflow-0.4.0.dev0/launchflow/cli/project/
+-rw-r--r--   0 calebvandyke   (501) staff       (20)        0 2024-05-14 13:08:59.000000 launchflow-0.4.0.dev0/launchflow/cli/project/__init__.py
+-rw-r--r--   0 calebvandyke   (501) staff       (20)     2667 2024-05-23 02:01:45.000000 launchflow-0.4.0.dev0/launchflow/cli/project/project_commands.py
+-rw-r--r--   0 calebvandyke   (501) staff       (20)     3220 2024-05-16 16:00:23.000000 launchflow-0.4.0.dev0/launchflow/cli/project_gen.py
+drwxr-xr-x   0 calebvandyke   (501) staff       (20)        0 2024-05-23 02:12:36.929504 launchflow-0.4.0.dev0/launchflow/cli/resources/
+-rw-r--r--   0 calebvandyke   (501) staff       (20)        0 2024-05-14 13:08:59.000000 launchflow-0.4.0.dev0/launchflow/cli/resources/__init__.py
+-rw-r--r--   0 calebvandyke   (501) staff       (20)     4436 2024-05-16 16:00:23.000000 launchflow-0.4.0.dev0/launchflow/cli/resources/resource_commands.py
+drwxr-xr-x   0 calebvandyke   (501) staff       (20)        0 2024-05-23 02:12:36.929780 launchflow-0.4.0.dev0/launchflow/cli/secrets/
+-rw-r--r--   0 calebvandyke   (501) staff       (20)        0 2024-05-14 13:08:59.000000 launchflow-0.4.0.dev0/launchflow/cli/secrets/__init__.py
+-rw-r--r--   0 calebvandyke   (501) staff       (20)     2807 2024-05-16 16:00:23.000000 launchflow-0.4.0.dev0/launchflow/cli/secrets/secret_commands.py
+drwxr-xr-x   0 calebvandyke   (501) staff       (20)        0 2024-05-23 02:12:36.930031 launchflow-0.4.0.dev0/launchflow/cli/services/
+-rw-r--r--   0 calebvandyke   (501) staff       (20)        0 2024-05-14 13:08:59.000000 launchflow-0.4.0.dev0/launchflow/cli/services/__init__.py
+-rw-r--r--   0 calebvandyke   (501) staff       (20)     4413 2024-05-16 16:00:23.000000 launchflow-0.4.0.dev0/launchflow/cli/services/service_commands.py
+-rw-r--r--   0 calebvandyke   (501) staff       (20)     3554 2024-05-14 13:08:59.000000 launchflow-0.4.0.dev0/launchflow/cli/utils.py
+-rw-r--r--   0 calebvandyke   (501) staff       (20)      482 2024-05-14 13:08:59.000000 launchflow-0.4.0.dev0/launchflow/cli/utyper.py
+drwxr-xr-x   0 calebvandyke   (501) staff       (20)        0 2024-05-23 02:12:36.932111 launchflow-0.4.0.dev0/launchflow/clients/
+-rw-r--r--   0 calebvandyke   (501) staff       (20)      368 2024-05-14 13:08:59.000000 launchflow-0.4.0.dev0/launchflow/clients/__init__.py
+-rw-r--r--   0 calebvandyke   (501) staff       (20)     1405 2024-05-17 15:58:02.000000 launchflow-0.4.0.dev0/launchflow/clients/accounts_client.py
+-rw-r--r--   0 calebvandyke   (501) staff       (20)      973 2024-05-21 20:59:12.000000 launchflow-0.4.0.dev0/launchflow/clients/client.py
+-rw-r--r--   0 calebvandyke   (501) staff       (20)     7680 2024-05-14 13:08:59.000000 launchflow-0.4.0.dev0/launchflow/clients/docker_client.py
+-rw-r--r--   0 calebvandyke   (501) staff       (20)     5297 2024-05-21 20:59:12.000000 launchflow-0.4.0.dev0/launchflow/clients/environments_client.py
+-rw-r--r--   0 calebvandyke   (501) staff       (20)     4178 2024-05-21 20:59:12.000000 launchflow-0.4.0.dev0/launchflow/clients/projects_client.py
+-rw-r--r--   0 calebvandyke   (501) staff       (20)     5542 2024-05-17 15:58:18.000000 launchflow-0.4.0.dev0/launchflow/clients/resources_client.py
+-rw-r--r--   0 calebvandyke   (501) staff       (20)     3767 2024-05-18 14:19:48.000000 launchflow-0.4.0.dev0/launchflow/clients/response_schemas.py
+-rw-r--r--   0 calebvandyke   (501) staff       (20)     4789 2024-05-17 15:58:21.000000 launchflow-0.4.0.dev0/launchflow/clients/services_client.py
+drwxr-xr-x   0 calebvandyke   (501) staff       (20)        0 2024-05-23 02:12:36.932933 launchflow-0.4.0.dev0/launchflow/config/
+-rw-r--r--   0 calebvandyke   (501) staff       (20)       99 2024-05-17 14:07:15.000000 launchflow-0.4.0.dev0/launchflow/config/__init__.py
+-rw-r--r--   0 calebvandyke   (501) staff       (20)     4755 2024-05-23 00:43:11.000000 launchflow-0.4.0.dev0/launchflow/config/launchflow_config.py
+-rw-r--r--   0 calebvandyke   (501) staff       (20)     2551 2024-05-14 13:08:59.000000 launchflow-0.4.0.dev0/launchflow/config/launchflow_env.py
+-rw-r--r--   0 calebvandyke   (501) staff       (20)     8294 2024-05-23 00:43:11.000000 launchflow-0.4.0.dev0/launchflow/config/launchflow_yaml.py
+drwxr-xr-x   0 calebvandyke   (501) staff       (20)        0 2024-05-23 02:12:36.933575 launchflow-0.4.0.dev0/launchflow/context/
+-rw-r--r--   0 calebvandyke   (501) staff       (20)      179 2024-05-14 13:08:59.000000 launchflow-0.4.0.dev0/launchflow/context/__init__.py
+-rw-r--r--   0 calebvandyke   (501) staff       (20)     8669 2024-05-16 16:00:23.000000 launchflow-0.4.0.dev0/launchflow/context/docker_ctx.py
+-rw-r--r--   0 calebvandyke   (501) staff       (20)    20696 2024-05-16 16:00:23.000000 launchflow-0.4.0.dev0/launchflow/context/launchflow_ctx.py
+drwxr-xr-x   0 calebvandyke   (501) staff       (20)        0 2024-05-23 02:12:36.934160 launchflow-0.4.0.dev0/launchflow/dependencies/
+-rw-r--r--   0 calebvandyke   (501) staff       (20)        0 2024-05-23 00:43:11.000000 launchflow-0.4.0.dev0/launchflow/dependencies/__init__.py
+-rw-r--r--   0 calebvandyke   (501) staff       (20)     1639 2024-05-23 02:03:58.000000 launchflow-0.4.0.dev0/launchflow/dependencies/opentofu.py
+drwxr-xr-x   0 calebvandyke   (501) staff       (20)        0 2024-05-23 02:12:36.934646 launchflow-0.4.0.dev0/launchflow/docker/
+-rw-r--r--   0 calebvandyke   (501) staff       (20)       81 2024-05-14 13:08:59.000000 launchflow-0.4.0.dev0/launchflow/docker/__init__.py
+-rw-r--r--   0 calebvandyke   (501) staff       (20)     5157 2024-05-16 16:00:23.000000 launchflow-0.4.0.dev0/launchflow/docker/postgres.py
+-rw-r--r--   0 calebvandyke   (501) staff       (20)     3552 2024-05-16 16:00:23.000000 launchflow-0.4.0.dev0/launchflow/docker/redis.py
+-rw-r--r--   0 calebvandyke   (501) staff       (20)     2856 2024-05-23 00:43:11.000000 launchflow-0.4.0.dev0/launchflow/docker/resource.py
+-rw-r--r--   0 calebvandyke   (501) staff       (20)     9300 2024-05-23 00:43:11.000000 launchflow-0.4.0.dev0/launchflow/exceptions.py
+-rw-r--r--   0 calebvandyke   (501) staff       (20)     5196 2024-05-14 13:08:59.000000 launchflow-0.4.0.dev0/launchflow/fastapi.py
+-rw-r--r--   0 calebvandyke   (501) staff       (20)       52 2024-05-14 13:08:59.000000 launchflow-0.4.0.dev0/launchflow/flask.py
+drwxr-xr-x   0 calebvandyke   (501) staff       (20)        0 2024-05-23 02:12:36.936094 launchflow-0.4.0.dev0/launchflow/flows/
+-rw-r--r--   0 calebvandyke   (501) staff       (20)      129 2024-05-14 13:08:59.000000 launchflow-0.4.0.dev0/launchflow/flows/__init__.py
+-rw-r--r--   0 calebvandyke   (501) staff       (20)     1237 2024-05-16 16:00:23.000000 launchflow-0.4.0.dev0/launchflow/flows/account_id.py
+-rw-r--r--   0 calebvandyke   (501) staff       (20)     4172 2024-05-16 16:00:23.000000 launchflow-0.4.0.dev0/launchflow/flows/auth.py
+-rw-r--r--   0 calebvandyke   (501) staff       (20)    38828 2024-05-16 16:00:23.000000 launchflow-0.4.0.dev0/launchflow/flows/cloud_provider.py
+-rw-r--r--   0 calebvandyke   (501) staff       (20)    12538 2024-05-21 20:59:12.000000 launchflow-0.4.0.dev0/launchflow/flows/environments_flows.py
+-rw-r--r--   0 calebvandyke   (501) staff       (20)     3538 2024-05-21 20:59:12.000000 launchflow-0.4.0.dev0/launchflow/flows/project_flows.py
+-rw-r--r--   0 calebvandyke   (501) staff       (20)    26523 2024-05-23 00:43:11.000000 launchflow-0.4.0.dev0/launchflow/flows/resource_flows.py
+-rw-r--r--   0 calebvandyke   (501) staff       (20)    10392 2024-05-16 16:00:23.000000 launchflow-0.4.0.dev0/launchflow/flows/service_flows.py
+drwxr-xr-x   0 calebvandyke   (501) staff       (20)        0 2024-05-23 02:12:36.938872 launchflow-0.4.0.dev0/launchflow/gcp/
+-rw-r--r--   0 calebvandyke   (501) staff       (20)      467 2024-05-14 13:23:06.000000 launchflow-0.4.0.dev0/launchflow/gcp/__init__.py
+-rw-r--r--   0 calebvandyke   (501) staff       (20)     6275 2024-05-16 16:00:23.000000 launchflow-0.4.0.dev0/launchflow/gcp/bigquery.py
+-rw-r--r--   0 calebvandyke   (501) staff       (20)     4208 2024-05-14 13:08:59.000000 launchflow-0.4.0.dev0/launchflow/gcp/cloud_run.py
+-rw-r--r--   0 calebvandyke   (501) staff       (20)     5467 2024-05-16 16:00:23.000000 launchflow-0.4.0.dev0/launchflow/gcp/cloud_tasks.py
+-rw-r--r--   0 calebvandyke   (501) staff       (20)     9268 2024-05-16 16:00:23.000000 launchflow-0.4.0.dev0/launchflow/gcp/cloudsql.py
+-rw-r--r--   0 calebvandyke   (501) staff       (20)    13241 2024-05-16 16:00:23.000000 launchflow-0.4.0.dev0/launchflow/gcp/compute_engine.py
+-rw-r--r--   0 calebvandyke   (501) staff       (20)     4039 2024-05-22 19:01:28.000000 launchflow-0.4.0.dev0/launchflow/gcp/gcs.py
+-rw-r--r--   0 calebvandyke   (501) staff       (20)     3624 2024-05-16 16:00:23.000000 launchflow-0.4.0.dev0/launchflow/gcp/memorystore.py
+-rw-r--r--   0 calebvandyke   (501) staff       (20)     2615 2024-05-16 16:00:23.000000 launchflow-0.4.0.dev0/launchflow/gcp/pubsub.py
+-rw-r--r--   0 calebvandyke   (501) staff       (20)      254 2024-05-14 13:08:59.000000 launchflow-0.4.0.dev0/launchflow/gcp/resource.py
+-rw-r--r--   0 calebvandyke   (501) staff       (20)     2997 2024-05-16 16:00:23.000000 launchflow-0.4.0.dev0/launchflow/gcp/secret_manager.py
+-rw-r--r--   0 calebvandyke   (501) staff       (20)     2630 2024-05-16 16:00:23.000000 launchflow-0.4.0.dev0/launchflow/gcp/utils.py
+-rw-r--r--   0 calebvandyke   (501) staff       (20)     1243 2024-05-21 20:59:12.000000 launchflow-0.4.0.dev0/launchflow/gcp_clients.py
+-rw-r--r--   0 calebvandyke   (501) staff       (20)      953 2024-05-14 13:08:59.000000 launchflow-0.4.0.dev0/launchflow/generic_clients.py
+-rw-r--r--   0 calebvandyke   (501) staff       (20)     4905 2024-05-16 16:00:23.000000 launchflow-0.4.0.dev0/launchflow/generics.py
+-rw-r--r--   0 calebvandyke   (501) staff       (20)     7247 2024-05-21 20:59:12.000000 launchflow-0.4.0.dev0/launchflow/locks.py
+drwxr-xr-x   0 calebvandyke   (501) staff       (20)        0 2024-05-23 02:12:36.940098 launchflow-0.4.0.dev0/launchflow/managers/
+-rw-r--r--   0 calebvandyke   (501) staff       (20)        0 2024-05-21 20:59:12.000000 launchflow-0.4.0.dev0/launchflow/managers/__init__.py
+-rw-r--r--   0 calebvandyke   (501) staff       (20)      530 2024-05-21 20:59:12.000000 launchflow-0.4.0.dev0/launchflow/managers/base.py
+-rw-r--r--   0 calebvandyke   (501) staff       (20)     8223 2024-05-23 00:43:11.000000 launchflow-0.4.0.dev0/launchflow/managers/environment_manager.py
+-rw-r--r--   0 calebvandyke   (501) staff       (20)     6311 2024-05-21 20:59:12.000000 launchflow-0.4.0.dev0/launchflow/managers/flow_state_manager.py
+-rw-r--r--   0 calebvandyke   (501) staff       (20)     6680 2024-05-23 00:43:11.000000 launchflow-0.4.0.dev0/launchflow/managers/resource_manager.py
+-rw-r--r--   0 calebvandyke   (501) staff       (20)     5001 2024-05-21 20:59:12.000000 launchflow-0.4.0.dev0/launchflow/managers/service_manager.py
+drwxr-xr-x   0 calebvandyke   (501) staff       (20)        0 2024-05-23 02:12:36.940468 launchflow-0.4.0.dev0/launchflow/models/
+-rw-r--r--   0 calebvandyke   (501) staff       (20)        0 2024-05-21 20:59:12.000000 launchflow-0.4.0.dev0/launchflow/models/__init__.py
+-rw-r--r--   0 calebvandyke   (501) staff       (20)     1241 2024-05-16 16:00:23.000000 launchflow-0.4.0.dev0/launchflow/models/enums.py
+-rw-r--r--   0 calebvandyke   (501) staff       (20)     2273 2024-05-23 00:43:11.000000 launchflow-0.4.0.dev0/launchflow/models/flow_state.py
+-rw-r--r--   0 calebvandyke   (501) staff       (20)     4633 2024-05-16 16:00:23.000000 launchflow-0.4.0.dev0/launchflow/operations.py
+-rw-r--r--   0 calebvandyke   (501) staff       (20)     4252 2024-05-23 00:43:11.000000 launchflow-0.4.0.dev0/launchflow/resource.py
+-rw-r--r--   0 calebvandyke   (501) staff       (20)     2965 2024-05-14 13:08:59.000000 launchflow-0.4.0.dev0/launchflow/service.py
+drwxr-xr-x   0 calebvandyke   (501) staff       (20)        0 2024-05-23 02:12:36.940680 launchflow-0.4.0.dev0/launchflow/tests/
+-rw-r--r--   0 calebvandyke   (501) staff       (20)        0 2024-05-14 13:08:59.000000 launchflow-0.4.0.dev0/launchflow/tests/__init__.py
+-rw-r--r--   0 calebvandyke   (501) staff       (20)     2751 2024-05-16 16:00:23.000000 launchflow-0.4.0.dev0/launchflow/tests/generics_test.py
+-rw-r--r--   0 calebvandyke   (501) staff       (20)     1519 2024-05-14 13:08:59.000000 launchflow-0.4.0.dev0/launchflow/utils.py
+-rw-r--r--   0 calebvandyke   (501) staff       (20)      950 2024-05-16 18:22:31.000000 launchflow-0.4.0.dev0/launchflow/validation.py
+drwxr-xr-x   0 calebvandyke   (501) staff       (20)        0 2024-05-23 02:12:36.941006 launchflow-0.4.0.dev0/launchflow/workflows/
+-rw-r--r--   0 calebvandyke   (501) staff       (20)      593 2024-05-16 18:22:31.000000 launchflow-0.4.0.dev0/launchflow/workflows/__init__.py
+drwxr-xr-x   0 calebvandyke   (501) staff       (20)        0 2024-05-23 02:12:36.941528 launchflow-0.4.0.dev0/launchflow/workflows/aws_env_creation/
+-rw-r--r--   0 calebvandyke   (501) staff       (20)        0 2024-05-16 18:22:31.000000 launchflow-0.4.0.dev0/launchflow/workflows/aws_env_creation/__init__.py
+-rw-r--r--   0 calebvandyke   (501) staff       (20)     4308 2024-05-21 20:59:12.000000 launchflow-0.4.0.dev0/launchflow/workflows/aws_env_creation/aws_environment_creation.py
+-rw-r--r--   0 calebvandyke   (501) staff       (20)      585 2024-05-21 20:59:12.000000 launchflow-0.4.0.dev0/launchflow/workflows/aws_env_creation/schemas.py
+drwxr-xr-x   0 calebvandyke   (501) staff       (20)        0 2024-05-23 02:12:36.941906 launchflow-0.4.0.dev0/launchflow/workflows/aws_env_deletion/
+-rw-r--r--   0 calebvandyke   (501) staff       (20)        0 2024-05-16 18:22:31.000000 launchflow-0.4.0.dev0/launchflow/workflows/aws_env_deletion/__init__.py
+-rw-r--r--   0 calebvandyke   (501) staff       (20)     2028 2024-05-21 20:59:12.000000 launchflow-0.4.0.dev0/launchflow/workflows/aws_env_deletion/aws_environment_deletion.py
+-rw-r--r--   0 calebvandyke   (501) staff       (20)      284 2024-05-21 20:59:12.000000 launchflow-0.4.0.dev0/launchflow/workflows/aws_env_deletion/schemas.py
+drwxr-xr-x   0 calebvandyke   (501) staff       (20)        0 2024-05-23 02:12:36.942161 launchflow-0.4.0.dev0/launchflow/workflows/commands/
+-rw-r--r--   0 calebvandyke   (501) staff       (20)        0 2024-05-14 14:57:43.000000 launchflow-0.4.0.dev0/launchflow/workflows/commands/__init__.py
+-rw-r--r--   0 calebvandyke   (501) staff       (20)     9755 2024-05-23 00:43:11.000000 launchflow-0.4.0.dev0/launchflow/workflows/commands/tf_commands.py
+drwxr-xr-x   0 calebvandyke   (501) staff       (20)        0 2024-05-23 02:12:36.942673 launchflow-0.4.0.dev0/launchflow/workflows/gcp_env_creation/
+-rw-r--r--   0 calebvandyke   (501) staff       (20)      124 2024-05-14 14:29:45.000000 launchflow-0.4.0.dev0/launchflow/workflows/gcp_env_creation/__init__.py
+-rw-r--r--   0 calebvandyke   (501) staff       (20)    12892 2024-05-21 20:59:12.000000 launchflow-0.4.0.dev0/launchflow/workflows/gcp_env_creation/gcp_environment_creation.py
+-rw-r--r--   0 calebvandyke   (501) staff       (20)      529 2024-05-21 20:59:12.000000 launchflow-0.4.0.dev0/launchflow/workflows/gcp_env_creation/schemas.py
+drwxr-xr-x   0 calebvandyke   (501) staff       (20)        0 2024-05-23 02:12:36.943041 launchflow-0.4.0.dev0/launchflow/workflows/gcp_env_deletion/
+-rw-r--r--   0 calebvandyke   (501) staff       (20)        0 2024-05-14 20:06:16.000000 launchflow-0.4.0.dev0/launchflow/workflows/gcp_env_deletion/__init__.py
+-rw-r--r--   0 calebvandyke   (501) staff       (20)     1557 2024-05-16 18:22:31.000000 launchflow-0.4.0.dev0/launchflow/workflows/gcp_env_deletion/gcp_environment_deletion.py
+-rw-r--r--   0 calebvandyke   (501) staff       (20)      236 2024-05-20 14:25:07.000000 launchflow-0.4.0.dev0/launchflow/workflows/gcp_env_deletion/schemas.py
+drwxr-xr-x   0 calebvandyke   (501) staff       (20)        0 2024-05-23 02:12:36.943649 launchflow-0.4.0.dev0/launchflow/workflows/tf/
+-rw-r--r--   0 calebvandyke   (501) staff       (20)     1695 2024-05-20 20:27:48.000000 launchflow-0.4.0.dev0/launchflow/workflows/tf/resource_schemas.py
+-rw-r--r--   0 calebvandyke   (501) staff       (20)     4253 2024-05-23 00:43:11.000000 launchflow-0.4.0.dev0/launchflow/workflows/tf/tf.py
+drwxr-xr-x   0 calebvandyke   (501) staff       (20)        0 2024-05-23 02:12:36.945934 launchflow-0.4.0.dev0/launchflow/workflows/tf/tf_resources/
+-rw-r--r--   0 calebvandyke   (501) staff       (20)        0 2024-05-20 20:27:48.000000 launchflow-0.4.0.dev0/launchflow/workflows/tf/tf_resources/__init__.py
+-rw-r--r--   0 calebvandyke   (501) staff       (20)     1790 2024-05-20 20:27:48.000000 launchflow-0.4.0.dev0/launchflow/workflows/tf/tf_resources/aws_ec2.py
+-rw-r--r--   0 calebvandyke   (501) staff       (20)     2958 2024-05-20 20:27:48.000000 launchflow-0.4.0.dev0/launchflow/workflows/tf/tf_resources/aws_elasticache_redis.py
+-rw-r--r--   0 calebvandyke   (501) staff       (20)      437 2024-05-20 20:27:48.000000 launchflow-0.4.0.dev0/launchflow/workflows/tf/tf_resources/aws_empty.py
+-rw-r--r--   0 calebvandyke   (501) staff       (20)     3408 2024-05-20 20:27:48.000000 launchflow-0.4.0.dev0/launchflow/workflows/tf/tf_resources/aws_rds_postgres.py
+-rw-r--r--   0 calebvandyke   (501) staff       (20)      952 2024-05-20 20:27:48.000000 launchflow-0.4.0.dev0/launchflow/workflows/tf/tf_resources/aws_s3_bucket.py
+-rw-r--r--   0 calebvandyke   (501) staff       (20)      980 2024-05-20 20:27:48.000000 launchflow-0.4.0.dev0/launchflow/workflows/tf/tf_resources/aws_secrets_manager_secret.py
+-rw-r--r--   0 calebvandyke   (501) staff       (20)     1017 2024-05-20 20:27:48.000000 launchflow-0.4.0.dev0/launchflow/workflows/tf/tf_resources/gcp_bigquery_dataset.py
+-rw-r--r--   0 calebvandyke   (501) staff       (20)     2076 2024-05-20 20:27:48.000000 launchflow-0.4.0.dev0/launchflow/workflows/tf/tf_resources/gcp_compute_engine.py
+-rw-r--r--   0 calebvandyke   (501) staff       (20)      389 2024-05-20 20:27:48.000000 launchflow-0.4.0.dev0/launchflow/workflows/tf/tf_resources/gcp_empty.py
+-rw-r--r--   0 calebvandyke   (501) staff       (20)     2757 2024-05-20 20:27:48.000000 launchflow-0.4.0.dev0/launchflow/workflows/tf/tf_resources/gcp_memorystore_redis.py
+-rw-r--r--   0 calebvandyke   (501) staff       (20)      717 2024-05-20 20:27:48.000000 launchflow-0.4.0.dev0/launchflow/workflows/tf/tf_resources/gcp_pubsub_topic.py
+-rw-r--r--   0 calebvandyke   (501) staff       (20)      731 2024-05-20 20:27:48.000000 launchflow-0.4.0.dev0/launchflow/workflows/tf/tf_resources/gcp_secret_manager_secret.py
+-rw-r--r--   0 calebvandyke   (501) staff       (20)     4011 2024-05-20 20:27:48.000000 launchflow-0.4.0.dev0/launchflow/workflows/tf/tf_resources/gcp_sql_postgres.py
+-rw-r--r--   0 calebvandyke   (501) staff       (20)      743 2024-05-22 19:01:28.000000 launchflow-0.4.0.dev0/launchflow/workflows/tf/tf_resources/gcp_storage_bucket.py
+-rw-r--r--   0 calebvandyke   (501) staff       (20)     1991 2024-05-23 00:43:11.000000 launchflow-0.4.0.dev0/launchflow/workflows/tf/tf_utils.py
+-rw-r--r--   0 calebvandyke   (501) staff       (20)     1455 2024-05-21 20:59:12.000000 launchflow-0.4.0.dev0/launchflow/workflows/utils.py
+drwxr-xr-x   0 calebvandyke   (501) staff       (20)        0 2024-05-23 02:12:36.946257 launchflow-0.4.0.dev0/launchflow.egg-info/
+-rw-r--r--   0 calebvandyke   (501) staff       (20)     3890 2024-05-23 02:12:36.000000 launchflow-0.4.0.dev0/launchflow.egg-info/PKG-INFO
+-rw-r--r--   0 calebvandyke   (501) staff       (20)    11381 2024-05-23 02:12:36.000000 launchflow-0.4.0.dev0/launchflow.egg-info/SOURCES.txt
+-rw-r--r--   0 calebvandyke   (501) staff       (20)        1 2024-05-23 02:12:36.000000 launchflow-0.4.0.dev0/launchflow.egg-info/dependency_links.txt
+-rw-r--r--   0 calebvandyke   (501) staff       (20)       84 2024-05-23 02:12:36.000000 launchflow-0.4.0.dev0/launchflow.egg-info/entry_points.txt
+-rw-r--r--   0 calebvandyke   (501) staff       (20)      471 2024-05-23 02:12:36.000000 launchflow-0.4.0.dev0/launchflow.egg-info/requires.txt
+-rw-r--r--   0 calebvandyke   (501) staff       (20)       11 2024-05-23 02:12:36.000000 launchflow-0.4.0.dev0/launchflow.egg-info/top_level.txt
+-rw-r--r--   0 calebvandyke   (501) staff       (20)     1786 2024-05-23 02:06:28.000000 launchflow-0.4.0.dev0/pyproject.toml
+-rw-r--r--   0 calebvandyke   (501) staff       (20)       38 2024-05-23 02:12:36.947377 launchflow-0.4.0.dev0/setup.cfg
```

### Comparing `launchflow-0.3.9.dev8/README.md` & `launchflow-0.4.0.dev0/README.md`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev8/launchflow/aws/rds.py` & `launchflow-0.4.0.dev0/launchflow/docker/postgres.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,7 @@
-# Handling imports and missing dependencies
-try:
-    import boto3
-except ImportError:
-    boto3 = None
-
 try:
     import asyncpg
 except ImportError:
     asyncpg = None
 
 try:
     import pg8000
@@ -22,108 +16,123 @@
 try:
     from sqlalchemy.ext.asyncio import create_async_engine
 except ImportError:
     async_sessionmaker = None
     create_async_engine = None
 
 try:
-    from sqlalchemy import create_engine, event
+    from sqlalchemy import create_engine
 except ImportError:
-    event = None
     create_engine = None
     DeclarativeBase = None
     sessionmaker = None
 
-# Importing the required modules
 
-from launchflow.resource import Resource
 from pydantic import BaseModel
 
+from launchflow.context.docker_ctx import find_open_port
+from launchflow.docker.resource import DockerResource
 
-# Connection information model
-class RDSPostgresConnectionInfo(BaseModel):
-    endpoint: str
-    username: str
+
+class DockerPostgresConnectionInfo(BaseModel):
     password: str
-    port: int
-    dbname: str
-    region: str
-
-
-class RDSPostgres(Resource[RDSPostgresConnectionInfo]):
-    """A RDS SQL Postgres resource.
-
-    Args:
-    - `name`: The name of the Cloud SQL Postgres instance.
-
-    Example usage:
-    ```python
-    import launchflow as lf
-    db = lf.aws.RDSPostgres("my-pg-db")
-    ```
-    """
-
-    def __init__(
-        self,
-        name: str,
-    ) -> None:
+    postgres_port: str
+
+
+
+
+class DockerPostgres(DockerResource[DockerPostgresConnectionInfo]):
+    def __init__(self, name: str, *, password: str = "password") -> None:
+        """A Postgres resource running in a Docker container.
+
+        **Args**:
+        - `name` (str): The name of the Postgres resource. This must be globally unique.
+        - `password` (str): The password for the Postgres DB. If not provided, a standard password will be used.
+
+        **Example usage**:
+        ```python
+        from sqlalchemy import text
+        import launchflow as lf
+
+        postgres = lf.docker.Postgres("postgres-db")
+        engine = postgres.sqlalchemy_engine()
+
+        with engine.connect() as connection:
+            print(connection.execute(text("SELECT 1")).fetchone())  # prints (1,)
+        ```
+        """
+        self.password = password
+        postgres_port = find_open_port()
+
         super().__init__(
             name=name,
-            product_name="aws_rds_postgres",
-            create_args={},
+            env_vars={
+                "POSTGRES_PASSWORD": self.password,
+                "POSTGRES_DB": "postgres",
+                "POSTGRES_USER": "postgres",
+            },
+            command=None,
+            ports={"5432/tcp": postgres_port},
+            docker_image="postgres",
+        )
+
+    def connection_info(self) -> DockerPostgresConnectionInfo:
+        return DockerPostgresConnectionInfo(
+            password=self.password,
+            postgres_port=str(self.ports["5432/tcp"]),
         )
 
     def django_settings(self):
         if psycopg2 is None:
             raise ImportError(
                 "psycopg2 is not installed. Please install it with `pip install psycopg2`."
             )
 
         connection_info = self.connect()
         return {
             "ENGINE": "django.db.backends.postgresql_psycopg2",
-            "NAME": connection_info.dbname,
-            "USER": connection_info.username,
+            "NAME": "postgres",
+            "USER": "postgres",
             "PASSWORD": connection_info.password,
-            "HOST": connection_info.endpoint,
-            "PORT": connection_info.port,
+            "HOST": "localhost",
+            "PORT": connection_info.postgres_port,
         }
 
     def sqlalchemy_engine_options(self):
         if pg8000 is None:
             raise ImportError(
                 "pg8000 is not installed. Please install it with `pip install pg8000`."
             )
 
         connection_info = self.connect()
         return {
-            "url": f"postgresql+pg8000://{connection_info.username}:{connection_info.password}@{connection_info.endpoint}:{connection_info.port}/{connection_info.dbname}",
+            "url": f"postgresql+pg8000://postgres:{connection_info.password}@localhost:{connection_info.postgres_port}/postgres",
         }
 
     async def sqlalchemy_async_engine_options(self):
         if asyncpg is None:
             raise ImportError(
                 "asyncpg is not installed. Please install it with `pip install asyncpg`."
             )
 
         connection_info = await self.connect_async()
         return {
-            "url": f"postgresql+asyncpg://{connection_info.username}:{connection_info.password}@{connection_info.endpoint}:{connection_info.port}/{connection_info.dbname}"
+            "url": f"postgresql+asyncpg://postgres:{connection_info.password}@localhost:{connection_info.postgres_port}/postgres"
         }
 
     def sqlalchemy_engine(self, **engine_kwargs):
-        """Returns a SQLAlchemy engine for connecting to the RDS SQL Postgres instance.
+        """Returns a SQLAlchemy engine for connecting to a postgres instance hosted on Docker.
 
         Args:
         - `**engine_kwargs`: Additional keyword arguments to pass to `sqlalchemy.create_engine`.
 
-        Example usage:
+        **Example usage:**
         ```python
         import launchflow as lf
-        db = lf.aws.RDSPostgres("my-pg-db")
+        db = lf.docker.Postgres("my-pg-db")
         engine = db.sqlalchemy_engine()
         ```
         """
         if create_engine is None:
             raise ImportError(
                 "SQLAlchemy is not installed. Please install it with "
                 "`pip install sqlalchemy`."
@@ -131,23 +140,23 @@
 
         engine_options = self.sqlalchemy_engine_options()
         engine_options.update(engine_kwargs)
 
         return create_engine(**engine_options)
 
     async def sqlalchemy_async_engine(self, **engine_kwargs):
-        """Returns an async SQLAlchemy engine for connecting to the RDS SQL Postgres instance.
+        """Returns an async SQLAlchemy engine for connecting to a postgres instance hosted on Docker.
 
         Args:
         - `**engine_kwargs`: Additional keyword arguments to pass to `create_async_engine`.
 
-        Example usage:
+        **Example usage:**
         ```python
         import launchflow as lf
-        db = lf.aws.RDSPostgres("my-pg-db")
+        db = lf.docker.Postgres("my-pg-db")
         engine = await db.sqlalchemy_async_engine()
         ```
         """
         if create_async_engine is None:
             raise ImportError(
                 "SQLAlchemy asyncio extension is not installed. "
                 "Please install it with `pip install sqlalchemy[asyncio]`."
```

### Comparing `launchflow-0.3.9.dev8/launchflow/aws/s3.py` & `launchflow-0.4.0.dev0/launchflow/aws/s3.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,38 +5,49 @@
     import boto3
 except ImportError:
     boto3 = None
 
 
 from typing import Union
 
-from launchflow.resource import Resource
 from pydantic import BaseModel
 
+from launchflow.aws.resource import AWSResource
+
 
 class S3BucketConnectionInfo(BaseModel):
     bucket_name: str
 
 
-class S3Bucket(Resource[S3BucketConnectionInfo]):
-    """A S3 Bucket resource.
-
-    **Attributes**:
-    - `name` (str): The name of the bucket. This must be globally unique.
-    - `region` (str): The region of the bucket. Defaults to the environment default.
+class S3Bucket(AWSResource[S3BucketConnectionInfo]):
+    """A storage bucket in AWS's S3 service.
 
-    Example usage:
+    **Example usage:**
     ```python
     import launchflow as lf
-    bucket = lf.aws.S3Bucket("my-bucket")
-    bucket.blob("my-file").upload_from_filename("my-file")
+
+    s3 = lf.aws.S3Bucket("my-bucket")
+
+    # Quick utilities for reading and writing file contents
+    s3.upload_from_string("file contents", "path/in/s3/file.txt")
+
+    # You can also use the boto3 library directly
+    bucket = s3.bucket()
+    with open("my-file", "r") as f:
+        bucket.upload_fileobj(f, "path/in/s3/file.txt")
     ```
     """
 
     def __init__(self, name: str, *, region=None) -> None:
+        """Create a new S3 bucket resource.
+
+        **Args**:
+        - `name` (str): The name of the bucket. This must be globally unique.
+        - `region` (str): The region of the bucket. Defaults to the environment default.
+        """
         super().__init__(
             name=name,
             product_name="aws_s3_bucket",
             create_args={"region": region},
         )
         # public metadata
         self.region = region
@@ -58,15 +69,15 @@
     def upload_file(self, to_upload: Union[str, IO], bucket_path: str):
         """Uploads a file to the S3 bucket.
 
         Args:
         - `to_upload` (Union[str, IO]): The file to upload. This can be a string representing the path to the file, or a file-like object.
         - `bucket_path` (str): The path to upload the file to in the bucket.
 
-        Example usage:
+        **Example usage:**
         ```python
         import launchflow as lf
         bucket = lf.aws.S3Bucket("my-bucket")
         bucket.upload_file("my-file.txt", "my-file.txt")
         bucket.upload_file(open("my-file.txt", "r"), "my-file.txt")
         ```
         """
@@ -79,15 +90,15 @@
     def upload_from_string(self, to_upload: str, bucket_path: str):
         """Uploads a string to the S3 bucket.
 
         Args:
         - `to_upload` (str): The string to upload.
         - `bucket_path` (str): The path to upload the string to in the bucket.
 
-        Example usage:
+        **Example usage:**
         ```python
         import launchflow as lf
 
         bucket = lf.aws.S3Bucket("my-bucket")
         bucket.upload_from_string("hello", "hello.txt")
         ```
         """
@@ -96,15 +107,15 @@
 
     def download_file(self, bucket_path: str):
         """Downloads a file from the S3 bucket.
 
         Args:
         - `bucket_path` (str): The path to the file in the bucket.
 
-        Example usage:
+        **Example usage:**
         ```python
         import launchflow as lf
         bucket = lf.aws.S3Bucket("my-bucket")
         with open("my-file.txt", "w") as f:
             f.write(bucket.download_file("my-file.txt"))
         ```
         """
```

### Comparing `launchflow-0.3.9.dev8/launchflow/cache/launchflow_tmp.py` & `launchflow-0.4.0.dev0/launchflow/cache/launchflow_tmp.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev8/launchflow/cli/accounts/account_commands.py` & `launchflow-0.4.0.dev0/launchflow/cli/accounts/account_commands.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import typer
+
 from launchflow.cli.utils import print_response
 from launchflow.cli.utyper import UTyper
-from launchflow.exceptions import LaunchFlowRequestFailure
-
 from launchflow.clients import async_launchflow_client_ctx
+from launchflow.exceptions import LaunchFlowRequestFailure
 
 app = UTyper(help="Commands for managing accounts in LaunchFlow")
 
 
 @app.command()
 async def get(
     account_id: str = typer.Argument("The account ID to fetch. Format: `account_123`"),
```

### Comparing `launchflow-0.3.9.dev8/launchflow/cli/config/config_commands.py` & `launchflow-0.4.0.dev0/launchflow/cli/config/config_commands.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from typing import Optional
 
 import typer
+
 from launchflow.cli.utils import print_response
 from launchflow.cli.utyper import UTyper
+from launchflow.clients import async_launchflow_client_ctx
 from launchflow.config import config
 from launchflow.flows.account_id import get_account_id_no_config
 
-from launchflow.clients import async_launchflow_client_ctx
-
 app = UTyper(help="Commands for interacting with your local LaunchFlow configuration.")
 
 
 @app.command()
 def get():
     """Print out the current LaunchFlow config."""
     print_response("Config", config.info())
```

### Comparing `launchflow-0.3.9.dev8/launchflow/cli/constants.py` & `launchflow-0.4.0.dev0/launchflow/cli/constants.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,6 +1,8 @@
 PROJECT_HELP = "The project name to use. If not specified, we will check your local config, if not in your config it will be selected interactively."
 ENVIRONMENT_HELP = "The environment name to use. If not specified, we will check your local config, if not in your config it will be selected interactively."
+RUN_ENVIRONMENT_HELP = "The environment name to use or `local` to run with local versions of your generic resources."
 SERVICE_HELP = "The service name to use. If not specified, we will check your local config, if not in your config it will be selected interactively."
 SCAN_DIRECTORY_HELP = (
     "Directory to scan for resources. Defaults to the current working directory."
 )
+API_KEY_HELP = "API key to use for this request. If not set will fallback to your user local credentials from `launchflow login`"
```

### Comparing `launchflow-0.3.9.dev8/launchflow/cli/gen/template.py` & `launchflow-0.4.0.dev0/launchflow/cli/gen/template.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import os
 import shutil
 from abc import ABC, abstractmethod
 from importlib import resources
 from pathlib import Path
+from typing import Tuple
 
 from jinja2 import Template
 
 
 class ProjectGenerator(ABC):
     @abstractmethod
-    def template_directory(self) -> str:
+    def template_path_info(self) -> Tuple[str, str]:
         """
         Returns the package-relative path to the templates directory for this project type.
         """
         pass
 
     @abstractmethod
     def context(self) -> dict:
@@ -25,19 +26,19 @@
     def generate_project(self, destination_path: str):
         """
         Generate the project by rendering all Jinja templates found within the specified template directory.
         """
         # Ensure the destination directory exists
         os.makedirs(destination_path, exist_ok=True)
 
-        template_dir = self.template_directory()
+        template_dir, template_name = self.template_path_info()
         render_context = self.context()
 
         # Access the directory of the specified template
-        with resources.path(template_dir, "") as template_dir_path:
+        with resources.path(template_dir, template_name) as template_dir_path:
             for root, dirs, files in os.walk(template_dir_path):
                 relative_root = Path(root).relative_to(template_dir_path)
                 destination_dir = Path(destination_path, relative_root)
 
                 # Create directories in the destination path
                 os.makedirs(destination_dir, exist_ok=True)
 
@@ -48,19 +49,21 @@
                     if file == "__pycache__":
                         continue
 
                     if file.endswith(".jinja"):
                         # Render Jinja template
                         if relative_root.name:
                             template_content = resources.read_text(
-                                f"{template_dir}.{'.'.join(relative_root.parts)}",
+                                f"{template_dir}.{template_name}.{'.'.join(relative_root.parts)}",
                                 file,
                             )
                         else:
-                            template_content = resources.read_text(template_dir, file)
+                            template_content = resources.read_text(
+                                f"{template_dir}.{template_name}", file
+                            )
                         template = Template(template_content)
                         output_content = template.render(render_context) + "\n"
 
                         # Save the rendered file, removing the '.jinja' extension
                         destination_file_path = destination_file_path.with_suffix("")
 
                         with open(destination_file_path, "w") as f:
```

### Comparing `launchflow-0.3.9.dev8/launchflow/cli/gen/templates/django/__pycache__/django_template.cpython-311.pyc` & `launchflow-0.4.0.dev0/launchflow/cli/gen/templates/flask/__pycache__/flask_template.cpython-311.pyc`

 * *Files 14% similar despite different names*

#### Python bytecode

```diff
@@ -1,813 +1,802 @@
 magic:    0xa70d0d0a
-moddate:  0x05430f66 (Fri Apr  5 00:17:09 2024 UTC)
-files sz: 14570
+moddate:  0x972d4666 (Thu May 16 16:00:23 2024 UTC)
+files sz: 18651
 code
    argcount  : 0
    nlocals   : 0
-   stacksize : 21
+   stacksize : 24
    flags     : 0
    code
-      0x9700640064016c005a00640064016c015a01640064026c026d035a0301
-      00640064036c046d055a056d065a066d075a076d085a080100640064046c
-      096d0a5a0a0100640064056c0b6d0c5a0c0100640064066c0d6d0e5a0e01
-      00640064076c0f6d105a100100640064086c116d125a120100640064096c
-      136d145a1401006400640a6c156d165a1601006400640b6c176d185a1801
-      00650302004700640c8400640da6020000ab020000000000000000a60000
-      00ab0000000000000000005a196512640e640f6410641164126413641464
-      156701640164169c096516641764186419641a6412641364146415670164
-      0164169c096514641b641c641d641e641f6420642164226701642364169c
-      096510642464256426642764016401640164286701640164169c09650c64
-      29642a642b641f642c642d642e642f6701642364309c09650a6431642564
-      32640164276401640164286701640164309c0969065a1a64336508651819
-      000000000000000000643465196604643584045a1b650302004700643684
-      006437650ea6030000ab030000000000000000a6000000ab000000000000
-      0000005a1c651d64386b0200000000723064395a1e0200651c6512651465
-      106703651e651e9b00643a9d02643b643cac3da6050000ab050000000000
-      0000005a1f651fa020000000000000000000000000000000000000000064
-      3eac3fa6010000ab01000000000000000001006401530064015300
+      0x9700640064016c005a00640064026c016d025a020100640064036c036d
+      045a046d055a056d065a066d075a070100640064046c086d095a09010064
+      0064056c0a6d0b5a0b0100640064066c0c6d0d5a0d0100640064076c0e6d
+      0f5a0f0100640064086c106d115a110100640064096c126d135a13010064
+      00640a6c146d155a1501006400640b6c166d175a1701006400640c6c186d
+      195a190100650202004700640d8400640ea6020000ab0200000000000000
+      00a6000000ab0000000000000000005a1a6515640f641064116412640164
+      016413670064146415670164169c0a651964176418641964126401640164
+      1a6700641b6415670164169c0a6517641c641d641e641264016401641f67
+      006420670064169c0a651364216422642364126401640164246425670264
+      266427642864296702642a9c0a650f642b642c642d641264016401642e67
+      00642f670064169c0a650b64306431643264126401640164336700641b64
+      15670164169c0a650d643464226435641264016401642464256702642664
+      27642864296702642a9c0a69075a1b643665076509190000000000000000
+      006437651a6604643884045a1c65020200470064398400643a6511a60300
+      00ab030000000000000000a6000000ab0000000000000000005a1d640153
+      00
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (None)
-                 6 IMPORT_NAME              0 (datetime)
-                 8 STORE_NAME               0 (datetime)
+                 6 IMPORT_NAME              0 (sys)
+                 8 STORE_NAME               0 (sys)
    
      2          10 LOAD_CONST               0 (0)
-                12 LOAD_CONST               1 (None)
-                14 IMPORT_NAME              1 (sys)
-                16 STORE_NAME               1 (sys)
+                12 LOAD_CONST               2 (('dataclass',))
+                14 IMPORT_NAME              1 (dataclasses)
+                16 IMPORT_FROM              2 (dataclass)
+                18 STORE_NAME               2 (dataclass)
+                20 POP_TOP
    
-     3          18 LOAD_CONST               0 (0)
-                20 LOAD_CONST               2 (('dataclass',))
-                22 IMPORT_NAME              2 (dataclasses)
-                24 IMPORT_FROM              3 (dataclass)
-                26 STORE_NAME               3 (dataclass)
-                28 POP_TOP
+     3          22 LOAD_CONST               0 (0)
+                24 LOAD_CONST               3 (('List', 'Literal', 'Optional', 'Type'))
+                26 IMPORT_NAME              3 (typing)
+                28 IMPORT_FROM              4 (List)
+                30 STORE_NAME               4 (List)
+                32 IMPORT_FROM              5 (Literal)
+                34 STORE_NAME               5 (Literal)
+                36 IMPORT_FROM              6 (Optional)
+                38 STORE_NAME               6 (Optional)
+                40 IMPORT_FROM              7 (Type)
+                42 STORE_NAME               7 (Type)
+                44 POP_TOP
    
-     4          30 LOAD_CONST               0 (0)
-                32 LOAD_CONST               3 (('List', 'Literal', 'Optional', 'Type'))
-                34 IMPORT_NAME              4 (typing)
-                36 IMPORT_FROM              5 (List)
-                38 STORE_NAME               5 (List)
-                40 IMPORT_FROM              6 (Literal)
-                42 STORE_NAME               6 (Literal)
-                44 IMPORT_FROM              7 (Optional)
-                46 STORE_NAME               7 (Optional)
-                48 IMPORT_FROM              8 (Type)
-                50 STORE_NAME               8 (Type)
-                52 POP_TOP
+     5          46 LOAD_CONST               0 (0)
+                48 LOAD_CONST               4 (('Resource',))
+                50 IMPORT_NAME              8 (launchflow)
+                52 IMPORT_FROM              9 (Resource)
+                54 STORE_NAME               9 (Resource)
+                56 POP_TOP
    
-     6          54 LOAD_CONST               0 (0)
-                56 LOAD_CONST               4 (('RDSPostgres',))
-                58 IMPORT_NAME              9 (launchflow.aws.rds)
-                60 IMPORT_FROM             10 (RDSPostgres)
-                62 STORE_NAME              10 (RDSPostgres)
-                64 POP_TOP
+     6          58 LOAD_CONST               0 (0)
+                60 LOAD_CONST               5 (('ElasticacheRedis',))
+                62 IMPORT_NAME             10 (launchflow.aws.elasticache)
+                64 IMPORT_FROM             11 (ElasticacheRedis)
+                66 STORE_NAME              11 (ElasticacheRedis)
+                68 POP_TOP
    
-     7          66 LOAD_CONST               0 (0)
-                68 LOAD_CONST               5 (('S3Bucket',))
-                70 IMPORT_NAME             11 (launchflow.aws.s3)
-                72 IMPORT_FROM             12 (S3Bucket)
-                74 STORE_NAME              12 (S3Bucket)
-                76 POP_TOP
+     7          70 LOAD_CONST               0 (0)
+                72 LOAD_CONST               6 (('RDSPostgres',))
+                74 IMPORT_NAME             12 (launchflow.aws.rds)
+                76 IMPORT_FROM             13 (RDSPostgres)
+                78 STORE_NAME              13 (RDSPostgres)
+                80 POP_TOP
    
-     8          78 LOAD_CONST               0 (0)
-                80 LOAD_CONST               6 (('ProjectGenerator',))
-                82 IMPORT_NAME             13 (launchflow.cli.gen.template)
-                84 IMPORT_FROM             14 (ProjectGenerator)
-                86 STORE_NAME              14 (ProjectGenerator)
-                88 POP_TOP
+     8          82 LOAD_CONST               0 (0)
+                84 LOAD_CONST               7 (('S3Bucket',))
+                86 IMPORT_NAME             14 (launchflow.aws.s3)
+                88 IMPORT_FROM             15 (S3Bucket)
+                90 STORE_NAME              15 (S3Bucket)
+                92 POP_TOP
    
-     9          90 LOAD_CONST               0 (0)
-                92 LOAD_CONST               7 (('CloudSQLPostgres',))
-                94 IMPORT_NAME             15 (launchflow.gcp.cloudsql)
-                96 IMPORT_FROM             16 (CloudSQLPostgres)
-                98 STORE_NAME              16 (CloudSQLPostgres)
-               100 POP_TOP
+     9          94 LOAD_CONST               0 (0)
+                96 LOAD_CONST               8 (('ProjectGenerator',))
+                98 IMPORT_NAME             16 (launchflow.cli.gen.template)
+               100 IMPORT_FROM             17 (ProjectGenerator)
+               102 STORE_NAME              17 (ProjectGenerator)
+               104 POP_TOP
    
-    10         102 LOAD_CONST               0 (0)
-               104 LOAD_CONST               8 (('ComputeEngineRedis',))
-               106 IMPORT_NAME             17 (launchflow.gcp.compute_engine)
-               108 IMPORT_FROM             18 (ComputeEngineRedis)
-               110 STORE_NAME              18 (ComputeEngineRedis)
-               112 POP_TOP
+    10         106 LOAD_CONST               0 (0)
+               108 LOAD_CONST               9 (('CloudSQLPostgres',))
+               110 IMPORT_NAME             18 (launchflow.gcp.cloudsql)
+               112 IMPORT_FROM             19 (CloudSQLPostgres)
+               114 STORE_NAME              19 (CloudSQLPostgres)
+               116 POP_TOP
    
-    11         114 LOAD_CONST               0 (0)
-               116 LOAD_CONST               9 (('GCSBucket',))
-               118 IMPORT_NAME             19 (launchflow.gcp.gcs)
-               120 IMPORT_FROM             20 (GCSBucket)
-               122 STORE_NAME              20 (GCSBucket)
-               124 POP_TOP
+    11         118 LOAD_CONST               0 (0)
+               120 LOAD_CONST              10 (('ComputeEngineRedis',))
+               122 IMPORT_NAME             20 (launchflow.gcp.compute_engine)
+               124 IMPORT_FROM             21 (ComputeEngineRedis)
+               126 STORE_NAME              21 (ComputeEngineRedis)
+               128 POP_TOP
    
-    12         126 LOAD_CONST               0 (0)
-               128 LOAD_CONST              10 (('MemorystoreRedis',))
-               130 IMPORT_NAME             21 (launchflow.gcp.memorystore)
-               132 IMPORT_FROM             22 (MemorystoreRedis)
-               134 STORE_NAME              22 (MemorystoreRedis)
-               136 POP_TOP
+    12         130 LOAD_CONST               0 (0)
+               132 LOAD_CONST              11 (('GCSBucket',))
+               134 IMPORT_NAME             22 (launchflow.gcp.gcs)
+               136 IMPORT_FROM             23 (GCSBucket)
+               138 STORE_NAME              23 (GCSBucket)
+               140 POP_TOP
    
-    14         138 LOAD_CONST               0 (0)
-               140 LOAD_CONST              11 (('Resource',))
-               142 IMPORT_NAME             23 (launchflow)
-               144 IMPORT_FROM             24 (Resource)
-               146 STORE_NAME              24 (Resource)
-               148 POP_TOP
+    13         142 LOAD_CONST               0 (0)
+               144 LOAD_CONST              12 (('MemorystoreRedis',))
+               146 IMPORT_NAME             24 (launchflow.gcp.memorystore)
+               148 IMPORT_FROM             25 (MemorystoreRedis)
+               150 STORE_NAME              25 (MemorystoreRedis)
+               152 POP_TOP
    
-    17         150 LOAD_NAME                3 (dataclass)
+    16         154 LOAD_NAME                2 (dataclass)
    
-    18         152 PUSH_NULL
-               154 LOAD_BUILD_CLASS
-               156 LOAD_CONST              12 (<code object ResourceInfo, file "/home/tanke/launchflow/launchflow/clients/python/launchflow/launchflow/cli/gen/templates/django/django_template.py", line 17>)
-               158 MAKE_FUNCTION            0
-               160 LOAD_CONST              13 ('ResourceInfo')
-               162 PRECALL                  2
-               166 CALL                     2
+    17         156 PUSH_NULL
+               158 LOAD_BUILD_CLASS
+               160 LOAD_CONST              13 (<code object ResourceInfo, file "/Users/calebvandyke/code/launchflow-oss/launchflow/cli/gen/templates/flask/flask_template.py", line 16>)
+               162 MAKE_FUNCTION            0
+               164 LOAD_CONST              14 ('ResourceInfo')
+               166 PRECALL                  2
+               170 CALL                     2
    
-    17         176 PRECALL                  0
-               180 CALL                     0
+    16         180 PRECALL                  0
+               184 CALL                     0
    
-    18         190 STORE_NAME              25 (ResourceInfo)
+    17         194 STORE_NAME              26 (ResourceInfo)
    
-    32         192 LOAD_NAME               18 (ComputeEngineRedis)
+    32         196 LOAD_NAME               21 (ComputeEngineRedis)
    
-    33         194 LOAD_CONST              14 ('https://docs.launchflow.com/reference/gcp-resources/compute-engine')
+    33         198 LOAD_CONST              15 ('https://docs.launchflow.com/reference/gcp-resources/compute-engine#compute-engine-redis')
    
-    34         196 LOAD_CONST              15 ('redis_vm')
+    34         200 LOAD_CONST              16 ('redis_vm')
    
-    35         198 LOAD_CONST              16 ('lf.gcp.ComputeEngineRedis')
+    35         202 LOAD_CONST              17 ('lf.gcp.ComputeEngineRedis')
    
-    36         200 LOAD_CONST              17 ('CACHES = {\n    "default": redis_vm.django_settings(),\n}\n')
+    36         204 LOAD_CONST              18 ('')
    
-    40         202 LOAD_CONST              18 ('from django.core.cache import cache')
+    37         206 LOAD_CONST               1 (None)
    
-    41         204 LOAD_CONST              19 ('\n# NOTE: This should normally use a POST request since it\'s modifying state, but we\'re\n# using GET so you can easily test it in your browser.\n@api_view(["GET"])\ndef test_redis(request, key):\n    # Write to cache (Redis)\n    cache.set(key, "Hello from Redis!", timeout=60)\n    # Immediately read from cache to verify write\n    return Response({"message": cache.get(key)})\n')
+    38         208 LOAD_CONST               1 (None)
    
-    51         206 LOAD_CONST              20 ('path("test_redis/<key>", views.test_redis),')
+    39         210 LOAD_CONST              19 ('# Connect to the Redis instance\nredis_client = redis_vm.redis()\n')
    
-    52         208 LOAD_CONST              21 ('redis>=4.2.0')
-               210 BUILD_LIST               1
+    40         212 BUILD_LIST               0
    
-    53         212 LOAD_CONST               1 (None)
+    41         214 LOAD_CONST              20 ('\n# NOTE: This should normally use a POST request since it\'s modifying state, but we\'re\n# using GET so you can easily test it in your browser.\n@app.get("/test_redis/<key>")\ndef test_redis(key: str):\n    value = request.json["value"]\n    # Write to Redis\n    redis_client.set(key, value)\n    # Immediately read from Redis to verify the write\n    value = redis_client.get(key)\n    return jsonify({"message": f"Set {key} to {value}"})\n')
    
-    32         214 LOAD_CONST              22 (('infra_docs_url', 'infra_name', 'infra_lf_class', 'django_settings', 'views_imports', 'django_test_endpoint', 'django_test_endpoint_url', 'requirements', 'installed_app'))
-               216 BUILD_CONST_KEY_MAP      9
+    53         216 LOAD_CONST              21 ('redis>=4.2.0')
+               218 BUILD_LIST               1
    
-    56         218 LOAD_NAME               22 (MemorystoreRedis)
+    32         220 LOAD_CONST              22 (('infra_docs_url', 'infra_name', 'infra_lf_class', 'launchflow_imports', 'infra_import', 'global_setup', 'infra_setup', 'app_imports', 'flask_test_endpoint', 'requirements'))
+               222 BUILD_CONST_KEY_MAP     10
    
-    57         220 LOAD_CONST              23 ('https://docs.launchflow.com/reference/gcp-resources/memorystore-redis')
+    56         224 LOAD_NAME               25 (MemorystoreRedis)
    
-    58         222 LOAD_CONST              24 ('redis_cluster')
+    57         226 LOAD_CONST              23 ('https://docs.launchflow.com/reference/gcp-resources/memorystore')
    
-    59         224 LOAD_CONST              25 ('lf.gcp.MemorystoreRedis')
+    58         228 LOAD_CONST              24 ('memorystore')
    
-    60         226 LOAD_CONST              26 ('CACHES = {\n    "default": redis_cluster.django_settings(),\n}\n')
+    59         230 LOAD_CONST              25 ('lf.gcp.MemorystoreRedis')
    
-    64         228 LOAD_CONST              18 ('from django.core.cache import cache')
+    60         232 LOAD_CONST              18 ('')
    
-    65         230 LOAD_CONST              19 ('\n# NOTE: This should normally use a POST request since it\'s modifying state, but we\'re\n# using GET so you can easily test it in your browser.\n@api_view(["GET"])\ndef test_redis(request, key):\n    # Write to cache (Redis)\n    cache.set(key, "Hello from Redis!", timeout=60)\n    # Immediately read from cache to verify write\n    return Response({"message": cache.get(key)})\n')
+    61         234 LOAD_CONST               1 (None)
    
-    75         232 LOAD_CONST              20 ('path("test_redis/<key>", views.test_redis),')
+    62         236 LOAD_CONST               1 (None)
    
-    76         234 LOAD_CONST              21 ('redis>=4.2.0')
-               236 BUILD_LIST               1
+    63         238 LOAD_CONST              26 ('# Connect to the Redis instance\nredis_client = memorystore.redis()\n')
    
-    77         238 LOAD_CONST               1 (None)
+    64         240 BUILD_LIST               0
    
-    56         240 LOAD_CONST              22 (('infra_docs_url', 'infra_name', 'infra_lf_class', 'django_settings', 'views_imports', 'django_test_endpoint', 'django_test_endpoint_url', 'requirements', 'installed_app'))
-               242 BUILD_CONST_KEY_MAP      9
+    65         242 LOAD_CONST              27 ('\n# NOTE: This should normally use a POST request since it\'s modifying state, but we\'re\n# using GET so you can easily test it in your browser.\n@app.get("/test_redis/<key>")\ndef test_redis(key: str):\n    # Write to Redis\n    value = request.json["value"]\n    redis_client.set(key, value)\n    # Immediately read from Redis to verify the write\n    value = redis_client.get(key)\n    return jsonify({"message": f"Set {key} to {value}"})\n')
    
-    80         244 LOAD_NAME               20 (GCSBucket)
+    77         244 LOAD_CONST              21 ('redis>=4.2.0')
+               246 BUILD_LIST               1
    
-    81         246 LOAD_CONST              27 ('https://docs.launchflow.com/reference/gcp-resources/gcs-bucket')
+    56         248 LOAD_CONST              22 (('infra_docs_url', 'infra_name', 'infra_lf_class', 'launchflow_imports', 'infra_import', 'global_setup', 'infra_setup', 'app_imports', 'flask_test_endpoint', 'requirements'))
+               250 BUILD_CONST_KEY_MAP     10
    
-    82         248 LOAD_CONST              28 ('gcs_bucket')
+    80         252 LOAD_NAME               23 (GCSBucket)
    
-    83         250 LOAD_CONST              29 ('lf.gcp.GCSBucket')
+    81         254 LOAD_CONST              28 ('https://docs.launchflow.com/reference/gcp-resources/gcs-bucket')
    
-    84         252 LOAD_CONST              30 ('STORAGES = {\n    "default": {\n        "BACKEND": "storages.backends.gcloud.GoogleCloudStorage",\n    },\n    "staticfiles": {\n        "BACKEND": "storages.backends.gcloud.GoogleCloudStorage",\n    },\n}\nGS_BUCKET_NAME = gcs_bucket.connect().bucket_name\nGS_CREDENTIALS = get_service_account_credentials()\n')
+    82         256 LOAD_CONST              29 ('gcs_bucket')
    
-    95         254 LOAD_CONST              31 ('from django.core.files.storage import default_storage')
+    83         258 LOAD_CONST              30 ('lf.gcp.GCSBucket')
    
-    96         256 LOAD_CONST              32 ('\n# NOTE: This should normally use a POST request since it\'s modifying state, but we\'re\n# using GET so you can easily test it in your browser.\n@api_view(["GET"])\ndef test_gcs(request, object_name):\n    # Write to GCS\n    with default_storage.open(object_name, "w") as file:\n        file.write("Hello from GCS!")\n    # Immediately read from GCS to verify write\n    with default_storage.open(object_name, "r") as file:\n        return Response({"message": file.read()})\n')
+    84         260 LOAD_CONST              18 ('')
    
-   108         258 LOAD_CONST              33 ('path("test_gcs/<object_name>", views.test_gcs),')
+    85         262 LOAD_CONST               1 (None)
    
-   109         260 LOAD_CONST              34 ('django-storages[google]')
-               262 BUILD_LIST               1
+    86         264 LOAD_CONST               1 (None)
    
-   110         264 LOAD_CONST              35 ('storages')
+    87         266 LOAD_CONST              31 ('# Connect to the storage Bucket\ngcs_bucket.connect()\n')
    
-    80         266 LOAD_CONST              22 (('infra_docs_url', 'infra_name', 'infra_lf_class', 'django_settings', 'views_imports', 'django_test_endpoint', 'django_test_endpoint_url', 'requirements', 'installed_app'))
-               268 BUILD_CONST_KEY_MAP      9
+    88         268 BUILD_LIST               0
    
-   113         270 LOAD_NAME               16 (CloudSQLPostgres)
+    89         270 LOAD_CONST              32 ('\n# NOTE: This should normally use a POST request since it\'s modifying state, but we\'re\n# using GET so you can easily test it in your browser.\n@app.get("/test_gcs/<object_name>")\ndef test_gcs(object_name: str):\n    # Write to GCS\n    gcs_bucket.upload_from_string("Hello, World!", object_name)\n    # Immediately read from GCS to verify the write\n    gcs_bucket.download_file(object_name).decode("utf-8")\n    return jsonify({"message": f"Uploaded {object_name} to GCS"})\n')
    
-   114         272 LOAD_CONST              36 ('https://docs.launchflow.com/reference/gcp-resources/cloud-sql')
+   100         272 BUILD_LIST               0
    
-   115         274 LOAD_CONST              37 ('postgres')
+    80         274 LOAD_CONST              22 (('infra_docs_url', 'infra_name', 'infra_lf_class', 'launchflow_imports', 'infra_import', 'global_setup', 'infra_setup', 'app_imports', 'flask_test_endpoint', 'requirements'))
+               276 BUILD_CONST_KEY_MAP     10
    
-   116         276 LOAD_CONST              38 ('lf.gcp.CloudSQLPostgres')
+   103         278 LOAD_NAME               19 (CloudSQLPostgres)
    
-   117         278 LOAD_CONST              39 ('DATABASES = {\n    "default": postgres.django_settings(),\n}\n')
+   104         280 LOAD_CONST              33 ('https://docs.launchflow.com/reference/gcp-resources/cloud-sql')
    
-   121         280 LOAD_CONST               1 (None)
+   105         282 LOAD_CONST              34 ('postgres')
    
-   122         282 LOAD_CONST               1 (None)
+   106         284 LOAD_CONST              35 ('lf.gcp.CloudSQLPostgres')
    
-   123         284 LOAD_CONST               1 (None)
+   107         286 LOAD_CONST              18 ('')
    
-   124         286 LOAD_CONST              40 ('psycopg2-binary')
-               288 BUILD_LIST               1
+   108         288 LOAD_CONST               1 (None)
    
-   125         290 LOAD_CONST               1 (None)
+   109         290 LOAD_CONST               1 (None)
    
-   113         292 LOAD_CONST              22 (('infra_docs_url', 'infra_name', 'infra_lf_class', 'django_settings', 'views_imports', 'django_test_endpoint', 'django_test_endpoint_url', 'requirements', 'installed_app'))
-               294 BUILD_CONST_KEY_MAP      9
+   111         292 LOAD_CONST              36 ('from app.models import Base, StorageUser')
    
-   128         296 LOAD_NAME               12 (S3Bucket)
+   112         294 LOAD_CONST              37 ('from app.schemas import ListUsersResponse, UserResponse')
    
-   129         298 LOAD_CONST              41 ('https://docs.launchflow.com/reference/aws-resources/s3-bucket')
+   110         296 BUILD_LIST               2
    
-   130         300 LOAD_CONST              42 ('s3_bucket')
+   114         298 LOAD_CONST              38 ('# Configure the Postgres database with Flask-SQLAlchemy\ndb = SQLAlchemy(\n    app,\n    model_class=Base,\n    engine_options=postgres.sqlalchemy_engine_options(),\n)\n\nwith app.app_context():\n    db.create_all()')
    
-   131         302 LOAD_CONST              43 ('lf.aws.S3Bucket')
+   123         300 LOAD_CONST              39 ('\n"""\nThe endpoints below define a simple CRUD API for a generic StorageUser model.\n\nThe StorageUser model is defined in app.models\nThe ListUsersResponse and UserResponse schemas are defined in app.schemas.\n"""\n\n\n@app.get("/users")\ndef list_users():\n    storage_users = db.session.execute(select(StorageUser)).scalars().all()\n    return jsonify(\n        ListUsersResponse.from_storage(storage_users).model_dump(mode="json")\n    )\n\n\n@app.post("/users")\ndef create_user():\n    data = request.json\n    storage_user = StorageUser(email=data["email"], name=data["name"])\n    db.session.add(storage_user)\n    db.session.commit()\n    return jsonify(UserResponse.from_storage(storage_user).model_dump(mode="json"))\n\n\n@app.get("/users/<int:user_id>")\ndef read_user(user_id: int):\n    storage_user = db.session.get(StorageUser, user_id)\n    if storage_user is None:\n        abort(404, "User not found")\n    return jsonify(UserResponse.from_storage(storage_user).model_dump(mode="json"))\n\n\n@app.put("/users/<int:user_id>")\ndef update_user(user_id: int):\n    storage_user = db.session.get(StorageUser, user_id)\n    if storage_user is None:\n        abort(404, "User not found")\n    data = request.json\n    storage_user.name = data["name"]\n    db.session.commit()\n    return jsonify(UserResponse.from_storage(storage_user).model_dump(mode="json"))\n\n\n@app.delete("/users/<int:user_id>")\ndef delete_user(user_id):\n    storage_user = db.session.get(StorageUser, user_id)\n    if storage_user is None:\n        abort(404, "User not found")\n    db.session.delete(storage_user)\n    db.session.commit()\n    return jsonify(UserResponse.from_storage(storage_user).model_dump(mode="json"))\n')
    
-   132         304 LOAD_CONST              31 ('from django.core.files.storage import default_storage')
+   177         302 LOAD_CONST              40 ('Flask-SQLAlchemy')
+               304 LOAD_CONST              41 ('pg8000')
+               306 BUILD_LIST               2
    
-   133         306 LOAD_CONST              44 ('STORAGES = {\n    "default": {\n        "BACKEND": "storages.backends.s3.S3Storage",\n    },\n    "staticfiles": {\n        "BACKEND": "storages.backends.s3.S3Storage",\n    },\n}\nAWS_STORAGE_BUCKET_NAME = s3_bucket.connect().bucket_name\n')
+   103         308 LOAD_CONST              42 (('infra_docs_url', 'infra_name', 'infra_lf_class', 'launchflow_imports', 'infra_import', 'global_setup', 'app_imports', 'infra_setup', 'flask_test_endpoint', 'requirements'))
+               310 BUILD_CONST_KEY_MAP     10
    
-   143         308 LOAD_CONST              45 ('\n# NOTE: This should normally use a POST request since it\'s modifying state, but we\'re\n# using GET so you can easily test it in your browser.\n@api_view(["GET"])\ndef test_s3(request, object_name):\n    # Write to S3\n    with default_storage.open(object_name, "w") as file:\n        file.write("Hello from S3!")\n    # Immediately read from S3 to verify write\n    with default_storage.open(object_name, "r") as file:\n        return Response({"message": file.read()})\n')
+   180         312 LOAD_NAME               15 (S3Bucket)
    
-   155         310 LOAD_CONST              46 ('path("test_s3/<object_name>", views.test_s3),')
+   181         314 LOAD_CONST              43 ('https://docs.launchflow.com/reference/aws-resources/s3-bucket')
    
-   156         312 LOAD_CONST              47 ('django-storages[s3]')
-               314 BUILD_LIST               1
+   182         316 LOAD_CONST              44 ('s3_bucket')
    
-   157         316 LOAD_CONST              35 ('storages')
+   183         318 LOAD_CONST              45 ('lf.aws.S3Bucket')
    
-   128         318 LOAD_CONST              48 (('infra_docs_url', 'infra_name', 'infra_lf_class', 'views_imports', 'django_settings', 'django_test_endpoint', 'django_test_endpoint_url', 'requirements', 'installed_app'))
-               320 BUILD_CONST_KEY_MAP      9
+   184         320 LOAD_CONST              18 ('')
    
-   160         322 LOAD_NAME               10 (RDSPostgres)
+   185         322 LOAD_CONST               1 (None)
    
-   161         324 LOAD_CONST              49 ('https://docs.launchflow.com/reference/aws-resources/rds')
+   186         324 LOAD_CONST               1 (None)
    
-   162         326 LOAD_CONST              37 ('postgres')
+   187         326 LOAD_CONST              46 ('# Connect to the storage Bucket\ns3_bucket.connect()\n')
    
-   163         328 LOAD_CONST              50 ('lf.aws.RDSPostgres')
+   188         328 BUILD_LIST               0
    
-   164         330 LOAD_CONST               1 (None)
+   189         330 LOAD_CONST              47 ('\n# NOTE: This should normally use a POST request since it\'s modifying state, but we\'re\n# using GET so you can easily test it in your browser.\n@app.get("/test_s3/<object_name>")\ndef test_s3(object_name: str):\n    # Write to S3\n    s3_bucket.upload_from_string("Hello, World!", object_name)\n    # Immediately read from S3 to verify the write\n    s3_bucket.download_file(object_name).decode("utf-8")\n    return jsonify({"message": f"Uploaded {object_name} to S3"})\n')
    
-   165         332 LOAD_CONST              39 ('DATABASES = {\n    "default": postgres.django_settings(),\n}\n')
+   200         332 BUILD_LIST               0
    
-   169         334 LOAD_CONST               1 (None)
+   180         334 LOAD_CONST              22 (('infra_docs_url', 'infra_name', 'infra_lf_class', 'launchflow_imports', 'infra_import', 'global_setup', 'infra_setup', 'app_imports', 'flask_test_endpoint', 'requirements'))
+               336 BUILD_CONST_KEY_MAP     10
    
-   170         336 LOAD_CONST               1 (None)
+   203         338 LOAD_NAME               11 (ElasticacheRedis)
    
-   171         338 LOAD_CONST              40 ('psycopg2-binary')
-               340 BUILD_LIST               1
+   204         340 LOAD_CONST              48 ('https://docs.launchflow.com/reference/aws-resources/elasticache-redis')
    
-   172         342 LOAD_CONST               1 (None)
+   205         342 LOAD_CONST              49 ('elasticache')
    
-   160         344 LOAD_CONST              48 (('infra_docs_url', 'infra_name', 'infra_lf_class', 'views_imports', 'django_settings', 'django_test_endpoint', 'django_test_endpoint_url', 'requirements', 'installed_app'))
-               346 BUILD_CONST_KEY_MAP      9
+   206         344 LOAD_CONST              50 ('lf.aws.ElasticacheRedis')
    
-    30         348 BUILD_MAP                6
-               350 STORE_NAME              26 (resource_type_to_resource_info_kwargs)
+   207         346 LOAD_CONST              18 ('')
    
-   177         352 LOAD_CONST              51 ('resource')
-               354 LOAD_NAME                8 (Type)
-               356 LOAD_NAME               24 (Resource)
-               358 BINARY_SUBSCR
-               368 LOAD_CONST              52 ('return')
-               370 LOAD_NAME               25 (ResourceInfo)
-               372 BUILD_TUPLE              4
-               374 LOAD_CONST              53 (<code object get_resource_info, file "/home/tanke/launchflow/launchflow/clients/python/launchflow/launchflow/cli/gen/templates/django/django_template.py", line 177>)
-               376 MAKE_FUNCTION            4 (annotations)
-               378 STORE_NAME              27 (get_resource_info)
+   208         348 LOAD_CONST               1 (None)
    
-   186         380 LOAD_NAME                3 (dataclass)
+   209         350 LOAD_CONST               1 (None)
    
-   187         382 PUSH_NULL
-               384 LOAD_BUILD_CLASS
-               386 LOAD_CONST              54 (<code object DjangoProjectGenerator, file "/home/tanke/launchflow/launchflow/clients/python/launchflow/launchflow/cli/gen/templates/django/django_template.py", line 186>)
-               388 MAKE_FUNCTION            0
-               390 LOAD_CONST              55 ('DjangoProjectGenerator')
-               392 LOAD_NAME               14 (ProjectGenerator)
-               394 PRECALL                  3
-               398 CALL                     3
+   210         352 LOAD_CONST              51 ('# Connect to the Redis instance\nredis_client = elasticache.redis()\n')
    
-   186         408 PRECALL                  0
-               412 CALL                     0
+   211         354 BUILD_LIST               0
    
-   187         422 STORE_NAME              28 (DjangoProjectGenerator)
+   212         356 LOAD_CONST              27 ('\n# NOTE: This should normally use a POST request since it\'s modifying state, but we\'re\n# using GET so you can easily test it in your browser.\n@app.get("/test_redis/<key>")\ndef test_redis(key: str):\n    # Write to Redis\n    value = request.json["value"]\n    redis_client.set(key, value)\n    # Immediately read from Redis to verify the write\n    value = redis_client.get(key)\n    return jsonify({"message": f"Set {key} to {value}"})\n')
    
-   385         424 LOAD_NAME               29 (__name__)
-               426 LOAD_CONST              56 ('__main__')
-               428 COMPARE_OP               2 (==)
-               434 POP_JUMP_FORWARD_IF_FALSE    48 (to 532)
+   224         358 LOAD_CONST              21 ('redis>=4.2.0')
+               360 BUILD_LIST               1
    
-   386         436 LOAD_CONST              57 ('gcp')
-               438 STORE_NAME              30 (cloud_provider)
+   203         362 LOAD_CONST              22 (('infra_docs_url', 'infra_name', 'infra_lf_class', 'launchflow_imports', 'infra_import', 'global_setup', 'infra_setup', 'app_imports', 'flask_test_endpoint', 'requirements'))
+               364 BUILD_CONST_KEY_MAP     10
    
-   387         440 PUSH_NULL
-               442 LOAD_NAME               28 (DjangoProjectGenerator)
+   227         366 LOAD_NAME               13 (RDSPostgres)
    
-   389         444 LOAD_NAME               18 (ComputeEngineRedis)
+   228         368 LOAD_CONST              52 ('https://docs.launchflow.com/reference/aws-resources/rds-postgres')
    
-   390         446 LOAD_NAME               20 (GCSBucket)
+   229         370 LOAD_CONST              34 ('postgres')
    
-   391         448 LOAD_NAME               16 (CloudSQLPostgres)
+   230         372 LOAD_CONST              53 ('lf.aws.RDSPostgres')
    
-   388         450 BUILD_LIST               3
+   231         374 LOAD_CONST              18 ('')
    
-   395         452 LOAD_NAME               30 (cloud_provider)
+   232         376 LOAD_CONST               1 (None)
    
-   396         454 LOAD_NAME               30 (cloud_provider)
-               456 FORMAT_VALUE             0
-               458 LOAD_CONST              58 ('-examples')
-               460 BUILD_STRING             2
+   233         378 LOAD_CONST               1 (None)
    
-   397         462 LOAD_CONST              59 ('dev')
+   235         380 LOAD_CONST              36 ('from app.models import Base, StorageUser')
    
-   398         464 LOAD_CONST              60 ('django-service')
+   236         382 LOAD_CONST              37 ('from app.schemas import ListUsersResponse, UserResponse')
    
-   387         466 KW_NAMES                61
-               468 PRECALL                  5
-               472 CALL                     5
-               482 STORE_NAME              31 (generator)
+   234         384 BUILD_LIST               2
    
-   400         484 LOAD_NAME               31 (generator)
-               486 LOAD_METHOD             32 (generate_project)
-               508 LOAD_CONST              62 ('/tmp/launchflow')
-               510 KW_NAMES                63
-               512 PRECALL                  1
-               516 CALL                     1
-               526 POP_TOP
-               528 LOAD_CONST               1 (None)
-               530 RETURN_VALUE
+   238         386 LOAD_CONST              38 ('# Configure the Postgres database with Flask-SQLAlchemy\ndb = SQLAlchemy(\n    app,\n    model_class=Base,\n    engine_options=postgres.sqlalchemy_engine_options(),\n)\n\nwith app.app_context():\n    db.create_all()')
    
-   385     >>  532 LOAD_CONST               1 (None)
-               534 RETURN_VALUE
+   247         388 LOAD_CONST              39 ('\n"""\nThe endpoints below define a simple CRUD API for a generic StorageUser model.\n\nThe StorageUser model is defined in app.models\nThe ListUsersResponse and UserResponse schemas are defined in app.schemas.\n"""\n\n\n@app.get("/users")\ndef list_users():\n    storage_users = db.session.execute(select(StorageUser)).scalars().all()\n    return jsonify(\n        ListUsersResponse.from_storage(storage_users).model_dump(mode="json")\n    )\n\n\n@app.post("/users")\ndef create_user():\n    data = request.json\n    storage_user = StorageUser(email=data["email"], name=data["name"])\n    db.session.add(storage_user)\n    db.session.commit()\n    return jsonify(UserResponse.from_storage(storage_user).model_dump(mode="json"))\n\n\n@app.get("/users/<int:user_id>")\ndef read_user(user_id: int):\n    storage_user = db.session.get(StorageUser, user_id)\n    if storage_user is None:\n        abort(404, "User not found")\n    return jsonify(UserResponse.from_storage(storage_user).model_dump(mode="json"))\n\n\n@app.put("/users/<int:user_id>")\ndef update_user(user_id: int):\n    storage_user = db.session.get(StorageUser, user_id)\n    if storage_user is None:\n        abort(404, "User not found")\n    data = request.json\n    storage_user.name = data["name"]\n    db.session.commit()\n    return jsonify(UserResponse.from_storage(storage_user).model_dump(mode="json"))\n\n\n@app.delete("/users/<int:user_id>")\ndef delete_user(user_id):\n    storage_user = db.session.get(StorageUser, user_id)\n    if storage_user is None:\n        abort(404, "User not found")\n    db.session.delete(storage_user)\n    db.session.commit()\n    return jsonify(UserResponse.from_storage(storage_user).model_dump(mode="json"))\n')
+   
+   301         390 LOAD_CONST              40 ('Flask-SQLAlchemy')
+               392 LOAD_CONST              41 ('pg8000')
+               394 BUILD_LIST               2
+   
+   227         396 LOAD_CONST              42 (('infra_docs_url', 'infra_name', 'infra_lf_class', 'launchflow_imports', 'infra_import', 'global_setup', 'app_imports', 'infra_setup', 'flask_test_endpoint', 'requirements'))
+               398 BUILD_CONST_KEY_MAP     10
+   
+    30         400 BUILD_MAP                7
+               402 STORE_NAME              27 (resource_type_to_resource_info_kwargs)
+   
+   306         404 LOAD_CONST              54 ('resource')
+               406 LOAD_NAME                7 (Type)
+               408 LOAD_NAME                9 (Resource)
+               410 BINARY_SUBSCR
+               420 LOAD_CONST              55 ('return')
+               422 LOAD_NAME               26 (ResourceInfo)
+               424 BUILD_TUPLE              4
+               426 LOAD_CONST              56 (<code object get_resource_info, file "/Users/calebvandyke/code/launchflow-oss/launchflow/cli/gen/templates/flask/flask_template.py", line 306>)
+               428 MAKE_FUNCTION            4 (annotations)
+               430 STORE_NAME              28 (get_resource_info)
+   
+   315         432 LOAD_NAME                2 (dataclass)
+   
+   316         434 PUSH_NULL
+               436 LOAD_BUILD_CLASS
+               438 LOAD_CONST              57 (<code object FlaskProjectGenerator, file "/Users/calebvandyke/code/launchflow-oss/launchflow/cli/gen/templates/flask/flask_template.py", line 315>)
+               440 MAKE_FUNCTION            0
+               442 LOAD_CONST              58 ('FlaskProjectGenerator')
+               444 LOAD_NAME               17 (ProjectGenerator)
+               446 PRECALL                  3
+               450 CALL                     3
+   
+   315         460 PRECALL                  0
+               464 CALL                     0
+   
+   316         474 STORE_NAME              29 (FlaskProjectGenerator)
+               476 LOAD_CONST               1 (None)
+               478 RETURN_VALUE
    consts
       0
       None
       ('dataclass',)
       ('List', 'Literal', 'Optional', 'Type')
+      ('Resource',)
+      ('ElasticacheRedis',)
       ('RDSPostgres',)
       ('S3Bucket',)
       ('ProjectGenerator',)
       ('CloudSQLPostgres',)
       ('ComputeEngineRedis',)
       ('GCSBucket',)
       ('MemorystoreRedis',)
-      ('Resource',)
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 3
          flags     : 0
          code
             0x970065005a0164005a0255006503650464013c0000006503650464023c
-            0000006503650464033c0000006505650319000000000000000000650464
-            043c0000006505650319000000000000000000650464053c000000650565
-            0319000000000000000000650464063c0000006505650319000000000000
-            000000650464073c0000006506650319000000000000000000650464083c
-            0000006505650319000000000000000000650464093c000000640a5300
-          17           0 RESUME                   0
+            0000006503650464033c0000006503650464043c00000065056503190000
+            00000000000000650464053c000000650565031900000000000000000065
+            0464063c0000006505650319000000000000000000650464073c00000065
+            06650319000000000000000000650464083c0000006503650464093c0000
+            0065066503190000000000000000006504640a3c000000640b5300
+          16           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('ResourceInfo')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
-          19          12 LOAD_NAME                3 (str)
+          18          12 LOAD_NAME                3 (str)
                       14 LOAD_NAME                4 (__annotations__)
                       16 LOAD_CONST               1 ('infra_docs_url')
                       18 STORE_SUBSCR
          
-          20          22 LOAD_NAME                3 (str)
+          19          22 LOAD_NAME                3 (str)
                       24 LOAD_NAME                4 (__annotations__)
                       26 LOAD_CONST               2 ('infra_name')
                       28 STORE_SUBSCR
          
-          21          32 LOAD_NAME                3 (str)
+          20          32 LOAD_NAME                3 (str)
                       34 LOAD_NAME                4 (__annotations__)
                       36 LOAD_CONST               3 ('infra_lf_class')
                       38 STORE_SUBSCR
          
-          22          42 LOAD_NAME                5 (Optional)
-                      44 LOAD_NAME                3 (str)
-                      46 BINARY_SUBSCR
-                      56 LOAD_NAME                4 (__annotations__)
-                      58 LOAD_CONST               4 ('django_settings')
-                      60 STORE_SUBSCR
-         
-          23          64 LOAD_NAME                5 (Optional)
-                      66 LOAD_NAME                3 (str)
-                      68 BINARY_SUBSCR
-                      78 LOAD_NAME                4 (__annotations__)
-                      80 LOAD_CONST               5 ('views_imports')
-                      82 STORE_SUBSCR
-         
-          24          86 LOAD_NAME                5 (Optional)
-                      88 LOAD_NAME                3 (str)
-                      90 BINARY_SUBSCR
-                     100 LOAD_NAME                4 (__annotations__)
-                     102 LOAD_CONST               6 ('django_test_endpoint')
-                     104 STORE_SUBSCR
-         
-          25         108 LOAD_NAME                5 (Optional)
-                     110 LOAD_NAME                3 (str)
-                     112 BINARY_SUBSCR
-                     122 LOAD_NAME                4 (__annotations__)
-                     124 LOAD_CONST               7 ('django_test_endpoint_url')
-                     126 STORE_SUBSCR
-         
-          26         130 LOAD_NAME                6 (List)
-                     132 LOAD_NAME                3 (str)
-                     134 BINARY_SUBSCR
-                     144 LOAD_NAME                4 (__annotations__)
-                     146 LOAD_CONST               8 ('requirements')
-                     148 STORE_SUBSCR
-         
-          27         152 LOAD_NAME                5 (Optional)
-                     154 LOAD_NAME                3 (str)
-                     156 BINARY_SUBSCR
-                     166 LOAD_NAME                4 (__annotations__)
-                     168 LOAD_CONST               9 ('installed_app')
-                     170 STORE_SUBSCR
-                     174 LOAD_CONST              10 (None)
-                     176 RETURN_VALUE
+          21          42 LOAD_NAME                3 (str)
+                      44 LOAD_NAME                4 (__annotations__)
+                      46 LOAD_CONST               4 ('launchflow_imports')
+                      48 STORE_SUBSCR
+         
+          22          52 LOAD_NAME                5 (Optional)
+                      54 LOAD_NAME                3 (str)
+                      56 BINARY_SUBSCR
+                      66 LOAD_NAME                4 (__annotations__)
+                      68 LOAD_CONST               5 ('infra_import')
+                      70 STORE_SUBSCR
+         
+          23          74 LOAD_NAME                5 (Optional)
+                      76 LOAD_NAME                3 (str)
+                      78 BINARY_SUBSCR
+                      88 LOAD_NAME                4 (__annotations__)
+                      90 LOAD_CONST               6 ('global_setup')
+                      92 STORE_SUBSCR
+         
+          24          96 LOAD_NAME                5 (Optional)
+                      98 LOAD_NAME                3 (str)
+                     100 BINARY_SUBSCR
+                     110 LOAD_NAME                4 (__annotations__)
+                     112 LOAD_CONST               7 ('infra_setup')
+                     114 STORE_SUBSCR
+         
+          25         118 LOAD_NAME                6 (List)
+                     120 LOAD_NAME                3 (str)
+                     122 BINARY_SUBSCR
+                     132 LOAD_NAME                4 (__annotations__)
+                     134 LOAD_CONST               8 ('app_imports')
+                     136 STORE_SUBSCR
+         
+          26         140 LOAD_NAME                3 (str)
+                     142 LOAD_NAME                4 (__annotations__)
+                     144 LOAD_CONST               9 ('flask_test_endpoint')
+                     146 STORE_SUBSCR
+         
+          27         150 LOAD_NAME                6 (List)
+                     152 LOAD_NAME                3 (str)
+                     154 BINARY_SUBSCR
+                     164 LOAD_NAME                4 (__annotations__)
+                     166 LOAD_CONST              10 ('requirements')
+                     168 STORE_SUBSCR
+                     172 LOAD_CONST              11 (None)
+                     174 RETURN_VALUE
          consts
             'ResourceInfo'
             'infra_docs_url'
             'infra_name'
             'infra_lf_class'
-            'django_settings'
-            'views_imports'
-            'django_test_endpoint'
-            'django_test_endpoint_url'
+            'launchflow_imports'
+            'infra_import'
+            'global_setup'
+            'infra_setup'
+            'app_imports'
+            'flask_test_endpoint'
             'requirements'
-            'installed_app'
             None
          names      ('__name__', '__module__', '__qualname__', 'str', '__annotations__', 'Optional', 'List')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/home/tanke/launchflow/launchflow/clients/python/launchflow/launchflow/cli/gen/templates/django/django_template.py'
+         filename   '/Users/calebvandyke/code/launchflow-oss/launchflow/cli/gen/templates/flask/flask_template.py'
          name       'ResourceInfo'
-         firstlineno 17
-         lnotab 0x0c020a010a010a0116011601160116011601
+         firstlineno 16
+         lnotab 0x0c020a010a010a010a0116011601160116010a01
       'ResourceInfo'
-      'https://docs.launchflow.com/reference/gcp-resources/compute-engine'
+      'https://docs.launchflow.com/reference/gcp-resources/compute-engine#compute-engine-redis'
       'redis_vm'
       'lf.gcp.ComputeEngineRedis'
-      'CACHES = {\n    "default": redis_vm.django_settings(),\n}\n'
-      'from django.core.cache import cache'
-      '\n# NOTE: This should normally use a POST request since it\'s modifying state, but we\'re\n# using GET so you can easily test it in your browser.\n@api_view(["GET"])\ndef test_redis(request, key):\n    # Write to cache (Redis)\n    cache.set(key, "Hello from Redis!", timeout=60)\n    # Immediately read from cache to verify write\n    return Response({"message": cache.get(key)})\n'
-      'path("test_redis/<key>", views.test_redis),'
+      ''
+      '# Connect to the Redis instance\nredis_client = redis_vm.redis()\n'
+      '\n# NOTE: This should normally use a POST request since it\'s modifying state, but we\'re\n# using GET so you can easily test it in your browser.\n@app.get("/test_redis/<key>")\ndef test_redis(key: str):\n    value = request.json["value"]\n    # Write to Redis\n    redis_client.set(key, value)\n    # Immediately read from Redis to verify the write\n    value = redis_client.get(key)\n    return jsonify({"message": f"Set {key} to {value}"})\n'
       'redis>=4.2.0'
-      ('infra_docs_url', 'infra_name', 'infra_lf_class', 'django_settings', 'views_imports', 'django_test_endpoint', 'django_test_endpoint_url', 'requirements', 'installed_app')
-      'https://docs.launchflow.com/reference/gcp-resources/memorystore-redis'
-      'redis_cluster'
+      ('infra_docs_url', 'infra_name', 'infra_lf_class', 'launchflow_imports', 'infra_import', 'global_setup', 'infra_setup', 'app_imports', 'flask_test_endpoint', 'requirements')
+      'https://docs.launchflow.com/reference/gcp-resources/memorystore'
+      'memorystore'
       'lf.gcp.MemorystoreRedis'
-      'CACHES = {\n    "default": redis_cluster.django_settings(),\n}\n'
+      '# Connect to the Redis instance\nredis_client = memorystore.redis()\n'
+      '\n# NOTE: This should normally use a POST request since it\'s modifying state, but we\'re\n# using GET so you can easily test it in your browser.\n@app.get("/test_redis/<key>")\ndef test_redis(key: str):\n    # Write to Redis\n    value = request.json["value"]\n    redis_client.set(key, value)\n    # Immediately read from Redis to verify the write\n    value = redis_client.get(key)\n    return jsonify({"message": f"Set {key} to {value}"})\n'
       'https://docs.launchflow.com/reference/gcp-resources/gcs-bucket'
       'gcs_bucket'
       'lf.gcp.GCSBucket'
-      'STORAGES = {\n    "default": {\n        "BACKEND": "storages.backends.gcloud.GoogleCloudStorage",\n    },\n    "staticfiles": {\n        "BACKEND": "storages.backends.gcloud.GoogleCloudStorage",\n    },\n}\nGS_BUCKET_NAME = gcs_bucket.connect().bucket_name\nGS_CREDENTIALS = get_service_account_credentials()\n'
-      'from django.core.files.storage import default_storage'
-      '\n# NOTE: This should normally use a POST request since it\'s modifying state, but we\'re\n# using GET so you can easily test it in your browser.\n@api_view(["GET"])\ndef test_gcs(request, object_name):\n    # Write to GCS\n    with default_storage.open(object_name, "w") as file:\n        file.write("Hello from GCS!")\n    # Immediately read from GCS to verify write\n    with default_storage.open(object_name, "r") as file:\n        return Response({"message": file.read()})\n'
-      'path("test_gcs/<object_name>", views.test_gcs),'
-      'django-storages[google]'
-      'storages'
+      '# Connect to the storage Bucket\ngcs_bucket.connect()\n'
+      '\n# NOTE: This should normally use a POST request since it\'s modifying state, but we\'re\n# using GET so you can easily test it in your browser.\n@app.get("/test_gcs/<object_name>")\ndef test_gcs(object_name: str):\n    # Write to GCS\n    gcs_bucket.upload_from_string("Hello, World!", object_name)\n    # Immediately read from GCS to verify the write\n    gcs_bucket.download_file(object_name).decode("utf-8")\n    return jsonify({"message": f"Uploaded {object_name} to GCS"})\n'
       'https://docs.launchflow.com/reference/gcp-resources/cloud-sql'
       'postgres'
       'lf.gcp.CloudSQLPostgres'
-      'DATABASES = {\n    "default": postgres.django_settings(),\n}\n'
-      'psycopg2-binary'
+      'from app.models import Base, StorageUser'
+      'from app.schemas import ListUsersResponse, UserResponse'
+      '# Configure the Postgres database with Flask-SQLAlchemy\ndb = SQLAlchemy(\n    app,\n    model_class=Base,\n    engine_options=postgres.sqlalchemy_engine_options(),\n)\n\nwith app.app_context():\n    db.create_all()'
+      '\n"""\nThe endpoints below define a simple CRUD API for a generic StorageUser model.\n\nThe StorageUser model is defined in app.models\nThe ListUsersResponse and UserResponse schemas are defined in app.schemas.\n"""\n\n\n@app.get("/users")\ndef list_users():\n    storage_users = db.session.execute(select(StorageUser)).scalars().all()\n    return jsonify(\n        ListUsersResponse.from_storage(storage_users).model_dump(mode="json")\n    )\n\n\n@app.post("/users")\ndef create_user():\n    data = request.json\n    storage_user = StorageUser(email=data["email"], name=data["name"])\n    db.session.add(storage_user)\n    db.session.commit()\n    return jsonify(UserResponse.from_storage(storage_user).model_dump(mode="json"))\n\n\n@app.get("/users/<int:user_id>")\ndef read_user(user_id: int):\n    storage_user = db.session.get(StorageUser, user_id)\n    if storage_user is None:\n        abort(404, "User not found")\n    return jsonify(UserResponse.from_storage(storage_user).model_dump(mode="json"))\n\n\n@app.put("/users/<int:user_id>")\ndef update_user(user_id: int):\n    storage_user = db.session.get(StorageUser, user_id)\n    if storage_user is None:\n        abort(404, "User not found")\n    data = request.json\n    storage_user.name = data["name"]\n    db.session.commit()\n    return jsonify(UserResponse.from_storage(storage_user).model_dump(mode="json"))\n\n\n@app.delete("/users/<int:user_id>")\ndef delete_user(user_id):\n    storage_user = db.session.get(StorageUser, user_id)\n    if storage_user is None:\n        abort(404, "User not found")\n    db.session.delete(storage_user)\n    db.session.commit()\n    return jsonify(UserResponse.from_storage(storage_user).model_dump(mode="json"))\n'
+      'Flask-SQLAlchemy'
+      'pg8000'
+      ('infra_docs_url', 'infra_name', 'infra_lf_class', 'launchflow_imports', 'infra_import', 'global_setup', 'app_imports', 'infra_setup', 'flask_test_endpoint', 'requirements')
       'https://docs.launchflow.com/reference/aws-resources/s3-bucket'
       's3_bucket'
       'lf.aws.S3Bucket'
-      'STORAGES = {\n    "default": {\n        "BACKEND": "storages.backends.s3.S3Storage",\n    },\n    "staticfiles": {\n        "BACKEND": "storages.backends.s3.S3Storage",\n    },\n}\nAWS_STORAGE_BUCKET_NAME = s3_bucket.connect().bucket_name\n'
-      '\n# NOTE: This should normally use a POST request since it\'s modifying state, but we\'re\n# using GET so you can easily test it in your browser.\n@api_view(["GET"])\ndef test_s3(request, object_name):\n    # Write to S3\n    with default_storage.open(object_name, "w") as file:\n        file.write("Hello from S3!")\n    # Immediately read from S3 to verify write\n    with default_storage.open(object_name, "r") as file:\n        return Response({"message": file.read()})\n'
-      'path("test_s3/<object_name>", views.test_s3),'
-      'django-storages[s3]'
-      ('infra_docs_url', 'infra_name', 'infra_lf_class', 'views_imports', 'django_settings', 'django_test_endpoint', 'django_test_endpoint_url', 'requirements', 'installed_app')
-      'https://docs.launchflow.com/reference/aws-resources/rds'
+      '# Connect to the storage Bucket\ns3_bucket.connect()\n'
+      '\n# NOTE: This should normally use a POST request since it\'s modifying state, but we\'re\n# using GET so you can easily test it in your browser.\n@app.get("/test_s3/<object_name>")\ndef test_s3(object_name: str):\n    # Write to S3\n    s3_bucket.upload_from_string("Hello, World!", object_name)\n    # Immediately read from S3 to verify the write\n    s3_bucket.download_file(object_name).decode("utf-8")\n    return jsonify({"message": f"Uploaded {object_name} to S3"})\n'
+      'https://docs.launchflow.com/reference/aws-resources/elasticache-redis'
+      'elasticache'
+      'lf.aws.ElasticacheRedis'
+      '# Connect to the Redis instance\nredis_client = elasticache.redis()\n'
+      'https://docs.launchflow.com/reference/aws-resources/rds-postgres'
       'lf.aws.RDSPostgres'
       'resource'
       'return'
       code
          argcount  : 1
          nlocals   : 2
          stacksize : 5
          flags     : 3
          code
             0x9700740000000000000000000000a00100000000000000000000000000
             000000000000007c006400a6020000ab0200000000000000007d017c0180
             1274050000000000000000000064017c009b009d02a6010000ab01000000
             00000000008201740700000000000000000000640269007c01a4018e0153
             00
-         177           0 RESUME                   0
+         306           0 RESUME                   0
          
-         178           2 LOAD_GLOBAL              0 (resource_type_to_resource_info_kwargs)
+         307           2 LOAD_GLOBAL              0 (resource_type_to_resource_info_kwargs)
                       14 LOAD_METHOD              1 (get)
                       36 LOAD_FAST                0 (resource)
                       38 LOAD_CONST               0 (None)
                       40 PRECALL                  2
                       44 CALL                     2
                       54 STORE_FAST               1 (resource_info_kwargs)
          
-         179          56 LOAD_FAST                1 (resource_info_kwargs)
+         308          56 LOAD_FAST                1 (resource_info_kwargs)
                       58 POP_JUMP_FORWARD_IF_NOT_NONE    18 (to 96)
          
-         180          60 LOAD_GLOBAL              5 (NULL + ValueError)
+         309          60 LOAD_GLOBAL              5 (NULL + ValueError)
                       72 LOAD_CONST               1 ('Unsupported resource type: ')
                       74 LOAD_FAST                0 (resource)
                       76 FORMAT_VALUE             0
                       78 BUILD_STRING             2
                       80 PRECALL                  1
                       84 CALL                     1
                       94 RAISE_VARARGS            1
          
-         181     >>   96 LOAD_GLOBAL              7 (NULL + ResourceInfo)
+         310     >>   96 LOAD_GLOBAL              7 (NULL + ResourceInfo)
                      108 LOAD_CONST               2 (())
                      110 BUILD_MAP                0
          
-         182         112 LOAD_FAST                1 (resource_info_kwargs)
+         311         112 LOAD_FAST                1 (resource_info_kwargs)
          
-         181         114 DICT_MERGE               1
+         310         114 DICT_MERGE               1
                      116 CALL_FUNCTION_EX         1
                      118 RETURN_VALUE
          consts
             None
             'Unsupported resource type: '
             ()
          names      ('resource_type_to_resource_info_kwargs', 'get', 'ValueError', 'ResourceInfo')
          varnames   ('resource', 'resource_info_kwargs')
          freevars   ()
          cellvars   ()
-         filename   '/home/tanke/launchflow/launchflow/clients/python/launchflow/launchflow/cli/gen/templates/django/django_template.py'
+         filename   '/Users/calebvandyke/code/launchflow-oss/launchflow/cli/gen/templates/flask/flask_template.py'
          name       'get_resource_info'
-         firstlineno 177
+         firstlineno 306
          lnotab 0x0201360104012401100102ff
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 4
          flags     : 0
          code
             0x970065005a0164005a0255006503650465051900000000000000000019
             000000000000000000650664013c00000065076402190000000000000000
             00650664033c0000006508650664043c0000006508650664053c00000064
             065a096508650664073c000000650a6a0b00000000000000006a0c000000
             00000000005a0d650e650664083c000000650a6a0b00000000000000006a
             0f00000000000000005a10650e650664093c000000640a5a116512640b65
-            086602640c8404a6000000ab0000000000000000005a136512640b650365
-            08190000000000000000006602640d8404a6000000ab0000000000000000
-            005a146512640b65086602640e8404a6000000ab0000000000000000005a
-            156512640b65036508190000000000000000006602640f8404a6000000ab
-            0000000000000000005a166512640b650365081900000000000000000066
-            0264108404a6000000ab0000000000000000005a176512640b6503650819
-            000000000000000000660264118404a6000000ab0000000000000000005a
-            186512640b6503650819000000000000000000660264128404a6000000ab
-            0000000000000000005a196512640b650365081900000000000000000066
-            0264138404a6000000ab0000000000000000005a1a6512640b6508660264
-            148404a6000000ab0000000000000000005a1b640b65086602641584045a
-            1c6512640b6508660264168404a6000000ab0000000000000000005a1d64
-            0b651e6602641784045a1f64185300
-         186           0 RESUME                   0
+            086602640c8404a6000000ab0000000000000000005a136512640b650866
+            02640d8404a6000000ab0000000000000000005a146512640b6503650819
+            0000000000000000006602640e8404a6000000ab0000000000000000005a
+            156512640b65086602640f8404a6000000ab0000000000000000005a1665
+            12640b6503650819000000000000000000660264108404a6000000ab0000
+            000000000000005a176512640b6503650819000000000000000000660264
+            118404a6000000ab0000000000000000005a186512640b65036508190000
+            00000000000000660264128404a6000000ab0000000000000000005a1965
+            12640b6508660264138404a6000000ab0000000000000000005a1a640b65
+            086602641484045a1b6512640b6508660264158404a6000000ab00000000
+            00000000005a1c640b651d6602641684045a1e64175300
+         315           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
-                       6 LOAD_CONST               0 ('DjangoProjectGenerator')
+                       6 LOAD_CONST               0 ('FlaskProjectGenerator')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
-         188          12 LOAD_NAME                3 (List)
+         317          12 LOAD_NAME                3 (List)
                       14 LOAD_NAME                4 (Type)
                       16 LOAD_NAME                5 (Resource)
                       18 BINARY_SUBSCR
                       28 BINARY_SUBSCR
                       38 LOAD_NAME                6 (__annotations__)
                       40 LOAD_CONST               1 ('resources')
                       42 STORE_SUBSCR
          
-         190          46 LOAD_NAME                7 (Literal)
+         319          46 LOAD_NAME                7 (Literal)
                       48 LOAD_CONST               2 (('aws', 'gcp'))
                       50 BINARY_SUBSCR
                       60 LOAD_NAME                6 (__annotations__)
                       62 LOAD_CONST               3 ('cloud_provider')
                       64 STORE_SUBSCR
          
-         192          68 LOAD_NAME                8 (str)
+         321          68 LOAD_NAME                8 (str)
                       70 LOAD_NAME                6 (__annotations__)
                       72 LOAD_CONST               4 ('launchflow_project_name')
                       74 STORE_SUBSCR
          
-         193          78 LOAD_NAME                8 (str)
+         322          78 LOAD_NAME                8 (str)
                       80 LOAD_NAME                6 (__annotations__)
                       82 LOAD_CONST               5 ('launchflow_environment_name')
                       84 STORE_SUBSCR
          
-         194          88 LOAD_CONST               6 ('django-service')
+         323          88 LOAD_CONST               6 ('flask-service')
                       90 STORE_NAME               9 (launchflow_service_name)
                       92 LOAD_NAME                8 (str)
                       94 LOAD_NAME                6 (__annotations__)
                       96 LOAD_CONST               7 ('launchflow_service_name')
                       98 STORE_SUBSCR
          
-         196         102 LOAD_NAME               10 (sys)
+         325         102 LOAD_NAME               10 (sys)
                      104 LOAD_ATTR               11 (version_info)
                      114 LOAD_ATTR               12 (major)
                      124 STORE_NAME              13 (python_major_version)
                      126 LOAD_NAME               14 (int)
                      128 LOAD_NAME                6 (__annotations__)
                      130 LOAD_CONST               8 ('python_major_version')
                      132 STORE_SUBSCR
          
-         197         136 LOAD_NAME               10 (sys)
+         326         136 LOAD_NAME               10 (sys)
                      138 LOAD_ATTR               11 (version_info)
                      148 LOAD_ATTR               15 (minor)
                      158 STORE_NAME              16 (python_minor_version)
                      160 LOAD_NAME               14 (int)
                      162 LOAD_NAME                6 (__annotations__)
                      164 LOAD_CONST               9 ('python_minor_version')
                      166 STORE_SUBSCR
          
-         198         170 LOAD_CONST              10 (8080)
+         327         170 LOAD_CONST              10 (8080)
                      172 STORE_NAME              17 (port)
          
-         201         174 LOAD_NAME               18 (property)
+         330         174 LOAD_NAME               18 (property)
          
-         202         176 LOAD_CONST              11 ('return')
+         331         176 LOAD_CONST              11 ('return')
                      178 LOAD_NAME                8 (str)
                      180 BUILD_TUPLE              2
-                     182 LOAD_CONST              12 (<code object infra_dot_py, file "/home/tanke/launchflow/launchflow/clients/python/launchflow/launchflow/cli/gen/templates/django/django_template.py", line 201>)
+                     182 LOAD_CONST              12 (<code object infra_dot_py, file "/Users/calebvandyke/code/launchflow-oss/launchflow/cli/gen/templates/flask/flask_template.py", line 330>)
                      184 MAKE_FUNCTION            4 (annotations)
          
-         201         186 PRECALL                  0
+         330         186 PRECALL                  0
                      190 CALL                     0
          
-         202         200 STORE_NAME              19 (infra_dot_py)
+         331         200 STORE_NAME              19 (infra_dot_py)
          
-         248         202 LOAD_NAME               18 (property)
+         377         202 LOAD_NAME               18 (property)
          
-         249         204 LOAD_CONST              11 ('return')
-                     206 LOAD_NAME                3 (List)
-                     208 LOAD_NAME                8 (str)
-                     210 BINARY_SUBSCR
-                     220 BUILD_TUPLE              2
-                     222 LOAD_CONST              13 (<code object app_infra_imports, file "/home/tanke/launchflow/launchflow/clients/python/launchflow/launchflow/cli/gen/templates/django/django_template.py", line 248>)
-                     224 MAKE_FUNCTION            4 (annotations)
+         378         204 LOAD_CONST              11 ('return')
+                     206 LOAD_NAME                8 (str)
+                     208 BUILD_TUPLE              2
+                     210 LOAD_CONST              13 (<code object flask_imports, file "/Users/calebvandyke/code/launchflow-oss/launchflow/cli/gen/templates/flask/flask_template.py", line 377>)
+                     212 MAKE_FUNCTION            4 (annotations)
          
-         248         226 PRECALL                  0
-                     230 CALL                     0
+         377         214 PRECALL                  0
+                     218 CALL                     0
          
-         249         240 STORE_NAME              20 (app_infra_imports)
+         378         228 STORE_NAME              20 (flask_imports)
          
-         274         242 LOAD_NAME               18 (property)
+         390         230 LOAD_NAME               18 (property)
          
-         275         244 LOAD_CONST              11 ('return')
-                     246 LOAD_NAME                8 (str)
+         391         232 LOAD_CONST              11 ('return')
+                     234 LOAD_NAME                3 (List)
+                     236 LOAD_NAME                8 (str)
+                     238 BINARY_SUBSCR
                      248 BUILD_TUPLE              2
-                     250 LOAD_CONST              14 (<code object app_django_settings, file "/home/tanke/launchflow/launchflow/clients/python/launchflow/launchflow/cli/gen/templates/django/django_template.py", line 274>)
+                     250 LOAD_CONST              14 (<code object app_infra_imports, file "/Users/calebvandyke/code/launchflow-oss/launchflow/cli/gen/templates/flask/flask_template.py", line 390>)
                      252 MAKE_FUNCTION            4 (annotations)
          
-         274         254 PRECALL                  0
+         390         254 PRECALL                  0
                      258 CALL                     0
          
-         275         268 STORE_NAME              21 (app_django_settings)
+         391         268 STORE_NAME              21 (app_infra_imports)
          
-         284         270 LOAD_NAME               18 (property)
+         415         270 LOAD_NAME               18 (property)
          
-         285         272 LOAD_CONST              11 ('return')
-                     274 LOAD_NAME                3 (List)
-                     276 LOAD_NAME                8 (str)
-                     278 BINARY_SUBSCR
-                     288 BUILD_TUPLE              2
-                     290 LOAD_CONST              15 (<code object app_installed_apps, file "/home/tanke/launchflow/launchflow/clients/python/launchflow/launchflow/cli/gen/templates/django/django_template.py", line 284>)
-                     292 MAKE_FUNCTION            4 (annotations)
+         416         272 LOAD_CONST              11 ('return')
+                     274 LOAD_NAME                8 (str)
+                     276 BUILD_TUPLE              2
+                     278 LOAD_CONST              15 (<code object app_global_setup, file "/Users/calebvandyke/code/launchflow-oss/launchflow/cli/gen/templates/flask/flask_template.py", line 415>)
+                     280 MAKE_FUNCTION            4 (annotations)
          
-         284         294 PRECALL                  0
-                     298 CALL                     0
+         415         282 PRECALL                  0
+                     286 CALL                     0
          
-         285         308 STORE_NAME              22 (app_installed_apps)
+         416         296 STORE_NAME              22 (app_global_setup)
          
-         294         310 LOAD_NAME               18 (property)
+         425         298 LOAD_NAME               18 (property)
          
-         295         312 LOAD_CONST              11 ('return')
-                     314 LOAD_NAME                3 (List)
-                     316 LOAD_NAME                8 (str)
-                     318 BINARY_SUBSCR
-                     328 BUILD_TUPLE              2
-                     330 LOAD_CONST              16 (<code object app_infra_urls, file "/home/tanke/launchflow/launchflow/clients/python/launchflow/launchflow/cli/gen/templates/django/django_template.py", line 294>)
-                     332 MAKE_FUNCTION            4 (annotations)
+         426         300 LOAD_CONST              11 ('return')
+                     302 LOAD_NAME                3 (List)
+                     304 LOAD_NAME                8 (str)
+                     306 BINARY_SUBSCR
+                     316 BUILD_TUPLE              2
+                     318 LOAD_CONST              16 (<code object app_infra_setup, file "/Users/calebvandyke/code/launchflow-oss/launchflow/cli/gen/templates/flask/flask_template.py", line 425>)
+                     320 MAKE_FUNCTION            4 (annotations)
          
-         294         334 PRECALL                  0
-                     338 CALL                     0
+         425         322 PRECALL                  0
+                     326 CALL                     0
          
-         295         348 STORE_NAME              23 (app_infra_urls)
+         426         336 STORE_NAME              23 (app_infra_setup)
          
-         304         350 LOAD_NAME               18 (property)
+         435         338 LOAD_NAME               18 (property)
          
-         305         352 LOAD_CONST              11 ('return')
-                     354 LOAD_NAME                3 (List)
-                     356 LOAD_NAME                8 (str)
-                     358 BINARY_SUBSCR
-                     368 BUILD_TUPLE              2
-                     370 LOAD_CONST              17 (<code object app_views_imports, file "/home/tanke/launchflow/launchflow/clients/python/launchflow/launchflow/cli/gen/templates/django/django_template.py", line 304>)
-                     372 MAKE_FUNCTION            4 (annotations)
+         436         340 LOAD_CONST              11 ('return')
+                     342 LOAD_NAME                3 (List)
+                     344 LOAD_NAME                8 (str)
+                     346 BINARY_SUBSCR
+                     356 BUILD_TUPLE              2
+                     358 LOAD_CONST              17 (<code object app_infra_endpoints, file "/Users/calebvandyke/code/launchflow-oss/launchflow/cli/gen/templates/flask/flask_template.py", line 435>)
+                     360 MAKE_FUNCTION            4 (annotations)
          
-         304         374 PRECALL                  0
-                     378 CALL                     0
+         435         362 PRECALL                  0
+                     366 CALL                     0
          
-         305         388 STORE_NAME              24 (app_views_imports)
+         436         376 STORE_NAME              24 (app_infra_endpoints)
          
-         314         390 LOAD_NAME               18 (property)
+         444         378 LOAD_NAME               18 (property)
          
-         315         392 LOAD_CONST              11 ('return')
-                     394 LOAD_NAME                3 (List)
-                     396 LOAD_NAME                8 (str)
-                     398 BINARY_SUBSCR
-                     408 BUILD_TUPLE              2
-                     410 LOAD_CONST              18 (<code object app_infra_endpoints, file "/home/tanke/launchflow/launchflow/clients/python/launchflow/launchflow/cli/gen/templates/django/django_template.py", line 314>)
-                     412 MAKE_FUNCTION            4 (annotations)
+         445         380 LOAD_CONST              11 ('return')
+                     382 LOAD_NAME                3 (List)
+                     384 LOAD_NAME                8 (str)
+                     386 BINARY_SUBSCR
+                     396 BUILD_TUPLE              2
+                     398 LOAD_CONST              18 (<code object additional_requirements, file "/Users/calebvandyke/code/launchflow-oss/launchflow/cli/gen/templates/flask/flask_template.py", line 444>)
+                     400 MAKE_FUNCTION            4 (annotations)
          
-         314         414 PRECALL                  0
-                     418 CALL                     0
+         444         402 PRECALL                  0
+                     406 CALL                     0
          
-         315         428 STORE_NAME              25 (app_infra_endpoints)
+         445         416 STORE_NAME              25 (additional_requirements)
          
-         324         430 LOAD_NAME               18 (property)
+         453         418 LOAD_NAME               18 (property)
          
-         325         432 LOAD_CONST              11 ('return')
-                     434 LOAD_NAME                3 (List)
-                     436 LOAD_NAME                8 (str)
-                     438 BINARY_SUBSCR
-                     448 BUILD_TUPLE              2
-                     450 LOAD_CONST              19 (<code object additional_requirements, file "/home/tanke/launchflow/launchflow/clients/python/launchflow/launchflow/cli/gen/templates/django/django_template.py", line 324>)
-                     452 MAKE_FUNCTION            4 (annotations)
+         454         420 LOAD_CONST              11 ('return')
+                     422 LOAD_NAME                8 (str)
+                     424 BUILD_TUPLE              2
+                     426 LOAD_CONST              19 (<code object launchflow_service_product, file "/Users/calebvandyke/code/launchflow-oss/launchflow/cli/gen/templates/flask/flask_template.py", line 453>)
+                     428 MAKE_FUNCTION            4 (annotations)
          
-         324         454 PRECALL                  0
-                     458 CALL                     0
+         453         430 PRECALL                  0
+                     434 CALL                     0
          
-         325         468 STORE_NAME              26 (additional_requirements)
+         454         444 STORE_NAME              26 (launchflow_service_product)
          
-         333         470 LOAD_NAME               18 (property)
+         461         446 LOAD_CONST              11 ('return')
+                     448 LOAD_NAME                8 (str)
+                     450 BUILD_TUPLE              2
+                     452 LOAD_CONST              20 (<code object template_path_info, file "/Users/calebvandyke/code/launchflow-oss/launchflow/cli/gen/templates/flask/flask_template.py", line 461>)
+                     454 MAKE_FUNCTION            4 (annotations)
+                     456 STORE_NAME              27 (template_path_info)
          
-         334         472 LOAD_CONST              11 ('return')
-                     474 LOAD_NAME                8 (str)
-                     476 BUILD_TUPLE              2
-                     478 LOAD_CONST              20 (<code object launchflow_service_product, file "/home/tanke/launchflow/launchflow/clients/python/launchflow/launchflow/cli/gen/templates/django/django_template.py", line 333>)
-                     480 MAKE_FUNCTION            4 (annotations)
+         472         458 LOAD_NAME               18 (property)
          
-         333         482 PRECALL                  0
-                     486 CALL                     0
+         473         460 LOAD_CONST              11 ('return')
+                     462 LOAD_NAME                8 (str)
+                     464 BUILD_TUPLE              2
+                     466 LOAD_CONST              21 (<code object docker_repository_prefix, file "/Users/calebvandyke/code/launchflow-oss/launchflow/cli/gen/templates/flask/flask_template.py", line 472>)
+                     468 MAKE_FUNCTION            4 (annotations)
          
-         334         496 STORE_NAME              27 (launchflow_service_product)
+         472         470 PRECALL                  0
+                     474 CALL                     0
          
-         341         498 LOAD_CONST              11 ('return')
-                     500 LOAD_NAME                8 (str)
-                     502 BUILD_TUPLE              2
-                     504 LOAD_CONST              21 (<code object template_directory, file "/home/tanke/launchflow/launchflow/clients/python/launchflow/launchflow/cli/gen/templates/django/django_template.py", line 341>)
-                     506 MAKE_FUNCTION            4 (annotations)
-                     508 STORE_NAME              28 (template_directory)
+         473         484 STORE_NAME              28 (docker_repository_prefix)
          
-         348         510 LOAD_NAME               18 (property)
-         
-         349         512 LOAD_CONST              11 ('return')
-                     514 LOAD_NAME                8 (str)
-                     516 BUILD_TUPLE              2
-                     518 LOAD_CONST              22 (<code object docker_repository_prefix, file "/home/tanke/launchflow/launchflow/clients/python/launchflow/launchflow/cli/gen/templates/django/django_template.py", line 348>)
-                     520 MAKE_FUNCTION            4 (annotations)
-         
-         348         522 PRECALL                  0
-                     526 CALL                     0
-         
-         349         536 STORE_NAME              29 (docker_repository_prefix)
-         
-         354         538 LOAD_CONST              11 ('return')
-                     540 LOAD_NAME               30 (dict)
-                     542 BUILD_TUPLE              2
-                     544 LOAD_CONST              23 (<code object context, file "/home/tanke/launchflow/launchflow/clients/python/launchflow/launchflow/cli/gen/templates/django/django_template.py", line 354>)
-                     546 MAKE_FUNCTION            4 (annotations)
-                     548 STORE_NAME              31 (context)
-                     550 LOAD_CONST              24 (None)
-                     552 RETURN_VALUE
+         478         486 LOAD_CONST              11 ('return')
+                     488 LOAD_NAME               29 (dict)
+                     490 BUILD_TUPLE              2
+                     492 LOAD_CONST              22 (<code object context, file "/Users/calebvandyke/code/launchflow-oss/launchflow/cli/gen/templates/flask/flask_template.py", line 478>)
+                     494 MAKE_FUNCTION            4 (annotations)
+                     496 STORE_NAME              30 (context)
+                     498 LOAD_CONST              23 (None)
+                     500 RETURN_VALUE
          consts
-            'DjangoProjectGenerator'
+            'FlaskProjectGenerator'
             'resources'
             ('aws', 'gcp')
             'cloud_provider'
             'launchflow_project_name'
             'launchflow_environment_name'
-            'django-service'
+            'flask-service'
             'launchflow_service_name'
             'python_major_version'
             'python_minor_version'
             8080
             'return'
             code
                argcount  : 1
@@ -831,156 +820,156 @@
                   0a7c036a0800000000000000009b00640b7c036a0900000000000000009b
                   00640c7c036a0a00000000000000009b00640d7c006a0400000000000000
                   009b00640e7c036a090000000000000000a00b0000000000000000000000
                   000000000000000000640f640ea6020000ab0200000000000000009b0064
                   109d0ba6010000ab01000000000000000001008c64640ba00c0000000000
                   0000000000000000000000000000007c01a6010000ab0100000000000000
                   005300
-               201           0 RESUME                   0
+               330           0 RESUME                   0
                
-               204           2 LOAD_CONST               1 ('"""\nThis is the recommended place to define all launchflow Resources, but you are free to\ndefine them anywhere in your Python project.\n\nTo create find and create all resources in your current directory, run:\n    $ launchflow create\n        - or -\n    $ lf create\n"""')
+               333           2 LOAD_CONST               1 ('"""\nThis is the recommended place to define all launchflow Resources, but you are free to\ndefine them anywhere in your Python project.\n\nTo create find and create all resources in your current directory, run:\n    $ launchflow create\n        - or -\n    $ lf create\n"""')
                
-               203           4 BUILD_LIST               1
+               332           4 BUILD_LIST               1
                              6 STORE_FAST               1 (lines)
                
-               215           8 LOAD_GLOBAL              1 (NULL + len)
+               344           8 LOAD_GLOBAL              1 (NULL + len)
                             20 LOAD_FAST                0 (self)
                             22 LOAD_ATTR                1 (resources)
                             32 PRECALL                  1
                             36 CALL                     1
                             46 LOAD_CONST               2 (0)
                             48 COMPARE_OP               2 (==)
                             54 POP_JUMP_FORWARD_IF_FALSE   109 (to 274)
                
-               216          56 LOAD_FAST                0 (self)
+               345          56 LOAD_FAST                0 (self)
                             58 LOAD_ATTR                2 (cloud_provider)
                             68 LOAD_CONST               3 ('aws')
                             70 COMPARE_OP               2 (==)
                             76 POP_JUMP_FORWARD_IF_FALSE    32 (to 142)
                
-               217          78 LOAD_FAST                1 (lines)
+               346          78 LOAD_FAST                1 (lines)
                             80 LOAD_METHOD              3 (extend)
                
-               219         102 LOAD_CONST               4 ("\n# Uncomment the following line and run `launchflow create` to create an S3 bucket.\n# s3_bucket = lf.aws.S3Bucket('")
+               348         102 LOAD_CONST               4 ("\n# Uncomment the following line and run `launchflow create` to create an S3 bucket.\n# s3_bucket = lf.aws.S3Bucket('")
                
-               221         104 LOAD_FAST                0 (self)
+               350         104 LOAD_FAST                0 (self)
                            106 LOAD_ATTR                4 (launchflow_project_name)
                
-               219         116 FORMAT_VALUE             0
+               348         116 FORMAT_VALUE             0
                            118 LOAD_CONST               5 ("-bucket')\n")
                            120 BUILD_STRING             3
                
-               218         122 BUILD_LIST               1
+               347         122 BUILD_LIST               1
                
-               217         124 PRECALL                  1
+               346         124 PRECALL                  1
                            128 CALL                     1
                            138 POP_TOP
                            140 JUMP_FORWARD           194 (to 530)
                
-               225     >>  142 LOAD_FAST                0 (self)
+               354     >>  142 LOAD_FAST                0 (self)
                            144 LOAD_ATTR                2 (cloud_provider)
                            154 LOAD_CONST               6 ('gcp')
                            156 COMPARE_OP               2 (==)
                            162 POP_JUMP_FORWARD_IF_FALSE    32 (to 228)
                
-               226         164 LOAD_FAST                1 (lines)
+               355         164 LOAD_FAST                1 (lines)
                            166 LOAD_METHOD              3 (extend)
                
-               228         188 LOAD_CONST               7 ("\n# Uncomment the following line and run `launchflow create` to create a GCS bucket.\n# gcs_bucket = lf.gcp.GCSBucket('")
+               357         188 LOAD_CONST               7 ("\n# Uncomment the following line and run `launchflow create` to create a GCS bucket.\n# gcs_bucket = lf.gcp.GCSBucket('")
                
-               230         190 LOAD_FAST                0 (self)
+               359         190 LOAD_FAST                0 (self)
                            192 LOAD_ATTR                4 (launchflow_project_name)
                
-               228         202 FORMAT_VALUE             0
+               357         202 FORMAT_VALUE             0
                            204 LOAD_CONST               5 ("-bucket')\n")
                            206 BUILD_STRING             3
                
-               227         208 BUILD_LIST               1
+               356         208 BUILD_LIST               1
                
-               226         210 PRECALL                  1
+               355         210 PRECALL                  1
                            214 CALL                     1
                            224 POP_TOP
                            226 JUMP_FORWARD           151 (to 530)
                
-               235     >>  228 LOAD_GLOBAL             11 (NULL + ValueError)
+               364     >>  228 LOAD_GLOBAL             11 (NULL + ValueError)
                            240 LOAD_CONST               8 ('Unsupported cloud provider: ')
                            242 LOAD_FAST                0 (self)
                            244 LOAD_ATTR                2 (cloud_provider)
                            254 FORMAT_VALUE             0
                            256 BUILD_STRING             2
                            258 PRECALL                  1
                            262 CALL                     1
                            272 RAISE_VARARGS            1
                
-               237     >>  274 LOAD_FAST                1 (lines)
+               366     >>  274 LOAD_FAST                1 (lines)
                            276 LOAD_METHOD              6 (append)
                            298 LOAD_CONST               9 ('import launchflow as lf\n')
                            300 PRECALL                  1
                            304 CALL                     1
                            314 POP_TOP
                
-               238         316 LOAD_FAST                0 (self)
+               367         316 LOAD_FAST                0 (self)
                            318 LOAD_ATTR                1 (resources)
                            328 GET_ITER
                        >>  330 FOR_ITER                99 (to 530)
                            332 STORE_FAST               2 (resource)
                
-               239         334 LOAD_GLOBAL             15 (NULL + get_resource_info)
+               368         334 LOAD_GLOBAL             15 (NULL + get_resource_info)
                            346 LOAD_FAST                2 (resource)
                            348 PRECALL                  1
                            352 CALL                     1
                            362 STORE_FAST               3 (resource_info)
                
-               240         364 LOAD_FAST                1 (lines)
+               369         364 LOAD_FAST                1 (lines)
                            366 LOAD_METHOD              6 (append)
                
-               241         388 LOAD_CONST              10 ('\n# Docs: ')
+               370         388 LOAD_CONST              10 ('\n# Docs: ')
                
-               242         390 LOAD_FAST                3 (resource_info)
+               371         390 LOAD_FAST                3 (resource_info)
                            392 LOAD_ATTR                8 (infra_docs_url)
                
-               241         402 FORMAT_VALUE             0
+               370         402 FORMAT_VALUE             0
                            404 LOAD_CONST              11 ('\n')
                
-               243         406 LOAD_FAST                3 (resource_info)
+               372         406 LOAD_FAST                3 (resource_info)
                            408 LOAD_ATTR                9 (infra_name)
                
-               241         418 FORMAT_VALUE             0
+               370         418 FORMAT_VALUE             0
                            420 LOAD_CONST              12 (' = ')
                
-               243         422 LOAD_FAST                3 (resource_info)
+               372         422 LOAD_FAST                3 (resource_info)
                            424 LOAD_ATTR               10 (infra_lf_class)
                
-               241         434 FORMAT_VALUE             0
+               370         434 FORMAT_VALUE             0
                            436 LOAD_CONST              13 ("('")
                
-               243         438 LOAD_FAST                0 (self)
+               372         438 LOAD_FAST                0 (self)
                            440 LOAD_ATTR                4 (launchflow_project_name)
                
-               241         450 FORMAT_VALUE             0
+               370         450 FORMAT_VALUE             0
                            452 LOAD_CONST              14 ('-')
                
-               243         454 LOAD_FAST                3 (resource_info)
+               372         454 LOAD_FAST                3 (resource_info)
                            456 LOAD_ATTR                9 (infra_name)
                            466 LOAD_METHOD             11 (replace)
                            488 LOAD_CONST              15 ('_')
                            490 LOAD_CONST              14 ('-')
                            492 PRECALL                  2
                            496 CALL                     2
                
-               241         506 FORMAT_VALUE             0
+               370         506 FORMAT_VALUE             0
                            508 LOAD_CONST              16 ("')")
                            510 BUILD_STRING            11
                
-               240         512 PRECALL                  1
+               369         512 PRECALL                  1
                            516 CALL                     1
                            526 POP_TOP
                            528 JUMP_BACKWARD          100 (to 330)
                
-               245     >>  530 LOAD_CONST              11 ('\n')
+               374     >>  530 LOAD_CONST              11 ('\n')
                            532 LOAD_METHOD             12 (join)
                            554 LOAD_FAST                1 (lines)
                            556 PRECALL                  1
                            560 CALL                     1
                            570 RETURN_VALUE
                consts
                   None
@@ -1000,456 +989,463 @@
                   '-'
                   '_'
                   "')"
                names      ('len', 'resources', 'cloud_provider', 'extend', 'launchflow_project_name', 'ValueError', 'append', 'get_resource_info', 'infra_docs_url', 'infra_name', 'infra_lf_class', 'replace', 'join')
                varnames   ('self', 'lines', 'resource', 'resource_info')
                freevars   ()
                cellvars   ()
-               filename   '/home/tanke/launchflow/launchflow/clients/python/launchflow/launchflow/cli/gen/templates/django/django_template.py'
+               filename   '/Users/calebvandyke/code/launchflow-oss/launchflow/cli/gen/templates/flask/flask_template.py'
                name       'infra_dot_py'
-               firstlineno 201
+               firstlineno 330
                lnotab
                   0x020302ff040c30011601180202020cfe06ff02ff12081601180202020c
                   fe06ff02ff12092e022a0112011e01180102010cff04020cfe04020cfe04
                   020cfe040234fe06ff1205
             code
                argcount  : 1
-               nlocals   : 5
+               nlocals   : 2
+               stacksize : 3
+               flags     : 3
+               code
+                  0x97007401000000000000000000007c006a010000000000000000a60100
+                  00ab01000000000000000064016b02000000007202640253007405000000
+                  000000000000007c006a010000000000000000a6010000ab010000000000
+                  0000007d017406000000000000000000007c017600730974080000000000
+                  00000000007c01760072026403530064045300
+               377           0 RESUME                   0
+               
+               379           2 LOAD_GLOBAL              1 (NULL + len)
+                            14 LOAD_FAST                0 (self)
+                            16 LOAD_ATTR                1 (resources)
+                            26 PRECALL                  1
+                            30 CALL                     1
+                            40 LOAD_CONST               1 (0)
+                            42 COMPARE_OP               2 (==)
+                            48 POP_JUMP_FORWARD_IF_FALSE     2 (to 54)
+               
+               380          50 LOAD_CONST               2 ('from flask import Flask, jsonify')
+                            52 RETURN_VALUE
+               
+               381     >>   54 LOAD_GLOBAL              5 (NULL + set)
+                            66 LOAD_FAST                0 (self)
+                            68 LOAD_ATTR                1 (resources)
+                            78 PRECALL                  1
+                            82 CALL                     1
+                            92 STORE_FAST               1 (resource_set)
+               
+               382          94 LOAD_GLOBAL              6 (CloudSQLPostgres)
+                           106 LOAD_FAST                1 (resource_set)
+                           108 CONTAINS_OP              0
+                           110 POP_JUMP_FORWARD_IF_TRUE     9 (to 130)
+                           112 LOAD_GLOBAL              8 (RDSPostgres)
+                           124 LOAD_FAST                1 (resource_set)
+                           126 CONTAINS_OP              0
+                           128 POP_JUMP_FORWARD_IF_FALSE     2 (to 134)
+               
+               383     >>  130 LOAD_CONST               3 ('from flask import Flask, abort, jsonify, request\nfrom flask_sqlalchemy import SQLAlchemy\nfrom sqlalchemy import select')
+                           132 RETURN_VALUE
+               
+               387     >>  134 LOAD_CONST               4 ('from flask import Flask, jsonify, request')
+                           136 RETURN_VALUE
+               consts
+                  None
+                  0
+                  'from flask import Flask, jsonify'
+                  'from flask import Flask, abort, jsonify, request\nfrom flask_sqlalchemy import SQLAlchemy\nfrom sqlalchemy import select'
+                  'from flask import Flask, jsonify, request'
+               names      ('len', 'resources', 'set', 'CloudSQLPostgres', 'RDSPostgres')
+               varnames   ('self', 'resource_set')
+               freevars   ()
+               cellvars   ()
+               filename   '/Users/calebvandyke/code/launchflow-oss/launchflow/cli/gen/templates/flask/flask_template.py'
+               name       'flask_imports'
+               firstlineno 377
+               lnotab 0x020230010401280124010404
+            code
+               argcount  : 1
+               nlocals   : 8
                stacksize : 8
                flags     : 3
                code
                   0x97007401000000000000000000007c006a010000000000000000a60100
                   00ab01000000000000000064016b020000000072026700530067007d0167
-                  007d027c006a01000000000000000044005d4b7d037c0374040000000000
-                  00000000006b020000000072157c01a00300000000000000000000000000
-                  000000000000006402a6010000ab01000000000000000001007409000000
-                  000000000000007c03a6010000ab0100000000000000007d047c02a00300
-                  000000000000000000000000000000000000007c046a0500000000000000
-                  00a6010000ab01000000000000000001008c4c7401000000000000000000
-                  007c02a6010000ab01000000000000000064016b020000000072027c0153
-                  007c01a003000000000000000000000000000000000000000064036404a0
-                  060000000000000000000000000000000000000000740f00000000000000
-                  0000007c02a6010000ab010000000000000000a6010000ab010000000000
-                  0000009b009d02a6010000ab01000000000000000001007c015300
-               248           0 RESUME                   0
+                  007d0267007d0367007d04740500000000000000000000a6000000ab0000
+                  000000000000007d057c006a01000000000000000044005d807d06740700
+                  0000000000000000007c06a6010000ab0100000000000000007d077c03a0
+                  0400000000000000000000000000000000000000007c076a050000000000
+                  000000a6010000ab01000000000000000001007c05a00600000000000000
+                  000000000000000000000000007c076a070000000000000000a6010000ab
+                  01000000000000000001007c04a008000000000000000000000000000000
+                  00000000007c076a090000000000000000a6010000ab0100000000000000
+                  0001007c076a0a0000000000000000811a7c02a004000000000000000000
+                  00000000000000000000007c076a0a0000000000000000a6010000ab0100
+                  0000000000000001008c817c01a008000000000000000000000000000000
+                  00000000007417000000000000000000007c02a6010000ab010000000000
+                  000000a6010000ab01000000000000000001007c01a00800000000000000
+                  000000000000000000000000007417000000000000000000007c05a60100
+                  00ab010000000000000000a6010000ab01000000000000000001007c01a0
+                  04000000000000000000000000000000000000000064026403a00c000000
+                  00000000000000000000000000000000007417000000000000000000007c
+                  03a6010000ab010000000000000000a6010000ab0100000000000000009b
+                  009d02a6010000ab01000000000000000001007c01a00800000000000000
+                  000000000000000000000000007417000000000000000000007c04a60100
+                  00ab010000000000000000a6010000ab01000000000000000001007c0153
+                  00
+               390           0 RESUME                   0
                
-               252           2 LOAD_GLOBAL              1 (NULL + len)
+               394           2 LOAD_GLOBAL              1 (NULL + len)
                             14 LOAD_FAST                0 (self)
                             16 LOAD_ATTR                1 (resources)
                             26 PRECALL                  1
                             30 CALL                     1
                             40 LOAD_CONST               1 (0)
                             42 COMPARE_OP               2 (==)
                             48 POP_JUMP_FORWARD_IF_FALSE     2 (to 54)
                
-               253          50 BUILD_LIST               0
+               395          50 BUILD_LIST               0
                             52 RETURN_VALUE
                
-               254     >>   54 BUILD_LIST               0
+               396     >>   54 BUILD_LIST               0
                             56 STORE_FAST               1 (to_return)
                
-               255          58 BUILD_LIST               0
-                            60 STORE_FAST               2 (infra_names)
+               397          58 BUILD_LIST               0
+                            60 STORE_FAST               2 (client_imports)
                
-               257          62 LOAD_FAST                0 (self)
-                            64 LOAD_ATTR                1 (resources)
-                            74 GET_ITER
-                       >>   76 FOR_ITER                75 (to 228)
-                            78 STORE_FAST               3 (resource)
-               
-               258          80 LOAD_FAST                3 (resource)
-                            82 LOAD_GLOBAL              4 (GCSBucket)
-                            94 COMPARE_OP               2 (==)
-                           100 POP_JUMP_FORWARD_IF_FALSE    21 (to 144)
-               
-               259         102 LOAD_FAST                1 (to_return)
-                           104 LOAD_METHOD              3 (append)
-               
-               260         126 LOAD_CONST               2 ('from launchflow.gcp import get_service_account_credentials')
-               
-               259         128 PRECALL                  1
-                           132 CALL                     1
-                           142 POP_TOP
-               
-               262     >>  144 LOAD_GLOBAL              9 (NULL + get_resource_info)
-                           156 LOAD_FAST                3 (resource)
-                           158 PRECALL                  1
-                           162 CALL                     1
-                           172 STORE_FAST               4 (resource_info)
-               
-               263         174 LOAD_FAST                2 (infra_names)
-                           176 LOAD_METHOD              3 (append)
-                           198 LOAD_FAST                4 (resource_info)
-                           200 LOAD_ATTR                5 (infra_name)
-                           210 PRECALL                  1
-                           214 CALL                     1
-                           224 POP_TOP
-                           226 JUMP_BACKWARD           76 (to 76)
+               398          62 BUILD_LIST               0
+                            64 STORE_FAST               3 (infra_names)
                
-               265     >>  228 LOAD_GLOBAL              1 (NULL + len)
-                           240 LOAD_FAST                2 (infra_names)
-                           242 PRECALL                  1
-                           246 CALL                     1
-                           256 LOAD_CONST               1 (0)
-                           258 COMPARE_OP               2 (==)
-                           264 POP_JUMP_FORWARD_IF_FALSE     2 (to 270)
-               
-               266         266 LOAD_FAST                1 (to_return)
-                           268 RETURN_VALUE
-               
-               268     >>  270 LOAD_FAST                1 (to_return)
-                           272 LOAD_METHOD              3 (append)
-               
-               269         294 LOAD_CONST               3 ('from django_app.infra import ')
-                           296 LOAD_CONST               4 (', ')
-                           298 LOAD_METHOD              6 (join)
-                           320 LOAD_GLOBAL             15 (NULL + sorted)
-                           332 LOAD_FAST                2 (infra_names)
-                           334 PRECALL                  1
-                           338 CALL                     1
-                           348 PRECALL                  1
-                           352 CALL                     1
-                           362 FORMAT_VALUE             0
-                           364 BUILD_STRING             2
+               399          66 BUILD_LIST               0
+                            68 STORE_FAST               4 (app_imports)
                
-               268         366 PRECALL                  1
-                           370 CALL                     1
-                           380 POP_TOP
+               400          70 LOAD_GLOBAL              5 (NULL + set)
+                            82 PRECALL                  0
+                            86 CALL                     0
+                            96 STORE_FAST               5 (launchflow_imports)
+               
+               401          98 LOAD_FAST                0 (self)
+                           100 LOAD_ATTR                1 (resources)
+                           110 GET_ITER
+                       >>  112 FOR_ITER               128 (to 370)
+                           114 STORE_FAST               6 (resource)
+               
+               402         116 LOAD_GLOBAL              7 (NULL + get_resource_info)
+                           128 LOAD_FAST                6 (resource)
+                           130 PRECALL                  1
+                           134 CALL                     1
+                           144 STORE_FAST               7 (resource_info)
+               
+               403         146 LOAD_FAST                3 (infra_names)
+                           148 LOAD_METHOD              4 (append)
+                           170 LOAD_FAST                7 (resource_info)
+                           172 LOAD_ATTR                5 (infra_name)
+                           182 PRECALL                  1
+                           186 CALL                     1
+                           196 POP_TOP
+               
+               404         198 LOAD_FAST                5 (launchflow_imports)
+                           200 LOAD_METHOD              6 (add)
+                           222 LOAD_FAST                7 (resource_info)
+                           224 LOAD_ATTR                7 (launchflow_imports)
+                           234 PRECALL                  1
+                           238 CALL                     1
+                           248 POP_TOP
+               
+               405         250 LOAD_FAST                4 (app_imports)
+                           252 LOAD_METHOD              8 (extend)
+                           274 LOAD_FAST                7 (resource_info)
+                           276 LOAD_ATTR                9 (app_imports)
+                           286 PRECALL                  1
+                           290 CALL                     1
+                           300 POP_TOP
+               
+               406         302 LOAD_FAST                7 (resource_info)
+                           304 LOAD_ATTR               10 (infra_import)
+                           314 POP_JUMP_FORWARD_IF_NONE    26 (to 368)
+               
+               407         316 LOAD_FAST                2 (client_imports)
+                           318 LOAD_METHOD              4 (append)
+                           340 LOAD_FAST                7 (resource_info)
+                           342 LOAD_ATTR               10 (infra_import)
+                           352 PRECALL                  1
+                           356 CALL                     1
+                           366 POP_TOP
+                       >>  368 JUMP_BACKWARD          129 (to 112)
+               
+               408     >>  370 LOAD_FAST                1 (to_return)
+                           372 LOAD_METHOD              8 (extend)
+                           394 LOAD_GLOBAL             23 (NULL + sorted)
+                           406 LOAD_FAST                2 (client_imports)
+                           408 PRECALL                  1
+                           412 CALL                     1
+                           422 PRECALL                  1
+                           426 CALL                     1
+                           436 POP_TOP
+               
+               409         438 LOAD_FAST                1 (to_return)
+                           440 LOAD_METHOD              8 (extend)
+                           462 LOAD_GLOBAL             23 (NULL + sorted)
+                           474 LOAD_FAST                5 (launchflow_imports)
+                           476 PRECALL                  1
+                           480 CALL                     1
+                           490 PRECALL                  1
+                           494 CALL                     1
+                           504 POP_TOP
+               
+               410         506 LOAD_FAST                1 (to_return)
+                           508 LOAD_METHOD              4 (append)
+                           530 LOAD_CONST               2 ('from app.infra import ')
+                           532 LOAD_CONST               3 (', ')
+                           534 LOAD_METHOD             12 (join)
+                           556 LOAD_GLOBAL             23 (NULL + sorted)
+                           568 LOAD_FAST                3 (infra_names)
+                           570 PRECALL                  1
+                           574 CALL                     1
+                           584 PRECALL                  1
+                           588 CALL                     1
+                           598 FORMAT_VALUE             0
+                           600 BUILD_STRING             2
+                           602 PRECALL                  1
+                           606 CALL                     1
+                           616 POP_TOP
+               
+               411         618 LOAD_FAST                1 (to_return)
+                           620 LOAD_METHOD              8 (extend)
+                           642 LOAD_GLOBAL             23 (NULL + sorted)
+                           654 LOAD_FAST                4 (app_imports)
+                           656 PRECALL                  1
+                           660 CALL                     1
+                           670 PRECALL                  1
+                           674 CALL                     1
+                           684 POP_TOP
                
-               271         382 LOAD_FAST                1 (to_return)
-                           384 RETURN_VALUE
+               412         686 LOAD_FAST                1 (to_return)
+                           688 RETURN_VALUE
                consts
                   None
                   0
-                  'from launchflow.gcp import get_service_account_credentials'
-                  'from django_app.infra import '
+                  'from app.infra import '
                   ', '
-               names      ('len', 'resources', 'GCSBucket', 'append', 'get_resource_info', 'infra_name', 'join', 'sorted')
-               varnames   ('self', 'to_return', 'infra_names', 'resource', 'resource_info')
+               names      ('len', 'resources', 'set', 'get_resource_info', 'append', 'infra_name', 'add', 'launchflow_imports', 'extend', 'app_imports', 'infra_import', 'sorted', 'join')
+               varnames   ('self', 'to_return', 'client_imports', 'infra_names', 'app_imports', 'launchflow_imports', 'resource', 'resource_info')
                freevars   ()
                cellvars   ()
-               filename   '/home/tanke/launchflow/launchflow/clients/python/launchflow/launchflow/cli/gen/templates/django/django_template.py'
+               filename   '/Users/calebvandyke/code/launchflow-oss/launchflow/cli/gen/templates/flask/flask_template.py'
                name       'app_infra_imports'
-               firstlineno 248
+               firstlineno 390
                lnotab
-                  0x0204300104010401040212011601180102ff10031e0136022601040218
-                  0148ff1003
+                  0x02043001040104010401040104011c0112011e013401340134010e0136
+                  014401440170014401
             code
                argcount  : 1
                nlocals   : 4
                stacksize : 4
                flags     : 3
                code
                   0x970067007d017c006a00000000000000000044005d327d027403000000
                   000000000000007c02a6010000ab0100000000000000007d037c036a0200
                   00000000000000811a7c01a0030000000000000000000000000000000000
                   0000007c036a020000000000000000a6010000ab01000000000000000001
                   008c336401a00400000000000000000000000000000000000000007c01a6
                   010000ab0100000000000000005300
-               274           0 RESUME                   0
+               415           0 RESUME                   0
                
-               276           2 BUILD_LIST               0
+               417           2 BUILD_LIST               0
                              4 STORE_FAST               1 (lines)
                
-               277           6 LOAD_FAST                0 (self)
+               418           6 LOAD_FAST                0 (self)
                              8 LOAD_ATTR                0 (resources)
                             18 GET_ITER
                        >>   20 FOR_ITER                50 (to 122)
                             22 STORE_FAST               2 (resource)
                
-               278          24 LOAD_GLOBAL              3 (NULL + get_resource_info)
+               419          24 LOAD_GLOBAL              3 (NULL + get_resource_info)
                             36 LOAD_FAST                2 (resource)
                             38 PRECALL                  1
                             42 CALL                     1
                             52 STORE_FAST               3 (resource_info)
                
-               279          54 LOAD_FAST                3 (resource_info)
-                            56 LOAD_ATTR                2 (django_settings)
+               420          54 LOAD_FAST                3 (resource_info)
+                            56 LOAD_ATTR                2 (global_setup)
                             66 POP_JUMP_FORWARD_IF_NONE    26 (to 120)
                
-               280          68 LOAD_FAST                1 (lines)
+               421          68 LOAD_FAST                1 (lines)
                             70 LOAD_METHOD              3 (append)
                             92 LOAD_FAST                3 (resource_info)
-                            94 LOAD_ATTR                2 (django_settings)
+                            94 LOAD_ATTR                2 (global_setup)
                            104 PRECALL                  1
                            108 CALL                     1
                            118 POP_TOP
                        >>  120 JUMP_BACKWARD           51 (to 20)
                
-               281     >>  122 LOAD_CONST               1 ('\n')
+               422     >>  122 LOAD_CONST               1 ('\n')
                            124 LOAD_METHOD              4 (join)
                            146 LOAD_FAST                1 (lines)
                            148 PRECALL                  1
                            152 CALL                     1
                            162 RETURN_VALUE
                consts
                   None
                   '\n'
-               names      ('resources', 'get_resource_info', 'django_settings', 'append', 'join')
+               names      ('resources', 'get_resource_info', 'global_setup', 'append', 'join')
                varnames   ('self', 'lines', 'resource', 'resource_info')
                freevars   ()
                cellvars   ()
-               filename   '/home/tanke/launchflow/launchflow/clients/python/launchflow/launchflow/cli/gen/templates/django/django_template.py'
-               name       'app_django_settings'
-               firstlineno 274
-               lnotab 0x0202040112011e010e013601
-            code
-               argcount  : 1
-               nlocals   : 4
-               stacksize : 4
-               flags     : 3
-               code
-                  0x970067007d017c006a00000000000000000044005d327d027403000000
-                  000000000000007c02a6010000ab0100000000000000007d037c036a0200
-                  00000000000000811a7c01a0030000000000000000000000000000000000
-                  0000007c036a020000000000000000a6010000ab01000000000000000001
-                  008c337c015300
-               284           0 RESUME                   0
-               
-               286           2 BUILD_LIST               0
-                             4 STORE_FAST               1 (installed_apps)
-               
-               287           6 LOAD_FAST                0 (self)
-                             8 LOAD_ATTR                0 (resources)
-                            18 GET_ITER
-                       >>   20 FOR_ITER                50 (to 122)
-                            22 STORE_FAST               2 (resource)
-               
-               288          24 LOAD_GLOBAL              3 (NULL + get_resource_info)
-                            36 LOAD_FAST                2 (resource)
-                            38 PRECALL                  1
-                            42 CALL                     1
-                            52 STORE_FAST               3 (resource_info)
-               
-               289          54 LOAD_FAST                3 (resource_info)
-                            56 LOAD_ATTR                2 (installed_app)
-                            66 POP_JUMP_FORWARD_IF_NONE    26 (to 120)
-               
-               290          68 LOAD_FAST                1 (installed_apps)
-                            70 LOAD_METHOD              3 (append)
-                            92 LOAD_FAST                3 (resource_info)
-                            94 LOAD_ATTR                2 (installed_app)
-                           104 PRECALL                  1
-                           108 CALL                     1
-                           118 POP_TOP
-                       >>  120 JUMP_BACKWARD           51 (to 20)
-               
-               291     >>  122 LOAD_FAST                1 (installed_apps)
-                           124 RETURN_VALUE
-               consts
-                  None
-               names      ('resources', 'get_resource_info', 'installed_app', 'append')
-               varnames   ('self', 'installed_apps', 'resource', 'resource_info')
-               freevars   ()
-               cellvars   ()
-               filename   '/home/tanke/launchflow/launchflow/clients/python/launchflow/launchflow/cli/gen/templates/django/django_template.py'
-               name       'app_installed_apps'
-               firstlineno 284
-               lnotab 0x0202040112011e010e013601
-            code
-               argcount  : 1
-               nlocals   : 4
-               stacksize : 4
-               flags     : 3
-               code
-                  0x970067007d017c006a00000000000000000044005d327d027403000000
-                  000000000000007c02a6010000ab0100000000000000007d037c036a0200
-                  00000000000000811a7c01a0030000000000000000000000000000000000
-                  0000007c036a020000000000000000a6010000ab01000000000000000001
-                  008c337c015300
-               294           0 RESUME                   0
-               
-               296           2 BUILD_LIST               0
-                             4 STORE_FAST               1 (urls)
-               
-               297           6 LOAD_FAST                0 (self)
-                             8 LOAD_ATTR                0 (resources)
-                            18 GET_ITER
-                       >>   20 FOR_ITER                50 (to 122)
-                            22 STORE_FAST               2 (resource)
-               
-               298          24 LOAD_GLOBAL              3 (NULL + get_resource_info)
-                            36 LOAD_FAST                2 (resource)
-                            38 PRECALL                  1
-                            42 CALL                     1
-                            52 STORE_FAST               3 (resource_info)
-               
-               299          54 LOAD_FAST                3 (resource_info)
-                            56 LOAD_ATTR                2 (django_test_endpoint_url)
-                            66 POP_JUMP_FORWARD_IF_NONE    26 (to 120)
-               
-               300          68 LOAD_FAST                1 (urls)
-                            70 LOAD_METHOD              3 (append)
-                            92 LOAD_FAST                3 (resource_info)
-                            94 LOAD_ATTR                2 (django_test_endpoint_url)
-                           104 PRECALL                  1
-                           108 CALL                     1
-                           118 POP_TOP
-                       >>  120 JUMP_BACKWARD           51 (to 20)
-               
-               301     >>  122 LOAD_FAST                1 (urls)
-                           124 RETURN_VALUE
-               consts
-                  None
-               names      ('resources', 'get_resource_info', 'django_test_endpoint_url', 'append')
-               varnames   ('self', 'urls', 'resource', 'resource_info')
-               freevars   ()
-               cellvars   ()
-               filename   '/home/tanke/launchflow/launchflow/clients/python/launchflow/launchflow/cli/gen/templates/django/django_template.py'
-               name       'app_infra_urls'
-               firstlineno 294
+               filename   '/Users/calebvandyke/code/launchflow-oss/launchflow/cli/gen/templates/flask/flask_template.py'
+               name       'app_global_setup'
+               firstlineno 415
                lnotab 0x0202040112011e010e013601
             code
                argcount  : 1
                nlocals   : 4
                stacksize : 4
                flags     : 3
                code
                   0x970067007d017c006a00000000000000000044005d327d027403000000
                   000000000000007c02a6010000ab0100000000000000007d037c036a0200
                   00000000000000811a7c01a0030000000000000000000000000000000000
                   0000007c036a020000000000000000a6010000ab01000000000000000001
-                  008c337c015300
-               304           0 RESUME                   0
+                  008c336401a00400000000000000000000000000000000000000007c01a6
+                  010000ab0100000000000000005300
+               425           0 RESUME                   0
                
-               306           2 BUILD_LIST               0
-                             4 STORE_FAST               1 (imports)
+               427           2 BUILD_LIST               0
+                             4 STORE_FAST               1 (infra_steps)
                
-               307           6 LOAD_FAST                0 (self)
+               428           6 LOAD_FAST                0 (self)
                              8 LOAD_ATTR                0 (resources)
                             18 GET_ITER
                        >>   20 FOR_ITER                50 (to 122)
                             22 STORE_FAST               2 (resource)
                
-               308          24 LOAD_GLOBAL              3 (NULL + get_resource_info)
+               429          24 LOAD_GLOBAL              3 (NULL + get_resource_info)
                             36 LOAD_FAST                2 (resource)
                             38 PRECALL                  1
                             42 CALL                     1
                             52 STORE_FAST               3 (resource_info)
                
-               309          54 LOAD_FAST                3 (resource_info)
-                            56 LOAD_ATTR                2 (views_imports)
+               430          54 LOAD_FAST                3 (resource_info)
+                            56 LOAD_ATTR                2 (infra_setup)
                             66 POP_JUMP_FORWARD_IF_NONE    26 (to 120)
                
-               310          68 LOAD_FAST                1 (imports)
+               431          68 LOAD_FAST                1 (infra_steps)
                             70 LOAD_METHOD              3 (append)
                             92 LOAD_FAST                3 (resource_info)
-                            94 LOAD_ATTR                2 (views_imports)
+                            94 LOAD_ATTR                2 (infra_setup)
                            104 PRECALL                  1
                            108 CALL                     1
                            118 POP_TOP
                        >>  120 JUMP_BACKWARD           51 (to 20)
                
-               311     >>  122 LOAD_FAST                1 (imports)
-                           124 RETURN_VALUE
+               432     >>  122 LOAD_CONST               1 ('\n')
+                           124 LOAD_METHOD              4 (join)
+                           146 LOAD_FAST                1 (infra_steps)
+                           148 PRECALL                  1
+                           152 CALL                     1
+                           162 RETURN_VALUE
                consts
                   None
-               names      ('resources', 'get_resource_info', 'views_imports', 'append')
-               varnames   ('self', 'imports', 'resource', 'resource_info')
+                  '\n'
+               names      ('resources', 'get_resource_info', 'infra_setup', 'append', 'join')
+               varnames   ('self', 'infra_steps', 'resource', 'resource_info')
                freevars   ()
                cellvars   ()
-               filename   '/home/tanke/launchflow/launchflow/clients/python/launchflow/launchflow/cli/gen/templates/django/django_template.py'
-               name       'app_views_imports'
-               firstlineno 304
+               filename   '/Users/calebvandyke/code/launchflow-oss/launchflow/cli/gen/templates/flask/flask_template.py'
+               name       'app_infra_setup'
+               firstlineno 425
                lnotab 0x0202040112011e010e013601
             code
                argcount  : 1
                nlocals   : 4
                stacksize : 4
                flags     : 3
                code
-                  0x970067007d017c006a00000000000000000044005d327d027403000000
-                  000000000000007c02a6010000ab0100000000000000007d037c036a0200
-                  00000000000000811a7c01a0030000000000000000000000000000000000
-                  0000007c036a020000000000000000a6010000ab01000000000000000001
-                  008c337c015300
-               314           0 RESUME                   0
+                  0x970067007d017c006a00000000000000000044005d2b7d027403000000
+                  000000000000007c02a6010000ab0100000000000000007d037c01a00200
+                  000000000000000000000000000000000000007c036a0300000000000000
+                  00a6010000ab01000000000000000001008c2c7c015300
+               435           0 RESUME                   0
                
-               316           2 BUILD_LIST               0
+               437           2 BUILD_LIST               0
                              4 STORE_FAST               1 (endpoints)
                
-               317           6 LOAD_FAST                0 (self)
+               438           6 LOAD_FAST                0 (self)
                              8 LOAD_ATTR                0 (resources)
                             18 GET_ITER
-                       >>   20 FOR_ITER                50 (to 122)
+                       >>   20 FOR_ITER                43 (to 108)
                             22 STORE_FAST               2 (resource)
                
-               318          24 LOAD_GLOBAL              3 (NULL + get_resource_info)
+               439          24 LOAD_GLOBAL              3 (NULL + get_resource_info)
                             36 LOAD_FAST                2 (resource)
                             38 PRECALL                  1
                             42 CALL                     1
                             52 STORE_FAST               3 (resource_info)
                
-               319          54 LOAD_FAST                3 (resource_info)
-                            56 LOAD_ATTR                2 (django_test_endpoint)
-                            66 POP_JUMP_FORWARD_IF_NONE    26 (to 120)
+               440          54 LOAD_FAST                1 (endpoints)
+                            56 LOAD_METHOD              2 (append)
+                            78 LOAD_FAST                3 (resource_info)
+                            80 LOAD_ATTR                3 (flask_test_endpoint)
+                            90 PRECALL                  1
+                            94 CALL                     1
+                           104 POP_TOP
+                           106 JUMP_BACKWARD           44 (to 20)
                
-               320          68 LOAD_FAST                1 (endpoints)
-                            70 LOAD_METHOD              3 (append)
-                            92 LOAD_FAST                3 (resource_info)
-                            94 LOAD_ATTR                2 (django_test_endpoint)
-                           104 PRECALL                  1
-                           108 CALL                     1
-                           118 POP_TOP
-                       >>  120 JUMP_BACKWARD           51 (to 20)
-               
-               321     >>  122 LOAD_FAST                1 (endpoints)
-                           124 RETURN_VALUE
+               441     >>  108 LOAD_FAST                1 (endpoints)
+                           110 RETURN_VALUE
                consts
                   None
-               names      ('resources', 'get_resource_info', 'django_test_endpoint', 'append')
+               names      ('resources', 'get_resource_info', 'append', 'flask_test_endpoint')
                varnames   ('self', 'endpoints', 'resource', 'resource_info')
                freevars   ()
                cellvars   ()
-               filename   '/home/tanke/launchflow/launchflow/clients/python/launchflow/launchflow/cli/gen/templates/django/django_template.py'
+               filename   '/Users/calebvandyke/code/launchflow-oss/launchflow/cli/gen/templates/flask/flask_template.py'
                name       'app_infra_endpoints'
-               firstlineno 314
-               lnotab 0x0202040112011e010e013601
+               firstlineno 435
+               lnotab 0x0202040112011e013601
             code
                argcount  : 1
                nlocals   : 4
                stacksize : 5
                flags     : 3
                code
                   0x9700740100000000000000000000a6000000ab0000000000000000007d
                   017c006a01000000000000000044005d2b7d027405000000000000000000
                   007c02a6010000ab0100000000000000007d037c01a00300000000000000
                   000000000000000000000000007c036a040000000000000000a6010000ab
                   01000000000000000001008c2c6401a00500000000000000000000000000
                   00000000000000740d000000000000000000007c01a6010000ab01000000
                   0000000000a6010000ab0100000000000000005300
-               324           0 RESUME                   0
+               444           0 RESUME                   0
                
-               326           2 LOAD_GLOBAL              1 (NULL + set)
+               446           2 LOAD_GLOBAL              1 (NULL + set)
                             14 PRECALL                  0
                             18 CALL                     0
                             28 STORE_FAST               1 (requirements)
                
-               327          30 LOAD_FAST                0 (self)
+               447          30 LOAD_FAST                0 (self)
                             32 LOAD_ATTR                1 (resources)
                             42 GET_ITER
                        >>   44 FOR_ITER                43 (to 132)
                             46 STORE_FAST               2 (resource)
                
-               328          48 LOAD_GLOBAL              5 (NULL + get_resource_info)
+               448          48 LOAD_GLOBAL              5 (NULL + get_resource_info)
                             60 LOAD_FAST                2 (resource)
                             62 PRECALL                  1
                             66 CALL                     1
                             76 STORE_FAST               3 (resource_info)
                
-               329          78 LOAD_FAST                1 (requirements)
+               449          78 LOAD_FAST                1 (requirements)
                             80 LOAD_METHOD              3 (update)
                            102 LOAD_FAST                3 (resource_info)
                            104 LOAD_ATTR                4 (requirements)
                            114 PRECALL                  1
                            118 CALL                     1
                            128 POP_TOP
                            130 JUMP_BACKWARD           44 (to 44)
                
-               330     >>  132 LOAD_CONST               1 ('\n')
+               450     >>  132 LOAD_CONST               1 ('\n')
                            134 LOAD_METHOD              5 (join)
                            156 LOAD_GLOBAL             13 (NULL + sorted)
                            168 LOAD_FAST                1 (requirements)
                            170 PRECALL                  1
                            174 CALL                     1
                            184 PRECALL                  1
                            188 CALL                     1
@@ -1457,49 +1453,49 @@
                consts
                   None
                   '\n'
                names      ('set', 'resources', 'get_resource_info', 'update', 'requirements', 'join', 'sorted')
                varnames   ('self', 'requirements', 'resource', 'resource_info')
                freevars   ()
                cellvars   ()
-               filename   '/home/tanke/launchflow/launchflow/clients/python/launchflow/launchflow/cli/gen/templates/django/django_template.py'
+               filename   '/Users/calebvandyke/code/launchflow-oss/launchflow/cli/gen/templates/flask/flask_template.py'
                name       'additional_requirements'
-               firstlineno 324
+               firstlineno 444
                lnotab 0x02021c0112011e013601
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 4
                flags     : 3
                code
                   0x97007c006a00000000000000000064016b02000000007202640253007c
                   006a00000000000000000064036b02000000007202640453007403000000
                   0000000000000064057c006a0000000000000000009b009d02a6010000ab
                   0100000000000000008201
-               333           0 RESUME                   0
+               453           0 RESUME                   0
                
-               335           2 LOAD_FAST                0 (self)
+               455           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (cloud_provider)
                             14 LOAD_CONST               1 ('aws')
                             16 COMPARE_OP               2 (==)
                             22 POP_JUMP_FORWARD_IF_FALSE     2 (to 28)
                
-               336          24 LOAD_CONST               2 ('aws_ecs_fargate')
+               456          24 LOAD_CONST               2 ('aws_ecs_fargate')
                             26 RETURN_VALUE
                
-               337     >>   28 LOAD_FAST                0 (self)
+               457     >>   28 LOAD_FAST                0 (self)
                             30 LOAD_ATTR                0 (cloud_provider)
                             40 LOAD_CONST               3 ('gcp')
                             42 COMPARE_OP               2 (==)
                             48 POP_JUMP_FORWARD_IF_FALSE     2 (to 54)
                
-               338          50 LOAD_CONST               4 ('gcp_cloud_run')
+               458          50 LOAD_CONST               4 ('gcp_cloud_run')
                             52 RETURN_VALUE
                
-               339     >>   54 LOAD_GLOBAL              3 (NULL + ValueError)
+               459     >>   54 LOAD_GLOBAL              3 (NULL + ValueError)
                             66 LOAD_CONST               5 ('Unsupported cloud provider: ')
                             68 LOAD_FAST                0 (self)
                             70 LOAD_ATTR                0 (cloud_provider)
                             80 FORMAT_VALUE             0
                             82 BUILD_STRING             2
                             84 PRECALL                  1
                             88 CALL                     1
@@ -1511,357 +1507,331 @@
                   'gcp'
                   'gcp_cloud_run'
                   'Unsupported cloud provider: '
                names      ('cloud_provider', 'ValueError')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   '/home/tanke/launchflow/launchflow/clients/python/launchflow/launchflow/cli/gen/templates/django/django_template.py'
+               filename   '/Users/calebvandyke/code/launchflow-oss/launchflow/cli/gen/templates/flask/flask_template.py'
                name       'launchflow_service_product'
-               firstlineno 333
+               firstlineno 453
                lnotab 0x02021601040116010401
             code
                argcount  : 1
-               nlocals   : 1
+               nlocals   : 3
                stacksize : 3
                flags     : 3
                code
-                  0x9700740000000000000000000000640184007c006a0100000000000000
-                  004400a6000000ab00000000000000000076007318740400000000000000
-                  000000640284007c006a0100000000000000004400a6000000ab00000000
-                  0000000000760072026403530064045300
-               341           0 RESUME                   0
-               
-               342           2 LOAD_GLOBAL              0 (CloudSQLPostgres)
-                            14 LOAD_CONST               1 (<code object <listcomp>, file "/home/tanke/launchflow/launchflow/clients/python/launchflow/launchflow/cli/gen/templates/django/django_template.py", line 342>)
-                            16 MAKE_FUNCTION            0
-               
-               343          18 LOAD_FAST                0 (self)
-                            20 LOAD_ATTR                1 (resources)
-               
-               342          30 GET_ITER
-                            32 PRECALL                  0
-                            36 CALL                     0
-                            46 CONTAINS_OP              0
-                            48 POP_JUMP_FORWARD_IF_TRUE    24 (to 98)
-               
-               344          50 LOAD_GLOBAL              4 (RDSPostgres)
-                            62 LOAD_CONST               2 (<code object <listcomp>, file "/home/tanke/launchflow/launchflow/clients/python/launchflow/launchflow/cli/gen/templates/django/django_template.py", line 344>)
-                            64 MAKE_FUNCTION            0
-                            66 LOAD_FAST                0 (self)
-                            68 LOAD_ATTR                1 (resources)
-                            78 GET_ITER
-                            80 PRECALL                  0
-                            84 CALL                     0
-                            94 CONTAINS_OP              0
-                            96 POP_JUMP_FORWARD_IF_FALSE     2 (to 102)
-               
-               345     >>   98 LOAD_CONST               3 ('launchflow.cli.gen.templates.django._postgres_template')
-                           100 RETURN_VALUE
-               
-               346     >>  102 LOAD_CONST               4 ('launchflow.cli.gen.templates.django._simple_template')
-                           104 RETURN_VALUE
+                  0x970064017d0164027d02740000000000000000000000640384007c006a
+                  0100000000000000004400a6000000ab0000000000000000007600731874
+                  0400000000000000000000640484007c006a0100000000000000004400a6
+                  000000ab0000000000000000007600720264057d027c017c0266025300
+               461           0 RESUME                   0
+               
+               462           2 LOAD_CONST               1 ('launchflow.cli.gen.templates.flask')
+                             4 STORE_FAST               1 (template_dir)
+               
+               463           6 LOAD_CONST               2 ('_simple_template')
+                             8 STORE_FAST               2 (template_name)
+               
+               465          10 LOAD_GLOBAL              0 (CloudSQLPostgres)
+                            22 LOAD_CONST               3 (<code object <listcomp>, file "/Users/calebvandyke/code/launchflow-oss/launchflow/cli/gen/templates/flask/flask_template.py", line 465>)
+                            24 MAKE_FUNCTION            0
+               
+               466          26 LOAD_FAST                0 (self)
+                            28 LOAD_ATTR                1 (resources)
+               
+               465          38 GET_ITER
+                            40 PRECALL                  0
+                            44 CALL                     0
+                            54 CONTAINS_OP              0
+                            56 POP_JUMP_FORWARD_IF_TRUE    24 (to 106)
+               
+               467          58 LOAD_GLOBAL              4 (RDSPostgres)
+                            70 LOAD_CONST               4 (<code object <listcomp>, file "/Users/calebvandyke/code/launchflow-oss/launchflow/cli/gen/templates/flask/flask_template.py", line 467>)
+                            72 MAKE_FUNCTION            0
+                            74 LOAD_FAST                0 (self)
+                            76 LOAD_ATTR                1 (resources)
+                            86 GET_ITER
+                            88 PRECALL                  0
+                            92 CALL                     0
+                           102 CONTAINS_OP              0
+                           104 POP_JUMP_FORWARD_IF_FALSE     2 (to 110)
+               
+               468     >>  106 LOAD_CONST               5 ('_postgres_template')
+                           108 STORE_FAST               2 (template_name)
+               
+               470     >>  110 LOAD_FAST                1 (template_dir)
+                           112 LOAD_FAST                2 (template_name)
+                           114 BUILD_TUPLE              2
+                           116 RETURN_VALUE
                consts
                   None
+                  'launchflow.cli.gen.templates.flask'
+                  '_simple_template'
                   code
                      argcount  : 1
                      nlocals   : 2
                      stacksize : 3
                      flags     : 19
                      code 0x970067007c005d047d017c0191028c055300
-                     342           0 RESUME                   0
+                     465           0 RESUME                   0
                                    2 BUILD_LIST               0
                                    4 LOAD_FAST                0 (.0)
                              >>    6 FOR_ITER                 4 (to 16)
                      
-                     343           8 STORE_FAST               1 (resource)
+                     466           8 STORE_FAST               1 (resource)
                                   10 LOAD_FAST                1 (resource)
                      
-                     342          12 LIST_APPEND              2
+                     465          12 LIST_APPEND              2
                                   14 JUMP_BACKWARD            5 (to 6)
                              >>   16 RETURN_VALUE
                      consts
                      names      ()
                      varnames   ('.0', 'resource')
                      freevars   ()
                      cellvars   ()
-                     filename   '/home/tanke/launchflow/launchflow/clients/python/launchflow/launchflow/cli/gen/templates/django/django_template.py'
+                     filename   '/Users/calebvandyke/code/launchflow-oss/launchflow/cli/gen/templates/flask/flask_template.py'
                      name       '<listcomp>'
-                     firstlineno 342
+                     firstlineno 465
                      lnotab 0x080104ff
                   code
                      argcount  : 1
                      nlocals   : 2
                      stacksize : 3
                      flags     : 19
                      code 0x970067007c005d047d017c0191028c055300
-                     344           0 RESUME                   0
+                     467           0 RESUME                   0
                                    2 BUILD_LIST               0
                                    4 LOAD_FAST                0 (.0)
                              >>    6 FOR_ITER                 4 (to 16)
                                    8 STORE_FAST               1 (resource)
                                   10 LOAD_FAST                1 (resource)
                                   12 LIST_APPEND              2
                                   14 JUMP_BACKWARD            5 (to 6)
                              >>   16 RETURN_VALUE
                      consts
                      names      ()
                      varnames   ('.0', 'resource')
                      freevars   ()
                      cellvars   ()
-                     filename   '/home/tanke/launchflow/launchflow/clients/python/launchflow/launchflow/cli/gen/templates/django/django_template.py'
+                     filename   '/Users/calebvandyke/code/launchflow-oss/launchflow/cli/gen/templates/flask/flask_template.py'
                      name       '<listcomp>'
-                     firstlineno 344
+                     firstlineno 467
                      lnotab 0x
-                  'launchflow.cli.gen.templates.django._postgres_template'
-                  'launchflow.cli.gen.templates.django._simple_template'
+                  '_postgres_template'
                names      ('CloudSQLPostgres', 'resources', 'RDSPostgres')
-               varnames   ('self',)
+               varnames   ('self', 'template_dir', 'template_name')
                freevars   ()
                cellvars   ()
-               filename   '/home/tanke/launchflow/launchflow/clients/python/launchflow/launchflow/cli/gen/templates/django/django_template.py'
-               name       'template_directory'
-               firstlineno 341
-               lnotab 0x020110010cff140230010401
+               filename   '/Users/calebvandyke/code/launchflow-oss/launchflow/cli/gen/templates/flask/flask_template.py'
+               name       'template_path_info'
+               firstlineno 461
+               lnotab 0x02010401040210010cff140230010402
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c006a00000000000000000064016b020000000072026402530064
                   035300
-               348           0 RESUME                   0
+               472           0 RESUME                   0
                
-               350           2 LOAD_FAST                0 (self)
+               474           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (cloud_provider)
                             14 LOAD_CONST               1 ('aws')
                             16 COMPARE_OP               2 (==)
                             22 POP_JUMP_FORWARD_IF_FALSE     2 (to 28)
                
-               351          24 LOAD_CONST               2 ('public.ecr.aws/docker/library/')
+               475          24 LOAD_CONST               2 ('public.ecr.aws/docker/library/')
                             26 RETURN_VALUE
                
-               352     >>   28 LOAD_CONST               3 ('')
+               476     >>   28 LOAD_CONST               3 ('')
                             30 RETURN_VALUE
                consts
                   None
                   'aws'
                   'public.ecr.aws/docker/library/'
                   ''
                names      ('cloud_provider',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   '/home/tanke/launchflow/launchflow/clients/python/launchflow/launchflow/cli/gen/templates/django/django_template.py'
+               filename   '/Users/calebvandyke/code/launchflow-oss/launchflow/cli/gen/templates/flask/flask_template.py'
                name       'docker_repository_prefix'
-               firstlineno 348
+               firstlineno 472
                lnotab 0x020216010401
             code
                argcount  : 1
                nlocals   : 1
-               stacksize : 5
+               stacksize : 3
                flags     : 3
                code
                   0x9700690064017c006a000000000000000000930164027c006a01000000
                   0000000000930164037c006a020000000000000000930164047c006a0300
                   00000000000000930164057c006a040000000000000000930164067c006a
                   050000000000000000930164077c006a060000000000000000930164087c
                   006a070000000000000000930164097c006a080000000000000000930164
                   0a7c006a0900000000000000009301640b7c006a0a000000000000000093
                   01640c7c006a0b00000000000000009301640d7c006a0c00000000000000
-                  009301640e7c006a0d00000000000000009301640f741c00000000000000
-                  0000006a0e0000000000000000a00f000000000000000000000000000000
-                  0000000000a6000000ab000000000000000000a010000000000000000000
-                  00000000000000000000006410a6010000ab010000000000000000930164
-                  117c006a110000000000000000930164127c006a12000000000000000093
-                  0164137c006a1300000000000000006901a5015300
-               354           0 RESUME                   0
+                  009301640e7c006a0d00000000000000009301640f7c006a0e0000000000
+                  000000930164107c006a0f000000000000000093015300
+               478           0 RESUME                   0
                
-               355           2 BUILD_MAP                0
+               479           2 BUILD_MAP                0
                
-               357           4 LOAD_CONST               1 ('cloud_provider')
+               481           4 LOAD_CONST               1 ('cloud_provider')
                              6 LOAD_FAST                0 (self)
                              8 LOAD_ATTR                0 (cloud_provider)
                
-               355          18 MAP_ADD                  1
+               479          18 MAP_ADD                  1
                
-               358          20 LOAD_CONST               2 ('additional_requirements')
+               482          20 LOAD_CONST               2 ('additional_requirements')
                             22 LOAD_FAST                0 (self)
                             24 LOAD_ATTR                1 (additional_requirements)
                
-               355          34 MAP_ADD                  1
+               479          34 MAP_ADD                  1
                
-               360          36 LOAD_CONST               3 ('launchflow_project_name')
+               484          36 LOAD_CONST               3 ('launchflow_project_name')
                             38 LOAD_FAST                0 (self)
                             40 LOAD_ATTR                2 (launchflow_project_name)
                
-               355          50 MAP_ADD                  1
+               479          50 MAP_ADD                  1
                
-               361          52 LOAD_CONST               4 ('launchflow_environment_name')
+               485          52 LOAD_CONST               4 ('launchflow_environment_name')
                             54 LOAD_FAST                0 (self)
                             56 LOAD_ATTR                3 (launchflow_environment_name)
                
-               355          66 MAP_ADD                  1
+               479          66 MAP_ADD                  1
                
-               362          68 LOAD_CONST               5 ('launchflow_service_name')
+               486          68 LOAD_CONST               5 ('launchflow_service_name')
                             70 LOAD_FAST                0 (self)
                             72 LOAD_ATTR                4 (launchflow_service_name)
                
-               355          82 MAP_ADD                  1
+               479          82 MAP_ADD                  1
                
-               363          84 LOAD_CONST               6 ('launchflow_service_product')
+               487          84 LOAD_CONST               6 ('launchflow_service_product')
                             86 LOAD_FAST                0 (self)
                             88 LOAD_ATTR                5 (launchflow_service_product)
                
-               355          98 MAP_ADD                  1
+               479          98 MAP_ADD                  1
                
-               365         100 LOAD_CONST               7 ('docker_repository_prefix')
+               489         100 LOAD_CONST               7 ('docker_repository_prefix')
                            102 LOAD_FAST                0 (self)
                            104 LOAD_ATTR                6 (docker_repository_prefix)
                
-               355         114 MAP_ADD                  1
+               479         114 MAP_ADD                  1
                
-               366         116 LOAD_CONST               8 ('python_major_version')
+               490         116 LOAD_CONST               8 ('python_major_version')
                            118 LOAD_FAST                0 (self)
                            120 LOAD_ATTR                7 (python_major_version)
                
-               355         130 MAP_ADD                  1
+               479         130 MAP_ADD                  1
                
-               367         132 LOAD_CONST               9 ('python_minor_version')
+               491         132 LOAD_CONST               9 ('python_minor_version')
                            134 LOAD_FAST                0 (self)
                            136 LOAD_ATTR                8 (python_minor_version)
                
-               355         146 MAP_ADD                  1
+               479         146 MAP_ADD                  1
                
-               368         148 LOAD_CONST              10 ('port')
+               492         148 LOAD_CONST              10 ('port')
                            150 LOAD_FAST                0 (self)
                            152 LOAD_ATTR                9 (port)
                
-               355         162 MAP_ADD                  1
+               479         162 MAP_ADD                  1
                
-               370         164 LOAD_CONST              11 ('infra_dot_py')
+               494         164 LOAD_CONST              11 ('infra_dot_py')
                            166 LOAD_FAST                0 (self)
                            168 LOAD_ATTR               10 (infra_dot_py)
                
-               355         178 MAP_ADD                  1
+               479         178 MAP_ADD                  1
                
-               372         180 LOAD_CONST              12 ('app_infra_imports')
+               496         180 LOAD_CONST              12 ('flask_imports')
                            182 LOAD_FAST                0 (self)
-                           184 LOAD_ATTR               11 (app_infra_imports)
+                           184 LOAD_ATTR               11 (flask_imports)
                
-               355         194 MAP_ADD                  1
+               479         194 MAP_ADD                  1
                
-               373         196 LOAD_CONST              13 ('app_django_settings')
+               497         196 LOAD_CONST              13 ('app_infra_imports')
                            198 LOAD_FAST                0 (self)
-                           200 LOAD_ATTR               12 (app_django_settings)
+                           200 LOAD_ATTR               12 (app_infra_imports)
                
-               355         210 MAP_ADD                  1
+               479         210 MAP_ADD                  1
                
-               374         212 LOAD_CONST              14 ('app_installed_apps')
+               498         212 LOAD_CONST              14 ('app_global_setup')
                            214 LOAD_FAST                0 (self)
-                           216 LOAD_ATTR               13 (app_installed_apps)
+                           216 LOAD_ATTR               13 (app_global_setup)
+               
+               479         226 MAP_ADD                  1
+               
+               499         228 LOAD_CONST              15 ('app_infra_setup')
+                           230 LOAD_FAST                0 (self)
+                           232 LOAD_ATTR               14 (app_infra_setup)
+               
+               479         242 MAP_ADD                  1
                
-               355         226 MAP_ADD                  1
+               500         244 LOAD_CONST              16 ('app_infra_endpoints')
+                           246 LOAD_FAST                0 (self)
+                           248 LOAD_ATTR               15 (app_infra_endpoints)
                
-               376         228 LOAD_CONST              15 ('current_timestamp')
-                           230 LOAD_GLOBAL             28 (datetime)
-                           242 LOAD_ATTR               14 (datetime)
-                           252 LOAD_METHOD             15 (now)
-                           274 PRECALL                  0
-                           278 CALL                     0
-                           288 LOAD_METHOD             16 (strftime)
-                           310 LOAD_CONST              16 ('%Y-%m-%d %H:%M')
-                           312 PRECALL                  1
-                           316 CALL                     1
-               
-               355         326 MAP_ADD                  1
-               
-               378         328 LOAD_CONST              17 ('app_infra_urls')
-                           330 LOAD_FAST                0 (self)
-                           332 LOAD_ATTR               17 (app_infra_urls)
-               
-               355         342 MAP_ADD                  1
-               
-               380         344 LOAD_CONST              18 ('app_infra_endpoints')
-                           346 LOAD_FAST                0 (self)
-                           348 LOAD_ATTR               18 (app_infra_endpoints)
-               
-               355         358 MAP_ADD                  1
-               
-               381         360 LOAD_CONST              19 ('app_views_imports')
-                           362 LOAD_FAST                0 (self)
-                           364 LOAD_ATTR               19 (app_views_imports)
-               
-               355         374 BUILD_MAP                1
-                           376 DICT_UPDATE              1
-                           378 RETURN_VALUE
+               479         258 MAP_ADD                  1
+                           260 RETURN_VALUE
                consts
                   None
                   'cloud_provider'
                   'additional_requirements'
                   'launchflow_project_name'
                   'launchflow_environment_name'
                   'launchflow_service_name'
                   'launchflow_service_product'
                   'docker_repository_prefix'
                   'python_major_version'
                   'python_minor_version'
                   'port'
                   'infra_dot_py'
+                  'flask_imports'
                   'app_infra_imports'
-                  'app_django_settings'
-                  'app_installed_apps'
-                  'current_timestamp'
-                  '%Y-%m-%d %H:%M'
-                  'app_infra_urls'
+                  'app_global_setup'
+                  'app_infra_setup'
                   'app_infra_endpoints'
-                  'app_views_imports'
-               names      ('cloud_provider', 'additional_requirements', 'launchflow_project_name', 'launchflow_environment_name', 'launchflow_service_name', 'launchflow_service_product', 'docker_repository_prefix', 'python_major_version', 'python_minor_version', 'port', 'infra_dot_py', 'app_infra_imports', 'app_django_settings', 'app_installed_apps', 'datetime', 'now', 'strftime', 'app_infra_urls', 'app_infra_endpoints', 'app_views_imports')
+               names      ('cloud_provider', 'additional_requirements', 'launchflow_project_name', 'launchflow_environment_name', 'launchflow_service_name', 'launchflow_service_product', 'docker_repository_prefix', 'python_major_version', 'python_minor_version', 'port', 'infra_dot_py', 'flask_imports', 'app_infra_imports', 'app_global_setup', 'app_infra_setup', 'app_infra_endpoints')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   '/home/tanke/launchflow/launchflow/clients/python/launchflow/launchflow/cli/gen/templates/django/django_template.py'
+               filename   '/Users/calebvandyke/code/launchflow-oss/launchflow/cli/gen/templates/flask/flask_template.py'
                name       'context'
-               firstlineno 354
+               firstlineno 478
                lnotab
                   0x020102020efe02030efd02050efb02060efa02070ef902080ef8020a0e
                   f6020b0ef5020c0ef4020d0ef3020f0ef102110eef02120eee02130eed02
-                  1562eb02170ee902190ee7021a0ee6
+                  140eec02150eeb
             None
-         names      ('__name__', '__module__', '__qualname__', 'List', 'Type', 'Resource', '__annotations__', 'Literal', 'str', 'launchflow_service_name', 'sys', 'version_info', 'major', 'python_major_version', 'int', 'minor', 'python_minor_version', 'port', 'property', 'infra_dot_py', 'app_infra_imports', 'app_django_settings', 'app_installed_apps', 'app_infra_urls', 'app_views_imports', 'app_infra_endpoints', 'additional_requirements', 'launchflow_service_product', 'template_directory', 'docker_repository_prefix', 'dict', 'context')
+         names      ('__name__', '__module__', '__qualname__', 'List', 'Type', 'Resource', '__annotations__', 'Literal', 'str', 'launchflow_service_name', 'sys', 'version_info', 'major', 'python_major_version', 'int', 'minor', 'python_minor_version', 'port', 'property', 'infra_dot_py', 'flask_imports', 'app_infra_imports', 'app_global_setup', 'app_infra_setup', 'app_infra_endpoints', 'additional_requirements', 'launchflow_service_product', 'template_path_info', 'docker_repository_prefix', 'dict', 'context')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/home/tanke/launchflow/launchflow/clients/python/launchflow/launchflow/cli/gen/templates/django/django_template.py'
-         name       'DjangoProjectGenerator'
-         firstlineno 186
+         filename   '/Users/calebvandyke/code/launchflow-oss/launchflow/cli/gen/templates/flask/flask_template.py'
+         name       'FlaskProjectGenerator'
+         firstlineno 315
          lnotab
-            0x0c02220216020a010a010e0222012201040302010aff0e01022e020116
-            ff0e01021902010aff0e010209020116ff0e010209020116ff0e01020902
-            0116ff0e010209020116ff0e010209020116ff0e01020802010aff0e0102
-            070c0702010aff0e010205
-      'DjangoProjectGenerator'
-      '__main__'
-      'gcp'
-      '-examples'
-      'dev'
-      'django-service'
-      ('resources', 'cloud_provider', 'launchflow_project_name', 'launchflow_environment_name', 'launchflow_service_name')
-      '/tmp/launchflow'
-      ('destination_path',)
-   names      ('datetime', 'sys', 'dataclasses', 'dataclass', 'typing', 'List', 'Literal', 'Optional', 'Type', 'launchflow.aws.rds', 'RDSPostgres', 'launchflow.aws.s3', 'S3Bucket', 'launchflow.cli.gen.template', 'ProjectGenerator', 'launchflow.gcp.cloudsql', 'CloudSQLPostgres', 'launchflow.gcp.compute_engine', 'ComputeEngineRedis', 'launchflow.gcp.gcs', 'GCSBucket', 'launchflow.gcp.memorystore', 'MemorystoreRedis', 'launchflow', 'Resource', 'ResourceInfo', 'resource_type_to_resource_info_kwargs', 'get_resource_info', 'DjangoProjectGenerator', '__name__', 'cloud_provider', 'generator', 'generate_project')
+            0x0c02220216020a010a010e0222012201040302010aff0e01022e02010a
+            ff0e01020c020116ff0e01021802010aff0e010209020116ff0e01020902
+            0116ff0e010208020116ff0e01020802010aff0e0102070c0b02010aff0e
+            010205
+      'FlaskProjectGenerator'
+   names      ('sys', 'dataclasses', 'dataclass', 'typing', 'List', 'Literal', 'Optional', 'Type', 'launchflow', 'Resource', 'launchflow.aws.elasticache', 'ElasticacheRedis', 'launchflow.aws.rds', 'RDSPostgres', 'launchflow.aws.s3', 'S3Bucket', 'launchflow.cli.gen.template', 'ProjectGenerator', 'launchflow.gcp.cloudsql', 'CloudSQLPostgres', 'launchflow.gcp.compute_engine', 'ComputeEngineRedis', 'launchflow.gcp.gcs', 'GCSBucket', 'launchflow.gcp.memorystore', 'MemorystoreRedis', 'ResourceInfo', 'resource_type_to_resource_info_kwargs', 'get_resource_info', 'FlaskProjectGenerator')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   '/home/tanke/launchflow/launchflow/clients/python/launchflow/launchflow/cli/gen/templates/django/django_template.py'
+   filename   '/Users/calebvandyke/code/launchflow-oss/launchflow/cli/gen/templates/flask/flask_template.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff0201080108010c0118020c010c010c010c010c010c010c020c0302
-      0118ff0e01020e020102010201020102040201020a0201040102eb041802
-      0102010201020102040201020a0201040102eb0418020102010201020102
-      0b0201020c0201040102e204210201020102010201020402010201020104
-      0102f4040f02010201020102010201020a020c0201040102e30420020102
-      01020102010201020402010201040102f4048000fe047f00141c0902011a
-      ff0e01027f00470c01040104020201020102fd020702010801020102f512
-      0d30f1
+      0x00ff020108010c0118020c010c010c010c010c010c010c010c010c0302
+      0118ff0e01020f020102010201020102010201020102010201020c04eb04
+      18020102010201020102010201020102010201020c04eb04180201020102
+      01020102010201020102010201020b02ec04170201020102010201020102
+      010202020102fe02040209023606b6044d02010201020102010201020102
+      0102010201020b02ec041702010201020102010201020102010201020102
+      0c04eb04180201020102010201020102010202020102fe02040209023606
+      b6048000bb047f007f00161c0902011aff0e01
```

### Comparing `launchflow-0.3.9.dev8/launchflow/cli/gen/templates/django/_postgres_template/Dockerfile.jinja` & `launchflow-0.4.0.dev0/launchflow/cli/gen/templates/django/_postgres_template/Dockerfile.jinja`

 * *Files 9% similar despite different names*

```diff
@@ -34,15 +34,14 @@
 COPY --from=builder /install /usr/local/lib/python{{ python_major_version }}.{{ python_minor_version }}/site-packages
 ENV PATH="${PATH}:/usr/local/lib/python{{ python_major_version }}.{{ python_minor_version }}/site-packages/bin"
 
 # Set the working directory and copy only the necessary application files
 WORKDIR /code
 COPY --chown=appuser:appuser ./app /code/app
 COPY --chown=appuser:appuser ./django_app /code/django_app
-COPY --chown=appuser:appuser ./launchflow.yaml /code/launchflow.yaml
 COPY --chown=appuser:appuser ./manage.py /code/manage.py
 
 # Expose the port the app runs on
 EXPOSE $PORT
 
 # Start the application
 CMD exec gunicorn --bind 0.0.0.0:$PORT --workers 1 --threads 8 --timeout 0 django_app.wsgi:application
```

### Comparing `launchflow-0.3.9.dev8/launchflow/cli/gen/templates/django/_postgres_template/README.md.jinja` & `launchflow-0.4.0.dev0/launchflow/cli/gen/templates/django/_postgres_template/README.md.jinja`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 ```
 
 ## 🏃 Run your Application (local)
 
 Run the Django application locally using [Django's Development Server](https://docs.djangoproject.com/en/5.0/intro/tutorial01/#the-development-server).
 
 ```bash
-python manage.py runserver 0.0.0.0:8000
+python manage.py runserver 127.0.0.1:8000
 ```
 
 #### NOTE: The Django Development Server is not suitable for production.
 #### The `Dockerfile` and `launchflow deploy` command uses [Gunicorn](https://gunicorn.org/) instead.
 
 ## 🚀 Deploy your Application (remote)
 
@@ -103,8 +103,8 @@
 
 Automatically <strong>delete</strong> all infrastructure associated with your application.
 
 ```bash
 launchflow destroy
 ```
 
-Learn how this command works in the [LaunchFlow Docs](https://docs.launchflow.com/reference/cli#launchflow-destroy).
+Learn how this command works in the [LaunchFlow Docs](https://docs.launchflow.com/reference/cli#launchflow-destroy).
```

### Comparing `launchflow-0.3.9.dev8/launchflow/cli/gen/templates/django/_postgres_template/app/migrations/0001_initial.py.jinja` & `launchflow-0.4.0.dev0/launchflow/cli/gen/templates/django/_postgres_template/app/migrations/0001_initial.py.jinja`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev8/launchflow/cli/gen/templates/django/_postgres_template/app/views.py.jinja` & `launchflow-0.4.0.dev0/launchflow/cli/gen/templates/django/_postgres_template/app/views.py.jinja`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev8/launchflow/cli/gen/templates/django/_postgres_template/django_app/settings.py.jinja` & `launchflow-0.4.0.dev0/launchflow/cli/gen/templates/django/_postgres_template/django_app/settings.py.jinja`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 import os
-{% for infra_import in app_infra_imports %}
-{{ infra_import }}
+
+{% for infra_import in app_infra_imports %}{{ infra_import }}
 {% endfor %}
 {{ app_django_settings }}
+
 BASE_DIR = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
 
+# TODO(developer): Replace this with your own secret key
 SECRET_KEY = "your_secret_key"
 
-DEBUG = True
-
-ALLOWED_HOSTS = ["*"]
-
 INSTALLED_APPS = [
     "django.contrib.admin",
     "django.contrib.auth",
     "django.contrib.contenttypes",
     "django.contrib.sessions",
     "django.contrib.messages",
     "django.contrib.staticfiles",
@@ -27,14 +25,15 @@
     "django.middleware.security.SecurityMiddleware",
     "django.contrib.sessions.middleware.SessionMiddleware",
     "django.middleware.common.CommonMiddleware",
     "django.middleware.csrf.CsrfViewMiddleware",
     "django.contrib.auth.middleware.AuthenticationMiddleware",
     "django.contrib.messages.middleware.MessageMiddleware",
     "django.middleware.clickjacking.XFrameOptionsMiddleware",
+    "django_app.middleware.HealthCheckMiddleware",
 ]
 
 ROOT_URLCONF = "django_app.urls"
 
 TEMPLATES = [
     {
         "BACKEND": "django.template.backends.django.DjangoTemplates",
```

### Comparing `launchflow-0.3.9.dev8/launchflow/cli/gen/templates/django/_postgres_template/manage.py.jinja` & `launchflow-0.4.0.dev0/launchflow/cli/gen/templates/django/_postgres_template/manage.py.jinja`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev8/launchflow/cli/gen/templates/django/_simple_template/Dockerfile.jinja` & `launchflow-0.4.0.dev0/launchflow/cli/gen/templates/django/_simple_template/Dockerfile.jinja`

 * *Files 9% similar despite different names*

```diff
@@ -34,15 +34,14 @@
 COPY --from=builder /install /usr/local/lib/python{{ python_major_version }}.{{ python_minor_version }}/site-packages
 ENV PATH="${PATH}:/usr/local/lib/python{{ python_major_version }}.{{ python_minor_version }}/site-packages/bin"
 
 # Set the working directory and copy only the necessary application files
 WORKDIR /code
 COPY --chown=appuser:appuser ./app /code/app
 COPY --chown=appuser:appuser ./django_app /code/django_app
-COPY --chown=appuser:appuser ./launchflow.yaml /code/launchflow.yaml
 COPY --chown=appuser:appuser ./manage.py /code/manage.py
 
 # Expose the port the app runs on
 EXPOSE $PORT
 
 # Start the application
 CMD exec gunicorn --bind 0.0.0.0:$PORT --workers 1 --threads 8 --timeout 0 django_app.wsgi:application
```

### Comparing `launchflow-0.3.9.dev8/launchflow/cli/gen/templates/django/_simple_template/README.md.jinja` & `launchflow-0.4.0.dev0/launchflow/cli/gen/templates/django/_simple_template/README.md.jinja`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 ```
 
 ## 🏃 Run your Application (local)
 
 Run the Django application locally using [Django's Development Server](https://docs.djangoproject.com/en/5.0/intro/tutorial01/#the-development-server).
 
 ```bash
-python manage.py runserver 0.0.0.0:8000
+python manage.py runserver 127.0.0.1:8000
 ```
 
 #### NOTE: The Django Development Server is not suitable for production.
 #### The `Dockerfile` and `launchflow deploy` command uses [Gunicorn](https://gunicorn.org/) instead.
 
 ## 🚀 Deploy your Application (remote)
 
@@ -103,8 +103,8 @@
 
 Automatically <strong>delete</strong> all infrastructure associated with your application.
 
 ```bash
 launchflow destroy
 ```
 
-Learn how this command works in the [LaunchFlow Docs](https://docs.launchflow.com/reference/cli#launchflow-destroy).
+Learn how this command works in the [LaunchFlow Docs](https://docs.launchflow.com/reference/cli#launchflow-destroy).
```

### Comparing `launchflow-0.3.9.dev8/launchflow/cli/gen/templates/django/_simple_template/django_app/settings.py.jinja` & `launchflow-0.4.0.dev0/launchflow/cli/gen/templates/django/_simple_template/django_app/settings.py.jinja`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 import os
-{% for infra_import in app_infra_imports %}
-{{ infra_import }}
+
+{% for infra_import in app_infra_imports %}{{ infra_import }}
 {% endfor %}
 {{ app_django_settings }}
+
 BASE_DIR = os.path.dirname(os.path.dirname(os.path.abspath(__file__)))
 
+# TODO(developer): Replace this with your own secret key
 SECRET_KEY = "your_secret_key"
 
-DEBUG = True
-
-ALLOWED_HOSTS = ["*"]
-
 INSTALLED_APPS = [
     "django.contrib.admin",
     "django.contrib.auth",
     "django.contrib.contenttypes",
     "django.contrib.sessions",
     "django.contrib.messages",
     "django.contrib.staticfiles",
@@ -27,14 +25,15 @@
     "django.middleware.security.SecurityMiddleware",
     "django.contrib.sessions.middleware.SessionMiddleware",
     "django.middleware.common.CommonMiddleware",
     "django.middleware.csrf.CsrfViewMiddleware",
     "django.contrib.auth.middleware.AuthenticationMiddleware",
     "django.contrib.messages.middleware.MessageMiddleware",
     "django.middleware.clickjacking.XFrameOptionsMiddleware",
+    "django_app.middleware.HealthCheckMiddleware",
 ]
 
 ROOT_URLCONF = "django_app.urls"
 
 TEMPLATES = [
     {
         "BACKEND": "django.template.backends.django.DjangoTemplates",
```

### Comparing `launchflow-0.3.9.dev8/launchflow/cli/gen/templates/django/_simple_template/manage.py.jinja` & `launchflow-0.4.0.dev0/launchflow/cli/gen/templates/django/_simple_template/manage.py.jinja`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev8/launchflow/cli/gen/templates/django/django_template.py` & `launchflow-0.4.0.dev0/launchflow/cli/gen/templates/django/django_template.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import datetime
 import sys
 from dataclasses import dataclass
 from typing import List, Literal, Optional, Type
 
+from launchflow import Resource
+from launchflow.aws.elasticache import ElasticacheRedis
 from launchflow.aws.rds import RDSPostgres
 from launchflow.aws.s3 import S3Bucket
 from launchflow.cli.gen.template import ProjectGenerator
 from launchflow.gcp.cloudsql import CloudSQLPostgres
 from launchflow.gcp.compute_engine import ComputeEngineRedis
 from launchflow.gcp.gcs import GCSBucket
 from launchflow.gcp.memorystore import MemorystoreRedis
 
-from launchflow import Resource
-
 
 @dataclass
 class ResourceInfo:
     infra_docs_url: str
     infra_name: str
     infra_lf_class: str
     django_settings: Optional[str]
@@ -26,15 +26,15 @@
     requirements: List[str]
     installed_app: Optional[str]
 
 
 resource_type_to_resource_info_kwargs = {
     # GCP Compute Engine Redis
     ComputeEngineRedis: {
-        "infra_docs_url": "https://docs.launchflow.com/reference/gcp-resources/compute-engine",
+        "infra_docs_url": "https://docs.launchflow.com/reference/gcp-resources/compute-engine#compute-engine-redis",
         "infra_name": "redis_vm",
         "infra_lf_class": "lf.gcp.ComputeEngineRedis",
         "django_settings": """CACHES = {
     "default": redis_vm.django_settings(),
 }
 """,
         "views_imports": "from django.core.cache import cache",
@@ -50,19 +50,19 @@
 """,
         "django_test_endpoint_url": 'path("test_redis/<key>", views.test_redis),',
         "requirements": ["redis>=4.2.0"],
         "installed_app": None,
     },
     # GCP Memorystore Redis
     MemorystoreRedis: {
-        "infra_docs_url": "https://docs.launchflow.com/reference/gcp-resources/memorystore-redis",
-        "infra_name": "redis_cluster",
+        "infra_docs_url": "https://docs.launchflow.com/reference/gcp-resources/memorystore",
+        "infra_name": "memorystore",
         "infra_lf_class": "lf.gcp.MemorystoreRedis",
         "django_settings": """CACHES = {
-    "default": redis_cluster.django_settings(),
+    "default": memorystore.django_settings(),
 }
 """,
         "views_imports": "from django.core.cache import cache",
         "django_test_endpoint": """
 # NOTE: This should normally use a POST request since it's modifying state, but we're
 # using GET so you can easily test it in your browser.
 @api_view(["GET"])
@@ -86,15 +86,15 @@
         "BACKEND": "storages.backends.gcloud.GoogleCloudStorage",
     },
     "staticfiles": {
         "BACKEND": "storages.backends.gcloud.GoogleCloudStorage",
     },
 }
 GS_BUCKET_NAME = gcs_bucket.connect().bucket_name
-GS_CREDENTIALS = get_service_account_credentials()
+GS_CREDENTIALS = lf.gcp.get_service_account_credentials()
 """,
         "views_imports": "from django.core.files.storage import default_storage",
         "django_test_endpoint": """
 # NOTE: This should normally use a POST request since it's modifying state, but we're
 # using GET so you can easily test it in your browser.
 @api_view(["GET"])
 def test_gcs(request, object_name):
@@ -152,17 +152,41 @@
     with default_storage.open(object_name, "r") as file:
         return Response({"message": file.read()})
 """,
         "django_test_endpoint_url": 'path("test_s3/<object_name>", views.test_s3),',
         "requirements": ["django-storages[s3]"],
         "installed_app": "storages",
     },
+    # AWS Elasticache Redis
+    ElasticacheRedis: {
+        "infra_docs_url": "https://docs.launchflow.com/reference/aws-resources/elasticache-redis",
+        "infra_name": "elasticache",
+        "infra_lf_class": "lf.aws.ElasticacheRedis",
+        "django_settings": """CACHES = {
+    "default": elasticache.django_settings(),
+}
+""",
+        "views_imports": "from django.core.cache import cache",
+        "django_test_endpoint": """
+# NOTE: This should normally use a POST request since it's modifying state, but we're
+# using GET so you can easily test it in your browser.
+@api_view(["GET"])
+def test_redis(request, key):
+    # Write to cache (Redis)
+    cache.set(key, "Hello from Redis!", timeout=60)
+    # Immediately read from cache to verify write
+    return Response({"message": cache.get(key)})
+""",
+        "django_test_endpoint_url": 'path("test_redis/<key>", views.test_redis),',
+        "requirements": ["redis>=4.2.0"],
+        "installed_app": None,
+    },
     # AWS RDS (Postgres)
     RDSPostgres: {
-        "infra_docs_url": "https://docs.launchflow.com/reference/aws-resources/rds",
+        "infra_docs_url": "https://docs.launchflow.com/reference/aws-resources/rds-postgres",
         "infra_name": "postgres",
         "infra_lf_class": "lf.aws.RDSPostgres",
         "views_imports": None,
         "django_settings": """DATABASES = {
     "default": postgres.django_settings(),
 }
 """,
@@ -246,23 +270,19 @@
 
     # Used by django_app/settings.py
     @property
     def app_infra_imports(self) -> List[str]:
         # TODO: Clean this up so that each import is added separately then sort the
         # whole list at the end
         if len(self.resources) == 0:
-            return []
-        to_return = []
+            return ["import launchflow as lf"]
+        to_return = ["import launchflow as lf"]
         infra_names = []
 
         for resource in self.resources:
-            if resource == GCSBucket:
-                to_return.append(
-                    "from launchflow.gcp import get_service_account_credentials"
-                )
             resource_info = get_resource_info(resource)
             infra_names.append(resource_info.infra_name)
 
         if len(infra_names) == 0:
             return to_return
 
         to_return.append(
@@ -274,14 +294,44 @@
     @property
     def app_django_settings(self) -> str:
         lines = []
         for resource in self.resources:
             resource_info = get_resource_info(resource)
             if resource_info.django_settings is not None:
                 lines.append(resource_info.django_settings)
+
+        if self.cloud_provider == "gcp":
+            lines.extend(
+                [
+                    "if lf.is_deployment():",
+                    '    ALLOWED_HOSTS = ["*"]',
+                    "    # TODO(developer): Replace this with your domain",
+                    '    CSRF_TRUSTED_ORIGINS = ["https://*.run.app"]',
+                    "    SECURE_SSL_REDIRECT = True",
+                    '    SECURE_PROXY_SSL_HEADER = ("HTTP_X_FORWARDED_PROTO", "https")',
+                    "else:",
+                    '    ALLOWED_HOSTS = ["*"]',
+                    "    DEBUG = True",
+                ]
+            )
+        elif self.cloud_provider == "aws":
+            lines.extend(
+                [
+                    "if lf.is_deployment():",
+                    '    ALLOWED_HOSTS = ["*"]',
+                    "    # TODO(developer): Replace this with your domain's HTTPS URL",
+                    '    CSRF_TRUSTED_ORIGINS = ["http://*.amazonaws.com"]',
+                    # TODO: Add this once AWS services have HTTPS support
+                    # "    SECURE_SSL_REDIRECT = True",
+                    # "    SECURE_PROXY_SSL_HEADER = ("HTTP_X_FORWARDED_PROTO", "https")",
+                    "else:",
+                    '    ALLOWED_HOSTS = ["*"]',
+                    "    DEBUG = True",
+                ]
+            )
         return "\n".join(lines)
 
     # Used by django_app/settings.py
     @property
     def app_installed_apps(self) -> List[str]:
         installed_apps = []
         for resource in self.resources:
@@ -334,20 +384,24 @@
     def launchflow_service_product(self) -> str:
         if self.cloud_provider == "aws":
             return "aws_ecs_fargate"
         elif self.cloud_provider == "gcp":
             return "gcp_cloud_run"
         raise ValueError(f"Unsupported cloud provider: {self.cloud_provider}")
 
-    def template_directory(self) -> str:
+    def template_path_info(self) -> str:
+        template_dir = "launchflow.cli.gen.templates.django"
+        template_name = "_simple_template"
+
         if CloudSQLPostgres in [
             resource for resource in self.resources
         ] or RDSPostgres in [resource for resource in self.resources]:
-            return "launchflow.cli.gen.templates.django._postgres_template"
-        return "launchflow.cli.gen.templates.django._simple_template"
+            template_name = "_postgres_template"
+
+        return template_dir, template_name
 
     @property
     def docker_repository_prefix(self) -> str:
         if self.cloud_provider == "aws":
             return "public.ecr.aws/docker/library/"
         return ""
 
@@ -378,23 +432,23 @@
             "app_infra_urls": self.app_infra_urls,
             # app/views.py
             "app_infra_endpoints": self.app_infra_endpoints,
             "app_views_imports": self.app_views_imports,
         }
 
 
-if __name__ == "__main__":
-    cloud_provider = "gcp"
-    generator = DjangoProjectGenerator(
-        resources=[
-            ComputeEngineRedis,
-            GCSBucket,
-            CloudSQLPostgres,
-            # S3Bucket,
-            # RDSPostgres,
-        ],
-        cloud_provider=cloud_provider,
-        launchflow_project_name=f"{cloud_provider}-examples",
-        launchflow_environment_name="dev",
-        launchflow_service_name="django-service",
-    )
-    generator.generate_project(destination_path="/tmp/launchflow")
+# if __name__ == "__main__":
+#     cloud_provider = "gcp"
+#     generator = DjangoProjectGenerator(
+#         resources=[
+#             ComputeEngineRedis,
+#             GCSBucket,
+#             CloudSQLPostgres,
+#             # S3Bucket,
+#             # RDSPostgres,
+#         ],
+#         cloud_provider=cloud_provider,
+#         launchflow_project_name=f"{cloud_provider}-examples",
+#         launchflow_environment_name="dev",
+#         launchflow_service_name="django-service",
+#     )
+#     generator.generate_project(destination_path="/tmp/launchflow")
```

### Comparing `launchflow-0.3.9.dev8/launchflow/cli/gen/templates/fastapi/__pycache__/fastapi_template.cpython-311.pyc` & `launchflow-0.4.0.dev0/launchflow/cli/gen/templates/fastapi/__pycache__/fastapi_template.cpython-311.pyc`

 * *Files 10% similar despite different names*

#### Python bytecode

```diff
@@ -1,35 +1,33 @@
 magic:    0xa70d0d0a
-moddate:  0x07430f66 (Fri Apr  5 00:17:11 2024 UTC)
-files sz: 18560
+moddate:  0x972d4666 (Thu May 16 16:00:23 2024 UTC)
+files sz: 19725
 code
    argcount  : 0
    nlocals   : 0
-   stacksize : 22
+   stacksize : 24
    flags     : 0
    code
       0x9700640064016c005a00640064026c016d025a020100640064036c036d
       045a046d055a056d065a066d075a070100640064046c086d095a09010064
       0064056c0a6d0b5a0b0100640064066c0c6d0d5a0d0100640064076c0e6d
       0f5a0f0100640064086c106d115a110100640064096c126d135a13010064
-      00640a6c146d155a1501006400640b6c166d175a17010065020200470064
-      0c8400640da6020000ab020000000000000000a6000000ab000000000000
-      0000005a186511640e640f64106411641264016401670064136414670164
-      159c0a65156416641764186411641264016401670064196414670164159c
-      0a6513641a641b641c64116401640164016700641d670064159c0a650f64
-      1e641f642064216422642364246425670264266427642864296702642a9c
-      0a650b642b642c642d64116411640164016700642e670064159c0a650964
-      2f641f643064216422642364246425670264266427642864296702642a9c
-      0a69065a1964316507651719000000000000000000643265186604643384
-      045a1a650202004700643484006435650da6030000ab0300000000000000
-      00a6000000ab0000000000000000005a1b651c64366b0200000000723064
-      375a1d0200651b65116513650f6703651d651d9b0064389d026439643aac
-      3ba6050000ab0500000000000000005a1e651ea01f000000000000000000
-      0000000000000000000000643cac3da6010000ab01000000000000000001
-      006401530064015300
+      00640a6c146d155a1501006400640b6c166d175a1701006400640c6c186d
+      195a190100650202004700640d8400640ea6020000ab0200000000000000
+      00a6000000ab0000000000000000005a1a6515640f641064116412641364
+      016401670064146415670164169c0a651964176418641964126413640164
+      016700641a6415670164169c0a6517641b641c641d641264016401640167
+      00641e670064169c0a6513641f6420642164226423642464256426670264
+      2764286429642a6702642b9c0a650f642c642d642e641264126401640167
+      00642f670064169c0a650b64306431643264126413640164016700643364
+      15670164169c0a650d643464206435642264236424642564266702642764
+      286429642a6702642b9c0a69075a1b643665076509190000000000000000
+      006437651a6604643884045a1c65020200470064398400643a6511a60300
+      00ab030000000000000000a6000000ab0000000000000000005a1d640153
+      00
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (None)
                  6 IMPORT_NAME              0 (sys)
                  8 STORE_NAME               0 (sys)
    
@@ -50,338 +48,326 @@
                 36 IMPORT_FROM              6 (Optional)
                 38 STORE_NAME               6 (Optional)
                 40 IMPORT_FROM              7 (Type)
                 42 STORE_NAME               7 (Type)
                 44 POP_TOP
    
      5          46 LOAD_CONST               0 (0)
-                48 LOAD_CONST               4 (('RDSPostgres',))
-                50 IMPORT_NAME              8 (launchflow.aws.rds)
-                52 IMPORT_FROM              9 (RDSPostgres)
-                54 STORE_NAME               9 (RDSPostgres)
+                48 LOAD_CONST               4 (('Resource',))
+                50 IMPORT_NAME              8 (launchflow)
+                52 IMPORT_FROM              9 (Resource)
+                54 STORE_NAME               9 (Resource)
                 56 POP_TOP
    
      6          58 LOAD_CONST               0 (0)
-                60 LOAD_CONST               5 (('S3Bucket',))
-                62 IMPORT_NAME             10 (launchflow.aws.s3)
-                64 IMPORT_FROM             11 (S3Bucket)
-                66 STORE_NAME              11 (S3Bucket)
+                60 LOAD_CONST               5 (('ElasticacheRedis',))
+                62 IMPORT_NAME             10 (launchflow.aws.elasticache)
+                64 IMPORT_FROM             11 (ElasticacheRedis)
+                66 STORE_NAME              11 (ElasticacheRedis)
                 68 POP_TOP
    
      7          70 LOAD_CONST               0 (0)
-                72 LOAD_CONST               6 (('ProjectGenerator',))
-                74 IMPORT_NAME             12 (launchflow.cli.gen.template)
-                76 IMPORT_FROM             13 (ProjectGenerator)
-                78 STORE_NAME              13 (ProjectGenerator)
+                72 LOAD_CONST               6 (('RDSPostgres',))
+                74 IMPORT_NAME             12 (launchflow.aws.rds)
+                76 IMPORT_FROM             13 (RDSPostgres)
+                78 STORE_NAME              13 (RDSPostgres)
                 80 POP_TOP
    
      8          82 LOAD_CONST               0 (0)
-                84 LOAD_CONST               7 (('CloudSQLPostgres',))
-                86 IMPORT_NAME             14 (launchflow.gcp.cloudsql)
-                88 IMPORT_FROM             15 (CloudSQLPostgres)
-                90 STORE_NAME              15 (CloudSQLPostgres)
+                84 LOAD_CONST               7 (('S3Bucket',))
+                86 IMPORT_NAME             14 (launchflow.aws.s3)
+                88 IMPORT_FROM             15 (S3Bucket)
+                90 STORE_NAME              15 (S3Bucket)
                 92 POP_TOP
    
      9          94 LOAD_CONST               0 (0)
-                96 LOAD_CONST               8 (('ComputeEngineRedis',))
-                98 IMPORT_NAME             16 (launchflow.gcp.compute_engine)
-               100 IMPORT_FROM             17 (ComputeEngineRedis)
-               102 STORE_NAME              17 (ComputeEngineRedis)
+                96 LOAD_CONST               8 (('ProjectGenerator',))
+                98 IMPORT_NAME             16 (launchflow.cli.gen.template)
+               100 IMPORT_FROM             17 (ProjectGenerator)
+               102 STORE_NAME              17 (ProjectGenerator)
                104 POP_TOP
    
     10         106 LOAD_CONST               0 (0)
-               108 LOAD_CONST               9 (('GCSBucket',))
-               110 IMPORT_NAME             18 (launchflow.gcp.gcs)
-               112 IMPORT_FROM             19 (GCSBucket)
-               114 STORE_NAME              19 (GCSBucket)
+               108 LOAD_CONST               9 (('CloudSQLPostgres',))
+               110 IMPORT_NAME             18 (launchflow.gcp.cloudsql)
+               112 IMPORT_FROM             19 (CloudSQLPostgres)
+               114 STORE_NAME              19 (CloudSQLPostgres)
                116 POP_TOP
    
     11         118 LOAD_CONST               0 (0)
-               120 LOAD_CONST              10 (('MemorystoreRedis',))
-               122 IMPORT_NAME             20 (launchflow.gcp.memorystore)
-               124 IMPORT_FROM             21 (MemorystoreRedis)
-               126 STORE_NAME              21 (MemorystoreRedis)
+               120 LOAD_CONST              10 (('ComputeEngineRedis',))
+               122 IMPORT_NAME             20 (launchflow.gcp.compute_engine)
+               124 IMPORT_FROM             21 (ComputeEngineRedis)
+               126 STORE_NAME              21 (ComputeEngineRedis)
                128 POP_TOP
    
-    13         130 LOAD_CONST               0 (0)
-               132 LOAD_CONST              11 (('Resource',))
-               134 IMPORT_NAME             22 (launchflow)
-               136 IMPORT_FROM             23 (Resource)
-               138 STORE_NAME              23 (Resource)
+    12         130 LOAD_CONST               0 (0)
+               132 LOAD_CONST              11 (('GCSBucket',))
+               134 IMPORT_NAME             22 (launchflow.gcp.gcs)
+               136 IMPORT_FROM             23 (GCSBucket)
+               138 STORE_NAME              23 (GCSBucket)
                140 POP_TOP
    
-    16         142 LOAD_NAME                2 (dataclass)
+    13         142 LOAD_CONST               0 (0)
+               144 LOAD_CONST              12 (('MemorystoreRedis',))
+               146 IMPORT_NAME             24 (launchflow.gcp.memorystore)
+               148 IMPORT_FROM             25 (MemorystoreRedis)
+               150 STORE_NAME              25 (MemorystoreRedis)
+               152 POP_TOP
    
-    17         144 PUSH_NULL
-               146 LOAD_BUILD_CLASS
-               148 LOAD_CONST              12 (<code object ResourceInfo, file "/home/tanke/launchflow/launchflow/clients/python/launchflow/launchflow/cli/gen/templates/fastapi/fastapi_template.py", line 16>)
-               150 MAKE_FUNCTION            0
-               152 LOAD_CONST              13 ('ResourceInfo')
-               154 PRECALL                  2
-               158 CALL                     2
+    16         154 LOAD_NAME                2 (dataclass)
    
-    16         168 PRECALL                  0
-               172 CALL                     0
+    17         156 PUSH_NULL
+               158 LOAD_BUILD_CLASS
+               160 LOAD_CONST              13 (<code object ResourceInfo, file "/Users/calebvandyke/code/launchflow-oss/launchflow/cli/gen/templates/fastapi/fastapi_template.py", line 16>)
+               162 MAKE_FUNCTION            0
+               164 LOAD_CONST              14 ('ResourceInfo')
+               166 PRECALL                  2
+               170 CALL                     2
    
-    17         182 STORE_NAME              24 (ResourceInfo)
+    16         180 PRECALL                  0
+               184 CALL                     0
    
-    32         184 LOAD_NAME               17 (ComputeEngineRedis)
+    17         194 STORE_NAME              26 (ResourceInfo)
    
-    33         186 LOAD_CONST              14 ('https://docs.launchflow.com/reference/gcp-resources/compute-engine')
+    32         196 LOAD_NAME               21 (ComputeEngineRedis)
    
-    34         188 LOAD_CONST              15 ('redis_vm')
+    33         198 LOAD_CONST              15 ('https://docs.launchflow.com/reference/gcp-resources/compute-engine#compute-engine-redis')
    
-    35         190 LOAD_CONST              16 ('lf.gcp.ComputeEngineRedis')
+    34         200 LOAD_CONST              16 ('redis_vm')
    
-    36         192 LOAD_CONST              17 ('')
+    35         202 LOAD_CONST              17 ('lf.gcp.ComputeEngineRedis')
    
-    37         194 LOAD_CONST              18 ('from redis.asyncio import Redis')
+    36         204 LOAD_CONST              18 ('')
    
-    38         196 LOAD_CONST               1 (None)
+    37         206 LOAD_CONST              19 ('from redis.asyncio import Redis')
    
-    39         198 LOAD_CONST               1 (None)
+    38         208 LOAD_CONST               1 (None)
    
-    40         200 BUILD_LIST               0
+    39         210 LOAD_CONST               1 (None)
    
-    41         202 LOAD_CONST              19 ('\n@app.post("/test_redis/{key}")\nasync def test_redis(\n    key: str, value: str, redis_client: Redis = Depends(redis_vm.redis_async)\n):\n    # Write to Redis\n    await redis_client.set(key, value)\n    # Immediately read from Redis to verify the write\n    value = await redis_client.get(key)\n    return {"message": f"Set {key} to {value}"}\n')
+    40         212 BUILD_LIST               0
    
-    52         204 LOAD_CONST              20 ('redis>=4.2.0')
-               206 BUILD_LIST               1
+    41         214 LOAD_CONST              20 ('\n@app.post("/test_redis/{key}")\nasync def test_redis(\n    key: str, value: str, redis_client: Redis = Depends(redis_vm.redis_async)\n):\n    # Write to Redis\n    await redis_client.set(key, value)\n    # Immediately read from Redis to verify the write\n    value = await redis_client.get(key)\n    return {"message": f"Set {key} to {value}"}\n')
    
-    32         208 LOAD_CONST              21 (('infra_docs_url', 'infra_name', 'infra_lf_class', 'launchflow_imports', 'infra_import', 'global_setup', 'fastapi_setup', 'app_imports', 'fastapi_test_endpoint', 'requirements'))
-               210 BUILD_CONST_KEY_MAP     10
+    52         216 LOAD_CONST              21 ('redis>=4.2.0')
+               218 BUILD_LIST               1
    
-    55         212 LOAD_NAME               21 (MemorystoreRedis)
+    32         220 LOAD_CONST              22 (('infra_docs_url', 'infra_name', 'infra_lf_class', 'launchflow_imports', 'infra_import', 'global_setup', 'fastapi_setup', 'app_imports', 'fastapi_test_endpoint', 'requirements'))
+               222 BUILD_CONST_KEY_MAP     10
    
-    56         214 LOAD_CONST              22 ('https://docs.launchflow.com/reference/gcp-resources/memorystore-redis')
+    55         224 LOAD_NAME               25 (MemorystoreRedis)
    
-    57         216 LOAD_CONST              23 ('redis_cluster')
+    56         226 LOAD_CONST              23 ('https://docs.launchflow.com/reference/gcp-resources/memorystore')
    
-    58         218 LOAD_CONST              24 ('lf.gcp.MemorystoreRedis')
+    57         228 LOAD_CONST              24 ('memorystore')
    
-    59         220 LOAD_CONST              17 ('')
+    58         230 LOAD_CONST              25 ('lf.gcp.MemorystoreRedis')
    
-    60         222 LOAD_CONST              18 ('from redis.asyncio import Redis')
+    59         232 LOAD_CONST              18 ('')
    
-    61         224 LOAD_CONST               1 (None)
+    60         234 LOAD_CONST              19 ('from redis.asyncio import Redis')
    
-    62         226 LOAD_CONST               1 (None)
+    61         236 LOAD_CONST               1 (None)
    
-    63         228 BUILD_LIST               0
+    62         238 LOAD_CONST               1 (None)
    
-    64         230 LOAD_CONST              25 ('\n@app.post("/test_redis/{key}")\nasync def test_redis(\n    key: str, value: str, redis_client: Redis = Depends(redis_cluster.redis_async)\n):\n    # Write to Redis\n    await redis_client.set(key, value)\n    # Immediately read from Redis to verify the write\n    value = await redis_client.get(key)\n    return {"message": f"Set {key} to {value}"}\n')
+    63         240 BUILD_LIST               0
    
-    75         232 LOAD_CONST              20 ('redis>=4.2.0')
-               234 BUILD_LIST               1
+    64         242 LOAD_CONST              26 ('\n@app.post("/test_redis/{key}")\nasync def test_redis(\n    key: str, value: str, redis_client: Redis = Depends(memorystore.redis_async)\n):\n    # Write to Redis\n    await redis_client.set(key, value)\n    # Immediately read from Redis to verify the write\n    value = await redis_client.get(key)\n    return {"message": f"Set {key} to {value}"}\n')
    
-    55         236 LOAD_CONST              21 (('infra_docs_url', 'infra_name', 'infra_lf_class', 'launchflow_imports', 'infra_import', 'global_setup', 'fastapi_setup', 'app_imports', 'fastapi_test_endpoint', 'requirements'))
-               238 BUILD_CONST_KEY_MAP     10
+    75         244 LOAD_CONST              21 ('redis>=4.2.0')
+               246 BUILD_LIST               1
    
-    78         240 LOAD_NAME               19 (GCSBucket)
+    55         248 LOAD_CONST              22 (('infra_docs_url', 'infra_name', 'infra_lf_class', 'launchflow_imports', 'infra_import', 'global_setup', 'fastapi_setup', 'app_imports', 'fastapi_test_endpoint', 'requirements'))
+               250 BUILD_CONST_KEY_MAP     10
    
-    79         242 LOAD_CONST              26 ('https://docs.launchflow.com/reference/gcp-resources/gcs-bucket')
+    78         252 LOAD_NAME               23 (GCSBucket)
    
-    80         244 LOAD_CONST              27 ('gcs_bucket')
+    79         254 LOAD_CONST              27 ('https://docs.launchflow.com/reference/gcp-resources/gcs-bucket')
    
-    81         246 LOAD_CONST              28 ('lf.gcp.GCSBucket')
+    80         256 LOAD_CONST              28 ('gcs_bucket')
    
-    82         248 LOAD_CONST              17 ('')
+    81         258 LOAD_CONST              29 ('lf.gcp.GCSBucket')
    
-    83         250 LOAD_CONST               1 (None)
+    82         260 LOAD_CONST              18 ('')
    
-    84         252 LOAD_CONST               1 (None)
+    83         262 LOAD_CONST               1 (None)
    
-    85         254 LOAD_CONST               1 (None)
+    84         264 LOAD_CONST               1 (None)
    
-    86         256 BUILD_LIST               0
+    85         266 LOAD_CONST               1 (None)
    
-    87         258 LOAD_CONST              29 ('\n# This endpoint uploads a file to GCS and reads it back to verify the bucket works\n@app.post("/test_gcs/{object_name}")\nasync def test_gcs(object_name: str):\n    # Write to GCS\n    gcs_bucket.upload_from_string("Hello, World!", object_name)\n    # Immediately read from GCS to verify the write\n    gcs_bucket.download_file(object_name).decode("utf-8")\n    return {"message": f"Uploaded {object_name} to GCS"}\n')
+    86         268 BUILD_LIST               0
    
-    97         260 BUILD_LIST               0
+    87         270 LOAD_CONST              30 ('\n# This endpoint uploads a file to GCS and reads it back to verify the bucket works\n@app.post("/test_gcs/{object_name}")\nasync def test_gcs(object_name: str):\n    # Write to GCS\n    gcs_bucket.upload_from_string("Hello, World!", object_name)\n    # Immediately read from GCS to verify the write\n    gcs_bucket.download_file(object_name).decode("utf-8")\n    return {"message": f"Uploaded {object_name} to GCS"}\n')
    
-    78         262 LOAD_CONST              21 (('infra_docs_url', 'infra_name', 'infra_lf_class', 'launchflow_imports', 'infra_import', 'global_setup', 'fastapi_setup', 'app_imports', 'fastapi_test_endpoint', 'requirements'))
-               264 BUILD_CONST_KEY_MAP     10
+    97         272 BUILD_LIST               0
    
-   100         266 LOAD_NAME               15 (CloudSQLPostgres)
+    78         274 LOAD_CONST              22 (('infra_docs_url', 'infra_name', 'infra_lf_class', 'launchflow_imports', 'infra_import', 'global_setup', 'fastapi_setup', 'app_imports', 'fastapi_test_endpoint', 'requirements'))
+               276 BUILD_CONST_KEY_MAP     10
    
-   101         268 LOAD_CONST              30 ('https://docs.launchflow.com/reference/gcp-resources/cloud-sql')
+   100         278 LOAD_NAME               19 (CloudSQLPostgres)
    
-   102         270 LOAD_CONST              31 ('postgres')
+   101         280 LOAD_CONST              31 ('https://docs.launchflow.com/reference/gcp-resources/cloud-sql')
    
-   103         272 LOAD_CONST              32 ('lf.gcp.CloudSQLPostgres')
+   102         282 LOAD_CONST              32 ('postgres')
    
-   104         274 LOAD_CONST              33 ('from launchflow.fastapi import sqlalchemy_async_depends')
+   103         284 LOAD_CONST              33 ('lf.gcp.CloudSQLPostgres')
    
-   105         276 LOAD_CONST              34 ('from sqlalchemy import select\nfrom sqlalchemy.ext.asyncio import AsyncSession\n')
+   104         286 LOAD_CONST              34 ('from launchflow.fastapi import sqlalchemy_async_depends')
    
-   108         278 LOAD_CONST              35 ('# Create the global FastAPI dependency for the SQLAlchemy async session\nasync_session = sqlalchemy_async_depends()')
+   105         288 LOAD_CONST              35 ('from sqlalchemy import select\nfrom sqlalchemy.ext.asyncio import AsyncSession\n')
    
-   111         280 LOAD_CONST              36 ('from app.models import Base, StorageUser')
+   108         290 LOAD_CONST              36 ('# Create the global FastAPI dependency for the SQLAlchemy async session\nasync_session = sqlalchemy_async_depends()')
    
-   112         282 LOAD_CONST              37 ('from app.schemas import ListUsersResponse, UserResponse')
+   111         292 LOAD_CONST              37 ('from app.models import Base, StorageUser')
    
-   110         284 BUILD_LIST               2
+   112         294 LOAD_CONST              38 ('from app.schemas import ListUsersResponse, UserResponse')
    
-   114         286 LOAD_CONST              38 ('    # Create the SQLAlchemy async engine (connection pool)\n    engine = await postgres.sqlalchemy_async_engine()\n    # Create the database tables using the engine\n    async with engine.begin() as conn:\n        await conn.run_sync(Base.metadata.create_all)\n    # Set up the FastAPI dependency\n    async_session.setup(engine)')
+   110         296 BUILD_LIST               2
    
-   121         288 LOAD_CONST              39 ('\n"""\nThe endpoints below define a simple CRUD API for a generic StorageUser model.\n\nThe StorageUser model is defined in app.models\nThe ListUsersResponse and UserResponse schemas are defined in app.schemas.\n"""\n\n@app.get("/users")\nasync def list_users(db: AsyncSession = Depends(async_session)):\n    storage_users = (await db.execute(select(StorageUser))).scalars().all()\n    return ListUsersResponse.from_storage(storage_users)\n\n\n@app.post("/users")\nasync def create_user(email: str, name: str, db: AsyncSession = Depends(async_session)):\n    storage_user = StorageUser(email=email, name=name)\n    db.add(storage_user)\n    await db.commit()\n    return UserResponse.from_storage(storage_user)\n\n\n@app.get("/users/{user_id}")\nasync def read_user(user_id: int, db: AsyncSession = Depends(async_session)):\n    storage_user = await db.get(StorageUser, user_id)\n    if storage_user is None:\n        raise HTTPException(status_code=404, detail="User not found")\n    return UserResponse.from_storage(storage_user)\n\n\n@app.put("/users/{user_id}")\nasync def update_user(\n    user_id: int, name: str, db: AsyncSession = Depends(async_session)\n):\n    storage_user = await db.get(StorageUser, user_id)\n    if storage_user is None:\n        raise HTTPException(status_code=404, detail="User not found")\n    storage_user.name = name\n    await db.commit()\n    return UserResponse.from_storage(storage_user)\n\n\n@app.delete("/users/{user_id}")\nasync def delete_user(user_id: int, db: AsyncSession = Depends(async_session)):\n    storage_user = await db.get(StorageUser, user_id)\n    if storage_user is None:\n        raise HTTPException(status_code=404, detail="User not found")\n    await db.delete(storage_user)\n    await db.commit()\n    return UserResponse.from_storage(storage_user)\n')
+   114         298 LOAD_CONST              39 ('    # Create the SQLAlchemy async engine (connection pool)\n    engine = await postgres.sqlalchemy_async_engine()\n    # Create the database tables using the engine\n    async with engine.begin() as conn:\n        await conn.run_sync(Base.metadata.create_all)\n    # Set up the FastAPI dependency\n    async_session.setup(engine)')
    
-   172         290 LOAD_CONST              40 ('sqlalchemy[async]')
-               292 LOAD_CONST              41 ('asyncpg')
-               294 BUILD_LIST               2
+   121         300 LOAD_CONST              40 ('\n"""\nThe endpoints below define a simple CRUD API for a generic StorageUser model.\n\nThe StorageUser model is defined in app.models\nThe ListUsersResponse and UserResponse schemas are defined in app.schemas.\n"""\n\n@app.get("/users")\nasync def list_users(db: AsyncSession = Depends(async_session)):\n    storage_users = (await db.execute(select(StorageUser))).scalars().all()\n    return ListUsersResponse.from_storage(storage_users)\n\n\n@app.post("/users")\nasync def create_user(email: str, name: str, db: AsyncSession = Depends(async_session)):\n    storage_user = StorageUser(email=email, name=name)\n    db.add(storage_user)\n    await db.commit()\n    return UserResponse.from_storage(storage_user)\n\n\n@app.get("/users/{user_id}")\nasync def read_user(user_id: int, db: AsyncSession = Depends(async_session)):\n    storage_user = await db.get(StorageUser, user_id)\n    if storage_user is None:\n        raise HTTPException(status_code=404, detail="User not found")\n    return UserResponse.from_storage(storage_user)\n\n\n@app.put("/users/{user_id}")\nasync def update_user(\n    user_id: int, name: str, db: AsyncSession = Depends(async_session)\n):\n    storage_user = await db.get(StorageUser, user_id)\n    if storage_user is None:\n        raise HTTPException(status_code=404, detail="User not found")\n    storage_user.name = name\n    await db.commit()\n    return UserResponse.from_storage(storage_user)\n\n\n@app.delete("/users/{user_id}")\nasync def delete_user(user_id: int, db: AsyncSession = Depends(async_session)):\n    storage_user = await db.get(StorageUser, user_id)\n    if storage_user is None:\n        raise HTTPException(status_code=404, detail="User not found")\n    await db.delete(storage_user)\n    await db.commit()\n    return UserResponse.from_storage(storage_user)\n')
    
-   100         296 LOAD_CONST              42 (('infra_docs_url', 'infra_name', 'infra_lf_class', 'launchflow_imports', 'infra_import', 'global_setup', 'app_imports', 'fastapi_setup', 'fastapi_test_endpoint', 'requirements'))
-               298 BUILD_CONST_KEY_MAP     10
+   172         302 LOAD_CONST              41 ('sqlalchemy[async]')
+               304 LOAD_CONST              42 ('asyncpg')
+               306 BUILD_LIST               2
    
-   175         300 LOAD_NAME               11 (S3Bucket)
+   100         308 LOAD_CONST              43 (('infra_docs_url', 'infra_name', 'infra_lf_class', 'launchflow_imports', 'infra_import', 'global_setup', 'app_imports', 'fastapi_setup', 'fastapi_test_endpoint', 'requirements'))
+               310 BUILD_CONST_KEY_MAP     10
    
-   176         302 LOAD_CONST              43 ('https://docs.launchflow.com/reference/aws-resources/s3-bucket')
+   175         312 LOAD_NAME               15 (S3Bucket)
    
-   177         304 LOAD_CONST              44 ('s3_bucket')
+   176         314 LOAD_CONST              44 ('https://docs.launchflow.com/reference/aws-resources/s3-bucket')
    
-   178         306 LOAD_CONST              45 ('lf.aws.S3Bucket')
+   177         316 LOAD_CONST              45 ('s3_bucket')
    
-   179         308 LOAD_CONST              17 ('')
+   178         318 LOAD_CONST              46 ('lf.aws.S3Bucket')
    
-   180         310 LOAD_CONST              17 ('')
+   179         320 LOAD_CONST              18 ('')
    
-   181         312 LOAD_CONST               1 (None)
+   180         322 LOAD_CONST              18 ('')
    
-   182         314 LOAD_CONST               1 (None)
+   181         324 LOAD_CONST               1 (None)
    
-   183         316 BUILD_LIST               0
+   182         326 LOAD_CONST               1 (None)
    
-   184         318 LOAD_CONST              46 ('\n# This endpoint uploads a file to S3 and reads it back to verify the bucket works\n@app.post("/test_s3/{object_name}")\nasync def test_s3(object_name: str):\n    # Write to S3\n    s3_bucket.upload_from_string("Hello, World!", object_name)\n    # Immediately read from S3 to verify the write\n    s3_bucket.download_file(object_name).decode("utf-8")\n    return {"message": f"Uploaded {object_name} to S3"}\n')
+   183         328 BUILD_LIST               0
    
-   194         320 BUILD_LIST               0
+   184         330 LOAD_CONST              47 ('\n# This endpoint uploads a file to S3 and reads it back to verify the bucket works\n@app.post("/test_s3/{object_name}")\nasync def test_s3(object_name: str):\n    # Write to S3\n    s3_bucket.upload_from_string("Hello, World!", object_name)\n    # Immediately read from S3 to verify the write\n    s3_bucket.download_file(object_name).decode("utf-8")\n    return {"message": f"Uploaded {object_name} to S3"}\n')
    
-   175         322 LOAD_CONST              21 (('infra_docs_url', 'infra_name', 'infra_lf_class', 'launchflow_imports', 'infra_import', 'global_setup', 'fastapi_setup', 'app_imports', 'fastapi_test_endpoint', 'requirements'))
-               324 BUILD_CONST_KEY_MAP     10
+   194         332 BUILD_LIST               0
    
-   197         326 LOAD_NAME                9 (RDSPostgres)
+   175         334 LOAD_CONST              22 (('infra_docs_url', 'infra_name', 'infra_lf_class', 'launchflow_imports', 'infra_import', 'global_setup', 'fastapi_setup', 'app_imports', 'fastapi_test_endpoint', 'requirements'))
+               336 BUILD_CONST_KEY_MAP     10
    
-   198         328 LOAD_CONST              47 ('https://docs.launchflow.com/reference/aws-resources/rds')
+   197         338 LOAD_NAME               11 (ElasticacheRedis)
    
-   199         330 LOAD_CONST              31 ('postgres')
+   198         340 LOAD_CONST              48 ('https://docs.launchflow.com/reference/aws-resources/elasticache-redis')
    
-   200         332 LOAD_CONST              48 ('lf.aws.RDSPostgres')
+   199         342 LOAD_CONST              49 ('elasticache')
    
-   201         334 LOAD_CONST              33 ('from launchflow.fastapi import sqlalchemy_async_depends')
+   200         344 LOAD_CONST              50 ('lf.aws.ElasticacheRedis')
    
-   202         336 LOAD_CONST              34 ('from sqlalchemy import select\nfrom sqlalchemy.ext.asyncio import AsyncSession\n')
+   201         346 LOAD_CONST              18 ('')
    
-   205         338 LOAD_CONST              35 ('# Create the global FastAPI dependency for the SQLAlchemy async session\nasync_session = sqlalchemy_async_depends()')
+   202         348 LOAD_CONST              19 ('from redis.asyncio import Redis')
    
-   208         340 LOAD_CONST              36 ('from app.models import Base, StorageUser')
+   203         350 LOAD_CONST               1 (None)
    
-   209         342 LOAD_CONST              37 ('from app.schemas import ListUsersResponse, UserResponse')
+   204         352 LOAD_CONST               1 (None)
    
-   207         344 BUILD_LIST               2
+   205         354 BUILD_LIST               0
    
-   211         346 LOAD_CONST              38 ('    # Create the SQLAlchemy async engine (connection pool)\n    engine = await postgres.sqlalchemy_async_engine()\n    # Create the database tables using the engine\n    async with engine.begin() as conn:\n        await conn.run_sync(Base.metadata.create_all)\n    # Set up the FastAPI dependency\n    async_session.setup(engine)')
+   206         356 LOAD_CONST              51 ('\n@app.post("/test_redis/{key}")\nasync def test_redis(\n    key: str, value: str, redis_client: Redis = Depends(elasticache.redis_async)\n):\n    # Write to Redis\n    await redis_client.set(key, value)\n    # Immediately read from Redis to verify the write\n    value = await redis_client.get(key)\n    return {"message": f"Set {key} to {value}"}\n')
    
-   218         348 LOAD_CONST              39 ('\n"""\nThe endpoints below define a simple CRUD API for a generic StorageUser model.\n\nThe StorageUser model is defined in app.models\nThe ListUsersResponse and UserResponse schemas are defined in app.schemas.\n"""\n\n@app.get("/users")\nasync def list_users(db: AsyncSession = Depends(async_session)):\n    storage_users = (await db.execute(select(StorageUser))).scalars().all()\n    return ListUsersResponse.from_storage(storage_users)\n\n\n@app.post("/users")\nasync def create_user(email: str, name: str, db: AsyncSession = Depends(async_session)):\n    storage_user = StorageUser(email=email, name=name)\n    db.add(storage_user)\n    await db.commit()\n    return UserResponse.from_storage(storage_user)\n\n\n@app.get("/users/{user_id}")\nasync def read_user(user_id: int, db: AsyncSession = Depends(async_session)):\n    storage_user = await db.get(StorageUser, user_id)\n    if storage_user is None:\n        raise HTTPException(status_code=404, detail="User not found")\n    return UserResponse.from_storage(storage_user)\n\n\n@app.put("/users/{user_id}")\nasync def update_user(\n    user_id: int, name: str, db: AsyncSession = Depends(async_session)\n):\n    storage_user = await db.get(StorageUser, user_id)\n    if storage_user is None:\n        raise HTTPException(status_code=404, detail="User not found")\n    storage_user.name = name\n    await db.commit()\n    return UserResponse.from_storage(storage_user)\n\n\n@app.delete("/users/{user_id}")\nasync def delete_user(user_id: int, db: AsyncSession = Depends(async_session)):\n    storage_user = await db.get(StorageUser, user_id)\n    if storage_user is None:\n        raise HTTPException(status_code=404, detail="User not found")\n    await db.delete(storage_user)\n    await db.commit()\n    return UserResponse.from_storage(storage_user)\n')
+   217         358 LOAD_CONST              21 ('redis>=4.2.0')
+               360 BUILD_LIST               1
    
-   269         350 LOAD_CONST              40 ('sqlalchemy[async]')
-               352 LOAD_CONST              41 ('asyncpg')
-               354 BUILD_LIST               2
+   197         362 LOAD_CONST              22 (('infra_docs_url', 'infra_name', 'infra_lf_class', 'launchflow_imports', 'infra_import', 'global_setup', 'fastapi_setup', 'app_imports', 'fastapi_test_endpoint', 'requirements'))
+               364 BUILD_CONST_KEY_MAP     10
    
-   197         356 LOAD_CONST              42 (('infra_docs_url', 'infra_name', 'infra_lf_class', 'launchflow_imports', 'infra_import', 'global_setup', 'app_imports', 'fastapi_setup', 'fastapi_test_endpoint', 'requirements'))
-               358 BUILD_CONST_KEY_MAP     10
+   220         366 LOAD_NAME               13 (RDSPostgres)
    
-    30         360 BUILD_MAP                6
-               362 STORE_NAME              25 (resource_type_to_resource_info_kwargs)
+   221         368 LOAD_CONST              52 ('https://docs.launchflow.com/reference/aws-resources/rds-postgres')
    
-   274         364 LOAD_CONST              49 ('resource')
-               366 LOAD_NAME                7 (Type)
-               368 LOAD_NAME               23 (Resource)
-               370 BINARY_SUBSCR
-               380 LOAD_CONST              50 ('return')
-               382 LOAD_NAME               24 (ResourceInfo)
-               384 BUILD_TUPLE              4
-               386 LOAD_CONST              51 (<code object get_resource_info, file "/home/tanke/launchflow/launchflow/clients/python/launchflow/launchflow/cli/gen/templates/fastapi/fastapi_template.py", line 274>)
-               388 MAKE_FUNCTION            4 (annotations)
-               390 STORE_NAME              26 (get_resource_info)
+   222         370 LOAD_CONST              32 ('postgres')
    
-   283         392 LOAD_NAME                2 (dataclass)
+   223         372 LOAD_CONST              53 ('lf.aws.RDSPostgres')
    
-   284         394 PUSH_NULL
-               396 LOAD_BUILD_CLASS
-               398 LOAD_CONST              52 (<code object FastAPIProjectGenerator, file "/home/tanke/launchflow/launchflow/clients/python/launchflow/launchflow/cli/gen/templates/fastapi/fastapi_template.py", line 283>)
-               400 MAKE_FUNCTION            0
-               402 LOAD_CONST              53 ('FastAPIProjectGenerator')
-               404 LOAD_NAME               13 (ProjectGenerator)
-               406 PRECALL                  3
-               410 CALL                     3
+   224         374 LOAD_CONST              34 ('from launchflow.fastapi import sqlalchemy_async_depends')
    
-   283         420 PRECALL                  0
-               424 CALL                     0
+   225         376 LOAD_CONST              35 ('from sqlalchemy import select\nfrom sqlalchemy.ext.asyncio import AsyncSession\n')
    
-   284         434 STORE_NAME              27 (FastAPIProjectGenerator)
+   228         378 LOAD_CONST              36 ('# Create the global FastAPI dependency for the SQLAlchemy async session\nasync_session = sqlalchemy_async_depends()')
    
-   485         436 LOAD_NAME               28 (__name__)
-               438 LOAD_CONST              54 ('__main__')
-               440 COMPARE_OP               2 (==)
-               446 POP_JUMP_FORWARD_IF_FALSE    48 (to 544)
+   231         380 LOAD_CONST              37 ('from app.models import Base, StorageUser')
    
-   486         448 LOAD_CONST              55 ('gcp')
-               450 STORE_NAME              29 (cloud_provider)
+   232         382 LOAD_CONST              38 ('from app.schemas import ListUsersResponse, UserResponse')
    
-   487         452 PUSH_NULL
-               454 LOAD_NAME               27 (FastAPIProjectGenerator)
+   230         384 BUILD_LIST               2
    
-   489         456 LOAD_NAME               17 (ComputeEngineRedis)
+   234         386 LOAD_CONST              39 ('    # Create the SQLAlchemy async engine (connection pool)\n    engine = await postgres.sqlalchemy_async_engine()\n    # Create the database tables using the engine\n    async with engine.begin() as conn:\n        await conn.run_sync(Base.metadata.create_all)\n    # Set up the FastAPI dependency\n    async_session.setup(engine)')
    
-   490         458 LOAD_NAME               19 (GCSBucket)
+   241         388 LOAD_CONST              40 ('\n"""\nThe endpoints below define a simple CRUD API for a generic StorageUser model.\n\nThe StorageUser model is defined in app.models\nThe ListUsersResponse and UserResponse schemas are defined in app.schemas.\n"""\n\n@app.get("/users")\nasync def list_users(db: AsyncSession = Depends(async_session)):\n    storage_users = (await db.execute(select(StorageUser))).scalars().all()\n    return ListUsersResponse.from_storage(storage_users)\n\n\n@app.post("/users")\nasync def create_user(email: str, name: str, db: AsyncSession = Depends(async_session)):\n    storage_user = StorageUser(email=email, name=name)\n    db.add(storage_user)\n    await db.commit()\n    return UserResponse.from_storage(storage_user)\n\n\n@app.get("/users/{user_id}")\nasync def read_user(user_id: int, db: AsyncSession = Depends(async_session)):\n    storage_user = await db.get(StorageUser, user_id)\n    if storage_user is None:\n        raise HTTPException(status_code=404, detail="User not found")\n    return UserResponse.from_storage(storage_user)\n\n\n@app.put("/users/{user_id}")\nasync def update_user(\n    user_id: int, name: str, db: AsyncSession = Depends(async_session)\n):\n    storage_user = await db.get(StorageUser, user_id)\n    if storage_user is None:\n        raise HTTPException(status_code=404, detail="User not found")\n    storage_user.name = name\n    await db.commit()\n    return UserResponse.from_storage(storage_user)\n\n\n@app.delete("/users/{user_id}")\nasync def delete_user(user_id: int, db: AsyncSession = Depends(async_session)):\n    storage_user = await db.get(StorageUser, user_id)\n    if storage_user is None:\n        raise HTTPException(status_code=404, detail="User not found")\n    await db.delete(storage_user)\n    await db.commit()\n    return UserResponse.from_storage(storage_user)\n')
    
-   491         460 LOAD_NAME               15 (CloudSQLPostgres)
+   292         390 LOAD_CONST              41 ('sqlalchemy[async]')
+               392 LOAD_CONST              42 ('asyncpg')
+               394 BUILD_LIST               2
    
-   488         462 BUILD_LIST               3
+   220         396 LOAD_CONST              43 (('infra_docs_url', 'infra_name', 'infra_lf_class', 'launchflow_imports', 'infra_import', 'global_setup', 'app_imports', 'fastapi_setup', 'fastapi_test_endpoint', 'requirements'))
+               398 BUILD_CONST_KEY_MAP     10
    
-   495         464 LOAD_NAME               29 (cloud_provider)
+    30         400 BUILD_MAP                7
+               402 STORE_NAME              27 (resource_type_to_resource_info_kwargs)
    
-   496         466 LOAD_NAME               29 (cloud_provider)
-               468 FORMAT_VALUE             0
-               470 LOAD_CONST              56 ('-examples')
-               472 BUILD_STRING             2
+   297         404 LOAD_CONST              54 ('resource')
+               406 LOAD_NAME                7 (Type)
+               408 LOAD_NAME                9 (Resource)
+               410 BINARY_SUBSCR
+               420 LOAD_CONST              55 ('return')
+               422 LOAD_NAME               26 (ResourceInfo)
+               424 BUILD_TUPLE              4
+               426 LOAD_CONST              56 (<code object get_resource_info, file "/Users/calebvandyke/code/launchflow-oss/launchflow/cli/gen/templates/fastapi/fastapi_template.py", line 297>)
+               428 MAKE_FUNCTION            4 (annotations)
+               430 STORE_NAME              28 (get_resource_info)
    
-   497         474 LOAD_CONST              57 ('dev')
+   306         432 LOAD_NAME                2 (dataclass)
    
-   498         476 LOAD_CONST              58 ('fastapi-service')
+   307         434 PUSH_NULL
+               436 LOAD_BUILD_CLASS
+               438 LOAD_CONST              57 (<code object FastAPIProjectGenerator, file "/Users/calebvandyke/code/launchflow-oss/launchflow/cli/gen/templates/fastapi/fastapi_template.py", line 306>)
+               440 MAKE_FUNCTION            0
+               442 LOAD_CONST              58 ('FastAPIProjectGenerator')
+               444 LOAD_NAME               17 (ProjectGenerator)
+               446 PRECALL                  3
+               450 CALL                     3
    
-   487         478 KW_NAMES                59
-               480 PRECALL                  5
-               484 CALL                     5
-               494 STORE_NAME              30 (generator)
+   306         460 PRECALL                  0
+               464 CALL                     0
    
-   500         496 LOAD_NAME               30 (generator)
-               498 LOAD_METHOD             31 (generate_project)
-               520 LOAD_CONST              60 ('/tmp/launchflow')
-               522 KW_NAMES                61
-               524 PRECALL                  1
-               528 CALL                     1
-               538 POP_TOP
-               540 LOAD_CONST               1 (None)
-               542 RETURN_VALUE
-   
-   485     >>  544 LOAD_CONST               1 (None)
-               546 RETURN_VALUE
+   307         474 STORE_NAME              29 (FastAPIProjectGenerator)
+               476 LOAD_CONST               1 (None)
+               478 RETURN_VALUE
    consts
       0
       None
       ('dataclass',)
       ('List', 'Literal', 'Optional', 'Type')
+      ('Resource',)
+      ('ElasticacheRedis',)
       ('RDSPostgres',)
       ('S3Bucket',)
       ('ProjectGenerator',)
       ('CloudSQLPostgres',)
       ('ComputeEngineRedis',)
       ('GCSBucket',)
       ('MemorystoreRedis',)
-      ('Resource',)
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 3
          flags     : 0
          code
             0x970065005a0164005a0255006503650464013c0000006503650464023c
@@ -471,31 +457,31 @@
             'fastapi_test_endpoint'
             'requirements'
             None
          names      ('__name__', '__module__', '__qualname__', 'str', '__annotations__', 'Optional', 'List')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/home/tanke/launchflow/launchflow/clients/python/launchflow/launchflow/cli/gen/templates/fastapi/fastapi_template.py'
+         filename   '/Users/calebvandyke/code/launchflow-oss/launchflow/cli/gen/templates/fastapi/fastapi_template.py'
          name       'ResourceInfo'
          firstlineno 16
          lnotab 0x0c020a010a010a010a0116011601160116010a01
       'ResourceInfo'
-      'https://docs.launchflow.com/reference/gcp-resources/compute-engine'
+      'https://docs.launchflow.com/reference/gcp-resources/compute-engine#compute-engine-redis'
       'redis_vm'
       'lf.gcp.ComputeEngineRedis'
       ''
       'from redis.asyncio import Redis'
       '\n@app.post("/test_redis/{key}")\nasync def test_redis(\n    key: str, value: str, redis_client: Redis = Depends(redis_vm.redis_async)\n):\n    # Write to Redis\n    await redis_client.set(key, value)\n    # Immediately read from Redis to verify the write\n    value = await redis_client.get(key)\n    return {"message": f"Set {key} to {value}"}\n'
       'redis>=4.2.0'
       ('infra_docs_url', 'infra_name', 'infra_lf_class', 'launchflow_imports', 'infra_import', 'global_setup', 'fastapi_setup', 'app_imports', 'fastapi_test_endpoint', 'requirements')
-      'https://docs.launchflow.com/reference/gcp-resources/memorystore-redis'
-      'redis_cluster'
+      'https://docs.launchflow.com/reference/gcp-resources/memorystore'
+      'memorystore'
       'lf.gcp.MemorystoreRedis'
-      '\n@app.post("/test_redis/{key}")\nasync def test_redis(\n    key: str, value: str, redis_client: Redis = Depends(redis_cluster.redis_async)\n):\n    # Write to Redis\n    await redis_client.set(key, value)\n    # Immediately read from Redis to verify the write\n    value = await redis_client.get(key)\n    return {"message": f"Set {key} to {value}"}\n'
+      '\n@app.post("/test_redis/{key}")\nasync def test_redis(\n    key: str, value: str, redis_client: Redis = Depends(memorystore.redis_async)\n):\n    # Write to Redis\n    await redis_client.set(key, value)\n    # Immediately read from Redis to verify the write\n    value = await redis_client.get(key)\n    return {"message": f"Set {key} to {value}"}\n'
       'https://docs.launchflow.com/reference/gcp-resources/gcs-bucket'
       'gcs_bucket'
       'lf.gcp.GCSBucket'
       '\n# This endpoint uploads a file to GCS and reads it back to verify the bucket works\n@app.post("/test_gcs/{object_name}")\nasync def test_gcs(object_name: str):\n    # Write to GCS\n    gcs_bucket.upload_from_string("Hello, World!", object_name)\n    # Immediately read from GCS to verify the write\n    gcs_bucket.download_file(object_name).decode("utf-8")\n    return {"message": f"Uploaded {object_name} to GCS"}\n'
       'https://docs.launchflow.com/reference/gcp-resources/cloud-sql'
       'postgres'
       'lf.gcp.CloudSQLPostgres'
@@ -509,71 +495,75 @@
       'sqlalchemy[async]'
       'asyncpg'
       ('infra_docs_url', 'infra_name', 'infra_lf_class', 'launchflow_imports', 'infra_import', 'global_setup', 'app_imports', 'fastapi_setup', 'fastapi_test_endpoint', 'requirements')
       'https://docs.launchflow.com/reference/aws-resources/s3-bucket'
       's3_bucket'
       'lf.aws.S3Bucket'
       '\n# This endpoint uploads a file to S3 and reads it back to verify the bucket works\n@app.post("/test_s3/{object_name}")\nasync def test_s3(object_name: str):\n    # Write to S3\n    s3_bucket.upload_from_string("Hello, World!", object_name)\n    # Immediately read from S3 to verify the write\n    s3_bucket.download_file(object_name).decode("utf-8")\n    return {"message": f"Uploaded {object_name} to S3"}\n'
-      'https://docs.launchflow.com/reference/aws-resources/rds'
+      'https://docs.launchflow.com/reference/aws-resources/elasticache-redis'
+      'elasticache'
+      'lf.aws.ElasticacheRedis'
+      '\n@app.post("/test_redis/{key}")\nasync def test_redis(\n    key: str, value: str, redis_client: Redis = Depends(elasticache.redis_async)\n):\n    # Write to Redis\n    await redis_client.set(key, value)\n    # Immediately read from Redis to verify the write\n    value = await redis_client.get(key)\n    return {"message": f"Set {key} to {value}"}\n'
+      'https://docs.launchflow.com/reference/aws-resources/rds-postgres'
       'lf.aws.RDSPostgres'
       'resource'
       'return'
       code
          argcount  : 1
          nlocals   : 2
          stacksize : 5
          flags     : 3
          code
             0x9700740000000000000000000000a00100000000000000000000000000
             000000000000007c006400a6020000ab0200000000000000007d017c0180
             1274050000000000000000000064017c009b009d02a6010000ab01000000
             00000000008201740700000000000000000000640269007c01a4018e0153
             00
-         274           0 RESUME                   0
+         297           0 RESUME                   0
          
-         275           2 LOAD_GLOBAL              0 (resource_type_to_resource_info_kwargs)
+         298           2 LOAD_GLOBAL              0 (resource_type_to_resource_info_kwargs)
                       14 LOAD_METHOD              1 (get)
                       36 LOAD_FAST                0 (resource)
                       38 LOAD_CONST               0 (None)
                       40 PRECALL                  2
                       44 CALL                     2
                       54 STORE_FAST               1 (resource_info_kwargs)
          
-         276          56 LOAD_FAST                1 (resource_info_kwargs)
+         299          56 LOAD_FAST                1 (resource_info_kwargs)
                       58 POP_JUMP_FORWARD_IF_NOT_NONE    18 (to 96)
          
-         277          60 LOAD_GLOBAL              5 (NULL + ValueError)
+         300          60 LOAD_GLOBAL              5 (NULL + ValueError)
                       72 LOAD_CONST               1 ('Unsupported resource type: ')
                       74 LOAD_FAST                0 (resource)
                       76 FORMAT_VALUE             0
                       78 BUILD_STRING             2
                       80 PRECALL                  1
                       84 CALL                     1
                       94 RAISE_VARARGS            1
          
-         278     >>   96 LOAD_GLOBAL              7 (NULL + ResourceInfo)
+         301     >>   96 LOAD_GLOBAL              7 (NULL + ResourceInfo)
                      108 LOAD_CONST               2 (())
                      110 BUILD_MAP                0
          
-         279         112 LOAD_FAST                1 (resource_info_kwargs)
+         302         112 LOAD_FAST                1 (resource_info_kwargs)
          
-         278         114 DICT_MERGE               1
+         301         114 DICT_MERGE               1
                      116 CALL_FUNCTION_EX         1
                      118 RETURN_VALUE
          consts
             None
             'Unsupported resource type: '
             ()
          names      ('resource_type_to_resource_info_kwargs', 'get', 'ValueError', 'ResourceInfo')
          varnames   ('resource', 'resource_info_kwargs')
          freevars   ()
          cellvars   ()
-         filename   '/home/tanke/launchflow/launchflow/clients/python/launchflow/launchflow/cli/gen/templates/fastapi/fastapi_template.py'
+         filename   '/Users/calebvandyke/code/launchflow-oss/launchflow/cli/gen/templates/fastapi/fastapi_template.py'
          name       'get_resource_info'
-         firstlineno 274
+         firstlineno 297
          lnotab 0x0201360104012401100102ff
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 4
          flags     : 0
          code
@@ -583,222 +573,220 @@
             065a096508650664073c000000650a6a0b00000000000000006a0c000000
             00000000005a0d650e650664083c000000650a6a0b00000000000000006a
             0f00000000000000005a10650e650664093c000000640a5a116512640b65
             086602640c8404a6000000ab0000000000000000005a136512640b650866
             02640d8404a6000000ab0000000000000000005a146512640b6503650819
             0000000000000000006602640e8404a6000000ab0000000000000000005a
             156512640b65086602640f8404a6000000ab0000000000000000005a1665
-            12640b6503650819000000000000000000660264108404a6000000ab0000
-            000000000000005a176512640b6503650819000000000000000000660264
-            118404a6000000ab0000000000000000005a186512640b65036508190000
-            00000000000000660264128404a6000000ab0000000000000000005a1965
-            12640b6508660264138404a6000000ab0000000000000000005a1a640b65
-            086602641484045a1b6512640b6508660264158404a6000000ab00000000
-            00000000005a1c640b651d6602641684045a1e64175300
-         283           0 RESUME                   0
+            12640b6508660264108404a6000000ab0000000000000000005a17651264
+            0b6503650819000000000000000000660264118404a6000000ab00000000
+            00000000005a186512640b65036508190000000000000000006602641284
+            04a6000000ab0000000000000000005a196512640b6508660264138404a6
+            000000ab0000000000000000005a1a640b65086602641484045a1b651264
+            0b6508660264158404a6000000ab0000000000000000005a1c640b651d66
+            02641684045a1e64175300
+         306           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('FastAPIProjectGenerator')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
-         285          12 LOAD_NAME                3 (List)
+         308          12 LOAD_NAME                3 (List)
                       14 LOAD_NAME                4 (Type)
                       16 LOAD_NAME                5 (Resource)
                       18 BINARY_SUBSCR
                       28 BINARY_SUBSCR
                       38 LOAD_NAME                6 (__annotations__)
                       40 LOAD_CONST               1 ('resources')
                       42 STORE_SUBSCR
          
-         287          46 LOAD_NAME                7 (Literal)
+         310          46 LOAD_NAME                7 (Literal)
                       48 LOAD_CONST               2 (('aws', 'gcp'))
                       50 BINARY_SUBSCR
                       60 LOAD_NAME                6 (__annotations__)
                       62 LOAD_CONST               3 ('cloud_provider')
                       64 STORE_SUBSCR
          
-         289          68 LOAD_NAME                8 (str)
+         312          68 LOAD_NAME                8 (str)
                       70 LOAD_NAME                6 (__annotations__)
                       72 LOAD_CONST               4 ('launchflow_project_name')
                       74 STORE_SUBSCR
          
-         290          78 LOAD_NAME                8 (str)
+         313          78 LOAD_NAME                8 (str)
                       80 LOAD_NAME                6 (__annotations__)
                       82 LOAD_CONST               5 ('launchflow_environment_name')
                       84 STORE_SUBSCR
          
-         291          88 LOAD_CONST               6 ('fastapi-service')
+         314          88 LOAD_CONST               6 ('fastapi-service')
                       90 STORE_NAME               9 (launchflow_service_name)
                       92 LOAD_NAME                8 (str)
                       94 LOAD_NAME                6 (__annotations__)
                       96 LOAD_CONST               7 ('launchflow_service_name')
                       98 STORE_SUBSCR
          
-         293         102 LOAD_NAME               10 (sys)
+         316         102 LOAD_NAME               10 (sys)
                      104 LOAD_ATTR               11 (version_info)
                      114 LOAD_ATTR               12 (major)
                      124 STORE_NAME              13 (python_major_version)
                      126 LOAD_NAME               14 (int)
                      128 LOAD_NAME                6 (__annotations__)
                      130 LOAD_CONST               8 ('python_major_version')
                      132 STORE_SUBSCR
          
-         294         136 LOAD_NAME               10 (sys)
+         317         136 LOAD_NAME               10 (sys)
                      138 LOAD_ATTR               11 (version_info)
                      148 LOAD_ATTR               15 (minor)
                      158 STORE_NAME              16 (python_minor_version)
                      160 LOAD_NAME               14 (int)
                      162 LOAD_NAME                6 (__annotations__)
                      164 LOAD_CONST               9 ('python_minor_version')
                      166 STORE_SUBSCR
          
-         295         170 LOAD_CONST              10 (8080)
+         318         170 LOAD_CONST              10 (8080)
                      172 STORE_NAME              17 (port)
          
-         298         174 LOAD_NAME               18 (property)
+         321         174 LOAD_NAME               18 (property)
          
-         299         176 LOAD_CONST              11 ('return')
+         322         176 LOAD_CONST              11 ('return')
                      178 LOAD_NAME                8 (str)
                      180 BUILD_TUPLE              2
-                     182 LOAD_CONST              12 (<code object infra_dot_py, file "/home/tanke/launchflow/launchflow/clients/python/launchflow/launchflow/cli/gen/templates/fastapi/fastapi_template.py", line 298>)
+                     182 LOAD_CONST              12 (<code object infra_dot_py, file "/Users/calebvandyke/code/launchflow-oss/launchflow/cli/gen/templates/fastapi/fastapi_template.py", line 321>)
                      184 MAKE_FUNCTION            4 (annotations)
          
-         298         186 PRECALL                  0
+         321         186 PRECALL                  0
                      190 CALL                     0
          
-         299         200 STORE_NAME              19 (infra_dot_py)
+         322         200 STORE_NAME              19 (infra_dot_py)
          
-         345         202 LOAD_NAME               18 (property)
+         368         202 LOAD_NAME               18 (property)
          
-         346         204 LOAD_CONST              11 ('return')
+         369         204 LOAD_CONST              11 ('return')
                      206 LOAD_NAME                8 (str)
                      208 BUILD_TUPLE              2
-                     210 LOAD_CONST              13 (<code object fastapi_imports, file "/home/tanke/launchflow/launchflow/clients/python/launchflow/launchflow/cli/gen/templates/fastapi/fastapi_template.py", line 345>)
+                     210 LOAD_CONST              13 (<code object fastapi_imports, file "/Users/calebvandyke/code/launchflow-oss/launchflow/cli/gen/templates/fastapi/fastapi_template.py", line 368>)
                      212 MAKE_FUNCTION            4 (annotations)
          
-         345         214 PRECALL                  0
+         368         214 PRECALL                  0
                      218 CALL                     0
          
-         346         228 STORE_NAME              20 (fastapi_imports)
+         369         228 STORE_NAME              20 (fastapi_imports)
          
-         366         230 LOAD_NAME               18 (property)
+         385         230 LOAD_NAME               18 (property)
          
-         367         232 LOAD_CONST              11 ('return')
+         386         232 LOAD_CONST              11 ('return')
                      234 LOAD_NAME                3 (List)
                      236 LOAD_NAME                8 (str)
                      238 BINARY_SUBSCR
                      248 BUILD_TUPLE              2
-                     250 LOAD_CONST              14 (<code object app_infra_imports, file "/home/tanke/launchflow/launchflow/clients/python/launchflow/launchflow/cli/gen/templates/fastapi/fastapi_template.py", line 366>)
+                     250 LOAD_CONST              14 (<code object app_infra_imports, file "/Users/calebvandyke/code/launchflow-oss/launchflow/cli/gen/templates/fastapi/fastapi_template.py", line 385>)
                      252 MAKE_FUNCTION            4 (annotations)
          
-         366         254 PRECALL                  0
+         385         254 PRECALL                  0
                      258 CALL                     0
          
-         367         268 STORE_NAME              21 (app_infra_imports)
+         386         268 STORE_NAME              21 (app_infra_imports)
          
-         392         270 LOAD_NAME               18 (property)
+         411         270 LOAD_NAME               18 (property)
          
-         393         272 LOAD_CONST              11 ('return')
+         412         272 LOAD_CONST              11 ('return')
                      274 LOAD_NAME                8 (str)
                      276 BUILD_TUPLE              2
-                     278 LOAD_CONST              15 (<code object app_global_setup, file "/home/tanke/launchflow/launchflow/clients/python/launchflow/launchflow/cli/gen/templates/fastapi/fastapi_template.py", line 392>)
+                     278 LOAD_CONST              15 (<code object app_global_setup, file "/Users/calebvandyke/code/launchflow-oss/launchflow/cli/gen/templates/fastapi/fastapi_template.py", line 411>)
                      280 MAKE_FUNCTION            4 (annotations)
          
-         392         282 PRECALL                  0
+         411         282 PRECALL                  0
                      286 CALL                     0
          
-         393         296 STORE_NAME              22 (app_global_setup)
+         412         296 STORE_NAME              22 (app_global_setup)
+         
+         421         298 LOAD_NAME               18 (property)
+         
+         422         300 LOAD_CONST              11 ('return')
+                     302 LOAD_NAME                8 (str)
+                     304 BUILD_TUPLE              2
+                     306 LOAD_CONST              16 (<code object app_infra_setup, file "/Users/calebvandyke/code/launchflow-oss/launchflow/cli/gen/templates/fastapi/fastapi_template.py", line 421>)
+                     308 MAKE_FUNCTION            4 (annotations)
+         
+         421         310 PRECALL                  0
+                     314 CALL                     0
+         
+         422         324 STORE_NAME              23 (app_infra_setup)
+         
+         447         326 LOAD_NAME               18 (property)
+         
+         448         328 LOAD_CONST              11 ('return')
+                     330 LOAD_NAME                3 (List)
+                     332 LOAD_NAME                8 (str)
+                     334 BINARY_SUBSCR
+                     344 BUILD_TUPLE              2
+                     346 LOAD_CONST              17 (<code object app_infra_endpoints, file "/Users/calebvandyke/code/launchflow-oss/launchflow/cli/gen/templates/fastapi/fastapi_template.py", line 447>)
+                     348 MAKE_FUNCTION            4 (annotations)
+         
+         447         350 PRECALL                  0
+                     354 CALL                     0
+         
+         448         364 STORE_NAME              24 (app_infra_endpoints)
+         
+         456         366 LOAD_NAME               18 (property)
+         
+         457         368 LOAD_CONST              11 ('return')
+                     370 LOAD_NAME                3 (List)
+                     372 LOAD_NAME                8 (str)
+                     374 BINARY_SUBSCR
+                     384 BUILD_TUPLE              2
+                     386 LOAD_CONST              18 (<code object additional_requirements, file "/Users/calebvandyke/code/launchflow-oss/launchflow/cli/gen/templates/fastapi/fastapi_template.py", line 456>)
+                     388 MAKE_FUNCTION            4 (annotations)
+         
+         456         390 PRECALL                  0
+                     394 CALL                     0
+         
+         457         404 STORE_NAME              25 (additional_requirements)
+         
+         465         406 LOAD_NAME               18 (property)
+         
+         466         408 LOAD_CONST              11 ('return')
+                     410 LOAD_NAME                8 (str)
+                     412 BUILD_TUPLE              2
+                     414 LOAD_CONST              19 (<code object launchflow_service_product, file "/Users/calebvandyke/code/launchflow-oss/launchflow/cli/gen/templates/fastapi/fastapi_template.py", line 465>)
+                     416 MAKE_FUNCTION            4 (annotations)
+         
+         465         418 PRECALL                  0
+                     422 CALL                     0
+         
+         466         432 STORE_NAME              26 (launchflow_service_product)
+         
+         473         434 LOAD_CONST              11 ('return')
+                     436 LOAD_NAME                8 (str)
+                     438 BUILD_TUPLE              2
+                     440 LOAD_CONST              20 (<code object template_path_info, file "/Users/calebvandyke/code/launchflow-oss/launchflow/cli/gen/templates/fastapi/fastapi_template.py", line 473>)
+                     442 MAKE_FUNCTION            4 (annotations)
+                     444 STORE_NAME              27 (template_path_info)
+         
+         484         446 LOAD_NAME               18 (property)
+         
+         485         448 LOAD_CONST              11 ('return')
+                     450 LOAD_NAME                8 (str)
+                     452 BUILD_TUPLE              2
+                     454 LOAD_CONST              21 (<code object docker_repository_prefix, file "/Users/calebvandyke/code/launchflow-oss/launchflow/cli/gen/templates/fastapi/fastapi_template.py", line 484>)
+                     456 MAKE_FUNCTION            4 (annotations)
+         
+         484         458 PRECALL                  0
+                     462 CALL                     0
          
-         402         298 LOAD_NAME               18 (property)
+         485         472 STORE_NAME              28 (docker_repository_prefix)
          
-         403         300 LOAD_CONST              11 ('return')
-                     302 LOAD_NAME                3 (List)
-                     304 LOAD_NAME                8 (str)
-                     306 BINARY_SUBSCR
-                     316 BUILD_TUPLE              2
-                     318 LOAD_CONST              16 (<code object app_infra_setup, file "/home/tanke/launchflow/launchflow/clients/python/launchflow/launchflow/cli/gen/templates/fastapi/fastapi_template.py", line 402>)
-                     320 MAKE_FUNCTION            4 (annotations)
-         
-         402         322 PRECALL                  0
-                     326 CALL                     0
-         
-         403         336 STORE_NAME              23 (app_infra_setup)
-         
-         420         338 LOAD_NAME               18 (property)
-         
-         421         340 LOAD_CONST              11 ('return')
-                     342 LOAD_NAME                3 (List)
-                     344 LOAD_NAME                8 (str)
-                     346 BINARY_SUBSCR
-                     356 BUILD_TUPLE              2
-                     358 LOAD_CONST              17 (<code object app_infra_endpoints, file "/home/tanke/launchflow/launchflow/clients/python/launchflow/launchflow/cli/gen/templates/fastapi/fastapi_template.py", line 420>)
-                     360 MAKE_FUNCTION            4 (annotations)
-         
-         420         362 PRECALL                  0
-                     366 CALL                     0
-         
-         421         376 STORE_NAME              24 (app_infra_endpoints)
-         
-         429         378 LOAD_NAME               18 (property)
-         
-         430         380 LOAD_CONST              11 ('return')
-                     382 LOAD_NAME                3 (List)
-                     384 LOAD_NAME                8 (str)
-                     386 BINARY_SUBSCR
-                     396 BUILD_TUPLE              2
-                     398 LOAD_CONST              18 (<code object additional_requirements, file "/home/tanke/launchflow/launchflow/clients/python/launchflow/launchflow/cli/gen/templates/fastapi/fastapi_template.py", line 429>)
-                     400 MAKE_FUNCTION            4 (annotations)
-         
-         429         402 PRECALL                  0
-                     406 CALL                     0
-         
-         430         416 STORE_NAME              25 (additional_requirements)
-         
-         438         418 LOAD_NAME               18 (property)
-         
-         439         420 LOAD_CONST              11 ('return')
-                     422 LOAD_NAME                8 (str)
-                     424 BUILD_TUPLE              2
-                     426 LOAD_CONST              19 (<code object launchflow_service_product, file "/home/tanke/launchflow/launchflow/clients/python/launchflow/launchflow/cli/gen/templates/fastapi/fastapi_template.py", line 438>)
-                     428 MAKE_FUNCTION            4 (annotations)
-         
-         438         430 PRECALL                  0
-                     434 CALL                     0
-         
-         439         444 STORE_NAME              26 (launchflow_service_product)
-         
-         446         446 LOAD_CONST              11 ('return')
-                     448 LOAD_NAME                8 (str)
-                     450 BUILD_TUPLE              2
-                     452 LOAD_CONST              20 (<code object template_directory, file "/home/tanke/launchflow/launchflow/clients/python/launchflow/launchflow/cli/gen/templates/fastapi/fastapi_template.py", line 446>)
-                     454 MAKE_FUNCTION            4 (annotations)
-                     456 STORE_NAME              27 (template_directory)
-         
-         453         458 LOAD_NAME               18 (property)
-         
-         454         460 LOAD_CONST              11 ('return')
-                     462 LOAD_NAME                8 (str)
-                     464 BUILD_TUPLE              2
-                     466 LOAD_CONST              21 (<code object docker_repository_prefix, file "/home/tanke/launchflow/launchflow/clients/python/launchflow/launchflow/cli/gen/templates/fastapi/fastapi_template.py", line 453>)
-                     468 MAKE_FUNCTION            4 (annotations)
-         
-         453         470 PRECALL                  0
-                     474 CALL                     0
-         
-         454         484 STORE_NAME              28 (docker_repository_prefix)
-         
-         459         486 LOAD_CONST              11 ('return')
-                     488 LOAD_NAME               29 (dict)
-                     490 BUILD_TUPLE              2
-                     492 LOAD_CONST              22 (<code object context, file "/home/tanke/launchflow/launchflow/clients/python/launchflow/launchflow/cli/gen/templates/fastapi/fastapi_template.py", line 459>)
-                     494 MAKE_FUNCTION            4 (annotations)
-                     496 STORE_NAME              30 (context)
-                     498 LOAD_CONST              23 (None)
-                     500 RETURN_VALUE
+         490         474 LOAD_CONST              11 ('return')
+                     476 LOAD_NAME               29 (dict)
+                     478 BUILD_TUPLE              2
+                     480 LOAD_CONST              22 (<code object context, file "/Users/calebvandyke/code/launchflow-oss/launchflow/cli/gen/templates/fastapi/fastapi_template.py", line 490>)
+                     482 MAKE_FUNCTION            4 (annotations)
+                     484 STORE_NAME              30 (context)
+                     486 LOAD_CONST              23 (None)
+                     488 RETURN_VALUE
          consts
             'FastAPIProjectGenerator'
             'resources'
             ('aws', 'gcp')
             'cloud_provider'
             'launchflow_project_name'
             'launchflow_environment_name'
@@ -830,156 +818,156 @@
                   0a7c036a0800000000000000009b00640b7c036a0900000000000000009b
                   00640c7c036a0a00000000000000009b00640d7c006a0400000000000000
                   009b00640e7c036a090000000000000000a00b0000000000000000000000
                   000000000000000000640f640ea6020000ab0200000000000000009b0064
                   109d0ba6010000ab01000000000000000001008c64640ba00c0000000000
                   0000000000000000000000000000007c01a6010000ab0100000000000000
                   005300
-               298           0 RESUME                   0
+               321           0 RESUME                   0
                
-               301           2 LOAD_CONST               1 ('"""\nThis is the recommended place to define all launchflow Resources, but you are free to\ndefine them anywhere in your Python project.\n\nTo create find and create all resources in your current directory, run:\n    $ launchflow create\n        - or -\n    $ lf create\n"""')
+               324           2 LOAD_CONST               1 ('"""\nThis is the recommended place to define all launchflow Resources, but you are free to\ndefine them anywhere in your Python project.\n\nTo create find and create all resources in your current directory, run:\n    $ launchflow create\n        - or -\n    $ lf create\n"""')
                
-               300           4 BUILD_LIST               1
+               323           4 BUILD_LIST               1
                              6 STORE_FAST               1 (lines)
                
-               312           8 LOAD_GLOBAL              1 (NULL + len)
+               335           8 LOAD_GLOBAL              1 (NULL + len)
                             20 LOAD_FAST                0 (self)
                             22 LOAD_ATTR                1 (resources)
                             32 PRECALL                  1
                             36 CALL                     1
                             46 LOAD_CONST               2 (0)
                             48 COMPARE_OP               2 (==)
                             54 POP_JUMP_FORWARD_IF_FALSE   109 (to 274)
                
-               313          56 LOAD_FAST                0 (self)
+               336          56 LOAD_FAST                0 (self)
                             58 LOAD_ATTR                2 (cloud_provider)
                             68 LOAD_CONST               3 ('aws')
                             70 COMPARE_OP               2 (==)
                             76 POP_JUMP_FORWARD_IF_FALSE    32 (to 142)
                
-               314          78 LOAD_FAST                1 (lines)
+               337          78 LOAD_FAST                1 (lines)
                             80 LOAD_METHOD              3 (extend)
                
-               316         102 LOAD_CONST               4 ("\n# Uncomment the following line and run `launchflow create` to create an S3 bucket.\n# s3_bucket = lf.aws.S3Bucket('")
+               339         102 LOAD_CONST               4 ("\n# Uncomment the following line and run `launchflow create` to create an S3 bucket.\n# s3_bucket = lf.aws.S3Bucket('")
                
-               318         104 LOAD_FAST                0 (self)
+               341         104 LOAD_FAST                0 (self)
                            106 LOAD_ATTR                4 (launchflow_project_name)
                
-               316         116 FORMAT_VALUE             0
+               339         116 FORMAT_VALUE             0
                            118 LOAD_CONST               5 ("-bucket')\n")
                            120 BUILD_STRING             3
                
-               315         122 BUILD_LIST               1
+               338         122 BUILD_LIST               1
                
-               314         124 PRECALL                  1
+               337         124 PRECALL                  1
                            128 CALL                     1
                            138 POP_TOP
                            140 JUMP_FORWARD           194 (to 530)
                
-               322     >>  142 LOAD_FAST                0 (self)
+               345     >>  142 LOAD_FAST                0 (self)
                            144 LOAD_ATTR                2 (cloud_provider)
                            154 LOAD_CONST               6 ('gcp')
                            156 COMPARE_OP               2 (==)
                            162 POP_JUMP_FORWARD_IF_FALSE    32 (to 228)
                
-               323         164 LOAD_FAST                1 (lines)
+               346         164 LOAD_FAST                1 (lines)
                            166 LOAD_METHOD              3 (extend)
                
-               325         188 LOAD_CONST               7 ("\n# Uncomment the following line and run `launchflow create` to create a GCS bucket.\n# gcs_bucket = lf.gcp.GCSBucket('")
+               348         188 LOAD_CONST               7 ("\n# Uncomment the following line and run `launchflow create` to create a GCS bucket.\n# gcs_bucket = lf.gcp.GCSBucket('")
                
-               327         190 LOAD_FAST                0 (self)
+               350         190 LOAD_FAST                0 (self)
                            192 LOAD_ATTR                4 (launchflow_project_name)
                
-               325         202 FORMAT_VALUE             0
+               348         202 FORMAT_VALUE             0
                            204 LOAD_CONST               5 ("-bucket')\n")
                            206 BUILD_STRING             3
                
-               324         208 BUILD_LIST               1
+               347         208 BUILD_LIST               1
                
-               323         210 PRECALL                  1
+               346         210 PRECALL                  1
                            214 CALL                     1
                            224 POP_TOP
                            226 JUMP_FORWARD           151 (to 530)
                
-               332     >>  228 LOAD_GLOBAL             11 (NULL + ValueError)
+               355     >>  228 LOAD_GLOBAL             11 (NULL + ValueError)
                            240 LOAD_CONST               8 ('Unsupported cloud provider: ')
                            242 LOAD_FAST                0 (self)
                            244 LOAD_ATTR                2 (cloud_provider)
                            254 FORMAT_VALUE             0
                            256 BUILD_STRING             2
                            258 PRECALL                  1
                            262 CALL                     1
                            272 RAISE_VARARGS            1
                
-               334     >>  274 LOAD_FAST                1 (lines)
+               357     >>  274 LOAD_FAST                1 (lines)
                            276 LOAD_METHOD              6 (append)
                            298 LOAD_CONST               9 ('import launchflow as lf\n')
                            300 PRECALL                  1
                            304 CALL                     1
                            314 POP_TOP
                
-               335         316 LOAD_FAST                0 (self)
+               358         316 LOAD_FAST                0 (self)
                            318 LOAD_ATTR                1 (resources)
                            328 GET_ITER
                        >>  330 FOR_ITER                99 (to 530)
                            332 STORE_FAST               2 (resource)
                
-               336         334 LOAD_GLOBAL             15 (NULL + get_resource_info)
+               359         334 LOAD_GLOBAL             15 (NULL + get_resource_info)
                            346 LOAD_FAST                2 (resource)
                            348 PRECALL                  1
                            352 CALL                     1
                            362 STORE_FAST               3 (resource_info)
                
-               337         364 LOAD_FAST                1 (lines)
+               360         364 LOAD_FAST                1 (lines)
                            366 LOAD_METHOD              6 (append)
                
-               338         388 LOAD_CONST              10 ('\n# Docs: ')
+               361         388 LOAD_CONST              10 ('\n# Docs: ')
                
-               339         390 LOAD_FAST                3 (resource_info)
+               362         390 LOAD_FAST                3 (resource_info)
                            392 LOAD_ATTR                8 (infra_docs_url)
                
-               338         402 FORMAT_VALUE             0
+               361         402 FORMAT_VALUE             0
                            404 LOAD_CONST              11 ('\n')
                
-               340         406 LOAD_FAST                3 (resource_info)
+               363         406 LOAD_FAST                3 (resource_info)
                            408 LOAD_ATTR                9 (infra_name)
                
-               338         418 FORMAT_VALUE             0
+               361         418 FORMAT_VALUE             0
                            420 LOAD_CONST              12 (' = ')
                
-               340         422 LOAD_FAST                3 (resource_info)
+               363         422 LOAD_FAST                3 (resource_info)
                            424 LOAD_ATTR               10 (infra_lf_class)
                
-               338         434 FORMAT_VALUE             0
+               361         434 FORMAT_VALUE             0
                            436 LOAD_CONST              13 ("('")
                
-               340         438 LOAD_FAST                0 (self)
+               363         438 LOAD_FAST                0 (self)
                            440 LOAD_ATTR                4 (launchflow_project_name)
                
-               338         450 FORMAT_VALUE             0
+               361         450 FORMAT_VALUE             0
                            452 LOAD_CONST              14 ('-')
                
-               340         454 LOAD_FAST                3 (resource_info)
+               363         454 LOAD_FAST                3 (resource_info)
                            456 LOAD_ATTR                9 (infra_name)
                            466 LOAD_METHOD             11 (replace)
                            488 LOAD_CONST              15 ('_')
                            490 LOAD_CONST              14 ('-')
                            492 PRECALL                  2
                            496 CALL                     2
                
-               338         506 FORMAT_VALUE             0
+               361         506 FORMAT_VALUE             0
                            508 LOAD_CONST              16 ("')")
                            510 BUILD_STRING            11
                
-               337         512 PRECALL                  1
+               360         512 PRECALL                  1
                            516 CALL                     1
                            526 POP_TOP
                            528 JUMP_BACKWARD          100 (to 330)
                
-               342     >>  530 LOAD_CONST              11 ('\n')
+               365     >>  530 LOAD_CONST              11 ('\n')
                            532 LOAD_METHOD             12 (join)
                            554 LOAD_FAST                1 (lines)
                            556 PRECALL                  1
                            560 CALL                     1
                            570 RETURN_VALUE
                consts
                   None
@@ -999,107 +987,80 @@
                   '-'
                   '_'
                   "')"
                names      ('len', 'resources', 'cloud_provider', 'extend', 'launchflow_project_name', 'ValueError', 'append', 'get_resource_info', 'infra_docs_url', 'infra_name', 'infra_lf_class', 'replace', 'join')
                varnames   ('self', 'lines', 'resource', 'resource_info')
                freevars   ()
                cellvars   ()
-               filename   '/home/tanke/launchflow/launchflow/clients/python/launchflow/launchflow/cli/gen/templates/fastapi/fastapi_template.py'
+               filename   '/Users/calebvandyke/code/launchflow-oss/launchflow/cli/gen/templates/fastapi/fastapi_template.py'
                name       'infra_dot_py'
-               firstlineno 298
+               firstlineno 321
                lnotab
                   0x020302ff040c30011601180202020cfe06ff02ff12081601180202020c
                   fe06ff02ff12092e022a0112011e01180102010cff04020cfe04020cfe04
                   020cfe040234fe06ff1205
             code
                argcount  : 1
                nlocals   : 2
                stacksize : 3
                flags     : 3
                code
                   0x97007401000000000000000000007c006a010000000000000000a60100
-                  00ab01000000000000000064016b02000000007202640253007405000000
-                  000000000000007c006a010000000000000000a6010000ab010000000000
-                  0000007d017401000000000000000000007c006a010000000000000000a6
-                  010000ab01000000000000000064036b0200000000721474060000000000
-                  00000000007c01760073097408000000000000000000007c017600720264
-                  045300740a000000000000000000007c0176007309740c00000000000000
-                  0000007c01760072026405530064065300
-               345           0 RESUME                   0
+                  00ab0100000000000000007d017405000000000000000000007c01a60100
+                  00ab01000000000000000064016b01000000007202640253007406000000
+                  000000000000007c01760073097408000000000000000000007c01760072
+                  026403530064045300
+               368           0 RESUME                   0
                
-               347           2 LOAD_GLOBAL              1 (NULL + len)
+               370           2 LOAD_GLOBAL              1 (NULL + set)
                             14 LOAD_FAST                0 (self)
                             16 LOAD_ATTR                1 (resources)
                             26 PRECALL                  1
                             30 CALL                     1
-                            40 LOAD_CONST               1 (0)
-                            42 COMPARE_OP               2 (==)
-                            48 POP_JUMP_FORWARD_IF_FALSE     2 (to 54)
+                            40 STORE_FAST               1 (resource_set)
                
-               348          50 LOAD_CONST               2 ('from fastapi import FastAPI')
-                            52 RETURN_VALUE
-               
-               349     >>   54 LOAD_GLOBAL              5 (NULL + set)
-                            66 LOAD_FAST                0 (self)
-                            68 LOAD_ATTR                1 (resources)
-                            78 PRECALL                  1
-                            82 CALL                     1
-                            92 STORE_FAST               1 (resource_set)
-               
-               350          94 LOAD_GLOBAL              1 (NULL + len)
-                           106 LOAD_FAST                0 (self)
-                           108 LOAD_ATTR                1 (resources)
-                           118 PRECALL                  1
-                           122 CALL                     1
-                           132 LOAD_CONST               3 (1)
-                           134 COMPARE_OP               2 (==)
-                           140 POP_JUMP_FORWARD_IF_FALSE    20 (to 182)
-               
-               351         142 LOAD_GLOBAL              6 (GCSBucket)
-                           154 LOAD_FAST                1 (resource_set)
-                           156 CONTAINS_OP              0
-                           158 POP_JUMP_FORWARD_IF_TRUE     9 (to 178)
-                           160 LOAD_GLOBAL              8 (S3Bucket)
-                           172 LOAD_FAST                1 (resource_set)
-                           174 CONTAINS_OP              0
-                           176 POP_JUMP_FORWARD_IF_FALSE     2 (to 182)
-               
-               353     >>  178 LOAD_CONST               4 ('from contextlib import asynccontextmanager\n\nfrom fastapi import FastAPI')
-                           180 RETURN_VALUE
-               
-               356     >>  182 LOAD_GLOBAL             10 (CloudSQLPostgres)
-                           194 LOAD_FAST                1 (resource_set)
-                           196 CONTAINS_OP              0
-                           198 POP_JUMP_FORWARD_IF_TRUE     9 (to 218)
-                           200 LOAD_GLOBAL             12 (RDSPostgres)
-                           212 LOAD_FAST                1 (resource_set)
-                           214 CONTAINS_OP              0
-                           216 POP_JUMP_FORWARD_IF_FALSE     2 (to 222)
+               371          42 LOAD_GLOBAL              5 (NULL + len)
+                            54 LOAD_FAST                1 (resource_set)
+                            56 PRECALL                  1
+                            60 CALL                     1
+                            70 LOAD_CONST               1 (1)
+                            72 COMPARE_OP               1 (<=)
+                            78 POP_JUMP_FORWARD_IF_FALSE     2 (to 84)
+               
+               372          80 LOAD_CONST               2 ('from contextlib import asynccontextmanager\n\nfrom fastapi import FastAPI')
+                            82 RETURN_VALUE
+               
+               375     >>   84 LOAD_GLOBAL              6 (CloudSQLPostgres)
+                            96 LOAD_FAST                1 (resource_set)
+                            98 CONTAINS_OP              0
+                           100 POP_JUMP_FORWARD_IF_TRUE     9 (to 120)
+                           102 LOAD_GLOBAL              8 (RDSPostgres)
+                           114 LOAD_FAST                1 (resource_set)
+                           116 CONTAINS_OP              0
+                           118 POP_JUMP_FORWARD_IF_FALSE     2 (to 124)
                
-               357     >>  218 LOAD_CONST               5 ('from contextlib import asynccontextmanager\n\nfrom fastapi import Depends, FastAPI, HTTPException')
-                           220 RETURN_VALUE
+               376     >>  120 LOAD_CONST               3 ('from contextlib import asynccontextmanager\n\nfrom fastapi import Depends, FastAPI, HTTPException')
+                           122 RETURN_VALUE
                
-               361     >>  222 LOAD_CONST               6 ('from contextlib import asynccontextmanager\n\nfrom fastapi import Depends, FastAPI')
-                           224 RETURN_VALUE
+               380     >>  124 LOAD_CONST               4 ('from contextlib import asynccontextmanager\n\nfrom fastapi import Depends, FastAPI')
+                           126 RETURN_VALUE
                consts
                   None
-                  0
-                  'from fastapi import FastAPI'
                   1
                   'from contextlib import asynccontextmanager\n\nfrom fastapi import FastAPI'
                   'from contextlib import asynccontextmanager\n\nfrom fastapi import Depends, FastAPI, HTTPException'
                   'from contextlib import asynccontextmanager\n\nfrom fastapi import Depends, FastAPI'
-               names      ('len', 'resources', 'set', 'GCSBucket', 'S3Bucket', 'CloudSQLPostgres', 'RDSPostgres')
+               names      ('set', 'resources', 'len', 'CloudSQLPostgres', 'RDSPostgres')
                varnames   ('self', 'resource_set')
                freevars   ()
                cellvars   ()
-               filename   '/home/tanke/launchflow/launchflow/clients/python/launchflow/launchflow/cli/gen/templates/fastapi/fastapi_template.py'
+               filename   '/Users/calebvandyke/code/launchflow-oss/launchflow/cli/gen/templates/fastapi/fastapi_template.py'
                name       'fastapi_imports'
-               firstlineno 345
-               lnotab 0x020230010401280130012402040324010404
+               firstlineno 368
+               lnotab 0x020228012601040324010404
             code
                argcount  : 1
                nlocals   : 8
                stacksize : 8
                flags     : 3
                code
                   0x97007401000000000000000000007c006a010000000000000000a60100
@@ -1123,122 +1084,122 @@
                   0000000000000001007c01a0040000000000000000000000000000000000
                   00000064036404a00c000000000000000000000000000000000000000074
                   17000000000000000000007c03a6010000ab010000000000000000a60100
                   00ab0100000000000000009b009d02a6010000ab01000000000000000001
                   007c01a00800000000000000000000000000000000000000007417000000
                   000000000000007c04a6010000ab010000000000000000a6010000ab0100
                   0000000000000001007c015300
-               366           0 RESUME                   0
+               385           0 RESUME                   0
                
-               370           2 LOAD_GLOBAL              1 (NULL + len)
+               389           2 LOAD_GLOBAL              1 (NULL + len)
                             14 LOAD_FAST                0 (self)
                             16 LOAD_ATTR                1 (resources)
                             26 PRECALL                  1
                             30 CALL                     1
                             40 LOAD_CONST               1 (0)
                             42 COMPARE_OP               2 (==)
                             48 POP_JUMP_FORWARD_IF_FALSE     2 (to 54)
                
-               371          50 BUILD_LIST               0
+               390          50 BUILD_LIST               0
                             52 RETURN_VALUE
                
-               372     >>   54 BUILD_LIST               0
+               391     >>   54 BUILD_LIST               0
                             56 STORE_FAST               1 (to_return)
                
-               373          58 BUILD_LIST               0
+               392          58 BUILD_LIST               0
                             60 STORE_FAST               2 (client_imports)
                
-               374          62 BUILD_LIST               0
+               393          62 BUILD_LIST               0
                             64 STORE_FAST               3 (infra_names)
                
-               375          66 BUILD_LIST               0
+               394          66 BUILD_LIST               0
                             68 STORE_FAST               4 (app_imports)
                
-               376          70 LOAD_GLOBAL              5 (NULL + set)
+               395          70 LOAD_GLOBAL              5 (NULL + set)
                             82 PRECALL                  0
                             86 CALL                     0
                             96 STORE_FAST               5 (launchflow_imports)
                
-               377          98 LOAD_FAST                0 (self)
+               396          98 LOAD_FAST                0 (self)
                            100 LOAD_ATTR                1 (resources)
                            110 GET_ITER
                        >>  112 FOR_ITER               128 (to 370)
                            114 STORE_FAST               6 (resource)
                
-               378         116 LOAD_GLOBAL              7 (NULL + get_resource_info)
+               397         116 LOAD_GLOBAL              7 (NULL + get_resource_info)
                            128 LOAD_FAST                6 (resource)
                            130 PRECALL                  1
                            134 CALL                     1
                            144 STORE_FAST               7 (resource_info)
                
-               379         146 LOAD_FAST                3 (infra_names)
+               398         146 LOAD_FAST                3 (infra_names)
                            148 LOAD_METHOD              4 (append)
                            170 LOAD_FAST                7 (resource_info)
                            172 LOAD_ATTR                5 (infra_name)
                            182 PRECALL                  1
                            186 CALL                     1
                            196 POP_TOP
                
-               380         198 LOAD_FAST                5 (launchflow_imports)
+               399         198 LOAD_FAST                5 (launchflow_imports)
                            200 LOAD_METHOD              6 (add)
                            222 LOAD_FAST                7 (resource_info)
                            224 LOAD_ATTR                7 (launchflow_imports)
                            234 PRECALL                  1
                            238 CALL                     1
                            248 POP_TOP
                
-               381         250 LOAD_FAST                4 (app_imports)
+               400         250 LOAD_FAST                4 (app_imports)
                            252 LOAD_METHOD              8 (extend)
                            274 LOAD_FAST                7 (resource_info)
                            276 LOAD_ATTR                9 (app_imports)
                            286 PRECALL                  1
                            290 CALL                     1
                            300 POP_TOP
                
-               382         302 LOAD_FAST                7 (resource_info)
+               401         302 LOAD_FAST                7 (resource_info)
                            304 LOAD_ATTR               10 (infra_import)
                            314 POP_JUMP_FORWARD_IF_NONE    26 (to 368)
                
-               383         316 LOAD_FAST                2 (client_imports)
+               402         316 LOAD_FAST                2 (client_imports)
                            318 LOAD_METHOD              4 (append)
                            340 LOAD_FAST                7 (resource_info)
                            342 LOAD_ATTR               10 (infra_import)
                            352 PRECALL                  1
                            356 CALL                     1
                            366 POP_TOP
                        >>  368 JUMP_BACKWARD          129 (to 112)
                
-               384     >>  370 LOAD_FAST                1 (to_return)
+               403     >>  370 LOAD_FAST                1 (to_return)
                            372 LOAD_METHOD              8 (extend)
                            394 LOAD_GLOBAL             23 (NULL + sorted)
                            406 LOAD_FAST                2 (client_imports)
                            408 PRECALL                  1
                            412 CALL                     1
                            422 PRECALL                  1
                            426 CALL                     1
                            436 POP_TOP
                
-               385         438 LOAD_FAST                1 (to_return)
+               404         438 LOAD_FAST                1 (to_return)
                            440 LOAD_METHOD              4 (append)
                            462 LOAD_CONST               2 ('import launchflow')
                            464 PRECALL                  1
                            468 CALL                     1
                            478 POP_TOP
                
-               386         480 LOAD_FAST                1 (to_return)
+               405         480 LOAD_FAST                1 (to_return)
                            482 LOAD_METHOD              8 (extend)
                            504 LOAD_GLOBAL             23 (NULL + sorted)
                            516 LOAD_FAST                5 (launchflow_imports)
                            518 PRECALL                  1
                            522 CALL                     1
                            532 PRECALL                  1
                            536 CALL                     1
                            546 POP_TOP
                
-               387         548 LOAD_FAST                1 (to_return)
+               406         548 LOAD_FAST                1 (to_return)
                            550 LOAD_METHOD              4 (append)
                            572 LOAD_CONST               3 ('from app.infra import ')
                            574 LOAD_CONST               4 (', ')
                            576 LOAD_METHOD             12 (join)
                            598 LOAD_GLOBAL             23 (NULL + sorted)
                            610 LOAD_FAST                3 (infra_names)
                            612 PRECALL                  1
@@ -1247,39 +1208,39 @@
                            630 CALL                     1
                            640 FORMAT_VALUE             0
                            642 BUILD_STRING             2
                            644 PRECALL                  1
                            648 CALL                     1
                            658 POP_TOP
                
-               388         660 LOAD_FAST                1 (to_return)
+               407         660 LOAD_FAST                1 (to_return)
                            662 LOAD_METHOD              8 (extend)
                            684 LOAD_GLOBAL             23 (NULL + sorted)
                            696 LOAD_FAST                4 (app_imports)
                            698 PRECALL                  1
                            702 CALL                     1
                            712 PRECALL                  1
                            716 CALL                     1
                            726 POP_TOP
                
-               389         728 LOAD_FAST                1 (to_return)
+               408         728 LOAD_FAST                1 (to_return)
                            730 RETURN_VALUE
                consts
                   None
                   0
                   'import launchflow'
                   'from app.infra import '
                   ', '
                names      ('len', 'resources', 'set', 'get_resource_info', 'append', 'infra_name', 'add', 'launchflow_imports', 'extend', 'app_imports', 'infra_import', 'sorted', 'join')
                varnames   ('self', 'to_return', 'client_imports', 'infra_names', 'app_imports', 'launchflow_imports', 'resource', 'resource_info')
                freevars   ()
                cellvars   ()
-               filename   '/home/tanke/launchflow/launchflow/clients/python/launchflow/launchflow/cli/gen/templates/fastapi/fastapi_template.py'
+               filename   '/Users/calebvandyke/code/launchflow-oss/launchflow/cli/gen/templates/fastapi/fastapi_template.py'
                name       'app_infra_imports'
-               firstlineno 366
+               firstlineno 385
                lnotab
                   0x02043001040104010401040104011c0112011e013401340134010e0136
                   0144012a01440170014401
             code
                argcount  : 1
                nlocals   : 4
                stacksize : 4
@@ -1287,247 +1248,274 @@
                code
                   0x970067007d017c006a00000000000000000044005d327d027403000000
                   000000000000007c02a6010000ab0100000000000000007d037c036a0200
                   00000000000000811a7c01a0030000000000000000000000000000000000
                   0000007c036a020000000000000000a6010000ab01000000000000000001
                   008c336401a00400000000000000000000000000000000000000007c01a6
                   010000ab0100000000000000005300
-               392           0 RESUME                   0
+               411           0 RESUME                   0
                
-               394           2 BUILD_LIST               0
+               413           2 BUILD_LIST               0
                              4 STORE_FAST               1 (lines)
                
-               395           6 LOAD_FAST                0 (self)
+               414           6 LOAD_FAST                0 (self)
                              8 LOAD_ATTR                0 (resources)
                             18 GET_ITER
                        >>   20 FOR_ITER                50 (to 122)
                             22 STORE_FAST               2 (resource)
                
-               396          24 LOAD_GLOBAL              3 (NULL + get_resource_info)
+               415          24 LOAD_GLOBAL              3 (NULL + get_resource_info)
                             36 LOAD_FAST                2 (resource)
                             38 PRECALL                  1
                             42 CALL                     1
                             52 STORE_FAST               3 (resource_info)
                
-               397          54 LOAD_FAST                3 (resource_info)
+               416          54 LOAD_FAST                3 (resource_info)
                             56 LOAD_ATTR                2 (global_setup)
                             66 POP_JUMP_FORWARD_IF_NONE    26 (to 120)
                
-               398          68 LOAD_FAST                1 (lines)
+               417          68 LOAD_FAST                1 (lines)
                             70 LOAD_METHOD              3 (append)
                             92 LOAD_FAST                3 (resource_info)
                             94 LOAD_ATTR                2 (global_setup)
                            104 PRECALL                  1
                            108 CALL                     1
                            118 POP_TOP
                        >>  120 JUMP_BACKWARD           51 (to 20)
                
-               399     >>  122 LOAD_CONST               1 ('\n')
+               418     >>  122 LOAD_CONST               1 ('\n')
                            124 LOAD_METHOD              4 (join)
                            146 LOAD_FAST                1 (lines)
                            148 PRECALL                  1
                            152 CALL                     1
                            162 RETURN_VALUE
                consts
                   None
                   '\n'
                names      ('resources', 'get_resource_info', 'global_setup', 'append', 'join')
                varnames   ('self', 'lines', 'resource', 'resource_info')
                freevars   ()
                cellvars   ()
-               filename   '/home/tanke/launchflow/launchflow/clients/python/launchflow/launchflow/cli/gen/templates/fastapi/fastapi_template.py'
+               filename   '/Users/calebvandyke/code/launchflow-oss/launchflow/cli/gen/templates/fastapi/fastapi_template.py'
                name       'app_global_setup'
-               firstlineno 392
+               firstlineno 411
                lnotab 0x0202040112011e010e013601
             code
                argcount  : 1
                nlocals   : 5
                stacksize : 7
                flags     : 3
                code
-                  0x970067007d0167007d027c006a00000000000000000044005d4c7d0374
-                  03000000000000000000007c03a6010000ab0100000000000000007d047c
-                  01a00200000000000000000000000000000000000000007c046a03000000
-                  0000000000a6010000ab01000000000000000001007c046a040000000000
-                  000000811a7c02a00200000000000000000000000000000000000000007c
-                  046a040000000000000000a6010000ab01000000000000000001008c4d64
-                  01a0050000000000000000000000000000000000000000640264036404a0
-                  0500000000000000000000000000000000000000007c01a6010000ab0100
-                  000000000000009b0064059d0367027c027a000000a6010000ab01000000
-                  00000000005300
-               402           0 RESUME                   0
-               
-               404           2 BUILD_LIST               0
-                             4 STORE_FAST               1 (infra_names)
-               
-               405           6 BUILD_LIST               0
-                             8 STORE_FAST               2 (infra_steps)
-               
-               406          10 LOAD_FAST                0 (self)
-                            12 LOAD_ATTR                0 (resources)
-                            22 GET_ITER
-                       >>   24 FOR_ITER                76 (to 178)
-                            26 STORE_FAST               3 (resource)
-               
-               407          28 LOAD_GLOBAL              3 (NULL + get_resource_info)
-                            40 LOAD_FAST                3 (resource)
-                            42 PRECALL                  1
-                            46 CALL                     1
-                            56 STORE_FAST               4 (resource_info)
-               
-               408          58 LOAD_FAST                1 (infra_names)
-                            60 LOAD_METHOD              2 (append)
-                            82 LOAD_FAST                4 (resource_info)
-                            84 LOAD_ATTR                3 (infra_name)
-                            94 PRECALL                  1
-                            98 CALL                     1
-                           108 POP_TOP
-               
-               409         110 LOAD_FAST                4 (resource_info)
-                           112 LOAD_ATTR                4 (fastapi_setup)
-                           122 POP_JUMP_FORWARD_IF_NONE    26 (to 176)
-               
-               410         124 LOAD_FAST                2 (infra_steps)
-                           126 LOAD_METHOD              2 (append)
-                           148 LOAD_FAST                4 (resource_info)
-                           150 LOAD_ATTR                4 (fastapi_setup)
-                           160 PRECALL                  1
-                           164 CALL                     1
-                           174 POP_TOP
-                       >>  176 JUMP_BACKWARD           77 (to 24)
-               
-               411     >>  178 LOAD_CONST               1 ('\n')
-                           180 LOAD_METHOD              5 (join)
-               
-               413         202 LOAD_CONST               2 ('# Connects to all resources on startup')
-               
-               414         204 LOAD_CONST               3 ('    await launchflow.connect_all(')
-                           206 LOAD_CONST               4 (', ')
-                           208 LOAD_METHOD              5 (join)
-                           230 LOAD_FAST                1 (infra_names)
-                           232 PRECALL                  1
-                           236 CALL                     1
-                           246 FORMAT_VALUE             0
-                           248 LOAD_CONST               5 (')')
-                           250 BUILD_STRING             3
-               
-               412         252 BUILD_LIST               2
-               
-               416         254 LOAD_FAST                2 (infra_steps)
-               
-               412         256 BINARY_OP                0 (+)
-               
-               411         260 PRECALL                  1
-                           264 CALL                     1
-                           274 RETURN_VALUE
+                  0x97007401000000000000000000007c006a010000000000000000a60100
+                  00ab01000000000000000064016b020000000072176402a0020000000000
+                  00000000000000000000000000000067006403a201a6010000ab01000000
+                  0000000000530067007d0167007d027c006a01000000000000000044005d
+                  4c7d037407000000000000000000007c03a6010000ab0100000000000000
+                  007d047c01a00400000000000000000000000000000000000000007c046a
+                  050000000000000000a6010000ab01000000000000000001007c046a0600
+                  00000000000000811a7c02a0040000000000000000000000000000000000
+                  0000007c046a060000000000000000a6010000ab01000000000000000001
+                  008c4d6402a0020000000000000000000000000000000000000000640464
+                  056406a00200000000000000000000000000000000000000007c01a60100
+                  00ab0100000000000000009b0064079d0367027c027a000000a6010000ab
+                  0100000000000000005300
+               421           0 RESUME                   0
+               
+               423           2 LOAD_GLOBAL              1 (NULL + len)
+                            14 LOAD_FAST                0 (self)
+                            16 LOAD_ATTR                1 (resources)
+                            26 PRECALL                  1
+                            30 CALL                     1
+                            40 LOAD_CONST               1 (0)
+                            42 COMPARE_OP               2 (==)
+                            48 POP_JUMP_FORWARD_IF_FALSE    23 (to 96)
+               
+               424          50 LOAD_CONST               2 ('\n')
+                            52 LOAD_METHOD              2 (join)
+               
+               425          74 BUILD_LIST               0
+                            76 LOAD_CONST               3 (('# NOTE: This is where you connect resources on startup', '    # For example, if you had a GCS bucket you would do:', '    # await gcs_bucket.connect()'))
+                            78 LIST_EXTEND              1
+               
+               424          80 PRECALL                  1
+                            84 CALL                     1
+                            94 RETURN_VALUE
+               
+               431     >>   96 BUILD_LIST               0
+                            98 STORE_FAST               1 (infra_names)
+               
+               432         100 BUILD_LIST               0
+                           102 STORE_FAST               2 (infra_steps)
+               
+               433         104 LOAD_FAST                0 (self)
+                           106 LOAD_ATTR                1 (resources)
+                           116 GET_ITER
+                       >>  118 FOR_ITER                76 (to 272)
+                           120 STORE_FAST               3 (resource)
+               
+               434         122 LOAD_GLOBAL              7 (NULL + get_resource_info)
+                           134 LOAD_FAST                3 (resource)
+                           136 PRECALL                  1
+                           140 CALL                     1
+                           150 STORE_FAST               4 (resource_info)
+               
+               435         152 LOAD_FAST                1 (infra_names)
+                           154 LOAD_METHOD              4 (append)
+                           176 LOAD_FAST                4 (resource_info)
+                           178 LOAD_ATTR                5 (infra_name)
+                           188 PRECALL                  1
+                           192 CALL                     1
+                           202 POP_TOP
+               
+               436         204 LOAD_FAST                4 (resource_info)
+                           206 LOAD_ATTR                6 (fastapi_setup)
+                           216 POP_JUMP_FORWARD_IF_NONE    26 (to 270)
+               
+               437         218 LOAD_FAST                2 (infra_steps)
+                           220 LOAD_METHOD              4 (append)
+                           242 LOAD_FAST                4 (resource_info)
+                           244 LOAD_ATTR                6 (fastapi_setup)
+                           254 PRECALL                  1
+                           258 CALL                     1
+                           268 POP_TOP
+                       >>  270 JUMP_BACKWARD           77 (to 118)
+               
+               438     >>  272 LOAD_CONST               2 ('\n')
+                           274 LOAD_METHOD              2 (join)
+               
+               440         296 LOAD_CONST               4 ('# Connects to all resources on startup')
+               
+               441         298 LOAD_CONST               5 ('    await launchflow.connect_all(')
+                           300 LOAD_CONST               6 (', ')
+                           302 LOAD_METHOD              2 (join)
+                           324 LOAD_FAST                1 (infra_names)
+                           326 PRECALL                  1
+                           330 CALL                     1
+                           340 FORMAT_VALUE             0
+                           342 LOAD_CONST               7 (')')
+                           344 BUILD_STRING             3
+               
+               439         346 BUILD_LIST               2
+               
+               443         348 LOAD_FAST                2 (infra_steps)
+               
+               439         350 BINARY_OP                0 (+)
+               
+               438         354 PRECALL                  1
+                           358 CALL                     1
+                           368 RETURN_VALUE
                consts
                   None
+                  0
                   '\n'
+                  ('# NOTE: This is where you connect resources on startup', '    # For example, if you had a GCS bucket you would do:', '    # await gcs_bucket.connect()')
                   '# Connects to all resources on startup'
                   '    await launchflow.connect_all('
                   ', '
                   ')'
-               names      ('resources', 'get_resource_info', 'append', 'infra_name', 'fastapi_setup', 'join')
+               names      ('len', 'resources', 'join', 'get_resource_info', 'append', 'infra_name', 'fastapi_setup')
                varnames   ('self', 'infra_names', 'infra_steps', 'resource', 'resource_info')
                freevars   ()
                cellvars   ()
-               filename   '/home/tanke/launchflow/launchflow/clients/python/launchflow/launchflow/cli/gen/templates/fastapi/fastapi_template.py'
+               filename   '/Users/calebvandyke/code/launchflow-oss/launchflow/cli/gen/templates/fastapi/fastapi_template.py'
                name       'app_infra_setup'
-               firstlineno 402
-               lnotab 0x02020401040112011e0134010e0136011802020130fe020402fc04ff
+               firstlineno 421
+               lnotab
+                  0x02023001180106ff10070401040112011e0134010e0136011802020130
+                  fe020402fc04ff
             code
                argcount  : 1
                nlocals   : 4
                stacksize : 4
                flags     : 3
                code
                   0x970067007d017c006a00000000000000000044005d2b7d027403000000
                   000000000000007c02a6010000ab0100000000000000007d037c01a00200
                   000000000000000000000000000000000000007c036a0300000000000000
                   00a6010000ab01000000000000000001008c2c7c015300
-               420           0 RESUME                   0
+               447           0 RESUME                   0
                
-               422           2 BUILD_LIST               0
+               449           2 BUILD_LIST               0
                              4 STORE_FAST               1 (endpoints)
                
-               423           6 LOAD_FAST                0 (self)
+               450           6 LOAD_FAST                0 (self)
                              8 LOAD_ATTR                0 (resources)
                             18 GET_ITER
                        >>   20 FOR_ITER                43 (to 108)
                             22 STORE_FAST               2 (resource)
                
-               424          24 LOAD_GLOBAL              3 (NULL + get_resource_info)
+               451          24 LOAD_GLOBAL              3 (NULL + get_resource_info)
                             36 LOAD_FAST                2 (resource)
                             38 PRECALL                  1
                             42 CALL                     1
                             52 STORE_FAST               3 (resource_info)
                
-               425          54 LOAD_FAST                1 (endpoints)
+               452          54 LOAD_FAST                1 (endpoints)
                             56 LOAD_METHOD              2 (append)
                             78 LOAD_FAST                3 (resource_info)
                             80 LOAD_ATTR                3 (fastapi_test_endpoint)
                             90 PRECALL                  1
                             94 CALL                     1
                            104 POP_TOP
                            106 JUMP_BACKWARD           44 (to 20)
                
-               426     >>  108 LOAD_FAST                1 (endpoints)
+               453     >>  108 LOAD_FAST                1 (endpoints)
                            110 RETURN_VALUE
                consts
                   None
                names      ('resources', 'get_resource_info', 'append', 'fastapi_test_endpoint')
                varnames   ('self', 'endpoints', 'resource', 'resource_info')
                freevars   ()
                cellvars   ()
-               filename   '/home/tanke/launchflow/launchflow/clients/python/launchflow/launchflow/cli/gen/templates/fastapi/fastapi_template.py'
+               filename   '/Users/calebvandyke/code/launchflow-oss/launchflow/cli/gen/templates/fastapi/fastapi_template.py'
                name       'app_infra_endpoints'
-               firstlineno 420
+               firstlineno 447
                lnotab 0x0202040112011e013601
             code
                argcount  : 1
                nlocals   : 4
                stacksize : 5
                flags     : 3
                code
                   0x9700740100000000000000000000a6000000ab0000000000000000007d
                   017c006a01000000000000000044005d2b7d027405000000000000000000
                   007c02a6010000ab0100000000000000007d037c01a00300000000000000
                   000000000000000000000000007c036a040000000000000000a6010000ab
                   01000000000000000001008c2c6401a00500000000000000000000000000
                   00000000000000740d000000000000000000007c01a6010000ab01000000
                   0000000000a6010000ab0100000000000000005300
-               429           0 RESUME                   0
+               456           0 RESUME                   0
                
-               431           2 LOAD_GLOBAL              1 (NULL + set)
+               458           2 LOAD_GLOBAL              1 (NULL + set)
                             14 PRECALL                  0
                             18 CALL                     0
                             28 STORE_FAST               1 (requirements)
                
-               432          30 LOAD_FAST                0 (self)
+               459          30 LOAD_FAST                0 (self)
                             32 LOAD_ATTR                1 (resources)
                             42 GET_ITER
                        >>   44 FOR_ITER                43 (to 132)
                             46 STORE_FAST               2 (resource)
                
-               433          48 LOAD_GLOBAL              5 (NULL + get_resource_info)
+               460          48 LOAD_GLOBAL              5 (NULL + get_resource_info)
                             60 LOAD_FAST                2 (resource)
                             62 PRECALL                  1
                             66 CALL                     1
                             76 STORE_FAST               3 (resource_info)
                
-               434          78 LOAD_FAST                1 (requirements)
+               461          78 LOAD_FAST                1 (requirements)
                             80 LOAD_METHOD              3 (update)
                            102 LOAD_FAST                3 (resource_info)
                            104 LOAD_ATTR                4 (requirements)
                            114 PRECALL                  1
                            118 CALL                     1
                            128 POP_TOP
                            130 JUMP_BACKWARD           44 (to 44)
                
-               435     >>  132 LOAD_CONST               1 ('\n')
+               462     >>  132 LOAD_CONST               1 ('\n')
                            134 LOAD_METHOD              5 (join)
                            156 LOAD_GLOBAL             13 (NULL + sorted)
                            168 LOAD_FAST                1 (requirements)
                            170 PRECALL                  1
                            174 CALL                     1
                            184 PRECALL                  1
                            188 CALL                     1
@@ -1535,49 +1523,49 @@
                consts
                   None
                   '\n'
                names      ('set', 'resources', 'get_resource_info', 'update', 'requirements', 'join', 'sorted')
                varnames   ('self', 'requirements', 'resource', 'resource_info')
                freevars   ()
                cellvars   ()
-               filename   '/home/tanke/launchflow/launchflow/clients/python/launchflow/launchflow/cli/gen/templates/fastapi/fastapi_template.py'
+               filename   '/Users/calebvandyke/code/launchflow-oss/launchflow/cli/gen/templates/fastapi/fastapi_template.py'
                name       'additional_requirements'
-               firstlineno 429
+               firstlineno 456
                lnotab 0x02021c0112011e013601
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 4
                flags     : 3
                code
                   0x97007c006a00000000000000000064016b02000000007202640253007c
                   006a00000000000000000064036b02000000007202640453007403000000
                   0000000000000064057c006a0000000000000000009b009d02a6010000ab
                   0100000000000000008201
-               438           0 RESUME                   0
+               465           0 RESUME                   0
                
-               440           2 LOAD_FAST                0 (self)
+               467           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (cloud_provider)
                             14 LOAD_CONST               1 ('aws')
                             16 COMPARE_OP               2 (==)
                             22 POP_JUMP_FORWARD_IF_FALSE     2 (to 28)
                
-               441          24 LOAD_CONST               2 ('aws_ecs_fargate')
+               468          24 LOAD_CONST               2 ('aws_ecs_fargate')
                             26 RETURN_VALUE
                
-               442     >>   28 LOAD_FAST                0 (self)
+               469     >>   28 LOAD_FAST                0 (self)
                             30 LOAD_ATTR                0 (cloud_provider)
                             40 LOAD_CONST               3 ('gcp')
                             42 COMPARE_OP               2 (==)
                             48 POP_JUMP_FORWARD_IF_FALSE     2 (to 54)
                
-               443          50 LOAD_CONST               4 ('gcp_cloud_run')
+               470          50 LOAD_CONST               4 ('gcp_cloud_run')
                             52 RETURN_VALUE
                
-               444     >>   54 LOAD_GLOBAL              3 (NULL + ValueError)
+               471     >>   54 LOAD_GLOBAL              3 (NULL + ValueError)
                             66 LOAD_CONST               5 ('Unsupported cloud provider: ')
                             68 LOAD_FAST                0 (self)
                             70 LOAD_ATTR                0 (cloud_provider)
                             80 FORMAT_VALUE             0
                             82 BUILD_STRING             2
                             84 PRECALL                  1
                             88 CALL                     1
@@ -1589,154 +1577,163 @@
                   'gcp'
                   'gcp_cloud_run'
                   'Unsupported cloud provider: '
                names      ('cloud_provider', 'ValueError')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   '/home/tanke/launchflow/launchflow/clients/python/launchflow/launchflow/cli/gen/templates/fastapi/fastapi_template.py'
+               filename   '/Users/calebvandyke/code/launchflow-oss/launchflow/cli/gen/templates/fastapi/fastapi_template.py'
                name       'launchflow_service_product'
-               firstlineno 438
+               firstlineno 465
                lnotab 0x02021601040116010401
             code
                argcount  : 1
-               nlocals   : 1
+               nlocals   : 3
                stacksize : 3
                flags     : 3
                code
-                  0x9700740000000000000000000000640184007c006a0100000000000000
-                  004400a6000000ab00000000000000000076007318740400000000000000
-                  000000640284007c006a0100000000000000004400a6000000ab00000000
-                  0000000000760072026403530064045300
-               446           0 RESUME                   0
-               
-               447           2 LOAD_GLOBAL              0 (CloudSQLPostgres)
-                            14 LOAD_CONST               1 (<code object <listcomp>, file "/home/tanke/launchflow/launchflow/clients/python/launchflow/launchflow/cli/gen/templates/fastapi/fastapi_template.py", line 447>)
-                            16 MAKE_FUNCTION            0
-               
-               448          18 LOAD_FAST                0 (self)
-                            20 LOAD_ATTR                1 (resources)
-               
-               447          30 GET_ITER
-                            32 PRECALL                  0
-                            36 CALL                     0
-                            46 CONTAINS_OP              0
-                            48 POP_JUMP_FORWARD_IF_TRUE    24 (to 98)
-               
-               449          50 LOAD_GLOBAL              4 (RDSPostgres)
-                            62 LOAD_CONST               2 (<code object <listcomp>, file "/home/tanke/launchflow/launchflow/clients/python/launchflow/launchflow/cli/gen/templates/fastapi/fastapi_template.py", line 449>)
-                            64 MAKE_FUNCTION            0
-                            66 LOAD_FAST                0 (self)
-                            68 LOAD_ATTR                1 (resources)
-                            78 GET_ITER
-                            80 PRECALL                  0
-                            84 CALL                     0
-                            94 CONTAINS_OP              0
-                            96 POP_JUMP_FORWARD_IF_FALSE     2 (to 102)
-               
-               450     >>   98 LOAD_CONST               3 ('launchflow.cli.gen.templates.fastapi._postgres_template')
-                           100 RETURN_VALUE
-               
-               451     >>  102 LOAD_CONST               4 ('launchflow.cli.gen.templates.fastapi._simple_template')
-                           104 RETURN_VALUE
+                  0x970064017d0164027d02740000000000000000000000640384007c006a
+                  0100000000000000004400a6000000ab0000000000000000007600731874
+                  0400000000000000000000640484007c006a0100000000000000004400a6
+                  000000ab0000000000000000007600720264057d027c017c0266025300
+               473           0 RESUME                   0
+               
+               474           2 LOAD_CONST               1 ('launchflow.cli.gen.templates.fastapi')
+                             4 STORE_FAST               1 (template_dir)
+               
+               475           6 LOAD_CONST               2 ('_simple_template')
+                             8 STORE_FAST               2 (template_name)
+               
+               477          10 LOAD_GLOBAL              0 (CloudSQLPostgres)
+                            22 LOAD_CONST               3 (<code object <listcomp>, file "/Users/calebvandyke/code/launchflow-oss/launchflow/cli/gen/templates/fastapi/fastapi_template.py", line 477>)
+                            24 MAKE_FUNCTION            0
+               
+               478          26 LOAD_FAST                0 (self)
+                            28 LOAD_ATTR                1 (resources)
+               
+               477          38 GET_ITER
+                            40 PRECALL                  0
+                            44 CALL                     0
+                            54 CONTAINS_OP              0
+                            56 POP_JUMP_FORWARD_IF_TRUE    24 (to 106)
+               
+               479          58 LOAD_GLOBAL              4 (RDSPostgres)
+                            70 LOAD_CONST               4 (<code object <listcomp>, file "/Users/calebvandyke/code/launchflow-oss/launchflow/cli/gen/templates/fastapi/fastapi_template.py", line 479>)
+                            72 MAKE_FUNCTION            0
+                            74 LOAD_FAST                0 (self)
+                            76 LOAD_ATTR                1 (resources)
+                            86 GET_ITER
+                            88 PRECALL                  0
+                            92 CALL                     0
+                           102 CONTAINS_OP              0
+                           104 POP_JUMP_FORWARD_IF_FALSE     2 (to 110)
+               
+               480     >>  106 LOAD_CONST               5 ('_postgres_template')
+                           108 STORE_FAST               2 (template_name)
+               
+               482     >>  110 LOAD_FAST                1 (template_dir)
+                           112 LOAD_FAST                2 (template_name)
+                           114 BUILD_TUPLE              2
+                           116 RETURN_VALUE
                consts
                   None
+                  'launchflow.cli.gen.templates.fastapi'
+                  '_simple_template'
                   code
                      argcount  : 1
                      nlocals   : 2
                      stacksize : 3
                      flags     : 19
                      code 0x970067007c005d047d017c0191028c055300
-                     447           0 RESUME                   0
+                     477           0 RESUME                   0
                                    2 BUILD_LIST               0
                                    4 LOAD_FAST                0 (.0)
                              >>    6 FOR_ITER                 4 (to 16)
                      
-                     448           8 STORE_FAST               1 (resource)
+                     478           8 STORE_FAST               1 (resource)
                                   10 LOAD_FAST                1 (resource)
                      
-                     447          12 LIST_APPEND              2
+                     477          12 LIST_APPEND              2
                                   14 JUMP_BACKWARD            5 (to 6)
                              >>   16 RETURN_VALUE
                      consts
                      names      ()
                      varnames   ('.0', 'resource')
                      freevars   ()
                      cellvars   ()
-                     filename   '/home/tanke/launchflow/launchflow/clients/python/launchflow/launchflow/cli/gen/templates/fastapi/fastapi_template.py'
+                     filename   '/Users/calebvandyke/code/launchflow-oss/launchflow/cli/gen/templates/fastapi/fastapi_template.py'
                      name       '<listcomp>'
-                     firstlineno 447
+                     firstlineno 477
                      lnotab 0x080104ff
                   code
                      argcount  : 1
                      nlocals   : 2
                      stacksize : 3
                      flags     : 19
                      code 0x970067007c005d047d017c0191028c055300
-                     449           0 RESUME                   0
+                     479           0 RESUME                   0
                                    2 BUILD_LIST               0
                                    4 LOAD_FAST                0 (.0)
                              >>    6 FOR_ITER                 4 (to 16)
                                    8 STORE_FAST               1 (resource)
                                   10 LOAD_FAST                1 (resource)
                                   12 LIST_APPEND              2
                                   14 JUMP_BACKWARD            5 (to 6)
                              >>   16 RETURN_VALUE
                      consts
                      names      ()
                      varnames   ('.0', 'resource')
                      freevars   ()
                      cellvars   ()
-                     filename   '/home/tanke/launchflow/launchflow/clients/python/launchflow/launchflow/cli/gen/templates/fastapi/fastapi_template.py'
+                     filename   '/Users/calebvandyke/code/launchflow-oss/launchflow/cli/gen/templates/fastapi/fastapi_template.py'
                      name       '<listcomp>'
-                     firstlineno 449
+                     firstlineno 479
                      lnotab 0x
-                  'launchflow.cli.gen.templates.fastapi._postgres_template'
-                  'launchflow.cli.gen.templates.fastapi._simple_template'
+                  '_postgres_template'
                names      ('CloudSQLPostgres', 'resources', 'RDSPostgres')
-               varnames   ('self',)
+               varnames   ('self', 'template_dir', 'template_name')
                freevars   ()
                cellvars   ()
-               filename   '/home/tanke/launchflow/launchflow/clients/python/launchflow/launchflow/cli/gen/templates/fastapi/fastapi_template.py'
-               name       'template_directory'
-               firstlineno 446
-               lnotab 0x020110010cff140230010401
+               filename   '/Users/calebvandyke/code/launchflow-oss/launchflow/cli/gen/templates/fastapi/fastapi_template.py'
+               name       'template_path_info'
+               firstlineno 473
+               lnotab 0x02010401040210010cff140230010402
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c006a00000000000000000064016b020000000072026402530064
                   035300
-               453           0 RESUME                   0
+               484           0 RESUME                   0
                
-               455           2 LOAD_FAST                0 (self)
+               486           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (cloud_provider)
                             14 LOAD_CONST               1 ('aws')
                             16 COMPARE_OP               2 (==)
                             22 POP_JUMP_FORWARD_IF_FALSE     2 (to 28)
                
-               456          24 LOAD_CONST               2 ('public.ecr.aws/docker/library/')
+               487          24 LOAD_CONST               2 ('public.ecr.aws/docker/library/')
                             26 RETURN_VALUE
                
-               457     >>   28 LOAD_CONST               3 ('')
+               488     >>   28 LOAD_CONST               3 ('')
                             30 RETURN_VALUE
                consts
                   None
                   'aws'
                   'public.ecr.aws/docker/library/'
                   ''
                names      ('cloud_provider',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   '/home/tanke/launchflow/launchflow/clients/python/launchflow/launchflow/cli/gen/templates/fastapi/fastapi_template.py'
+               filename   '/Users/calebvandyke/code/launchflow-oss/launchflow/cli/gen/templates/fastapi/fastapi_template.py'
                name       'docker_repository_prefix'
-               firstlineno 453
+               firstlineno 484
                lnotab 0x020216010401
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 3
                flags     : 3
                code
@@ -1745,113 +1742,113 @@
                   00000000000000930164057c006a040000000000000000930164067c006a
                   050000000000000000930164077c006a060000000000000000930164087c
                   006a070000000000000000930164097c006a080000000000000000930164
                   0a7c006a0900000000000000009301640b7c006a0a000000000000000093
                   01640c7c006a0b00000000000000009301640d7c006a0c00000000000000
                   009301640e7c006a0d00000000000000009301640f7c006a0e0000000000
                   000000930164107c006a0f000000000000000093015300
-               459           0 RESUME                   0
+               490           0 RESUME                   0
                
-               460           2 BUILD_MAP                0
+               491           2 BUILD_MAP                0
                
-               462           4 LOAD_CONST               1 ('cloud_provider')
+               493           4 LOAD_CONST               1 ('cloud_provider')
                              6 LOAD_FAST                0 (self)
                              8 LOAD_ATTR                0 (cloud_provider)
                
-               460          18 MAP_ADD                  1
+               491          18 MAP_ADD                  1
                
-               463          20 LOAD_CONST               2 ('additional_requirements')
+               494          20 LOAD_CONST               2 ('additional_requirements')
                             22 LOAD_FAST                0 (self)
                             24 LOAD_ATTR                1 (additional_requirements)
                
-               460          34 MAP_ADD                  1
+               491          34 MAP_ADD                  1
                
-               465          36 LOAD_CONST               3 ('launchflow_project_name')
+               496          36 LOAD_CONST               3 ('launchflow_project_name')
                             38 LOAD_FAST                0 (self)
                             40 LOAD_ATTR                2 (launchflow_project_name)
                
-               460          50 MAP_ADD                  1
+               491          50 MAP_ADD                  1
                
-               466          52 LOAD_CONST               4 ('launchflow_environment_name')
+               497          52 LOAD_CONST               4 ('launchflow_environment_name')
                             54 LOAD_FAST                0 (self)
                             56 LOAD_ATTR                3 (launchflow_environment_name)
                
-               460          66 MAP_ADD                  1
+               491          66 MAP_ADD                  1
                
-               467          68 LOAD_CONST               5 ('launchflow_service_name')
+               498          68 LOAD_CONST               5 ('launchflow_service_name')
                             70 LOAD_FAST                0 (self)
                             72 LOAD_ATTR                4 (launchflow_service_name)
                
-               460          82 MAP_ADD                  1
+               491          82 MAP_ADD                  1
                
-               468          84 LOAD_CONST               6 ('launchflow_service_product')
+               499          84 LOAD_CONST               6 ('launchflow_service_product')
                             86 LOAD_FAST                0 (self)
                             88 LOAD_ATTR                5 (launchflow_service_product)
                
-               460          98 MAP_ADD                  1
+               491          98 MAP_ADD                  1
                
-               470         100 LOAD_CONST               7 ('docker_repository_prefix')
+               501         100 LOAD_CONST               7 ('docker_repository_prefix')
                            102 LOAD_FAST                0 (self)
                            104 LOAD_ATTR                6 (docker_repository_prefix)
                
-               460         114 MAP_ADD                  1
+               491         114 MAP_ADD                  1
                
-               471         116 LOAD_CONST               8 ('python_major_version')
+               502         116 LOAD_CONST               8 ('python_major_version')
                            118 LOAD_FAST                0 (self)
                            120 LOAD_ATTR                7 (python_major_version)
                
-               460         130 MAP_ADD                  1
+               491         130 MAP_ADD                  1
                
-               472         132 LOAD_CONST               9 ('python_minor_version')
+               503         132 LOAD_CONST               9 ('python_minor_version')
                            134 LOAD_FAST                0 (self)
                            136 LOAD_ATTR                8 (python_minor_version)
                
-               460         146 MAP_ADD                  1
+               491         146 MAP_ADD                  1
                
-               473         148 LOAD_CONST              10 ('port')
+               504         148 LOAD_CONST              10 ('port')
                            150 LOAD_FAST                0 (self)
                            152 LOAD_ATTR                9 (port)
                
-               460         162 MAP_ADD                  1
+               491         162 MAP_ADD                  1
                
-               475         164 LOAD_CONST              11 ('infra_dot_py')
+               506         164 LOAD_CONST              11 ('infra_dot_py')
                            166 LOAD_FAST                0 (self)
                            168 LOAD_ATTR               10 (infra_dot_py)
                
-               460         178 MAP_ADD                  1
+               491         178 MAP_ADD                  1
                
-               477         180 LOAD_CONST              12 ('fastapi_imports')
+               508         180 LOAD_CONST              12 ('fastapi_imports')
                            182 LOAD_FAST                0 (self)
                            184 LOAD_ATTR               11 (fastapi_imports)
                
-               460         194 MAP_ADD                  1
+               491         194 MAP_ADD                  1
                
-               478         196 LOAD_CONST              13 ('app_infra_imports')
+               509         196 LOAD_CONST              13 ('app_infra_imports')
                            198 LOAD_FAST                0 (self)
                            200 LOAD_ATTR               12 (app_infra_imports)
                
-               460         210 MAP_ADD                  1
+               491         210 MAP_ADD                  1
                
-               479         212 LOAD_CONST              14 ('app_global_setup')
+               510         212 LOAD_CONST              14 ('app_global_setup')
                            214 LOAD_FAST                0 (self)
                            216 LOAD_ATTR               13 (app_global_setup)
                
-               460         226 MAP_ADD                  1
+               491         226 MAP_ADD                  1
                
-               480         228 LOAD_CONST              15 ('app_infra_setup')
+               511         228 LOAD_CONST              15 ('app_infra_setup')
                            230 LOAD_FAST                0 (self)
                            232 LOAD_ATTR               14 (app_infra_setup)
                
-               460         242 MAP_ADD                  1
+               491         242 MAP_ADD                  1
                
-               481         244 LOAD_CONST              16 ('app_infra_endpoints')
+               512         244 LOAD_CONST              16 ('app_infra_endpoints')
                            246 LOAD_FAST                0 (self)
                            248 LOAD_ATTR               15 (app_infra_endpoints)
                
-               460         258 MAP_ADD                  1
+               491         258 MAP_ADD                  1
                            260 RETURN_VALUE
                consts
                   None
                   'cloud_provider'
                   'additional_requirements'
                   'launchflow_project_name'
                   'launchflow_environment_name'
@@ -1867,52 +1864,44 @@
                   'app_global_setup'
                   'app_infra_setup'
                   'app_infra_endpoints'
                names      ('cloud_provider', 'additional_requirements', 'launchflow_project_name', 'launchflow_environment_name', 'launchflow_service_name', 'launchflow_service_product', 'docker_repository_prefix', 'python_major_version', 'python_minor_version', 'port', 'infra_dot_py', 'fastapi_imports', 'app_infra_imports', 'app_global_setup', 'app_infra_setup', 'app_infra_endpoints')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   '/home/tanke/launchflow/launchflow/clients/python/launchflow/launchflow/cli/gen/templates/fastapi/fastapi_template.py'
+               filename   '/Users/calebvandyke/code/launchflow-oss/launchflow/cli/gen/templates/fastapi/fastapi_template.py'
                name       'context'
-               firstlineno 459
+               firstlineno 490
                lnotab
                   0x020102020efe02030efd02050efb02060efa02070ef902080ef8020a0e
                   f6020b0ef5020c0ef4020d0ef3020f0ef102110eef02120eee02130eed02
                   140eec02150eeb
             None
-         names      ('__name__', '__module__', '__qualname__', 'List', 'Type', 'Resource', '__annotations__', 'Literal', 'str', 'launchflow_service_name', 'sys', 'version_info', 'major', 'python_major_version', 'int', 'minor', 'python_minor_version', 'port', 'property', 'infra_dot_py', 'fastapi_imports', 'app_infra_imports', 'app_global_setup', 'app_infra_setup', 'app_infra_endpoints', 'additional_requirements', 'launchflow_service_product', 'template_directory', 'docker_repository_prefix', 'dict', 'context')
+         names      ('__name__', '__module__', '__qualname__', 'List', 'Type', 'Resource', '__annotations__', 'Literal', 'str', 'launchflow_service_name', 'sys', 'version_info', 'major', 'python_major_version', 'int', 'minor', 'python_minor_version', 'port', 'property', 'infra_dot_py', 'fastapi_imports', 'app_infra_imports', 'app_global_setup', 'app_infra_setup', 'app_infra_endpoints', 'additional_requirements', 'launchflow_service_product', 'template_path_info', 'docker_repository_prefix', 'dict', 'context')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/home/tanke/launchflow/launchflow/clients/python/launchflow/launchflow/cli/gen/templates/fastapi/fastapi_template.py'
+         filename   '/Users/calebvandyke/code/launchflow-oss/launchflow/cli/gen/templates/fastapi/fastapi_template.py'
          name       'FastAPIProjectGenerator'
-         firstlineno 283
+         firstlineno 306
          lnotab
             0x0c02220216020a010a010e0222012201040302010aff0e01022e02010a
-            ff0e010214020116ff0e01021902010aff0e010209020116ff0e01021102
-            0116ff0e010208020116ff0e01020802010aff0e0102070c0702010aff0e
+            ff0e010210020116ff0e01021902010aff0e01020902010aff0e01021902
+            0116ff0e010208020116ff0e01020802010aff0e0102070c0b02010aff0e
             010205
       'FastAPIProjectGenerator'
-      '__main__'
-      'gcp'
-      '-examples'
-      'dev'
-      'fastapi-service'
-      ('resources', 'cloud_provider', 'launchflow_project_name', 'launchflow_environment_name', 'launchflow_service_name')
-      '/tmp/launchflow'
-      ('destination_path',)
-   names      ('sys', 'dataclasses', 'dataclass', 'typing', 'List', 'Literal', 'Optional', 'Type', 'launchflow.aws.rds', 'RDSPostgres', 'launchflow.aws.s3', 'S3Bucket', 'launchflow.cli.gen.template', 'ProjectGenerator', 'launchflow.gcp.cloudsql', 'CloudSQLPostgres', 'launchflow.gcp.compute_engine', 'ComputeEngineRedis', 'launchflow.gcp.gcs', 'GCSBucket', 'launchflow.gcp.memorystore', 'MemorystoreRedis', 'launchflow', 'Resource', 'ResourceInfo', 'resource_type_to_resource_info_kwargs', 'get_resource_info', 'FastAPIProjectGenerator', '__name__', 'cloud_provider', 'generator', 'generate_project')
+   names      ('sys', 'dataclasses', 'dataclass', 'typing', 'List', 'Literal', 'Optional', 'Type', 'launchflow', 'Resource', 'launchflow.aws.elasticache', 'ElasticacheRedis', 'launchflow.aws.rds', 'RDSPostgres', 'launchflow.aws.s3', 'S3Bucket', 'launchflow.cli.gen.template', 'ProjectGenerator', 'launchflow.gcp.cloudsql', 'CloudSQLPostgres', 'launchflow.gcp.compute_engine', 'ComputeEngineRedis', 'launchflow.gcp.gcs', 'GCSBucket', 'launchflow.gcp.memorystore', 'MemorystoreRedis', 'ResourceInfo', 'resource_type_to_resource_info_kwargs', 'get_resource_info', 'FastAPIProjectGenerator')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   '/home/tanke/launchflow/launchflow/clients/python/launchflow/launchflow/cli/gen/templates/fastapi/fastapi_template.py'
+   filename   '/Users/calebvandyke/code/launchflow-oss/launchflow/cli/gen/templates/fastapi/fastapi_template.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff020108010c0118020c010c010c010c010c010c010c020c03020118
-      ff0e01020f020102010201020102010201020102010201020b04ec041702
-      0102010201020102010201020102010201020b04ec041702010201020102
-      0102010201020102010201020a02ed041602010201020102010201020302
-      03020102fe02040207023306b8044b020102010201020102010201020102
-      010201020a02ed04160201020102010201020102030203020102fe020402
-      07023306b8048000d9047f00751c0902011aff0e01027f004a0c01040104
-      020201020102fd020702010801020102f5120d30f1
+      0x00ff020108010c0118020c010c010c010c010c010c010c010c010c0302
+      0118ff0e01020f020102010201020102010201020102010201020b04ec04
+      17020102010201020102010201020102010201020b04ec04170201020102
+      01020102010201020102010201020a02ed04160201020102010201020102
+      030203020102fe02040207023306b8044b02010201020102010201020102
+      0102010201020a02ed041602010201020102010201020102010201020102
+      0b04ec04170201020102010201020102030203020102fe02040207023306
+      b8048000c2047f007f000d1c0902011aff0e01
```

### Comparing `launchflow-0.3.9.dev8/launchflow/cli/gen/templates/fastapi/_postgres_template/Dockerfile.jinja` & `launchflow-0.4.0.dev0/launchflow/cli/gen/templates/fastapi/_postgres_template/Dockerfile.jinja`

 * *Files 13% similar despite different names*

```diff
@@ -33,14 +33,13 @@
 # Copy installed dependencies from the builder stage
 COPY --from=builder /install /usr/local/lib/python{{ python_major_version }}.{{ python_minor_version }}/site-packages
 ENV PATH="${PATH}:/usr/local/lib/python{{ python_major_version }}.{{ python_minor_version }}/site-packages/bin"
 
 # Set the working directory and copy only the necessary application files
 WORKDIR /code
 COPY --chown=appuser:appuser ./app /code/app
-COPY --chown=appuser:appuser ./launchflow.yaml /code/launchflow.yaml
 
 # Expose the port the app runs on
 EXPOSE $PORT
 
 # Start the application
 CMD uvicorn app.main:app --host 0.0.0.0 --port $PORT
```

### Comparing `launchflow-0.3.9.dev8/launchflow/cli/gen/templates/fastapi/_postgres_template/README.md.jinja` & `launchflow-0.4.0.dev0/launchflow/cli/gen/templates/fastapi/_postgres_template/README.md.jinja`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -80,8 +80,8 @@
 
 Automatically <strong>delete</strong> all infrastructure associated with your application.
 
 ```bash
 launchflow destroy
 ```
 
-Learn how this command works in the [LaunchFlow Docs](https://docs.launchflow.com/reference/cli#launchflow-destroy).
+Learn how this command works in the [LaunchFlow Docs](https://docs.launchflow.com/reference/cli#launchflow-destroy).
```

### Comparing `launchflow-0.3.9.dev8/launchflow/cli/gen/templates/fastapi/_postgres_template/app/main.py.jinja` & `launchflow-0.4.0.dev0/launchflow/cli/gen/templates/fastapi/_postgres_template/app/main.py.jinja`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev8/launchflow/cli/gen/templates/fastapi/_postgres_template/app/schemas.py.jinja` & `launchflow-0.4.0.dev0/launchflow/cli/gen/templates/fastapi/_postgres_template/app/schemas.py.jinja`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev8/launchflow/cli/gen/templates/fastapi/_simple_template/Dockerfile.jinja` & `launchflow-0.4.0.dev0/launchflow/cli/gen/templates/fastapi/_simple_template/Dockerfile.jinja`

 * *Files 13% similar despite different names*

```diff
@@ -33,14 +33,13 @@
 # Copy installed dependencies from the builder stage
 COPY --from=builder /install /usr/local/lib/python{{ python_major_version }}.{{ python_minor_version }}/site-packages
 ENV PATH="${PATH}:/usr/local/lib/python{{ python_major_version }}.{{ python_minor_version }}/site-packages/bin"
 
 # Set the working directory and copy only the necessary application files
 WORKDIR /code
 COPY --chown=appuser:appuser ./app /code/app
-COPY --chown=appuser:appuser ./launchflow.yaml /code/launchflow.yaml
 
 # Expose the port the app runs on
 EXPOSE $PORT
 
 # Start the application
 CMD uvicorn app.main:app --host 0.0.0.0 --port $PORT
```

### Comparing `launchflow-0.3.9.dev8/launchflow/cli/gen/templates/fastapi/_simple_template/README.md.jinja` & `launchflow-0.4.0.dev0/launchflow/cli/gen/templates/fastapi/_simple_template/README.md.jinja`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -80,8 +80,8 @@
 
 Automatically <strong>delete</strong> all infrastructure associated with your application.
 
 ```bash
 launchflow destroy
 ```
 
-Learn how this command works in the [LaunchFlow Docs](https://docs.launchflow.com/reference/cli#launchflow-destroy).
+Learn how this command works in the [LaunchFlow Docs](https://docs.launchflow.com/reference/cli#launchflow-destroy).
```

### Comparing `launchflow-0.3.9.dev8/launchflow/cli/gen/templates/fastapi/_simple_template/app/main.py.jinja` & `launchflow-0.4.0.dev0/launchflow/cli/gen/templates/fastapi/_simple_template/app/main.py.jinja`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev8/launchflow/cli/gen/templates/fastapi/fastapi_template.py` & `launchflow-0.4.0.dev0/launchflow/cli/gen/templates/fastapi/fastapi_template.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import sys
 from dataclasses import dataclass
 from typing import List, Literal, Optional, Type
 
+from launchflow import Resource
+from launchflow.aws.elasticache import ElasticacheRedis
 from launchflow.aws.rds import RDSPostgres
 from launchflow.aws.s3 import S3Bucket
 from launchflow.cli.gen.template import ProjectGenerator
 from launchflow.gcp.cloudsql import CloudSQLPostgres
 from launchflow.gcp.compute_engine import ComputeEngineRedis
 from launchflow.gcp.gcs import GCSBucket
 from launchflow.gcp.memorystore import MemorystoreRedis
 
-from launchflow import Resource
-
 
 @dataclass
 class ResourceInfo:
     infra_docs_url: str
     infra_name: str
     infra_lf_class: str
     launchflow_imports: str
@@ -26,15 +26,15 @@
     fastapi_test_endpoint: str
     requirements: List[str]
 
 
 resource_type_to_resource_info_kwargs = {
     # GCP Compute Engine Redis
     ComputeEngineRedis: {
-        "infra_docs_url": "https://docs.launchflow.com/reference/gcp-resources/compute-engine",
+        "infra_docs_url": "https://docs.launchflow.com/reference/gcp-resources/compute-engine#compute-engine-redis",
         "infra_name": "redis_vm",
         "infra_lf_class": "lf.gcp.ComputeEngineRedis",
         "launchflow_imports": "",
         "infra_import": "from redis.asyncio import Redis",
         "global_setup": None,
         "fastapi_setup": None,
         "app_imports": [],
@@ -49,26 +49,26 @@
     value = await redis_client.get(key)
     return {"message": f"Set {key} to {value}"}
 """,
         "requirements": ["redis>=4.2.0"],
     },
     # GCP Memorystore Redis
     MemorystoreRedis: {
-        "infra_docs_url": "https://docs.launchflow.com/reference/gcp-resources/memorystore-redis",
-        "infra_name": "redis_cluster",
+        "infra_docs_url": "https://docs.launchflow.com/reference/gcp-resources/memorystore",
+        "infra_name": "memorystore",
         "infra_lf_class": "lf.gcp.MemorystoreRedis",
         "launchflow_imports": "",
         "infra_import": "from redis.asyncio import Redis",
         "global_setup": None,
         "fastapi_setup": None,
         "app_imports": [],
         "fastapi_test_endpoint": """
 @app.post("/test_redis/{key}")
 async def test_redis(
-    key: str, value: str, redis_client: Redis = Depends(redis_cluster.redis_async)
+    key: str, value: str, redis_client: Redis = Depends(memorystore.redis_async)
 ):
     # Write to Redis
     await redis_client.set(key, value)
     # Immediately read from Redis to verify the write
     value = await redis_client.get(key)
     return {"message": f"Set {key} to {value}"}
 """,
@@ -189,17 +189,40 @@
     s3_bucket.upload_from_string("Hello, World!", object_name)
     # Immediately read from S3 to verify the write
     s3_bucket.download_file(object_name).decode("utf-8")
     return {"message": f"Uploaded {object_name} to S3"}
 """,
         "requirements": [],
     },
+    # AWS Elasticache Redis
+    ElasticacheRedis: {
+        "infra_docs_url": "https://docs.launchflow.com/reference/aws-resources/elasticache-redis",
+        "infra_name": "elasticache",
+        "infra_lf_class": "lf.aws.ElasticacheRedis",
+        "launchflow_imports": "",
+        "infra_import": "from redis.asyncio import Redis",
+        "global_setup": None,
+        "fastapi_setup": None,
+        "app_imports": [],
+        "fastapi_test_endpoint": """
+@app.post("/test_redis/{key}")
+async def test_redis(
+    key: str, value: str, redis_client: Redis = Depends(elasticache.redis_async)
+):
+    # Write to Redis
+    await redis_client.set(key, value)
+    # Immediately read from Redis to verify the write
+    value = await redis_client.get(key)
+    return {"message": f"Set {key} to {value}"}
+""",
+        "requirements": ["redis>=4.2.0"],
+    },
     # AWS RDS (Postgres)
     RDSPostgres: {
-        "infra_docs_url": "https://docs.launchflow.com/reference/aws-resources/rds",
+        "infra_docs_url": "https://docs.launchflow.com/reference/aws-resources/rds-postgres",
         "infra_name": "postgres",
         "infra_lf_class": "lf.aws.RDSPostgres",
         "launchflow_imports": "from launchflow.fastapi import sqlalchemy_async_depends",
         "infra_import": """from sqlalchemy import select
 from sqlalchemy.ext.asyncio import AsyncSession
 """,
         "global_setup": """# Create the global FastAPI dependency for the SQLAlchemy async session
@@ -340,20 +363,16 @@
 {resource_info.infra_name} = {resource_info.infra_lf_class}('{self.launchflow_project_name}-{resource_info.infra_name.replace('_', '-')}')"""
                 )
         return "\n".join(lines)
 
     # Used by app/main.py
     @property
     def fastapi_imports(self) -> str:
-        if len(self.resources) == 0:
-            return "from fastapi import FastAPI"
         resource_set = set(self.resources)
-        if len(self.resources) == 1 and (
-            GCSBucket in resource_set or S3Bucket in resource_set
-        ):
+        if len(resource_set) <= 1:
             return """from contextlib import asynccontextmanager
 
 from fastapi import FastAPI"""
         if CloudSQLPostgres in resource_set or RDSPostgres in resource_set:
             return """from contextlib import asynccontextmanager
 
 from fastapi import Depends, FastAPI, HTTPException"""
@@ -396,15 +415,23 @@
             resource_info = get_resource_info(resource)
             if resource_info.global_setup is not None:
                 lines.append(resource_info.global_setup)
         return "\n".join(lines)
 
     # Used by app/main.py
     @property
-    def app_infra_setup(self) -> List[str]:
+    def app_infra_setup(self) -> str:
+        if len(self.resources) == 0:
+            return "\n".join(
+                [
+                    "# NOTE: This is where you connect resources on startup",
+                    "    # For example, if you had a GCS bucket you would do:",
+                    "    # await gcs_bucket.connect()",
+                ]
+            )
         infra_names = []
         infra_steps = []
         for resource in self.resources:
             resource_info = get_resource_info(resource)
             infra_names.append(resource_info.infra_name)
             if resource_info.fastapi_setup is not None:
                 infra_steps.append(resource_info.fastapi_setup)
@@ -439,20 +466,24 @@
     def launchflow_service_product(self) -> str:
         if self.cloud_provider == "aws":
             return "aws_ecs_fargate"
         elif self.cloud_provider == "gcp":
             return "gcp_cloud_run"
         raise ValueError(f"Unsupported cloud provider: {self.cloud_provider}")
 
-    def template_directory(self) -> str:
+    def template_path_info(self) -> str:
+        template_dir = "launchflow.cli.gen.templates.fastapi"
+        template_name = "_simple_template"
+
         if CloudSQLPostgres in [
             resource for resource in self.resources
         ] or RDSPostgres in [resource for resource in self.resources]:
-            return "launchflow.cli.gen.templates.fastapi._postgres_template"
-        return "launchflow.cli.gen.templates.fastapi._simple_template"
+            template_name = "_postgres_template"
+
+        return template_dir, template_name
 
     @property
     def docker_repository_prefix(self) -> str:
         if self.cloud_provider == "aws":
             return "public.ecr.aws/docker/library/"
         return ""
 
@@ -478,23 +509,23 @@
             "app_infra_imports": self.app_infra_imports,
             "app_global_setup": self.app_global_setup,
             "app_infra_setup": self.app_infra_setup,
             "app_infra_endpoints": self.app_infra_endpoints,
         }
 
 
-if __name__ == "__main__":
-    cloud_provider = "gcp"
-    generator = FastAPIProjectGenerator(
-        resources=[
-            ComputeEngineRedis,
-            GCSBucket,
-            CloudSQLPostgres,
-            # S3Bucket,
-            # RDSPostgres,
-        ],
-        cloud_provider=cloud_provider,
-        launchflow_project_name=f"{cloud_provider}-examples",
-        launchflow_environment_name="dev",
-        launchflow_service_name="fastapi-service",
-    )
-    generator.generate_project(destination_path="/tmp/launchflow")
+# if __name__ == "__main__":
+#     cloud_provider = "gcp"
+#     generator = FastAPIProjectGenerator(
+#         resources=[
+#             ComputeEngineRedis,
+#             GCSBucket,
+#             CloudSQLPostgres,
+#             # S3Bucket,
+#             # RDSPostgres,
+#         ],
+#         cloud_provider=cloud_provider,
+#         launchflow_project_name=f"{cloud_provider}-examples",
+#         launchflow_environment_name="dev",
+#         launchflow_service_name="fastapi-service",
+#     )
+#     generator.generate_project(destination_path="/tmp/launchflow")
```

### Comparing `launchflow-0.3.9.dev8/launchflow/cli/gen/templates/flask/__pycache__/flask_template.cpython-311.pyc` & `launchflow-0.4.0.dev0/launchflow/cli/gen/templates/django/__pycache__/django_template.cpython-311.pyc`

 * *Files 23% similar despite different names*

#### Python bytecode

```diff
@@ -1,811 +1,801 @@
 magic:    0xa70d0d0a
-moddate:  0xfc420f66 (Fri Apr  5 00:17:00 2024 UTC)
-files sz: 17509
+moddate:  0x972d4666 (Thu May 16 16:00:23 2024 UTC)
+files sz: 16928
 code
    argcount  : 0
    nlocals   : 0
-   stacksize : 22
+   stacksize : 23
    flags     : 0
    code
-      0x9700640064016c005a00640064026c016d025a020100640064036c036d
-      045a046d055a056d065a066d075a070100640064046c086d095a09010064
-      0064056c0a6d0b5a0b0100640064066c0c6d0d5a0d0100640064076c0e6d
-      0f5a0f0100640064086c106d115a110100640064096c126d135a13010064
-      00640a6c146d155a1501006400640b6c166d175a17010065020200470064
-      0c8400640da6020000ab020000000000000000a6000000ab000000000000
-      0000005a186511640e640f64106411640164016412670064136414670164
-      159c0a65156416641764186411640164016412670064196414670164159c
-      0a6513641a641b641c641164016401641d6700641e670064159c0a650f64
-      1f642064216411640164016422642367026424642564266427670264289c
-      0a650b6429642a642b641164016401642c6700642d670064159c0a650964
-      2e6420642f6411640164016422642367026424642564266427670264289c
-      0a69065a1964306507651719000000000000000000643165186604643284
-      045a1a650202004700643384006434650da6030000ab0300000000000000
-      00a6000000ab0000000000000000005a1b651c64356b0200000000723064
-      365a1d0200651b65116513650f6703651d651d9b0064379d0264386439ac
-      3aa6050000ab0500000000000000005a1e651ea01f000000000000000000
-      0000000000000000000000643bac3ca6010000ab01000000000000000001
-      006401530064015300
+      0x9700640064016c005a00640064016c015a01640064026c026d035a0301
+      00640064036c046d055a056d065a066d075a076d085a080100640064046c
+      096d0a5a0a0100640064056c0b6d0c5a0c0100640064066c0d6d0e5a0e01
+      00640064076c0f6d105a100100640064086c116d125a120100640064096c
+      136d145a1401006400640a6c156d165a1601006400640b6c176d185a1801
+      006400640c6c196d1a5a1a0100650302004700640d8400640ea6020000ab
+      020000000000000000a6000000ab0000000000000000005a1b6516640f64
+      106411641264136414641564166701640164179c09651a64186419641a64
+      1b64136414641564166701640164179c096518641c641d641e641f642064
+      21642264236701642464179c096514642564266427642864016401640164
+      296701640164179c096510642a642b642c6420642d642e642f6430670164
+      2464319c09650c643264336434643564136414641564166701640164179c
+      09650e643664266437640164286401640164296701640164319c0969075a
+      1c64386508650a190000000000000000006439651b6604643a84045a1d65
+      0302004700643b8400643c6512a6030000ab030000000000000000a60000
+      00ab0000000000000000005a1e64015300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (None)
-                 6 IMPORT_NAME              0 (sys)
-                 8 STORE_NAME               0 (sys)
+                 6 IMPORT_NAME              0 (datetime)
+                 8 STORE_NAME               0 (datetime)
    
      2          10 LOAD_CONST               0 (0)
-                12 LOAD_CONST               2 (('dataclass',))
-                14 IMPORT_NAME              1 (dataclasses)
-                16 IMPORT_FROM              2 (dataclass)
-                18 STORE_NAME               2 (dataclass)
-                20 POP_TOP
+                12 LOAD_CONST               1 (None)
+                14 IMPORT_NAME              1 (sys)
+                16 STORE_NAME               1 (sys)
    
-     3          22 LOAD_CONST               0 (0)
-                24 LOAD_CONST               3 (('List', 'Literal', 'Optional', 'Type'))
-                26 IMPORT_NAME              3 (typing)
-                28 IMPORT_FROM              4 (List)
-                30 STORE_NAME               4 (List)
-                32 IMPORT_FROM              5 (Literal)
-                34 STORE_NAME               5 (Literal)
-                36 IMPORT_FROM              6 (Optional)
-                38 STORE_NAME               6 (Optional)
-                40 IMPORT_FROM              7 (Type)
-                42 STORE_NAME               7 (Type)
-                44 POP_TOP
+     3          18 LOAD_CONST               0 (0)
+                20 LOAD_CONST               2 (('dataclass',))
+                22 IMPORT_NAME              2 (dataclasses)
+                24 IMPORT_FROM              3 (dataclass)
+                26 STORE_NAME               3 (dataclass)
+                28 POP_TOP
    
-     5          46 LOAD_CONST               0 (0)
-                48 LOAD_CONST               4 (('RDSPostgres',))
-                50 IMPORT_NAME              8 (launchflow.aws.rds)
-                52 IMPORT_FROM              9 (RDSPostgres)
-                54 STORE_NAME               9 (RDSPostgres)
-                56 POP_TOP
+     4          30 LOAD_CONST               0 (0)
+                32 LOAD_CONST               3 (('List', 'Literal', 'Optional', 'Type'))
+                34 IMPORT_NAME              4 (typing)
+                36 IMPORT_FROM              5 (List)
+                38 STORE_NAME               5 (List)
+                40 IMPORT_FROM              6 (Literal)
+                42 STORE_NAME               6 (Literal)
+                44 IMPORT_FROM              7 (Optional)
+                46 STORE_NAME               7 (Optional)
+                48 IMPORT_FROM              8 (Type)
+                50 STORE_NAME               8 (Type)
+                52 POP_TOP
    
-     6          58 LOAD_CONST               0 (0)
-                60 LOAD_CONST               5 (('S3Bucket',))
-                62 IMPORT_NAME             10 (launchflow.aws.s3)
-                64 IMPORT_FROM             11 (S3Bucket)
-                66 STORE_NAME              11 (S3Bucket)
-                68 POP_TOP
+     6          54 LOAD_CONST               0 (0)
+                56 LOAD_CONST               4 (('Resource',))
+                58 IMPORT_NAME              9 (launchflow)
+                60 IMPORT_FROM             10 (Resource)
+                62 STORE_NAME              10 (Resource)
+                64 POP_TOP
    
-     7          70 LOAD_CONST               0 (0)
-                72 LOAD_CONST               6 (('ProjectGenerator',))
-                74 IMPORT_NAME             12 (launchflow.cli.gen.template)
-                76 IMPORT_FROM             13 (ProjectGenerator)
-                78 STORE_NAME              13 (ProjectGenerator)
-                80 POP_TOP
+     7          66 LOAD_CONST               0 (0)
+                68 LOAD_CONST               5 (('ElasticacheRedis',))
+                70 IMPORT_NAME             11 (launchflow.aws.elasticache)
+                72 IMPORT_FROM             12 (ElasticacheRedis)
+                74 STORE_NAME              12 (ElasticacheRedis)
+                76 POP_TOP
    
-     8          82 LOAD_CONST               0 (0)
-                84 LOAD_CONST               7 (('CloudSQLPostgres',))
-                86 IMPORT_NAME             14 (launchflow.gcp.cloudsql)
-                88 IMPORT_FROM             15 (CloudSQLPostgres)
-                90 STORE_NAME              15 (CloudSQLPostgres)
-                92 POP_TOP
+     8          78 LOAD_CONST               0 (0)
+                80 LOAD_CONST               6 (('RDSPostgres',))
+                82 IMPORT_NAME             13 (launchflow.aws.rds)
+                84 IMPORT_FROM             14 (RDSPostgres)
+                86 STORE_NAME              14 (RDSPostgres)
+                88 POP_TOP
    
-     9          94 LOAD_CONST               0 (0)
-                96 LOAD_CONST               8 (('ComputeEngineRedis',))
-                98 IMPORT_NAME             16 (launchflow.gcp.compute_engine)
-               100 IMPORT_FROM             17 (ComputeEngineRedis)
-               102 STORE_NAME              17 (ComputeEngineRedis)
-               104 POP_TOP
+     9          90 LOAD_CONST               0 (0)
+                92 LOAD_CONST               7 (('S3Bucket',))
+                94 IMPORT_NAME             15 (launchflow.aws.s3)
+                96 IMPORT_FROM             16 (S3Bucket)
+                98 STORE_NAME              16 (S3Bucket)
+               100 POP_TOP
    
-    10         106 LOAD_CONST               0 (0)
-               108 LOAD_CONST               9 (('GCSBucket',))
-               110 IMPORT_NAME             18 (launchflow.gcp.gcs)
-               112 IMPORT_FROM             19 (GCSBucket)
-               114 STORE_NAME              19 (GCSBucket)
-               116 POP_TOP
+    10         102 LOAD_CONST               0 (0)
+               104 LOAD_CONST               8 (('ProjectGenerator',))
+               106 IMPORT_NAME             17 (launchflow.cli.gen.template)
+               108 IMPORT_FROM             18 (ProjectGenerator)
+               110 STORE_NAME              18 (ProjectGenerator)
+               112 POP_TOP
    
-    11         118 LOAD_CONST               0 (0)
-               120 LOAD_CONST              10 (('MemorystoreRedis',))
-               122 IMPORT_NAME             20 (launchflow.gcp.memorystore)
-               124 IMPORT_FROM             21 (MemorystoreRedis)
-               126 STORE_NAME              21 (MemorystoreRedis)
-               128 POP_TOP
+    11         114 LOAD_CONST               0 (0)
+               116 LOAD_CONST               9 (('CloudSQLPostgres',))
+               118 IMPORT_NAME             19 (launchflow.gcp.cloudsql)
+               120 IMPORT_FROM             20 (CloudSQLPostgres)
+               122 STORE_NAME              20 (CloudSQLPostgres)
+               124 POP_TOP
    
-    13         130 LOAD_CONST               0 (0)
-               132 LOAD_CONST              11 (('Resource',))
-               134 IMPORT_NAME             22 (launchflow)
-               136 IMPORT_FROM             23 (Resource)
-               138 STORE_NAME              23 (Resource)
-               140 POP_TOP
+    12         126 LOAD_CONST               0 (0)
+               128 LOAD_CONST              10 (('ComputeEngineRedis',))
+               130 IMPORT_NAME             21 (launchflow.gcp.compute_engine)
+               132 IMPORT_FROM             22 (ComputeEngineRedis)
+               134 STORE_NAME              22 (ComputeEngineRedis)
+               136 POP_TOP
    
-    16         142 LOAD_NAME                2 (dataclass)
+    13         138 LOAD_CONST               0 (0)
+               140 LOAD_CONST              11 (('GCSBucket',))
+               142 IMPORT_NAME             23 (launchflow.gcp.gcs)
+               144 IMPORT_FROM             24 (GCSBucket)
+               146 STORE_NAME              24 (GCSBucket)
+               148 POP_TOP
    
-    17         144 PUSH_NULL
-               146 LOAD_BUILD_CLASS
-               148 LOAD_CONST              12 (<code object ResourceInfo, file "/home/tanke/launchflow/launchflow/clients/python/launchflow/launchflow/cli/gen/templates/flask/flask_template.py", line 16>)
-               150 MAKE_FUNCTION            0
-               152 LOAD_CONST              13 ('ResourceInfo')
-               154 PRECALL                  2
-               158 CALL                     2
+    14         150 LOAD_CONST               0 (0)
+               152 LOAD_CONST              12 (('MemorystoreRedis',))
+               154 IMPORT_NAME             25 (launchflow.gcp.memorystore)
+               156 IMPORT_FROM             26 (MemorystoreRedis)
+               158 STORE_NAME              26 (MemorystoreRedis)
+               160 POP_TOP
    
-    16         168 PRECALL                  0
-               172 CALL                     0
+    17         162 LOAD_NAME                3 (dataclass)
    
-    17         182 STORE_NAME              24 (ResourceInfo)
+    18         164 PUSH_NULL
+               166 LOAD_BUILD_CLASS
+               168 LOAD_CONST              13 (<code object ResourceInfo, file "/Users/calebvandyke/code/launchflow-oss/launchflow/cli/gen/templates/django/django_template.py", line 17>)
+               170 MAKE_FUNCTION            0
+               172 LOAD_CONST              14 ('ResourceInfo')
+               174 PRECALL                  2
+               178 CALL                     2
    
-    32         184 LOAD_NAME               17 (ComputeEngineRedis)
+    17         188 PRECALL                  0
+               192 CALL                     0
    
-    33         186 LOAD_CONST              14 ('https://docs.launchflow.com/reference/gcp-resources/compute-engine')
+    18         202 STORE_NAME              27 (ResourceInfo)
    
-    34         188 LOAD_CONST              15 ('redis_vm')
+    32         204 LOAD_NAME               22 (ComputeEngineRedis)
    
-    35         190 LOAD_CONST              16 ('lf.gcp.ComputeEngineRedis')
+    33         206 LOAD_CONST              15 ('https://docs.launchflow.com/reference/gcp-resources/compute-engine#compute-engine-redis')
    
-    36         192 LOAD_CONST              17 ('')
+    34         208 LOAD_CONST              16 ('redis_vm')
    
-    37         194 LOAD_CONST               1 (None)
+    35         210 LOAD_CONST              17 ('lf.gcp.ComputeEngineRedis')
    
-    38         196 LOAD_CONST               1 (None)
+    36         212 LOAD_CONST              18 ('CACHES = {\n    "default": redis_vm.django_settings(),\n}\n')
    
-    39         198 LOAD_CONST              18 ('# Connect to the Redis instance\nredis_client = redis_vm.redis()\n')
+    40         214 LOAD_CONST              19 ('from django.core.cache import cache')
    
-    40         200 BUILD_LIST               0
+    41         216 LOAD_CONST              20 ('\n# NOTE: This should normally use a POST request since it\'s modifying state, but we\'re\n# using GET so you can easily test it in your browser.\n@api_view(["GET"])\ndef test_redis(request, key):\n    # Write to cache (Redis)\n    cache.set(key, "Hello from Redis!", timeout=60)\n    # Immediately read from cache to verify write\n    return Response({"message": cache.get(key)})\n')
    
-    41         202 LOAD_CONST              19 ('\n# NOTE: This should normally use a POST request since it\'s modifying state, but we\'re\n# using GET so you can easily test it in your browser.\n@app.get("/test_redis/<key>")\ndef test_redis(key: str):\n    value = request.json["value"]\n    # Write to Redis\n    redis_client.set(key, value)\n    # Immediately read from Redis to verify the write\n    value = redis_client.get(key)\n    return jsonify({"message": f"Set {key} to {value}"})\n')
+    51         218 LOAD_CONST              21 ('path("test_redis/<key>", views.test_redis),')
    
-    53         204 LOAD_CONST              20 ('redis>=4.2.0')
-               206 BUILD_LIST               1
+    52         220 LOAD_CONST              22 ('redis>=4.2.0')
+               222 BUILD_LIST               1
    
-    32         208 LOAD_CONST              21 (('infra_docs_url', 'infra_name', 'infra_lf_class', 'launchflow_imports', 'infra_import', 'global_setup', 'infra_setup', 'app_imports', 'flask_test_endpoint', 'requirements'))
-               210 BUILD_CONST_KEY_MAP     10
+    53         224 LOAD_CONST               1 (None)
    
-    56         212 LOAD_NAME               21 (MemorystoreRedis)
+    32         226 LOAD_CONST              23 (('infra_docs_url', 'infra_name', 'infra_lf_class', 'django_settings', 'views_imports', 'django_test_endpoint', 'django_test_endpoint_url', 'requirements', 'installed_app'))
+               228 BUILD_CONST_KEY_MAP      9
    
-    57         214 LOAD_CONST              22 ('https://docs.launchflow.com/reference/gcp-resources/memorystore-redis')
+    56         230 LOAD_NAME               26 (MemorystoreRedis)
    
-    58         216 LOAD_CONST              23 ('redis_cluster')
+    57         232 LOAD_CONST              24 ('https://docs.launchflow.com/reference/gcp-resources/memorystore')
    
-    59         218 LOAD_CONST              24 ('lf.gcp.MemorystoreRedis')
+    58         234 LOAD_CONST              25 ('memorystore')
    
-    60         220 LOAD_CONST              17 ('')
+    59         236 LOAD_CONST              26 ('lf.gcp.MemorystoreRedis')
    
-    61         222 LOAD_CONST               1 (None)
+    60         238 LOAD_CONST              27 ('CACHES = {\n    "default": memorystore.django_settings(),\n}\n')
    
-    62         224 LOAD_CONST               1 (None)
+    64         240 LOAD_CONST              19 ('from django.core.cache import cache')
    
-    63         226 LOAD_CONST              18 ('# Connect to the Redis instance\nredis_client = redis_vm.redis()\n')
+    65         242 LOAD_CONST              20 ('\n# NOTE: This should normally use a POST request since it\'s modifying state, but we\'re\n# using GET so you can easily test it in your browser.\n@api_view(["GET"])\ndef test_redis(request, key):\n    # Write to cache (Redis)\n    cache.set(key, "Hello from Redis!", timeout=60)\n    # Immediately read from cache to verify write\n    return Response({"message": cache.get(key)})\n')
    
-    64         228 BUILD_LIST               0
+    75         244 LOAD_CONST              21 ('path("test_redis/<key>", views.test_redis),')
    
-    65         230 LOAD_CONST              25 ('\n# NOTE: This should normally use a POST request since it\'s modifying state, but we\'re\n# using GET so you can easily test it in your browser.\n@app.get("/test_redis/<key>")\ndef test_redis(key: str):\n    # Write to Redis\n    value = request.json["value"]\n    redis_client.set(key, value)\n    # Immediately read from Redis to verify the write\n    value = redis_client.get(key)\n    return jsonify({"message": f"Set {key} to {value}"})\n')
+    76         246 LOAD_CONST              22 ('redis>=4.2.0')
+               248 BUILD_LIST               1
    
-    77         232 LOAD_CONST              20 ('redis>=4.2.0')
-               234 BUILD_LIST               1
+    77         250 LOAD_CONST               1 (None)
    
-    56         236 LOAD_CONST              21 (('infra_docs_url', 'infra_name', 'infra_lf_class', 'launchflow_imports', 'infra_import', 'global_setup', 'infra_setup', 'app_imports', 'flask_test_endpoint', 'requirements'))
-               238 BUILD_CONST_KEY_MAP     10
+    56         252 LOAD_CONST              23 (('infra_docs_url', 'infra_name', 'infra_lf_class', 'django_settings', 'views_imports', 'django_test_endpoint', 'django_test_endpoint_url', 'requirements', 'installed_app'))
+               254 BUILD_CONST_KEY_MAP      9
    
-    80         240 LOAD_NAME               19 (GCSBucket)
+    80         256 LOAD_NAME               24 (GCSBucket)
    
-    81         242 LOAD_CONST              26 ('https://docs.launchflow.com/reference/gcp-resources/gcs-bucket')
+    81         258 LOAD_CONST              28 ('https://docs.launchflow.com/reference/gcp-resources/gcs-bucket')
    
-    82         244 LOAD_CONST              27 ('gcs_bucket')
+    82         260 LOAD_CONST              29 ('gcs_bucket')
    
-    83         246 LOAD_CONST              28 ('lf.gcp.GCSBucket')
+    83         262 LOAD_CONST              30 ('lf.gcp.GCSBucket')
    
-    84         248 LOAD_CONST              17 ('')
+    84         264 LOAD_CONST              31 ('STORAGES = {\n    "default": {\n        "BACKEND": "storages.backends.gcloud.GoogleCloudStorage",\n    },\n    "staticfiles": {\n        "BACKEND": "storages.backends.gcloud.GoogleCloudStorage",\n    },\n}\nGS_BUCKET_NAME = gcs_bucket.connect().bucket_name\nGS_CREDENTIALS = lf.gcp.get_service_account_credentials()\n')
    
-    85         250 LOAD_CONST               1 (None)
+    95         266 LOAD_CONST              32 ('from django.core.files.storage import default_storage')
    
-    86         252 LOAD_CONST               1 (None)
+    96         268 LOAD_CONST              33 ('\n# NOTE: This should normally use a POST request since it\'s modifying state, but we\'re\n# using GET so you can easily test it in your browser.\n@api_view(["GET"])\ndef test_gcs(request, object_name):\n    # Write to GCS\n    with default_storage.open(object_name, "w") as file:\n        file.write("Hello from GCS!")\n    # Immediately read from GCS to verify write\n    with default_storage.open(object_name, "r") as file:\n        return Response({"message": file.read()})\n')
    
-    87         254 LOAD_CONST              29 ('# Connect to the storage Bucket\ngcs_bucket.connect()\n')
+   108         270 LOAD_CONST              34 ('path("test_gcs/<object_name>", views.test_gcs),')
    
-    88         256 BUILD_LIST               0
+   109         272 LOAD_CONST              35 ('django-storages[google]')
+               274 BUILD_LIST               1
    
-    89         258 LOAD_CONST              30 ('\n# NOTE: This should normally use a POST request since it\'s modifying state, but we\'re\n# using GET so you can easily test it in your browser.\n@app.get("/test_gcs/<object_name>")\ndef test_gcs(object_name: str):\n    # Write to GCS\n    gcs_bucket.upload_from_string("Hello, World!", object_name)\n    # Immediately read from GCS to verify the write\n    gcs_bucket.download_file(object_name).decode("utf-8")\n    return jsonify({"message": f"Uploaded {object_name} to GCS"})\n')
+   110         276 LOAD_CONST              36 ('storages')
    
-   100         260 BUILD_LIST               0
+    80         278 LOAD_CONST              23 (('infra_docs_url', 'infra_name', 'infra_lf_class', 'django_settings', 'views_imports', 'django_test_endpoint', 'django_test_endpoint_url', 'requirements', 'installed_app'))
+               280 BUILD_CONST_KEY_MAP      9
    
-    80         262 LOAD_CONST              21 (('infra_docs_url', 'infra_name', 'infra_lf_class', 'launchflow_imports', 'infra_import', 'global_setup', 'infra_setup', 'app_imports', 'flask_test_endpoint', 'requirements'))
-               264 BUILD_CONST_KEY_MAP     10
+   113         282 LOAD_NAME               20 (CloudSQLPostgres)
    
-   103         266 LOAD_NAME               15 (CloudSQLPostgres)
+   114         284 LOAD_CONST              37 ('https://docs.launchflow.com/reference/gcp-resources/cloud-sql')
    
-   104         268 LOAD_CONST              31 ('https://docs.launchflow.com/reference/gcp-resources/cloud-sql')
+   115         286 LOAD_CONST              38 ('postgres')
    
-   105         270 LOAD_CONST              32 ('postgres')
+   116         288 LOAD_CONST              39 ('lf.gcp.CloudSQLPostgres')
    
-   106         272 LOAD_CONST              33 ('lf.gcp.CloudSQLPostgres')
+   117         290 LOAD_CONST              40 ('DATABASES = {\n    "default": postgres.django_settings(),\n}\n')
    
-   107         274 LOAD_CONST              17 ('')
+   121         292 LOAD_CONST               1 (None)
    
-   108         276 LOAD_CONST               1 (None)
+   122         294 LOAD_CONST               1 (None)
    
-   109         278 LOAD_CONST               1 (None)
+   123         296 LOAD_CONST               1 (None)
    
-   111         280 LOAD_CONST              34 ('from app.models import Base, StorageUser')
+   124         298 LOAD_CONST              41 ('psycopg2-binary')
+               300 BUILD_LIST               1
    
-   112         282 LOAD_CONST              35 ('from app.schemas import ListUsersResponse, UserResponse')
+   125         302 LOAD_CONST               1 (None)
    
-   110         284 BUILD_LIST               2
+   113         304 LOAD_CONST              23 (('infra_docs_url', 'infra_name', 'infra_lf_class', 'django_settings', 'views_imports', 'django_test_endpoint', 'django_test_endpoint_url', 'requirements', 'installed_app'))
+               306 BUILD_CONST_KEY_MAP      9
    
-   114         286 LOAD_CONST              36 ('# Configure the Postgres database with Flask-SQLAlchemy\ndb = SQLAlchemy(\n    app,\n    model_class=Base,\n    engine_options=postgres.sqlalchemy_engine_options(),\n)\n\nwith app.app_context():\n    db.create_all()')
+   128         308 LOAD_NAME               16 (S3Bucket)
    
-   123         288 LOAD_CONST              37 ('\n"""\nThe endpoints below define a simple CRUD API for a generic StorageUser model.\n\nThe StorageUser model is defined in app.models\nThe ListUsersResponse and UserResponse schemas are defined in app.schemas.\n"""\n\n\n@app.get("/users")\ndef list_users():\n    storage_users = db.session.execute(select(StorageUser)).scalars().all()\n    return jsonify(\n        ListUsersResponse.from_storage(storage_users).model_dump(mode="json")\n    )\n\n\n@app.post("/users")\ndef create_user():\n    data = request.json\n    storage_user = StorageUser(email=data["email"], name=data["name"])\n    db.session.add(storage_user)\n    db.session.commit()\n    return jsonify(UserResponse.from_storage(storage_user).model_dump(mode="json"))\n\n\n@app.get("/users/<int:user_id>")\ndef read_user(user_id: int):\n    storage_user = db.session.get(StorageUser, user_id)\n    if storage_user is None:\n        abort(404, "User not found")\n    return jsonify(UserResponse.from_storage(storage_user).model_dump(mode="json"))\n\n\n@app.put("/users/<int:user_id>")\ndef update_user(user_id: int):\n    storage_user = db.session.get(StorageUser, user_id)\n    if storage_user is None:\n        abort(404, "User not found")\n    data = request.json\n    storage_user.name = data["name"]\n    db.session.commit()\n    return jsonify(UserResponse.from_storage(storage_user).model_dump(mode="json"))\n\n\n@app.delete("/users/<int:user_id>")\ndef delete_user(user_id):\n    storage_user = db.session.get(StorageUser, user_id)\n    if storage_user is None:\n        abort(404, "User not found")\n    db.session.delete(storage_user)\n    db.session.commit()\n    return jsonify(UserResponse.from_storage(storage_user).model_dump(mode="json"))\n')
+   129         310 LOAD_CONST              42 ('https://docs.launchflow.com/reference/aws-resources/s3-bucket')
    
-   177         290 LOAD_CONST              38 ('Flask-SQLAlchemy')
-               292 LOAD_CONST              39 ('pg8000')
-               294 BUILD_LIST               2
+   130         312 LOAD_CONST              43 ('s3_bucket')
    
-   103         296 LOAD_CONST              40 (('infra_docs_url', 'infra_name', 'infra_lf_class', 'launchflow_imports', 'infra_import', 'global_setup', 'app_imports', 'infra_setup', 'flask_test_endpoint', 'requirements'))
-               298 BUILD_CONST_KEY_MAP     10
+   131         314 LOAD_CONST              44 ('lf.aws.S3Bucket')
    
-   180         300 LOAD_NAME               11 (S3Bucket)
+   132         316 LOAD_CONST              32 ('from django.core.files.storage import default_storage')
    
-   181         302 LOAD_CONST              41 ('https://docs.launchflow.com/reference/aws-resources/s3-bucket')
+   133         318 LOAD_CONST              45 ('STORAGES = {\n    "default": {\n        "BACKEND": "storages.backends.s3.S3Storage",\n    },\n    "staticfiles": {\n        "BACKEND": "storages.backends.s3.S3Storage",\n    },\n}\nAWS_STORAGE_BUCKET_NAME = s3_bucket.connect().bucket_name\n')
    
-   182         304 LOAD_CONST              42 ('s3_bucket')
+   143         320 LOAD_CONST              46 ('\n# NOTE: This should normally use a POST request since it\'s modifying state, but we\'re\n# using GET so you can easily test it in your browser.\n@api_view(["GET"])\ndef test_s3(request, object_name):\n    # Write to S3\n    with default_storage.open(object_name, "w") as file:\n        file.write("Hello from S3!")\n    # Immediately read from S3 to verify write\n    with default_storage.open(object_name, "r") as file:\n        return Response({"message": file.read()})\n')
    
-   183         306 LOAD_CONST              43 ('lf.aws.S3Bucket')
+   155         322 LOAD_CONST              47 ('path("test_s3/<object_name>", views.test_s3),')
    
-   184         308 LOAD_CONST              17 ('')
+   156         324 LOAD_CONST              48 ('django-storages[s3]')
+               326 BUILD_LIST               1
    
-   185         310 LOAD_CONST               1 (None)
+   157         328 LOAD_CONST              36 ('storages')
    
-   186         312 LOAD_CONST               1 (None)
+   128         330 LOAD_CONST              49 (('infra_docs_url', 'infra_name', 'infra_lf_class', 'views_imports', 'django_settings', 'django_test_endpoint', 'django_test_endpoint_url', 'requirements', 'installed_app'))
+               332 BUILD_CONST_KEY_MAP      9
    
-   187         314 LOAD_CONST              44 ('# Connect to the storage Bucket\ns3_bucket.connect()\n')
+   160         334 LOAD_NAME               12 (ElasticacheRedis)
    
-   188         316 BUILD_LIST               0
+   161         336 LOAD_CONST              50 ('https://docs.launchflow.com/reference/aws-resources/elasticache-redis')
    
-   189         318 LOAD_CONST              45 ('\n# NOTE: This should normally use a POST request since it\'s modifying state, but we\'re\n# using GET so you can easily test it in your browser.\n@app.get("/test_s3/<object_name>")\ndef test_s3(object_name: str):\n    # Write to S3\n    s3_bucket.upload_from_string("Hello, World!", object_name)\n    # Immediately read from S3 to verify the write\n    s3_bucket.download_file(object_name).decode("utf-8")\n    return jsonify({"message": f"Uploaded {object_name} to S3"})\n')
+   162         338 LOAD_CONST              51 ('elasticache')
    
-   200         320 BUILD_LIST               0
+   163         340 LOAD_CONST              52 ('lf.aws.ElasticacheRedis')
    
-   180         322 LOAD_CONST              21 (('infra_docs_url', 'infra_name', 'infra_lf_class', 'launchflow_imports', 'infra_import', 'global_setup', 'infra_setup', 'app_imports', 'flask_test_endpoint', 'requirements'))
-               324 BUILD_CONST_KEY_MAP     10
+   164         342 LOAD_CONST              53 ('CACHES = {\n    "default": elasticache.django_settings(),\n}\n')
    
-   203         326 LOAD_NAME                9 (RDSPostgres)
+   168         344 LOAD_CONST              19 ('from django.core.cache import cache')
    
-   204         328 LOAD_CONST              46 ('https://docs.launchflow.com/reference/aws-resources/rds')
+   169         346 LOAD_CONST              20 ('\n# NOTE: This should normally use a POST request since it\'s modifying state, but we\'re\n# using GET so you can easily test it in your browser.\n@api_view(["GET"])\ndef test_redis(request, key):\n    # Write to cache (Redis)\n    cache.set(key, "Hello from Redis!", timeout=60)\n    # Immediately read from cache to verify write\n    return Response({"message": cache.get(key)})\n')
    
-   205         330 LOAD_CONST              32 ('postgres')
+   179         348 LOAD_CONST              21 ('path("test_redis/<key>", views.test_redis),')
    
-   206         332 LOAD_CONST              47 ('lf.aws.RDSPostgres')
+   180         350 LOAD_CONST              22 ('redis>=4.2.0')
+               352 BUILD_LIST               1
    
-   207         334 LOAD_CONST              17 ('')
+   181         354 LOAD_CONST               1 (None)
    
-   208         336 LOAD_CONST               1 (None)
+   160         356 LOAD_CONST              23 (('infra_docs_url', 'infra_name', 'infra_lf_class', 'django_settings', 'views_imports', 'django_test_endpoint', 'django_test_endpoint_url', 'requirements', 'installed_app'))
+               358 BUILD_CONST_KEY_MAP      9
    
-   209         338 LOAD_CONST               1 (None)
+   184         360 LOAD_NAME               14 (RDSPostgres)
    
-   211         340 LOAD_CONST              34 ('from app.models import Base, StorageUser')
+   185         362 LOAD_CONST              54 ('https://docs.launchflow.com/reference/aws-resources/rds-postgres')
    
-   212         342 LOAD_CONST              35 ('from app.schemas import ListUsersResponse, UserResponse')
+   186         364 LOAD_CONST              38 ('postgres')
    
-   210         344 BUILD_LIST               2
+   187         366 LOAD_CONST              55 ('lf.aws.RDSPostgres')
    
-   214         346 LOAD_CONST              36 ('# Configure the Postgres database with Flask-SQLAlchemy\ndb = SQLAlchemy(\n    app,\n    model_class=Base,\n    engine_options=postgres.sqlalchemy_engine_options(),\n)\n\nwith app.app_context():\n    db.create_all()')
+   188         368 LOAD_CONST               1 (None)
    
-   223         348 LOAD_CONST              37 ('\n"""\nThe endpoints below define a simple CRUD API for a generic StorageUser model.\n\nThe StorageUser model is defined in app.models\nThe ListUsersResponse and UserResponse schemas are defined in app.schemas.\n"""\n\n\n@app.get("/users")\ndef list_users():\n    storage_users = db.session.execute(select(StorageUser)).scalars().all()\n    return jsonify(\n        ListUsersResponse.from_storage(storage_users).model_dump(mode="json")\n    )\n\n\n@app.post("/users")\ndef create_user():\n    data = request.json\n    storage_user = StorageUser(email=data["email"], name=data["name"])\n    db.session.add(storage_user)\n    db.session.commit()\n    return jsonify(UserResponse.from_storage(storage_user).model_dump(mode="json"))\n\n\n@app.get("/users/<int:user_id>")\ndef read_user(user_id: int):\n    storage_user = db.session.get(StorageUser, user_id)\n    if storage_user is None:\n        abort(404, "User not found")\n    return jsonify(UserResponse.from_storage(storage_user).model_dump(mode="json"))\n\n\n@app.put("/users/<int:user_id>")\ndef update_user(user_id: int):\n    storage_user = db.session.get(StorageUser, user_id)\n    if storage_user is None:\n        abort(404, "User not found")\n    data = request.json\n    storage_user.name = data["name"]\n    db.session.commit()\n    return jsonify(UserResponse.from_storage(storage_user).model_dump(mode="json"))\n\n\n@app.delete("/users/<int:user_id>")\ndef delete_user(user_id):\n    storage_user = db.session.get(StorageUser, user_id)\n    if storage_user is None:\n        abort(404, "User not found")\n    db.session.delete(storage_user)\n    db.session.commit()\n    return jsonify(UserResponse.from_storage(storage_user).model_dump(mode="json"))\n')
+   189         370 LOAD_CONST              40 ('DATABASES = {\n    "default": postgres.django_settings(),\n}\n')
    
-   277         350 LOAD_CONST              38 ('Flask-SQLAlchemy')
-               352 LOAD_CONST              39 ('pg8000')
-               354 BUILD_LIST               2
+   193         372 LOAD_CONST               1 (None)
    
-   203         356 LOAD_CONST              40 (('infra_docs_url', 'infra_name', 'infra_lf_class', 'launchflow_imports', 'infra_import', 'global_setup', 'app_imports', 'infra_setup', 'flask_test_endpoint', 'requirements'))
-               358 BUILD_CONST_KEY_MAP     10
+   194         374 LOAD_CONST               1 (None)
    
-    30         360 BUILD_MAP                6
-               362 STORE_NAME              25 (resource_type_to_resource_info_kwargs)
+   195         376 LOAD_CONST              41 ('psycopg2-binary')
+               378 BUILD_LIST               1
    
-   282         364 LOAD_CONST              48 ('resource')
-               366 LOAD_NAME                7 (Type)
-               368 LOAD_NAME               23 (Resource)
-               370 BINARY_SUBSCR
-               380 LOAD_CONST              49 ('return')
-               382 LOAD_NAME               24 (ResourceInfo)
-               384 BUILD_TUPLE              4
-               386 LOAD_CONST              50 (<code object get_resource_info, file "/home/tanke/launchflow/launchflow/clients/python/launchflow/launchflow/cli/gen/templates/flask/flask_template.py", line 282>)
-               388 MAKE_FUNCTION            4 (annotations)
-               390 STORE_NAME              26 (get_resource_info)
+   196         380 LOAD_CONST               1 (None)
    
-   291         392 LOAD_NAME                2 (dataclass)
+   184         382 LOAD_CONST              49 (('infra_docs_url', 'infra_name', 'infra_lf_class', 'views_imports', 'django_settings', 'django_test_endpoint', 'django_test_endpoint_url', 'requirements', 'installed_app'))
+               384 BUILD_CONST_KEY_MAP      9
    
-   292         394 PUSH_NULL
-               396 LOAD_BUILD_CLASS
-               398 LOAD_CONST              51 (<code object FlaskProjectGenerator, file "/home/tanke/launchflow/launchflow/clients/python/launchflow/launchflow/cli/gen/templates/flask/flask_template.py", line 291>)
-               400 MAKE_FUNCTION            0
-               402 LOAD_CONST              52 ('FlaskProjectGenerator')
-               404 LOAD_NAME               13 (ProjectGenerator)
-               406 PRECALL                  3
-               410 CALL                     3
+    30         386 BUILD_MAP                7
+               388 STORE_NAME              28 (resource_type_to_resource_info_kwargs)
    
-   291         420 PRECALL                  0
-               424 CALL                     0
+   201         390 LOAD_CONST              56 ('resource')
+               392 LOAD_NAME                8 (Type)
+               394 LOAD_NAME               10 (Resource)
+               396 BINARY_SUBSCR
+               406 LOAD_CONST              57 ('return')
+               408 LOAD_NAME               27 (ResourceInfo)
+               410 BUILD_TUPLE              4
+               412 LOAD_CONST              58 (<code object get_resource_info, file "/Users/calebvandyke/code/launchflow-oss/launchflow/cli/gen/templates/django/django_template.py", line 201>)
+               414 MAKE_FUNCTION            4 (annotations)
+               416 STORE_NAME              29 (get_resource_info)
    
-   292         434 STORE_NAME              27 (FlaskProjectGenerator)
+   210         418 LOAD_NAME                3 (dataclass)
    
-   476         436 LOAD_NAME               28 (__name__)
-               438 LOAD_CONST              53 ('__main__')
-               440 COMPARE_OP               2 (==)
-               446 POP_JUMP_FORWARD_IF_FALSE    48 (to 544)
+   211         420 PUSH_NULL
+               422 LOAD_BUILD_CLASS
+               424 LOAD_CONST              59 (<code object DjangoProjectGenerator, file "/Users/calebvandyke/code/launchflow-oss/launchflow/cli/gen/templates/django/django_template.py", line 210>)
+               426 MAKE_FUNCTION            0
+               428 LOAD_CONST              60 ('DjangoProjectGenerator')
+               430 LOAD_NAME               18 (ProjectGenerator)
+               432 PRECALL                  3
+               436 CALL                     3
    
-   477         448 LOAD_CONST              54 ('gcp')
-               450 STORE_NAME              29 (cloud_provider)
+   210         446 PRECALL                  0
+               450 CALL                     0
    
-   478         452 PUSH_NULL
-               454 LOAD_NAME               27 (FlaskProjectGenerator)
-   
-   480         456 LOAD_NAME               17 (ComputeEngineRedis)
-   
-   481         458 LOAD_NAME               19 (GCSBucket)
-   
-   482         460 LOAD_NAME               15 (CloudSQLPostgres)
-   
-   479         462 BUILD_LIST               3
-   
-   486         464 LOAD_NAME               29 (cloud_provider)
-   
-   487         466 LOAD_NAME               29 (cloud_provider)
-               468 FORMAT_VALUE             0
-               470 LOAD_CONST              55 ('-examples')
-               472 BUILD_STRING             2
-   
-   488         474 LOAD_CONST              56 ('dev')
-   
-   489         476 LOAD_CONST              57 ('flask-service')
-   
-   478         478 KW_NAMES                58
-               480 PRECALL                  5
-               484 CALL                     5
-               494 STORE_NAME              30 (generator)
-   
-   491         496 LOAD_NAME               30 (generator)
-               498 LOAD_METHOD             31 (generate_project)
-               520 LOAD_CONST              59 ('/tmp/launchflow')
-               522 KW_NAMES                60
-               524 PRECALL                  1
-               528 CALL                     1
-               538 POP_TOP
-               540 LOAD_CONST               1 (None)
-               542 RETURN_VALUE
-   
-   476     >>  544 LOAD_CONST               1 (None)
-               546 RETURN_VALUE
+   211         460 STORE_NAME              30 (DjangoProjectGenerator)
+               462 LOAD_CONST               1 (None)
+               464 RETURN_VALUE
    consts
       0
       None
       ('dataclass',)
       ('List', 'Literal', 'Optional', 'Type')
+      ('Resource',)
+      ('ElasticacheRedis',)
       ('RDSPostgres',)
       ('S3Bucket',)
       ('ProjectGenerator',)
       ('CloudSQLPostgres',)
       ('ComputeEngineRedis',)
       ('GCSBucket',)
       ('MemorystoreRedis',)
-      ('Resource',)
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 3
          flags     : 0
          code
             0x970065005a0164005a0255006503650464013c0000006503650464023c
-            0000006503650464033c0000006503650464043c00000065056503190000
-            00000000000000650464053c000000650565031900000000000000000065
-            0464063c0000006505650319000000000000000000650464073c00000065
-            06650319000000000000000000650464083c0000006503650464093c0000
-            0065066503190000000000000000006504640a3c000000640b5300
-          16           0 RESUME                   0
+            0000006503650464033c0000006505650319000000000000000000650464
+            043c0000006505650319000000000000000000650464053c000000650565
+            0319000000000000000000650464063c0000006505650319000000000000
+            000000650464073c0000006506650319000000000000000000650464083c
+            0000006505650319000000000000000000650464093c000000640a5300
+          17           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('ResourceInfo')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
-          18          12 LOAD_NAME                3 (str)
+          19          12 LOAD_NAME                3 (str)
                       14 LOAD_NAME                4 (__annotations__)
                       16 LOAD_CONST               1 ('infra_docs_url')
                       18 STORE_SUBSCR
          
-          19          22 LOAD_NAME                3 (str)
+          20          22 LOAD_NAME                3 (str)
                       24 LOAD_NAME                4 (__annotations__)
                       26 LOAD_CONST               2 ('infra_name')
                       28 STORE_SUBSCR
          
-          20          32 LOAD_NAME                3 (str)
+          21          32 LOAD_NAME                3 (str)
                       34 LOAD_NAME                4 (__annotations__)
                       36 LOAD_CONST               3 ('infra_lf_class')
                       38 STORE_SUBSCR
          
-          21          42 LOAD_NAME                3 (str)
-                      44 LOAD_NAME                4 (__annotations__)
-                      46 LOAD_CONST               4 ('launchflow_imports')
-                      48 STORE_SUBSCR
-         
-          22          52 LOAD_NAME                5 (Optional)
-                      54 LOAD_NAME                3 (str)
-                      56 BINARY_SUBSCR
-                      66 LOAD_NAME                4 (__annotations__)
-                      68 LOAD_CONST               5 ('infra_import')
-                      70 STORE_SUBSCR
-         
-          23          74 LOAD_NAME                5 (Optional)
-                      76 LOAD_NAME                3 (str)
-                      78 BINARY_SUBSCR
-                      88 LOAD_NAME                4 (__annotations__)
-                      90 LOAD_CONST               6 ('global_setup')
-                      92 STORE_SUBSCR
-         
-          24          96 LOAD_NAME                5 (Optional)
-                      98 LOAD_NAME                3 (str)
-                     100 BINARY_SUBSCR
-                     110 LOAD_NAME                4 (__annotations__)
-                     112 LOAD_CONST               7 ('infra_setup')
-                     114 STORE_SUBSCR
-         
-          25         118 LOAD_NAME                6 (List)
-                     120 LOAD_NAME                3 (str)
-                     122 BINARY_SUBSCR
-                     132 LOAD_NAME                4 (__annotations__)
-                     134 LOAD_CONST               8 ('app_imports')
-                     136 STORE_SUBSCR
-         
-          26         140 LOAD_NAME                3 (str)
-                     142 LOAD_NAME                4 (__annotations__)
-                     144 LOAD_CONST               9 ('flask_test_endpoint')
-                     146 STORE_SUBSCR
-         
-          27         150 LOAD_NAME                6 (List)
-                     152 LOAD_NAME                3 (str)
-                     154 BINARY_SUBSCR
-                     164 LOAD_NAME                4 (__annotations__)
-                     166 LOAD_CONST              10 ('requirements')
-                     168 STORE_SUBSCR
-                     172 LOAD_CONST              11 (None)
-                     174 RETURN_VALUE
+          22          42 LOAD_NAME                5 (Optional)
+                      44 LOAD_NAME                3 (str)
+                      46 BINARY_SUBSCR
+                      56 LOAD_NAME                4 (__annotations__)
+                      58 LOAD_CONST               4 ('django_settings')
+                      60 STORE_SUBSCR
+         
+          23          64 LOAD_NAME                5 (Optional)
+                      66 LOAD_NAME                3 (str)
+                      68 BINARY_SUBSCR
+                      78 LOAD_NAME                4 (__annotations__)
+                      80 LOAD_CONST               5 ('views_imports')
+                      82 STORE_SUBSCR
+         
+          24          86 LOAD_NAME                5 (Optional)
+                      88 LOAD_NAME                3 (str)
+                      90 BINARY_SUBSCR
+                     100 LOAD_NAME                4 (__annotations__)
+                     102 LOAD_CONST               6 ('django_test_endpoint')
+                     104 STORE_SUBSCR
+         
+          25         108 LOAD_NAME                5 (Optional)
+                     110 LOAD_NAME                3 (str)
+                     112 BINARY_SUBSCR
+                     122 LOAD_NAME                4 (__annotations__)
+                     124 LOAD_CONST               7 ('django_test_endpoint_url')
+                     126 STORE_SUBSCR
+         
+          26         130 LOAD_NAME                6 (List)
+                     132 LOAD_NAME                3 (str)
+                     134 BINARY_SUBSCR
+                     144 LOAD_NAME                4 (__annotations__)
+                     146 LOAD_CONST               8 ('requirements')
+                     148 STORE_SUBSCR
+         
+          27         152 LOAD_NAME                5 (Optional)
+                     154 LOAD_NAME                3 (str)
+                     156 BINARY_SUBSCR
+                     166 LOAD_NAME                4 (__annotations__)
+                     168 LOAD_CONST               9 ('installed_app')
+                     170 STORE_SUBSCR
+                     174 LOAD_CONST              10 (None)
+                     176 RETURN_VALUE
          consts
             'ResourceInfo'
             'infra_docs_url'
             'infra_name'
             'infra_lf_class'
-            'launchflow_imports'
-            'infra_import'
-            'global_setup'
-            'infra_setup'
-            'app_imports'
-            'flask_test_endpoint'
+            'django_settings'
+            'views_imports'
+            'django_test_endpoint'
+            'django_test_endpoint_url'
             'requirements'
+            'installed_app'
             None
          names      ('__name__', '__module__', '__qualname__', 'str', '__annotations__', 'Optional', 'List')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/home/tanke/launchflow/launchflow/clients/python/launchflow/launchflow/cli/gen/templates/flask/flask_template.py'
+         filename   '/Users/calebvandyke/code/launchflow-oss/launchflow/cli/gen/templates/django/django_template.py'
          name       'ResourceInfo'
-         firstlineno 16
-         lnotab 0x0c020a010a010a010a0116011601160116010a01
+         firstlineno 17
+         lnotab 0x0c020a010a010a0116011601160116011601
       'ResourceInfo'
-      'https://docs.launchflow.com/reference/gcp-resources/compute-engine'
+      'https://docs.launchflow.com/reference/gcp-resources/compute-engine#compute-engine-redis'
       'redis_vm'
       'lf.gcp.ComputeEngineRedis'
-      ''
-      '# Connect to the Redis instance\nredis_client = redis_vm.redis()\n'
-      '\n# NOTE: This should normally use a POST request since it\'s modifying state, but we\'re\n# using GET so you can easily test it in your browser.\n@app.get("/test_redis/<key>")\ndef test_redis(key: str):\n    value = request.json["value"]\n    # Write to Redis\n    redis_client.set(key, value)\n    # Immediately read from Redis to verify the write\n    value = redis_client.get(key)\n    return jsonify({"message": f"Set {key} to {value}"})\n'
+      'CACHES = {\n    "default": redis_vm.django_settings(),\n}\n'
+      'from django.core.cache import cache'
+      '\n# NOTE: This should normally use a POST request since it\'s modifying state, but we\'re\n# using GET so you can easily test it in your browser.\n@api_view(["GET"])\ndef test_redis(request, key):\n    # Write to cache (Redis)\n    cache.set(key, "Hello from Redis!", timeout=60)\n    # Immediately read from cache to verify write\n    return Response({"message": cache.get(key)})\n'
+      'path("test_redis/<key>", views.test_redis),'
       'redis>=4.2.0'
-      ('infra_docs_url', 'infra_name', 'infra_lf_class', 'launchflow_imports', 'infra_import', 'global_setup', 'infra_setup', 'app_imports', 'flask_test_endpoint', 'requirements')
-      'https://docs.launchflow.com/reference/gcp-resources/memorystore-redis'
-      'redis_cluster'
+      ('infra_docs_url', 'infra_name', 'infra_lf_class', 'django_settings', 'views_imports', 'django_test_endpoint', 'django_test_endpoint_url', 'requirements', 'installed_app')
+      'https://docs.launchflow.com/reference/gcp-resources/memorystore'
+      'memorystore'
       'lf.gcp.MemorystoreRedis'
-      '\n# NOTE: This should normally use a POST request since it\'s modifying state, but we\'re\n# using GET so you can easily test it in your browser.\n@app.get("/test_redis/<key>")\ndef test_redis(key: str):\n    # Write to Redis\n    value = request.json["value"]\n    redis_client.set(key, value)\n    # Immediately read from Redis to verify the write\n    value = redis_client.get(key)\n    return jsonify({"message": f"Set {key} to {value}"})\n'
+      'CACHES = {\n    "default": memorystore.django_settings(),\n}\n'
       'https://docs.launchflow.com/reference/gcp-resources/gcs-bucket'
       'gcs_bucket'
       'lf.gcp.GCSBucket'
-      '# Connect to the storage Bucket\ngcs_bucket.connect()\n'
-      '\n# NOTE: This should normally use a POST request since it\'s modifying state, but we\'re\n# using GET so you can easily test it in your browser.\n@app.get("/test_gcs/<object_name>")\ndef test_gcs(object_name: str):\n    # Write to GCS\n    gcs_bucket.upload_from_string("Hello, World!", object_name)\n    # Immediately read from GCS to verify the write\n    gcs_bucket.download_file(object_name).decode("utf-8")\n    return jsonify({"message": f"Uploaded {object_name} to GCS"})\n'
+      'STORAGES = {\n    "default": {\n        "BACKEND": "storages.backends.gcloud.GoogleCloudStorage",\n    },\n    "staticfiles": {\n        "BACKEND": "storages.backends.gcloud.GoogleCloudStorage",\n    },\n}\nGS_BUCKET_NAME = gcs_bucket.connect().bucket_name\nGS_CREDENTIALS = lf.gcp.get_service_account_credentials()\n'
+      'from django.core.files.storage import default_storage'
+      '\n# NOTE: This should normally use a POST request since it\'s modifying state, but we\'re\n# using GET so you can easily test it in your browser.\n@api_view(["GET"])\ndef test_gcs(request, object_name):\n    # Write to GCS\n    with default_storage.open(object_name, "w") as file:\n        file.write("Hello from GCS!")\n    # Immediately read from GCS to verify write\n    with default_storage.open(object_name, "r") as file:\n        return Response({"message": file.read()})\n'
+      'path("test_gcs/<object_name>", views.test_gcs),'
+      'django-storages[google]'
+      'storages'
       'https://docs.launchflow.com/reference/gcp-resources/cloud-sql'
       'postgres'
       'lf.gcp.CloudSQLPostgres'
-      'from app.models import Base, StorageUser'
-      'from app.schemas import ListUsersResponse, UserResponse'
-      '# Configure the Postgres database with Flask-SQLAlchemy\ndb = SQLAlchemy(\n    app,\n    model_class=Base,\n    engine_options=postgres.sqlalchemy_engine_options(),\n)\n\nwith app.app_context():\n    db.create_all()'
-      '\n"""\nThe endpoints below define a simple CRUD API for a generic StorageUser model.\n\nThe StorageUser model is defined in app.models\nThe ListUsersResponse and UserResponse schemas are defined in app.schemas.\n"""\n\n\n@app.get("/users")\ndef list_users():\n    storage_users = db.session.execute(select(StorageUser)).scalars().all()\n    return jsonify(\n        ListUsersResponse.from_storage(storage_users).model_dump(mode="json")\n    )\n\n\n@app.post("/users")\ndef create_user():\n    data = request.json\n    storage_user = StorageUser(email=data["email"], name=data["name"])\n    db.session.add(storage_user)\n    db.session.commit()\n    return jsonify(UserResponse.from_storage(storage_user).model_dump(mode="json"))\n\n\n@app.get("/users/<int:user_id>")\ndef read_user(user_id: int):\n    storage_user = db.session.get(StorageUser, user_id)\n    if storage_user is None:\n        abort(404, "User not found")\n    return jsonify(UserResponse.from_storage(storage_user).model_dump(mode="json"))\n\n\n@app.put("/users/<int:user_id>")\ndef update_user(user_id: int):\n    storage_user = db.session.get(StorageUser, user_id)\n    if storage_user is None:\n        abort(404, "User not found")\n    data = request.json\n    storage_user.name = data["name"]\n    db.session.commit()\n    return jsonify(UserResponse.from_storage(storage_user).model_dump(mode="json"))\n\n\n@app.delete("/users/<int:user_id>")\ndef delete_user(user_id):\n    storage_user = db.session.get(StorageUser, user_id)\n    if storage_user is None:\n        abort(404, "User not found")\n    db.session.delete(storage_user)\n    db.session.commit()\n    return jsonify(UserResponse.from_storage(storage_user).model_dump(mode="json"))\n'
-      'Flask-SQLAlchemy'
-      'pg8000'
-      ('infra_docs_url', 'infra_name', 'infra_lf_class', 'launchflow_imports', 'infra_import', 'global_setup', 'app_imports', 'infra_setup', 'flask_test_endpoint', 'requirements')
+      'DATABASES = {\n    "default": postgres.django_settings(),\n}\n'
+      'psycopg2-binary'
       'https://docs.launchflow.com/reference/aws-resources/s3-bucket'
       's3_bucket'
       'lf.aws.S3Bucket'
-      '# Connect to the storage Bucket\ns3_bucket.connect()\n'
-      '\n# NOTE: This should normally use a POST request since it\'s modifying state, but we\'re\n# using GET so you can easily test it in your browser.\n@app.get("/test_s3/<object_name>")\ndef test_s3(object_name: str):\n    # Write to S3\n    s3_bucket.upload_from_string("Hello, World!", object_name)\n    # Immediately read from S3 to verify the write\n    s3_bucket.download_file(object_name).decode("utf-8")\n    return jsonify({"message": f"Uploaded {object_name} to S3"})\n'
-      'https://docs.launchflow.com/reference/aws-resources/rds'
+      'STORAGES = {\n    "default": {\n        "BACKEND": "storages.backends.s3.S3Storage",\n    },\n    "staticfiles": {\n        "BACKEND": "storages.backends.s3.S3Storage",\n    },\n}\nAWS_STORAGE_BUCKET_NAME = s3_bucket.connect().bucket_name\n'
+      '\n# NOTE: This should normally use a POST request since it\'s modifying state, but we\'re\n# using GET so you can easily test it in your browser.\n@api_view(["GET"])\ndef test_s3(request, object_name):\n    # Write to S3\n    with default_storage.open(object_name, "w") as file:\n        file.write("Hello from S3!")\n    # Immediately read from S3 to verify write\n    with default_storage.open(object_name, "r") as file:\n        return Response({"message": file.read()})\n'
+      'path("test_s3/<object_name>", views.test_s3),'
+      'django-storages[s3]'
+      ('infra_docs_url', 'infra_name', 'infra_lf_class', 'views_imports', 'django_settings', 'django_test_endpoint', 'django_test_endpoint_url', 'requirements', 'installed_app')
+      'https://docs.launchflow.com/reference/aws-resources/elasticache-redis'
+      'elasticache'
+      'lf.aws.ElasticacheRedis'
+      'CACHES = {\n    "default": elasticache.django_settings(),\n}\n'
+      'https://docs.launchflow.com/reference/aws-resources/rds-postgres'
       'lf.aws.RDSPostgres'
       'resource'
       'return'
       code
          argcount  : 1
          nlocals   : 2
          stacksize : 5
          flags     : 3
          code
             0x9700740000000000000000000000a00100000000000000000000000000
             000000000000007c006400a6020000ab0200000000000000007d017c0180
             1274050000000000000000000064017c009b009d02a6010000ab01000000
             00000000008201740700000000000000000000640269007c01a4018e0153
             00
-         282           0 RESUME                   0
+         201           0 RESUME                   0
          
-         283           2 LOAD_GLOBAL              0 (resource_type_to_resource_info_kwargs)
+         202           2 LOAD_GLOBAL              0 (resource_type_to_resource_info_kwargs)
                       14 LOAD_METHOD              1 (get)
                       36 LOAD_FAST                0 (resource)
                       38 LOAD_CONST               0 (None)
                       40 PRECALL                  2
                       44 CALL                     2
                       54 STORE_FAST               1 (resource_info_kwargs)
          
-         284          56 LOAD_FAST                1 (resource_info_kwargs)
+         203          56 LOAD_FAST                1 (resource_info_kwargs)
                       58 POP_JUMP_FORWARD_IF_NOT_NONE    18 (to 96)
          
-         285          60 LOAD_GLOBAL              5 (NULL + ValueError)
+         204          60 LOAD_GLOBAL              5 (NULL + ValueError)
                       72 LOAD_CONST               1 ('Unsupported resource type: ')
                       74 LOAD_FAST                0 (resource)
                       76 FORMAT_VALUE             0
                       78 BUILD_STRING             2
                       80 PRECALL                  1
                       84 CALL                     1
                       94 RAISE_VARARGS            1
          
-         286     >>   96 LOAD_GLOBAL              7 (NULL + ResourceInfo)
+         205     >>   96 LOAD_GLOBAL              7 (NULL + ResourceInfo)
                      108 LOAD_CONST               2 (())
                      110 BUILD_MAP                0
          
-         287         112 LOAD_FAST                1 (resource_info_kwargs)
+         206         112 LOAD_FAST                1 (resource_info_kwargs)
          
-         286         114 DICT_MERGE               1
+         205         114 DICT_MERGE               1
                      116 CALL_FUNCTION_EX         1
                      118 RETURN_VALUE
          consts
             None
             'Unsupported resource type: '
             ()
          names      ('resource_type_to_resource_info_kwargs', 'get', 'ValueError', 'ResourceInfo')
          varnames   ('resource', 'resource_info_kwargs')
          freevars   ()
          cellvars   ()
-         filename   '/home/tanke/launchflow/launchflow/clients/python/launchflow/launchflow/cli/gen/templates/flask/flask_template.py'
+         filename   '/Users/calebvandyke/code/launchflow-oss/launchflow/cli/gen/templates/django/django_template.py'
          name       'get_resource_info'
-         firstlineno 282
+         firstlineno 201
          lnotab 0x0201360104012401100102ff
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 4
          flags     : 0
          code
             0x970065005a0164005a0255006503650465051900000000000000000019
             000000000000000000650664013c00000065076402190000000000000000
             00650664033c0000006508650664043c0000006508650664053c00000064
             065a096508650664073c000000650a6a0b00000000000000006a0c000000
             00000000005a0d650e650664083c000000650a6a0b00000000000000006a
             0f00000000000000005a10650e650664093c000000640a5a116512640b65
-            086602640c8404a6000000ab0000000000000000005a136512640b650866
-            02640d8404a6000000ab0000000000000000005a146512640b6503650819
-            0000000000000000006602640e8404a6000000ab0000000000000000005a
-            156512640b65086602640f8404a6000000ab0000000000000000005a1665
-            12640b6503650819000000000000000000660264108404a6000000ab0000
-            000000000000005a176512640b6503650819000000000000000000660264
-            118404a6000000ab0000000000000000005a186512640b65036508190000
-            00000000000000660264128404a6000000ab0000000000000000005a1965
-            12640b6508660264138404a6000000ab0000000000000000005a1a640b65
-            086602641484045a1b6512640b6508660264158404a6000000ab00000000
-            00000000005a1c640b651d6602641684045a1e64175300
-         291           0 RESUME                   0
+            086602640c8404a6000000ab0000000000000000005a136512640b650365
+            08190000000000000000006602640d8404a6000000ab0000000000000000
+            005a146512640b65086602640e8404a6000000ab0000000000000000005a
+            156512640b65036508190000000000000000006602640f8404a6000000ab
+            0000000000000000005a166512640b650365081900000000000000000066
+            0264108404a6000000ab0000000000000000005a176512640b6503650819
+            000000000000000000660264118404a6000000ab0000000000000000005a
+            186512640b6503650819000000000000000000660264128404a6000000ab
+            0000000000000000005a196512640b650365081900000000000000000066
+            0264138404a6000000ab0000000000000000005a1a6512640b6508660264
+            148404a6000000ab0000000000000000005a1b640b65086602641584045a
+            1c6512640b6508660264168404a6000000ab0000000000000000005a1d64
+            0b651e6602641784045a1f64185300
+         210           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
-                       6 LOAD_CONST               0 ('FlaskProjectGenerator')
+                       6 LOAD_CONST               0 ('DjangoProjectGenerator')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
-         293          12 LOAD_NAME                3 (List)
+         212          12 LOAD_NAME                3 (List)
                       14 LOAD_NAME                4 (Type)
                       16 LOAD_NAME                5 (Resource)
                       18 BINARY_SUBSCR
                       28 BINARY_SUBSCR
                       38 LOAD_NAME                6 (__annotations__)
                       40 LOAD_CONST               1 ('resources')
                       42 STORE_SUBSCR
          
-         295          46 LOAD_NAME                7 (Literal)
+         214          46 LOAD_NAME                7 (Literal)
                       48 LOAD_CONST               2 (('aws', 'gcp'))
                       50 BINARY_SUBSCR
                       60 LOAD_NAME                6 (__annotations__)
                       62 LOAD_CONST               3 ('cloud_provider')
                       64 STORE_SUBSCR
          
-         297          68 LOAD_NAME                8 (str)
+         216          68 LOAD_NAME                8 (str)
                       70 LOAD_NAME                6 (__annotations__)
                       72 LOAD_CONST               4 ('launchflow_project_name')
                       74 STORE_SUBSCR
          
-         298          78 LOAD_NAME                8 (str)
+         217          78 LOAD_NAME                8 (str)
                       80 LOAD_NAME                6 (__annotations__)
                       82 LOAD_CONST               5 ('launchflow_environment_name')
                       84 STORE_SUBSCR
          
-         299          88 LOAD_CONST               6 ('flask-service')
+         218          88 LOAD_CONST               6 ('django-service')
                       90 STORE_NAME               9 (launchflow_service_name)
                       92 LOAD_NAME                8 (str)
                       94 LOAD_NAME                6 (__annotations__)
                       96 LOAD_CONST               7 ('launchflow_service_name')
                       98 STORE_SUBSCR
          
-         301         102 LOAD_NAME               10 (sys)
+         220         102 LOAD_NAME               10 (sys)
                      104 LOAD_ATTR               11 (version_info)
                      114 LOAD_ATTR               12 (major)
                      124 STORE_NAME              13 (python_major_version)
                      126 LOAD_NAME               14 (int)
                      128 LOAD_NAME                6 (__annotations__)
                      130 LOAD_CONST               8 ('python_major_version')
                      132 STORE_SUBSCR
          
-         302         136 LOAD_NAME               10 (sys)
+         221         136 LOAD_NAME               10 (sys)
                      138 LOAD_ATTR               11 (version_info)
                      148 LOAD_ATTR               15 (minor)
                      158 STORE_NAME              16 (python_minor_version)
                      160 LOAD_NAME               14 (int)
                      162 LOAD_NAME                6 (__annotations__)
                      164 LOAD_CONST               9 ('python_minor_version')
                      166 STORE_SUBSCR
          
-         303         170 LOAD_CONST              10 (8080)
+         222         170 LOAD_CONST              10 (8080)
                      172 STORE_NAME              17 (port)
          
-         306         174 LOAD_NAME               18 (property)
+         225         174 LOAD_NAME               18 (property)
          
-         307         176 LOAD_CONST              11 ('return')
+         226         176 LOAD_CONST              11 ('return')
                      178 LOAD_NAME                8 (str)
                      180 BUILD_TUPLE              2
-                     182 LOAD_CONST              12 (<code object infra_dot_py, file "/home/tanke/launchflow/launchflow/clients/python/launchflow/launchflow/cli/gen/templates/flask/flask_template.py", line 306>)
+                     182 LOAD_CONST              12 (<code object infra_dot_py, file "/Users/calebvandyke/code/launchflow-oss/launchflow/cli/gen/templates/django/django_template.py", line 225>)
                      184 MAKE_FUNCTION            4 (annotations)
          
-         306         186 PRECALL                  0
+         225         186 PRECALL                  0
                      190 CALL                     0
          
-         307         200 STORE_NAME              19 (infra_dot_py)
+         226         200 STORE_NAME              19 (infra_dot_py)
          
-         353         202 LOAD_NAME               18 (property)
+         272         202 LOAD_NAME               18 (property)
          
-         354         204 LOAD_CONST              11 ('return')
-                     206 LOAD_NAME                8 (str)
-                     208 BUILD_TUPLE              2
-                     210 LOAD_CONST              13 (<code object flask_imports, file "/home/tanke/launchflow/launchflow/clients/python/launchflow/launchflow/cli/gen/templates/flask/flask_template.py", line 353>)
-                     212 MAKE_FUNCTION            4 (annotations)
+         273         204 LOAD_CONST              11 ('return')
+                     206 LOAD_NAME                3 (List)
+                     208 LOAD_NAME                8 (str)
+                     210 BINARY_SUBSCR
+                     220 BUILD_TUPLE              2
+                     222 LOAD_CONST              13 (<code object app_infra_imports, file "/Users/calebvandyke/code/launchflow-oss/launchflow/cli/gen/templates/django/django_template.py", line 272>)
+                     224 MAKE_FUNCTION            4 (annotations)
          
-         353         214 PRECALL                  0
-                     218 CALL                     0
+         272         226 PRECALL                  0
+                     230 CALL                     0
          
-         354         228 STORE_NAME              20 (flask_imports)
+         273         240 STORE_NAME              20 (app_infra_imports)
          
-         366         230 LOAD_NAME               18 (property)
+         294         242 LOAD_NAME               18 (property)
          
-         367         232 LOAD_CONST              11 ('return')
-                     234 LOAD_NAME                3 (List)
-                     236 LOAD_NAME                8 (str)
-                     238 BINARY_SUBSCR
+         295         244 LOAD_CONST              11 ('return')
+                     246 LOAD_NAME                8 (str)
                      248 BUILD_TUPLE              2
-                     250 LOAD_CONST              14 (<code object app_infra_imports, file "/home/tanke/launchflow/launchflow/clients/python/launchflow/launchflow/cli/gen/templates/flask/flask_template.py", line 366>)
+                     250 LOAD_CONST              14 (<code object app_django_settings, file "/Users/calebvandyke/code/launchflow-oss/launchflow/cli/gen/templates/django/django_template.py", line 294>)
                      252 MAKE_FUNCTION            4 (annotations)
          
-         366         254 PRECALL                  0
+         294         254 PRECALL                  0
                      258 CALL                     0
          
-         367         268 STORE_NAME              21 (app_infra_imports)
+         295         268 STORE_NAME              21 (app_django_settings)
+         
+         334         270 LOAD_NAME               18 (property)
          
-         391         270 LOAD_NAME               18 (property)
+         335         272 LOAD_CONST              11 ('return')
+                     274 LOAD_NAME                3 (List)
+                     276 LOAD_NAME                8 (str)
+                     278 BINARY_SUBSCR
+                     288 BUILD_TUPLE              2
+                     290 LOAD_CONST              15 (<code object app_installed_apps, file "/Users/calebvandyke/code/launchflow-oss/launchflow/cli/gen/templates/django/django_template.py", line 334>)
+                     292 MAKE_FUNCTION            4 (annotations)
          
-         392         272 LOAD_CONST              11 ('return')
-                     274 LOAD_NAME                8 (str)
-                     276 BUILD_TUPLE              2
-                     278 LOAD_CONST              15 (<code object app_global_setup, file "/home/tanke/launchflow/launchflow/clients/python/launchflow/launchflow/cli/gen/templates/flask/flask_template.py", line 391>)
-                     280 MAKE_FUNCTION            4 (annotations)
+         334         294 PRECALL                  0
+                     298 CALL                     0
          
-         391         282 PRECALL                  0
-                     286 CALL                     0
+         335         308 STORE_NAME              22 (app_installed_apps)
          
-         392         296 STORE_NAME              22 (app_global_setup)
+         344         310 LOAD_NAME               18 (property)
          
-         401         298 LOAD_NAME               18 (property)
+         345         312 LOAD_CONST              11 ('return')
+                     314 LOAD_NAME                3 (List)
+                     316 LOAD_NAME                8 (str)
+                     318 BINARY_SUBSCR
+                     328 BUILD_TUPLE              2
+                     330 LOAD_CONST              16 (<code object app_infra_urls, file "/Users/calebvandyke/code/launchflow-oss/launchflow/cli/gen/templates/django/django_template.py", line 344>)
+                     332 MAKE_FUNCTION            4 (annotations)
          
-         402         300 LOAD_CONST              11 ('return')
-                     302 LOAD_NAME                3 (List)
-                     304 LOAD_NAME                8 (str)
-                     306 BINARY_SUBSCR
-                     316 BUILD_TUPLE              2
-                     318 LOAD_CONST              16 (<code object app_infra_setup, file "/home/tanke/launchflow/launchflow/clients/python/launchflow/launchflow/cli/gen/templates/flask/flask_template.py", line 401>)
-                     320 MAKE_FUNCTION            4 (annotations)
+         344         334 PRECALL                  0
+                     338 CALL                     0
          
-         401         322 PRECALL                  0
-                     326 CALL                     0
+         345         348 STORE_NAME              23 (app_infra_urls)
          
-         402         336 STORE_NAME              23 (app_infra_setup)
+         354         350 LOAD_NAME               18 (property)
          
-         411         338 LOAD_NAME               18 (property)
+         355         352 LOAD_CONST              11 ('return')
+                     354 LOAD_NAME                3 (List)
+                     356 LOAD_NAME                8 (str)
+                     358 BINARY_SUBSCR
+                     368 BUILD_TUPLE              2
+                     370 LOAD_CONST              17 (<code object app_views_imports, file "/Users/calebvandyke/code/launchflow-oss/launchflow/cli/gen/templates/django/django_template.py", line 354>)
+                     372 MAKE_FUNCTION            4 (annotations)
          
-         412         340 LOAD_CONST              11 ('return')
-                     342 LOAD_NAME                3 (List)
-                     344 LOAD_NAME                8 (str)
-                     346 BINARY_SUBSCR
-                     356 BUILD_TUPLE              2
-                     358 LOAD_CONST              17 (<code object app_infra_endpoints, file "/home/tanke/launchflow/launchflow/clients/python/launchflow/launchflow/cli/gen/templates/flask/flask_template.py", line 411>)
-                     360 MAKE_FUNCTION            4 (annotations)
+         354         374 PRECALL                  0
+                     378 CALL                     0
          
-         411         362 PRECALL                  0
-                     366 CALL                     0
+         355         388 STORE_NAME              24 (app_views_imports)
          
-         412         376 STORE_NAME              24 (app_infra_endpoints)
+         364         390 LOAD_NAME               18 (property)
          
-         420         378 LOAD_NAME               18 (property)
+         365         392 LOAD_CONST              11 ('return')
+                     394 LOAD_NAME                3 (List)
+                     396 LOAD_NAME                8 (str)
+                     398 BINARY_SUBSCR
+                     408 BUILD_TUPLE              2
+                     410 LOAD_CONST              18 (<code object app_infra_endpoints, file "/Users/calebvandyke/code/launchflow-oss/launchflow/cli/gen/templates/django/django_template.py", line 364>)
+                     412 MAKE_FUNCTION            4 (annotations)
          
-         421         380 LOAD_CONST              11 ('return')
-                     382 LOAD_NAME                3 (List)
-                     384 LOAD_NAME                8 (str)
-                     386 BINARY_SUBSCR
-                     396 BUILD_TUPLE              2
-                     398 LOAD_CONST              18 (<code object additional_requirements, file "/home/tanke/launchflow/launchflow/clients/python/launchflow/launchflow/cli/gen/templates/flask/flask_template.py", line 420>)
-                     400 MAKE_FUNCTION            4 (annotations)
+         364         414 PRECALL                  0
+                     418 CALL                     0
          
-         420         402 PRECALL                  0
-                     406 CALL                     0
+         365         428 STORE_NAME              25 (app_infra_endpoints)
          
-         421         416 STORE_NAME              25 (additional_requirements)
+         374         430 LOAD_NAME               18 (property)
          
-         429         418 LOAD_NAME               18 (property)
+         375         432 LOAD_CONST              11 ('return')
+                     434 LOAD_NAME                3 (List)
+                     436 LOAD_NAME                8 (str)
+                     438 BINARY_SUBSCR
+                     448 BUILD_TUPLE              2
+                     450 LOAD_CONST              19 (<code object additional_requirements, file "/Users/calebvandyke/code/launchflow-oss/launchflow/cli/gen/templates/django/django_template.py", line 374>)
+                     452 MAKE_FUNCTION            4 (annotations)
          
-         430         420 LOAD_CONST              11 ('return')
-                     422 LOAD_NAME                8 (str)
-                     424 BUILD_TUPLE              2
-                     426 LOAD_CONST              19 (<code object launchflow_service_product, file "/home/tanke/launchflow/launchflow/clients/python/launchflow/launchflow/cli/gen/templates/flask/flask_template.py", line 429>)
-                     428 MAKE_FUNCTION            4 (annotations)
+         374         454 PRECALL                  0
+                     458 CALL                     0
          
-         429         430 PRECALL                  0
-                     434 CALL                     0
+         375         468 STORE_NAME              26 (additional_requirements)
          
-         430         444 STORE_NAME              26 (launchflow_service_product)
+         383         470 LOAD_NAME               18 (property)
          
-         437         446 LOAD_CONST              11 ('return')
-                     448 LOAD_NAME                8 (str)
-                     450 BUILD_TUPLE              2
-                     452 LOAD_CONST              20 (<code object template_directory, file "/home/tanke/launchflow/launchflow/clients/python/launchflow/launchflow/cli/gen/templates/flask/flask_template.py", line 437>)
-                     454 MAKE_FUNCTION            4 (annotations)
-                     456 STORE_NAME              27 (template_directory)
+         384         472 LOAD_CONST              11 ('return')
+                     474 LOAD_NAME                8 (str)
+                     476 BUILD_TUPLE              2
+                     478 LOAD_CONST              20 (<code object launchflow_service_product, file "/Users/calebvandyke/code/launchflow-oss/launchflow/cli/gen/templates/django/django_template.py", line 383>)
+                     480 MAKE_FUNCTION            4 (annotations)
          
-         444         458 LOAD_NAME               18 (property)
+         383         482 PRECALL                  0
+                     486 CALL                     0
          
-         445         460 LOAD_CONST              11 ('return')
-                     462 LOAD_NAME                8 (str)
-                     464 BUILD_TUPLE              2
-                     466 LOAD_CONST              21 (<code object docker_repository_prefix, file "/home/tanke/launchflow/launchflow/clients/python/launchflow/launchflow/cli/gen/templates/flask/flask_template.py", line 444>)
-                     468 MAKE_FUNCTION            4 (annotations)
+         384         496 STORE_NAME              27 (launchflow_service_product)
          
-         444         470 PRECALL                  0
-                     474 CALL                     0
+         391         498 LOAD_CONST              11 ('return')
+                     500 LOAD_NAME                8 (str)
+                     502 BUILD_TUPLE              2
+                     504 LOAD_CONST              21 (<code object template_path_info, file "/Users/calebvandyke/code/launchflow-oss/launchflow/cli/gen/templates/django/django_template.py", line 391>)
+                     506 MAKE_FUNCTION            4 (annotations)
+                     508 STORE_NAME              28 (template_path_info)
          
-         445         484 STORE_NAME              28 (docker_repository_prefix)
+         402         510 LOAD_NAME               18 (property)
          
-         450         486 LOAD_CONST              11 ('return')
-                     488 LOAD_NAME               29 (dict)
-                     490 BUILD_TUPLE              2
-                     492 LOAD_CONST              22 (<code object context, file "/home/tanke/launchflow/launchflow/clients/python/launchflow/launchflow/cli/gen/templates/flask/flask_template.py", line 450>)
-                     494 MAKE_FUNCTION            4 (annotations)
-                     496 STORE_NAME              30 (context)
-                     498 LOAD_CONST              23 (None)
-                     500 RETURN_VALUE
+         403         512 LOAD_CONST              11 ('return')
+                     514 LOAD_NAME                8 (str)
+                     516 BUILD_TUPLE              2
+                     518 LOAD_CONST              22 (<code object docker_repository_prefix, file "/Users/calebvandyke/code/launchflow-oss/launchflow/cli/gen/templates/django/django_template.py", line 402>)
+                     520 MAKE_FUNCTION            4 (annotations)
+         
+         402         522 PRECALL                  0
+                     526 CALL                     0
+         
+         403         536 STORE_NAME              29 (docker_repository_prefix)
+         
+         408         538 LOAD_CONST              11 ('return')
+                     540 LOAD_NAME               30 (dict)
+                     542 BUILD_TUPLE              2
+                     544 LOAD_CONST              23 (<code object context, file "/Users/calebvandyke/code/launchflow-oss/launchflow/cli/gen/templates/django/django_template.py", line 408>)
+                     546 MAKE_FUNCTION            4 (annotations)
+                     548 STORE_NAME              31 (context)
+                     550 LOAD_CONST              24 (None)
+                     552 RETURN_VALUE
          consts
-            'FlaskProjectGenerator'
+            'DjangoProjectGenerator'
             'resources'
             ('aws', 'gcp')
             'cloud_provider'
             'launchflow_project_name'
             'launchflow_environment_name'
-            'flask-service'
+            'django-service'
             'launchflow_service_name'
             'python_major_version'
             'python_minor_version'
             8080
             'return'
             code
                argcount  : 1
@@ -829,156 +819,156 @@
                   0a7c036a0800000000000000009b00640b7c036a0900000000000000009b
                   00640c7c036a0a00000000000000009b00640d7c006a0400000000000000
                   009b00640e7c036a090000000000000000a00b0000000000000000000000
                   000000000000000000640f640ea6020000ab0200000000000000009b0064
                   109d0ba6010000ab01000000000000000001008c64640ba00c0000000000
                   0000000000000000000000000000007c01a6010000ab0100000000000000
                   005300
-               306           0 RESUME                   0
+               225           0 RESUME                   0
                
-               309           2 LOAD_CONST               1 ('"""\nThis is the recommended place to define all launchflow Resources, but you are free to\ndefine them anywhere in your Python project.\n\nTo create find and create all resources in your current directory, run:\n    $ launchflow create\n        - or -\n    $ lf create\n"""')
+               228           2 LOAD_CONST               1 ('"""\nThis is the recommended place to define all launchflow Resources, but you are free to\ndefine them anywhere in your Python project.\n\nTo create find and create all resources in your current directory, run:\n    $ launchflow create\n        - or -\n    $ lf create\n"""')
                
-               308           4 BUILD_LIST               1
+               227           4 BUILD_LIST               1
                              6 STORE_FAST               1 (lines)
                
-               320           8 LOAD_GLOBAL              1 (NULL + len)
+               239           8 LOAD_GLOBAL              1 (NULL + len)
                             20 LOAD_FAST                0 (self)
                             22 LOAD_ATTR                1 (resources)
                             32 PRECALL                  1
                             36 CALL                     1
                             46 LOAD_CONST               2 (0)
                             48 COMPARE_OP               2 (==)
                             54 POP_JUMP_FORWARD_IF_FALSE   109 (to 274)
                
-               321          56 LOAD_FAST                0 (self)
+               240          56 LOAD_FAST                0 (self)
                             58 LOAD_ATTR                2 (cloud_provider)
                             68 LOAD_CONST               3 ('aws')
                             70 COMPARE_OP               2 (==)
                             76 POP_JUMP_FORWARD_IF_FALSE    32 (to 142)
                
-               322          78 LOAD_FAST                1 (lines)
+               241          78 LOAD_FAST                1 (lines)
                             80 LOAD_METHOD              3 (extend)
                
-               324         102 LOAD_CONST               4 ("\n# Uncomment the following line and run `launchflow create` to create an S3 bucket.\n# s3_bucket = lf.aws.S3Bucket('")
+               243         102 LOAD_CONST               4 ("\n# Uncomment the following line and run `launchflow create` to create an S3 bucket.\n# s3_bucket = lf.aws.S3Bucket('")
                
-               326         104 LOAD_FAST                0 (self)
+               245         104 LOAD_FAST                0 (self)
                            106 LOAD_ATTR                4 (launchflow_project_name)
                
-               324         116 FORMAT_VALUE             0
+               243         116 FORMAT_VALUE             0
                            118 LOAD_CONST               5 ("-bucket')\n")
                            120 BUILD_STRING             3
                
-               323         122 BUILD_LIST               1
+               242         122 BUILD_LIST               1
                
-               322         124 PRECALL                  1
+               241         124 PRECALL                  1
                            128 CALL                     1
                            138 POP_TOP
                            140 JUMP_FORWARD           194 (to 530)
                
-               330     >>  142 LOAD_FAST                0 (self)
+               249     >>  142 LOAD_FAST                0 (self)
                            144 LOAD_ATTR                2 (cloud_provider)
                            154 LOAD_CONST               6 ('gcp')
                            156 COMPARE_OP               2 (==)
                            162 POP_JUMP_FORWARD_IF_FALSE    32 (to 228)
                
-               331         164 LOAD_FAST                1 (lines)
+               250         164 LOAD_FAST                1 (lines)
                            166 LOAD_METHOD              3 (extend)
                
-               333         188 LOAD_CONST               7 ("\n# Uncomment the following line and run `launchflow create` to create a GCS bucket.\n# gcs_bucket = lf.gcp.GCSBucket('")
+               252         188 LOAD_CONST               7 ("\n# Uncomment the following line and run `launchflow create` to create a GCS bucket.\n# gcs_bucket = lf.gcp.GCSBucket('")
                
-               335         190 LOAD_FAST                0 (self)
+               254         190 LOAD_FAST                0 (self)
                            192 LOAD_ATTR                4 (launchflow_project_name)
                
-               333         202 FORMAT_VALUE             0
+               252         202 FORMAT_VALUE             0
                            204 LOAD_CONST               5 ("-bucket')\n")
                            206 BUILD_STRING             3
                
-               332         208 BUILD_LIST               1
+               251         208 BUILD_LIST               1
                
-               331         210 PRECALL                  1
+               250         210 PRECALL                  1
                            214 CALL                     1
                            224 POP_TOP
                            226 JUMP_FORWARD           151 (to 530)
                
-               340     >>  228 LOAD_GLOBAL             11 (NULL + ValueError)
+               259     >>  228 LOAD_GLOBAL             11 (NULL + ValueError)
                            240 LOAD_CONST               8 ('Unsupported cloud provider: ')
                            242 LOAD_FAST                0 (self)
                            244 LOAD_ATTR                2 (cloud_provider)
                            254 FORMAT_VALUE             0
                            256 BUILD_STRING             2
                            258 PRECALL                  1
                            262 CALL                     1
                            272 RAISE_VARARGS            1
                
-               342     >>  274 LOAD_FAST                1 (lines)
+               261     >>  274 LOAD_FAST                1 (lines)
                            276 LOAD_METHOD              6 (append)
                            298 LOAD_CONST               9 ('import launchflow as lf\n')
                            300 PRECALL                  1
                            304 CALL                     1
                            314 POP_TOP
                
-               343         316 LOAD_FAST                0 (self)
+               262         316 LOAD_FAST                0 (self)
                            318 LOAD_ATTR                1 (resources)
                            328 GET_ITER
                        >>  330 FOR_ITER                99 (to 530)
                            332 STORE_FAST               2 (resource)
                
-               344         334 LOAD_GLOBAL             15 (NULL + get_resource_info)
+               263         334 LOAD_GLOBAL             15 (NULL + get_resource_info)
                            346 LOAD_FAST                2 (resource)
                            348 PRECALL                  1
                            352 CALL                     1
                            362 STORE_FAST               3 (resource_info)
                
-               345         364 LOAD_FAST                1 (lines)
+               264         364 LOAD_FAST                1 (lines)
                            366 LOAD_METHOD              6 (append)
                
-               346         388 LOAD_CONST              10 ('\n# Docs: ')
+               265         388 LOAD_CONST              10 ('\n# Docs: ')
                
-               347         390 LOAD_FAST                3 (resource_info)
+               266         390 LOAD_FAST                3 (resource_info)
                            392 LOAD_ATTR                8 (infra_docs_url)
                
-               346         402 FORMAT_VALUE             0
+               265         402 FORMAT_VALUE             0
                            404 LOAD_CONST              11 ('\n')
                
-               348         406 LOAD_FAST                3 (resource_info)
+               267         406 LOAD_FAST                3 (resource_info)
                            408 LOAD_ATTR                9 (infra_name)
                
-               346         418 FORMAT_VALUE             0
+               265         418 FORMAT_VALUE             0
                            420 LOAD_CONST              12 (' = ')
                
-               348         422 LOAD_FAST                3 (resource_info)
+               267         422 LOAD_FAST                3 (resource_info)
                            424 LOAD_ATTR               10 (infra_lf_class)
                
-               346         434 FORMAT_VALUE             0
+               265         434 FORMAT_VALUE             0
                            436 LOAD_CONST              13 ("('")
                
-               348         438 LOAD_FAST                0 (self)
+               267         438 LOAD_FAST                0 (self)
                            440 LOAD_ATTR                4 (launchflow_project_name)
                
-               346         450 FORMAT_VALUE             0
+               265         450 FORMAT_VALUE             0
                            452 LOAD_CONST              14 ('-')
                
-               348         454 LOAD_FAST                3 (resource_info)
+               267         454 LOAD_FAST                3 (resource_info)
                            456 LOAD_ATTR                9 (infra_name)
                            466 LOAD_METHOD             11 (replace)
                            488 LOAD_CONST              15 ('_')
                            490 LOAD_CONST              14 ('-')
                            492 PRECALL                  2
                            496 CALL                     2
                
-               346         506 FORMAT_VALUE             0
+               265         506 FORMAT_VALUE             0
                            508 LOAD_CONST              16 ("')")
                            510 BUILD_STRING            11
                
-               345         512 PRECALL                  1
+               264         512 PRECALL                  1
                            516 CALL                     1
                            526 POP_TOP
                            528 JUMP_BACKWARD          100 (to 330)
                
-               350     >>  530 LOAD_CONST              11 ('\n')
+               269     >>  530 LOAD_CONST              11 ('\n')
                            532 LOAD_METHOD             12 (join)
                            554 LOAD_FAST                1 (lines)
                            556 PRECALL                  1
                            560 CALL                     1
                            570 RETURN_VALUE
                consts
                   None
@@ -998,463 +988,484 @@
                   '-'
                   '_'
                   "')"
                names      ('len', 'resources', 'cloud_provider', 'extend', 'launchflow_project_name', 'ValueError', 'append', 'get_resource_info', 'infra_docs_url', 'infra_name', 'infra_lf_class', 'replace', 'join')
                varnames   ('self', 'lines', 'resource', 'resource_info')
                freevars   ()
                cellvars   ()
-               filename   '/home/tanke/launchflow/launchflow/clients/python/launchflow/launchflow/cli/gen/templates/flask/flask_template.py'
+               filename   '/Users/calebvandyke/code/launchflow-oss/launchflow/cli/gen/templates/django/django_template.py'
                name       'infra_dot_py'
-               firstlineno 306
+               firstlineno 225
                lnotab
                   0x020302ff040c30011601180202020cfe06ff02ff12081601180202020c
                   fe06ff02ff12092e022a0112011e01180102010cff04020cfe04020cfe04
                   020cfe040234fe06ff1205
             code
                argcount  : 1
-               nlocals   : 2
-               stacksize : 3
+               nlocals   : 5
+               stacksize : 8
                flags     : 3
                code
                   0x97007401000000000000000000007c006a010000000000000000a60100
-                  00ab01000000000000000064016b02000000007202640253007405000000
-                  000000000000007c006a010000000000000000a6010000ab010000000000
-                  0000007d017406000000000000000000007c017600730974080000000000
-                  00000000007c01760072026403530064045300
-               353           0 RESUME                   0
+                  00ab01000000000000000064016b02000000007203640267015300640267
+                  017d0167007d027c006a01000000000000000044005d2b7d037405000000
+                  000000000000007c03a6010000ab0100000000000000007d047c02a00300
+                  000000000000000000000000000000000000007c046a0400000000000000
+                  00a6010000ab01000000000000000001008c2c7401000000000000000000
+                  007c02a6010000ab01000000000000000064016b020000000072027c0153
+                  007c01a003000000000000000000000000000000000000000064036404a0
+                  050000000000000000000000000000000000000000740d00000000000000
+                  0000007c02a6010000ab010000000000000000a6010000ab010000000000
+                  0000009b009d02a6010000ab01000000000000000001007c015300
+               272           0 RESUME                   0
                
-               355           2 LOAD_GLOBAL              1 (NULL + len)
+               276           2 LOAD_GLOBAL              1 (NULL + len)
                             14 LOAD_FAST                0 (self)
                             16 LOAD_ATTR                1 (resources)
                             26 PRECALL                  1
                             30 CALL                     1
                             40 LOAD_CONST               1 (0)
                             42 COMPARE_OP               2 (==)
-                            48 POP_JUMP_FORWARD_IF_FALSE     2 (to 54)
+                            48 POP_JUMP_FORWARD_IF_FALSE     3 (to 56)
                
-               356          50 LOAD_CONST               2 ('from flask import Flask, jsonify')
-                            52 RETURN_VALUE
+               277          50 LOAD_CONST               2 ('import launchflow as lf')
+                            52 BUILD_LIST               1
+                            54 RETURN_VALUE
+               
+               278     >>   56 LOAD_CONST               2 ('import launchflow as lf')
+                            58 BUILD_LIST               1
+                            60 STORE_FAST               1 (to_return)
+               
+               279          62 BUILD_LIST               0
+                            64 STORE_FAST               2 (infra_names)
                
-               357     >>   54 LOAD_GLOBAL              5 (NULL + set)
-                            66 LOAD_FAST                0 (self)
+               281          66 LOAD_FAST                0 (self)
                             68 LOAD_ATTR                1 (resources)
-                            78 PRECALL                  1
-                            82 CALL                     1
-                            92 STORE_FAST               1 (resource_set)
-               
-               358          94 LOAD_GLOBAL              6 (CloudSQLPostgres)
-                           106 LOAD_FAST                1 (resource_set)
-                           108 CONTAINS_OP              0
-                           110 POP_JUMP_FORWARD_IF_TRUE     9 (to 130)
-                           112 LOAD_GLOBAL              8 (RDSPostgres)
-                           124 LOAD_FAST                1 (resource_set)
-                           126 CONTAINS_OP              0
-                           128 POP_JUMP_FORWARD_IF_FALSE     2 (to 134)
+                            78 GET_ITER
+                       >>   80 FOR_ITER                43 (to 168)
+                            82 STORE_FAST               3 (resource)
+               
+               282          84 LOAD_GLOBAL              5 (NULL + get_resource_info)
+                            96 LOAD_FAST                3 (resource)
+                            98 PRECALL                  1
+                           102 CALL                     1
+                           112 STORE_FAST               4 (resource_info)
+               
+               283         114 LOAD_FAST                2 (infra_names)
+                           116 LOAD_METHOD              3 (append)
+                           138 LOAD_FAST                4 (resource_info)
+                           140 LOAD_ATTR                4 (infra_name)
+                           150 PRECALL                  1
+                           154 CALL                     1
+                           164 POP_TOP
+                           166 JUMP_BACKWARD           44 (to 80)
                
-               359     >>  130 LOAD_CONST               3 ('from flask import Flask, abort, jsonify, request\nfrom flask_sqlalchemy import SQLAlchemy\nfrom sqlalchemy import select')
-                           132 RETURN_VALUE
+               285     >>  168 LOAD_GLOBAL              1 (NULL + len)
+                           180 LOAD_FAST                2 (infra_names)
+                           182 PRECALL                  1
+                           186 CALL                     1
+                           196 LOAD_CONST               1 (0)
+                           198 COMPARE_OP               2 (==)
+                           204 POP_JUMP_FORWARD_IF_FALSE     2 (to 210)
+               
+               286         206 LOAD_FAST                1 (to_return)
+                           208 RETURN_VALUE
+               
+               288     >>  210 LOAD_FAST                1 (to_return)
+                           212 LOAD_METHOD              3 (append)
+               
+               289         234 LOAD_CONST               3 ('from django_app.infra import ')
+                           236 LOAD_CONST               4 (', ')
+                           238 LOAD_METHOD              5 (join)
+                           260 LOAD_GLOBAL             13 (NULL + sorted)
+                           272 LOAD_FAST                2 (infra_names)
+                           274 PRECALL                  1
+                           278 CALL                     1
+                           288 PRECALL                  1
+                           292 CALL                     1
+                           302 FORMAT_VALUE             0
+                           304 BUILD_STRING             2
+               
+               288         306 PRECALL                  1
+                           310 CALL                     1
+                           320 POP_TOP
                
-               363     >>  134 LOAD_CONST               4 ('from flask import Flask, jsonify, request')
-                           136 RETURN_VALUE
+               291         322 LOAD_FAST                1 (to_return)
+                           324 RETURN_VALUE
                consts
                   None
                   0
-                  'from flask import Flask, jsonify'
-                  'from flask import Flask, abort, jsonify, request\nfrom flask_sqlalchemy import SQLAlchemy\nfrom sqlalchemy import select'
-                  'from flask import Flask, jsonify, request'
-               names      ('len', 'resources', 'set', 'CloudSQLPostgres', 'RDSPostgres')
-               varnames   ('self', 'resource_set')
+                  'import launchflow as lf'
+                  'from django_app.infra import '
+                  ', '
+               names      ('len', 'resources', 'get_resource_info', 'append', 'infra_name', 'join', 'sorted')
+               varnames   ('self', 'to_return', 'infra_names', 'resource', 'resource_info')
                freevars   ()
                cellvars   ()
-               filename   '/home/tanke/launchflow/launchflow/clients/python/launchflow/launchflow/cli/gen/templates/flask/flask_template.py'
-               name       'flask_imports'
-               firstlineno 353
-               lnotab 0x020230010401280124010404
+               filename   '/Users/calebvandyke/code/launchflow-oss/launchflow/cli/gen/templates/django/django_template.py'
+               name       'app_infra_imports'
+               firstlineno 272
+               lnotab 0x0204300106010601040212011e01360226010402180148ff1003
             code
                argcount  : 1
-               nlocals   : 8
-               stacksize : 8
+               nlocals   : 4
+               stacksize : 4
                flags     : 3
                code
-                  0x97007401000000000000000000007c006a010000000000000000a60100
-                  00ab01000000000000000064016b020000000072026700530067007d0167
-                  007d0267007d0367007d04740500000000000000000000a6000000ab0000
-                  000000000000007d057c006a01000000000000000044005d807d06740700
-                  0000000000000000007c06a6010000ab0100000000000000007d077c03a0
-                  0400000000000000000000000000000000000000007c076a050000000000
-                  000000a6010000ab01000000000000000001007c05a00600000000000000
-                  000000000000000000000000007c076a070000000000000000a6010000ab
-                  01000000000000000001007c04a008000000000000000000000000000000
-                  00000000007c076a090000000000000000a6010000ab0100000000000000
-                  0001007c076a0a0000000000000000811a7c02a004000000000000000000
-                  00000000000000000000007c076a0a0000000000000000a6010000ab0100
-                  0000000000000001008c817c01a008000000000000000000000000000000
-                  00000000007417000000000000000000007c02a6010000ab010000000000
-                  000000a6010000ab01000000000000000001007c01a00800000000000000
-                  000000000000000000000000007417000000000000000000007c05a60100
-                  00ab010000000000000000a6010000ab01000000000000000001007c01a0
-                  04000000000000000000000000000000000000000064026403a00c000000
-                  00000000000000000000000000000000007417000000000000000000007c
-                  03a6010000ab010000000000000000a6010000ab0100000000000000009b
-                  009d02a6010000ab01000000000000000001007c01a00800000000000000
-                  000000000000000000000000007417000000000000000000007c04a60100
-                  00ab010000000000000000a6010000ab01000000000000000001007c0153
-                  00
-               366           0 RESUME                   0
-               
-               370           2 LOAD_GLOBAL              1 (NULL + len)
-                            14 LOAD_FAST                0 (self)
-                            16 LOAD_ATTR                1 (resources)
-                            26 PRECALL                  1
-                            30 CALL                     1
-                            40 LOAD_CONST               1 (0)
-                            42 COMPARE_OP               2 (==)
-                            48 POP_JUMP_FORWARD_IF_FALSE     2 (to 54)
+                  0x970067007d017c006a00000000000000000044005d327d027403000000
+                  000000000000007c02a6010000ab0100000000000000007d037c036a0200
+                  00000000000000811a7c01a0030000000000000000000000000000000000
+                  0000007c036a020000000000000000a6010000ab01000000000000000001
+                  008c337c006a04000000000000000064016b020000000072187c01a00500
+                  0000000000000000000000000000000000000067006402a201a6010000ab
+                  01000000000000000001006e227c006a04000000000000000064036b0200
+                  00000072177c01a005000000000000000000000000000000000000000067
+                  006404a201a6010000ab01000000000000000001006405a0060000000000
+                  0000000000000000000000000000007c01a6010000ab0100000000000000
+                  005300
+               294           0 RESUME                   0
                
-               371          50 BUILD_LIST               0
-                            52 RETURN_VALUE
+               296           2 BUILD_LIST               0
+                             4 STORE_FAST               1 (lines)
                
-               372     >>   54 BUILD_LIST               0
-                            56 STORE_FAST               1 (to_return)
+               297           6 LOAD_FAST                0 (self)
+                             8 LOAD_ATTR                0 (resources)
+                            18 GET_ITER
+                       >>   20 FOR_ITER                50 (to 122)
+                            22 STORE_FAST               2 (resource)
                
-               373          58 BUILD_LIST               0
-                            60 STORE_FAST               2 (client_imports)
+               298          24 LOAD_GLOBAL              3 (NULL + get_resource_info)
+                            36 LOAD_FAST                2 (resource)
+                            38 PRECALL                  1
+                            42 CALL                     1
+                            52 STORE_FAST               3 (resource_info)
                
-               374          62 BUILD_LIST               0
-                            64 STORE_FAST               3 (infra_names)
+               299          54 LOAD_FAST                3 (resource_info)
+                            56 LOAD_ATTR                2 (django_settings)
+                            66 POP_JUMP_FORWARD_IF_NONE    26 (to 120)
                
-               375          66 BUILD_LIST               0
-                            68 STORE_FAST               4 (app_imports)
-               
-               376          70 LOAD_GLOBAL              5 (NULL + set)
-                            82 PRECALL                  0
-                            86 CALL                     0
-                            96 STORE_FAST               5 (launchflow_imports)
-               
-               377          98 LOAD_FAST                0 (self)
-                           100 LOAD_ATTR                1 (resources)
-                           110 GET_ITER
-                       >>  112 FOR_ITER               128 (to 370)
-                           114 STORE_FAST               6 (resource)
-               
-               378         116 LOAD_GLOBAL              7 (NULL + get_resource_info)
-                           128 LOAD_FAST                6 (resource)
-                           130 PRECALL                  1
-                           134 CALL                     1
-                           144 STORE_FAST               7 (resource_info)
-               
-               379         146 LOAD_FAST                3 (infra_names)
-                           148 LOAD_METHOD              4 (append)
-                           170 LOAD_FAST                7 (resource_info)
-                           172 LOAD_ATTR                5 (infra_name)
-                           182 PRECALL                  1
-                           186 CALL                     1
-                           196 POP_TOP
+               300          68 LOAD_FAST                1 (lines)
+                            70 LOAD_METHOD              3 (append)
+                            92 LOAD_FAST                3 (resource_info)
+                            94 LOAD_ATTR                2 (django_settings)
+                           104 PRECALL                  1
+                           108 CALL                     1
+                           118 POP_TOP
+                       >>  120 JUMP_BACKWARD           51 (to 20)
                
-               380         198 LOAD_FAST                5 (launchflow_imports)
-                           200 LOAD_METHOD              6 (add)
-                           222 LOAD_FAST                7 (resource_info)
-                           224 LOAD_ATTR                7 (launchflow_imports)
-                           234 PRECALL                  1
-                           238 CALL                     1
-                           248 POP_TOP
-               
-               381         250 LOAD_FAST                4 (app_imports)
-                           252 LOAD_METHOD              8 (extend)
-                           274 LOAD_FAST                7 (resource_info)
-                           276 LOAD_ATTR                9 (app_imports)
+               302     >>  122 LOAD_FAST                0 (self)
+                           124 LOAD_ATTR                4 (cloud_provider)
+                           134 LOAD_CONST               1 ('gcp')
+                           136 COMPARE_OP               2 (==)
+                           142 POP_JUMP_FORWARD_IF_FALSE    24 (to 192)
+               
+               303         144 LOAD_FAST                1 (lines)
+                           146 LOAD_METHOD              5 (extend)
+               
+               304         168 BUILD_LIST               0
+                           170 LOAD_CONST               2 (('if lf.is_deployment():', '    ALLOWED_HOSTS = ["*"]', '    # TODO(developer): Replace this with your domain', '    CSRF_TRUSTED_ORIGINS = ["https://*.run.app"]', '    SECURE_SSL_REDIRECT = True', '    SECURE_PROXY_SSL_HEADER = ("HTTP_X_FORWARDED_PROTO", "https")', 'else:', '    ALLOWED_HOSTS = ["*"]', '    DEBUG = True'))
+                           172 LIST_EXTEND              1
+               
+               303         174 PRECALL                  1
+                           178 CALL                     1
+                           188 POP_TOP
+                           190 JUMP_FORWARD            34 (to 260)
+               
+               316     >>  192 LOAD_FAST                0 (self)
+                           194 LOAD_ATTR                4 (cloud_provider)
+                           204 LOAD_CONST               3 ('aws')
+                           206 COMPARE_OP               2 (==)
+                           212 POP_JUMP_FORWARD_IF_FALSE    23 (to 260)
+               
+               317         214 LOAD_FAST                1 (lines)
+                           216 LOAD_METHOD              5 (extend)
+               
+               318         238 BUILD_LIST               0
+                           240 LOAD_CONST               4 (('if lf.is_deployment():', '    ALLOWED_HOSTS = ["*"]', "    # TODO(developer): Replace this with your domain's HTTPS URL", '    CSRF_TRUSTED_ORIGINS = ["http://*.amazonaws.com"]', 'else:', '    ALLOWED_HOSTS = ["*"]', '    DEBUG = True'))
+                           242 LIST_EXTEND              1
+               
+               317         244 PRECALL                  1
+                           248 CALL                     1
+                           258 POP_TOP
+               
+               331     >>  260 LOAD_CONST               5 ('\n')
+                           262 LOAD_METHOD              6 (join)
+                           284 LOAD_FAST                1 (lines)
                            286 PRECALL                  1
                            290 CALL                     1
-                           300 POP_TOP
+                           300 RETURN_VALUE
+               consts
+                  None
+                  'gcp'
+                  ('if lf.is_deployment():', '    ALLOWED_HOSTS = ["*"]', '    # TODO(developer): Replace this with your domain', '    CSRF_TRUSTED_ORIGINS = ["https://*.run.app"]', '    SECURE_SSL_REDIRECT = True', '    SECURE_PROXY_SSL_HEADER = ("HTTP_X_FORWARDED_PROTO", "https")', 'else:', '    ALLOWED_HOSTS = ["*"]', '    DEBUG = True')
+                  'aws'
+                  ('if lf.is_deployment():', '    ALLOWED_HOSTS = ["*"]', "    # TODO(developer): Replace this with your domain's HTTPS URL", '    CSRF_TRUSTED_ORIGINS = ["http://*.amazonaws.com"]', 'else:', '    ALLOWED_HOSTS = ["*"]', '    DEBUG = True')
+                  '\n'
+               names      ('resources', 'get_resource_info', 'django_settings', 'append', 'cloud_provider', 'extend', 'join')
+               varnames   ('self', 'lines', 'resource', 'resource_info')
+               freevars   ()
+               cellvars   ()
+               filename   '/Users/calebvandyke/code/launchflow-oss/launchflow/cli/gen/templates/django/django_template.py'
+               name       'app_django_settings'
+               firstlineno 294
+               lnotab 0x0202040112011e010e0136021601180106ff120d1601180106ff100e
+            code
+               argcount  : 1
+               nlocals   : 4
+               stacksize : 4
+               flags     : 3
+               code
+                  0x970067007d017c006a00000000000000000044005d327d027403000000
+                  000000000000007c02a6010000ab0100000000000000007d037c036a0200
+                  00000000000000811a7c01a0030000000000000000000000000000000000
+                  0000007c036a020000000000000000a6010000ab01000000000000000001
+                  008c337c015300
+               334           0 RESUME                   0
                
-               382         302 LOAD_FAST                7 (resource_info)
-                           304 LOAD_ATTR               10 (infra_import)
-                           314 POP_JUMP_FORWARD_IF_NONE    26 (to 368)
-               
-               383         316 LOAD_FAST                2 (client_imports)
-                           318 LOAD_METHOD              4 (append)
-                           340 LOAD_FAST                7 (resource_info)
-                           342 LOAD_ATTR               10 (infra_import)
-                           352 PRECALL                  1
-                           356 CALL                     1
-                           366 POP_TOP
-                       >>  368 JUMP_BACKWARD          129 (to 112)
-               
-               384     >>  370 LOAD_FAST                1 (to_return)
-                           372 LOAD_METHOD              8 (extend)
-                           394 LOAD_GLOBAL             23 (NULL + sorted)
-                           406 LOAD_FAST                2 (client_imports)
-                           408 PRECALL                  1
-                           412 CALL                     1
-                           422 PRECALL                  1
-                           426 CALL                     1
-                           436 POP_TOP
-               
-               385         438 LOAD_FAST                1 (to_return)
-                           440 LOAD_METHOD              8 (extend)
-                           462 LOAD_GLOBAL             23 (NULL + sorted)
-                           474 LOAD_FAST                5 (launchflow_imports)
-                           476 PRECALL                  1
-                           480 CALL                     1
-                           490 PRECALL                  1
-                           494 CALL                     1
-                           504 POP_TOP
-               
-               386         506 LOAD_FAST                1 (to_return)
-                           508 LOAD_METHOD              4 (append)
-                           530 LOAD_CONST               2 ('from app.infra import ')
-                           532 LOAD_CONST               3 (', ')
-                           534 LOAD_METHOD             12 (join)
-                           556 LOAD_GLOBAL             23 (NULL + sorted)
-                           568 LOAD_FAST                3 (infra_names)
-                           570 PRECALL                  1
-                           574 CALL                     1
-                           584 PRECALL                  1
-                           588 CALL                     1
-                           598 FORMAT_VALUE             0
-                           600 BUILD_STRING             2
-                           602 PRECALL                  1
-                           606 CALL                     1
-                           616 POP_TOP
-               
-               387         618 LOAD_FAST                1 (to_return)
-                           620 LOAD_METHOD              8 (extend)
-                           642 LOAD_GLOBAL             23 (NULL + sorted)
-                           654 LOAD_FAST                4 (app_imports)
-                           656 PRECALL                  1
-                           660 CALL                     1
-                           670 PRECALL                  1
-                           674 CALL                     1
-                           684 POP_TOP
+               336           2 BUILD_LIST               0
+                             4 STORE_FAST               1 (installed_apps)
                
-               388         686 LOAD_FAST                1 (to_return)
-                           688 RETURN_VALUE
+               337           6 LOAD_FAST                0 (self)
+                             8 LOAD_ATTR                0 (resources)
+                            18 GET_ITER
+                       >>   20 FOR_ITER                50 (to 122)
+                            22 STORE_FAST               2 (resource)
+               
+               338          24 LOAD_GLOBAL              3 (NULL + get_resource_info)
+                            36 LOAD_FAST                2 (resource)
+                            38 PRECALL                  1
+                            42 CALL                     1
+                            52 STORE_FAST               3 (resource_info)
+               
+               339          54 LOAD_FAST                3 (resource_info)
+                            56 LOAD_ATTR                2 (installed_app)
+                            66 POP_JUMP_FORWARD_IF_NONE    26 (to 120)
+               
+               340          68 LOAD_FAST                1 (installed_apps)
+                            70 LOAD_METHOD              3 (append)
+                            92 LOAD_FAST                3 (resource_info)
+                            94 LOAD_ATTR                2 (installed_app)
+                           104 PRECALL                  1
+                           108 CALL                     1
+                           118 POP_TOP
+                       >>  120 JUMP_BACKWARD           51 (to 20)
+               
+               341     >>  122 LOAD_FAST                1 (installed_apps)
+                           124 RETURN_VALUE
                consts
                   None
-                  0
-                  'from app.infra import '
-                  ', '
-               names      ('len', 'resources', 'set', 'get_resource_info', 'append', 'infra_name', 'add', 'launchflow_imports', 'extend', 'app_imports', 'infra_import', 'sorted', 'join')
-               varnames   ('self', 'to_return', 'client_imports', 'infra_names', 'app_imports', 'launchflow_imports', 'resource', 'resource_info')
+               names      ('resources', 'get_resource_info', 'installed_app', 'append')
+               varnames   ('self', 'installed_apps', 'resource', 'resource_info')
                freevars   ()
                cellvars   ()
-               filename   '/home/tanke/launchflow/launchflow/clients/python/launchflow/launchflow/cli/gen/templates/flask/flask_template.py'
-               name       'app_infra_imports'
-               firstlineno 366
-               lnotab
-                  0x02043001040104010401040104011c0112011e013401340134010e0136
-                  014401440170014401
+               filename   '/Users/calebvandyke/code/launchflow-oss/launchflow/cli/gen/templates/django/django_template.py'
+               name       'app_installed_apps'
+               firstlineno 334
+               lnotab 0x0202040112011e010e013601
             code
                argcount  : 1
                nlocals   : 4
                stacksize : 4
                flags     : 3
                code
                   0x970067007d017c006a00000000000000000044005d327d027403000000
                   000000000000007c02a6010000ab0100000000000000007d037c036a0200
                   00000000000000811a7c01a0030000000000000000000000000000000000
                   0000007c036a020000000000000000a6010000ab01000000000000000001
-                  008c336401a00400000000000000000000000000000000000000007c01a6
-                  010000ab0100000000000000005300
-               391           0 RESUME                   0
+                  008c337c015300
+               344           0 RESUME                   0
                
-               393           2 BUILD_LIST               0
-                             4 STORE_FAST               1 (lines)
+               346           2 BUILD_LIST               0
+                             4 STORE_FAST               1 (urls)
                
-               394           6 LOAD_FAST                0 (self)
+               347           6 LOAD_FAST                0 (self)
                              8 LOAD_ATTR                0 (resources)
                             18 GET_ITER
                        >>   20 FOR_ITER                50 (to 122)
                             22 STORE_FAST               2 (resource)
                
-               395          24 LOAD_GLOBAL              3 (NULL + get_resource_info)
+               348          24 LOAD_GLOBAL              3 (NULL + get_resource_info)
                             36 LOAD_FAST                2 (resource)
                             38 PRECALL                  1
                             42 CALL                     1
                             52 STORE_FAST               3 (resource_info)
                
-               396          54 LOAD_FAST                3 (resource_info)
-                            56 LOAD_ATTR                2 (global_setup)
+               349          54 LOAD_FAST                3 (resource_info)
+                            56 LOAD_ATTR                2 (django_test_endpoint_url)
                             66 POP_JUMP_FORWARD_IF_NONE    26 (to 120)
                
-               397          68 LOAD_FAST                1 (lines)
+               350          68 LOAD_FAST                1 (urls)
                             70 LOAD_METHOD              3 (append)
                             92 LOAD_FAST                3 (resource_info)
-                            94 LOAD_ATTR                2 (global_setup)
+                            94 LOAD_ATTR                2 (django_test_endpoint_url)
                            104 PRECALL                  1
                            108 CALL                     1
                            118 POP_TOP
                        >>  120 JUMP_BACKWARD           51 (to 20)
                
-               398     >>  122 LOAD_CONST               1 ('\n')
-                           124 LOAD_METHOD              4 (join)
-                           146 LOAD_FAST                1 (lines)
-                           148 PRECALL                  1
-                           152 CALL                     1
-                           162 RETURN_VALUE
+               351     >>  122 LOAD_FAST                1 (urls)
+                           124 RETURN_VALUE
                consts
                   None
-                  '\n'
-               names      ('resources', 'get_resource_info', 'global_setup', 'append', 'join')
-               varnames   ('self', 'lines', 'resource', 'resource_info')
+               names      ('resources', 'get_resource_info', 'django_test_endpoint_url', 'append')
+               varnames   ('self', 'urls', 'resource', 'resource_info')
                freevars   ()
                cellvars   ()
-               filename   '/home/tanke/launchflow/launchflow/clients/python/launchflow/launchflow/cli/gen/templates/flask/flask_template.py'
-               name       'app_global_setup'
-               firstlineno 391
+               filename   '/Users/calebvandyke/code/launchflow-oss/launchflow/cli/gen/templates/django/django_template.py'
+               name       'app_infra_urls'
+               firstlineno 344
                lnotab 0x0202040112011e010e013601
             code
                argcount  : 1
                nlocals   : 4
                stacksize : 4
                flags     : 3
                code
                   0x970067007d017c006a00000000000000000044005d327d027403000000
                   000000000000007c02a6010000ab0100000000000000007d037c036a0200
                   00000000000000811a7c01a0030000000000000000000000000000000000
                   0000007c036a020000000000000000a6010000ab01000000000000000001
-                  008c336401a00400000000000000000000000000000000000000007c01a6
-                  010000ab0100000000000000005300
-               401           0 RESUME                   0
+                  008c337c015300
+               354           0 RESUME                   0
                
-               403           2 BUILD_LIST               0
-                             4 STORE_FAST               1 (infra_steps)
+               356           2 BUILD_LIST               0
+                             4 STORE_FAST               1 (imports)
                
-               404           6 LOAD_FAST                0 (self)
+               357           6 LOAD_FAST                0 (self)
                              8 LOAD_ATTR                0 (resources)
                             18 GET_ITER
                        >>   20 FOR_ITER                50 (to 122)
                             22 STORE_FAST               2 (resource)
                
-               405          24 LOAD_GLOBAL              3 (NULL + get_resource_info)
+               358          24 LOAD_GLOBAL              3 (NULL + get_resource_info)
                             36 LOAD_FAST                2 (resource)
                             38 PRECALL                  1
                             42 CALL                     1
                             52 STORE_FAST               3 (resource_info)
                
-               406          54 LOAD_FAST                3 (resource_info)
-                            56 LOAD_ATTR                2 (infra_setup)
+               359          54 LOAD_FAST                3 (resource_info)
+                            56 LOAD_ATTR                2 (views_imports)
                             66 POP_JUMP_FORWARD_IF_NONE    26 (to 120)
                
-               407          68 LOAD_FAST                1 (infra_steps)
+               360          68 LOAD_FAST                1 (imports)
                             70 LOAD_METHOD              3 (append)
                             92 LOAD_FAST                3 (resource_info)
-                            94 LOAD_ATTR                2 (infra_setup)
+                            94 LOAD_ATTR                2 (views_imports)
                            104 PRECALL                  1
                            108 CALL                     1
                            118 POP_TOP
                        >>  120 JUMP_BACKWARD           51 (to 20)
                
-               408     >>  122 LOAD_CONST               1 ('\n')
-                           124 LOAD_METHOD              4 (join)
-                           146 LOAD_FAST                1 (infra_steps)
-                           148 PRECALL                  1
-                           152 CALL                     1
-                           162 RETURN_VALUE
+               361     >>  122 LOAD_FAST                1 (imports)
+                           124 RETURN_VALUE
                consts
                   None
-                  '\n'
-               names      ('resources', 'get_resource_info', 'infra_setup', 'append', 'join')
-               varnames   ('self', 'infra_steps', 'resource', 'resource_info')
+               names      ('resources', 'get_resource_info', 'views_imports', 'append')
+               varnames   ('self', 'imports', 'resource', 'resource_info')
                freevars   ()
                cellvars   ()
-               filename   '/home/tanke/launchflow/launchflow/clients/python/launchflow/launchflow/cli/gen/templates/flask/flask_template.py'
-               name       'app_infra_setup'
-               firstlineno 401
+               filename   '/Users/calebvandyke/code/launchflow-oss/launchflow/cli/gen/templates/django/django_template.py'
+               name       'app_views_imports'
+               firstlineno 354
                lnotab 0x0202040112011e010e013601
             code
                argcount  : 1
                nlocals   : 4
                stacksize : 4
                flags     : 3
                code
-                  0x970067007d017c006a00000000000000000044005d2b7d027403000000
-                  000000000000007c02a6010000ab0100000000000000007d037c01a00200
-                  000000000000000000000000000000000000007c036a0300000000000000
-                  00a6010000ab01000000000000000001008c2c7c015300
-               411           0 RESUME                   0
+                  0x970067007d017c006a00000000000000000044005d327d027403000000
+                  000000000000007c02a6010000ab0100000000000000007d037c036a0200
+                  00000000000000811a7c01a0030000000000000000000000000000000000
+                  0000007c036a020000000000000000a6010000ab01000000000000000001
+                  008c337c015300
+               364           0 RESUME                   0
                
-               413           2 BUILD_LIST               0
+               366           2 BUILD_LIST               0
                              4 STORE_FAST               1 (endpoints)
                
-               414           6 LOAD_FAST                0 (self)
+               367           6 LOAD_FAST                0 (self)
                              8 LOAD_ATTR                0 (resources)
                             18 GET_ITER
-                       >>   20 FOR_ITER                43 (to 108)
+                       >>   20 FOR_ITER                50 (to 122)
                             22 STORE_FAST               2 (resource)
                
-               415          24 LOAD_GLOBAL              3 (NULL + get_resource_info)
+               368          24 LOAD_GLOBAL              3 (NULL + get_resource_info)
                             36 LOAD_FAST                2 (resource)
                             38 PRECALL                  1
                             42 CALL                     1
                             52 STORE_FAST               3 (resource_info)
                
-               416          54 LOAD_FAST                1 (endpoints)
-                            56 LOAD_METHOD              2 (append)
-                            78 LOAD_FAST                3 (resource_info)
-                            80 LOAD_ATTR                3 (flask_test_endpoint)
-                            90 PRECALL                  1
-                            94 CALL                     1
-                           104 POP_TOP
-                           106 JUMP_BACKWARD           44 (to 20)
+               369          54 LOAD_FAST                3 (resource_info)
+                            56 LOAD_ATTR                2 (django_test_endpoint)
+                            66 POP_JUMP_FORWARD_IF_NONE    26 (to 120)
                
-               417     >>  108 LOAD_FAST                1 (endpoints)
-                           110 RETURN_VALUE
+               370          68 LOAD_FAST                1 (endpoints)
+                            70 LOAD_METHOD              3 (append)
+                            92 LOAD_FAST                3 (resource_info)
+                            94 LOAD_ATTR                2 (django_test_endpoint)
+                           104 PRECALL                  1
+                           108 CALL                     1
+                           118 POP_TOP
+                       >>  120 JUMP_BACKWARD           51 (to 20)
+               
+               371     >>  122 LOAD_FAST                1 (endpoints)
+                           124 RETURN_VALUE
                consts
                   None
-               names      ('resources', 'get_resource_info', 'append', 'flask_test_endpoint')
+               names      ('resources', 'get_resource_info', 'django_test_endpoint', 'append')
                varnames   ('self', 'endpoints', 'resource', 'resource_info')
                freevars   ()
                cellvars   ()
-               filename   '/home/tanke/launchflow/launchflow/clients/python/launchflow/launchflow/cli/gen/templates/flask/flask_template.py'
+               filename   '/Users/calebvandyke/code/launchflow-oss/launchflow/cli/gen/templates/django/django_template.py'
                name       'app_infra_endpoints'
-               firstlineno 411
-               lnotab 0x0202040112011e013601
+               firstlineno 364
+               lnotab 0x0202040112011e010e013601
             code
                argcount  : 1
                nlocals   : 4
                stacksize : 5
                flags     : 3
                code
                   0x9700740100000000000000000000a6000000ab0000000000000000007d
                   017c006a01000000000000000044005d2b7d027405000000000000000000
                   007c02a6010000ab0100000000000000007d037c01a00300000000000000
                   000000000000000000000000007c036a040000000000000000a6010000ab
                   01000000000000000001008c2c6401a00500000000000000000000000000
                   00000000000000740d000000000000000000007c01a6010000ab01000000
                   0000000000a6010000ab0100000000000000005300
-               420           0 RESUME                   0
+               374           0 RESUME                   0
                
-               422           2 LOAD_GLOBAL              1 (NULL + set)
+               376           2 LOAD_GLOBAL              1 (NULL + set)
                             14 PRECALL                  0
                             18 CALL                     0
                             28 STORE_FAST               1 (requirements)
                
-               423          30 LOAD_FAST                0 (self)
+               377          30 LOAD_FAST                0 (self)
                             32 LOAD_ATTR                1 (resources)
                             42 GET_ITER
                        >>   44 FOR_ITER                43 (to 132)
                             46 STORE_FAST               2 (resource)
                
-               424          48 LOAD_GLOBAL              5 (NULL + get_resource_info)
+               378          48 LOAD_GLOBAL              5 (NULL + get_resource_info)
                             60 LOAD_FAST                2 (resource)
                             62 PRECALL                  1
                             66 CALL                     1
                             76 STORE_FAST               3 (resource_info)
                
-               425          78 LOAD_FAST                1 (requirements)
+               379          78 LOAD_FAST                1 (requirements)
                             80 LOAD_METHOD              3 (update)
                            102 LOAD_FAST                3 (resource_info)
                            104 LOAD_ATTR                4 (requirements)
                            114 PRECALL                  1
                            118 CALL                     1
                            128 POP_TOP
                            130 JUMP_BACKWARD           44 (to 44)
                
-               426     >>  132 LOAD_CONST               1 ('\n')
+               380     >>  132 LOAD_CONST               1 ('\n')
                            134 LOAD_METHOD              5 (join)
                            156 LOAD_GLOBAL             13 (NULL + sorted)
                            168 LOAD_FAST                1 (requirements)
                            170 PRECALL                  1
                            174 CALL                     1
                            184 PRECALL                  1
                            188 CALL                     1
@@ -1462,49 +1473,49 @@
                consts
                   None
                   '\n'
                names      ('set', 'resources', 'get_resource_info', 'update', 'requirements', 'join', 'sorted')
                varnames   ('self', 'requirements', 'resource', 'resource_info')
                freevars   ()
                cellvars   ()
-               filename   '/home/tanke/launchflow/launchflow/clients/python/launchflow/launchflow/cli/gen/templates/flask/flask_template.py'
+               filename   '/Users/calebvandyke/code/launchflow-oss/launchflow/cli/gen/templates/django/django_template.py'
                name       'additional_requirements'
-               firstlineno 420
+               firstlineno 374
                lnotab 0x02021c0112011e013601
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 4
                flags     : 3
                code
                   0x97007c006a00000000000000000064016b02000000007202640253007c
                   006a00000000000000000064036b02000000007202640453007403000000
                   0000000000000064057c006a0000000000000000009b009d02a6010000ab
                   0100000000000000008201
-               429           0 RESUME                   0
+               383           0 RESUME                   0
                
-               431           2 LOAD_FAST                0 (self)
+               385           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (cloud_provider)
                             14 LOAD_CONST               1 ('aws')
                             16 COMPARE_OP               2 (==)
                             22 POP_JUMP_FORWARD_IF_FALSE     2 (to 28)
                
-               432          24 LOAD_CONST               2 ('aws_ecs_fargate')
+               386          24 LOAD_CONST               2 ('aws_ecs_fargate')
                             26 RETURN_VALUE
                
-               433     >>   28 LOAD_FAST                0 (self)
+               387     >>   28 LOAD_FAST                0 (self)
                             30 LOAD_ATTR                0 (cloud_provider)
                             40 LOAD_CONST               3 ('gcp')
                             42 COMPARE_OP               2 (==)
                             48 POP_JUMP_FORWARD_IF_FALSE     2 (to 54)
                
-               434          50 LOAD_CONST               4 ('gcp_cloud_run')
+               388          50 LOAD_CONST               4 ('gcp_cloud_run')
                             52 RETURN_VALUE
                
-               435     >>   54 LOAD_GLOBAL              3 (NULL + ValueError)
+               389     >>   54 LOAD_GLOBAL              3 (NULL + ValueError)
                             66 LOAD_CONST               5 ('Unsupported cloud provider: ')
                             68 LOAD_FAST                0 (self)
                             70 LOAD_ATTR                0 (cloud_provider)
                             80 FORMAT_VALUE             0
                             82 BUILD_STRING             2
                             84 PRECALL                  1
                             88 CALL                     1
@@ -1516,330 +1527,357 @@
                   'gcp'
                   'gcp_cloud_run'
                   'Unsupported cloud provider: '
                names      ('cloud_provider', 'ValueError')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   '/home/tanke/launchflow/launchflow/clients/python/launchflow/launchflow/cli/gen/templates/flask/flask_template.py'
+               filename   '/Users/calebvandyke/code/launchflow-oss/launchflow/cli/gen/templates/django/django_template.py'
                name       'launchflow_service_product'
-               firstlineno 429
+               firstlineno 383
                lnotab 0x02021601040116010401
             code
                argcount  : 1
-               nlocals   : 1
+               nlocals   : 3
                stacksize : 3
                flags     : 3
                code
-                  0x9700740000000000000000000000640184007c006a0100000000000000
-                  004400a6000000ab00000000000000000076007318740400000000000000
-                  000000640284007c006a0100000000000000004400a6000000ab00000000
-                  0000000000760072026403530064045300
-               437           0 RESUME                   0
-               
-               438           2 LOAD_GLOBAL              0 (CloudSQLPostgres)
-                            14 LOAD_CONST               1 (<code object <listcomp>, file "/home/tanke/launchflow/launchflow/clients/python/launchflow/launchflow/cli/gen/templates/flask/flask_template.py", line 438>)
-                            16 MAKE_FUNCTION            0
-               
-               439          18 LOAD_FAST                0 (self)
-                            20 LOAD_ATTR                1 (resources)
-               
-               438          30 GET_ITER
-                            32 PRECALL                  0
-                            36 CALL                     0
-                            46 CONTAINS_OP              0
-                            48 POP_JUMP_FORWARD_IF_TRUE    24 (to 98)
-               
-               440          50 LOAD_GLOBAL              4 (RDSPostgres)
-                            62 LOAD_CONST               2 (<code object <listcomp>, file "/home/tanke/launchflow/launchflow/clients/python/launchflow/launchflow/cli/gen/templates/flask/flask_template.py", line 440>)
-                            64 MAKE_FUNCTION            0
-                            66 LOAD_FAST                0 (self)
-                            68 LOAD_ATTR                1 (resources)
-                            78 GET_ITER
-                            80 PRECALL                  0
-                            84 CALL                     0
-                            94 CONTAINS_OP              0
-                            96 POP_JUMP_FORWARD_IF_FALSE     2 (to 102)
+                  0x970064017d0164027d02740000000000000000000000640384007c006a
+                  0100000000000000004400a6000000ab0000000000000000007600731874
+                  0400000000000000000000640484007c006a0100000000000000004400a6
+                  000000ab0000000000000000007600720264057d027c017c0266025300
+               391           0 RESUME                   0
                
-               441     >>   98 LOAD_CONST               3 ('launchflow.cli.gen.templates.flask._postgres_template')
-                           100 RETURN_VALUE
+               392           2 LOAD_CONST               1 ('launchflow.cli.gen.templates.django')
+                             4 STORE_FAST               1 (template_dir)
                
-               442     >>  102 LOAD_CONST               4 ('launchflow.cli.gen.templates.flask._simple_template')
-                           104 RETURN_VALUE
+               393           6 LOAD_CONST               2 ('_simple_template')
+                             8 STORE_FAST               2 (template_name)
+               
+               395          10 LOAD_GLOBAL              0 (CloudSQLPostgres)
+                            22 LOAD_CONST               3 (<code object <listcomp>, file "/Users/calebvandyke/code/launchflow-oss/launchflow/cli/gen/templates/django/django_template.py", line 395>)
+                            24 MAKE_FUNCTION            0
+               
+               396          26 LOAD_FAST                0 (self)
+                            28 LOAD_ATTR                1 (resources)
+               
+               395          38 GET_ITER
+                            40 PRECALL                  0
+                            44 CALL                     0
+                            54 CONTAINS_OP              0
+                            56 POP_JUMP_FORWARD_IF_TRUE    24 (to 106)
+               
+               397          58 LOAD_GLOBAL              4 (RDSPostgres)
+                            70 LOAD_CONST               4 (<code object <listcomp>, file "/Users/calebvandyke/code/launchflow-oss/launchflow/cli/gen/templates/django/django_template.py", line 397>)
+                            72 MAKE_FUNCTION            0
+                            74 LOAD_FAST                0 (self)
+                            76 LOAD_ATTR                1 (resources)
+                            86 GET_ITER
+                            88 PRECALL                  0
+                            92 CALL                     0
+                           102 CONTAINS_OP              0
+                           104 POP_JUMP_FORWARD_IF_FALSE     2 (to 110)
+               
+               398     >>  106 LOAD_CONST               5 ('_postgres_template')
+                           108 STORE_FAST               2 (template_name)
+               
+               400     >>  110 LOAD_FAST                1 (template_dir)
+                           112 LOAD_FAST                2 (template_name)
+                           114 BUILD_TUPLE              2
+                           116 RETURN_VALUE
                consts
                   None
+                  'launchflow.cli.gen.templates.django'
+                  '_simple_template'
                   code
                      argcount  : 1
                      nlocals   : 2
                      stacksize : 3
                      flags     : 19
                      code 0x970067007c005d047d017c0191028c055300
-                     438           0 RESUME                   0
+                     395           0 RESUME                   0
                                    2 BUILD_LIST               0
                                    4 LOAD_FAST                0 (.0)
                              >>    6 FOR_ITER                 4 (to 16)
                      
-                     439           8 STORE_FAST               1 (resource)
+                     396           8 STORE_FAST               1 (resource)
                                   10 LOAD_FAST                1 (resource)
                      
-                     438          12 LIST_APPEND              2
+                     395          12 LIST_APPEND              2
                                   14 JUMP_BACKWARD            5 (to 6)
                              >>   16 RETURN_VALUE
                      consts
                      names      ()
                      varnames   ('.0', 'resource')
                      freevars   ()
                      cellvars   ()
-                     filename   '/home/tanke/launchflow/launchflow/clients/python/launchflow/launchflow/cli/gen/templates/flask/flask_template.py'
+                     filename   '/Users/calebvandyke/code/launchflow-oss/launchflow/cli/gen/templates/django/django_template.py'
                      name       '<listcomp>'
-                     firstlineno 438
+                     firstlineno 395
                      lnotab 0x080104ff
                   code
                      argcount  : 1
                      nlocals   : 2
                      stacksize : 3
                      flags     : 19
                      code 0x970067007c005d047d017c0191028c055300
-                     440           0 RESUME                   0
+                     397           0 RESUME                   0
                                    2 BUILD_LIST               0
                                    4 LOAD_FAST                0 (.0)
                              >>    6 FOR_ITER                 4 (to 16)
                                    8 STORE_FAST               1 (resource)
                                   10 LOAD_FAST                1 (resource)
                                   12 LIST_APPEND              2
                                   14 JUMP_BACKWARD            5 (to 6)
                              >>   16 RETURN_VALUE
                      consts
                      names      ()
                      varnames   ('.0', 'resource')
                      freevars   ()
                      cellvars   ()
-                     filename   '/home/tanke/launchflow/launchflow/clients/python/launchflow/launchflow/cli/gen/templates/flask/flask_template.py'
+                     filename   '/Users/calebvandyke/code/launchflow-oss/launchflow/cli/gen/templates/django/django_template.py'
                      name       '<listcomp>'
-                     firstlineno 440
+                     firstlineno 397
                      lnotab 0x
-                  'launchflow.cli.gen.templates.flask._postgres_template'
-                  'launchflow.cli.gen.templates.flask._simple_template'
+                  '_postgres_template'
                names      ('CloudSQLPostgres', 'resources', 'RDSPostgres')
-               varnames   ('self',)
+               varnames   ('self', 'template_dir', 'template_name')
                freevars   ()
                cellvars   ()
-               filename   '/home/tanke/launchflow/launchflow/clients/python/launchflow/launchflow/cli/gen/templates/flask/flask_template.py'
-               name       'template_directory'
-               firstlineno 437
-               lnotab 0x020110010cff140230010401
+               filename   '/Users/calebvandyke/code/launchflow-oss/launchflow/cli/gen/templates/django/django_template.py'
+               name       'template_path_info'
+               firstlineno 391
+               lnotab 0x02010401040210010cff140230010402
             code
                argcount  : 1
                nlocals   : 1
                stacksize : 2
                flags     : 3
                code
                   0x97007c006a00000000000000000064016b020000000072026402530064
                   035300
-               444           0 RESUME                   0
+               402           0 RESUME                   0
                
-               446           2 LOAD_FAST                0 (self)
+               404           2 LOAD_FAST                0 (self)
                              4 LOAD_ATTR                0 (cloud_provider)
                             14 LOAD_CONST               1 ('aws')
                             16 COMPARE_OP               2 (==)
                             22 POP_JUMP_FORWARD_IF_FALSE     2 (to 28)
                
-               447          24 LOAD_CONST               2 ('public.ecr.aws/docker/library/')
+               405          24 LOAD_CONST               2 ('public.ecr.aws/docker/library/')
                             26 RETURN_VALUE
                
-               448     >>   28 LOAD_CONST               3 ('')
+               406     >>   28 LOAD_CONST               3 ('')
                             30 RETURN_VALUE
                consts
                   None
                   'aws'
                   'public.ecr.aws/docker/library/'
                   ''
                names      ('cloud_provider',)
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   '/home/tanke/launchflow/launchflow/clients/python/launchflow/launchflow/cli/gen/templates/flask/flask_template.py'
+               filename   '/Users/calebvandyke/code/launchflow-oss/launchflow/cli/gen/templates/django/django_template.py'
                name       'docker_repository_prefix'
-               firstlineno 444
+               firstlineno 402
                lnotab 0x020216010401
             code
                argcount  : 1
                nlocals   : 1
-               stacksize : 3
+               stacksize : 5
                flags     : 3
                code
                   0x9700690064017c006a000000000000000000930164027c006a01000000
                   0000000000930164037c006a020000000000000000930164047c006a0300
                   00000000000000930164057c006a040000000000000000930164067c006a
                   050000000000000000930164077c006a060000000000000000930164087c
                   006a070000000000000000930164097c006a080000000000000000930164
                   0a7c006a0900000000000000009301640b7c006a0a000000000000000093
                   01640c7c006a0b00000000000000009301640d7c006a0c00000000000000
-                  009301640e7c006a0d00000000000000009301640f7c006a0e0000000000
-                  000000930164107c006a0f000000000000000093015300
-               450           0 RESUME                   0
+                  009301640e7c006a0d00000000000000009301640f741c00000000000000
+                  0000006a0e0000000000000000a00f000000000000000000000000000000
+                  0000000000a6000000ab000000000000000000a010000000000000000000
+                  00000000000000000000006410a6010000ab010000000000000000930164
+                  117c006a110000000000000000930164127c006a12000000000000000093
+                  0164137c006a1300000000000000006901a5015300
+               408           0 RESUME                   0
                
-               451           2 BUILD_MAP                0
+               409           2 BUILD_MAP                0
                
-               453           4 LOAD_CONST               1 ('cloud_provider')
+               411           4 LOAD_CONST               1 ('cloud_provider')
                              6 LOAD_FAST                0 (self)
                              8 LOAD_ATTR                0 (cloud_provider)
                
-               451          18 MAP_ADD                  1
+               409          18 MAP_ADD                  1
                
-               454          20 LOAD_CONST               2 ('additional_requirements')
+               412          20 LOAD_CONST               2 ('additional_requirements')
                             22 LOAD_FAST                0 (self)
                             24 LOAD_ATTR                1 (additional_requirements)
                
-               451          34 MAP_ADD                  1
+               409          34 MAP_ADD                  1
                
-               456          36 LOAD_CONST               3 ('launchflow_project_name')
+               414          36 LOAD_CONST               3 ('launchflow_project_name')
                             38 LOAD_FAST                0 (self)
                             40 LOAD_ATTR                2 (launchflow_project_name)
                
-               451          50 MAP_ADD                  1
+               409          50 MAP_ADD                  1
                
-               457          52 LOAD_CONST               4 ('launchflow_environment_name')
+               415          52 LOAD_CONST               4 ('launchflow_environment_name')
                             54 LOAD_FAST                0 (self)
                             56 LOAD_ATTR                3 (launchflow_environment_name)
                
-               451          66 MAP_ADD                  1
+               409          66 MAP_ADD                  1
                
-               458          68 LOAD_CONST               5 ('launchflow_service_name')
+               416          68 LOAD_CONST               5 ('launchflow_service_name')
                             70 LOAD_FAST                0 (self)
                             72 LOAD_ATTR                4 (launchflow_service_name)
                
-               451          82 MAP_ADD                  1
+               409          82 MAP_ADD                  1
                
-               459          84 LOAD_CONST               6 ('launchflow_service_product')
+               417          84 LOAD_CONST               6 ('launchflow_service_product')
                             86 LOAD_FAST                0 (self)
                             88 LOAD_ATTR                5 (launchflow_service_product)
                
-               451          98 MAP_ADD                  1
+               409          98 MAP_ADD                  1
                
-               461         100 LOAD_CONST               7 ('docker_repository_prefix')
+               419         100 LOAD_CONST               7 ('docker_repository_prefix')
                            102 LOAD_FAST                0 (self)
                            104 LOAD_ATTR                6 (docker_repository_prefix)
                
-               451         114 MAP_ADD                  1
+               409         114 MAP_ADD                  1
                
-               462         116 LOAD_CONST               8 ('python_major_version')
+               420         116 LOAD_CONST               8 ('python_major_version')
                            118 LOAD_FAST                0 (self)
                            120 LOAD_ATTR                7 (python_major_version)
                
-               451         130 MAP_ADD                  1
+               409         130 MAP_ADD                  1
                
-               463         132 LOAD_CONST               9 ('python_minor_version')
+               421         132 LOAD_CONST               9 ('python_minor_version')
                            134 LOAD_FAST                0 (self)
                            136 LOAD_ATTR                8 (python_minor_version)
                
-               451         146 MAP_ADD                  1
+               409         146 MAP_ADD                  1
                
-               464         148 LOAD_CONST              10 ('port')
+               422         148 LOAD_CONST              10 ('port')
                            150 LOAD_FAST                0 (self)
                            152 LOAD_ATTR                9 (port)
                
-               451         162 MAP_ADD                  1
+               409         162 MAP_ADD                  1
                
-               466         164 LOAD_CONST              11 ('infra_dot_py')
+               424         164 LOAD_CONST              11 ('infra_dot_py')
                            166 LOAD_FAST                0 (self)
                            168 LOAD_ATTR               10 (infra_dot_py)
                
-               451         178 MAP_ADD                  1
+               409         178 MAP_ADD                  1
                
-               468         180 LOAD_CONST              12 ('flask_imports')
+               426         180 LOAD_CONST              12 ('app_infra_imports')
                            182 LOAD_FAST                0 (self)
-                           184 LOAD_ATTR               11 (flask_imports)
+                           184 LOAD_ATTR               11 (app_infra_imports)
                
-               451         194 MAP_ADD                  1
+               409         194 MAP_ADD                  1
                
-               469         196 LOAD_CONST              13 ('app_infra_imports')
+               427         196 LOAD_CONST              13 ('app_django_settings')
                            198 LOAD_FAST                0 (self)
-                           200 LOAD_ATTR               12 (app_infra_imports)
+                           200 LOAD_ATTR               12 (app_django_settings)
                
-               451         210 MAP_ADD                  1
+               409         210 MAP_ADD                  1
                
-               470         212 LOAD_CONST              14 ('app_global_setup')
+               428         212 LOAD_CONST              14 ('app_installed_apps')
                            214 LOAD_FAST                0 (self)
-                           216 LOAD_ATTR               13 (app_global_setup)
-               
-               451         226 MAP_ADD                  1
-               
-               471         228 LOAD_CONST              15 ('app_infra_setup')
-                           230 LOAD_FAST                0 (self)
-                           232 LOAD_ATTR               14 (app_infra_setup)
-               
-               451         242 MAP_ADD                  1
+                           216 LOAD_ATTR               13 (app_installed_apps)
                
-               472         244 LOAD_CONST              16 ('app_infra_endpoints')
-                           246 LOAD_FAST                0 (self)
-                           248 LOAD_ATTR               15 (app_infra_endpoints)
+               409         226 MAP_ADD                  1
                
-               451         258 MAP_ADD                  1
-                           260 RETURN_VALUE
+               430         228 LOAD_CONST              15 ('current_timestamp')
+                           230 LOAD_GLOBAL             28 (datetime)
+                           242 LOAD_ATTR               14 (datetime)
+                           252 LOAD_METHOD             15 (now)
+                           274 PRECALL                  0
+                           278 CALL                     0
+                           288 LOAD_METHOD             16 (strftime)
+                           310 LOAD_CONST              16 ('%Y-%m-%d %H:%M')
+                           312 PRECALL                  1
+                           316 CALL                     1
+               
+               409         326 MAP_ADD                  1
+               
+               432         328 LOAD_CONST              17 ('app_infra_urls')
+                           330 LOAD_FAST                0 (self)
+                           332 LOAD_ATTR               17 (app_infra_urls)
+               
+               409         342 MAP_ADD                  1
+               
+               434         344 LOAD_CONST              18 ('app_infra_endpoints')
+                           346 LOAD_FAST                0 (self)
+                           348 LOAD_ATTR               18 (app_infra_endpoints)
+               
+               409         358 MAP_ADD                  1
+               
+               435         360 LOAD_CONST              19 ('app_views_imports')
+                           362 LOAD_FAST                0 (self)
+                           364 LOAD_ATTR               19 (app_views_imports)
+               
+               409         374 BUILD_MAP                1
+                           376 DICT_UPDATE              1
+                           378 RETURN_VALUE
                consts
                   None
                   'cloud_provider'
                   'additional_requirements'
                   'launchflow_project_name'
                   'launchflow_environment_name'
                   'launchflow_service_name'
                   'launchflow_service_product'
                   'docker_repository_prefix'
                   'python_major_version'
                   'python_minor_version'
                   'port'
                   'infra_dot_py'
-                  'flask_imports'
                   'app_infra_imports'
-                  'app_global_setup'
-                  'app_infra_setup'
+                  'app_django_settings'
+                  'app_installed_apps'
+                  'current_timestamp'
+                  '%Y-%m-%d %H:%M'
+                  'app_infra_urls'
                   'app_infra_endpoints'
-               names      ('cloud_provider', 'additional_requirements', 'launchflow_project_name', 'launchflow_environment_name', 'launchflow_service_name', 'launchflow_service_product', 'docker_repository_prefix', 'python_major_version', 'python_minor_version', 'port', 'infra_dot_py', 'flask_imports', 'app_infra_imports', 'app_global_setup', 'app_infra_setup', 'app_infra_endpoints')
+                  'app_views_imports'
+               names      ('cloud_provider', 'additional_requirements', 'launchflow_project_name', 'launchflow_environment_name', 'launchflow_service_name', 'launchflow_service_product', 'docker_repository_prefix', 'python_major_version', 'python_minor_version', 'port', 'infra_dot_py', 'app_infra_imports', 'app_django_settings', 'app_installed_apps', 'datetime', 'now', 'strftime', 'app_infra_urls', 'app_infra_endpoints', 'app_views_imports')
                varnames   ('self',)
                freevars   ()
                cellvars   ()
-               filename   '/home/tanke/launchflow/launchflow/clients/python/launchflow/launchflow/cli/gen/templates/flask/flask_template.py'
+               filename   '/Users/calebvandyke/code/launchflow-oss/launchflow/cli/gen/templates/django/django_template.py'
                name       'context'
-               firstlineno 450
+               firstlineno 408
                lnotab
                   0x020102020efe02030efd02050efb02060efa02070ef902080ef8020a0e
                   f6020b0ef5020c0ef4020d0ef3020f0ef102110eef02120eee02130eed02
-                  140eec02150eeb
+                  1562eb02170ee902190ee7021a0ee6
             None
-         names      ('__name__', '__module__', '__qualname__', 'List', 'Type', 'Resource', '__annotations__', 'Literal', 'str', 'launchflow_service_name', 'sys', 'version_info', 'major', 'python_major_version', 'int', 'minor', 'python_minor_version', 'port', 'property', 'infra_dot_py', 'flask_imports', 'app_infra_imports', 'app_global_setup', 'app_infra_setup', 'app_infra_endpoints', 'additional_requirements', 'launchflow_service_product', 'template_directory', 'docker_repository_prefix', 'dict', 'context')
+         names      ('__name__', '__module__', '__qualname__', 'List', 'Type', 'Resource', '__annotations__', 'Literal', 'str', 'launchflow_service_name', 'sys', 'version_info', 'major', 'python_major_version', 'int', 'minor', 'python_minor_version', 'port', 'property', 'infra_dot_py', 'app_infra_imports', 'app_django_settings', 'app_installed_apps', 'app_infra_urls', 'app_views_imports', 'app_infra_endpoints', 'additional_requirements', 'launchflow_service_product', 'template_path_info', 'docker_repository_prefix', 'dict', 'context')
          varnames   ()
          freevars   ()
          cellvars   ()
-         filename   '/home/tanke/launchflow/launchflow/clients/python/launchflow/launchflow/cli/gen/templates/flask/flask_template.py'
-         name       'FlaskProjectGenerator'
-         firstlineno 291
+         filename   '/Users/calebvandyke/code/launchflow-oss/launchflow/cli/gen/templates/django/django_template.py'
+         name       'DjangoProjectGenerator'
+         firstlineno 210
          lnotab
-            0x0c02220216020a010a010e0222012201040302010aff0e01022e02010a
-            ff0e01020c020116ff0e01021802010aff0e010209020116ff0e01020902
-            0116ff0e010208020116ff0e01020802010aff0e0102070c0702010aff0e
-            010205
-      'FlaskProjectGenerator'
-      '__main__'
-      'gcp'
-      '-examples'
-      'dev'
-      'flask-service'
-      ('resources', 'cloud_provider', 'launchflow_project_name', 'launchflow_environment_name', 'launchflow_service_name')
-      '/tmp/launchflow'
-      ('destination_path',)
-   names      ('sys', 'dataclasses', 'dataclass', 'typing', 'List', 'Literal', 'Optional', 'Type', 'launchflow.aws.rds', 'RDSPostgres', 'launchflow.aws.s3', 'S3Bucket', 'launchflow.cli.gen.template', 'ProjectGenerator', 'launchflow.gcp.cloudsql', 'CloudSQLPostgres', 'launchflow.gcp.compute_engine', 'ComputeEngineRedis', 'launchflow.gcp.gcs', 'GCSBucket', 'launchflow.gcp.memorystore', 'MemorystoreRedis', 'launchflow', 'Resource', 'ResourceInfo', 'resource_type_to_resource_info_kwargs', 'get_resource_info', 'FlaskProjectGenerator', '__name__', 'cloud_provider', 'generator', 'generate_project')
+            0x0c02220216020a010a010e0222012201040302010aff0e01022e020116
+            ff0e01021502010aff0e010227020116ff0e010209020116ff0e01020902
+            0116ff0e010209020116ff0e010209020116ff0e01020802010aff0e0102
+            070c0b02010aff0e010205
+      'DjangoProjectGenerator'
+   names      ('datetime', 'sys', 'dataclasses', 'dataclass', 'typing', 'List', 'Literal', 'Optional', 'Type', 'launchflow', 'Resource', 'launchflow.aws.elasticache', 'ElasticacheRedis', 'launchflow.aws.rds', 'RDSPostgres', 'launchflow.aws.s3', 'S3Bucket', 'launchflow.cli.gen.template', 'ProjectGenerator', 'launchflow.gcp.cloudsql', 'CloudSQLPostgres', 'launchflow.gcp.compute_engine', 'ComputeEngineRedis', 'launchflow.gcp.gcs', 'GCSBucket', 'launchflow.gcp.memorystore', 'MemorystoreRedis', 'ResourceInfo', 'resource_type_to_resource_info_kwargs', 'get_resource_info', 'DjangoProjectGenerator')
    varnames   ()
    freevars   ()
    cellvars   ()
-   filename   '/home/tanke/launchflow/launchflow/clients/python/launchflow/launchflow/cli/gen/templates/flask/flask_template.py'
+   filename   '/Users/calebvandyke/code/launchflow-oss/launchflow/cli/gen/templates/django/django_template.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff020108010c0118020c010c010c010c010c010c010c020c03020118
-      ff0e01020f020102010201020102010201020102010201020c04eb041802
-      0102010201020102010201020102010201020c04eb041802010201020102
-      0102010201020102010201020b02ec041702010201020102010201020102
-      02020102fe02040209023606b6044d020102010201020102010201020102
-      010201020b02ec04170201020102010201020102010202020102fe020402
-      09023606b6048000d3047f007d1c0902011aff0e01027f00390c01040104
-      020201020102fd020702010801020102f5120d30f1
+      0x00ff0201080108010c0118020c010c010c010c010c010c010c010c010c
+      03020118ff0e01020e020102010201020102040201020a0201040102eb04
+      18020102010201020102040201020a0201040102eb041802010201020102
+      01020b0201020c0201040102e20421020102010201020102040201020102
+      01040102f4040f02010201020102010201020a020c0201040102e3042002
+      0102010201020102040201020a0201040102eb0418020102010201020102
+      01020402010201040102f4048000e6047f002c1c0902011aff0e01
```

### Comparing `launchflow-0.3.9.dev8/launchflow/cli/gen/templates/flask/_postgres_template/Dockerfile.jinja` & `launchflow-0.4.0.dev0/launchflow/cli/gen/templates/flask/_postgres_template/Dockerfile.jinja`

 * *Files 5% similar despite different names*

```diff
@@ -33,14 +33,13 @@
 # Copy installed dependencies from the builder stage
 COPY --from=builder /install /usr/local/lib/python{{ python_major_version }}.{{ python_minor_version }}/site-packages
 ENV PATH="${PATH}:/usr/local/lib/python{{ python_major_version }}.{{ python_minor_version }}/site-packages/bin"
 
 # Set the working directory and copy only the necessary application files
 WORKDIR /code
 COPY --chown=appuser:appuser ./app /code/app
-COPY --chown=appuser:appuser ./launchflow.yaml /code/launchflow.yaml
 
 # Expose the port the app runs on
 EXPOSE $PORT
 
 # Start the application
 CMD exec gunicorn --bind :$PORT --workers 1 --threads 8 --timeout 0 app.main:app
```

### Comparing `launchflow-0.3.9.dev8/launchflow/cli/gen/templates/flask/_postgres_template/README.md.jinja` & `launchflow-0.4.0.dev0/launchflow/cli/gen/templates/flask/_postgres_template/README.md.jinja`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -81,8 +81,8 @@
 
 Automatically <strong>delete</strong> all infrastructure associated with your application.
 
 ```bash
 launchflow destroy
 ```
 
-Learn how this command works in the [LaunchFlow Docs](https://docs.launchflow.com/reference/cli#launchflow-destroy).
+Learn how this command works in the [LaunchFlow Docs](https://docs.launchflow.com/reference/cli#launchflow-destroy).
```

### Comparing `launchflow-0.3.9.dev8/launchflow/cli/gen/templates/flask/_postgres_template/app/schemas.py.jinja` & `launchflow-0.4.0.dev0/launchflow/cli/gen/templates/flask/_postgres_template/app/schemas.py.jinja`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev8/launchflow/cli/gen/templates/flask/_simple_template/Dockerfile.jinja` & `launchflow-0.4.0.dev0/launchflow/cli/gen/templates/flask/_simple_template/Dockerfile.jinja`

 * *Files 5% similar despite different names*

```diff
@@ -33,14 +33,13 @@
 # Copy installed dependencies from the builder stage
 COPY --from=builder /install /usr/local/lib/python{{ python_major_version }}.{{ python_minor_version }}/site-packages
 ENV PATH="${PATH}:/usr/local/lib/python{{ python_major_version }}.{{ python_minor_version }}/site-packages/bin"
 
 # Set the working directory and copy only the necessary application files
 WORKDIR /code
 COPY --chown=appuser:appuser ./app /code/app
-COPY --chown=appuser:appuser ./launchflow.yaml /code/launchflow.yaml
 
 # Expose the port the app runs on
 EXPOSE $PORT
 
 # Start the application
 CMD exec gunicorn --bind :$PORT --workers 1 --threads 8 --timeout 0 app.main:app
```

### Comparing `launchflow-0.3.9.dev8/launchflow/cli/gen/templates/flask/_simple_template/README.md.jinja` & `launchflow-0.4.0.dev0/launchflow/cli/gen/templates/flask/_simple_template/README.md.jinja`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -81,8 +81,8 @@
 
 Automatically <strong>delete</strong> all infrastructure associated with your application.
 
 ```bash
 launchflow destroy
 ```
 
-Learn how this command works in the [LaunchFlow Docs](https://docs.launchflow.com/reference/cli#launchflow-destroy).
+Learn how this command works in the [LaunchFlow Docs](https://docs.launchflow.com/reference/cli#launchflow-destroy).
```

### Comparing `launchflow-0.3.9.dev8/launchflow/cli/gen/templates/flask/flask_template.py` & `launchflow-0.4.0.dev0/launchflow/cli/gen/templates/flask/flask_template.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import sys
 from dataclasses import dataclass
 from typing import List, Literal, Optional, Type
 
+from launchflow import Resource
+from launchflow.aws.elasticache import ElasticacheRedis
 from launchflow.aws.rds import RDSPostgres
 from launchflow.aws.s3 import S3Bucket
 from launchflow.cli.gen.template import ProjectGenerator
 from launchflow.gcp.cloudsql import CloudSQLPostgres
 from launchflow.gcp.compute_engine import ComputeEngineRedis
 from launchflow.gcp.gcs import GCSBucket
 from launchflow.gcp.memorystore import MemorystoreRedis
 
-from launchflow import Resource
-
 
 @dataclass
 class ResourceInfo:
     infra_docs_url: str
     infra_name: str
     infra_lf_class: str
     launchflow_imports: str
@@ -26,15 +26,15 @@
     flask_test_endpoint: str
     requirements: List[str]
 
 
 resource_type_to_resource_info_kwargs = {
     # GCP Compute Engine Redis
     ComputeEngineRedis: {
-        "infra_docs_url": "https://docs.launchflow.com/reference/gcp-resources/compute-engine",
+        "infra_docs_url": "https://docs.launchflow.com/reference/gcp-resources/compute-engine#compute-engine-redis",
         "infra_name": "redis_vm",
         "infra_lf_class": "lf.gcp.ComputeEngineRedis",
         "launchflow_imports": "",
         "infra_import": None,
         "global_setup": None,
         "infra_setup": "# Connect to the Redis instance\nredis_client = redis_vm.redis()\n",
         "app_imports": [],
@@ -50,21 +50,21 @@
     value = redis_client.get(key)
     return jsonify({"message": f"Set {key} to {value}"})
 """,
         "requirements": ["redis>=4.2.0"],
     },
     # GCP Memorystore Redis
     MemorystoreRedis: {
-        "infra_docs_url": "https://docs.launchflow.com/reference/gcp-resources/memorystore-redis",
-        "infra_name": "redis_cluster",
+        "infra_docs_url": "https://docs.launchflow.com/reference/gcp-resources/memorystore",
+        "infra_name": "memorystore",
         "infra_lf_class": "lf.gcp.MemorystoreRedis",
         "launchflow_imports": "",
         "infra_import": None,
         "global_setup": None,
-        "infra_setup": "# Connect to the Redis instance\nredis_client = redis_vm.redis()\n",
+        "infra_setup": "# Connect to the Redis instance\nredis_client = memorystore.redis()\n",
         "app_imports": [],
         "flask_test_endpoint": """
 # NOTE: This should normally use a POST request since it's modifying state, but we're
 # using GET so you can easily test it in your browser.
 @app.get("/test_redis/<key>")
 def test_redis(key: str):
     # Write to Redis
@@ -195,17 +195,41 @@
     s3_bucket.upload_from_string("Hello, World!", object_name)
     # Immediately read from S3 to verify the write
     s3_bucket.download_file(object_name).decode("utf-8")
     return jsonify({"message": f"Uploaded {object_name} to S3"})
 """,
         "requirements": [],
     },
+    # AWS Elasticache Redis
+    ElasticacheRedis: {
+        "infra_docs_url": "https://docs.launchflow.com/reference/aws-resources/elasticache-redis",
+        "infra_name": "elasticache",
+        "infra_lf_class": "lf.aws.ElasticacheRedis",
+        "launchflow_imports": "",
+        "infra_import": None,
+        "global_setup": None,
+        "infra_setup": "# Connect to the Redis instance\nredis_client = elasticache.redis()\n",
+        "app_imports": [],
+        "flask_test_endpoint": """
+# NOTE: This should normally use a POST request since it's modifying state, but we're
+# using GET so you can easily test it in your browser.
+@app.get("/test_redis/<key>")
+def test_redis(key: str):
+    # Write to Redis
+    value = request.json["value"]
+    redis_client.set(key, value)
+    # Immediately read from Redis to verify the write
+    value = redis_client.get(key)
+    return jsonify({"message": f"Set {key} to {value}"})
+""",
+        "requirements": ["redis>=4.2.0"],
+    },
     # AWS RDS (Postgres)
     RDSPostgres: {
-        "infra_docs_url": "https://docs.launchflow.com/reference/aws-resources/rds",
+        "infra_docs_url": "https://docs.launchflow.com/reference/aws-resources/rds-postgres",
         "infra_name": "postgres",
         "infra_lf_class": "lf.aws.RDSPostgres",
         "launchflow_imports": "",
         "infra_import": None,
         "global_setup": None,
         "app_imports": [
             "from app.models import Base, StorageUser",
@@ -430,20 +454,24 @@
     def launchflow_service_product(self) -> str:
         if self.cloud_provider == "aws":
             return "aws_ecs_fargate"
         elif self.cloud_provider == "gcp":
             return "gcp_cloud_run"
         raise ValueError(f"Unsupported cloud provider: {self.cloud_provider}")
 
-    def template_directory(self) -> str:
+    def template_path_info(self) -> str:
+        template_dir = "launchflow.cli.gen.templates.flask"
+        template_name = "_simple_template"
+
         if CloudSQLPostgres in [
             resource for resource in self.resources
         ] or RDSPostgres in [resource for resource in self.resources]:
-            return "launchflow.cli.gen.templates.flask._postgres_template"
-        return "launchflow.cli.gen.templates.flask._simple_template"
+            template_name = "_postgres_template"
+
+        return template_dir, template_name
 
     @property
     def docker_repository_prefix(self) -> str:
         if self.cloud_provider == "aws":
             return "public.ecr.aws/docker/library/"
         return ""
 
@@ -469,23 +497,23 @@
             "app_infra_imports": self.app_infra_imports,
             "app_global_setup": self.app_global_setup,
             "app_infra_setup": self.app_infra_setup,
             "app_infra_endpoints": self.app_infra_endpoints,
         }
 
 
-if __name__ == "__main__":
-    cloud_provider = "gcp"
-    generator = FlaskProjectGenerator(
-        resources=[
-            ComputeEngineRedis,
-            GCSBucket,
-            CloudSQLPostgres,
-            # S3Bucket,
-            # RDSPostgres,
-        ],
-        cloud_provider=cloud_provider,
-        launchflow_project_name=f"{cloud_provider}-examples",
-        launchflow_environment_name="dev",
-        launchflow_service_name="flask-service",
-    )
-    generator.generate_project(destination_path="/tmp/launchflow")
+# if __name__ == "__main__":
+#     cloud_provider = "gcp"
+#     generator = FlaskProjectGenerator(
+#         resources=[
+#             ComputeEngineRedis,
+#             GCSBucket,
+#             CloudSQLPostgres,
+#             # S3Bucket,
+#             # RDSPostgres,
+#         ],
+#         cloud_provider=cloud_provider,
+#         launchflow_project_name=f"{cloud_provider}-examples",
+#         launchflow_environment_name="dev",
+#         launchflow_service_name="flask-service",
+#     )
+#     generator.generate_project(destination_path="/tmp/launchflow")
```

### Comparing `launchflow-0.3.9.dev8/launchflow/cli/project/project_commands.py` & `launchflow-0.4.0.dev0/launchflow/cli/project/project_commands.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,37 +1,55 @@
+import httpx
+import rich
 import typer
+
 from launchflow.cli.utils import print_response
 from launchflow.cli.utyper import UTyper
+from launchflow.clients import async_launchflow_client_ctx
+from launchflow.clients.projects_client import ProjectsAsyncClient
 from launchflow.config import config
 from launchflow.exceptions import LaunchFlowException
 from launchflow.flows.project_flows import create_project
 
-from launchflow.clients import async_launchflow_client_ctx
-
 app = UTyper(help="Interact with your LaunchFlow projects.")
 
 
 @app.command()
-async def list():
+async def list(
+    launch_url: str = typer.Option(
+        "https://launch.launchflow.com", help="The LaunchFlow URL.", hidden=True
+    )
+):
     """Lists all current projects in your account."""
-    async with async_launchflow_client_ctx() as client:
-        projects = await client.projects.list(config.settings.default_account_id)
 
+    async with httpx.AsyncClient(timeout=60) as client:
+        proj_client = ProjectsAsyncClient(http_client=client, base_url=launch_url)
+        projects = await proj_client.list(config.settings.default_account_id)
     print_response(
-        "Projects", {"projects": [projects.model_dump() for projects in projects]}
+        "Projects",
+        {
+            "projects": [
+                projects.model_dump(exclude_defaults=True) for projects in projects
+            ]
+        },
     )
 
 
 @app.command()
-async def get(project_name: str):
+async def get(
+    project_name: str,
+    launch_url: str = typer.Option(
+        "https://launch.launchflow.com", help="The LaunchFlow URL.", hidden=True
+    ),
+):
     """Get information about a specific project."""
-    async with async_launchflow_client_ctx() as client:
-        project = await client.projects.get(project_name)
-
-    print_response("Project", project.model_dump())
+    async with httpx.AsyncClient(timeout=60) as client:
+        proj_client = ProjectsAsyncClient(http_client=client, base_url=launch_url)
+        project = await proj_client.get(project_name)
+    print_response("Project", project.model_dump(exclude_defaults=True))
 
 
 @app.command()
 async def create(
     project_name: str = typer.Argument(None, help="The name of the project to create."),
     account_id: str = typer.Option(
         None,
@@ -40,12 +58,25 @@
 ):
     """Create a new project in your account."""
     async with async_launchflow_client_ctx() as client:
         try:
             project = await create_project(
                 client=client, project_name=project_name, account_id=account_id
             )
-        except LaunchFlowException as e:
-            e.pretty_print()
+        except LaunchFlowException:
             raise typer.Exit(1)
 
-    print_response("Project", project.model_dump())
+    print_response("Project", project.model_dump(exclude_defaults=True))
+
+
+@app.command()
+async def delete(name: str = typer.Argument(..., help="The project name.")):
+    """Delete a project."""
+    try:
+        async with async_launchflow_client_ctx() as client:
+            await client.projects.delete(name)
+
+    except Exception as e:
+        typer.echo(e)
+        raise typer.Exit(1)
+
+    rich.print("[green]✓[/green] Project deleted.")
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `launchflow-0.3.9.dev8/launchflow/cli/project_gen.py` & `launchflow-0.4.0.dev0/launchflow/cli/project_gen.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 from enum import Enum
 from typing import List, Literal, Optional, Type
 
 import beaupy
 import rich
+
+from launchflow import Resource
+from launchflow.aws.elasticache import ElasticacheRedis
 from launchflow.aws.rds import RDSPostgres
 from launchflow.aws.s3 import S3Bucket
 from launchflow.clients.client import LaunchFlowAsyncClient
 from launchflow.flows.project_flows import get_project
 from launchflow.gcp.cloudsql import CloudSQLPostgres
 from launchflow.gcp.compute_engine import ComputeEngineRedis
 from launchflow.gcp.gcs import GCSBucket
 from launchflow.gcp.memorystore import MemorystoreRedis
 
-from launchflow import Resource
-
 
 class Framework(Enum):
     FASTAPI = "fastapi"
     FLASK = "flask"
     DJANGO = "django"
 
 
 FRAMEWORK_CHOICES = [
     (
         Framework.FASTAPI,
-        "FastAPI framework, high performance, easy to learn, fast to code, ready for production",
+        "FastAPI framework, high performance, easy to learn, fast to code, ready for production.",
     ),
     (
         Framework.FLASK,
         "The Python micro framework for building web applications.",
     ),
     (
         Framework.DJANGO,
@@ -61,14 +62,18 @@
         S3Bucket,
         "Storage bucket. Powered by Amazon S3.",
     ),
     (
         RDSPostgres,
         "PostgreSQL database. Powered by Amazon RDS.",
     ),
+    (
+        ElasticacheRedis,
+        "Redis Cluster. Powered by Amazon ElastiCache.",
+    ),
 ]
 
 
 async def project(client: LaunchFlowAsyncClient, account_id: Optional[str]):
     print()
     print("Welcome to launchflow!")
     print("This tool will help you create a new application.")
```

### Comparing `launchflow-0.3.9.dev8/launchflow/cli/resources/resource_commands.py` & `launchflow-0.4.0.dev0/launchflow/cli/resources/resource_commands.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import typer
+from rich.progress import Progress, SpinnerColumn, TextColumn
+
 from launchflow.cli.constants import ENVIRONMENT_HELP, PROJECT_HELP
 from launchflow.cli.utils import print_response
 from launchflow.cli.utyper import UTyper
+from launchflow.clients import async_launchflow_client_ctx
 from launchflow.clients.response_schemas import OperationStatus
 from launchflow.exceptions import LaunchFlowRequestFailure
 from launchflow.flows.environments_flows import get_environment
 from launchflow.flows.project_flows import get_project
-from rich.progress import Progress, SpinnerColumn, TextColumn
-
-from launchflow.clients import async_launchflow_client_ctx
 
 app = UTyper(help="Commands for managing resources in LaunchFlow")
 
 
 @app.command()
 async def get(
     resource_name: str = typer.Argument(..., help="Resource to fetch information for."),
```

### Comparing `launchflow-0.3.9.dev8/launchflow/cli/resources_ast.py` & `launchflow-0.4.0.dev0/launchflow/cli/ast_search.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,54 +1,86 @@
 import ast
 import importlib
 import logging
 import os
-from typing import List
+from typing import List, Literal
 
+from launchflow.generics import GenericResource
 from launchflow.resource import Resource
+from launchflow.service import Service
 
 # TODO: add primitive ones here.
 # NOTE: We do this to ensure we don't trigger imports in files we don't need to.
 # For instance if someone uses `launchflow.fastapi` in a file, we don't want to
 # execute that file.
-KNOWN_RESOURCE_IMPORT_PATHS = ["launchflow.gcp", "launchflow.aws"]
+KNOWN_IMPORT_PATHS = [
+    "launchflow.gcp",
+    "launchflow.aws",
+    "launchflow.docker",
+    "launchflow",
+]
 
 
-def _is_launchflow_resource(import_path: str) -> bool:
-    maybe_resource = False
-    for known_import in KNOWN_RESOURCE_IMPORT_PATHS:
+def _is_launchflow_entity(import_path: str) -> bool:
+    maybe_entity = False
+    for known_import in KNOWN_IMPORT_PATHS:
         if known_import in import_path:
-            maybe_resource = True
+            maybe_entity = True
             break
-    if not maybe_resource:
+    if not maybe_entity:
         return False
     split_path = import_path.split(".")
     resource_name = split_path[-1]
-    module = ".".join(split_path[:-1])
-    module_type = importlib.import_module(module)
 
     # This checks if the resource_name starts with a lowercase character to act as a
     # proxy check for the resource being a class. This is not foolproof but should
     # filter out most utility functions.
     if resource_name[0].islower():
         return False
+    return maybe_entity
+
+
+def _is_launchflow_resource(import_path: str) -> bool:
+    if not _is_launchflow_entity(import_path):
+        return False
+    split_path = import_path.split(".")
+    resource_name = split_path[-1]
+    module = ".".join(split_path[:-1])
+    module_type = importlib.import_module(module)
+
+    if hasattr(module_type, resource_name) and (
+        issubclass(getattr(module_type, resource_name), Resource)
+        or issubclass(getattr(module_type, resource_name), GenericResource)
+    ):
+        return True
+    return False
+
+
+def _is_launchflow_service(import_path: str) -> bool:
+    if not _is_launchflow_entity(import_path):
+        return False
+    split_path = import_path.split(".")
+    service_name = split_path[-1]
+    module = ".".join(split_path[:-1])
+    module_type = importlib.import_module(module)
 
-    if hasattr(module_type, resource_name) and issubclass(
-        getattr(module_type, resource_name), Resource
+    if hasattr(module_type, service_name) and issubclass(
+        getattr(module_type, service_name), Service
     ):
         return True
     return False
 
 
 class LaunchFlowAssignmentVisitor(ast.NodeVisitor):
-    def __init__(self):
+    def __init__(self, scan_type: Literal["resources", "services"]):
         super().__init__()
         self.launchflow_imported_names = {}
         self.launchflow_vars = []
         self.nesting_level = 0
+        self.scan_type = scan_type
 
     def visit_Import(self, node):
         for alias in node.names:
             if alias.name == "launchflow":
                 self.launchflow_imported_names[
                     alias.asname if alias.asname else alias.name
                 ] = "launchflow"
@@ -96,56 +128,68 @@
         call_name = None
         if isinstance(node.value.func, ast.Name):
             call_name = self.launchflow_imported_names.get(node.value.func.id)
         elif isinstance(node.value.func, ast.Attribute):
             call_name = self._reconstruct_full_name(node.value.func)
         else:
             return
-        if call_name and _is_launchflow_resource(call_name):
-            if self.nesting_level != 0:
-                logging.error(
-                    "Resource is not defined as a global variable `%s` of type `%s` and will be ignored",
-                    assigned_var,
-                    call_name,
-                )
-                return
-            self.launchflow_vars.append(assigned_var)
+        if call_name:
+            if (
+                self.scan_type == "resources" and _is_launchflow_resource(call_name)
+            ) or (self.scan_type == "services" and _is_launchflow_service(call_name)):
+                if self.nesting_level != 0:
+                    logging.error(
+                        "Not defined as a global variable `%s` of type `%s` and will be ignored",
+                        assigned_var,
+                        call_name,
+                    )
+                    return
+                self.launchflow_vars.append(assigned_var)
 
     def _reconstruct_full_name(self, node):
         parts = []
         while isinstance(node, ast.Attribute):
             parts.append(node.attr)
             node = node.value
         if isinstance(node, ast.Name) and node.id in self.launchflow_imported_names:
             parts.append(self.launchflow_imported_names[node.id])
         else:
             return None
         parts.reverse()
         return ".".join(parts)
 
 
-def find_launchflow_resources(directory: str):
+def find_launchflow_resources(directory: str) -> List[str]:
+    to_scan = []
+    for root, dirs, files in os.walk(directory):
+        for file in files:
+            if file.endswith(".py"):
+                to_scan.append(os.path.join(root, file))
+    return _scan_for(to_scan, root=directory, scan_type="resources")
+
+
+def find_launchflow_services(directory: str) -> List[str]:
     to_scan = []
     for root, dirs, files in os.walk(directory):
         for file in files:
             if file.endswith(".py"):
                 to_scan.append(os.path.join(root, file))
-    return _scan_for_resources(to_scan, root=directory)
+    return _scan_for(to_scan, root=directory, scan_type="services")
 
 
-def _scan_for_resources(files: List[str], root: str):
-    resource_imports = []
+def _scan_for(files: List[str], root: str, scan_type: Literal["resources", "services"]):
+    entity_imports = []
     for file_path in files:
         with open(file_path, "r") as f:
             file_contents = f.read()
         tree = ast.parse(file_contents)
-        finder = LaunchFlowAssignmentVisitor()
+        finder = LaunchFlowAssignmentVisitor(scan_type=scan_type)
         finder.visit(tree)
         base_module_path = (
             os.path.relpath(file_path, root)[:-3].split(os.path.sep)
             if file_path.endswith(".py")
             else os.path.relpath(file_path, root).split(os.path.sep)
         )
         module_path = ".".join(base_module_path)
         for var in finder.launchflow_vars:
-            resource_imports.append(f"{module_path}:{var}")
-    return resource_imports
+            entity_imports.append(f"{module_path}:{var}")
+    return entity_imports
```

### Comparing `launchflow-0.3.9.dev8/launchflow/cli/services/service_commands.py` & `launchflow-0.4.0.dev0/launchflow/cli/services/service_commands.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import typer
+from rich.progress import Progress, SpinnerColumn, TextColumn
+
 from launchflow.cli.constants import ENVIRONMENT_HELP, PROJECT_HELP
 from launchflow.cli.utils import print_response
 from launchflow.cli.utyper import UTyper
+from launchflow.clients import async_launchflow_client_ctx
 from launchflow.clients.response_schemas import OperationStatus
 from launchflow.exceptions import LaunchFlowRequestFailure
 from launchflow.flows.environments_flows import get_environment
 from launchflow.flows.project_flows import get_project
-from rich.progress import Progress, SpinnerColumn, TextColumn
-
-from launchflow.clients import async_launchflow_client_ctx
 
 app = UTyper(help="Commands for managing services in LaunchFlow")
 
 
 @app.command()
 async def get(
     service_name: str = typer.Argument(..., help="Service to fetch information for."),
```

### Comparing `launchflow-0.3.9.dev8/launchflow/cli/utils.py` & `launchflow-0.4.0.dev0/launchflow/cli/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -73,25 +73,27 @@
 def print_response(header: str, response: Dict[str, Any]):
     response = _preprocess_dict(response)
     print(header)
     print("-" * len(header))
     print(json_to_yaml(response))
 
 
-def tar_source_in_memory(
-    directory: str = ".",
-    ignore_patterns: List[str] = [
-        "*.log",
-        "__pycache__/",
-        ".env",
-        ".git/",
-        ".terraform/",
-        ".terraform.lock.hcl",
-    ],
-):
+_DEFAULT_IGNORE_PATTERNS = [
+    "*.log",
+    "__pycache__/",
+    ".env",
+    ".git/",
+    ".terraform/",
+    ".terraform.lock.hcl",
+]
+
+
+def tar_source_in_memory(directory: str, ignore_patterns: List[str]):
+    ignore_patterns = set(ignore_patterns + _DEFAULT_IGNORE_PATTERNS)
+
     def should_include_file(pathspec: PathSpec, file_path: str, root_dir: str):
         relative_path = os.path.relpath(file_path, root_dir)
         return not pathspec.match_file(relative_path)
 
     pathspec = PathSpec.from_lines("gitwildmatch", ignore_patterns)
 
     # Use BytesIO object as an in-memory file
```

### Comparing `launchflow-0.3.9.dev8/launchflow/clients/accounts_client.py` & `launchflow-0.4.0.dev0/launchflow/clients/accounts_client.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,31 +1,42 @@
+from typing import Optional
+
 import httpx
+
 from launchflow.clients.response_schemas import AccountResponse
 from launchflow.config import config
 from launchflow.exceptions import LaunchFlowRequestFailure
 
 
 class AccountsAsyncClient:
-    def __init__(self, http_client: httpx.AsyncClient):
+    def __init__(self, http_client: httpx.AsyncClient, api_key: Optional[str] = None):
         self.http_client = http_client
         self.url = f"{config.settings.account_service_address}/accounts"
+        self._api_key = api_key
+
+    @property
+    def access_token(self):
+        if self._api_key is not None:
+            return self._api_key
+        else:
+            return config.get_access_token()
 
     async def list(self):
         response = await self.http_client.get(
             self.url,
-            headers={"Authorization": f"Bearer {config.get_access_token()}"},
+            headers={"Authorization": f"Bearer {self.access_token}"},
         )
         if response.status_code != 200:
             raise LaunchFlowRequestFailure(response)
         return [
             AccountResponse.model_validate(account)
             for account in response.json()["accounts"]
         ]
 
     async def get(self, account_id: str):
         response = await self.http_client.get(
             f"{self.url}/{account_id}",
-            headers={"Authorization": f"Bearer {config.get_access_token()}"},
+            headers={"Authorization": f"Bearer {self.access_token}"},
         )
         if response.status_code != 200:
             raise LaunchFlowRequestFailure(response)
         return AccountResponse.model_validate(response.json())
```

### Comparing `launchflow-0.3.9.dev8/launchflow/clients/client.py` & `launchflow-0.4.0.dev0/launchflow/clients/client.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,23 @@
+from typing import Optional
+
 import httpx
+
 from launchflow.clients.accounts_client import AccountsAsyncClient
-from launchflow.clients.connect_client import CloudConectAsyncClient
 from launchflow.clients.environments_client import EnvironmentsAsyncClient
-from launchflow.clients.operations_client import OperationsAsyncClient
 from launchflow.clients.projects_client import ProjectsAsyncClient
 from launchflow.clients.resources_client import ResourcesAsyncClient
 from launchflow.clients.services_client import ServicesAsyncClient
 
 
 class LaunchFlowAsyncClient:
-    def __init__(self) -> None:
+    def __init__(self, api_key: Optional[str] = None) -> None:
         self.http_client = httpx.AsyncClient(timeout=60)
 
-        self.accounts = AccountsAsyncClient(self.http_client)
-        self.environments = EnvironmentsAsyncClient(self.http_client)
-        self.projects = ProjectsAsyncClient(self.http_client)
-        self.connect = CloudConectAsyncClient(self.http_client)
-        self.resources = ResourcesAsyncClient(self.http_client)
-        self.operations = OperationsAsyncClient(self.http_client)
-        self.services = ServicesAsyncClient(self.http_client)
+        self.accounts = AccountsAsyncClient(self.http_client, api_key)
+        self.environments = EnvironmentsAsyncClient(self.http_client, api_key)
+        self.projects = ProjectsAsyncClient(self.http_client, api_key)
+        self.resources = ResourcesAsyncClient(self.http_client, api_key)
+        self.services = ServicesAsyncClient(self.http_client, api_key)
 
     async def close(self):
         await self.http_client.aclose()
```

### Comparing `launchflow-0.3.9.dev8/launchflow/clients/resources_client.py` & `launchflow-0.4.0.dev0/launchflow/clients/resources_client.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,33 +1,42 @@
 from typing import Any, Dict, List, Optional
 
 import httpx
+
 from launchflow.clients.response_schemas import OperationResponse, ResourceResponse
 from launchflow.config import config
 from launchflow.exceptions import LaunchFlowRequestFailure, ResourceProductMismatch
 
 
 class ResourcesSyncClient:
-    def __init__(self, http_client: httpx.Client):
+    def __init__(self, http_client: httpx.Client, api_key: Optional[str] = None):
         self.http_client = http_client
+        self._api_key = api_key
+
+    @property
+    def access_token(self):
+        if self._api_key is not None:
+            return self._api_key
+        else:
+            return config.get_access_token()
 
     def base_url(self, project_name: str, environment_name: str) -> str:
         return f"{config.settings.launch_service_address}/projects/{project_name}/environments/{environment_name}/resources"
 
     def get(
         self,
         project_name: str,
         environment_name: str,
         resource_name: str,
         product_name_to_validate: Optional[str] = None,
     ):
         url = f"{self.base_url(project_name, environment_name)}/{resource_name}"
         response = self.http_client.get(
             url,
-            headers={"Authorization": f"Bearer {config.get_access_token()}"},
+            headers={"Authorization": f"Bearer {self.access_token}"},
         )
         if response.status_code != 200:
             raise LaunchFlowRequestFailure(response)
 
         resource_info = ResourceResponse.model_validate(response.json())
 
         # Validate product name matches if provided
@@ -39,16 +48,24 @@
                 product_name_to_validate, resource_info.resource_product
             )
 
         return resource_info
 
 
 class ResourcesAsyncClient:
-    def __init__(self, http_client: httpx.AsyncClient):
+    def __init__(self, http_client: httpx.AsyncClient, api_key: Optional[str] = None):
         self.http_client = http_client
+        self._api_key = api_key
+
+    @property
+    def access_token(self):
+        if self._api_key is not None:
+            return self._api_key
+        else:
+            return config.get_access_token()
 
     def base_url(self, project_name: str, environment_name: str) -> str:
         return f"{config.settings.launch_service_address}/projects/{project_name}/environments/{environment_name}/resources"
 
     async def create(
         self,
         project_name: str,
@@ -56,15 +73,15 @@
         product_name: str,
         resource_name: str,
         create_args: Dict[str, Any],
     ):
         response = await self.http_client.post(
             f"{self.base_url(project_name, environment_name)}/{product_name}/{resource_name}",
             json=create_args,
-            headers={"Authorization": f"Bearer {config.get_access_token()}"},
+            headers={"Authorization": f"Bearer {self.access_token}"},
         )
         if response.status_code != 201:
             raise LaunchFlowRequestFailure(response)
         return OperationResponse.model_validate(response.json())
 
     async def replace(
         self,
@@ -73,15 +90,15 @@
         product_name: str,
         resource_name: str,
         create_args: Dict[str, Any],
     ):
         response = await self.http_client.put(
             f"{self.base_url(project_name, environment_name)}/{product_name}/{resource_name}",
             json=create_args,
-            headers={"Authorization": f"Bearer {config.get_access_token()}"},
+            headers={"Authorization": f"Bearer {self.access_token}"},
         )
         if response.status_code != 201:
             raise LaunchFlowRequestFailure(response)
         return OperationResponse.model_validate(response.json())
 
     # NOTE: Product name is optional because its only used for opt-in validation.
     async def get(
@@ -90,15 +107,15 @@
         environment_name: str,
         resource_name: str,
         product_name_to_validate: Optional[str] = None,
     ):
         url = f"{self.base_url(project_name, environment_name)}/{resource_name}"
         response = await self.http_client.get(
             url,
-            headers={"Authorization": f"Bearer {config.get_access_token()}"},
+            headers={"Authorization": f"Bearer {self.access_token}"},
         )
         if response.status_code != 200:
             raise LaunchFlowRequestFailure(response)
 
         resource_info = ResourceResponse.model_validate(response.json())
 
         # Validate product name matches if provided
@@ -114,27 +131,27 @@
 
     async def list(
         self, project_name: str, environment_name: str
     ) -> List[ResourceResponse]:
         url = self.base_url(project_name, environment_name)
         response = await self.http_client.get(
             url,
-            headers={"Authorization": f"Bearer {config.get_access_token()}"},
+            headers={"Authorization": f"Bearer {self.access_token}"},
         )
         if response.status_code != 200:
             raise LaunchFlowRequestFailure(response)
         return [
             ResourceResponse.model_validate(resource)
             for resource in response.json()["resources"]
         ]
 
     async def delete(
         self, project_name: str, environment_name: str, resource_name: str
     ):
         url = f"{self.base_url(project_name, environment_name)}/{resource_name}"
         response = await self.http_client.delete(
             url,
-            headers={"Authorization": f"Bearer {config.get_access_token()}"},
+            headers={"Authorization": f"Bearer {self.access_token}"},
         )
         if response.status_code != 202:
             raise LaunchFlowRequestFailure(response)
         return OperationResponse.model_validate(response.json())
```

### Comparing `launchflow-0.3.9.dev8/launchflow/clients/response_schemas.py` & `launchflow-0.4.0.dev0/launchflow/clients/response_schemas.py`

 * *Files identical despite different names*

### Comparing `launchflow-0.3.9.dev8/launchflow/clients/services_client.py` & `launchflow-0.4.0.dev0/launchflow/clients/services_client.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,56 +1,99 @@
 import io
 from typing import Any, Dict, List, Optional
 
 import httpx
+
 from launchflow.clients.response_schemas import OperationResponse, ServiceResponse
 from launchflow.config import config
 from launchflow.exceptions import LaunchFlowRequestFailure, ServiceProductMismatch
 
 
 class ServicesAsyncClient:
-    def __init__(self, http_client: httpx.AsyncClient):
+    def __init__(self, http_client: httpx.AsyncClient, api_key: Optional[str] = None):
         self.http_client = http_client
+        self._api_key = api_key
+
+    @property
+    def access_token(self):
+        if self._api_key is not None:
+            return self._api_key
+        else:
+            return config.get_access_token()
 
     def base_url(self, project_name: str, environment_name: str) -> str:
         return f"{config.settings.launch_service_address}/projects/{project_name}/environments/{environment_name}/services"
 
     async def deploy(
         self,
         project_name: str,
         environment_name: str,
         product_name: str,
         service_name: str,
         tar_bytes: io.BytesIO,
-        # TODO: add create args on client
+        dockerfile_path: str,
         create_args: Dict[str, Any],
+        notify_on_failure: bool = False,
     ):
+
+        data = {
+            "dockerfile_path": dockerfile_path,
+            "notify_on_failure": notify_on_failure,
+            **create_args,
+        }
         response = await self.http_client.post(
             f"{self.base_url(project_name, environment_name)}/{product_name}/{service_name}",
             files={"source_tarball": ("source.tar.gz", tar_bytes, "application/zip")},
-            headers={"Authorization": f"Bearer {config.get_access_token()}"},
+            data=data,
+            headers={
+                "Authorization": f"Bearer {self.access_token}",
+            },
             # default timeout is 5 seconds, but submitting a build can take a while
             timeout=60,
         )
         if response.status_code != 201:
             raise LaunchFlowRequestFailure(response)
         return OperationResponse.model_validate(response.json())
 
+    async def promote(
+        self,
+        service_name: str,
+        project_name: str,
+        from_environment_name: str,
+        to_environment_name: str,
+        create_args: Dict[str, Any],
+        notify_on_failure: bool = False,
+    ):
+        response = await self.http_client.post(
+            f"{self.base_url(project_name, from_environment_name)}/{service_name}/promote",
+            json={
+                "to_environment_name": to_environment_name,
+                "notify_on_failure": notify_on_failure,
+                "create_args": create_args,
+            },
+            headers={
+                "Authorization": f"Bearer {self.access_token}",
+            },
+        )
+        if response.status_code != 202:
+            raise LaunchFlowRequestFailure(response)
+        return OperationResponse.model_validate(response.json())
+
     # NOTE: Product name is optional because its only used for opt-in validation.
     async def get(
         self,
         project_name: str,
         environment_name: str,
         service_name: str,
         product_name_to_validate: Optional[str] = None,
-    ):
+    ) -> ServiceResponse:
         url = f"{self.base_url(project_name, environment_name)}/{service_name}"
         response = await self.http_client.get(
             url,
-            headers={"Authorization": f"Bearer {config.get_access_token()}"},
+            headers={"Authorization": f"Bearer {self.access_token}"},
         )
         if response.status_code != 200:
             raise LaunchFlowRequestFailure(response)
 
         service_info = ServiceResponse.model_validate(response.json())
 
         # Validate product name matches if provided
@@ -66,25 +109,25 @@
 
     async def list(
         self, project_name: str, environment_name: str
     ) -> List[ServiceResponse]:
         url = self.base_url(project_name, environment_name)
         response = await self.http_client.get(
             url,
-            headers={"Authorization": f"Bearer {config.get_access_token()}"},
+            headers={"Authorization": f"Bearer {self.access_token}"},
         )
         if response.status_code != 200:
             raise LaunchFlowRequestFailure(response)
         return [
             ServiceResponse.model_validate(service)
             for service in response.json()["services"]
         ]
 
     async def delete(self, project_name: str, environment_name: str, service_name: str):
         url = f"{self.base_url(project_name, environment_name)}/{service_name}"
         response = await self.http_client.delete(
             url,
-            headers={"Authorization": f"Bearer {config.get_access_token()}"},
+            headers={"Authorization": f"Bearer {self.access_token}"},
         )
         if response.status_code != 202:
             raise LaunchFlowRequestFailure(response)
         return OperationResponse.model_validate(response.json())
```

### Comparing `launchflow-0.3.9.dev8/launchflow/config/launchflow_config.py` & `launchflow-0.4.0.dev0/launchflow/config/launchflow_config.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import dataclasses
 import os
 import time
 from typing import Any, Dict, Optional
 
 import requests
 import toml
+
 from launchflow.config.launchflow_env import LaunchFlowEnvVars, load_launchflow_env
 from launchflow.config.launchflow_yaml import (
     LaunchFlowDotYaml,
     load_launchflow_dot_yaml,
 )
 from launchflow.exceptions import LaunchFlowRequestFailure
 
@@ -34,18 +35,27 @@
         return self.expires_at_seconds - _REFRESH_BUFFER < int(time.time())
 
 
 @dataclasses.dataclass
 class LaunchFlowConfig:
     settings: Settings
     credentials: Optional[Credentials]
-    launchflow_yaml: Optional[LaunchFlowDotYaml]
+    # NOTE: this is lazy loaded since it requires network operations
     env: LaunchFlowEnvVars
 
     @property
+    def launchflow_yaml(self) -> Optional[LaunchFlowDotYaml]:
+        """This is a property so it can be lazily loaded."""
+        # TODO: the callers of this should check if its none before proceeding
+        try:
+            return load_launchflow_dot_yaml()
+        except FileNotFoundError:
+            return None
+
+    @property
     def project(self):
         # Environment variable takes precedence
         if self.env.project is not None:
             return self.env.project
         # Then launchflow.yaml
         if self.launchflow_yaml is not None:
             return self.launchflow_yaml.project
@@ -59,14 +69,22 @@
             return self.env.environment
         # Then launchflow.yaml
         if self.launchflow_yaml is not None:
             return self.launchflow_yaml.environment
         # Default to None
         return None
 
+    @property
+    def local_mode(self):
+        return self.env.local_mode_enabled
+
+    @local_mode.setter
+    def local_mode(self, value):
+        self.env.local_mode_enabled = value
+
     def list_service_configs(self):
         if self.launchflow_yaml is not None:
             return self.launchflow_yaml.services
         return []
 
     @classmethod
     def load(cls):
@@ -81,25 +99,19 @@
                 toml.dump(dataclasses.asdict(settings), f)
 
         credentials = None
         if os.path.exists(CREDENTIALS_PATH):
             with open(CREDENTIALS_PATH) as f:
                 credentials = Credentials(**toml.load(f))
 
-        try:
-            launchflow_dot_yaml = load_launchflow_dot_yaml()
-        except FileNotFoundError:
-            launchflow_dot_yaml = None
-
         launchflow_env = load_launchflow_env()
 
         return cls(
             settings=settings,
             credentials=credentials,
-            launchflow_yaml=launchflow_dot_yaml,
             env=launchflow_env,
         )
 
     def get_access_token(self):
         if self.credentials is None:
             raise ValueError("No credentials")
         if self.credentials.is_expired():
```

### Comparing `launchflow-0.3.9.dev8/launchflow/config/launchflow_yaml.py` & `launchflow-0.4.0.dev0/launchflow/config/launchflow_yaml.py`

 * *Files 25% similar despite different names*

```diff
@@ -9,26 +9,56 @@
 
 
 @dataclass
 class ProductConfig:
     pass
 
     def to_dict(self):
-        dict_with_nones = asdict(self)
-        return {k: v for k, v in dict_with_nones.items() if v is not None}
+        to_ret = {}
+        for k, v in asdict(self).items():
+            if v is None:
+                continue
+            elif isinstance(v, list):
+                to_ret[k] = ",".join(v)
+            else:
+                to_ret[k] = v
+        return to_ret
+
+    def merge(self, other):
+        for k, v in asdict(other).items():
+            if isinstance(v, list):
+                curr = getattr(self, k)
+                if curr is not None:
+                    curr.extend(v)
+                    setattr(self, k, curr)
+                else:
+                    setattr(self, k, v)
+            elif v is not None:
+                setattr(self, k, v)
 
 
 @dataclass
 class GcpCloudRunConfig(ProductConfig):
-    location: Optional[str] = None
+    region: Optional[str] = None
     cpu: Optional[int] = None
     memory: Optional[str] = None
-    min_instances: Optional[int] = None
-    max_instances: Optional[int] = None
-    container_concurrency: Optional[int] = None
+    port: Optional[int] = None
+    publicly_accessible: Optional[bool] = None
+    min_instance_count: Optional[int] = None
+    max_instance_count: Optional[int] = None
+    max_instance_request_concurrency: Optional[int] = None
+    invokers: Optional[List[str]] = None
+    custom_audiences: Optional[List[str]] = None
+    ingress: Optional[
+        Literal[
+            "INGRESS_TRAFFIC_ALL",
+            "INGRESS_TRAFFIC_INTERNAL_ONLY",
+            "INGRESS_TRAFFIC_INTERNAL_LOAD_BALANCER",
+        ]
+    ] = None
 
 
 @dataclass
 class AwsEcsFargateConfig(ProductConfig):
     cpu: Optional[str] = None
     memory: Optional[int] = None
 
@@ -43,59 +73,94 @@
         raise ValueError(f"Unsupported product type: {product_type}")
 
 
 @dataclass
 class ServiceConfig:
     name: str
     product: ProductType
-    product_config: Optional[Union[GcpCloudRunConfig, AwsEcsFargateConfig]] = None
-    directory: str = "."
-    dockerfile: str = None
+    product_configs: Dict[str, Union[GcpCloudRunConfig, AwsEcsFargateConfig]] = field(
+        default_factory=dict
+    )
+    # The directory to run the build from
+    build_directory: str = "."
+    # Files to ignore uploading in the build context
+    # This can be of the gitignore format
+    build_ignore: List[str] = field(default_factory=list)
+    # The path to the dockerfile. Defaults to the Docker file being in the build directory
+    # This should be relative to the build directory
+    dockerfile: str = "Dockerfile"
     domain_name: Optional[str] = None
 
     @classmethod
     def from_dict(cls, data: dict):
         product_type = data.get("product")
-        product_config_data = data.get("product-config", {})
-        product_config = create_product_config(product_type, product_config_data)
-
+        product_configs = data.get("product_configs", {})
+        for env, config in product_configs.items():
+            product_configs[env] = create_product_config(product_type, config)
         return cls(
             name=data.get("name", ""),
             product=product_type,
-            product_config=product_config,
-            directory=data.get("directory", "."),
-            dockerfile=data.get("dockerfile"),
+            product_configs=product_configs,
+            build_directory=data.get("build_directory", "."),
+            build_ignore=data.get("build_ignore", []),
+            dockerfile=data.get("dockerfile", "Dockerfile"),
             domain_name=data.get("domain_name"),
         )
 
     def to_dict(self):
         to_return = {
             "name": self.name,
             "product": self.product,
         }
-        if self.product_config:
-            to_return["product-config"] = self.product_config.to_dict()
-        if self.directory:
-            to_return["directory"] = self.directory
+        if self.product_configs:
+            configs = {}
+            for env, config in self.product_configs.items():
+                configs[env] = config.to_dict()
+            to_return["product_configs"] = configs
+        if self.build_directory:
+            to_return["build_directory"] = self.build_directory
+        if self.build_ignore:
+            to_return["build_ignore"] = self.build_ignore
         if self.dockerfile:
             to_return["dockerfile"] = self.dockerfile
         if self.domain_name:
             to_return["domain_name"] = self.domain_name
         return to_return
 
 
 class Dumper(yaml.Dumper):
     def increase_indent(self, flow=False, *args, **kwargs):
         return super().increase_indent(flow=flow, indentless=False)
 
 
 @dataclass
+class LocalBackend:
+    path: str
+
+
+@dataclass
+class LaunchFlowBackend:
+    launchflow_url: str = "https://launch.launchflow.com"
+    # TODO: should also set this via an environment variable
+    launchflow_api_key: Optional[str] = None
+
+
+@dataclass
+class GCSBackend:
+    bucket: str
+    # Defaults to an empty string, or no string
+    prefix: str = ""
+
+
+@dataclass
 class LaunchFlowDotYaml:
     project: str
     environment: str
+    path: str
+    backend: Union[LocalBackend, LaunchFlowBackend, GCSBackend]
     services: List[ServiceConfig] = field(default_factory=list)
 
     @classmethod
     def load_from_cwd(cls, start_path="."):
         file_path = find_launchflow_yaml(start_path)
         if file_path is None:
             raise FileNotFoundError("Could not find 'launchflow.yaml' file.")
@@ -106,25 +171,52 @@
         if not os.path.exists(file_path):
             raise FileNotFoundError(f"The file '{file_path}' does not exist.")
 
         with open(file_path, "r") as file:
             data = yaml.safe_load(file)
             project = data.get("project", "")
             environment = data.get("environment", "")
+            backend = data.get("backend", {})
             services_data = data.get("services", [])
             services = [ServiceConfig.from_dict(service) for service in services_data]
 
-        return cls(project=project, environment=environment, services=services)
+        if len(backend) > 1:
+            raise ValueError("Only one backend type is allowed in the configuration.")
+        if "local" in backend:
+            backend = LocalBackend(**backend["local"])
+        elif "gcs" in backend:
+            backend = GCSBackend(**backend["gcs"])
+        elif "launchflow" in backend:
+            backend = LaunchFlowBackend(**backend["launchflow"])
+        elif len(backend) == 0:
+            backend = LocalBackend(path="launchflow_state")
+        else:
+            raise ValueError(f"Unsupported backend type: {backend}")
+
+        return cls(
+            project=project,
+            environment=environment,
+            services=services,
+            path=file_path,
+            backend=backend,
+        )
 
     def save_to_file(self, file_path: str):
         services_data = [service.to_dict() for service in self.services]
 
+        if isinstance(LocalBackend, self.backend):
+            backend_key = "local"
+        elif isinstance(LaunchFlowBackend, self.backend):
+            backend_key = "launchflow"
+        else:
+            raise ValueError(f"Unsupported backend type: {self.backend}")
         data = {
             "project": self.project,
             "environment": self.environment,
+            "backend": {backend_key: asdict(self.backend)},
         }
         if services_data:
             data["services"] = services_data
 
         with open(file_path, "w") as file:
             yaml.dump(data, file, Dumper=Dumper)
```

### Comparing `launchflow-0.3.9.dev8/launchflow/fastapi.py` & `launchflow-0.4.0.dev0/launchflow/fastapi.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,30 +82,30 @@
 
     Args:
     - `engine`: A SQLAlchemy engine to use for creating the session.
     - `autocommit`: Whether to autocommit the session after a commit.
     - `autoflush`: Whether to autoflush the session after a commit.
     - `expire_on_commit`: Whether to expire all instances after a commit.
 
-    Example usage:
+    **Example usage:**
     ```python
     import launchflow as lf
 
     from fastapi import FastAPI, Depends
     from sqlalchemy import text
     from sqlalchemy.orm import Session
 
     # Create the Postgres database instance
     postgres = lf.gcp.CloudSQLPostgres("my-pg-db")
 
     # Create the SQLAlchemy engine (connection pool)
     engine = postgres.sqlalchemy_engine()
 
     # Create the FastAPI dependency
-    session = lf.fastapi.sqlalchemy(engine)
+    session = lf.fastapi.sqlalchemy_depends(engine)
 
     app = FastAPI()
 
     @app.get("/")
     def read_root(db: Session = Depends(session)):
         # Use the session to query the database
         return db.execute(text("SELECT 1")).scalar_one_or_none()
@@ -129,15 +129,15 @@
 
     Args:
     - `engine`: A SQLAlchemy engine to use for creating the session.
     - `autocommit`: Whether to autocommit the session after a commit.
     - `autoflush`: Whether to autoflush the session after a commit.
     - `expire_on_commit`: Whether to expire all instances after a commit.
 
-    Example usage:
+    **Example usage:**
     ```python
     from contextlib import asynccontextmanager
 
     import launchflow as lf
 
     from fastapi import FastAPI, Depends
     from sqlalchemy import text
```

### Comparing `launchflow-0.3.9.dev8/launchflow/flows/account_id.py` & `launchflow-0.4.0.dev0/launchflow/flows/account_id.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import Optional
 
 import beaupy
 import rich
+from rich.progress import Progress, SpinnerColumn, TextColumn
+
 from launchflow.clients.client import LaunchFlowAsyncClient
 from launchflow.config import config
-from rich.progress import Progress, SpinnerColumn, TextColumn
 
 
 async def get_account_id_from_config(
     client: LaunchFlowAsyncClient, account_id: Optional[str]
 ) -> str:
     if account_id is None:
         account_id = config.settings.default_account_id
```

### Comparing `launchflow-0.3.9.dev8/launchflow/flows/auth.py` & `launchflow-0.4.0.dev0/launchflow/flows/auth.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 import asyncio
 import base64
 import secrets
 import webbrowser
+from typing import Optional
 
+import beaupy
 import requests
 import rich
+from rich.progress import Progress, SpinnerColumn, TextColumn
+
 from launchflow.clients.client import LaunchFlowAsyncClient
 from launchflow.config import config
-from rich.progress import Progress, SpinnerColumn, TextColumn
 
 
 def _generate_state(length=64):
     random_bytes = secrets.token_bytes(length)
     code_verifier = base64.urlsafe_b64encode(random_bytes).decode("utf-8")
     code_verifier = code_verifier.rstrip("=")
     return code_verifier
@@ -51,22 +54,34 @@
                 raise RuntimeError(f"Failed to get access token. {response.reason}")
             else:
                 await asyncio.sleep(3)
 
         config.update_credentials(credentials)
         accounts = await client.accounts.list()
 
-        if config.settings.default_account_id is None:
-            # TODO: prompt user to select account
-            if len(accounts) == 1:
-                config.settings.default_account_id = accounts[0].id
-                config.save()
-            else:
-                # TODO: prompt the user to select an account as their default
-                pass
+        account_id = None
+        if not accounts:
+            raise RuntimeError(
+                "Account information not found. Please try again and contact founders@launchflow.com if the issue persists."
+            )
+        if len(accounts) == 1:
+            account_id = accounts[0].id
+        else:
+            account_id: Optional[str] = beaupy.select(
+                "Select an account",
+                [account.id for account in accounts],
+                strict=True,
+            )
+            if account_id is None:
+                raise RuntimeError("No account selected")
+
+        if config.settings.default_account_id != account_id:
+            config.settings.default_account_id = account_id
+            config.save()
+
         progress.remove_task(task)
         progress.console.print("[green]✓[/green] Login successful")
 
 
 def logout_flow():
     if config.credentials is None:
         print("Not logged in")
```

### Comparing `launchflow-0.3.9.dev8/launchflow/flows/cloud_provider.py` & `launchflow-0.4.0.dev0/launchflow/flows/cloud_provider.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,20 +9,20 @@
 from enum import Enum
 from typing import Optional
 
 import beaupy
 import requests
 import rich
 import typer
-from launchflow.exceptions import LaunchFlowRequestFailure
-from launchflow.flows.account_id import get_account_id_from_config
 from rich.progress import Progress, SpinnerColumn, TextColumn
 from rich.prompt import Prompt
 
 from launchflow.clients import LaunchFlowAsyncClient
+from launchflow.exceptions import LaunchFlowRequestFailure
+from launchflow.flows.account_id import get_account_id_from_config
 
 XML_TEMPLATE = """
 <?xml version="1.0" encoding="UTF-8"?>
 <!DOCTYPE plist PUBLIC "-//Apple//DTD PLIST 1.0//EN" "http://www.apple.com/DTDs/PropertyList-1.0.dtd">
 <plist version="1.0">
   <array>
     <dict>
@@ -71,32 +71,47 @@
         provider = select_cloud_provider()
 
     setup_status = await client.connect.status(
         account_id=account_id, include_aws_template_url=True
     )
     if provider == CloudProvider.GCP:
         if setup_status.gcp_connection_info.verified_at:
-            rich.print(
-                "[green][bold]GCP is already connected[/bold][/green] 🚀\n"
-                "You can now create environments and deploy resources to your GCP account using LaunchFlow.\n"
+            reverify = beaupy.confirm(
+                "[green bold] GCP has already been connected. Would you like to re-verify your connection? [/green bold]",
             )
-            _setup_local_gcp_env()
+            if reverify:
+                await _connect_gcp(
+                    client,
+                    account_id,
+                    setup_status.gcp_connection_info.admin_service_account_email,
+                    add_permissions=False,
+                )
+            else:
+                _setup_local_gcp_env()
         else:
             await _connect_gcp(
                 client,
                 account_id,
                 setup_status.gcp_connection_info.admin_service_account_email,
+                add_permissions=True,
             )
     elif provider == CloudProvider.AWS:
         if setup_status.aws_connection_info.verified_at:
-            rich.print(
-                "[green][bold]AWS is already connected[/bold][/green] 🚀\n"
-                "You can now create environments and deploy resources to your AWS account using LaunchFlow.\n"
+            reverify = beaupy.confirm(
+                "[green bold] AWS has already been connected. Would you like to re-verify your connection? [/green bold]",
             )
-            _setup_local_aws_env()
+            if reverify:
+                await _connect_aws(
+                    client,
+                    account_id,
+                    setup_status.aws_connection_info.external_role_id,
+                    setup_status.aws_connection_info.cloud_foundation_template_url,
+                )
+            else:
+                _setup_local_aws_env()
         else:
             await _connect_aws(
                 client,
                 account_id,
                 setup_status.aws_connection_info.external_role_id,
                 setup_status.aws_connection_info.cloud_foundation_template_url,
             )
@@ -296,21 +311,36 @@
             add_to_path = beaupy.confirm(
                 "Would you like to add the `aws` binary to your PATH?",
                 default_is_yes=True,
             )
             if add_to_path:
                 if os.path.exists(os.path.expanduser("~/.bashrc")):
                     with open(os.path.expanduser("~/.bashrc"), "a") as f:
-                        f.write(f'export PATH="$PATH:{bin_dir}"\n')
+                        f.write(
+                            f'\n# The next line updates PATH for the aws CLI.\nexport PATH="$PATH:{bin_dir}"\n'
+                        )
+                        f.write(
+                            f'\n# The next line enables shell command completion for aws CLI.\ncomplete -C "{bin_dir}/aws_completer" aws\n'
+                        )
                 if os.path.exists(os.path.expanduser("~/.bash_profile")):
                     with open(os.path.expanduser("~/.bash_profile"), "a") as f:
-                        f.write(f'export PATH="$PATH:{bin_dir}"\n')
+                        f.write(
+                            f'\n# The next line updates PATH for the aws CLI.\nexport PATH="$PATH:{bin_dir}"\n'
+                        )
+                        f.write(
+                            f'\n# The next line enables shell command completion for aws CLI.\ncomplete -C "{bin_dir}/aws_completer" aws\n'
+                        )
                 if os.path.exists(os.path.expanduser("~/.zshrc")):
                     with open(os.path.expanduser("~/.zshrc"), "a") as f:
-                        f.write(f'export PATH="$PATH:{bin_dir}"\n')
+                        f.write(
+                            f'\n# The next line updates PATH for the aws CLI.\nexport PATH="$PATH:{bin_dir}"\n'
+                        )
+                        f.write(
+                            f'\n# The next line enables shell command completion for aws CLI.\ncomplete -C "{bin_dir}/aws_completer" aws\n'
+                        )
             rich.print(
                 "[green]`aws` CLI successfully installed. You will need to reload your terminal to use it.[/green]"
             )
             aws_bin = os.path.join(bin_dir, "aws")
         else:
             rich.print("[green]`aws` CLI is installed[/green]")
             aws_bin = "aws"
@@ -361,17 +391,16 @@
                 rich.print(
                     f"[green]`aws` successfully authenticated with profile `{profile_name}`[/green]"
                 )
         else:
             rich.print("[green]`aws` is authenticated[/green]")
 
     rich.print(
-        "\n[i]Your local machine is setup to interact with AWS resources using LaunchFlow's Python SDK or the `aws` CLI.[/i]"
+        "\n[i]Your local machine is setup to interact with AWS resources using LaunchFlow's Python SDK and/or the `aws` CLI.[/i]"
     )
-    rich.print("Happy launching! 🚀\n")
 
 
 async def _connect_aws(
     client: LaunchFlowAsyncClient,
     account_id: str,
     external_role_id: str,
     template_url: str,
@@ -540,39 +569,56 @@
                 )
                 return
             rich.print(
                 "[green]`gcloud` successfully installed. You will need to reload your terminal to use it.[/green]"
             )
         else:
             rich.print("[green]`gcloud` is installed[/green]")
-        process = subprocess.run(
-            "gcloud auth application-default print-access-token",
-            shell=True,
-            capture_output=True,
-            start_new_session=True,
+
+        check_auth = beaupy.confirm(
+            "Would you like to check if you are authenticated with `gcloud`?",
+            default_is_yes=True,
         )
-        if process.returncode != 0:
-            rich.print("[red]Error: No default `gcloud` credentials found.[/red]")
-            set_up_auth = beaupy.confirm(
-                "Would you like us to authenticate for you?", default_is_yes=True
+        if check_auth:
+            rich.print(
+                "Checking local `gcloud` authentication. NOTE: Older versions of `gcloud` may prompt you for a password."
             )
-            if set_up_auth:
-                rich.print(
-                    "Running:\n\n\t$ gcloud auth login --update-adc\n\nYou can run this whenever you need to reauthenticate your machine with GCP.\n"
-                )
-                process = subprocess.run(
-                    "gcloud auth login --update-adc", shell=True, start_new_session=True
+            rich.print(
+                "Running: \n\n\t$ gcloud auth application-default print-access-token\n\n"
+            )
+            process = subprocess.run(
+                "gcloud auth application-default print-access-token",
+                shell=True,
+                capture_output=True,
+                start_new_session=True,
+            )
+            if process.returncode != 0:
+                rich.print("[red]Error: No default `gcloud` credentials found.[/red]")
+                set_up_auth = beaupy.confirm(
+                    "Would you like us to authenticate for you?", default_is_yes=True
                 )
+                if set_up_auth:
+                    rich.print(
+                        "Running:\n\n\t$ gcloud auth login --update-adc\n\nYou can run this whenever you need to reauthenticate your machine with GCP.\n"
+                    )
+                    process = subprocess.run(
+                        "gcloud auth login --update-adc",
+                        shell=True,
+                        start_new_session=True,
+                    )
+            else:
+                rich.print("[green]`gcloud` is authenticated[/green]")
         else:
-            rich.print("[green]`gcloud` is authenticated[/green]")
+            rich.print(
+                "[i]Skipping gcloud auth check. You can run `gcloud auth login --update-adc` to authenticate with GCP.[/i]"
+            )
 
     rich.print(
-        "\n[i]Your local machine is setup to interact with GCP resources using LaunchFlow's Python SDK or the `gcloud` CLI.[/i]"
+        "\n[i]Your local machine is setup to interact with GCP resources using LaunchFlow's Python SDK and/or the `gcloud` CLI.[/i]"
     )
-    rich.print("Happy launching! 🚀\n")
 
 
 async def _add_gcp_permissions(service_account: str):
     try:
         import googleapiclient.discovery
         from google.auth import exceptions
         from google.cloud import resourcemanager_v3
@@ -600,27 +646,105 @@
         orgs = []
         prompts = []
         async for org in orgs_pager:
             orgs.append(org)
             prompts.append(f"{org.display_name} ({org.name})")
         progress.remove_task(task)
     if not orgs:
-        rich.print("[red]Error: no organizations found.[/red]")
+        rich.print(
+            "[red]Error: no organizations found.[/red]\n\nVisit https://cloud.google.com/resource-manager/docs/creating-managing-organization to learn how to set this up.\n"
+            "Please contact founders@launchflow.com if you would like help setting up your GCP organization."
+        )
         raise typer.Exit(1)
     rich.print("Select the organization you would like to connect LaunchFlow to:")
     answer = beaupy.select(prompts, return_index=True, strict=True)
     rich.print(f"[pink1]>[/pink1] {prompts[answer]}\n")
     org = orgs[answer]
     with Progress(
         SpinnerColumn(),
         TextColumn("[progress.description]{task.description}"),
     ) as progress:
         task = progress.add_task(
             f"Connecting LaunchFlow to `{org.display_name}`...", total=None
         )
+
+        # Ensures the Organization has a billing account, and prompts the user to select one if not
+        billing_service = googleapiclient.discovery.build("cloudbilling", "v1")
+        req = billing_service.organizations().billingAccounts().list(parent=org.name)
+        response = req.execute()
+        billing_accounts = response.get("billingAccounts", [])
+        if not billing_accounts:
+            rich.print(
+                f"[red]Error: No billing account attached to Org `{org.display_name}`.[/red]"
+            )
+            # First we list all the billing accounts the user has access to
+            req = billing_service.billingAccounts().list()
+            response = req.execute()
+            billing_accounts = response.get("billingAccounts", [])
+            if not billing_accounts:
+                rich.print(
+                    "[red]Error: No billing accounts found for the current Google user.[/red]\n"
+                    "Visit https://console.cloud.google.com/billing to create a billing account.\n\nPlease contact founders@launchflow.com if you need help setting up GCP billing."
+                )
+                raise typer.Exit(1)
+
+            if len(billing_accounts) == 1:
+                billing_account = billing_accounts[0]
+                answer = beaupy.confirm(
+                    f"Would you like to use the billing account `{billing_account['displayName']}`?",
+                    default_is_yes=True,
+                )
+                if not answer:
+                    rich.print(
+                        "[red]Error: No billing account selected - Exiting.[/red]\n\nPlease contact founders@launchflow.com if you need help setting up GCP billing."
+                    )
+                    raise typer.Exit(1)
+            else:
+                rich.print("Select the billing account you would like to use:")
+                prompts = [
+                    f"{ba['displayName']} ({ba['name']})" for ba in billing_accounts
+                ]
+                answer = beaupy.select(prompts, return_index=True, strict=True)
+                rich.print(f"[pink1]>[/pink1] {prompts[answer]}\n")
+                billing_account = billing_accounts[answer]
+
+            while True:
+                try:
+                    policy = (
+                        billing_service.billingAccounts()
+                        .getIamPolicy(resource=billing_account["name"])
+                        .execute()
+                    )
+                    bindings = policy.get("bindings", [])
+                    for role in ["roles/billing.user"]:
+                        bindings.append(
+                            {
+                                "role": role,
+                                "members": [f"serviceAccount:{service_account}"],
+                            }
+                        )
+                    policy["bindings"] = bindings
+                    billing_service.billingAccounts().setIamPolicy(
+                        resource=billing_account["name"], body={"policy": policy}
+                    ).execute()
+                    break
+                except HttpError as e:
+                    if e.status_code == 409:
+                        # NOTE: this can happen sometimes when a concurrent policy modification
+                        # happens, we just retry in this case after waiting a bit.
+                        await asyncio.sleep(2)
+                        continue
+                    rich.print(
+                        f"[red]Error: failed to add permissions to billing account: {e}[/red]"
+                    )
+                    typer.Exit(1)
+            progress.console.print(
+                f"[green]✓[/green] Permissions added to `{billing_account['displayName']}`."
+            )
+
         while True:
             try:
                 service = googleapiclient.discovery.build(
                     "cloudresourcemanager", "v1"
                 ).organizations()
                 get_request = service.getIamPolicy(resource=org.name)
                 policy = get_request.execute()
@@ -653,42 +777,46 @@
         progress.console.print(
             f"[green]✓[/green] Permissions added to `{org.display_name}`."
         )
         progress.remove_task(task)
 
 
 async def _connect_gcp(
-    client: LaunchFlowAsyncClient, account_id: str, service_account_email: str
+    client: LaunchFlowAsyncClient,
+    account_id: str,
+    service_account_email: str,
+    add_permissions: bool,
 ):
-    rich.print(
-        f"\n`[cyan]{service_account_email}[/cyan]` needs the following roles on your GCP organization:"
-    )
-    rich.print("- Folder Creator ([i]roles/resourcemanager.folderCreator[/i])")
-    rich.print(
-        "- Organization Viewer ([i]roles/resourcemanager.organizationViewer[/i])"
-    )
-    rich.print("- Billing Account User ([i]roles/billing.user[/i])\n")
+    if add_permissions:
+        rich.print(
+            f"\n`[cyan]{service_account_email}[/cyan]` needs the following roles on your GCP organization:"
+        )
+        rich.print("- Folder Creator ([i]roles/resourcemanager.folderCreator[/i])")
+        rich.print(
+            "- Organization Viewer ([i]roles/resourcemanager.organizationViewer[/i])"
+        )
+        rich.print("- Billing Account User ([i]roles/billing.user[/i])\n")
 
-    rich.print(
-        "[i]These roles will be used to create a unique GCP project for every environment in your account.[/i]\n"
-    )
+        rich.print(
+            "[i]These roles will be used to create a unique GCP project for every environment in your account.[/i]\n"
+        )
 
-    rich.print("How would you like to add these roles?")
-    options = [
-        "Have LaunchFlow add them using my local credentials",
-        "Manually add these roles via the GCP console",
-    ]
-    answer = beaupy.select(options, strict=True, return_index=True)
-    rich.print(f"[pink1]>[/pink1] {options[answer]}")
-    if answer == 0:
-        rich.print("Verifying local GCP setup...")
-        _setup_local_gcp_env(ask=False)
-        await _add_gcp_permissions(service_account_email)
-    else:
-        _ = Prompt.ask("Hit enter once complete and we will verify your setup")
+        rich.print("How would you like to add these roles?")
+        options = [
+            "Have LaunchFlow add them using my local credentials",
+            "Manually add these roles via the GCP console",
+        ]
+        answer = beaupy.select(options, strict=True, return_index=True)
+        rich.print(f"[pink1]>[/pink1] {options[answer]}")
+        if answer == 0:
+            rich.print("Verifying local GCP setup...")
+            _setup_local_gcp_env(ask=False)
+            await _add_gcp_permissions(service_account_email)
+        else:
+            _ = Prompt.ask("Hit enter once complete and we will verify your setup")
     # polls for a successful connection for up to 60 seconds
     start_time = time.time()
     with Progress(
         SpinnerColumn(),
         TextColumn("[progress.description]{task.description}"),
     ) as progress:
         task = progress.add_task(
@@ -696,23 +824,47 @@
         )
 
         done = False
         while not done:
             try:
                 await client.connect.connect_gcp(account_id=account_id)
                 done = True
-            except LaunchFlowRequestFailure:
+            except LaunchFlowRequestFailure as e:
+                if e.status_code == 409:
+                    progress.remove_task(task)
+                    rich.print(
+                        f"[red]Error: GCP verification failed: {e}[/red]\n\nPlease contact founders@launchflow.com if you need help connecting your account to GCP."
+                    )
+                    raise typer.Exit(1)
+                elif e.status_code == 422:
+                    progress.remove_task(task)
+                    rich.print(f"[red]Error: GCP verification failed: {e}[/red]")
+                    # ask if they'd like to retry
+                    retry = beaupy.confirm(
+                        "Would you like us to add the permissions and retry the connection?",
+                        default_is_yes=True,
+                    )
+                    if retry:
+                        progress.stop()
+                        await _connect_gcp(
+                            client,
+                            account_id,
+                            service_account_email,
+                            add_permissions=True,
+                        )
+                        return
+                    else:
+                        raise typer.Exit(1)
                 if time.time() - start_time > 60:
                     raise TimeoutError(
                         "GCP setup verification timed out. Please try again."
                     )
             await asyncio.sleep(3)
 
         progress.remove_task(task)
 
     rich.print("[bold]GCP successfully connected[/bold] 🚀\n")
 
-    if answer == 1:
-        _setup_local_gcp_env()
+    _setup_local_gcp_env()
     rich.print(
         "[i]You can now create environments and deploy resources to your GCP account using LaunchFlow.[/i]"
     )
```

### Comparing `launchflow-0.3.9.dev8/launchflow/flows/project_flows.py` & `launchflow-0.4.0.dev0/launchflow/flows/project_flows.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 from typing import Optional
 
 import beaupy
 import rich
-from launchflow.clients.response_schemas import OperationStatus, ProjectResponse
-from launchflow.exceptions import LaunchFlowOperationFailure, LaunchFlowRequestFailure
-from launchflow.flows.account_id import get_account_id_from_config
-from launchflow.flows.cloud_provider import select_cloud_provider
-from launchflow.operations import AsyncOp
 from rich.progress import Progress, SpinnerColumn, TextColumn
 
 from launchflow.clients import LaunchFlowAsyncClient
+from launchflow.clients.response_schemas import ProjectResponse
+from launchflow.exceptions import LaunchFlowRequestFailure
+from launchflow.flows.account_id import get_account_id_from_config
 
 
 async def get_project(
     client: LaunchFlowAsyncClient,
     project_name: Optional[str],
     prompt_for_creation: bool = False,
     include_non_ready: bool = False,
@@ -64,39 +62,29 @@
     project_name: Optional[str] = None,
     account_id: Optional[str] = None,
 ):
     if project_name is None:
         project_name = beaupy.prompt("Enter a project name:")
         rich.print(f"[pink1]>[/pink1] {project_name}")
     print()
-    print("Select a cloud provider for your project: (Azure coming soon)")
-    cloud_provider = select_cloud_provider()
 
     account_id = await get_account_id_from_config(client, account_id)
-    print()
     project = None
     with Progress(
         SpinnerColumn(),
         TextColumn("[progress.description]{task.description}"),
     ) as progress:
         task = progress.add_task("Creating LaunchFlow Project...", total=None)
         try:
-
-            async def create_op():
-                return await client.projects.create(
-                    project_name, cloud_provider.value.lower(), account_id
-                )
-
-            op = AsyncOp(operation_id=None, client=client, _op=create_op)
-            status = await op.result()
-            project = await client.projects.get(project_name)
-            if status != OperationStatus.SUCCESS:
-                raise LaunchFlowOperationFailure(project.status_message)
-
+            project = await client.projects.create(project_name, account_id)
         except Exception as e:
             progress.console.print("[red]✗[/red] Failed to create project.")
+            progress.console.print(
+                "    └── Run this command again to retry creating the project."
+            )
+            progress.console.print(f"    └── {str(e)}")
             raise e
         finally:
             progress.update(task, advance=1)
             progress.remove_task(task)
     progress.console.print("[green]✓[/green] Project created successfully.")
     return project
```

### Comparing `launchflow-0.3.9.dev8/launchflow/gcp/cloudsql.py` & `launchflow-0.4.0.dev0/launchflow/gcp/cloudsql.py`

 * *Files 26% similar despite different names*

```diff
@@ -35,71 +35,98 @@
     DeclarativeBase = None
     sessionmaker = None
 
 # Importing the required modules
 
 import enum
 
-from launchflow.resource import Resource
 from pydantic import BaseModel
 
+from launchflow.gcp.resource import GCPResource
+from launchflow.generic_clients import PostgresClient
+
 
 # Connection information model
 class CloudSQLPostgresConnectionInfo(BaseModel):
     connection_name: str
     user: str
     password: str
     database_name: str
     public_ip_address: str
     private_ip_address: str
     public_ip_enabled: bool
 
 
+# TODO: Add Enums and other input types to generated docs.
+# Punting for now since it goes to the top of the docs page - we need an option to
+# have it go to the bottom.
 class PostgresVersion(enum.Enum):
     POSTGRES_15 = "POSTGRES_15"
     POSTGRES_14 = "POSTGRES_14"
     POSTGRES_13 = "POSTGRES_13"
     POSTGRES_12 = "POSTGRES_12"
     POSTGRES_11 = "POSTGRES_11"
     POSTGRES_10 = "POSTGRES_10"
     POSTGRES_9_6 = "POSTGRES_9_6"
 
 
-class CloudSQLPostgres(Resource[CloudSQLPostgresConnectionInfo]):
-    """A Cloud SQL Postgres resource.
-
-    Args:
-    - `name`: The name of the Cloud SQL Postgres instance.
-
-    Attributes:
-    - `connection_name`: The connection name of the Cloud SQL Postgres instance. This is available after the resource is created.
+class CloudSQLPostgres(GCPResource[CloudSQLPostgresConnectionInfo], PostgresClient):
+    """A Postgres cluster running on Google Cloud SQL.
 
-    Example usage:
+    **Example usage:**
     ```python
+    from sqlalchemy import text
     import launchflow as lf
 
-    db = lf.gcp.CloudSQLPostgres("my-pg-db")
+    postgres = lf.gcp.CloudSQLPostgres("my-pg-db")
+
+    # Quick utilities for connecting to SQLAlchemy, Django, and other ORMs
+    engine = postgres.sqlalchemy_engine()
+
+    with engine.connect() as connection:
+        print(connection.execute(text("SELECT 1")).fetchone())  # prints (1,)
     ```
     """
 
     def __init__(
         self,
         name: str,
         *,
         postgres_version: PostgresVersion = PostgresVersion.POSTGRES_15,
     ) -> None:
+        """Create a new Cloud SQL Postgres resource.
+
+        **Args**:
+        - `name`: The name of the Cloud SQL Postgres instance.
+        - `postgres_version`: The version of Postgres to use. Defaults to `PostgresVersion.POSTGRES_15`.
+        """
         super().__init__(
             name=name,
             product_name="gcp_sql_postgres",
             create_args={
                 "postgres_version": postgres_version.value,
             },
         )
 
     def django_settings(self):
+        """Returns a Django settings dictionary for connecting to the Cloud SQL Postgres instance.
+
+        **Example usage:**
+        ```python
+        import launchflow as lf
+
+        postgres = lf.gcp.CloudSQLPostgres("my-pg-db")
+
+        # settings.py
+        DATABASES = {
+            # Connect Django's ORM to the Cloud SQL Postgres instance
+            "default": postgres.django_settings(),
+        }
+        ```
+        """
         if psycopg2 is None:
             raise ImportError(
                 "psycopg2 is not installed. Please install it with `pip install psycopg2`."
             )
 
         connection_info = self.connect()
 
@@ -185,20 +212,25 @@
 
         Args:
         - `ip_type`: The IP type to use for the connection. If not provided will default to the most permisive IP address.
             For example if your Cloud SQL instance is provisioned with a public IP address, the default will be `IPTypes.PUBLIC`.
             Otherwise it will default to `IPTypes.PRIVATE`.
         - `**engine_kwargs`: Additional keyword arguments to pass to `sqlalchemy.create_engine`.
 
-        Example usage:
+        **Example usage:**
         ```python
         import launchflow as lf
 
-        db = lf.gcp.CloudSQLPostgres("my-pg-db")
-        engine = db.sqlalchemy_engine()
+        postgres = lf.gcp.CloudSQLPostgres("my-pg-db")
+
+        # Creates a SQLAlchemy engine for connecting to the Cloud SQL Postgres instance
+        engine = postgres.sqlalchemy_engine()
+
+        with engine.connect() as connection:
+            print(connection.execute("SELECT 1").fetchone())  # prints (1,)
         ```
         """
         if create_engine is None:
             raise ImportError(
                 "SQLAlchemy is not installed. Please install it with "
                 "`pip install sqlalchemy`."
             )
@@ -212,20 +244,26 @@
         """Returns an async SQLAlchemy engine for connecting to the Cloud SQL Postgres instance.
 
         Args:
         - `ip_type`: The IP type to use for the connection. If not provided will default to the most permisive IP address.
             For example if your Cloud SQL instance is provisioned with a public IP address, the default will be `IPTypes.PUBLIC`.
             Otherwise it will default to `IPTypes.PRIVATE`.        - `**engine_kwargs`: Additional keyword arguments to pass to `create_async_engine`.
 
-        Example usage:
+        **Example usage:**
         ```python
         import launchflow as lf
 
-        db = lf.gcp.CloudSQLPostgres("my-pg-db")
-        engine = await db.sqlalchemy_async_engine()
+        postgres = lf.gcp.CloudSQLPostgres("my-pg-db")
+
+        # Creates an async SQLAlchemy engine for connecting to the Cloud SQL Postgres instance
+        engine = await postgres.sqlalchemy_async_engine()
+
+        async with engine.begin() as connection:
+            result = await connection.execute("SELECT 1")
+            print(await result.fetchone())
         ```
         """
         if create_async_engine is None:
             raise ImportError(
                 "SQLAlchemy asyncio extension is not installed. "
                 "Please install it with `pip install sqlalchemy[asyncio]`."
             )
```

### Comparing `launchflow-0.3.9.dev8/launchflow/gcp/gcs.py` & `launchflow-0.4.0.dev0/launchflow/gcp/gcs.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,43 +1,53 @@
 import io
 from typing import IO
 
+from launchflow.gcp_clients import get_storage_client
+
 try:
     from google.cloud import storage
 except ImportError:
     storage = None
 
 
 from typing import Union
 
-from launchflow.resource import Resource
 from pydantic import BaseModel
 
+from launchflow.gcp.resource import GCPResource
+
 
 class GCSBucketConnectionInfo(BaseModel):
     bucket_name: str
 
 
-class GCSBucket(Resource[GCSBucketConnectionInfo]):
-    """A GCS Bucket resource.
+class GCSBucket(GCPResource[GCSBucketConnectionInfo]):
+    """A storage bucket in Google Cloud Storage.
 
-    **Attributes**:
-    - `name` (str): The name of the bucket. This must be globally unique.
-    - `location` (str): The location of the bucket. Defaults to "US".
-
-    Example usage:
+    **Example usage:**
     ```python
     import launchflow as lf
 
-    bucket = lf.gcp.GCSBucket("my-bucket")
+    gcs = lf.gcp.GCSBucket("my-bucket")
+
+    # Quick utilities for reading and writing file contents
+    gcs.upload_from_string("file contents", "path/in/gcs/file.txt")
+
+    # You can also use the google-cloud-storage library directly
+    bucket = gcs.bucket()
     bucket.blob("my-file").upload_from_filename("my-file")
     ```
     """
 
     def __init__(self, name: str, *, location="US") -> None:
+        """Create a new GCS Bucket resource.
+
+        **Args**:
+        - `name` (str): The name of the bucket. This must be globally unique.
+        """
         super().__init__(
             name=name,
             product_name="gcp_storage_bucket",
             create_args={"location": location},
         )
         # public metadata
         self.location = location
@@ -50,24 +60,27 @@
         """
         if storage is None:
             raise ImportError(
                 "google-cloud-storage not found. "
                 "You can install it with pip install launchflow[gcp]"
             )
         connection_info = self.connect()
-        return storage.Client().get_bucket(connection_info.bucket_name)
+        # TODO: Add project_id to connection_info and pass it to the client.
+        # Once this is added, add a client() method to GCPResource that returns the
+        # client setup with the project_id
+        return get_storage_client().get_bucket(connection_info.bucket_name)
 
     def upload_file(self, to_upload: Union[str, IO], bucket_path: str):
         """Uploads a file to the GCS bucket.
 
         Args:
         - `to_upload` (Union[str, IO]): The file to upload. This can be a string representing the path to the file, or a file-like object.
         - `bucket_path` (str): The path to upload the file to in the bucket.
 
-        Example usage:
+        **Example usage:**
 
         ```python
         import launchflow as lf
 
         bucket = lf.gcp.GCSBucket("my-bucket")
         bucket.upload_file("my-file.txt", "my-file.txt")
         bucket.upload_file(open("my-file.txt", "r"), "my-file.txt")
@@ -82,15 +95,15 @@
     def upload_from_string(self, to_upload: str, bucket_path: str):
         """Uploads a string to the GCS bucket.
 
         Args:
         - `to_upload` (str): The string to upload.
         - `bucket_path` (str): The path to upload the string to in the bucket.
 
-        Example usage:
+        **Example usage:**
         ```python
         import launchflow as lf
 
         bucket = lf.gcp.GCSBucket("my-bucket")
         bucket.upload_from_string("hello", "hello.txt")
         ```
         """
@@ -99,15 +112,15 @@
 
     def download_file(self, bucket_path: str):
         """Downloads a file from the GCS bucket.
 
         Args:
         - `bucket_path` (str): The path to the file in the bucket.
 
-        Example usage:
+        **Example usage:**
         ```python
         import launchflow as lf
 
         bucket = lf.gcp.GCSBucket("my-bucket")
         with open("my-file.txt", "w") as f:
             f.write(bucket.download_file("my-file.txt"))
         ```
```

### Comparing `launchflow-0.3.9.dev8/launchflow/gcp/utils.py` & `launchflow-0.4.0.dev0/launchflow/gcp/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 from typing import Optional
 
 import requests
 from google.auth import default, impersonated_credentials
-from launchflow.context import ctx
+
+from launchflow.context import LaunchFlowContext
 
 _ProjectIdMetadataKey = "project/project-id"
 _ProjectNumberMetadataKey = "project/numeric-project-id"
 _RegionMetadataKey = "instance/region"
 _InstanceIdMetadataKey = "instance/id"
 _ServiceAccountEmailMetadataKey = "instance/service-accounts/default/email"
 _ServiceAccountTokenMetadataKey = "instance/service-accounts/default/token"
@@ -39,23 +40,23 @@
 def get_service_account_credentials(
     project_name: Optional[str] = None,
     environment_name: Optional[str] = None,
 ) -> str:
     """
     Get the GCP service account credentials for the specified project and environment.
     """
-
+    context = LaunchFlowContext()
     if _is_running_on_cloud_run():
         # If running on Cloud Run, fetch the service account from the metadata server
         gcp_service_account_email = _get_cloud_run_metadata(
             _ServiceAccountEmailMetadataKey
         )
     else:
         # If not on Cloud Run, fetch the GCP service account email from LaunchFlow
-        gcp_service_account_email = ctx.get_gcp_service_account_email(
+        gcp_service_account_email = context.get_gcp_service_account_email(
             project_name, environment_name
         )
 
     # Load the default credentials (from environment, compute engine, etc.)
     creds, _ = default()
     # Define the target service account to impersonate
     target_scopes = ["https://www.googleapis.com/auth/cloud-platform"]
```

### Comparing `launchflow-0.3.9.dev8/pyproject.toml` & `launchflow-0.4.0.dev0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 [project]
 name = "launchflow"
-version = "0.3.9.dev8"
+version = "0.4.0.dev0"
 description = "Python-native infrastructure for the cloud: LaunchFlow provides a Python SDK that automatically creates and connects to production-ready infrastructure (such as Postgres, Redis, etc..) in your own cloud account. LaunchFlow completely removes the need for DevOps allowing you to focus on your application logic."
 authors = [
     { name = "CalebTVanDyke", email = "caleb@launchflow.com" },
     { name = "Josh Tanke", email = "josh@launchflow.com" },
+    { name = "Michael Noronha", email = "michael@launchflow.com" },
 ]
 readme = "README.md"
 license = { file = "LICENSE" }
 classifiers = ["Operating System :: OS Independent"]
 dependencies = [
     "beaupy",
     "rich",
@@ -21,30 +22,40 @@
     "requests",
     "s3fs",
     "gcsfs",
     "fsspec",
     "httpx",
     "uvloop",
     "Jinja2",
+    "docker",
 ]
 requires-python = ">=3.8"
 
+# TODO these are underspecified, e.g. google.cloud.billing is not there
 [project.optional-dependencies]
 gcp = [
     "cloud-sql-python-connector",
     "google-cloud-storage",
     "google-cloud-resource-manager",
     "google-api-python-client",
+    "google-cloud-bigquery",
+    "google-cloud-secret-manager",
+    "google-cloud-pubsub",
+    "google-cloud-billing",
+    "google-cloud-compute",
 ]
 aws = ["boto3"]
 dev = [
     "pytest>=7.4.4",
     "pytest-asyncio",
     "sqlalchemy[asyncio]>=2.0.27",
     "pytest-httpx",
+    "boto3-stubs[secretsmanager]",
+    "freezegun",
+    "moto",
 ]
 
 [project.scripts]
 launchflow = "launchflow.cli.main:app"
 lf = "launchflow.cli.main:app"
 
 [build-system]
```

